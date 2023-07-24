# Comparing `tmp/sysnet-pdffiller-1.0.1.tar.gz` & `tmp/sysnet-pdffiller-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-pdffiller-1.0.1.tar", last modified: Mon Jul 24 15:42:33 2023, max compression
+gzip compressed data, was "sysnet-pdffiller-1.0.2.tar", last modified: Mon Jul 24 15:52:12 2023, max compression
```

## Comparing `sysnet-pdffiller-1.0.1.tar` & `sysnet-pdffiller-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.383350 sysnet-pdffiller-1.0.1/
--rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pdffiller-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      740 2023-07-24 15:42:33.383350 sysnet-pdffiller-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-24 15:13:41.000000 sysnet-pdffiller-1.0.1/README.md
--rw-rw-rw-   0        0        0      900 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      118 2023-07-24 12:26:39.000000 sysnet-pdffiller-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:42:33.384348 sysnet-pdffiller-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.370348 sysnet-pdffiller-1.0.1/sysnet_pdf/
--rw-rw-rw-   0        0        0        0 2023-07-24 14:42:45.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/__init__.py
--rw-rw-rw-   0        0        0      292 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/config.py
--rw-rw-rw-   0        0        0      830 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/jasper.py
--rw-rw-rw-   0        0        0    12233 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.1/sysnet_pdf/pdf_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.379347 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/
--rw-rw-rw-   0        0        0      740 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 15:42:33.000000 sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:33.381348 sysnet-pdffiller-1.0.1/tests/
--rw-rw-rw-   0        0        0      664 2023-07-24 15:23:03.000000 sysnet-pdffiller-1.0.1/tests/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:52:12.468171 sysnet-pdffiller-1.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pdffiller-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-07-24 15:52:12.467171 sysnet-pdffiller-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-24 15:13:41.000000 sysnet-pdffiller-1.0.2/README.md
+-rw-rw-rw-   0        0        0      900 2023-07-24 15:52:01.000000 sysnet-pdffiller-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      118 2023-07-24 12:26:39.000000 sysnet-pdffiller-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:52:12.468171 sysnet-pdffiller-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 15:52:12.454169 sysnet-pdffiller-1.0.2/sysnet_pdf/
+-rw-rw-rw-   0        0        0        0 2023-07-24 14:42:45.000000 sysnet-pdffiller-1.0.2/sysnet_pdf/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-07-24 15:42:06.000000 sysnet-pdffiller-1.0.2/sysnet_pdf/config.py
+-rw-rw-rw-   0        0        0      816 2023-07-24 15:52:01.000000 sysnet-pdffiller-1.0.2/sysnet_pdf/jasper.py
+-rw-rw-rw-   0        0        0    12198 2023-07-24 15:52:01.000000 sysnet-pdffiller-1.0.2/sysnet_pdf/pdf_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:52:12.463168 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-07-24 15:52:12.000000 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-24 15:52:12.000000 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:52:12.000000 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-24 15:52:12.000000 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 15:52:12.000000 sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:52:12.465169 sysnet-pdffiller-1.0.2/tests/
+-rw-rw-rw-   0        0        0      657 2023-07-24 15:49:55.000000 sysnet-pdffiller-1.0.2/tests/test_suite.py
```

### Comparing `sysnet-pdffiller-1.0.1/LICENSE` & `sysnet-pdffiller-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-pdffiller-1.0.1/PKG-INFO` & `sysnet-pdffiller-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-pdffiller
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tools for filling PDF templates with data
 Author-email: Data Developer <info@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/pdf/tree/master/pdf-filler
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Home Use
```

### Comparing `sysnet-pdffiller-1.0.1/pyproject.toml` & `sysnet-pdffiller-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-pdffiller"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Tools for filling PDF templates with data"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-pdffiller-1.0.1/sysnet_pdf/jasper.py` & `sysnet-pdffiller-1.0.2/sysnet_pdf/jasper.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,14 @@
         'data_file': os.path.join(TEST_DATA_DIRECTORY, 'picture_cert_data.json'),
         'json_query': ''
     }
     pyreportjasper = PyReportJasper()
     pyreportjasper.config(
         input_file,
         output_file,
-        output_formats=["sysnet_pdf"],
+        output_formats=["pdf"],
         db_connection=conn
     )
     pyreportjasper.process_report()
     del pyreportjasper
     print('Result is the file below.')
-    print(output_file + '.sysnet_pdf')
+    print(output_file + '.pdf')
```

### Comparing `sysnet-pdffiller-1.0.1/sysnet_pdf/pdf_utils.py` & `sysnet-pdffiller-1.0.2/sysnet_pdf/pdf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from PyPDF3.generic import NameObject, IndirectObject, BooleanObject, NumberObject
 from fillpdf.fillpdfs import write_fillable_pdf
 
 from settings import PDF_OUTPUT_DIR, PDF_TEMP_FILE, PDF_OWNER_PASSWORD, \
     PDF_TEMPLATES_DIR, LOG, CONFIG, CC
 from sysnet_pdf.config import PdfError
 
-EXTENSION_PDF = 'sysnet_pdf'
+EXTENSION_PDF = 'pdf'
 EXTENSION_JASPER = 'jrxml'
-TEMPLATE_TYPE_PDF = 'sysnet_pdf'
+TEMPLATE_TYPE_PDF = 'pdf'
 TEMPLATE_TYPE_JASPER = 'jasper'
 TEMPLATE_TYPE_OTHER = 'other'
 KEY_TEMPLATES_PDF = 'pdf_templates'
 KEY_TEMPLATES_JASPER = 'jasper_templates'
 
 
 def xfdf_to_dict(filename=None):
@@ -136,15 +136,15 @@
         return TEMPLATE_TYPE_JASPER
     else:
         return TEMPLATE_TYPE_OTHER
 
 
 class PdfFactory(object, metaclass=pu.Singleton):
     def __init__(self):
-        self.pdf_templates = CONFIG['templates']['sysnet_pdf']
+        self.pdf_templates = CONFIG['templates']['pdf']
         self.jasper_templates = CONFIG['templates']['jasper']
         LOG.logger.info('PdfFactory created')
 
     def _identify_template_type(self, source_path=None):
         template_type = parse_template_type(source_path=source_path)        # PDF/JASPER
         if template_type == TEMPLATE_TYPE_PDF:
             templates = self.pdf_templates
@@ -252,21 +252,21 @@
 
         pdf_file_path = os.path.join(PDF_OUTPUT_DIR, pdf_file_name)
         data = xfdf_to_dict(filename=xfdf_file_path)
         self.fill_pdf_form(template_filename=template_filename, data=data)
         return flatten_pdf(data_dict=data, output_pdf=pdf_file_path)
 
     def check_templates(self):
-        out = {'sysnet_pdf': [],  'jasper': []}
+        out = {'pdf': [],  'jasper': []}
         for item in self.pdf_templates:
             fname = item
             fpath = os.path.join(PDF_TEMPLATES_DIR, fname)
             exists = os.path.exists(fpath)
             t = (fname, fpath, exists)
-            out['sysnet_pdf'].append(t)
+            out['pdf'].append(t)
         for item in self.jasper_templates:
             fname = item
             fpath = os.path.join(PDF_TEMPLATES_DIR, fname)
             exists = os.path.exists(fpath)
             t = (fname, fpath, exists)
             out['jasper'].append(t)
         return out
```

### Comparing `sysnet-pdffiller-1.0.1/sysnet_pdffiller.egg-info/PKG-INFO` & `sysnet-pdffiller-1.0.2/sysnet_pdffiller.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-pdffiller
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tools for filling PDF templates with data
 Author-email: Data Developer <info@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/pdf/tree/master/pdf-filler
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Home Use
```

### Comparing `sysnet-pdffiller-1.0.1/tests/test_suite.py` & `sysnet-pdffiller-1.0.2/tests/test_suite.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     def test_xfdf_to_dict(self):
         d = xfdf_to_dict(TEST_XFDF)
         self.assertIsNotNone(d, 'xfdf_to_dict: OK')
 
     def test_fill_form(self):
         f = PDF_FACTORY
         out = f.create_pdf_from_xfdf(
-            template_filename='051-certificate_form.sysnet_pdf',
+            template_filename='051-certificate_form.pdf',
             xfdf_file_path=TEST_XFDF,
             pdf_file_name=TEST_PDF_OUT_FILE)
         self.assertIsNotNone(out, 'test_fill_form: Filled PDF')
```

