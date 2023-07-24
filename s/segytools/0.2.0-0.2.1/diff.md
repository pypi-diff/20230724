# Comparing `tmp/segytools-0.2.0.tar.gz` & `tmp/segytools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segytools-0.2.0.tar", max compression
+gzip compressed data, was "segytools-0.2.1.tar", max compression
```

## Comparing `segytools-0.2.0.tar` & `segytools-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.2.0/LICENSE
--rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.2.0/README.md
--rw-r--r--   0        0        0      870 2023-06-04 20:39:52.857422 segytools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      215 2023-02-04 10:18:01.553258 segytools-0.2.0/src/segytools/__init__.py
--rw-r--r--   0        0        0     1165 2023-01-29 16:40:13.789248 segytools-0.2.0/src/segytools/datatypes.py
--rw-r--r--   0        0        0     4192 2023-06-02 08:15:34.847622 segytools-0.2.0/src/segytools/segy_abstract_header.py
--rw-r--r--   0        0        0    14741 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/segy_file_header.py
--rw-r--r--   0        0        0     8540 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/segy_header_item.py
--rw-r--r--   0        0        0    35111 2023-06-02 08:15:34.847622 segytools-0.2.0/src/segytools/segy_trace_header.py
--rw-r--r--   0        0        0     2543 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/toolkit.py
--rw-r--r--   0        0        0       95 2023-01-29 16:40:13.789248 segytools-0.2.0/src/segytools/utils.py
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 segytools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.2.1/README.md
+-rw-r--r--   0        0        0      870 2023-07-24 10:01:38.982087 segytools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1274 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/__init__.py
+-rw-r--r--   0        0        0     2223 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/datatypes.py
+-rw-r--r--   0        0        0     5249 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_abstract_header.py
+-rw-r--r--   0        0        0    15798 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_file_header.py
+-rw-r--r--   0        0        0     9597 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_header_item.py
+-rw-r--r--   0        0        0    36170 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/segy_trace_header.py
+-rw-r--r--   0        0        0     3602 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/toolkit.py
+-rw-r--r--   0        0        0     1154 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/utils.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 segytools-0.2.1/PKG-INFO
```

### Comparing `segytools-0.2.0/LICENSE` & `segytools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segytools-0.2.0/README.md` & `segytools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `segytools-0.2.0/pyproject.toml` & `segytools-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "segytools"
-version = "0.2.0"
+version = "0.2.1"
 description = "low level toolkit for manipulating and analyzing segy formatted data"
 authors = ["anthonytorlucci <anthonytorlucci@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `segytools-0.2.0/src/segytools/segy_file_header.py` & `segytools-0.2.1/src/segytools/segy_file_header.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-'''
+"""
 segy file header aka binary header
-'''
+
+Copyright 2022 Anthony Torlucci
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
 
 # import python standard modules
 
 # import 3rd party libraries
 
 # import local python
 from segytools.datatypes import (DataSampleFormat,
```

### Comparing `segytools-0.2.0/src/segytools/segy_trace_header.py` & `segytools-0.2.1/src/segytools/segy_trace_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-"""segy trace header"""
+"""
+segy trace header
+
+Copyright 2022 Anthony Torlucci
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
 
 # import python standard modules
 
 # import 3rd party libraries
 
 # import local python
 from segytools.datatypes import (DATA_SAMPLE_FORMAT_INT16,
```

### Comparing `segytools-0.2.0/PKG-INFO` & `segytools-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: segytools
-Version: 0.2.0
+Version: 0.2.1
 Summary: low level toolkit for manipulating and analyzing segy formatted data
 License: MIT
 Author: anthonytorlucci
 Author-email: anthonytorlucci@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: ibm2ieee (>=1.2.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # segytools
 
 [Documentation](https://anthonytorlucci.github.io/segytools/)
```

