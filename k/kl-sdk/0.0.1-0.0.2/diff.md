# Comparing `tmp/kl_sdk-0.0.1.tar.gz` & `tmp/kl_sdk-0.0.2.tar.gz`

## Comparing `kl_sdk-0.0.1.tar` & `kl_sdk-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/src/killbills_sdk/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/src/killbills_sdk/cryptoService.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/src/killbills_sdk/example.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/src/killbills_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/src/killbills_sdk/validatorService.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kl_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/cryptoService.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/example.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/validatorService.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/PKG-INFO
```

### Comparing `kl_sdk-0.0.1/src/killbills_sdk/sendDataWithHmac.py` & `kl_sdk-0.0.2/src/kl_sdk/sendDataWithHmac.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.1/src/killbills_sdk/validatorService.py` & `kl_sdk-0.0.2/src/kl_sdk/validatorService.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.1/.gitignore` & `kl_sdk-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.1/LICENSE` & `kl_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.1/pyproject.toml` & `kl_sdk-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kl_sdk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `kl_sdk-0.0.1/PKG-INFO` & `kl_sdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kl_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: KillBills e-receipt sdk
 Project-URL: Homepage, https://github.com/killbillsdev/killbills-sdk-python
 Project-URL: Bug Tracker, https://github.com/killbillsdev/killbills-sdk-python/issues
 Author-email: killbillsdev <cto@killbills.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

