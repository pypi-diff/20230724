# Comparing `tmp/cytotransform-0.2.11.tar.gz` & `tmp/cytotransform-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytotransform-0.2.11.tar", max compression
+gzip compressed data, was "cytotransform-0.2.12.tar", max compression
```

## Comparing `cytotransform-0.2.11.tar` & `cytotransform-0.2.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1062 2023-07-24 14:16:50.303332 cytotransform-0.2.11/LICENSE
--rw-r--r--   0        0        0     3536 2023-07-24 14:16:50.303332 cytotransform-0.2.11/README.md
--rw-r--r--   0        0        0      578 2023-07-24 14:16:50.303332 cytotransform-0.2.11/build.py
--rw-r--r--   0        0        0      154 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/__init__.py
--rw-r--r--   0        0        0     2282 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/asinh.py
--rw-r--r--   0        0        0     3011 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/base.py
--rw-r--r--   0        0        0     3166 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/hyperlog.py
--rw-r--r--   0        0        0     1888 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/log.py
--rw-r--r--   0        0        0     3885 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle.py
--rw-r--r--   0        0        0       92 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle_ext/.gitignore
--rw-r--r--   0        0        0     4216 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle_ext/FastLogicle.cpp
--rw-r--r--   0        0        0     1760 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle_ext/LICENSE.txt
--rw-r--r--   0        0        0     8799 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle_ext/Logicle.cpp
--rw-r--r--   0        0        0     5726 2023-07-24 14:16:50.303332 cytotransform-0.2.11/cytotransform/logicle_ext/logicle.h
--rw-r--r--   0        0        0     1983 2023-07-24 14:16:50.307332 cytotransform-0.2.11/pyproject.toml
--rw-r--r--   0        0        0     4501 1970-01-01 00:00:00.000000 cytotransform-0.2.11/setup.py
--rw-r--r--   0        0        0     4371 1970-01-01 00:00:00.000000 cytotransform-0.2.11/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-24 14:24:18.541369 cytotransform-0.2.12/LICENSE
+-rw-r--r--   0        0        0     3536 2023-07-24 14:24:18.541369 cytotransform-0.2.12/README.md
+-rw-r--r--   0        0        0      578 2023-07-24 14:24:18.541369 cytotransform-0.2.12/build.py
+-rw-r--r--   0        0        0      154 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/__init__.py
+-rw-r--r--   0        0        0     2282 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/asinh.py
+-rw-r--r--   0        0        0     3011 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/base.py
+-rw-r--r--   0        0        0     3166 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/hyperlog.py
+-rw-r--r--   0        0        0     1888 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/log.py
+-rw-r--r--   0        0        0     3885 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle.py
+-rw-r--r--   0        0        0       92 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle_ext/.gitignore
+-rw-r--r--   0        0        0     4216 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle_ext/FastLogicle.cpp
+-rw-r--r--   0        0        0     1760 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle_ext/LICENSE.txt
+-rw-r--r--   0        0        0     8799 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle_ext/Logicle.cpp
+-rw-r--r--   0        0        0     5726 2023-07-24 14:24:18.541369 cytotransform-0.2.12/cytotransform/logicle_ext/logicle.h
+-rw-r--r--   0        0        0     1984 2023-07-24 14:24:18.541369 cytotransform-0.2.12/pyproject.toml
+-rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 cytotransform-0.2.12/setup.py
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 cytotransform-0.2.12/PKG-INFO
```

### Comparing `cytotransform-0.2.11/LICENSE` & `cytotransform-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/README.md` & `cytotransform-0.2.12/README.md`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/build.py` & `cytotransform-0.2.12/build.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/asinh.py` & `cytotransform-0.2.12/cytotransform/asinh.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/base.py` & `cytotransform-0.2.12/cytotransform/base.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/hyperlog.py` & `cytotransform-0.2.12/cytotransform/hyperlog.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/log.py` & `cytotransform-0.2.12/cytotransform/log.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/logicle.py` & `cytotransform-0.2.12/cytotransform/logicle.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/logicle_ext/FastLogicle.cpp` & `cytotransform-0.2.12/cytotransform/logicle_ext/FastLogicle.cpp`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/logicle_ext/LICENSE.txt` & `cytotransform-0.2.12/cytotransform/logicle_ext/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/logicle_ext/Logicle.cpp` & `cytotransform-0.2.12/cytotransform/logicle_ext/Logicle.cpp`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/cytotransform/logicle_ext/logicle.h` & `cytotransform-0.2.12/cytotransform/logicle_ext/logicle.h`

 * *Files identical despite different names*

### Comparing `cytotransform-0.2.11/pyproject.toml` & `cytotransform-0.2.12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "cytotransform"
-version = "0.2.11"
+version = "0.2.12"
 description = "Rapid transformations for cytometry data"
 authors = ["Ross Burton <burtonrossj@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-numpy = "^1.24.2"
+numpy = ">=1.17.0"
 joblib = "^1.2.0"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 setuptools = "^67.7.1"
 pybind11 = "^2.10.4"
 pandas = ">=1.3.0,<2.0.0"
```

### Comparing `cytotransform-0.2.11/setup.py` & `cytotransform-0.2.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 package_data = \
 {'': ['*'], 'cytotransform': ['logicle_ext/*']}
 
 install_requires = \
 ['joblib>=1.2.0,<2.0.0',
  'matplotlib>=3.7.1,<4.0.0',
- 'numpy>=1.24.2,<2.0.0',
+ 'numpy>=1.17.0',
  'pandas>=1.3.0,<2.0.0',
  'pybind11>=2.10.4,<3.0.0',
  'scipy>=1.10.1,<2.0.0',
  'setuptools>=67.7.1,<68.0.0']
 
 setup_kwargs = {
     'name': 'cytotransform',
-    'version': '0.2.11',
+    'version': '0.2.12',
     'description': 'Rapid transformations for cytometry data',
     'long_description': '# Cytotransfrom\n\n![PyPI](https://img.shields.io/pypi/v/cytotransform)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cytotransform)\n![PyPI - Wheel](https://img.shields.io/pypi/wheel/cytotransform)\n![PyPI - License](https://img.shields.io/pypi/l/cytotransform)\n![Codecov](https://img.shields.io/codecov/c/github/burtonrj/cytotransform)\n![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/burtonrj/cytotransform/build.yaml)\n\n## Description\n\nCytotransform is a python package for transforming flow cytometry data. It implements the following transformations\naccording to the GatingML 2.0 definitions (https://flowcyt.sourceforge.net/gating/latest.pdf):\n\n- Parametrized logarithmic transformation\n- Parametrized inverse hyperbolic sine transformation (asinh)\n- Logicle transformation\n- Hyperlog transformation\n\nEach transformation is implemented as a `Transform` class with a `transform` method that takes a numpy array as input\nand returns the transformed array. The `Transform` class also has a `transform_inverse` method that takes a numpy array\nas input and returns the inverse transformed array. Each implementation includes validation of the input parameters. The\ntransform classes support multiprocessing out of the box and if `n_jobs` is set to more than 0, then the input data will\nbe split into `n` batches depending on the number of cores available and each batch will be transformed in parallel.\nIf `n_jobs` is set to -1, then all available cores will be used. If `n_jobs` is set to 0, then no multiprocessing will\nbe used.\n\nCytotransform is thanks to the fantastic community of scientists and developers in the single cell and flow\ncytometry data analysis ecosystem. It implements the FastLogicle C++ library for logicle transformations\noriginally implemented by Wayne A Moore and David R Parks (see https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4761345/).\nCode was inspired by the great work by Scott White (https://github.com/whitews/FlowKit) and Brian Teague\n(https://github.com/cytoflow).\n\n## Installation\n\nCytotransform can be installed from PyPi using pip:\n\n```bash\npip install cytotransform\n```\n\n## Usage\n\nThe `transform` and `inverse_transform` methods take a numpy array or Pandas DataFrame as input and return a numpy the\ntransformed array/dataframe.\n\n### Parametrized logarithmic transformation\n\n```python\nfrom cytotransform import ParametrizedLogTransform\ntransformer = ParametrizedLogTransform(m=4.5, t=262144, n_jobs=-1)\ntransformed_data = transformer.transform(data)\ndata = transformer.inverse_transform(transformed_data)\n```\n\n### Parametrized inverse hyperbolic sine transformation (asinh)\n\n```python\nfrom cytotransform import AsinhTransform\ntransformer = AsinhTransform(m=4.5, t=262144, a=0.0, n_jobs=-1)\ntransformed_data = transformer.transform(data)\ndata = transformer.inverse_transform(transformed_data)\n```\n\n### Logicle transformation\n\n```python\nfrom cytotransform import LogicleTransform\ntransformer = LogicleTransform(t=262144, w=0.5, m=4.5, a=0.0, n_jobs=-1)\ntransformed_data = transformer.transform(data)\ndata = transformer.inverse_transform(transformed_data)\n```\n\n### Hyperlog transformation\n\n```python\nfrom cytotransform import HyperlogTransform\ntransformer = HyperlogTransform(t=262144, w=0.5, m=4.5, a=0.0, n_jobs=-1)\ntransformed_data = transformer.transform(data)\ndata = transformer.inverse_transform(transformed_data)\n```\n\n## License\n\nCytotransform is licensed under the MIT license, is free to use, and comes with no warranty whatsoever.\n',
     'author': 'Ross Burton',
     'author_email': 'burtonrossj@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cytotransform-0.2.11/PKG-INFO` & `cytotransform-0.2.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cytotransform
-Version: 0.2.11
+Version: 0.2.12
 Summary: Rapid transformations for cytometry data
 License: MIT
 Author: Ross Burton
 Author-email: burtonrossj@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.17.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: setuptools (>=67.7.1,<68.0.0)
 Description-Content-Type: text/markdown
 
 # Cytotransfrom
```

