# Comparing `tmp/twinlab-1.1.4.tar.gz` & `tmp/twinlab-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.4.tar", max compression
+gzip compressed data, was "twinlab-1.1.5.tar", max compression
```

## Comparing `twinlab-1.1.4.tar` & `twinlab-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.4/LICENSE
--rw-r--r--   0        0        0     2037 2023-06-15 08:30:01.835810 twinlab-1.1.4/README.md
--rw-r--r--   0        0        0      932 2023-06-15 08:30:01.841314 twinlab-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      574 2023-06-15 08:30:01.844913 twinlab-1.1.4/twinlab/__init__.py
--rw-r--r--   0        0        0      130 2023-06-15 08:30:01.845288 twinlab-1.1.4/twinlab/_version.py
--rw-r--r--   0        0        0    13412 2023-06-15 08:30:01.845725 twinlab-1.1.4/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.4/twinlab/plotting.py
--rw-r--r--   0        0        0     1322 2023-06-15 08:30:01.846138 twinlab-1.1.4/twinlab/settings.py
--rw-r--r--   0        0        0     4777 2023-06-15 08:30:01.846448 twinlab-1.1.4/twinlab/utils.py
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 twinlab-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2038 2023-07-24 08:09:31.663734 twinlab-1.1.5/README.md
+-rw-r--r--   0        0        0      918 2023-07-24 15:42:01.456202 twinlab-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      574 2023-07-24 08:06:55.154794 twinlab-1.1.5/twinlab/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-24 08:06:55.155110 twinlab-1.1.5/twinlab/_version.py
+-rw-r--r--   0        0        0    13412 2023-07-24 08:06:55.155460 twinlab-1.1.5/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.5/twinlab/plotting.py
+-rw-r--r--   0        0        0     1322 2023-07-24 08:06:55.155767 twinlab-1.1.5/twinlab/settings.py
+-rw-r--r--   0        0        0     4928 2023-07-24 08:09:31.665511 twinlab-1.1.5/twinlab/utils.py
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 twinlab-1.1.5/PKG-INFO
```

### Comparing `twinlab-1.1.4/LICENSE` & `twinlab-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.4/README.md` & `twinlab-1.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ## Commands
 
 Testing:
 
 ```shell
 poetry run python scripts/test.py
 ```
-where `test.py` can be replaced with any of the scripts in the `script` directory.
+where `test.py` can be replaced with any of the scripts in the `scripts` directory.
 
 ## Example
 
 Here we create some mock data (which has a quadratic relationship between `X` and `y`) and use `twinLab` to create a surrogate model with quantified uncertainty.
 ```python
 # Import libraries
 import twinlab as tl
```

### Comparing `twinlab-1.1.4/pyproject.toml` & `twinlab-1.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.4"
+version = "1.1.5"
 description = "Client interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab-client"
 authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
@@ -13,19 +13,18 @@
     "Jordan Hart <jordan@digilab.co.uk>",
 ]
 keywords = ["machine-learning", "AI", "cloud", "twinLab", "digiLab"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
+numpy = "^1.25.1"
 pandas = "^1.5.3"
 pydantic = { version = "^1.10.7", extras = ["dotenv"] }
 requests = "^2.28.2"
-
-[tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 IPython = "^8.11"
 matplotlib = "^3.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `twinlab-1.1.4/twinlab/__init__.py` & `twinlab-1.1.5/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.4/twinlab/client.py` & `twinlab-1.1.5/twinlab/client.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.4/twinlab/settings.py` & `twinlab-1.1.5/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.4/twinlab/utils.py` & `twinlab-1.1.5/twinlab/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,21 @@
     print()
 
 
 def print_response_message(r: requests.Response) -> None:
     """
     Print response message
     """
-    print("Response:", json.loads(r.text)["message"])
+    response_text = r.text
+    try:
+        response_dict = json.loads(response_text)
+        message = response_dict["message"]
+    except:
+        message = response_text
+    print("Response:", message)
     print()
 
 
 def check_response(r: requests.Response) -> None:
     if r.status_code != 200:
         print("Status code:", r.status_code)
         print_response_message(r)
```

### Comparing `twinlab-1.1.4/PKG-INFO` & `twinlab-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.1.4
+Version: 1.1.5
 Summary: Client interface for twinLab machine-learning in the cloud.
 Home-page: https://www.digilab.co.uk/
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: DigiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
 Maintainer-email: alexander@digilab.co.uk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: IPython (>=8.11,<9.0)
+Requires-Dist: ipykernel (>=6.22.0,<7.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://digilab-ai.github.io/twinLab-client
 Project-URL: Repository, https://github.com/digiLab-ai/twinLab-client
 Description-Content-Type: text/markdown
 
@@ -58,15 +62,15 @@
 ## Commands
 
 Testing:
 
 ```shell
 poetry run python scripts/test.py
 ```
-where `test.py` can be replaced with any of the scripts in the `script` directory.
+where `test.py` can be replaced with any of the scripts in the `scripts` directory.
 
 ## Example
 
 Here we create some mock data (which has a quadratic relationship between `X` and `y`) and use `twinLab` to create a surrogate model with quantified uncertainty.
 ```python
 # Import libraries
 import twinlab as tl
```

