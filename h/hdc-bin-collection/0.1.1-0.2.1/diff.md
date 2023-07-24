# Comparing `tmp/hdc_bin_collection-0.1.1.tar.gz` & `tmp/hdc_bin_collection-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdc_bin_collection-0.1.1.tar", max compression
+gzip compressed data, was "hdc_bin_collection-0.2.1.tar", max compression
```

## Comparing `hdc_bin_collection-0.1.1.tar` & `hdc_bin_collection-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1069 2022-04-08 21:16:26.764162 hdc_bin_collection-0.1.1/LICENSE
--rw-r--r--   0        0        0      235 2022-04-08 21:44:43.553391 hdc_bin_collection-0.1.1/README.md
--rw-r--r--   0        0        0       45 2022-04-08 21:50:29.456248 hdc_bin_collection-0.1.1/hdc_bin_collection/__init__.py
--rw-r--r--   0        0        0     2049 2022-05-08 15:17:58.168542 hdc_bin_collection-0.1.1/hdc_bin_collection/hdc_bin_collection.py
--rw-r--r--   0        0        0      871 2022-05-08 15:38:32.958376 hdc_bin_collection-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1114 2022-05-08 15:39:03.215090 hdc_bin_collection-0.1.1/setup.py
--rw-r--r--   0        0        0     1092 2022-05-08 15:39:03.215313 hdc_bin_collection-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.2.1/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.2.1/README.md
+-rw-r--r--   0        0        0       45 2023-07-24 18:28:19.170044 hdc_bin_collection-0.2.1/hdc_bin_collection/__init__.py
+-rw-r--r--   0        0        0     7665 2023-07-24 19:07:07.873134 hdc_bin_collection-0.2.1/hdc_bin_collection/hdc_bin_collection.py
+-rw-r--r--   0        0        0      927 2023-07-24 19:07:20.205252 hdc_bin_collection-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 hdc_bin_collection-0.2.1/PKG-INFO
```

### Comparing `hdc_bin_collection-0.1.1/LICENSE` & `hdc_bin_collection-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.1.1/pyproject.toml` & `hdc_bin_collection-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdc_bin_collection"
-version = "0.1.1"
+version = "0.2.1"
 description = "A module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
 authors = ["Aaron Carson <aaron@aaroncarson.co.uk>"]
 keywords = ["hdc", "bin", "collection", "Market", "Harborough", "garbage", "trash", "rubbish", "recycling"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/caraar12345/hdc-bin-collection"
 include = ["LICENSE"]
@@ -18,13 +18,16 @@
 requests = "^2.27.1"
 aiohttp = "^3.8.1"
 asyncio = "^3.4.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+
 [tool.pyright]
 reportOptionalMemberAccess = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hdc_bin_collection-0.1.1/PKG-INFO` & `hdc_bin_collection-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: hdc-bin-collection
-Version: 0.1.1
+Version: 0.2.1
 Summary: A module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
 Home-page: https://github.com/caraar12345/hdc-bin-collection
 License: MIT
 Keywords: hdc,bin,collection,Market,Harborough,garbage,trash,rubbish,recycling
 Author: Aaron Carson
 Author-email: aaron@aaroncarson.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.0,<5.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Harborough District Council - Bin Collection Dates
```

