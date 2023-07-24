# Comparing `tmp/NASTI-0.1.2.tar.gz` & `tmp/nasti-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NASTI-0.1.2.tar", last modified: Sun Jul 23 18:25:25 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `NASTI-0.1.2.tar` & `nasti-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,46 @@
-drwxr-xr-x   0 adamdrew  (1000) adamdrew  (1000)        0 2023-07-23 18:25:25.386651 NASTI-0.1.2/
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)    35149 2023-07-23 17:23:07.000000 NASTI-0.1.2/LICENSE
-drwxr-xr-x   0 adamdrew  (1000) adamdrew  (1000)        0 2023-07-23 18:25:25.385651 NASTI-0.1.2/NASTI.egg-info/
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     7237 2023-07-23 18:25:25.000000 NASTI-0.1.2/NASTI.egg-info/PKG-INFO
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)      490 2023-07-23 18:25:25.000000 NASTI-0.1.2/NASTI.egg-info/SOURCES.txt
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)        1 2023-07-23 18:25:25.000000 NASTI-0.1.2/NASTI.egg-info/dependency_links.txt
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)       40 2023-07-23 18:25:25.000000 NASTI-0.1.2/NASTI.egg-info/entry_points.txt
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)       12 2023-07-23 18:25:25.000000 NASTI-0.1.2/NASTI.egg-info/top_level.txt
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     7237 2023-07-23 18:25:25.386651 NASTI-0.1.2/PKG-INFO
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     6772 2023-07-23 17:17:03.000000 NASTI-0.1.2/README.md
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)       39 2023-07-23 18:24:48.000000 NASTI-0.1.2/entry_points.txt
-drwxr-xr-x   0 adamdrew  (1000) adamdrew  (1000)        0 2023-07-23 18:25:25.386651 NASTI-0.1.2/nasti/
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)        0 2023-07-22 16:17:53.000000 NASTI-0.1.2/nasti/__init__.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1256 2023-07-23 12:54:01.000000 NASTI-0.1.2/nasti/cli.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1048 2023-07-23 15:52:01.000000 NASTI-0.1.2/nasti/exceptions.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     4272 2023-07-23 16:09:18.000000 NASTI-0.1.2/nasti/mutation.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     3043 2023-07-23 12:55:39.000000 NASTI-0.1.2/nasti/nasti.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     2583 2023-07-23 15:49:29.000000 NASTI-0.1.2/nasti/nastifile.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     3200 2023-07-23 15:42:52.000000 NASTI-0.1.2/nasti/source_handlers.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1940 2023-07-23 15:32:28.000000 NASTI-0.1.2/nasti/validation.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)      105 2023-07-23 18:23:16.000000 NASTI-0.1.2/pyproject.toml
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)      592 2023-07-23 18:25:25.387651 NASTI-0.1.2/setup.cfg
-drwxr-xr-x   0 adamdrew  (1000) adamdrew  (1000)        0 2023-07-23 18:25:25.386651 NASTI-0.1.2/tests/
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)      335 2023-07-23 13:21:15.000000 NASTI-0.1.2/tests/__init__.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1330 2023-07-23 16:12:36.000000 NASTI-0.1.2/tests/mocks.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     4908 2023-07-23 16:17:51.000000 NASTI-0.1.2/tests/test_mutation.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1726 2023-07-23 15:49:17.000000 NASTI-0.1.2/tests/test_nastifile.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     2660 2023-07-23 15:43:52.000000 NASTI-0.1.2/tests/test_source_handlers.py
--rw-r--r--   0 adamdrew  (1000) adamdrew  (1000)     1505 2023-07-23 15:34:43.000000 NASTI-0.1.2/tests/test_validation.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 nasti-0.1.3/Makefile
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nasti-0.1.3/Pipfile
+-rw-r--r--   0        0        0    28335 2020-02-02 00:00:00.000000 nasti-0.1.3/Pipfile.lock
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nasti-0.1.3/entry_points.txt
+-rw-r--r--   0        0        0    70731 2020-02-02 00:00:00.000000 nasti-0.1.3/logo.png
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nasti-0.1.3/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nasti-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/cli.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/exceptions.py
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/mutation.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/nasti.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/nastifile.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/source_handlers.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/validation.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/mocks.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_mutation.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_nastifile.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_source_handlers.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_validation.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/bad_yaml/nasti.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_empty_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/test.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_files_dont_exist/nasti.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_misconfigured_validation/nasti.yaml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_no_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_run/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_text_replacement_fails/nasti.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_text_replacement_fails/test.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unknown_keys/nasti.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/nasti.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/.dontsearch
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/ref.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/unmentioned
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/nested/searchbutnotfind
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/nested/unmentioned
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/no_mutations/nasti.yaml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/valid/nasti.yaml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nasti-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nasti-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 nasti-0.1.3/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nasti-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 nasti-0.1.3/PKG-INFO
```

### Comparing `NASTI-0.1.2/LICENSE` & `nasti-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/NASTI.egg-info/PKG-INFO` & `nasti-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: NASTI
-Version: 0.1.2
+Version: 0.1.3
 Summary: NASTI is Not A Starndard Templating Implementation
-Home-page: https://github.com/adamrdrew/nasti
-Author: Adam Drew
-Author-email: adamrdrew@live.com
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/adamrdrew/nasti
+Project-URL: Bug Tracker, https://github.com/adamrdrew/nasti/issues
+Author-email: Adam Drew <adamrdrew@live.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Build Status](https://github.com/adamrdrew/nasti/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/adamrdrew/nasti/actions)
 [![codecov](https://codecov.io/gh/adamrdrew/nasti/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/adamrdrew/nasti?branch=master)
 
+ <center><img src="logo.png"></center>
+
 # NASTI
 NASTI is A Strange Templating Implementation.
 
 
 NASTI allows you to create project templates, similar to tools like [Cookiecutter](https://github.com/cookiecutter/cookiecutter). What makes NASTI unique is that your project templates remain as valid, living code. You can run, test, and debug your project templates just like any other application while still enabling end users to bootstrap new projects from your template.
 
 ## Features
 * Templates remain valid source code you can run, build, etc
 * No opinionated project or directory structure
 * Works with any language
 * Tightly scoped single-file template definition
 * Powerful template and project validation system
 * Super easy, barely an inconvenience
 
+## Installation
+```sh
+$ pip install NASTI
+```
+
 ## Usage
 
 ```sh
 # Process a template on github
 $ nasti process git@github.com:somedev/some-template.git
 # Or gitlab, or any other git repo you can clone
 $ nasti process git@gitlab.mycomand.com:someorg/some-template.git
@@ -88,14 +95,27 @@
 
 $ nasti validate 
 Error: Invalid mutation config: {'name': 'quay', 'help': 'The quay repo is the location of your container image. Should be in the form of quay.io/username/repo', 'replace': 'quay.io/someorg/some-project', 'files': ['Makefile'], 'validations': ['^quay\\.io/[a-zA-Z0-9_-]+/[a-zA-Z0-9_-]+$']} missing 'prompt'
 ```
 
 You can easily build out your nastifile by adding or updating mutations, validating, and fixing what doesn't work. It also makes a good fit for an automated PR check in your repo.
 
+### Find Files Matching a Mutation
+Mutations are file-scoped, meaning they'll only replace text in files in the mutation's file list. But what if you aren't sure whether you have the file list complete? Maybe the text you want to replace is in a file you forgot to add to the file list. The `find` command solves this problem by finding all files that contain your mutation replacement text but aren't in your mutation file lists:
+
+```
+$ nasti find tests/nastifiles/mutation_unmentioned_files/
+The following mutations match files not listed in the nastifile:
+
+Mutation example_mutation matches but does not reference:
+    files/nested/unmentioned    files/unmentioned
+```
+
+In the example above the nastifile has a mutation called `example_mutation` that would match the files `files/nested/unmentioned` and `files/unmentioned` but those files don't appear in the `example_mutation` file list.
+
 ### Validation Kinds
 As shown above you can create any custom validation regex you want, but for common tasks we ship a bunch of prebuilt validations thanks to the excellent [Validators](https://github.com/python-validators/validators) library.
 
 Here's an example:
 ```yaml
 ---
 mutations:
@@ -117,14 +137,40 @@
     "ip_address":   validators.ip_address,
     "slug":         validators.slug,
     "url":          validators.url,
     "uuid":         validators.uuid,
 }
 ```
 
+## Development
+
+### Dependency Management & Virtual Environment
+This project uses [pipenv](https://github.com/pypa/pipenv) to manage dependencies and the virtual environment. You'll want to make sure you have pipenv installed. Then after you pull down the NASTI code run `pipenv install`. You can then enter the virtual environment and get to hacking with `pipenv shell`.
+
+### Running from Source
+If you are hacking on the app and you want to run the version you have in the source tree enter the venv with `pipenv shell` and then run the app directly:
+
+```
+$ python nasti.py [COMMANDS] [OPTIONS]
+```
+
+Even if you have NASTI installed as a command on your machine globally this should run the version in the source tree.
+
+### Tests & Code Coverage
+You can run tests with `make test` and generate a codecoverage report with `make coverage`. PRs are very, very much welcome but please make sure anything you introduce or refactor passes tests and includes new tests if required.
+
+### Building & Publishing
+I barely understand Python packaging publishing. Describing it as a complex mess would be an understatement. I think I have it working as simply as possible, but I had to do so much trial and error I don't know whether what seems to work on my machine will work on someone else's. Help very much welcome on this!
+
+1. Exit the venv if you are in it
+2. Bump the version in `setup.cfg`
+2. Install build deps with `make install-build-deps`
+3. Build `make build-app`
+4. Publish `make publish`
+
 ## Project Justification
 Do we really need another project template system? And if we do, do we really want one this weird?
 
 A cookiecutter template contains a bunch of source files that have bits of text stripped out and replaced with jinja template syntax along with a JSON config file that contains the prompts, default values, and more. It is a great system and many projects use it. However, for some use cases it has a fatal flaw. Once the project has been converted to a template it is no longer valid source code. You can't run, debug, test, build, or develop on it without a complex and error prone process.
 
 NASTI attempts to solve this problem by flipping the concept of a template on its head. The source files are left as is, to be worked with as normal and no specific directory structure is mandated. All NASTI requires is a file called `nasti.yaml`, in your project's root directory. The nastifile defines a set of mutations. Each mutation defines a text string to be replaced, a list of files that text string occurs in, and some extras like prompts and validations. NASTI clones or copies the nastified™️ project, applies the mutations, and the result is a brand new project ready to build on.
```

### Comparing `NASTI-0.1.2/PKG-INFO` & `nasti-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: NASTI
-Version: 0.1.2
-Summary: NASTI is Not A Starndard Templating Implementation
-Home-page: https://github.com/adamrdrew/nasti
-Author: Adam Drew
-Author-email: adamrdrew@live.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://github.com/adamrdrew/nasti/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/adamrdrew/nasti/actions)
 [![codecov](https://codecov.io/gh/adamrdrew/nasti/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/adamrdrew/nasti?branch=master)
 
+ <center><img src="logo.png"></center>
+
 # NASTI
 NASTI is A Strange Templating Implementation.
 
 
 NASTI allows you to create project templates, similar to tools like [Cookiecutter](https://github.com/cookiecutter/cookiecutter). What makes NASTI unique is that your project templates remain as valid, living code. You can run, test, and debug your project templates just like any other application while still enabling end users to bootstrap new projects from your template.
 
 ## Features
 * Templates remain valid source code you can run, build, etc
 * No opinionated project or directory structure
 * Works with any language
 * Tightly scoped single-file template definition
 * Powerful template and project validation system
 * Super easy, barely an inconvenience
 
+## Installation
+```sh
+$ pip install NASTI
+```
+
 ## Usage
 
 ```sh
 # Process a template on github
 $ nasti process git@github.com:somedev/some-template.git
 # Or gitlab, or any other git repo you can clone
 $ nasti process git@gitlab.mycomand.com:someorg/some-template.git
@@ -88,14 +81,27 @@
 
 $ nasti validate 
 Error: Invalid mutation config: {'name': 'quay', 'help': 'The quay repo is the location of your container image. Should be in the form of quay.io/username/repo', 'replace': 'quay.io/someorg/some-project', 'files': ['Makefile'], 'validations': ['^quay\\.io/[a-zA-Z0-9_-]+/[a-zA-Z0-9_-]+$']} missing 'prompt'
 ```
 
 You can easily build out your nastifile by adding or updating mutations, validating, and fixing what doesn't work. It also makes a good fit for an automated PR check in your repo.
 
+### Find Files Matching a Mutation
+Mutations are file-scoped, meaning they'll only replace text in files in the mutation's file list. But what if you aren't sure whether you have the file list complete? Maybe the text you want to replace is in a file you forgot to add to the file list. The `find` command solves this problem by finding all files that contain your mutation replacement text but aren't in your mutation file lists:
+
+```
+$ nasti find tests/nastifiles/mutation_unmentioned_files/
+The following mutations match files not listed in the nastifile:
+
+Mutation example_mutation matches but does not reference:
+    files/nested/unmentioned    files/unmentioned
+```
+
+In the example above the nastifile has a mutation called `example_mutation` that would match the files `files/nested/unmentioned` and `files/unmentioned` but those files don't appear in the `example_mutation` file list.
+
 ### Validation Kinds
 As shown above you can create any custom validation regex you want, but for common tasks we ship a bunch of prebuilt validations thanks to the excellent [Validators](https://github.com/python-validators/validators) library.
 
 Here's an example:
 ```yaml
 ---
 mutations:
@@ -117,14 +123,40 @@
     "ip_address":   validators.ip_address,
     "slug":         validators.slug,
     "url":          validators.url,
     "uuid":         validators.uuid,
 }
 ```
 
+## Development
+
+### Dependency Management & Virtual Environment
+This project uses [pipenv](https://github.com/pypa/pipenv) to manage dependencies and the virtual environment. You'll want to make sure you have pipenv installed. Then after you pull down the NASTI code run `pipenv install`. You can then enter the virtual environment and get to hacking with `pipenv shell`.
+
+### Running from Source
+If you are hacking on the app and you want to run the version you have in the source tree enter the venv with `pipenv shell` and then run the app directly:
+
+```
+$ python nasti.py [COMMANDS] [OPTIONS]
+```
+
+Even if you have NASTI installed as a command on your machine globally this should run the version in the source tree.
+
+### Tests & Code Coverage
+You can run tests with `make test` and generate a codecoverage report with `make coverage`. PRs are very, very much welcome but please make sure anything you introduce or refactor passes tests and includes new tests if required.
+
+### Building & Publishing
+I barely understand Python packaging publishing. Describing it as a complex mess would be an understatement. I think I have it working as simply as possible, but I had to do so much trial and error I don't know whether what seems to work on my machine will work on someone else's. Help very much welcome on this!
+
+1. Exit the venv if you are in it
+2. Bump the version in `setup.cfg`
+2. Install build deps with `make install-build-deps`
+3. Build `make build-app`
+4. Publish `make publish`
+
 ## Project Justification
 Do we really need another project template system? And if we do, do we really want one this weird?
 
 A cookiecutter template contains a bunch of source files that have bits of text stripped out and replaced with jinja template syntax along with a JSON config file that contains the prompts, default values, and more. It is a great system and many projects use it. However, for some use cases it has a fatal flaw. Once the project has been converted to a template it is no longer valid source code. You can't run, debug, test, build, or develop on it without a complex and error prone process.
 
 NASTI attempts to solve this problem by flipping the concept of a template on its head. The source files are left as is, to be worked with as normal and no specific directory structure is mandated. All NASTI requires is a file called `nasti.yaml`, in your project's root directory. The nastifile defines a set of mutations. Each mutation defines a text string to be replaced, a list of files that text string occurs in, and some extras like prompts and validations. NASTI clones or copies the nastified™️ project, applies the mutations, and the result is a brand new project ready to build on.
```

### Comparing `NASTI-0.1.2/nasti/cli.py` & `nasti-0.1.3/nasti/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,9 +47,27 @@
         })
         nasti_file.validate()
         click.echo("Nastifile is valid.")
     except Exception as e:
         print(e)
         sys.exit(1)
 
+@click.command()
+@click.argument("path", required=False)
+def find(path):
+    if not path:
+        path = "."
+    try:
+        nasti_file = NastiFile({
+            "path": path,
+            "os_dep": os,
+            "open_dep": open,
+        })
+        unmentioned_files = nasti_file.find_unmentioned_files()
+        click.echo(unmentioned_files.get_report())
+    except Exception as e:
+        print(e)
+        sys.exit(1)
+
 cli.add_command(process)
-cli.add_command(validate)
+cli.add_command(validate)
+cli.add_command(find)
```

### Comparing `NASTI-0.1.2/nasti/exceptions.py` & `nasti-0.1.3/nasti/exceptions.py`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/nasti/nasti.py` & `nasti-0.1.3/nasti/nasti.py`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/nasti/source_handlers.py` & `nasti-0.1.3/nasti/source_handlers.py`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/nasti/validation.py` & `nasti-0.1.3/nasti/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
             self.kind = validation_config[self.KIND_KEY]
     
     def validate(self, input):
         if self.regex:
             return self.__is_valid_regex(input)
         if self.kind:
             return self.__is_valid_kind(input)
-        return False
 
     def __is_valid_regex(self, input):
         return bool(re.match(self.regex, input))
     
     def __is_valid_kind(self, input):
         return bool(self.kinds[self.kind](input))
```

### Comparing `NASTI-0.1.2/tests/mocks.py` & `nasti-0.1.3/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/tests/test_mutation.py` & `nasti-0.1.3/tests/test_mutation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,23 @@
         with open("tests/nastifiles/mutation_empty_files/nasti.yaml", "r") as f:
             config = yaml.safe_load(f)
         mutation_config = config["mutations"][0]
         mutation = Mutation(mutation_config, "tests/nastifiles/mutation_empty_files")
         with self.assertRaises(exceptions.MutationEmptyFilesException):
             mutation.validate()
 
+    def test_unmentioned_files(self):
+        #open the yaml file
+        with open("tests/nastifiles/mutation_unmentioned_files/nasti.yaml", "r") as f:
+            config = yaml.safe_load(f)
+        mutation_config = config["mutations"][0]
+        mutation = Mutation(mutation_config, "tests/nastifiles/mutation_unmentioned_files")
+        unmentioned_files = mutation.find_unmentioned_files("tests/nastifiles/mutation_unmentioned_files")
+        assert unmentioned_files == ['files/nested/unmentioned', 'files/unmentioned']
+
     # this tests that the files array is not present
     def test_no_files(self):
         #open the yaml file
         with open("tests/nastifiles/mutation_no_files/nasti.yaml", "r") as f:
             config = yaml.safe_load(f)
         mutation_config = config["mutations"][0]
         with self.assertRaises(exceptions.MutationRequiredKeysMissingException):
```

### Comparing `NASTI-0.1.2/tests/test_source_handlers.py` & `nasti-0.1.3/tests/test_source_handlers.py`

 * *Files identical despite different names*

### Comparing `NASTI-0.1.2/tests/test_validation.py` & `nasti-0.1.3/tests/test_validation.py`

 * *Files identical despite different names*

