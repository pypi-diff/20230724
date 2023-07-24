# Comparing `tmp/atbu-common-pkg-0.0.7.tar.gz` & `tmp/atbu-common-pkg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atbu-common-pkg-0.0.7.tar", last modified: Mon Jul 24 12:08:37 2023, max compression
+gzip compressed data, was "atbu-common-pkg-0.0.8.tar", last modified: Mon Jul 24 20:35:04 2023, max compression
```

## Comparing `atbu-common-pkg-0.0.7.tar` & `atbu-common-pkg-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.260083 atbu-common-pkg-0.0.7/
--rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2419 2023-07-24 12:08:37.259094 atbu-common-pkg-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.7/README.md
--rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 12:08:37.260083 atbu-common-pkg-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1782 2023-07-24 12:01:38.000000 atbu-common-pkg-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.197087 atbu-common-pkg-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.196092 atbu-common-pkg-0.0.7/src/atbu/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.225083 atbu-common-pkg-0.0.7/src/atbu/common/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/src/atbu/common/__init__.py
--rw-rw-rw-   0        0        0     6142 2022-06-08 21:42:34.000000 atbu-common-pkg-0.0.7/src/atbu/common/aes_cbc.py
--rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.7/src/atbu/common/exception.py
--rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.7/src/atbu/common/hasher.py
--rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/src/atbu/common/multi_json_enc_dec.py
--rw-rw-rw-   0        0        0     3946 2022-07-26 01:57:07.000000 atbu-common-pkg-0.0.7/src/atbu/common/profile.py
--rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/src/atbu/common/simple_report.py
--rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/src/atbu/common/singleton.py
--rw-rw-rw-   0        0        0    10618 2023-07-24 11:21:50.000000 atbu-common-pkg-0.0.7/src/atbu/common/util_helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.255088 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/
--rw-rw-rw-   0        0        0     2419 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.257082 atbu-common-pkg-0.0.7/tests/
--rw-rw-rw-   0        0        0     3282 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/tests/test_enc_dec.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.678740 atbu-common-pkg-0.0.8/
+-rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2419 2023-07-24 20:35:04.677754 atbu-common-pkg-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.8/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 20:35:04.679737 atbu-common-pkg-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1782 2023-07-24 20:23:22.000000 atbu-common-pkg-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.609738 atbu-common-pkg-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.608738 atbu-common-pkg-0.0.8/src/atbu/
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.641739 atbu-common-pkg-0.0.8/src/atbu/common/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.8/src/atbu/common/__init__.py
+-rw-rw-rw-   0        0        0     6142 2023-07-24 20:12:02.000000 atbu-common-pkg-0.0.8/src/atbu/common/aes_cbc.py
+-rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.8/src/atbu/common/exception.py
+-rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.8/src/atbu/common/hasher.py
+-rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.8/src/atbu/common/multi_json_enc_dec.py
+-rw-rw-rw-   0        0        0     3946 2023-07-24 20:12:02.000000 atbu-common-pkg-0.0.8/src/atbu/common/profile.py
+-rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.8/src/atbu/common/simple_report.py
+-rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.8/src/atbu/common/singleton.py
+-rw-rw-rw-   0        0        0    10618 2023-07-24 20:13:22.000000 atbu-common-pkg-0.0.8/src/atbu/common/util_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.673737 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/
+-rw-rw-rw-   0        0        0     2419 2023-07-24 20:35:04.000000 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-24 20:35:04.000000 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 20:35:04.000000 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-24 20:35:04.000000 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 20:35:04.000000 atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 20:35:04.675739 atbu-common-pkg-0.0.8/tests/
+-rw-rw-rw-   0        0        0     3282 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.8/tests/test_enc_dec.py
```

### Comparing `atbu-common-pkg-0.0.7/LICENSE` & `atbu-common-pkg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/PKG-INFO` & `atbu-common-pkg-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.7
+Version: 0.0.8
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-common-pkg-0.0.7/README.md` & `atbu-common-pkg-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/setup.py` & `atbu-common-pkg-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="atbu-common-pkg",
-    version="0.0.7",
+    version="0.0.8",
     author="Ashley R. Thomas",
     author_email="ashley.r.thomas.701@gmail.com",
     description= (
         "ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/aes_cbc.py` & `atbu-common-pkg-0.0.8/src/atbu/common/aes_cbc.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/exception.py` & `atbu-common-pkg-0.0.8/src/atbu/common/exception.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/hasher.py` & `atbu-common-pkg-0.0.8/src/atbu/common/hasher.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/multi_json_enc_dec.py` & `atbu-common-pkg-0.0.8/src/atbu/common/multi_json_enc_dec.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/profile.py` & `atbu-common-pkg-0.0.8/src/atbu/common/profile.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/simple_report.py` & `atbu-common-pkg-0.0.8/src/atbu/common/simple_report.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/singleton.py` & `atbu-common-pkg-0.0.8/src/atbu/common/singleton.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/src/atbu/common/util_helpers.py` & `atbu-common-pkg-0.0.8/src/atbu/common/util_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 def clear_file(fileobj: Union[io.IOBase, str, Path], byte_pattern: list[int] = None):
     """This should not be considered secure as it
     cannot guarantee filesystem buffering anomalies.
     """
     if isinstance(fileobj, str):
         fileobj = Path(fileobj)
     if isinstance(fileobj, Path):
-        fileobj = fileobj.open("w+b")
+        fileobj = fileobj.open("r+b")
     if not isinstance(fileobj, io.IOBase):
         raise InvalidFunctionArgument(
             f"Expecting io.IOBase derived fileobj, str path, or Path object."
         )
     if byte_pattern is None:
         byte_pattern = [0xCC, 0x55, 0x00]
     fileobj.seek(0, SEEK_END)
```

### Comparing `atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/PKG-INFO` & `atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.7
+Version: 0.0.8
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/SOURCES.txt` & `atbu-common-pkg-0.0.8/src/atbu_common_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.7/tests/test_enc_dec.py` & `atbu-common-pkg-0.0.8/tests/test_enc_dec.py`

 * *Files identical despite different names*

