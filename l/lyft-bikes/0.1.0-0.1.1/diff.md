# Comparing `tmp/lyft_bikes-0.1.0.tar.gz` & `tmp/lyft_bikes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyft_bikes-0.1.0.tar", max compression
+gzip compressed data, was "lyft_bikes-0.1.1.tar", max compression
```

## Comparing `lyft_bikes-0.1.0.tar` & `lyft_bikes-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-03-04 10:14:26.958194 lyft_bikes-0.1.0/LICENSE
--rw-r--r--   0        0        0      990 2023-07-24 06:49:31.289367 lyft_bikes-0.1.0/README.md
--rw-r--r--   0        0        0     3034 2023-07-24 06:49:31.292843 lyft_bikes-0.1.0/lyft_bikes/__init__.py
--rw-r--r--   0        0        0      467 2023-07-24 06:49:31.292955 lyft_bikes-0.1.0/lyft_bikes/bikes.py
--rw-r--r--   0        0        0      653 2023-07-24 06:49:31.293047 lyft_bikes-0.1.0/lyft_bikes/geo/__init__.py
--rw-r--r--   0        0        0     1474 2023-07-24 06:49:31.293116 lyft_bikes-0.1.0/lyft_bikes/geo/fees.geojson
--rw-r--r--   0        0        0        0 2023-07-24 06:49:31.293158 lyft_bikes-0.1.0/lyft_bikes/historical/__init__.py
--rw-r--r--   0        0        0     2141 2023-07-24 06:49:31.293318 lyft_bikes-0.1.0/lyft_bikes/historical/dates.py
--rw-r--r--   0        0        0     3556 2023-07-24 06:49:31.293438 lyft_bikes-0.1.0/lyft_bikes/historical/downloader.py
--rw-r--r--   0        0        0     2553 2023-07-24 06:49:31.293568 lyft_bikes-0.1.0/lyft_bikes/historical/historical.py
--rw-r--r--   0        0        0     1245 2023-07-24 06:49:31.293682 lyft_bikes-0.1.0/lyft_bikes/live.py
--rw-r--r--   0        0        0     1583 2023-07-24 06:49:31.293797 lyft_bikes-0.1.0/lyft_bikes/pricing.py
--rw-r--r--   0        0        0        0 2023-07-24 06:49:31.293829 lyft_bikes-0.1.0/lyft_bikes/py.typed
--rw-r--r--   0        0        0      380 2023-07-24 06:49:31.293945 lyft_bikes-0.1.0/lyft_bikes/stations.py
--rw-r--r--   0        0        0     1437 2023-07-24 06:49:31.295183 lyft_bikes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1881 1970-01-01 00:00:00.000000 lyft_bikes-0.1.0/setup.py
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 lyft_bikes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-04 10:14:26.958194 lyft_bikes-0.1.1/LICENSE
+-rw-r--r--   0        0        0      990 2023-07-24 06:49:31.289367 lyft_bikes-0.1.1/README.md
+-rw-r--r--   0        0        0     3034 2023-07-24 06:49:31.292843 lyft_bikes-0.1.1/lyft_bikes/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-24 06:49:31.292955 lyft_bikes-0.1.1/lyft_bikes/bikes.py
+-rw-r--r--   0        0        0      653 2023-07-24 06:49:31.293047 lyft_bikes-0.1.1/lyft_bikes/geo/__init__.py
+-rw-r--r--   0        0        0     1474 2023-07-24 06:49:31.293116 lyft_bikes-0.1.1/lyft_bikes/geo/fees.geojson
+-rw-r--r--   0        0        0        0 2023-07-24 06:49:31.293158 lyft_bikes-0.1.1/lyft_bikes/historical/__init__.py
+-rw-r--r--   0        0        0     2141 2023-07-24 06:49:31.293318 lyft_bikes-0.1.1/lyft_bikes/historical/dates.py
+-rw-r--r--   0        0        0     3556 2023-07-24 06:49:31.293438 lyft_bikes-0.1.1/lyft_bikes/historical/downloader.py
+-rw-r--r--   0        0        0     2553 2023-07-24 06:49:31.293568 lyft_bikes-0.1.1/lyft_bikes/historical/historical.py
+-rw-r--r--   0        0        0     1245 2023-07-24 06:49:31.293682 lyft_bikes-0.1.1/lyft_bikes/live.py
+-rw-r--r--   0        0        0     1583 2023-07-24 06:49:31.293797 lyft_bikes-0.1.1/lyft_bikes/pricing.py
+-rw-r--r--   0        0        0        0 2023-07-24 06:49:31.293829 lyft_bikes-0.1.1/lyft_bikes/py.typed
+-rw-r--r--   0        0        0      380 2023-07-24 06:49:31.293945 lyft_bikes-0.1.1/lyft_bikes/stations.py
+-rw-r--r--   0        0        0     1393 2023-07-24 06:57:09.655151 lyft_bikes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 lyft_bikes-0.1.1/setup.py
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 lyft_bikes-0.1.1/PKG-INFO
```

### Comparing `lyft_bikes-0.1.0/LICENSE` & `lyft_bikes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/README.md` & `lyft_bikes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/__init__.py` & `lyft_bikes-0.1.1/lyft_bikes/__init__.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/geo/__init__.py` & `lyft_bikes-0.1.1/lyft_bikes/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/geo/fees.geojson` & `lyft_bikes-0.1.1/lyft_bikes/geo/fees.geojson`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/historical/dates.py` & `lyft_bikes-0.1.1/lyft_bikes/historical/dates.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/historical/downloader.py` & `lyft_bikes-0.1.1/lyft_bikes/historical/downloader.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/historical/historical.py` & `lyft_bikes-0.1.1/lyft_bikes/historical/historical.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/live.py` & `lyft_bikes-0.1.1/lyft_bikes/live.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/lyft_bikes/pricing.py` & `lyft_bikes-0.1.1/lyft_bikes/pricing.py`

 * *Files identical despite different names*

### Comparing `lyft_bikes-0.1.0/pyproject.toml` & `lyft_bikes-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "lyft-bikes"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python Client for Lyft Bike Sharing Data."
 authors = ["Will Dean <wd60622@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://wd60622.github.io/divvy/"
-documentation = "https://wd60622.github.io/divvy/"
-repository = "https://github.com/wd60622/divvy/"
+homepage = "https://wd60622.github.io/lyft-bikes/"
+documentation = "https://wd60622.github.io/lyft-bikes/"
+repository = "https://github.com/wd60622/lyft-bikes/"
 packages = [
     { include = "lyft_bikes" },
     { include = "lyft_bikes/py.typed" },
     { include = "lyft_bikes/geo/*" }, 
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -25,20 +25,18 @@
     "Operating System :: MacOS",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pandas = "*"
 requests = "*"
-lxml = { version = "*", optional = true }
 geopandas = { version = "*", optional = true}
 
 [tool.poetry.extras]
 boundary = ["geopandas"]
-index = ["lxml"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 ipython = "8.8.0"
 matplotlib = "^3.7.2"
```

### Comparing `lyft_bikes-0.1.0/setup.py` & `lyft_bikes-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 modules = \
 ['py']
 install_requires = \
 ['pandas', 'requests']
 
 extras_require = \
-{'boundary': ['geopandas'], 'index': ['lxml']}
+{'boundary': ['geopandas']}
 
 setup_kwargs = {
     'name': 'lyft-bikes',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python Client for Lyft Bike Sharing Data.',
     'long_description': '# Lyft Bike Share Data\n\nPython client for Lyft bike share data.\n\n## Features \n\n- Support for [cities](https://www.lyft.com/bikes#cities) with Lyft bike share\n- [Historical trips](https://wd60622.github.io/lyft-bikes/examples/historical-trips/)\n- Live station and bike / scooter availability\n- [Applying pricing to trips](https://wd60622.github.io/lyft-bikes/examples/new-pricing/)\n    - Unlock Fees\n    - Minute Rates\n\n## Installation \n\nInstall from `pip` \n\n```shell \n$ pip install lyft-bikes\n```\n\n## Documentation\n\nThe documentation is hosted on [GitHub Pages](https://wd60622.github.io/lyft-bikes/).\n\n## Development\n\nThe development environment was created with [`poetry`](https://python-poetry.org/docs/). The `pyproject.toml` file is the main configuration file for the project.\n\n```bash\npoetry install . \n```\n\n## Contributing\n\nIf you would like to contribute or find some issue in the code, please [open an Issue](https://github.com/wd60622/divvy/issues/new) or a PR on GitHub. Thanks!',
     'author': 'Will Dean',
     'author_email': 'wd60622@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://wd60622.github.io/divvy/',
+    'url': 'https://wd60622.github.io/lyft-bikes/',
     'packages': packages,
     'package_data': package_data,
     'py_modules': modules,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `lyft_bikes-0.1.0/PKG-INFO` & `lyft_bikes-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lyft-bikes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Client for Lyft Bike Sharing Data.
-Home-page: https://wd60622.github.io/divvy/
+Home-page: https://wd60622.github.io/lyft-bikes/
 License: MIT
 Author: Will Dean
 Author-email: wd60622@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -19,21 +19,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: boundary
-Provides-Extra: index
 Requires-Dist: geopandas; extra == "boundary"
-Requires-Dist: lxml; extra == "index"
 Requires-Dist: pandas
 Requires-Dist: requests
-Project-URL: Documentation, https://wd60622.github.io/divvy/
-Project-URL: Repository, https://github.com/wd60622/divvy/
+Project-URL: Documentation, https://wd60622.github.io/lyft-bikes/
+Project-URL: Repository, https://github.com/wd60622/lyft-bikes/
 Description-Content-Type: text/markdown
 
 # Lyft Bike Share Data
 
 Python client for Lyft bike share data.
 
 ## Features
```

