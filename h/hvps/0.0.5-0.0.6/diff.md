# Comparing `tmp/hvps-0.0.5.tar.gz` & `tmp/hvps-0.0.6.tar.gz`

## Comparing `hvps-0.0.5.tar` & `hvps-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hvps-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hvps-0.0.5/.github/CODEOWNERS
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 hvps-0.0.5/.github/workflows/build-test.yml
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 hvps-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 hvps-0.0.5/bindings/nodejs/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hvps-0.0.5/bindings/nodejs/cli.js
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 hvps-0.0.5/bindings/nodejs/index.js
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 hvps-0.0.5/bindings/nodejs/package-lock.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hvps-0.0.5/bindings/nodejs/package.json
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/__init__.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/__main__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/caen/__init__.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/caen/channel.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/caen/module.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/iseg/__init__.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/iseg/channel.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/commands/iseg/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/channel.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/hvps.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/caen/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/caen/caen.py
--rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/caen/channel.py
--rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/caen/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/__init__.py
--rw-r--r--   0        0        0    39273 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/channel.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/iseg.py
--rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/module.py
--rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/output.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/devices/iseg/script.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/utils/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hvps-0.0.5/src/hvps/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_caen_commands.py
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_caen_serial.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_cli.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_iseg_commands.py
--rw-r--r--   0        0        0    10901 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_iseg_serial.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hvps-0.0.5/tests/test_utils.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hvps-0.0.5/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hvps-0.0.5/LICENSE
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 hvps-0.0.5/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hvps-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 hvps-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hvps-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hvps-0.0.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 hvps-0.0.6/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 hvps-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 hvps-0.0.6/bindings/nodejs/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hvps-0.0.6/bindings/nodejs/cli.js
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 hvps-0.0.6/bindings/nodejs/index.js
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 hvps-0.0.6/bindings/nodejs/package-lock.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hvps-0.0.6/bindings/nodejs/package.json
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/__main__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/caen/__init__.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/caen/channel.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/caen/module.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/iseg/__init__.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/iseg/channel.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/commands/iseg/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/channel.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/hvps.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/caen/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/caen/caen.py
+-rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/caen/channel.py
+-rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/caen/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/__init__.py
+-rw-r--r--   0        0        0    39273 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/channel.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/iseg.py
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/module.py
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/output.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/devices/iseg/script.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/utils/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hvps-0.0.6/src/hvps/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_caen_commands.py
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_caen_serial.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_cli.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_iseg_commands.py
+-rw-r--r--   0        0        0    10901 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_iseg_serial.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hvps-0.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hvps-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hvps-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 hvps-0.0.6/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hvps-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 hvps-0.0.6/PKG-INFO
```

### Comparing `hvps-0.0.5/.pre-commit-config.yaml` & `hvps-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/.github/workflows/build-test.yml` & `hvps-0.0.6/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/.github/workflows/publish.yml` & `hvps-0.0.6/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         uses: actions/checkout@v3
 
       - uses: actions/setup-node@v3
         with:
           node-version: 18
           cache: 'npm'
           cache-dependency-path: bindings/nodejs/package-lock.json
+          registry-url: 'https://registry.npmjs.org'
 
       - name: Install dependencies
         run: npm ci
 
       - name: Publish to npm
         run: npm publish
         env:
```

### Comparing `hvps-0.0.5/bindings/nodejs/cli.js` & `hvps-0.0.6/bindings/nodejs/cli.js`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/bindings/nodejs/index.js` & `hvps-0.0.6/bindings/nodejs/index.js`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/bindings/nodejs/package-lock.json` & `hvps-0.0.6/bindings/nodejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/bindings/nodejs/package.json` & `hvps-0.0.6/bindings/nodejs/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.0.6'"}*

```diff
@@ -17,9 +17,9 @@
     "repository": {
         "type": "git",
         "url": "git+https://github.com/lobis/hvps.git"
     },
     "scripts": {
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "0.0.5"
+    "version": "0.0.6"
 }
```

### Comparing `hvps-0.0.5/src/hvps/__main__.py` & `hvps-0.0.6/src/hvps/__main__.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/caen/__init__.py` & `hvps-0.0.6/src/hvps/commands/caen/__init__.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/caen/channel.py` & `hvps-0.0.6/src/hvps/commands/caen/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/caen/module.py` & `hvps-0.0.6/src/hvps/commands/caen/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/iseg/__init__.py` & `hvps-0.0.6/src/hvps/commands/iseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/iseg/channel.py` & `hvps-0.0.6/src/hvps/commands/iseg/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/commands/iseg/module.py` & `hvps-0.0.6/src/hvps/commands/iseg/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/channel.py` & `hvps-0.0.6/src/hvps/devices/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/hvps.py` & `hvps-0.0.6/src/hvps/devices/hvps.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/module.py` & `hvps-0.0.6/src/hvps/devices/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/caen/channel.py` & `hvps-0.0.6/src/hvps/devices/caen/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/caen/module.py` & `hvps-0.0.6/src/hvps/devices/caen/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/iseg/channel.py` & `hvps-0.0.6/src/hvps/devices/iseg/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/iseg/module.py` & `hvps-0.0.6/src/hvps/devices/iseg/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/iseg/output.py` & `hvps-0.0.6/src/hvps/devices/iseg/output.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/devices/iseg/script.py` & `hvps-0.0.6/src/hvps/devices/iseg/script.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/src/hvps/utils/utils.py` & `hvps-0.0.6/src/hvps/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_caen_commands.py` & `hvps-0.0.6/tests/test_caen_commands.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_caen_serial.py` & `hvps-0.0.6/tests/test_caen_serial.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_cli.py` & `hvps-0.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_iseg_commands.py` & `hvps-0.0.6/tests/test_iseg_commands.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_iseg_serial.py` & `hvps-0.0.6/tests/test_iseg_serial.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/tests/test_utils.py` & `hvps-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/.gitignore` & `hvps-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/LICENSE` & `hvps-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/README.md` & `hvps-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/pyproject.toml` & `hvps-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hvps-0.0.5/PKG-INFO` & `hvps-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvps
-Version: 0.0.5
+Version: 0.0.6
 Summary: An unofficial Python package 🐍📦 to interface with CAEN high voltage power supplies
 Project-URL: Download, https://github.com/lobis/hvps/releases
 Project-URL: Homepage, https://github.com/lobis/hvps
 Project-URL: Bug Tracker, https://github.com/lobis/hvps/issues
 Author-email: Luis Antonio Obis Aparicio <luis.antonio.obis@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

