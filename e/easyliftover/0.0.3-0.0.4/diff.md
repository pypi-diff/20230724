# Comparing `tmp/easyliftover-0.0.3.tar.gz` & `tmp/easyliftover-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyliftover-0.0.3.tar", max compression
+gzip compressed data, was "easyliftover-0.0.4.tar", max compression
```

## Comparing `easyliftover-0.0.3.tar` & `easyliftover-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2023-07-24 07:58:03.872847 easyliftover-0.0.3/LICENSE
--rw-r--r--   0        0        0      459 2023-07-24 07:58:03.872847 easyliftover-0.0.3/README.md
--rw-r--r--   0        0        0       67 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/__init__.py
--rw-r--r--   0        0        0      189 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/genomes.py
--rw-r--r--   0        0        0      117 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/lifters/__init__.py
--rw-r--r--   0        0        0     1931 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/lifters/abstract.py
--rw-r--r--   0        0        0      680 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/lifters/bed.py
--rw-r--r--   0        0        0      661 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/lifters/gff.py
--rw-r--r--   0        0        0       62 2023-07-24 07:58:04.792845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/.git
--rw-r--r--   0        0        0      303 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/.gitignore
--rw-r--r--   0        0        0      139 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/.travis.yml
--rw-r--r--   0        0        0      416 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/CHANGELOG.txt
--rw-r--r--   0        0        0     1064 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/LICENSE
--rw-r--r--   0        0        0       32 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/MANIFEST.in
--rw-r--r--   0        0        0     2670 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/README.rst
--rw-r--r--   0        0        0     1661 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/__init__.py
--rw-r--r--   0        0        0    11116 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/chainfile.py
--rw-r--r--   0        0        0     6795 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py
--rw-r--r--   0        0        0     5516 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/liftover.py
--rw-r--r--   0        0        0      178 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/setup.cfg
--rw-r--r--   0        0        0     1972 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/setup.py
--rw-r--r--   0        0        0      210 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/__init__.py
--rw-r--r--   0        0        0     3756 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/chainfile_test.py
--rw-r--r--   0        0        0      299 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/README.txt
--rw-r--r--   0        0        0    85433 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz
--rw-r--r--   0        0        0    68588 2023-07-24 07:58:04.800845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz
--rw-r--r--   0        0        0  1246411 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz
--rw-r--r--   0        0        0      818 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt
--rw-r--r--   0        0        0      523 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt
--rw-r--r--   0        0        0      902 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver
--rw-r--r--   0        0        0     1247 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/intervaltree_test.py
--rw-r--r--   0        0        0     3618 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/liftover_test.py
--rw-r--r--   0        0        0     3952 2023-07-24 07:58:04.804845 easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py
--rw-r--r--   0        0        0     1825 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/lifters/wig.py
--rw-r--r--   0        0        0      573 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/targets.py
--rw-r--r--   0        0        0     1231 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/types.json
--rw-r--r--   0        0        0     1655 2023-07-24 07:58:03.872847 easyliftover-0.0.3/easyliftover/uplift.py
--rw-r--r--   0        0        0      685 2023-07-24 07:58:03.872847 easyliftover-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 easyliftover-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 12:36:52.596630 easyliftover-0.0.4/LICENSE
+-rw-r--r--   0        0        0      459 2023-07-24 12:36:52.596630 easyliftover-0.0.4/README.md
+-rw-r--r--   0        0        0       67 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/genomes.py
+-rw-r--r--   0        0        0      117 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/lifters/__init__.py
+-rw-r--r--   0        0        0     1931 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/lifters/abstract.py
+-rw-r--r--   0        0        0      680 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/lifters/bed.py
+-rw-r--r--   0        0        0      661 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/lifters/gff.py
+-rw-r--r--   0        0        0       62 2023-07-24 12:36:53.412636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/.git
+-rw-r--r--   0        0        0      303 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/.gitignore
+-rw-r--r--   0        0        0      139 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/.travis.yml
+-rw-r--r--   0        0        0      416 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/CHANGELOG.txt
+-rw-r--r--   0        0        0     1064 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/LICENSE
+-rw-r--r--   0        0        0       32 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/MANIFEST.in
+-rw-r--r--   0        0        0     2670 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/README.rst
+-rw-r--r--   0        0        0     1661 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/__init__.py
+-rw-r--r--   0        0        0    11116 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/chainfile.py
+-rw-r--r--   0        0        0     6795 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py
+-rw-r--r--   0        0        0     5516 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/liftover.py
+-rw-r--r--   0        0        0      178 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/setup.cfg
+-rw-r--r--   0        0        0     1972 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/setup.py
+-rw-r--r--   0        0        0      210 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/__init__.py
+-rw-r--r--   0        0        0     3756 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/chainfile_test.py
+-rw-r--r--   0        0        0      299 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/README.txt
+-rw-r--r--   0        0        0    85433 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz
+-rw-r--r--   0        0        0    68588 2023-07-24 12:36:53.420636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz
+-rw-r--r--   0        0        0  1246411 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz
+-rw-r--r--   0        0        0      818 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt
+-rw-r--r--   0        0        0      523 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt
+-rw-r--r--   0        0        0      902 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver
+-rw-r--r--   0        0        0     1247 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/intervaltree_test.py
+-rw-r--r--   0        0        0     3618 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/liftover_test.py
+-rw-r--r--   0        0        0     3952 2023-07-24 12:36:53.424636 easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py
+-rw-r--r--   0        0        0     1825 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/lifters/wig.py
+-rw-r--r--   0        0        0      573 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/targets.py
+-rw-r--r--   0        0        0     1231 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/types.json
+-rw-r--r--   0        0        0     1655 2023-07-24 12:36:52.596630 easyliftover-0.0.4/easyliftover/uplift.py
+-rw-r--r--   0        0        0      707 2023-07-24 12:36:52.596630 easyliftover-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 easyliftover-0.0.4/PKG-INFO
```

### Comparing `easyliftover-0.0.3/LICENSE` & `easyliftover-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/abstract.py` & `easyliftover-0.0.4/easyliftover/lifters/abstract.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/bed.py` & `easyliftover-0.0.4/easyliftover/lifters/bed.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/gff.py` & `easyliftover-0.0.4/easyliftover/lifters/gff.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/LICENSE` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/LICENSE`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/README.rst` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/README.rst`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/__init__.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/__init__.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/chainfile.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/chainfile.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/pyliftover/liftover.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/pyliftover/liftover.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/setup.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/setup.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/chainfile_test.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/chainfile_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/intervaltree_test.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/intervaltree_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/liftover_test.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/liftover_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py` & `easyliftover-0.0.4/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/lifters/wig.py` & `easyliftover-0.0.4/easyliftover/lifters/wig.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/targets.py` & `easyliftover-0.0.4/easyliftover/targets.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/types.json` & `easyliftover-0.0.4/easyliftover/types.json`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/easyliftover/uplift.py` & `easyliftover-0.0.4/easyliftover/uplift.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.3/pyproject.toml` & `easyliftover-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "easyliftover"
-version = "0.0.3"
+version = "0.0.4"
 description = "A python package for lifting over biological files"
 license = "MIT"
 authors = ["Nico Trummer <nictru32@gmail.com>"]
 repository = "https://github.com/biomedbigdata/easyUplift"
 homepage = "https://github.com/biomedbigdata/easyUplift"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1"
+python = ">=3.9"
 requests = "^2.26.0"
 beautifulsoup4 = "^4.9.3"
+pyodide-http = "^0.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 pytest-cov = "^2.12.1"
 flake8 = "^6.0.0"
 
 [tool.pytest.ini_options]
```

### Comparing `easyliftover-0.0.3/PKG-INFO` & `easyliftover-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: easyliftover
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for lifting over biological files
 Home-page: https://github.com/biomedbigdata/easyUplift
 License: MIT
 Author: Nico Trummer
 Author-email: nictru32@gmail.com
-Requires-Python: >=3.8.1
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
+Requires-Dist: pyodide-http (>=0.2.1,<0.3.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/biomedbigdata/easyUplift
 Description-Content-Type: text/markdown
 
 # easy-liftover
 
 This repository wraps the [pyliftover](https://pypi.org/project/pyliftover/) package to provide an option for uplifting whole files.
```

