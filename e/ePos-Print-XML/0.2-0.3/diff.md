# Comparing `tmp/epos_print_xml-0.2.tar.gz` & `tmp/epos_print_xml-0.3.tar.gz`

## Comparing `epos_print_xml-0.2.tar` & `epos_print_xml-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 epos_print_xml-0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/__init__.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/attributes.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/constants.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/document.py
--rw-r--r--   0        0        0    17239 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/elements.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/printer.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/status.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 epos_print_xml-0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 epos_print_xml-0.2/LICENSE
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 epos_print_xml-0.2/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 epos_print_xml-0.2/pyproject.toml
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 epos_print_xml-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 epos_print_xml-0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/__init__.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/attributes.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/constants.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/document.py
+-rw-r--r--   0        0        0    17241 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/elements.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/printer.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 epos_print_xml-0.3/src/epos/status.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 epos_print_xml-0.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 epos_print_xml-0.3/LICENSE
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 epos_print_xml-0.3/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 epos_print_xml-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 epos_print_xml-0.3/PKG-INFO
```

### Comparing `epos_print_xml-0.2/.github/workflows/python-package.yml` & `epos_print_xml-0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/src/test.py` & `epos_print_xml-0.3/src/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from epos.printer import Printer
 from epos.document import EposDocument
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align, BarcodeType, HRI
 
 # Create a new printer object with 10.0.0.10 as ip
-printer = Printer('10.0.0.10')
+printer = Printer('100.0.0.10')
 # Check if we can connect to the printer with no errors, otherwise exit
-if not printer.try_connection():
+if not printer.printer_ready():
     print("Printer error!")
+    exit()
 else:
     print('Connection with printer established.')
 
 # Create a new EposDocument object
 # This will contain all the individual elements
 doc = EposDocument()
```

### Comparing `epos_print_xml-0.2/src/epos/attributes.py` & `epos_print_xml-0.3/src/epos/attributes.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/src/epos/constants.py` & `epos_print_xml-0.3/src/epos/constants.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/src/epos/document.py` & `epos_print_xml-0.3/src/epos/document.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 
 @dataclass
 class EposDocument:
     parameters: list = field(default_factory=list)
     body: list[Type[BaseElement]] = field(default_factory=list)
 
-    def add_parameter(self, element: Generic[B]):
+    def add_parameter(self, element: Generic[B]) -> None:
         self.parameters.append(element)
 
-    def add_body(self, element: Generic[B]):
+    def add_body(self, element: Generic[B]) -> None:
         self.body.append(element)
 
     def parameters_to_xml(self) -> ET.Element:
         return _to_xml('parameter', self.parameters)
 
     def body_to_xml(self) -> ET.Element:
         return _to_xml('epos-print', self.body)
@@ -31,15 +31,15 @@
         s = ET.tostring(self.body_to_xml(), encoding='unicode')
         s = s.replace(' />', '/>')
         if url_encode_newlines:
             s = s.replace('\n', '&#10;')
         return s
 
 
-def _to_xml(base_tag: str, element_list: list[Type[BaseElement], ...]) -> ET.Element:
+def _to_xml(base_tag: str, element_list: list[Type[B], ...]) -> ET.Element:
     root = ET.Element(
         base_tag,
         xmlns='http://www.epson-pos.com/schemas/2011/03/epos-print',
     )
     for element in element_list:
         root.append(element.to_xml())
     return root
```

### Comparing `epos_print_xml-0.2/src/epos/elements.py` & `epos_print_xml-0.3/src/epos/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         self.underline = ul
 
     @property
     def bold(self) -> bool:
         return self._bold
 
     @bold.setter
-    def bold(self, bold: bool|str):
+    def bold(self, bold: bool | str):
         if bold == 'true':
             self._bold = True
         elif bold == 'false':
             self._bold = False
         else:
             self._bold = bold
```

### Comparing `epos_print_xml-0.2/src/epos/printer.py` & `epos_print_xml-0.3/src/epos/printer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,71 @@
 import xml.etree.ElementTree as ET
 
 import requests
 
 from .document import EposDocument
 from .elements import Cut, Response
 
-
 namespaces = {
     's': 'http://schemas.xmlsoap.org/soap/envelope/',
     'epos-print': 'http://www.epson-pos.com/schemas/2011/03/epos-print',
 }
 
+
 class Printer:
-    def __init__(self, ip):
+    def __init__(
+            self,
+            ip: str,
+            request_timeout: int = 3,
+            use_https: bool = False,
+            devid: str = 'local_printer',
+            job_timeout: int = 5000,
+            url: str = '/cgi-bin/epos/service.cgi',
+    ):
         self.ip = ip
+        self.request_timeout = request_timeout
+        self.use_https = use_https
+        self.devid = devid
+        self.job_timeout = job_timeout
+        self.url = url
+
+    def printer_ready(self) -> bool:
+        """
+        Send empty page to check the status
+
+        Returns true if online, false if offline.
+
+        :return Boolean
+        """
+        response = self.print_empty()
+        return response.success
+
+    def print_empty(self) -> Response:
+        """
+        Send an empty document to the printer.
+        Used to gather status information
 
-        # Defaults, normally not changed
-        self.use_https = False
-        self.devid = 'local_printer'
-        self.timeout = 5000
-        self.url = '/cgi-bin/epos/service.cgi'
-
-    def try_connection(self):
-        """Send empty page to check the status"""
+        :return: Response
+        """
         doc = EposDocument()
-        resp = self.print(doc, autocut=False)
-        return resp.success
+        response = self.print(doc, autocut=False)
+        return response
 
-    def print(self, doc: EposDocument, autocut=True) -> Response:
+    def print(self, doc: EposDocument, autocut: bool = True) -> Response:
         if autocut:
             doc.add_body(Cut())
         r = self._send_printjob(doc.body_to_str())
 
         response = Response(success=False)
+        try:
+            xml_dom = ET.fromstring(r)
+        except ET.ParseError:
+            response.code = 'PARSING_ERROR'
+            return response
 
-        xml_dom = ET.fromstring(r)
         body = xml_dom.find('./s:Body', namespaces)
         if not body:
             response.code = 'NO_BODY_FOUND'
             return response
 
         for element in body:
             if 'response' in element.tag:
@@ -51,29 +78,30 @@
         response.success = attr['success'] == 'true'
         response.code = attr['code']
         response.status = int(attr['status'])
         response.battery = int(attr['battery'])
 
         return response
 
-    def _send_printjob(self, data):
+    def _send_printjob(self, data: str) -> str:
         prefix = 'https://' if self.use_https else 'http://'
         url = prefix + self.ip + self.url
         headers = {
             'content-type': 'text/xml; charset=utf-8',
             'If-Modified-Since': 'Thu, 01 Jan 1970 00:00:00 GMT',
             'SOAPAction': '""',
         }
-        params = {'devid': self.devid, 'timeout': self.timeout}
+        params = {'devid': self.devid, 'timeout': self.job_timeout}
 
         response = requests.post(
             url,
             data=_add_soap_enveloppe(data),
             headers=headers,
             params=params,
+            timeout=self.request_timeout,
         )
 
         return response.text
 
 
 def _add_soap_enveloppe(body: str, header: str = '') -> str:
     """Add the soap enveloppe, header and body"""
```

### Comparing `epos_print_xml-0.2/src/epos/status.py` & `epos_print_xml-0.3/src/epos/status.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/.gitignore` & `epos_print_xml-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/LICENSE` & `epos_print_xml-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.2/README.md` & `epos_print_xml-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # py-epos-print-xml
 Python library to communicate with Epson thermal printers via ePos-Print XML.
 This makes it easy and intuitive to create print orders for ePos-Print XML compatible printers, like the Epson TM-T20, TM-m30 and TM-m50 series.
 Depending on the printer model, some elements are not supported. Check your manual or the [Epson reference](https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?vid=ref_epos_print_xml_en_devicespecifications_supportedelementslist) to see which elements are supported.
 
-This is still in active development, don't expect everything to work.
-
 ## Instaling
 ```
 pip install ePos-Print-XML
 ```
 
 ## Example
 
@@ -17,24 +15,24 @@
 from epos.document import EposDocument
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align
 
 # Create a new printer object with 10.0.0.12 as ip
 printer = Printer('10.0.0.12')
 # Check if we can connect to the printer with no errors, otherwise exit
-if not printer.try_connection():
+if not printer.printer_ready():
     exit()
 
 # Create a new EposDocument object
 # This will contain all the individual elements
 doc = EposDocument()
 
 # Add an element directly to the body of the document
 doc.add_body(Text('This is example text!\n'))
-doc.add_body(Feed()) # Another way to add a newline
+doc.add_body(Feed())  # Another way to add a newline
 
 # It's also possible to first create the text object and then change the properties
 t = Text('Some special text :O\n')
 t.bold = True
 t.align = Align.CENTER
 doc.add_body(t)
```

### Comparing `epos_print_xml-0.2/pyproject.toml` & `epos_print_xml-0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "ePos-Print-XML"
-version = "0.2"
+version = "0.3"
 dependencies = [
   'requests',
 ]
 authors = [
   { name="Merten Fermont" },
 ]
 description = "Library to communicate with Epson thermal printers via ePOS-Print XML protocol"
```

### Comparing `epos_print_xml-0.2/PKG-INFO` & `epos_print_xml-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ePos-Print-XML
-Version: 0.2
+Version: 0.3
 Summary: Library to communicate with Epson thermal printers via ePOS-Print XML protocol
 Project-URL: Homepage, https://github.com/MertenF/epos-print-xml
 Project-URL: Bug Tracker, https://github.com/MertenF/epos-print-xml/issues
 Author: Merten Fermont
 License-File: LICENSE
 Keywords: epos,printing,receipt,thermoprinter,voucher printer
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,14 @@
 Description-Content-Type: text/markdown
 
 # py-epos-print-xml
 Python library to communicate with Epson thermal printers via ePos-Print XML.
 This makes it easy and intuitive to create print orders for ePos-Print XML compatible printers, like the Epson TM-T20, TM-m30 and TM-m50 series.
 Depending on the printer model, some elements are not supported. Check your manual or the [Epson reference](https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?vid=ref_epos_print_xml_en_devicespecifications_supportedelementslist) to see which elements are supported.
 
-This is still in active development, don't expect everything to work.
-
 ## Instaling
 ```
 pip install ePos-Print-XML
 ```
 
 ## Example
 
@@ -35,24 +33,24 @@
 from epos.document import EposDocument
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align
 
 # Create a new printer object with 10.0.0.12 as ip
 printer = Printer('10.0.0.12')
 # Check if we can connect to the printer with no errors, otherwise exit
-if not printer.try_connection():
+if not printer.printer_ready():
     exit()
 
 # Create a new EposDocument object
 # This will contain all the individual elements
 doc = EposDocument()
 
 # Add an element directly to the body of the document
 doc.add_body(Text('This is example text!\n'))
-doc.add_body(Feed()) # Another way to add a newline
+doc.add_body(Feed())  # Another way to add a newline
 
 # It's also possible to first create the text object and then change the properties
 t = Text('Some special text :O\n')
 t.bold = True
 t.align = Align.CENTER
 doc.add_body(t)
```

