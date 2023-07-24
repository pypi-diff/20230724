# Comparing `tmp/sparglim-0.0.1a0.tar.gz` & `tmp/sparglim-0.1.0rc0.tar.gz`

## Comparing `sparglim-0.0.1a0.tar` & `sparglim-0.1.0rc0.tar`

### file list

```diff
@@ -1,29 +1,49 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/RELEASE.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/docs/Makefile
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/docs/conf.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/docs/index.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/docs/make.bat
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/docs/usage.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/py.typed
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/utils.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/config/__init__.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/config/builder.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/config/k8s.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/tests/test_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/tests/test_magic.py
--rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/.gitignore
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/README.md
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 sparglim-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/RELEASE.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/Makefile
+-rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/conf.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/index.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/make.bat
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/usage.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/Dockerfile.lab
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/Dockerfile.lab
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/lab-service.yaml
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/reload.sh
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/PKG-INFO
```

### Comparing `sparglim-0.0.1a0/.pre-commit-config.yaml` & `sparglim-0.1.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/RELEASE.md` & `sparglim-0.1.0rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/.github/workflows/python-package.yml` & `sparglim-0.1.0rc0/.github/workflows/python-package.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[test]
+    - name: Test with pytype
+      continue-on-error: true
+      run: |
+        pytype ./sparglim
     - name: Test with pytest
       run: |
         pytest -vv
```

### Comparing `sparglim-0.0.1a0/.github/workflows/python-publish.yml` & `sparglim-0.1.0rc0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/docs/Makefile` & `sparglim-0.1.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/docs/conf.py` & `sparglim-0.1.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/docs/make.bat` & `sparglim-0.1.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sparglim-0.0.1a0/sparglim/config/k8s.py` & `sparglim-0.1.0rc0/sparglim/config/k8s.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2023 Wh1isper
 #  Licensed under the BSD 3-Clause License
+
 import os
 
 from kubernetes import config
 from kubernetes.client import Configuration
 
 INCLUSTER = os.path.exists("/var/run/secrets/kubernetes.io/serviceaccount/namespace")
 
@@ -12,20 +13,29 @@
         default_namespace = f.read()
 else:
     default_namespace = "spark-app"
 
 NAMESPACE = os.getenv("SPARK_EXECUTOR_NS", default_namespace)
 
 
-def get_k8s_config():
+def get_k8s_config(config_file_path=None):
     if INCLUSTER:
         config.load_incluster_config()
     else:
-        config.load_kube_config(os.path.expanduser("~/.kube/config"))
+        config_file_path = config_file_path or os.path.expanduser("~/.kube/config")
+        config.load_kube_config(config_file_path)
     k8s_config = Configuration.get_default_copy()
     token = k8s_config.api_key.get("authorization")
     host = k8s_config.host
     ca = k8s_config.ssl_ca_cert
     key_file = k8s_config.key_file
     cert_file = k8s_config.cert_file
 
     return host, token, ca, key_file, cert_file
+
+
+def get_namespace():
+    if not INCLUSTER:
+        return "sparglim"
+    with open("/var/run/secrets/kubernetes.io/serviceaccount/namespace") as f:
+        default_namespace = f.read()
+    return default_namespace
```

### Comparing `sparglim-0.0.1a0/.gitignore` & `sparglim-0.1.0rc0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -564,7 +564,9 @@
 .pyre/
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
+
+spark-warehouse/
```

### Comparing `sparglim-0.0.1a0/LICENSE` & `sparglim-0.1.0rc0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
+BSD 3-Clause License
 
+Copyright (c) 2023, Wh1isper
 
-BSD License
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-Copyright (c) 2023, wh1isper
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice, this
-  list of conditions and the following disclaimer in the documentation and/or
-  other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from this
-  software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
-OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sparglim-0.0.1a0/README.md` & `sparglim-0.1.0rc0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 # Feature
 
 ## Config pyspark via Environment Variables
 
 ## SQL Magic
 
+## Connect Server daemon
+
 ## Install
 
 `pip install sparglim`
 
 ## Usage
 
 ## Develop
```

### Comparing `sparglim-0.0.1a0/pyproject.toml` & `sparglim-0.1.0rc0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "sparglim"
 description = "sparglim"
 keywords = ["sparglim"]
 requires-python = ">=3.8"
-dependencies = ["pyspark", "findspark", "loguru"]
+dependencies = ["loguru", "click", "findspark", "psutil"]
 dynamic = ["version"]
 classifiers = [
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 [project.optional-dependencies]
-test = ["pytest"]
-magic = ["ipython"]
-k8s = ["kubernetes"]
-all = [
-    "pyspark[pandas_on_spark]",
-    "pyspark[sql]",
-    "pyspark[connect]",
-    "sparglim[magic]",
-    "sparglim[k8s]",
-]
-dev = ["sparglim[all]", "sparglim[test]"]
+pyspark = ["pyspark[pandas_on_spark,sql,connect]"]
+magic = ["sparglim[pyspark]", "ipython"]
+k8s = ["sparglim[pyspark]", "kubernetes"]
+
+all = ["sparglim[pyspark]", "sparglim[magic]", "sparglim[k8s]"]
+test = ["sparglim[all]", "pytest", "pytest-cov", "pytype", "pytest-timeout"]
+# TODO: Docs and its dependencies
+dev = ["sparglim[test]"]
 
+[project.scripts]
+sparglim-server = "sparglim.server.cli:cli"
 
 [[project.authors]]
 name = "wh1isper"
 email = "9573586@qq.com"
 
 [project.readme]
 file = "README.md"
```

### Comparing `sparglim-0.0.1a0/PKG-INFO` & `sparglim-0.1.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.0.1a0
+Version: 0.1.0rc0
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: sparglim
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: click
 Requires-Dist: findspark
 Requires-Dist: loguru
-Requires-Dist: pyspark
+Requires-Dist: psutil
 Provides-Extra: all
-Requires-Dist: pyspark[connect]; extra == 'all'
-Requires-Dist: pyspark[pandas-on-spark]; extra == 'all'
-Requires-Dist: pyspark[sql]; extra == 'all'
 Requires-Dist: sparglim[k8s]; extra == 'all'
 Requires-Dist: sparglim[magic]; extra == 'all'
+Requires-Dist: sparglim[pyspark]; extra == 'all'
 Provides-Extra: dev
-Requires-Dist: sparglim[all]; extra == 'dev'
 Requires-Dist: sparglim[test]; extra == 'dev'
 Provides-Extra: k8s
 Requires-Dist: kubernetes; extra == 'k8s'
+Requires-Dist: sparglim[pyspark]; extra == 'k8s'
 Provides-Extra: magic
 Requires-Dist: ipython; extra == 'magic'
+Requires-Dist: sparglim[pyspark]; extra == 'magic'
+Provides-Extra: pyspark
+Requires-Dist: pyspark[connect,pandas-on-spark,sql]; extra == 'pyspark'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-timeout; extra == 'test'
+Requires-Dist: pytype; extra == 'test'
+Requires-Dist: sparglim[all]; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![](https://img.shields.io/github/license/wh1isper/sparglim)
 ![](https://img.shields.io/github/v/release/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
@@ -44,14 +51,16 @@
 
 # Feature
 
 ## Config pyspark via Environment Variables
 
 ## SQL Magic
 
+## Connect Server daemon
+
 ## Install
 
 `pip install sparglim`
 
 ## Usage
 
 ## Develop
```

