# Comparing `tmp/amazon-textract-response-parser-0.1.9.tar.gz` & `tmp/amazon-textract-response-parser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon-textract-response-parser-0.1.9.tar", last modified: Fri Apr 30 20:38:01 2021, max compression
+gzip compressed data, was "amazon-textract-response-parser-1.0.0.tar", last modified: Mon Jul 24 11:11:26 2023, max compression
```

## Comparing `amazon-textract-response-parser-0.1.9.tar` & `amazon-textract-response-parser-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.172180 amazon-textract-response-parser-0.1.9/
--rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 20:38:01.172477 amazon-textract-response-parser-0.1.9/PKG-INFO
--rw-r--r--   0 schadem  (1964830885) staff       (20)     6148 2021-04-30 16:54:10.000000 amazon-textract-response-parser-0.1.9/README.md
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.165054 amazon-textract-response-parser-0.1.9/a2i/
--rw-r--r--   0 schadem  (1964830885) staff       (20)      108 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/a2i/__init__.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     7188 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.9/a2i/a2irp.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1355 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.9/a2i/a2irptest.py
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.168402 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/
--rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/PKG-INFO
--rw-r--r--   0 schadem  (1964830885) staff       (20)      423 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/SOURCES.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)        1 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/dependency_links.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)       26 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/requires.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)        8 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/top_level.txt
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.169117 amazon-textract-response-parser-0.1.9/bin/
--rwxr-xr-x   0 schadem  (1964830885) staff       (20)     1175 2021-04-30 20:32:03.000000 amazon-textract-response-parser-0.1.9/bin/amazon-textract-pipeline
--rw-r--r--   0 schadem  (1964830885) staff       (20)      505 2021-04-30 20:38:01.173522 amazon-textract-response-parser-0.1.9/setup.cfg
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1874 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/setup.py
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.171014 amazon-textract-response-parser-0.1.9/trp/
--rw-r--r--   0 schadem  (1964830885) staff       (20)    15507 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/trp/__init__.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1574 2021-04-29 15:28:03.000000 amazon-textract-response-parser-0.1.9/trp/t_pipeline.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)    19506 2021-04-30 16:27:39.000000 amazon-textract-response-parser-0.1.9/trp/trp2.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-07-24 11:11:26.553153 amazon-textract-response-parser-1.0.0/
+-rw-r--r--   0 schadem    (504) staff       (20)    13435 2023-07-24 11:11:26.553302 amazon-textract-response-parser-1.0.0/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)    10299 2023-03-21 18:49:27.000000 amazon-textract-response-parser-1.0.0/README.md
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-07-24 11:11:26.549841 amazon-textract-response-parser-1.0.0/a2i/
+-rw-r--r--   0 schadem    (504) staff       (20)      108 2023-07-24 11:10:56.000000 amazon-textract-response-parser-1.0.0/a2i/__init__.py
+-rw-r--r--   0 schadem    (504) staff       (20)     7188 2022-09-14 19:59:35.000000 amazon-textract-response-parser-1.0.0/a2i/a2irp.py
+-rw-r--r--   0 schadem    (504) staff       (20)     1355 2022-09-14 19:59:35.000000 amazon-textract-response-parser-1.0.0/a2i/a2irptest.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-07-24 11:11:26.550623 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/
+-rw-r--r--   0 schadem    (504) staff       (20)    13435 2023-07-24 11:11:26.000000 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)      501 2023-07-24 11:11:26.000000 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem    (504) staff       (20)        1 2023-07-24 11:11:26.000000 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       27 2023-07-24 11:11:26.000000 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/requires.txt
+-rw-r--r--   0 schadem    (504) staff       (20)        8 2023-07-24 11:11:26.000000 amazon-textract-response-parser-1.0.0/amazon_textract_response_parser.egg-info/top_level.txt
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-07-24 11:11:26.550777 amazon-textract-response-parser-1.0.0/bin/
+-rwxr-xr-x   0 schadem    (504) staff       (20)     1696 2022-09-14 19:59:35.000000 amazon-textract-response-parser-1.0.0/bin/amazon-textract-pipeline
+-rw-r--r--   0 schadem    (504) staff       (20)      505 2023-07-24 11:11:26.553707 amazon-textract-response-parser-1.0.0/setup.cfg
+-rw-r--r--   0 schadem    (504) staff       (20)     1949 2023-07-24 11:10:56.000000 amazon-textract-response-parser-1.0.0/setup.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-07-24 11:11:26.552916 amazon-textract-response-parser-1.0.0/trp/
+-rw-r--r--   0 schadem    (504) staff       (20)    20320 2023-07-24 11:10:56.000000 amazon-textract-response-parser-1.0.0/trp/__init__.py
+-rw-r--r--   0 schadem    (504) staff       (20)     9009 2023-03-23 15:34:54.000000 amazon-textract-response-parser-1.0.0/trp/t_pipeline.py
+-rw-r--r--   0 schadem    (504) staff       (20)     4884 2023-03-21 18:49:27.000000 amazon-textract-response-parser-1.0.0/trp/t_tables.py
+-rw-r--r--   0 schadem    (504) staff       (20)    37318 2023-06-16 13:04:38.000000 amazon-textract-response-parser-1.0.0/trp/trp2.py
+-rw-r--r--   0 schadem    (504) staff       (20)     7635 2023-03-21 18:49:27.000000 amazon-textract-response-parser-1.0.0/trp/trp2_analyzeid.py
+-rw-r--r--   0 schadem    (504) staff       (20)    14208 2023-04-18 17:34:02.000000 amazon-textract-response-parser-1.0.0/trp/trp2_expense.py
+-rw-r--r--   0 schadem    (504) staff       (20)     8106 2023-03-21 18:49:27.000000 amazon-textract-response-parser-1.0.0/trp/trp2_lending.py
```

### Comparing `amazon-textract-response-parser-0.1.9/a2i/a2irp.py` & `amazon-textract-response-parser-1.0.0/a2i/a2irp.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.9/a2i/a2irptest.py` & `amazon-textract-response-parser-1.0.0/a2i/a2irptest.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.9/bin/amazon-textract-pipeline` & `amazon-textract-response-parser-1.0.0/bin/amazon-textract-pipeline`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 #!/usr/bin/env python
 
 import json
 import sys
 from trp.trp2 import TDocumentSchema
-from trp.t_pipeline import order_blocks_by_geo, add_page_orientation
+from trp.t_pipeline import order_blocks_by_geo, add_page_orientation, pipeline_merge_tables, add_kv_ocr_confidence
 import argparse
 from trp import __version__
 from enum import Enum, auto
 
+
 class TPipelineComponents(Enum):
     order_blocks_by_geo = auto()
     add_page_orientation = auto()
-
-
+    merge_tables = auto()
+    kv_ocr_confidence = auto()
 
 
 parser = argparse.ArgumentParser()
-parser.add_argument("--components", nargs='+', choices=[TPipelineComponents.add_page_orientation.name, TPipelineComponents.order_blocks_by_geo.name], help="define which components to call", required=True)
+parser.add_argument("--components",
+                    nargs='+',
+                    choices=[
+                        TPipelineComponents.add_page_orientation.name, TPipelineComponents.order_blocks_by_geo.name,
+                        TPipelineComponents.merge_tables.name, TPipelineComponents.kv_ocr_confidence.name
+                    ],
+                    help="define which components to call",
+                    required=True)
 parser.add_argument("--version",
                     action='version',
                     version='%(prog)s {version}'.format(version=__version__),
                     help="print version information")
 
-
 args = parser.parse_args()
 components = [TPipelineComponents[x] for x in args.components]
 
-
 doc_json = json.load(sys.stdin)
 t_doc = TDocumentSchema().load(doc_json)
 if TPipelineComponents.order_blocks_by_geo in components:
     t_doc = order_blocks_by_geo(t_doc)
 if TPipelineComponents.add_page_orientation in components:
     t_doc = add_page_orientation(t_doc)
+if TPipelineComponents.merge_tables in components:
+    t_doc = pipeline_merge_tables(t_doc)
+if TPipelineComponents.kv_ocr_confidence in components:
+    t_doc = add_kv_ocr_confidence(t_doc)
 
 print(TDocumentSchema().dumps(t_doc))
-
```

### Comparing `amazon-textract-response-parser-0.1.9/setup.py` & `amazon-textract-response-parser-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 import sys
 from setuptools import setup
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
-requirements = ['boto3', 'marshmallow==3.11.1']
+
+requirements = ['boto3', 'marshmallow>=3.14,<4']
 
 if sys.argv[-1] == 'publish-test':
     os.system(f"cd {os.path.dirname(__file__)}")
     os.system('rm -rf dist/ build/ amazon_textract_response_parser.egg-info/')
-    os.system('python setup.py sdist bdist_wheel')
+    os.system('python3 setup.py sdist bdist_wheel')
     os.system('twine check dist/*')
     os.system('twine upload --repository pypitest dist/*')
     sys.exit()
 
 if sys.argv[-1] == 'publish':
-    os.system(f"cd {os.path.dirname(__file__)}")
+    script_path = str(f"cd {os.path.dirname(__file__)}")
+    os.system(script_path)
     os.system('rm -rf dist/ build/ amazon_textract_response_parser.egg-info/')
-    os.system('python setup.py sdist bdist_wheel')
+    os.system('python3 setup.py sdist bdist_wheel')
     os.system('twine check dist/*')
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
-setup(
-    name='amazon-textract-response-parser',
-    packages=['trp', 'a2i'],
-    version='0.1.9',
-    description='Easily parse JSON returned by Amazon Textract.',
-    install_requires=requirements,
-    scripts=['bin/amazon-textract-pipeline'],
-    long_description_content_type='text/markdown',
-    long_description=read('README.md'),
-    author='Amazon Rekognition Textract Demoes',
-    author_email='rekognition-textract-demos@amazon.com',
-    url='https://github.com/aws-samples/amazon-textract-response-parser',
-    keywords=
-    'amazon-textract-response-parser trp aws amazon textract ocr response parser',
-    license="Apache License Version 2.0",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Topic :: Utilities",
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    python_requires='>=3.6')
+setup(name='amazon-textract-response-parser',
+      packages=['trp', 'a2i'],
+      version='1.0.0',
+      description='Easily parse JSON returned by Amazon Textract.',
+      install_requires=requirements,
+      scripts=['bin/amazon-textract-pipeline'],
+      long_description_content_type='text/markdown',
+      long_description=read('README.md'),
+      author='Amazon Rekognition Textract Demoes',
+      author_email='rekognition-textract-demos@amazon.com',
+      url='https://github.com/aws-samples/amazon-textract-response-parser',
+      keywords='amazon-textract-response-parser trp aws amazon textract ocr response parser',
+      license="Apache License Version 2.0",
+      classifiers=[
+          "Development Status :: 4 - Beta",
+          "Topic :: Utilities",
+          'License :: OSI Approved :: Apache Software License',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+      ],
+      python_requires='>=3.8')
```

### Comparing `amazon-textract-response-parser-0.1.9/trp/__init__.py` & `amazon-textract-response-parser-1.0.0/trp/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # -*- coding: utf-8 -*-
 """Top-level package for amazon-textract-response-parser."""
 import logging
+from typing import List
 from logging import NullHandler
 
 logging.getLogger(__name__).addHandler(NullHandler())
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.1.9'
+__version__ = '1.0.0'
+
+ENTITY_TYPE_COLUMN_HEADER = "COLUMN_HEADER"
+ENTITY_TYPE_MERGED_CELL = "MERGED_CELL"
+
 
 class BaseBlock():
+
     def __init__(self, block, blockMap):
         self._block = block
         self._confidence = block['Confidence']
         self._geometry = Geometry(block['Geometry'])
         self._id = block['Id']
         self._text = ""
-        if 'Text' in block:
+        self._text_type = ""
+        if 'Text' in block and block['Text']:
             self._text = block['Text']
-        if "Custom" in block:
+        if "Custom" in block and block['Custom']:
             self._custom = block["Custom"]
+        if 'TextType' in block and block['TextType']:
+            self._text_type = block['TextType']
 
     def __str__(self):
         return self._text
 
     @property
     def custom(self):
         return self._custom
@@ -44,24 +53,29 @@
     def text(self):
         return self._text
 
     @property
     def block(self):
         return self._block
 
+    @property
+    def textType(self):
+        return self._text_type
+
+
 class BoundingBox:
+
     def __init__(self, width, height, left, top):
         self._width = width
         self._height = height
         self._left = left
         self._top = top
 
     def __str__(self):
-        return "width: {}, height: {}, left: {}, top: {}".format(
-            self._width, self._height, self._left, self._top)
+        return "width: {}, height: {}, left: {}, top: {}".format(self._width, self._height, self._left, self._top)
 
     @property
     def width(self):
         return self._width
 
     @property
     def height(self):
@@ -73,14 +87,15 @@
 
     @property
     def top(self):
         return self._top
 
 
 class Polygon:
+
     def __init__(self, x, y):
         self._x = x
         self._y = y
 
     def __str__(self):
         return "x: {}, y: {}".format(self._x, self._y)
 
@@ -90,19 +105,19 @@
 
     @property
     def y(self):
         return self._y
 
 
 class Geometry:
+
     def __init__(self, geometry):
         boundingBox = geometry["BoundingBox"]
         polygon = geometry["Polygon"]
-        bb = BoundingBox(boundingBox["Width"], boundingBox["Height"],
-                         boundingBox["Left"], boundingBox["Top"])
+        bb = BoundingBox(boundingBox["Width"], boundingBox["Height"], boundingBox["Left"], boundingBox["Top"])
         pgs = []
         for pg in polygon:
             pgs.append(Polygon(pg["X"], pg["Y"]))
 
         self._boundingBox = bb
         self._polygon = pgs
 
@@ -116,19 +131,21 @@
 
     @property
     def polygon(self):
         return self._polygon
 
 
 class Word(BaseBlock):
+
     def __init__(self, block, blockMap):
         super().__init__(block, blockMap)
 
 
 class Line(BaseBlock):
+
     def __init__(self, block, blockMap):
         super().__init__(block, blockMap)
 
         self._words = []
         if ('Relationships' in block and block['Relationships']):
             for rs in block['Relationships']:
                 if (rs['Type'] == 'CHILD'):
@@ -140,22 +157,21 @@
         s = "Line\n==========\n"
         s = s + self._text + "\n"
         s = s + "Words\n----------\n"
         for word in self._words:
             s = s + "[{}]".format(str(word))
         return s
 
-
     @property
     def words(self):
         return self._words
 
 
-
 class SelectionElement:
+
     def __init__(self, block, blockMap):
         self._confidence = block['Confidence']
         self._geometry = Geometry(block['Geometry'])
         self._id = block['Id']
         self._selectionStatus = block['SelectionStatus']
 
     @property
@@ -172,14 +188,15 @@
 
     @property
     def selectionStatus(self):
         return self._selectionStatus
 
 
 class FieldKey(BaseBlock):
+
     def __init__(self, block, children, blockMap):
         super().__init__(block, blockMap)
         self._content = []
 
         t = []
 
         for eid in children:
@@ -188,21 +205,21 @@
                 w = Word(wb, blockMap)
                 self._content.append(w)
                 t.append(w.text)
 
         if (t):
             self._text = ' '.join(t)
 
-
     @property
     def content(self):
         return self._content
 
 
 class FieldValue(BaseBlock):
+
     def __init__(self, block, children, blockMap):
         super().__init__(block, blockMap)
         self._content = []
 
         t = []
 
         for eid in children:
@@ -215,38 +232,40 @@
                 se = SelectionElement(wb, blockMap)
                 self._content.append(se)
                 self._text = se.selectionStatus
 
         if (t):
             self._text = ' '.join(t)
 
-
     @property
     def content(self):
         return self._content
 
 
 class Field(BaseBlock):
+
     def __init__(self, block, blockMap):
         super().__init__(block, blockMap)
         self._key = None
         self._value = None
 
-        for item in block['Relationships']:
-            if (item["Type"] == "CHILD"):
-                self._key = FieldKey(block, item['Ids'], blockMap)
-            elif (item["Type"] == "VALUE"):
-                for eid in item['Ids']:
-                    vkvs = blockMap[eid]
-                    if 'VALUE' in vkvs['EntityTypes']:
-                        if ('Relationships' in vkvs):
-                            for vitem in vkvs['Relationships']:
-                                if (vitem["Type"] == "CHILD"):
-                                    self._value = FieldValue(
-                                        vkvs, vitem['Ids'], blockMap)
+        if 'Relationships' in block:
+            for item in block['Relationships']:
+                if (item["Type"] == "CHILD"):
+                    self._key = FieldKey(block, item['Ids'], blockMap)
+                elif (item["Type"] == "VALUE"):
+                    for eid in item['Ids']:
+                        vkvs = blockMap[eid]
+                        if 'VALUE' in vkvs['EntityTypes']:
+                            if ('Relationships' in vkvs):
+                                for vitem in vkvs['Relationships']:
+                                    if (vitem["Type"] == "CHILD"):
+                                        self._value = FieldValue(vkvs, vitem['Ids'], blockMap)
+        else:
+            logger.warning(f"no 'Relationships' in block: {block}")
 
     def __str__(self):
         s = "\nField\n==========\n"
         k = ""
         v = ""
         if (self._key):
             k = str(self._key)
@@ -261,14 +280,15 @@
 
     @property
     def value(self):
         return self._value
 
 
 class Form:
+
     def __init__(self):
         self._fields = []
         self._fieldsMap = {}
 
     def addField(self, field):
         self._fields.append(field)
         self._fieldsMap[field.key.text] = field
@@ -294,35 +314,25 @@
         results = []
         for field in self._fields:
             if (field.key and searchKey in field.key.text.lower()):
                 results.append(field)
         return results
 
 
-class Cell(BaseBlock):
+class BaseCell(BaseBlock):
+
     def __init__(self, block, blockMap):
         super().__init__(block, blockMap)
         self._rowIndex = block['RowIndex']
         self._columnIndex = block['ColumnIndex']
         self._rowSpan = block['RowSpan']
         self._columnSpan = block['ColumnSpan']
         self._content = []
-        if ('Relationships' in block and block['Relationships']):
-            for rs in block['Relationships']:
-                if (rs['Type'] == 'CHILD'):
-                    for cid in rs['Ids']:
-                        blockType = blockMap[cid]["BlockType"]
-                        if (blockType == "WORD"):
-                            w = Word(blockMap[cid], blockMap)
-                            self._content.append(w)
-                            self._text = self._text + w.text + ' '
-                        elif (blockType == "SELECTION_ELEMENT"):
-                            se = SelectionElement(blockMap[cid], blockMap)
-                            self._content.append(se)
-                            self._text = self._text + se.selectionStatus + ', '
+        self._entityTypes: List[str] = list()
+        self._isChildOfMergedCell = False
 
     @property
     def rowIndex(self):
         return self._rowIndex
 
     @property
     def columnIndex(self):
@@ -336,64 +346,191 @@
     def columnSpan(self):
         return self._columnSpan
 
     @property
     def content(self):
         return self._content
 
+    @property
+    def entityTypes(self):
+        """at the moment for COLUMN_HEADER"""
+        return self._entityTypes
+
+
+class Cell(BaseCell):
+
+    def __init__(self, block, blockMap):
+        super().__init__(block, blockMap)
+        self._mergedText = None
+        self._mergedCellParent: MergedCell
+
+        if 'Relationships' in block and block['Relationships']:
+            for rs in block['Relationships']:
+                if rs['Type'] == 'CHILD':
+                    for cid in rs['Ids']:
+                        blockType = blockMap[cid]["BlockType"]
+                        if (blockType == "WORD"):
+                            w = Word(blockMap[cid], blockMap)
+                            self._content.append(w)
+                            self._text = self._text + w.text + ' '
+                        elif (blockType == "SELECTION_ELEMENT"):
+                            se = SelectionElement(blockMap[cid], blockMap)
+                            self._content.append(se)
+                            self._text = self._text + se.selectionStatus + ', '
+        if ('EntityTypes' in block and block['EntityTypes']):
+            self._entityTypes = block['EntityTypes']
+
+    @property
+    def mergedText(self):
+        if self._isChildOfMergedCell and self._mergedCellParent != None:
+            return self._mergedCellParent._text.strip()
+        else:
+            return self._text.strip()
+
+
+class MergedCell(BaseCell):
+
+    def __init__(self, block, blockMap, rows):
+        super().__init__(block, blockMap)
+        self._rowIndex = block['RowIndex']
+        self._columnIndex = block['ColumnIndex']
+        self._rowSpan = block['RowSpan']
+        self._columnSpan = block['ColumnSpan']
+        self._entityTypes: List[str] = list()
+        if 'Relationships' in block and block['Relationships']:
+            for rs in block['Relationships']:
+                if rs['Type'] == 'CHILD':
+                    cells = []
+                    for row in rows:
+                        cells.extend(row._cells)
+                    for cid in rs['Ids']:
+                        blockType = blockMap[cid]["BlockType"]
+                        if (blockType == "CELL"):
+                            child_cell = next((x for x in cells if x.id == cid), None)
+                            if child_cell != None:
+                                child_cell._isChildOfMergedCell = True
+                                child_cell._mergedCellParent = self
+                                if len(self._text) == 0 and len(child_cell.text) > 0:
+                                    self._text = child_cell.text.strip()
+        if ('EntityTypes' in block and block['EntityTypes']):
+            self._entityTypes = block['EntityTypes']
 
 
 class Row:
+
     def __init__(self):
-        self._cells = []
+        self._cells: List[Cell] = []
 
     def __str__(self):
         s = ""
         for cell in self._cells:
             s = s + "[{}]".format(str(cell))
         return s
 
     @property
     def cells(self):
         return self._cells
 
+    @cells.setter
+    def cells(self, cells: List[Cell]):
+        self._cells = cells
+
+    @property
+    def merged_cells(self):
+        return self._cells
+
 
 class Table(BaseBlock):
+
     def __init__(self, block, blockMap):
         super().__init__(block, blockMap)
-        self._rows = []
-        ri = 1
-        row = Row()
-        cell = None
+        self._rows: List[Row] = []
+        self._merged_cells: List[MergedCell] = []
+        self._merged_cells_ids = []
         if ('Relationships' in block and block['Relationships']):
             for rs in block['Relationships']:
                 if (rs['Type'] == 'CHILD'):
+                    cells: List[Cell] = list()
                     for cid in rs['Ids']:
                         cell = Cell(blockMap[cid], blockMap)
-                        if (cell.rowIndex > ri):
-                            self._rows.append(row)
-                            row = Row()
-                            ri = cell.rowIndex
-                        row.cells.append(cell)
-                    if (row and row.cells):
-                        self._rows.append(row)
+                        cells.append(cell)
+                    cells.sort(key=lambda cell: (cell.rowIndex, cell.columnIndex))
+                    for row_index in range(1, max([x.rowIndex for x in cells]) + 1):
+                        new_row: Row = Row()
+                        new_row.cells = [x for x in cells if x.rowIndex == row_index]
+                        self._rows.append(new_row)
+                elif (rs['Type'] == 'MERGED_CELL'):
+                    self._merged_cells_ids = rs['Ids']
+
+            if len(self._merged_cells_ids) > 0:
+                self._resolve_merged_cells(blockMap)
 
     def __str__(self):
         s = "Table\n==========\n"
         for row in self._rows:
             s = s + "Row\n==========\n"
             s = s + str(row) + "\n"
         return s
 
+    def _resolve_merged_cells(self, blockMap):
+        for cid in self._merged_cells_ids:
+            merged_cell = MergedCell(blockMap[cid], blockMap, self._rows)
+            self._merged_cells.append(merged_cell)
+
+    def get_header_field_names(self):
+        header_cells = self.header
+        header_names = []
+        for header in header_cells:
+            s = []
+            for cell in header:
+                if cell._isChildOfMergedCell:
+                    s.append(cell.mergedText.strip())
+                else:
+                    s.append(cell.text.strip())
+            header_names.append(s)
+        return header_names
+
     @property
-    def rows(self):
+    def rows(self) -> List[Row]:
         return self._rows
 
+    @property
+    def header(self) -> List[List[Cell]]:
+        header_rows = []
+        for row in self._rows:
+            header_cells: List[Cell] = list()
+            for cell in row.cells:
+                for entity_type in cell.entityTypes:
+                    if entity_type == ENTITY_TYPE_COLUMN_HEADER:
+                        header_cells.append(cell)
+            if (len(header_cells) > 0):
+                header_rows.append(header_cells)
+
+        return header_rows
+
+    @property
+    def rows_without_header(self) -> List[Row]:
+        non_header_rows: List[Row] = list()
+        for row in self.rows:
+            header = False
+            for cell in row.cells:
+                for entity_type in cell.entityTypes:
+                    if entity_type == ENTITY_TYPE_COLUMN_HEADER:
+                        header = True
+            if not header:
+                non_header_rows.append(row)
+        return non_header_rows
+
+    @property
+    def merged_cells(self) -> List[MergedCell]:
+        return self._merged_cells
+
 
 class Page:
+
     def __init__(self, blocks, blockMap):
         self._blocks = blocks
         self._text = ""
         self._lines = []
         self._form = Form()
         self._tables = []
         self._content = []
@@ -430,39 +567,34 @@
                         self._form.addField(f)
                         self._content.append(f)
                     else:
                         logger.info(
                             f"INFO: Detected K/V where key does not have content. Excluding key from output. {f} - {item}"
                         )
 
-
     def getLinesInReadingOrder(self):
         columns = []
         lines = []
         for item in self._lines:
             column_found = False
             for index, column in enumerate(columns):
                 bbox_left = item.geometry.boundingBox.left
                 bbox_right = item.geometry.boundingBox.left + item.geometry.boundingBox.width
                 bbox_centre = item.geometry.boundingBox.left + item.geometry.boundingBox.width / 2
                 column_centre = column['left'] + column['right'] / 2
-                if (bbox_centre > column['left'] and bbox_centre <
-                        column['right']) or (column_centre > bbox_left
-                                             and column_centre < bbox_right):
+                if (bbox_centre > column['left'] and bbox_centre < column['right']) or (column_centre > bbox_left
+                                                                                        and column_centre < bbox_right):
                     #Bbox appears inside the column
                     lines.append([index, item.text])
                     column_found = True
                     break
             if not column_found:
                 columns.append({
-                    'left':
-                    item.geometry.boundingBox.left,
-                    'right':
-                    item.geometry.boundingBox.left +
-                    item.geometry.boundingBox.width
+                    'left': item.geometry.boundingBox.left,
+                    'right': item.geometry.boundingBox.left + item.geometry.boundingBox.width
                 })
                 lines.append([len(columns) - 1, item.text])
 
         lines.sort(key=lambda x: x[0])
         return lines
 
     def getTextInReadingOrder(self):
@@ -506,14 +638,15 @@
 
     @property
     def custom(self):
         return self._custom
 
 
 class Document:
+
     def __init__(self, responsePages):
 
         if (not isinstance(responsePages, list)):
             rps = []
             rps.append(responsePages)
             responsePages = rps
 
@@ -541,23 +674,25 @@
 
                 if (block['BlockType'] == 'PAGE'):
                     if (documentPage):
                         documentPages.append({"Blocks": documentPage})
                     documentPage = []
                     documentPage.append(block)
                 else:
-                    documentPage.append(block)
+                    if documentPage:
+                        documentPage.append(block)
+                    else:
+                        logger.error("assumed documentPage not None, but was None")
         if (documentPage):
             documentPages.append({"Blocks": documentPage})
         return documentPages, blockMap
 
     def _parse(self):
 
-        self._responseDocumentPages, self._blockMap = self._parseDocumentPagesAndBlockMap(
-        )
+        self._responseDocumentPages, self._blockMap = self._parseDocumentPagesAndBlockMap()
         for documentPage in self._responseDocumentPages:
             page = Page(documentPage["Blocks"], self._blockMap)
             self._pages.append(page)
 
     @property
     def blocks(self):
         return self._responsePages
```

