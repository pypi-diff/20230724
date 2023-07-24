# Comparing `tmp/nasa-wildfires-1.1.0.tar.gz` & `tmp/nasa-wildfires-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasa-wildfires-1.1.0.tar", last modified: Mon May 30 12:36:36 2022, max compression
+gzip compressed data, was "nasa-wildfires-1.1.1.tar", last modified: Mon Jul 24 19:51:32 2023, max compression
```

## Comparing `nasa-wildfires-1.1.0.tar` & `nasa-wildfires-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.742764 nasa-wildfires-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.742764 nasa-wildfires-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5213 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    34746 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.766764 nasa-wildfires-1.1.0/data/
--rw-r--r--   0 runner    (1001) docker     (121)  3904659 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/data/modis.json
--rw-r--r--   0 runner    (1001) docker     (121) 16419176 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/data/viirs-noaa.json
--rw-r--r--   0 runner    (1001) docker     (121) 16221200 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/data/viirs-suomi.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.742764 nasa-wildfires-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/nasa_wildfires/
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/nasa_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/nasa_wildfires/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/nasa_wildfires/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-30 12:36:36.000000 nasa-wildfires-1.1.0/nasa_wildfires.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-30 12:36:36.782764 nasa-wildfires-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-05-30 12:35:39.000000 nasa-wildfires-1.1.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.909660 nasa-wildfires-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.913660 nasa-wildfires-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    54927 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.913660 nasa-wildfires-1.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/modis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/viirs-noaa.json
+-rw-r--r--   0 runner    (1001) docker     (123) 43384153 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/viirs-suomi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.909660 nasa-wildfires-1.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/nasa_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/test.py
```

### Comparing `nasa-wildfires-1.1.0/.github/workflows/continuous-deployment.yml` & `nasa-wildfires-1.1.1/.github/workflows/continuous-deployment.yml`

 * *Files 24% similar despite different names*

```diff
@@ -7,76 +7,110 @@
   lint-python:
     name: Lint
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
-      - name: Install pipenv
-        run: pipx install pipenv
-
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install --dev --python `which python`
 
       - id: run
         name: Run
         run: pipenv run flake8 nasa_wildfires
 
+  mypy-python:
+    name: Static-types check
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+
+      - id: setup-python
+        name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+          cache: 'pipenv'
+
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
+      - id: install-python-dependencies
+        name: Install Python dependencies
+        run: pipenv sync --dev
+        shell: bash
+
+      - id: mypy
+        name: Run mypy
+        run: pipenv run mypy ./nasa_wildfires --ignore-missing-imports --verbose
+        shell: bash
+
   test-python:
     strategy:
       matrix:
-        python: ['3.7', '3.8', '3.9', '3.10']
+        python: ['3.8', '3.9', '3.10', '3.11']
     name: Test
     runs-on: ubuntu-latest
+    needs: [lint-python, mypy-python]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
-      - name: Install pipenv
-        run: pipx install pipenv
-
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           cache: 'pipenv'
 
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install --skip-lock --python `which python`
         shell: bash
 
       - id: run
         name: Run
         run: pipenv run python test.py
-        env:
-          AIRNOW_KEYS: ${{ secrets.AIRNOW_KEYS }}
         shell: bash
 
   test-build:
     name: Build Python package
     runs-on: ubuntu-latest
     needs: [test-python]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
-      - name: Install pipenv
-        run: pipx install pipenv
-
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install --dev --python `which python`
 
       - id: build
         name: Build release
         run: |
@@ -87,33 +121,29 @@
       - id: check
         name: Check release
         run: |
             pipenv run twine check dist/*
 
       - id: save
         name: Save artifact
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: test-release-${{ github.run_number }}
           path: ./dist
           if-no-files-found: error
 
   tag-release:
     name: Tagged PyPI release
     runs-on: ubuntu-latest
     needs: [test-build]
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     steps:
-      - uses: actions/setup-python@v3
-        with:
-          python-version: '3.9'
-
       - id: fetch
         name: Fetch artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: test-release-${{ github.run_number }}
           path: ./dist
 
       - id: publish
         name: Publish release
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `nasa-wildfires-1.1.0/.github/workflows/docs.yml` & `nasa-wildfires-1.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/.github/workflows/scrape.yml` & `nasa-wildfires-1.1.1/.github/workflows/scrape.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 name: Scrape
+
 on:
   workflow_dispatch:
   schedule:
     - cron: '0 6 * * *'
 
 jobs:
   scrape:
     name: Scrape
     runs-on: ubuntu-latest
     steps:
       - id: checkout
         name: Checkout
         uses: actions/checkout@v3
 
-      - name: Install pipenv
-        run: pipx install pipenv
-
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
       - id: make
         name: Run scrape command
         run: |
           pipenv run python setup.py install
           pipenv run nasawildfires modis --indent=2 > data/modis.json
           pipenv run nasawildfires viirs-suomi --indent=2 > data/viirs-suomi.json
           pipenv run nasawildfires viirs-noaa --indent=2 > data/viirs-noaa.json
-        env:
-          AIRNOW_KEYS: ${{ secrets.AIRNOW_KEYS }}
         shell: bash
 
       - id: commit
         name: Commit results
         run: |
           git config --global user.name "github-actions[bot]"
           git config --global user.email "actions@github.com"
```

### Comparing `nasa-wildfires-1.1.0/.gitignore` & `nasa-wildfires-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/.pre-commit-config.yaml` & `nasa-wildfires-1.1.1/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
         args: ['--maxkb=10000']
     -   id: check-case-conflict
     -   id: mixed-line-ending
 
 -   repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.7.0
     hooks:
     -   id: black
 
 -   repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.15.0
     hooks:
     -   id: blacken-docs
         additional_dependencies: [black]
 
 -   repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
         args: ["--profile", "black", "--filter-files"]
 
--   repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+-   repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
     - id: flake8
 
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.9.0
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
+
+-   repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.3.0
+    hooks:
+    -   id: mypy
+        additional_dependencies:
+          - types-requests
```

### Comparing `nasa-wildfires-1.1.0/CODE_OF_CONDUCT.md` & `nasa-wildfires-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/LICENSE` & `nasa-wildfires-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/PKG-INFO` & `nasa-wildfires-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nasa-wildfires
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download wildfire hotspots detected by NASA satellites and the Fire Information for Resource Management System (FIRMS)
 Home-page: https://palewi.re/docs/nasa-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nasa-wildfires
 Project-URL: Tracker, https://github.com/datadesk/nasa-wildfires/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Links
```

### Comparing `nasa-wildfires-1.1.0/docs/Makefile` & `nasa-wildfires-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/docs/_static/css/custom.css` & `nasa-wildfires-1.1.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/docs/_templates/nav.html` & `nasa-wildfires-1.1.1/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/docs/conf.py` & `nasa-wildfires-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/docs/index.md` & `nasa-wildfires-1.1.1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,220 +8,224 @@
 00000070: 6e64 2074 6865 205b 4669 7265 2049 6e66  nd the [Fire Inf
 00000080: 6f72 6d61 7469 6f6e 2066 6f72 2052 6573  ormation for Res
 00000090: 6f75 7263 6520 4d61 6e61 6765 6d65 6e74  ource Management
 000000a0: 2053 7973 7465 6d20 2846 4952 4d53 295d   System (FIRMS)]
 000000b0: 2868 7474 7073 3a2f 2f66 6972 6d73 2e6d  (https://firms.m
 000000c0: 6f64 6170 732e 656f 7364 6973 2e6e 6173  odaps.eosdis.nas
 000000d0: 612e 676f 762f 6163 7469 7665 5f66 6972  a.gov/active_fir
-000000e0: 652f 290a 0a23 2320 496e 7374 616c 6c61  e/)..## Installa
-000000f0: 7469 6f6e 0a0a 6060 6062 6173 680a 7069  tion..```bash.pi
-00000100: 7065 6e76 2069 6e73 7461 6c6c 206e 6173  penv install nas
-00000110: 612d 7769 6c64 6669 7265 730a 6060 600a  a-wildfires.```.
-00000120: 0a23 2320 436f 6d6d 616e 642d 6c69 6e65  .## Command-line
-00000130: 2075 7361 6765 0a0a 6060 6062 6173 680a   usage..```bash.
-00000140: 5573 6167 653a 206e 6173 6177 696c 6466  Usage: nasawildf
-00000150: 6972 6573 205b 4f50 5449 4f4e 535d 2043  ires [OPTIONS] C
-00000160: 4f4d 4d41 4e44 205b 4152 4753 5d2e 2e2e  OMMAND [ARGS]...
-00000170: 0a0a 2020 4120 636f 6d6d 616e 642d 6c69  ..  A command-li
-00000180: 6e65 2069 6e74 6572 6661 6365 2066 6f72  ne interface for
-00000190: 2064 6f77 6e6c 6f61 6469 6e67 2077 696c   downloading wil
-000001a0: 6466 6972 6520 6461 7461 2066 726f 6d20  dfire data from 
-000001b0: 4e41 5341 0a20 2073 6174 656c 6c69 7465  NASA.  satellite
-000001c0: 732e 0a0a 2020 5265 7475 726e 7320 776f  s...  Returns wo
-000001d0: 726c 6420 4765 6f4a 534f 4e20 696e 2061  rld GeoJSON in a
-000001e0: 2072 6563 656e 7420 3234 2d68 6f75 7220   recent 24-hour 
-000001f0: 7065 7269 6f64 2e20 466f 7220 6176 6169  period. For avai
-00000200: 6c61 626c 6520 7265 6769 6f6e 7320 616e  lable regions an
-00000210: 6420 7469 6d65 2072 616e 6765 732c 2073  d time ranges, s
-00000220: 6565 206f 7074 696f 6e73 2e0a 0a4f 7074  ee options...Opt
-00000230: 696f 6e73 3a0a 2020 2d2d 6865 6c70 2020  ions:.  --help  
-00000240: 5368 6f77 2074 6869 7320 6d65 7373 6167  Show this messag
-00000250: 6520 616e 6420 6578 6974 2e0a 0a43 6f6d  e and exit...Com
-00000260: 6d61 6e64 733a 0a20 206d 6f64 6973 2020  mands:.  modis  
-00000270: 486f 7473 706f 7473 2064 6574 6563 7465  Hotspots detecte
-00000280: 6420 6279 2074 6865 204d 4f44 4953 2073  d by the MODIS s
-00000290: 6174 656c 6c69 7465 6c0a 2020 7669 6972  atellitel.  viir
-000002a0: 735f 7375 6f6d 6920 2048 6f74 7370 6f74  s_suomi  Hotspot
-000002b0: 7320 6465 7465 6374 6564 2062 7920 7468  s detected by th
-000002c0: 6520 5649 5252 5320 532d 4e50 5020 7361  e VIRRS S-NPP sa
-000002d0: 7465 6c6c 6974 652e 0a20 2076 6969 7273  tellite..  viirs
-000002e0: 5f6e 6f61 6120 2048 6f74 7370 6f74 7320  _noaa  Hotspots 
-000002f0: 6465 7465 6374 6564 2062 7920 7468 6520  detected by the 
-00000300: 5649 5252 5320 4e4f 4141 2d32 3020 7361  VIRRS NOAA-20 sa
-00000310: 7465 6c6c 6974 652e 0a60 6060 0a44 6f77  tellite..```.Dow
-00000320: 6e6c 6f61 6420 6120 4765 6f4a 534f 4e20  nload a GeoJSON 
-00000330: 6f66 2068 6f74 7370 6f74 7320 6465 7465  of hotspots dete
-00000340: 6374 6564 2062 7920 7468 6520 4d4f 4449  cted by the MODI
-00000350: 5320 7361 7465 6c6c 6974 6520 696e 2061  S satellite in a
-00000360: 2072 6563 656e 7420 3234 2d68 6f75 7220   recent 24-hour 
-00000370: 7065 7269 6f64 2e0a 0a60 6060 6261 7368  period...```bash
-00000380: 0a6e 6173 6177 696c 6466 6972 6573 206d  .nasawildfires m
-00000390: 6f64 6973 0a60 6060 0a0a 446f 776e 6c6f  odis.```..Downlo
-000003a0: 6164 2061 2047 656f 4a53 4f4e 206f 6620  ad a GeoJSON of 
-000003b0: 686f 7473 706f 7473 2064 6574 6563 7465  hotspots detecte
-000003c0: 6420 6279 2074 6865 204d 4f44 4953 2073  d by the MODIS s
-000003d0: 6174 656c 6c69 7465 2066 6f72 2055 5341  atellite for USA
-000003e0: 2061 6e64 2048 6177 6169 6920 696e 2061   and Hawaii in a
-000003f0: 2072 6563 656e 7420 3438 2d68 6f75 7220   recent 48-hour 
-00000400: 7065 7269 6f64 2e0a 0a60 6060 6261 7368  period...```bash
-00000410: 0a6e 6173 6177 696c 6466 6972 6573 206d  .nasawildfires m
-00000420: 6f64 6973 202d 7220 7573 612d 6861 7761  odis -r usa-hawa
-00000430: 6969 202d 7420 3438 680a 6060 600a 0a44  ii -t 48h.```..D
-00000440: 6f77 6e6c 6f61 6420 6120 4765 6f4a 534f  ownload a GeoJSO
-00000450: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
-00000460: 7465 6374 6564 2062 7920 7468 6520 5649  tected by the VI
-00000470: 4952 5320 532d 4e50 5020 7361 7465 6c6c  IRS S-NPP satell
-00000480: 6974 6520 696e 2061 2072 6563 656e 7420  ite in a recent 
-00000490: 3234 2d68 6f75 7220 7065 7269 6f64 2e0a  24-hour period..
-000004a0: 0a60 6060 6261 7368 0a6e 6173 6177 696c  .```bash.nasawil
-000004b0: 6466 6972 6573 2076 6969 7273 2d73 756f  dfires viirs-suo
-000004c0: 6d69 0a60 6060 0a0a 446f 776e 6c6f 6164  mi.```..Download
-000004d0: 2061 2047 656f 4a53 4f4e 206f 6620 686f   a GeoJSON of ho
-000004e0: 7473 706f 7473 2064 6574 6563 7465 6420  tspots detected 
-000004f0: 6279 2074 6865 2056 4949 5253 204e 4f41  by the VIIRS NOA
-00000500: 412d 3230 2073 6174 656c 6c69 7465 2069  A-20 satellite i
-00000510: 6e20 6120 7265 6365 6e74 2032 342d 686f  n a recent 24-ho
-00000520: 7572 2070 6572 696f 642e 0a0a 6060 6062  ur period...```b
-00000530: 6173 680a 6e61 7361 7769 6c64 6669 7265  ash.nasawildfire
-00000540: 7320 7669 6972 732d 6e6f 6161 0a60 6060  s viirs-noaa.```
-00000550: 0a0a 2323 2050 7974 686f 6e20 7573 6167  ..## Python usag
-00000560: 650a 0a49 6d70 6f72 7420 7468 6520 6c69  e..Import the li
-00000570: 6272 6172 792e 0a0a 6060 6070 7974 686f  brary...```pytho
-00000580: 6e0a 696d 706f 7274 206e 6173 615f 7769  n.import nasa_wi
-00000590: 6c64 6669 7265 730a 6060 600a 0a56 6965  ldfires.```..Vie
-000005a0: 7720 6c69 7374 206f 6620 6176 6169 6c61  w list of availa
-000005b0: 626c 6520 7265 6769 6f6e 730a 6060 6070  ble regions.```p
-000005c0: 7974 686f 6e0a 6e61 7361 5f77 696c 6466  ython.nasa_wildf
-000005d0: 6972 6573 2e52 4547 494f 4e5f 4c49 5354  ires.REGION_LIST
-000005e0: 0a5b 0a20 2020 2022 676c 6f62 616c 222c  .[.    "global",
-000005f0: 0a20 2020 2022 6361 6e61 6461 222c 0a20  .    "canada",. 
-00000600: 2020 2022 616c 6173 6b61 222c 0a20 2020     "alaska",.   
-00000610: 2022 7573 612d 6861 7761 6969 222c 0a20   "usa-hawaii",. 
-00000620: 2020 2022 6365 6e74 7261 6c2d 616d 6572     "central-amer
-00000630: 6963 6122 2c0a 2020 2020 2273 6f75 7468  ica",.    "south
-00000640: 2d61 6d65 7269 6361 222c 0a20 2020 2022  -america",.    "
-00000650: 6575 726f 7065 222c 0a20 2020 2022 6e6f  europe",.    "no
-00000660: 7274 682d 6365 6e74 7261 6c2d 6166 7269  rth-central-afri
-00000670: 6361 222c 0a20 2020 2022 736f 7574 6865  ca",.    "southe
-00000680: 726e 2d61 6672 6963 6122 2c0a 2020 2020  rn-africa",.    
-00000690: 2272 7573 7369 612d 6173 6961 222c 0a20  "russia-asia",. 
-000006a0: 2020 2022 736f 7574 682d 6173 6961 222c     "south-asia",
-000006b0: 0a20 2020 2022 736f 7574 6865 6173 742d  .    "southeast-
-000006c0: 6173 6961 222c 0a20 2020 2022 6175 7374  asia",.    "aust
-000006d0: 7261 6c69 612d 6e65 777a 6561 6c61 6e64  ralia-newzealand
-000006e0: 222c 0a5d 0a60 6060 0a0a 5669 6577 206c  ",.].```..View l
-000006f0: 6973 7420 6f66 2061 7661 696c 6162 6520  ist of availabe 
-00000700: 7469 6d65 2072 616e 6765 730a 6060 6070  time ranges.```p
-00000710: 7974 686f 6e0a 6e61 7361 5f77 696c 6466  ython.nasa_wildf
-00000720: 6972 6573 2e54 494d 455f 5241 4e47 455f  ires.TIME_RANGE_
-00000730: 4c49 5354 0a5b 2232 3468 222c 2022 3438  LIST.["24h", "48
-00000740: 6822 2c20 2237 6422 5d0a 6060 600a 0a44  h", "7d"].```..D
-00000750: 6f77 6e6c 6f61 6420 6120 4765 6f4a 534f  ownload a GeoJSO
-00000760: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
-00000770: 7465 6374 6564 2062 7920 7468 6520 4d4f  tected by the MO
-00000780: 4449 5320 7361 7465 6c6c 6974 6520 696e  DIS satellite in
-00000790: 2061 2072 6563 656e 7420 3234 2d68 6f75   a recent 24-hou
-000007a0: 7220 7065 7269 6f64 2e20 5265 7475 726e  r period. Return
-000007b0: 7320 4765 6f4a 534f 4e2e 0a0a 6060 6070  s GeoJSON...```p
-000007c0: 7974 686f 6e0a 6461 7461 203d 206e 6173  ython.data = nas
-000007d0: 615f 7769 6c64 6669 7265 732e 6765 745f  a_wildfires.get_
-000007e0: 6d6f 6469 7328 290a 6060 600a 0a44 6f77  modis().```..Dow
-000007f0: 6e6c 6f61 6420 6120 7265 6769 6f6e 616c  nload a regional
-00000800: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
-00000810: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
-00000820: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
-00000830: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
-00000840: 2032 342d 686f 7572 2070 6572 696f 642e   24-hour period.
-00000850: 0a0a 6060 6070 7974 686f 6e0a 6461 7461  ..```python.data
-00000860: 203d 206e 6173 615f 7769 6c64 6669 7265   = nasa_wildfire
-00000870: 732e 6765 745f 6d6f 6469 7328 7265 6769  s.get_modis(regi
-00000880: 6f6e 3d22 7573 612d 6861 7761 6969 2229  on="usa-hawaii")
-00000890: 0a60 6060 0a0a 446f 776e 6c6f 6164 2061  .```..Download a
-000008a0: 2072 6567 696f 6e61 6c20 4765 6f4a 534f   regional GeoJSO
-000008b0: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
-000008c0: 7465 6374 6564 2062 7920 7468 6520 4d4f  tected by the MO
-000008d0: 4449 5320 7361 7465 6c6c 6974 6520 696e  DIS satellite in
-000008e0: 2061 2072 6563 656e 7420 372d 6461 7920   a recent 7-day 
-000008f0: 7065 7269 6f64 2e0a 0a60 6060 7079 7468  period...```pyth
-00000900: 6f6e 0a64 6174 6120 3d20 6e61 7361 5f77  on.data = nasa_w
-00000910: 696c 6466 6972 6573 2e67 6574 5f6d 6f64  ildfires.get_mod
-00000920: 6973 2872 6567 696f 6e3d 2275 7361 2d68  is(region="usa-h
-00000930: 6177 6169 6922 2c20 7469 6d65 5f72 616e  awaii", time_ran
-00000940: 6765 3d22 3764 2229 0a60 6060 0a0a 446f  ge="7d").```..Do
-00000950: 776e 6c6f 6164 2061 2047 656f 4a53 4f4e  wnload a GeoJSON
-00000960: 206f 6620 686f 7473 706f 7473 2064 6574   of hotspots det
-00000970: 6563 7465 6420 6279 2074 6865 2056 4949  ected by the VII
-00000980: 5253 2053 2d4e 5050 2073 6174 656c 6c69  RS S-NPP satelli
-00000990: 7465 2069 6e20 6120 7265 6365 6e74 2032  te in a recent 2
-000009a0: 342d 686f 7572 2070 6572 696f 642e 2052  4-hour period. R
-000009b0: 6574 7572 6e73 2047 656f 4a53 4f4e 2e0a  eturns GeoJSON..
-000009c0: 0a60 6060 7079 7468 6f6e 0a64 6174 6120  .```python.data 
-000009d0: 3d20 6e61 7361 5f77 696c 6466 6972 6573  = nasa_wildfires
-000009e0: 2e67 6574 5f76 6969 7273 5f73 756f 6d69  .get_viirs_suomi
-000009f0: 2829 0a60 6060 0a0a 446f 776e 6c6f 6164  ().```..Download
-00000a00: 2061 2047 656f 4a53 4f4e 206f 6620 686f   a GeoJSON of ho
-00000a10: 7473 706f 7473 2064 6574 6563 7465 6420  tspots detected 
-00000a20: 6279 2074 6865 2056 4949 5253 204e 4f41  by the VIIRS NOA
-00000a30: 412d 3230 2073 6174 656c 6c69 7465 2069  A-20 satellite i
-00000a40: 6e20 6120 7265 6365 6e74 2032 342d 686f  n a recent 24-ho
-00000a50: 7572 2070 6572 696f 642e 2052 6574 7572  ur period. Retur
-00000a60: 6e73 2047 656f 4a53 4f4e 2e0a 0a60 6060  ns GeoJSON...```
-00000a70: 7079 7468 6f6e 0a64 6174 6120 3d20 6e61  python.data = na
-00000a80: 7361 5f77 696c 6466 6972 6573 2e67 6574  sa_wildfires.get
-00000a90: 5f76 6969 7273 5f6e 6f61 6128 290a 6060  _viirs_noaa().``
-00000aa0: 600a 0a23 2320 436f 6e74 7269 6275 7469  `..## Contributi
-00000ab0: 6e67 0a0a 496e 7374 616c 6c20 6465 7065  ng..Install depe
-00000ac0: 6e64 656e 6369 6573 2066 6f72 2064 6576  ndencies for dev
-00000ad0: 656c 6f70 6d65 6e74 2e0a 0a60 6060 6261  elopment...```ba
-00000ae0: 7368 0a70 6970 656e 7620 696e 7374 616c  sh.pipenv instal
-00000af0: 6c20 2d2d 6465 760a 6060 600a 0a52 756e  l --dev.```..Run
-00000b00: 2074 6573 7473 2e0a 0a60 6060 6261 7368   tests...```bash
-00000b10: 0a70 6970 656e 7620 7275 6e20 7079 7468  .pipenv run pyth
-00000b20: 6f6e 2074 6573 742e 7079 0a60 6060 0a0a  on test.py.```..
-00000b30: 2323 2044 6576 656c 6f70 696e 6720 7468  ## Developing th
-00000b40: 6520 434c 490a 0a54 6865 2063 6f6d 6d61  e CLI..The comma
-00000b50: 6e64 2d6c 696e 6520 696e 7465 7266 6163  nd-line interfac
-00000b60: 6520 6973 2069 6d70 6c65 6d65 6e74 6564  e is implemented
-00000b70: 2075 7369 6e67 2043 6c69 636b 2061 6e64   using Click and
-00000b80: 2073 6574 7570 746f 6f6c 732e 2054 6f20   setuptools. To 
-00000b90: 696e 7374 616c 6c20 6974 206c 6f63 616c  install it local
-00000ba0: 6c79 2066 6f72 2064 6576 656c 6f70 6d65  ly for developme
-00000bb0: 6e74 2069 6e73 6964 6520 796f 7572 2076  nt inside your v
-00000bc0: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000bd0: 6e74 2c20 7275 6e20 7468 6520 666f 6c6c  nt, run the foll
-00000be0: 6f77 696e 6720 696e 7374 616c 6c61 7469  owing installati
-00000bf0: 6f6e 2063 6f6d 6d61 6e64 2c20 6173 205b  on command, as [
-00000c00: 7072 6573 6372 6962 6564 2062 7920 7468  prescribed by th
-00000c10: 6520 436c 6963 6b20 646f 6375 6d65 6e74  e Click document
-00000c20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f63  ation](https://c
-00000c30: 6c69 636b 2e70 616c 6c65 7473 7072 6f6a  lick.palletsproj
-00000c40: 6563 7473 2e63 6f6d 2f65 6e2f 372e 782f  ects.com/en/7.x/
-00000c50: 7365 7475 7074 6f6f 6c73 2f23 7365 7475  setuptools/#setu
-00000c60: 7074 6f6f 6c73 2d69 6e74 6567 7261 7469  ptools-integrati
-00000c70: 6f6e 292e 0a0a 6060 6062 6173 680a 7069  on)...```bash.pi
-00000c80: 7020 696e 7374 616c 6c20 2d2d 6564 6974  p install --edit
-00000c90: 6162 6c65 202e 0a60 6060 0a0a 2323 204c  able ..```..## L
-00000ca0: 696e 6b73 0a0a 2a20 446f 6373 3a20 5b70  inks..* Docs: [p
-00000cb0: 616c 6577 692e 7265 2f64 6f63 732f 6e61  alewi.re/docs/na
-00000cc0: 7361 2d77 696c 6466 6972 6573 2f5d 2868  sa-wildfires/](h
-00000cd0: 7474 7073 3a2f 2f70 616c 6577 692e 7265  ttps://palewi.re
-00000ce0: 2f64 6f63 732f 6e61 7361 2d77 696c 6466  /docs/nasa-wildf
-00000cf0: 6972 6573 2f29 0a2a 2049 7373 7565 733a  ires/).* Issues:
-00000d00: 205b 6769 7468 7562 2e63 6f6d 2f64 6174   [github.com/dat
-00000d10: 6164 6573 6b2f 6e61 7361 2d77 696c 6466  adesk/nasa-wildf
-00000d20: 6972 6573 2f69 7373 7565 735d 2868 7474  ires/issues](htt
-00000d30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d40: 6461 7461 6465 736b 2f6e 6173 612d 7769  datadesk/nasa-wi
-00000d50: 6c64 6669 7265 732f 6973 7375 6573 290a  ldfires/issues).
-00000d60: 2a20 5061 636b 6167 696e 673a 205b 7079  * Packaging: [py
-00000d70: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-00000d80: 7069 2f6e 6173 612d 7769 6c64 6669 7265  pi/nasa-wildfire
-00000d90: 735d 2868 7474 7073 3a2f 2f70 7970 692e  s](https://pypi.
-00000da0: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-00000db0: 6e61 7361 2d77 696c 6466 6972 6573 290a  nasa-wildfires).
-00000dc0: 2a20 5465 7374 696e 673a 205b 6769 7468  * Testing: [gith
-00000dd0: 7562 2e63 6f6d 2f64 6174 6164 6573 6b2f  ub.com/datadesk/
-00000de0: 6e61 7361 2d77 696c 6466 6972 6573 2f61  nasa-wildfires/a
-00000df0: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
-00000e00: 6769 7468 7562 2e63 6f6d 2f64 6174 6164  github.com/datad
-00000e10: 6573 6b2f 6e61 7361 2d77 696c 6466 6972  esk/nasa-wildfir
-00000e20: 6573 2f61 6374 696f 6e73 290a            es/actions).
+000000e0: 652f 290a 0a60 6060 7b63 6f6e 7465 6e74  e/)..```{content
+000000f0: 737d 2054 6162 6c65 206f 6620 636f 6e74  s} Table of cont
+00000100: 656e 7473 0a3a 6c6f 6361 6c3a 0a3a 6465  ents.:local:.:de
+00000110: 7074 683a 2032 0a60 6060 0a0a 2323 2049  pth: 2.```..## I
+00000120: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
+00000130: 6261 7368 0a70 6970 656e 7620 696e 7374  bash.pipenv inst
+00000140: 616c 6c20 6e61 7361 2d77 696c 6466 6972  all nasa-wildfir
+00000150: 6573 0a60 6060 0a0a 2323 2043 6f6d 6d61  es.```..## Comma
+00000160: 6e64 2d6c 696e 6520 7573 6167 650a 0a60  nd-line usage..`
+00000170: 6060 6261 7368 0a55 7361 6765 3a20 6e61  ``bash.Usage: na
+00000180: 7361 7769 6c64 6669 7265 7320 5b4f 5054  sawildfires [OPT
+00000190: 494f 4e53 5d20 434f 4d4d 414e 4420 5b41  IONS] COMMAND [A
+000001a0: 5247 535d 2e2e 2e0a 0a20 2041 2063 6f6d  RGS].....  A com
+000001b0: 6d61 6e64 2d6c 696e 6520 696e 7465 7266  mand-line interf
+000001c0: 6163 6520 666f 7220 646f 776e 6c6f 6164  ace for download
+000001d0: 696e 6720 7769 6c64 6669 7265 2064 6174  ing wildfire dat
+000001e0: 6120 6672 6f6d 204e 4153 410a 2020 7361  a from NASA.  sa
+000001f0: 7465 6c6c 6974 6573 2e0a 0a20 2052 6574  tellites...  Ret
+00000200: 7572 6e73 2077 6f72 6c64 2047 656f 4a53  urns world GeoJS
+00000210: 4f4e 2069 6e20 6120 7265 6365 6e74 2032  ON in a recent 2
+00000220: 342d 686f 7572 2070 6572 696f 642e 2046  4-hour period. F
+00000230: 6f72 2061 7661 696c 6162 6c65 2072 6567  or available reg
+00000240: 696f 6e73 2061 6e64 2074 696d 6520 7261  ions and time ra
+00000250: 6e67 6573 2c20 7365 6520 6f70 7469 6f6e  nges, see option
+00000260: 732e 0a0a 4f70 7469 6f6e 733a 0a20 202d  s...Options:.  -
+00000270: 2d68 656c 7020 2053 686f 7720 7468 6973  -help  Show this
+00000280: 206d 6573 7361 6765 2061 6e64 2065 7869   message and exi
+00000290: 742e 0a0a 436f 6d6d 616e 6473 3a0a 2020  t...Commands:.  
+000002a0: 6d6f 6469 7320 2048 6f74 7370 6f74 7320  modis  Hotspots 
+000002b0: 6465 7465 6374 6564 2062 7920 7468 6520  detected by the 
+000002c0: 4d4f 4449 5320 7361 7465 6c6c 6974 656c  MODIS satellitel
+000002d0: 0a20 2076 6969 7273 5f73 756f 6d69 2020  .  viirs_suomi  
+000002e0: 486f 7473 706f 7473 2064 6574 6563 7465  Hotspots detecte
+000002f0: 6420 6279 2074 6865 2056 4952 5253 2053  d by the VIRRS S
+00000300: 2d4e 5050 2073 6174 656c 6c69 7465 2e0a  -NPP satellite..
+00000310: 2020 7669 6972 735f 6e6f 6161 2020 486f    viirs_noaa  Ho
+00000320: 7473 706f 7473 2064 6574 6563 7465 6420  tspots detected 
+00000330: 6279 2074 6865 2056 4952 5253 204e 4f41  by the VIRRS NOA
+00000340: 412d 3230 2073 6174 656c 6c69 7465 2e0a  A-20 satellite..
+00000350: 6060 600a 446f 776e 6c6f 6164 2061 2047  ```.Download a G
+00000360: 656f 4a53 4f4e 206f 6620 686f 7473 706f  eoJSON of hotspo
+00000370: 7473 2064 6574 6563 7465 6420 6279 2074  ts detected by t
+00000380: 6865 204d 4f44 4953 2073 6174 656c 6c69  he MODIS satelli
+00000390: 7465 2069 6e20 6120 7265 6365 6e74 2032  te in a recent 2
+000003a0: 342d 686f 7572 2070 6572 696f 642e 0a0a  4-hour period...
+000003b0: 6060 6062 6173 680a 6e61 7361 7769 6c64  ```bash.nasawild
+000003c0: 6669 7265 7320 6d6f 6469 730a 6060 600a  fires modis.```.
+000003d0: 0a44 6f77 6e6c 6f61 6420 6120 4765 6f4a  .Download a GeoJ
+000003e0: 534f 4e20 6f66 2068 6f74 7370 6f74 7320  SON of hotspots 
+000003f0: 6465 7465 6374 6564 2062 7920 7468 6520  detected by the 
+00000400: 4d4f 4449 5320 7361 7465 6c6c 6974 6520  MODIS satellite 
+00000410: 666f 7220 5553 4120 616e 6420 4861 7761  for USA and Hawa
+00000420: 6969 2069 6e20 6120 7265 6365 6e74 2034  ii in a recent 4
+00000430: 382d 686f 7572 2070 6572 696f 642e 0a0a  8-hour period...
+00000440: 6060 6062 6173 680a 6e61 7361 7769 6c64  ```bash.nasawild
+00000450: 6669 7265 7320 6d6f 6469 7320 2d72 2075  fires modis -r u
+00000460: 7361 2d68 6177 6169 6920 2d74 2034 3868  sa-hawaii -t 48h
+00000470: 0a60 6060 0a0a 446f 776e 6c6f 6164 2061  .```..Download a
+00000480: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
+00000490: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
+000004a0: 2074 6865 2056 4949 5253 2053 2d4e 5050   the VIIRS S-NPP
+000004b0: 2073 6174 656c 6c69 7465 2069 6e20 6120   satellite in a 
+000004c0: 7265 6365 6e74 2032 342d 686f 7572 2070  recent 24-hour p
+000004d0: 6572 696f 642e 0a0a 6060 6062 6173 680a  eriod...```bash.
+000004e0: 6e61 7361 7769 6c64 6669 7265 7320 7669  nasawildfires vi
+000004f0: 6972 732d 7375 6f6d 690a 6060 600a 0a44  irs-suomi.```..D
+00000500: 6f77 6e6c 6f61 6420 6120 4765 6f4a 534f  ownload a GeoJSO
+00000510: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
+00000520: 7465 6374 6564 2062 7920 7468 6520 5649  tected by the VI
+00000530: 4952 5320 4e4f 4141 2d32 3020 7361 7465  IRS NOAA-20 sate
+00000540: 6c6c 6974 6520 696e 2061 2072 6563 656e  llite in a recen
+00000550: 7420 3234 2d68 6f75 7220 7065 7269 6f64  t 24-hour period
+00000560: 2e0a 0a60 6060 6261 7368 0a6e 6173 6177  ...```bash.nasaw
+00000570: 696c 6466 6972 6573 2076 6969 7273 2d6e  ildfires viirs-n
+00000580: 6f61 610a 6060 600a 0a23 2320 5079 7468  oaa.```..## Pyth
+00000590: 6f6e 2075 7361 6765 0a0a 496d 706f 7274  on usage..Import
+000005a0: 2074 6865 206c 6962 7261 7279 2e0a 0a60   the library...`
+000005b0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+000005c0: 6e61 7361 5f77 696c 6466 6972 6573 0a60  nasa_wildfires.`
+000005d0: 6060 0a0a 5669 6577 206c 6973 7420 6f66  ``..View list of
+000005e0: 2061 7661 696c 6162 6c65 2072 6567 696f   available regio
+000005f0: 6e73 0a60 6060 7079 7468 6f6e 0a6e 6173  ns.```python.nas
+00000600: 615f 7769 6c64 6669 7265 732e 5245 4749  a_wildfires.REGI
+00000610: 4f4e 5f4c 4953 540a 5b0a 2020 2020 2267  ON_LIST.[.    "g
+00000620: 6c6f 6261 6c22 2c0a 2020 2020 2263 616e  lobal",.    "can
+00000630: 6164 6122 2c0a 2020 2020 2261 6c61 736b  ada",.    "alask
+00000640: 6122 2c0a 2020 2020 2275 7361 2d68 6177  a",.    "usa-haw
+00000650: 6169 6922 2c0a 2020 2020 2263 656e 7472  aii",.    "centr
+00000660: 616c 2d61 6d65 7269 6361 222c 0a20 2020  al-america",.   
+00000670: 2022 736f 7574 682d 616d 6572 6963 6122   "south-america"
+00000680: 2c0a 2020 2020 2265 7572 6f70 6522 2c0a  ,.    "europe",.
+00000690: 2020 2020 226e 6f72 7468 2d63 656e 7472      "north-centr
+000006a0: 616c 2d61 6672 6963 6122 2c0a 2020 2020  al-africa",.    
+000006b0: 2273 6f75 7468 6572 6e2d 6166 7269 6361  "southern-africa
+000006c0: 222c 0a20 2020 2022 7275 7373 6961 2d61  ",.    "russia-a
+000006d0: 7369 6122 2c0a 2020 2020 2273 6f75 7468  sia",.    "south
+000006e0: 2d61 7369 6122 2c0a 2020 2020 2273 6f75  -asia",.    "sou
+000006f0: 7468 6561 7374 2d61 7369 6122 2c0a 2020  theast-asia",.  
+00000700: 2020 2261 7573 7472 616c 6961 2d6e 6577    "australia-new
+00000710: 7a65 616c 616e 6422 2c0a 5d0a 6060 600a  zealand",.].```.
+00000720: 0a56 6965 7720 6c69 7374 206f 6620 6176  .View list of av
+00000730: 6169 6c61 6265 2074 696d 6520 7261 6e67  ailabe time rang
+00000740: 6573 0a60 6060 7079 7468 6f6e 0a6e 6173  es.```python.nas
+00000750: 615f 7769 6c64 6669 7265 732e 5449 4d45  a_wildfires.TIME
+00000760: 5f52 414e 4745 5f4c 4953 540a 5b22 3234  _RANGE_LIST.["24
+00000770: 6822 2c20 2234 3868 222c 2022 3764 225d  h", "48h", "7d"]
+00000780: 0a60 6060 0a0a 446f 776e 6c6f 6164 2061  .```..Download a
+00000790: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
+000007a0: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
+000007b0: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
+000007c0: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
+000007d0: 2032 342d 686f 7572 2070 6572 696f 642e   24-hour period.
+000007e0: 2052 6574 7572 6e73 2047 656f 4a53 4f4e   Returns GeoJSON
+000007f0: 2e0a 0a60 6060 7079 7468 6f6e 0a64 6174  ...```python.dat
+00000800: 6120 3d20 6e61 7361 5f77 696c 6466 6972  a = nasa_wildfir
+00000810: 6573 2e67 6574 5f6d 6f64 6973 2829 0a60  es.get_modis().`
+00000820: 6060 0a0a 446f 776e 6c6f 6164 2061 2072  ``..Download a r
+00000830: 6567 696f 6e61 6c20 4765 6f4a 534f 4e20  egional GeoJSON 
+00000840: 6f66 2068 6f74 7370 6f74 7320 6465 7465  of hotspots dete
+00000850: 6374 6564 2062 7920 7468 6520 4d4f 4449  cted by the MODI
+00000860: 5320 7361 7465 6c6c 6974 6520 696e 2061  S satellite in a
+00000870: 2072 6563 656e 7420 3234 2d68 6f75 7220   recent 24-hour 
+00000880: 7065 7269 6f64 2e0a 0a60 6060 7079 7468  period...```pyth
+00000890: 6f6e 0a64 6174 6120 3d20 6e61 7361 5f77  on.data = nasa_w
+000008a0: 696c 6466 6972 6573 2e67 6574 5f6d 6f64  ildfires.get_mod
+000008b0: 6973 2872 6567 696f 6e3d 2275 7361 2d68  is(region="usa-h
+000008c0: 6177 6169 6922 290a 6060 600a 0a44 6f77  awaii").```..Dow
+000008d0: 6e6c 6f61 6420 6120 7265 6769 6f6e 616c  nload a regional
+000008e0: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
+000008f0: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
+00000900: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
+00000910: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
+00000920: 2037 2d64 6179 2070 6572 696f 642e 0a0a   7-day period...
+00000930: 6060 6070 7974 686f 6e0a 6461 7461 203d  ```python.data =
+00000940: 206e 6173 615f 7769 6c64 6669 7265 732e   nasa_wildfires.
+00000950: 6765 745f 6d6f 6469 7328 7265 6769 6f6e  get_modis(region
+00000960: 3d22 7573 612d 6861 7761 6969 222c 2074  ="usa-hawaii", t
+00000970: 696d 655f 7261 6e67 653d 2237 6422 290a  ime_range="7d").
+00000980: 6060 600a 0a44 6f77 6e6c 6f61 6420 6120  ```..Download a 
+00000990: 4765 6f4a 534f 4e20 6f66 2068 6f74 7370  GeoJSON of hotsp
+000009a0: 6f74 7320 6465 7465 6374 6564 2062 7920  ots detected by 
+000009b0: 7468 6520 5649 4952 5320 532d 4e50 5020  the VIIRS S-NPP 
+000009c0: 7361 7465 6c6c 6974 6520 696e 2061 2072  satellite in a r
+000009d0: 6563 656e 7420 3234 2d68 6f75 7220 7065  ecent 24-hour pe
+000009e0: 7269 6f64 2e20 5265 7475 726e 7320 4765  riod. Returns Ge
+000009f0: 6f4a 534f 4e2e 0a0a 6060 6070 7974 686f  oJSON...```pytho
+00000a00: 6e0a 6461 7461 203d 206e 6173 615f 7769  n.data = nasa_wi
+00000a10: 6c64 6669 7265 732e 6765 745f 7669 6972  ldfires.get_viir
+00000a20: 735f 7375 6f6d 6928 290a 6060 600a 0a44  s_suomi().```..D
+00000a30: 6f77 6e6c 6f61 6420 6120 4765 6f4a 534f  ownload a GeoJSO
+00000a40: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
+00000a50: 7465 6374 6564 2062 7920 7468 6520 5649  tected by the VI
+00000a60: 4952 5320 4e4f 4141 2d32 3020 7361 7465  IRS NOAA-20 sate
+00000a70: 6c6c 6974 6520 696e 2061 2072 6563 656e  llite in a recen
+00000a80: 7420 3234 2d68 6f75 7220 7065 7269 6f64  t 24-hour period
+00000a90: 2e20 5265 7475 726e 7320 4765 6f4a 534f  . Returns GeoJSO
+00000aa0: 4e2e 0a0a 6060 6070 7974 686f 6e0a 6461  N...```python.da
+00000ab0: 7461 203d 206e 6173 615f 7769 6c64 6669  ta = nasa_wildfi
+00000ac0: 7265 732e 6765 745f 7669 6972 735f 6e6f  res.get_viirs_no
+00000ad0: 6161 2829 0a60 6060 0a0a 2323 2043 6f6e  aa().```..## Con
+00000ae0: 7472 6962 7574 696e 670a 0a49 6e73 7461  tributing..Insta
+00000af0: 6c6c 2064 6570 656e 6465 6e63 6965 7320  ll dependencies 
+00000b00: 666f 7220 6465 7665 6c6f 706d 656e 742e  for development.
+00000b10: 0a0a 6060 6062 6173 680a 7069 7065 6e76  ..```bash.pipenv
+00000b20: 2069 6e73 7461 6c6c 202d 2d64 6576 0a60   install --dev.`
+00000b30: 6060 0a0a 5275 6e20 7465 7374 732e 0a0a  ``..Run tests...
+00000b40: 6060 6062 6173 680a 7069 7065 6e76 2072  ```bash.pipenv r
+00000b50: 756e 2070 7974 686f 6e20 7465 7374 2e70  un python test.p
+00000b60: 790a 6060 600a 0a23 2320 4465 7665 6c6f  y.```..## Develo
+00000b70: 7069 6e67 2074 6865 2043 4c49 0a0a 5468  ping the CLI..Th
+00000b80: 6520 636f 6d6d 616e 642d 6c69 6e65 2069  e command-line i
+00000b90: 6e74 6572 6661 6365 2069 7320 696d 706c  nterface is impl
+00000ba0: 656d 656e 7465 6420 7573 696e 6720 436c  emented using Cl
+00000bb0: 6963 6b20 616e 6420 7365 7475 7074 6f6f  ick and setuptoo
+00000bc0: 6c73 2e20 546f 2069 6e73 7461 6c6c 2069  ls. To install i
+00000bd0: 7420 6c6f 6361 6c6c 7920 666f 7220 6465  t locally for de
+00000be0: 7665 6c6f 706d 656e 7420 696e 7369 6465  velopment inside
+00000bf0: 2079 6f75 7220 7669 7274 7561 6c20 656e   your virtual en
+00000c00: 7669 726f 6e6d 656e 742c 2072 756e 2074  vironment, run t
+00000c10: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e73  he following ins
+00000c20: 7461 6c6c 6174 696f 6e20 636f 6d6d 616e  tallation comman
+00000c30: 642c 2061 7320 5b70 7265 7363 7269 6265  d, as [prescribe
+00000c40: 6420 6279 2074 6865 2043 6c69 636b 2064  d by the Click d
+00000c50: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00000c60: 7470 733a 2f2f 636c 6963 6b2e 7061 6c6c  tps://click.pall
+00000c70: 6574 7370 726f 6a65 6374 732e 636f 6d2f  etsprojects.com/
+00000c80: 656e 2f37 2e78 2f73 6574 7570 746f 6f6c  en/7.x/setuptool
+00000c90: 732f 2373 6574 7570 746f 6f6c 732d 696e  s/#setuptools-in
+00000ca0: 7465 6772 6174 696f 6e29 2e0a 0a60 6060  tegration)...```
+00000cb0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
+00000cc0: 202d 2d65 6469 7461 626c 6520 2e0a 6060   --editable ..``
+00000cd0: 600a 0a23 2320 4c69 6e6b 730a 0a2a 2044  `..## Links..* D
+00000ce0: 6f63 733a 205b 7061 6c65 7769 2e72 652f  ocs: [palewi.re/
+00000cf0: 646f 6373 2f6e 6173 612d 7769 6c64 6669  docs/nasa-wildfi
+00000d00: 7265 732f 5d28 6874 7470 733a 2f2f 7061  res/](https://pa
+00000d10: 6c65 7769 2e72 652f 646f 6373 2f6e 6173  lewi.re/docs/nas
+00000d20: 612d 7769 6c64 6669 7265 732f 290a 2a20  a-wildfires/).* 
+00000d30: 4973 7375 6573 3a20 5b67 6974 6875 622e  Issues: [github.
+00000d40: 636f 6d2f 6461 7461 6465 736b 2f6e 6173  com/datadesk/nas
+00000d50: 612d 7769 6c64 6669 7265 732f 6973 7375  a-wildfires/issu
+00000d60: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00000d70: 7562 2e63 6f6d 2f64 6174 6164 6573 6b2f  ub.com/datadesk/
+00000d80: 6e61 7361 2d77 696c 6466 6972 6573 2f69  nasa-wildfires/i
+00000d90: 7373 7565 7329 0a2a 2050 6163 6b61 6769  ssues).* Packagi
+00000da0: 6e67 3a20 5b70 7970 692e 7079 7468 6f6e  ng: [pypi.python
+00000db0: 2e6f 7267 2f70 7970 692f 6e61 7361 2d77  .org/pypi/nasa-w
+00000dc0: 696c 6466 6972 6573 5d28 6874 7470 733a  ildfires](https:
+00000dd0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000de0: 672f 7079 7069 2f6e 6173 612d 7769 6c64  g/pypi/nasa-wild
+00000df0: 6669 7265 7329 0a2a 2054 6573 7469 6e67  fires).* Testing
+00000e00: 3a20 5b67 6974 6875 622e 636f 6d2f 6461  : [github.com/da
+00000e10: 7461 6465 736b 2f6e 6173 612d 7769 6c64  tadesk/nasa-wild
+00000e20: 6669 7265 732f 6163 7469 6f6e 735d 2868  fires/actions](h
+00000e30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000e40: 6d2f 6461 7461 6465 736b 2f6e 6173 612d  m/datadesk/nasa-
+00000e50: 7769 6c64 6669 7265 732f 6163 7469 6f6e  wildfires/action
+00000e60: 7329 0a                                  s).
```

### Comparing `nasa-wildfires-1.1.0/docs/make.bat` & `nasa-wildfires-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/nasa_wildfires/__init__.py` & `nasa-wildfires-1.1.1/nasa_wildfires/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,54 +4,60 @@
 import requests
 
 from .options import REGION_DICT
 
 REGION_LIST = list(REGION_DICT.keys())
 
 
-def get_modis(region="global", time_range="24h"):
+def get_modis(
+    region: str = "global", time_range: str = "24h"
+) -> geojson.FeatureCollection:
     """
     Hotspots detected by the MODIS satellite. Defaults to the world in a recent 24-hour period.
 
     Returns GeoJSON.
     """
     base_url = "https://firms.modaps.eosdis.nasa.gov/data/active_fire/modis-c6.1/csv/MODIS_C6_1_{}_{}.csv"
     name = REGION_DICT[region]
     url = base_url.format(name, time_range)
     features = _get_features(url)
     return geojson.FeatureCollection(features)
 
 
-def get_viirs_suomi(region="global", time_range="24h"):
+def get_viirs_suomi(
+    region: str = "global", time_range: str = "24h"
+) -> geojson.FeatureCollection:
     """
     Hotspots detected by the VIIRS Suomi-NPP (S-NPP) satellite. Defaults to the world in a recent 24-hour period.
 
     Returns GeoJSON.
     """
     base_url = "https://firms.modaps.eosdis.nasa.gov/data/active_fire/suomi-npp-viirs-c2/csv/SUOMI_VIIRS_C2_{}_{}.csv"
     name = REGION_DICT[region]
     url = base_url.format(name, time_range)
     features = _get_features(url)
     return geojson.FeatureCollection(features)
 
 
-def get_viirs_noaa(region="global", time_range="24h"):
+def get_viirs_noaa(
+    region: str = "global", time_range: str = "24h"
+) -> geojson.FeatureCollection:
     """
     Hotspots detected by the VIIRS NOAA-20 satellite. Defaults to the world in a recent 24-hour period.
 
     Returns GeoJSON.
     """
     base_url = "https://firms.modaps.eosdis.nasa.gov/data/active_fire/noaa-20-viirs-c2/csv/J1_VIIRS_C2_{}_{}.csv"
     name = REGION_DICT[region]
     url = base_url.format(name, time_range)
     features = _get_features(url)
     return geojson.FeatureCollection(features)
 
 
-def _get_features(url):
+def _get_features(url: str) -> list:
     """
     Generic function for downloading data from NASA and reformatting as GeoJSON.
     """
     download = requests.get(url)
     decoded_content = download.content.decode("utf-8")
     reader = csv.DictReader(decoded_content.splitlines(), delimiter=",")
     features = []
```

### Comparing `nasa-wildfires-1.1.0/nasa_wildfires/cli.py` & `nasa-wildfires-1.1.1/nasa_wildfires/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 @cmd.command(help="Hotspots detected by the MODIS satellite in a recent 24-hour period")
 @click.option(
     "-r",
     "--region",
     default="Global",
-    type=click.Choice(options.REGION_DICT.keys(), case_sensitive=False),
+    type=click.Choice(list(options.REGION_DICT.keys()), case_sensitive=False),
     help="Hotspot region",
 )
 @click.option(
     "-t",
     "--time-range",
     default="24h",
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
@@ -42,15 +42,15 @@
 @cmd.command(
     help="Hotspots detected by the VIIRS satellite (S-NPP) in a recent 24-hour period"
 )
 @click.option(
     "-r",
     "--region",
     default="Global",
-    type=click.Choice(options.REGION_DICT.keys(), case_sensitive=False),
+    type=click.Choice(list(options.REGION_DICT.keys()), case_sensitive=False),
     help="Hotspot region",
 )
 @click.option(
     "-t",
     "--time-range",
     default="24h",
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
@@ -69,15 +69,15 @@
 @cmd.command(
     help="Hotspots detected by the VIIRS satellite (NOAA-20) in a recent 24-hour period"
 )
 @click.option(
     "-r",
     "--region",
     default="Global",
-    type=click.Choice(options.REGION_DICT.keys(), case_sensitive=False),
+    type=click.Choice(list(options.REGION_DICT.keys()), case_sensitive=False),
     help="Hotspot region",
 )
 @click.option(
     "-t",
     "--time-range",
     default="24h",
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
```

### Comparing `nasa-wildfires-1.1.0/nasa_wildfires/options.py` & `nasa-wildfires-1.1.1/nasa_wildfires/options.py`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.0/nasa_wildfires.egg-info/PKG-INFO` & `nasa-wildfires-1.1.1/nasa_wildfires.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nasa-wildfires
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download wildfire hotspots detected by NASA satellites and the Fire Information for Resource Management System (FIRMS)
 Home-page: https://palewi.re/docs/nasa-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nasa-wildfires
 Project-URL: Tracker, https://github.com/datadesk/nasa-wildfires/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Links
```

### Comparing `nasa-wildfires-1.1.0/nasa_wildfires.egg-info/SOURCES.txt` & `nasa-wildfires-1.1.1/nasa_wildfires.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
-Makefile
 Pipfile
 Pipfile.lock
 README.md
 setup.cfg
 setup.py
 test.py
 .github/workflows/continuous-deployment.yml
```

### Comparing `nasa-wildfires-1.1.0/setup.py` & `nasa-wildfires-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         [console_scripts]
         nasawildfires=nasa_wildfires.cli:cmd
     """,
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
     ],
     project_urls={
         "Maintainer": "https://github.com/datadesk",
         "Source": "https://github.com/datadesk/nasa-wildfires",
         "Tracker": "https://github.com/datadesk/nasa-wildfires/issues",
```

### Comparing `nasa-wildfires-1.1.0/test.py` & `nasa-wildfires-1.1.1/test.py`

 * *Files identical despite different names*

