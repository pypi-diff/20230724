# Comparing `tmp/sysnet-pdffiller-1.0.0.tar.gz` & `tmp/sysnet-pdffiller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-pdffiller-1.0.0.tar", last modified: Mon Jul 24 15:23:11 2023, max compression
+gzip compressed data, was "sysnet-pdffiller-1.0.1.tar", last modified: Mon Jul 24 15:42:33 2023, max compression
```

## Comparing `sysnet-pdffiller-1.0.0.tar` & `sysnet-pdffiller-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:23:11.986926 sysnet-pdffiller-1.0.0/
--rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pdffiller-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      740 2023-07-24 15:23:11.985926 sysnet-pdffiller-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-24 15:13:41.000000 sysnet-pdffiller-1.0.0/README.md
--rw-rw-rw-   0        0        0      900 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      118 2023-07-24 12:26:39.000000 sysnet-pdffiller-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:23:11.986926 sysnet-pdffiller-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 15:23:11.970928 sysnet-pdffiller-1.0.0/sysnet_pdf/
--rw-rw-rw-   0        0        0        0 2023-07-24 14:42:45.000000 sysnet-pdffiller-1.0.0/sysnet_pdf/__init__.py
--rw-rw-rw-   0        0        0      830 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.0/sysnet_pdf/jasper.py
--rw-rw-rw-   0        0        0    12203 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.0/sysnet_pdf/pdf_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:23:11.981928 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/
--rw-rw-rw-   0        0        0      740 2023-07-24 15:23:11.000000 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-24 15:23:11.000000 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:23:11.000000 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-24 15:23:11.000000 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 15:23:11.000000 sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 15:23:11.983927 sysnet-pdffiller-1.0.0/tests/
--rw-rw-rw-   0        0        0      664 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.0/tests/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.383350 sysnet-pdffiller-1.0.1/
+-rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pdffiller-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-07-24 15:42:33.383350 sysnet-pdffiller-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-24 15:13:41.000000 sysnet-pdffiller-1.0.1/README.md
+-rw-rw-rw-   0        0        0      900 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      118 2023-07-24 12:26:39.000000 sysnet-pdffiller-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:42:33.384348 sysnet-pdffiller-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.370348 sysnet-pdffiller-1.0.1/sysnet_pdf/
+-rw-rw-rw-   0        0        0        0 2023-07-24 14:42:45.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/config.py
+-rw-rw-rw-   0        0        0      830 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/jasper.py
+-rw-rw-rw-   0        0        0    12233 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/pdf_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.379347 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.381348 sysnet-pdffiller-1.0.1/tests/
+-rw-rw-rw-   0        0        0      664 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.1/tests/test_suite.py
```

### Comparing `sysnet-pdffiller-1.0.0/LICENSE` & `sysnet-pdffiller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-pdffiller-1.0.0/PKG-INFO` & `sysnet-pdffiller-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-pdffiller
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for filling PDF templates with data
 Author-email: Data Developer <info@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/pdf/tree/master/pdf-filler
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Home Use
```

### Comparing `sysnet-pdffiller-1.0.0/pyproject.toml` & `sysnet-pdffiller-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-pdffiller"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Tools for filling PDF templates with data"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-pdffiller-1.0.0/sysnet_pdf/jasper.py` & `sysnet-pdffiller-1.0.1/sysnet_pdf/jasper.py`

 * *Files identical despite different names*

### Comparing `sysnet-pdffiller-1.0.0/sysnet_pdf/pdf_utils.py` & `sysnet-pdffiller-1.0.1/sysnet_pdf/pdf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from xml.etree.ElementTree import ParseError
 
 import PyPDF3
 from PyPDF3 import PdfFileWriter
 from PyPDF3.generic import NameObject, IndirectObject, BooleanObject, NumberObject
 from fillpdf.fillpdfs import write_fillable_pdf
 
-from settings import PDF_OUTPUT_DIR, PdfError, PDF_TEMP_FILE, PDF_OWNER_PASSWORD, \
+from settings import PDF_OUTPUT_DIR, PDF_TEMP_FILE, PDF_OWNER_PASSWORD, \
     PDF_TEMPLATES_DIR, LOG, CONFIG, CC
+from sysnet_pdf.config import PdfError
 
 EXTENSION_PDF = 'sysnet_pdf'
 EXTENSION_JASPER = 'jrxml'
 TEMPLATE_TYPE_PDF = 'sysnet_pdf'
 TEMPLATE_TYPE_JASPER = 'jasper'
 TEMPLATE_TYPE_OTHER = 'other'
 KEY_TEMPLATES_PDF = 'pdf_templates'
```

### Comparing `sysnet-pdffiller-1.0.0/sysnet_pdffiller.egg-info/PKG-INFO` & `sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-pdffiller
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for filling PDF templates with data
 Author-email: Data Developer <info@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/pdf/tree/master/pdf-filler
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Home Use
```

### Comparing `sysnet-pdffiller-1.0.0/tests/test_suite.py` & `sysnet-pdffiller-1.0.1/tests/test_suite.py`

 * *Files identical despite different names*

