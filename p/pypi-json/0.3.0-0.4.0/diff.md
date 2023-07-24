# Comparing `tmp/pypi_json-0.3.0.tar.gz` & `tmp/pypi_json-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_json-0.3.0.tar", last modified: Fri Jul  8 08:43:16 2022, max compression
+gzip compressed data, was "pypi_json-0.4.0.tar", last modified: Mon Jul 24 09:18:49 2023, max compression
```

## Comparing `pypi_json-0.3.0.tar` & `pypi_json-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     6550 2022-07-08 08:43:16.858957 pypi_json-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-07-08 08:43:16.854957 pypi_json-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-07-08 08:43:16.850957 pypi_json-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-07-08 08:43:16.854957 pypi_json-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-08 08:43:16.854957 pypi_json-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 08:42:43.958382 pypi_json-0.3.0/pypi_json/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5992 2022-07-08 08:42:43.958382 pypi_json-0.3.0/pypi_json/typehints.py
--rw-r--r--   0 runner    (1001) docker     (121)    11418 2022-07-08 08:42:43.958382 pypi_json-0.3.0/pypi_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-24 09:18:49.092639 pypi_json-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-24 09:18:49.100639 pypi_json-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-07-24 09:18:49.100639 pypi_json-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-07-24 09:18:49.100639 pypi_json-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4647 2023-07-24 09:18:49.096639 pypi_json-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    11443 2023-07-24 09:18:05.271532 pypi_json-0.4.0/pypi_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 09:18:05.271532 pypi_json-0.4.0/pypi_json/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5996 2023-07-24 09:18:05.271532 pypi_json-0.4.0/pypi_json/typehints.py
```

### Comparing `pypi_json-0.3.0/PKG-INFO` & `pypi_json-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-json
-Version: 0.3.0
+Version: 0.4.0
 Summary: PyPI JSON API client library
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: json,packaging,pypi,warehouse
 Home-page: https://github.com/repo-helper/pypi-json
 Project-URL: Issue Tracker, https://github.com/repo-helper/pypi-json/issues
 Project-URL: Source Code, https://github.com/repo-helper/pypi-json
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: apeye>=1.1.0
 Requires-Dist: packaging>=21.0
@@ -90,16 +91,16 @@
 	:target: https://github.com/repo-helper/pypi-json/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pypi-json/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pypi-json/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pypi-json/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pypi-json/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pypi-json/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pypi-json/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/pypi-json/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/pypi-json?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pypi-json?logo=codefactor
@@ -133,23 +134,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pypi-json
 	:target: https://github.com/repo-helper/pypi-json/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pypi-json
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pypi-json/v0.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pypi-json/v0.4.0
 	:target: https://github.com/repo-helper/pypi-json/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pypi-json
 	:target: https://github.com/repo-helper/pypi-json/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pypi-json
 	:target: https://pypi.org/project/pypi-json/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pypi_json-0.3.0/pyproject.toml` & `pypi_json-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "pypi-json"
-version = "0.3.0"
+version = "0.4.0"
 description = "PyPI JSON API client library"
 readme = "README.rst"
 keywords = [ "json", "packaging", "pypi", "warehouse",]
 dynamic = []
 dependencies = [ "apeye>=1.1.0", "packaging>=21.0", "requests>=2.26.0",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -133,22 +134,22 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "pypi_json"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `pypi_json-0.3.0/LICENSE` & `pypi_json-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_json-0.3.0/README.rst` & `pypi_json-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/repo-helper/pypi-json/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pypi-json/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pypi-json/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pypi-json/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pypi-json/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pypi-json/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pypi-json/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/pypi-json/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/pypi-json?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pypi-json?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pypi-json
 	:target: https://github.com/repo-helper/pypi-json/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pypi-json
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pypi-json/v0.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pypi-json/v0.4.0
 	:target: https://github.com/repo-helper/pypi-json/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pypi-json
 	:target: https://github.com/repo-helper/pypi-json/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pypi-json
 	:target: https://pypi.org/project/pypi-json/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pypi_json-0.3.0/pypi_json/typehints.py` & `pypi_json-0.4.0/pypi_json/typehints.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 
 	#: Deprecated
 	downloads: int
 
 	#: The basename of the package file (including extension).
 	filename: str
 
-	#: Whether the package file is accompanied by a PGP signature file.
-	has_sig: bool
+	# #: Whether the package file is accompanied by a PGP signature file.
+	# has_sig: bool
 
 	#: Deprecated
 	md5_digest: str
 
 	packagetype: str
 	"""
 	The distribution package type.
```

### Comparing `pypi_json-0.3.0/pypi_json/__init__.py` & `pypi_json-0.4.0/pypi_json/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,36 +30,37 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import platform
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, NamedTuple, Optional, Tuple, Union
-from urllib.parse import urlparse, urlunparse
 
 # 3rd party
 import requests
 from apeye import URL
 from apeye.requests_url import RequestsURL, TrailingRequestsURL
 from packaging.requirements import InvalidRequirement
 from packaging.tags import Tag
 from packaging.utils import canonicalize_name, parse_wheel_filename
 from packaging.version import Version
 
 # this package
 from pypi_json.typehints import DistributionPackageDict, FileURL, ProjectInfoDict, Self, VulnerabilityInfoDict
 
+# from urllib.parse import urlparse, urlunparse
+
 if TYPE_CHECKING:
 	# stdlib
 	from typing import NoReturn
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.3.0"
+__version__: str = "0.4.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PyPIJSON", "ProjectMetadata", "USER_AGENT"]
 
 #: The User-Agent header used for requests; not used when the user provides their own session object.
 USER_AGENT: str = ' '.join([
 		f"pypi-json/{__version__} (https://github.com/repo-helper/pypi-json)",
@@ -356,22 +357,22 @@
 		"""
 
 		if isinstance(url, URL):
 			url = str(url)
 
 		return self.endpoint.session.get(url)
 
-	@staticmethod
-	def get_signature_url(download_url: Union[str, URL]) -> str:
-		"""
-		Returns the URL of the PGP signature for the download URL.
+	# @staticmethod
+	# def get_signature_url(download_url: Union[str, URL]) -> str:
+	# 	"""
+	# 	Returns the URL of the PGP signature for the download URL.
 
-		A file only has a PGP signature if it's ``has_sig`` key is :py:obj:`True`.
+	# 	A file only has a PGP signature if it's ``has_sig`` key is :py:obj:`True`.
 
-		:param download_url:
-		"""
+	# 	:param download_url:
+	# 	"""
 
-		if isinstance(download_url, URL):
-			download_url = str(download_url)
+	# 	if isinstance(download_url, URL):
+	# 		download_url = str(download_url)
 
-		u = urlparse(download_url)
-		return urlunparse((u[0], u[1], u[2] + ".asc", '', '', ''))
+	# 	u = urlparse(download_url)
+	# 	return urlunparse((u[0], u[1], u[2] + ".asc", '', '', ''))
```

