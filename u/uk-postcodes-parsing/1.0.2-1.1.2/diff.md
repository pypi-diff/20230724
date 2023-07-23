# Comparing `tmp/uk_postcodes_parsing-1.0.2.tar.gz` & `tmp/uk_postcodes_parsing-1.1.2.tar.gz`

## Comparing `uk_postcodes_parsing-1.0.2.tar` & `uk_postcodes_parsing-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcodes_nov_2022.py
--rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/LICENSE
--rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0   109947 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/scripts/process_onspd.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0 20568480 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/postcodes_may_2023.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/LICENSE
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.1.2/PKG-INFO
```

### Comparing `uk_postcodes_parsing-1.0.2/.pre-commit-config.yaml` & `uk_postcodes_parsing-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/.github/workflows/test.yml` & `uk_postcodes_parsing-1.1.2/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         run: |
           python -m pip install --upgrade pip
           pip install .
           pip install black pytest pandas
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint check with black
         run: |
-          black src/uk_postcodes_parsing/ --check --exclude src/uk_postcodes_parsing/postcodes_nov_2022.py
+          black src/uk_postcodes_parsing/ --check --exclude src/uk_postcodes_parsing/postcodes_may_2023.py
       - name: Test with pytest
         run: |
           pytest -v
```

### Comparing `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 postcode_utils.py: Utilities for working with postcodes.
 """
 import re
 from typing import Union
 
-from uk_postcodes_parsing.postcodes_nov_2022 import POSTCODE_NOV_2022
-
 
 # Tests for district
 DISTRICT_SPLIT_REGEX = re.compile(r"^([a-z]{1,2}\d)([a-z])$", re.I)
 
 # Tests for the unit section of a postcode
 UNIT_REGEX = re.compile(r"[a-z]{2}$", re.I)
```

### Comparing `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-1.1.2/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     to_area,
     to_sector,
     to_unit,
     to_district,
     to_sub_district,
 )
 from uk_postcodes_parsing.fix import fix, fix_with_options
-from uk_postcodes_parsing.postcodes_nov_2022 import POSTCODE_NOV_2022
+from uk_postcodes_parsing.postcodes_may_2023 import POSTCODE_MAY_2023
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("uk-postcodes-parsing.ukpostcode")
 
 # Test for a valid postcode embedded in text
 POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
     r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}", re.I
 )
 
 SPECIAL_CASE_POSTCODES = ("GIR", "NPT", "BX", "BF")
 
-logger.debug("Imported POSTCODE_NOV_2022 with length: %s", len(POSTCODE_NOV_2022))
+logger.debug("Imported POSTCODE_NOV_2022 with length: %s", len(POSTCODE_MAY_2023))
 
 
 @dataclass(order=True)
 class Postcode:
     """Class to hold the parsed postcode.
     Constructor arguments:
         original (str): The raw (original) string of the postcode.
@@ -206,8 +206,8 @@
 
     Args:
         postcode (str): The postcode to check
 
     Returns:
         bool: True if the postcode is valid, False otherwise
     """
-    return postcode in POSTCODE_NOV_2022
+    return postcode in POSTCODE_MAY_2023
```

### Comparing `uk_postcodes_parsing-1.0.2/tests/test_all.py` & `uk_postcodes_parsing-1.1.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/.gitignore` & `uk_postcodes_parsing-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/LICENSE` & `uk_postcodes_parsing-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.2/README.md` & `uk_postcodes_parsing-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 | A9 9AA   | A9       | 9AA     | A     | A9        | `None`       | A9 9    | AA    |
 | A99 9AA  | A99      | 9AA     | A     | A99       | `None`       | A99 9   | AA    |
 | AA9 9AA  | AA9      | 9AA     | AA    | AA9       | `None`       | AA9 9   | AA    |
 | AA99 9AA | AA99     | 9AA     | AA    | AA99      | `None`       | AA99 9  | AA    |
 
 
 - Utilities to validate postcode
-- NEW: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory (Nov 2022)
+- Updated to May 2023: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory
 
 
 ## Usage
 
 - Parsing text to get a list of postcodes.
 
 ```python
@@ -183,10 +183,15 @@
 
 # Testing
 
 ```bash
 pytest tests/
 ```
 
+# Updating this library with newer version of ONS postcode directory
+
+This library has been updated with May 2023 ONS postcode directory. To update this to a newer, version, see: [process_onspd.ipynb](scripts/process_onspd.ipynb).
+
+
 ## Similar work
 
 This package started as a Python replica of the postcode.io JavaScript library: https://github.com/ideal-postcodes/postcode
```

### Comparing `uk_postcodes_parsing-1.0.2/pyproject.toml` & `uk_postcodes_parsing-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "1.0.2"
+version = "1.1.2"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
 description = "A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `uk_postcodes_parsing-1.0.2/PKG-INFO` & `uk_postcodes_parsing-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 1.0.2
+Version: 1.1.2
 Summary: A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 | A9 9AA   | A9       | 9AA     | A     | A9        | `None`       | A9 9    | AA    |
 | A99 9AA  | A99      | 9AA     | A     | A99       | `None`       | A99 9   | AA    |
 | AA9 9AA  | AA9      | 9AA     | AA    | AA9       | `None`       | AA9 9   | AA    |
 | AA99 9AA | AA99     | 9AA     | AA    | AA99      | `None`       | AA99 9  | AA    |
 
 
 - Utilities to validate postcode
-- NEW: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory (Nov 2022)
+- Updated to May 2023: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory
 
 
 ## Usage
 
 - Parsing text to get a list of postcodes.
 
 ```python
@@ -203,10 +203,15 @@
 
 # Testing
 
 ```bash
 pytest tests/
 ```
 
+# Updating this library with newer version of ONS postcode directory
+
+This library has been updated with May 2023 ONS postcode directory. To update this to a newer, version, see: [process_onspd.ipynb](scripts/process_onspd.ipynb).
+
+
 ## Similar work
 
 This package started as a Python replica of the postcode.io JavaScript library: https://github.com/ideal-postcodes/postcode
```

