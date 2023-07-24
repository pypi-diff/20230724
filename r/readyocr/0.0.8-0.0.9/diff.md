# Comparing `tmp/readyocr-0.0.8.tar.gz` & `tmp/readyocr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyocr-0.0.8.tar", last modified: Tue Jul 18 03:54:12 2023, max compression
+gzip compressed data, was "readyocr-0.0.9.tar", last modified: Tue Jul 18 08:29:16 2023, max compression
```

## Comparing `readyocr-0.0.8.tar` & `readyocr-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.729426 readyocr-0.0.8/
--rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.8/LICENSE
--rw-r--r--   0 annguyen   (501) staff       (20)     5273 2023-07-18 03:54:12.729266 readyocr-0.0.8/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     3517 2023-07-18 03:52:51.000000 readyocr-0.0.8/README.md
--rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-18 03:53:05.000000 readyocr-0.0.8/pyproject.toml
--rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-18 03:54:12.729479 readyocr-0.0.8/setup.cfg
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.717564 readyocr-0.0.8/src/
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.719091 readyocr-0.0.8/src/readyocr/
--rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.8/src/readyocr/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.8/src/readyocr/__main__.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.726919 readyocr-0.0.8/src/readyocr/entities/
--rw-r--r--   0 annguyen   (501) staff       (20)      673 2023-07-07 07:27:48.000000 readyocr-0.0.8/src/readyocr/entities/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)     6272 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/bbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.8/src/readyocr/entities/block.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2010 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3299 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/document.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.8/src/readyocr/entities/entity_list.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-07 09:42:13.000000 readyocr-0.0.8/src/readyocr/entities/entity_tag.py
--rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.8/src/readyocr/entities/key.py
--rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.8/src/readyocr/entities/line.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2098 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/merged_cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3314 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/page.py
--rw-r--r--   0 annguyen   (501) staff       (20)     5142 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/page_entity.py
--rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.8/src/readyocr/entities/paragraph.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1241 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/table.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2211 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/textbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.8/src/readyocr/entities/value.py
--rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.8/src/readyocr/entities/word.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.8/src/readyocr/exceptions.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.727877 readyocr-0.0.8/src/readyocr/parsers/
--rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.8/src/readyocr/parsers/google_document_ai_parser.py
--rw-r--r--   0 annguyen   (501) staff       (20)     7781 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/parsers/readyocr_parser.py
--rw-r--r--   0 annguyen   (501) staff       (20)     7360 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/parsers/textract_parser.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.728818 readyocr-0.0.8/src/readyocr/utils/
--rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.8/src/readyocr/utils/geometry_utils.py
--rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.8/src/readyocr/utils/languages.py
--rw-r--r--   0 annguyen   (501) staff       (20)     4165 2023-07-07 08:41:10.000000 readyocr-0.0.8/src/readyocr/utils/visualize.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.720116 readyocr-0.0.8/src/readyocr.egg-info/
--rw-r--r--   0 annguyen   (501) staff       (20)     5273 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     1074 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/SOURCES.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/dependency_links.txt
--rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/requires.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/top_level.txt
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.218459 readyocr-0.0.9/
+-rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.9/LICENSE
+-rw-r--r--   0 annguyen   (501) staff       (20)     5277 2023-07-18 08:29:16.218306 readyocr-0.0.9/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     3521 2023-07-18 04:17:01.000000 readyocr-0.0.9/README.md
+-rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-18 08:24:20.000000 readyocr-0.0.9/pyproject.toml
+-rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-18 08:29:16.218519 readyocr-0.0.9/setup.cfg
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.208293 readyocr-0.0.9/src/
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.209854 readyocr-0.0.9/src/readyocr/
+-rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.9/src/readyocr/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.9/src/readyocr/__main__.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.216222 readyocr-0.0.9/src/readyocr/entities/
+-rw-r--r--   0 annguyen   (501) staff       (20)      673 2023-07-07 07:27:48.000000 readyocr-0.0.9/src/readyocr/entities/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     6272 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/bbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.9/src/readyocr/entities/block.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2010 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3299 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/document.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.9/src/readyocr/entities/entity_list.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-07 09:42:13.000000 readyocr-0.0.9/src/readyocr/entities/entity_tag.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.9/src/readyocr/entities/key.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.9/src/readyocr/entities/line.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2098 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/merged_cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3314 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/page.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     5141 2023-07-18 08:23:36.000000 readyocr-0.0.9/src/readyocr/entities/page_entity.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.9/src/readyocr/entities/paragraph.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1241 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/table.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2211 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/entities/textbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.9/src/readyocr/entities/value.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.9/src/readyocr/entities/word.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.9/src/readyocr/exceptions.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.217188 readyocr-0.0.9/src/readyocr/parsers/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.9/src/readyocr/parsers/google_document_ai_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7776 2023-07-18 08:23:34.000000 readyocr-0.0.9/src/readyocr/parsers/readyocr_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7360 2023-07-18 03:36:31.000000 readyocr-0.0.9/src/readyocr/parsers/textract_parser.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.217967 readyocr-0.0.9/src/readyocr/utils/
+-rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.9/src/readyocr/utils/geometry_utils.py
+-rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.9/src/readyocr/utils/languages.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     4165 2023-07-07 08:41:10.000000 readyocr-0.0.9/src/readyocr/utils/visualize.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 08:29:16.210956 readyocr-0.0.9/src/readyocr.egg-info/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5277 2023-07-18 08:29:16.000000 readyocr-0.0.9/src/readyocr.egg-info/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     1074 2023-07-18 08:29:16.000000 readyocr-0.0.9/src/readyocr.egg-info/SOURCES.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-18 08:29:16.000000 readyocr-0.0.9/src/readyocr.egg-info/dependency_links.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-18 08:29:16.000000 readyocr-0.0.9/src/readyocr.egg-info/requires.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-18 08:29:16.000000 readyocr-0.0.9/src/readyocr.egg-info/top_level.txt
```

### Comparing `readyocr-0.0.8/LICENSE` & `readyocr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/PKG-INFO` & `readyocr-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.8
+Version: 0.0.9
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -101,39 +101,40 @@
     cell.tags.add('COLUMN_HEADER')
     table.children.add(cell)
 
     # Get all table cell which is column header
     table.children.filter_by_tags('COLUMN_HEADER') 
     ```
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    # python object -> python dict
+    dict_resp = document.export_json()
+
+    # python dict -> python object
+    same_document = load(dict_resp)
+    ```
+
 * ReadyOCR support visualize for bounding box and textbox
 
     ```
     for item in page.descendants.filter_by_class(Line):
         visualize_image = draw_textbox(
             image=visualize_image, 
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
-* ReadyOCR support export json object and also load from same json object
-
-    ```
-    from readyocr.parsers.readyocr_parser import load
-
-    ...
-    dict_resp = document.export_json()
-
-    #TODO: finish load function, please refer to Textract Package
-    same_document = load(dict_resp)
-    ```
-
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.8/README.md` & `readyocr-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,39 +74,40 @@
     cell.tags.add('COLUMN_HEADER')
     table.children.add(cell)
 
     # Get all table cell which is column header
     table.children.filter_by_tags('COLUMN_HEADER') 
     ```
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    # python object -> python dict
+    dict_resp = document.export_json()
+
+    # python dict -> python object
+    same_document = load(dict_resp)
+    ```
+
 * ReadyOCR support visualize for bounding box and textbox
 
     ```
     for item in page.descendants.filter_by_class(Line):
         visualize_image = draw_textbox(
             image=visualize_image, 
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
-* ReadyOCR support export json object and also load from same json object
-
-    ```
-    from readyocr.parsers.readyocr_parser import load
-
-    ...
-    dict_resp = document.export_json()
-
-    #TODO: finish load function, please refer to Textract Package
-    same_document = load(dict_resp)
-    ```
-
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.8/pyproject.toml` & `readyocr-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "readyocr"
-version = "0.0.8"
+version = "0.0.9"
 description = "A nice package OCR for Amazon Textract and Google Document AI"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name="Sy An", email="syan.vn@gmail.com" },
 ]
 classifiers = [
```

### Comparing `readyocr-0.0.8/src/readyocr/entities/__init__.py` & `readyocr-0.0.9/src/readyocr/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/bbox.py` & `readyocr-0.0.9/src/readyocr/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/block.py` & `readyocr-0.0.9/src/readyocr/entities/block.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/cell.py` & `readyocr-0.0.9/src/readyocr/entities/cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/document.py` & `readyocr-0.0.9/src/readyocr/entities/document.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/entity_list.py` & `readyocr-0.0.9/src/readyocr/entities/entity_list.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/entity_tag.py` & `readyocr-0.0.9/src/readyocr/entities/entity_tag.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/key.py` & `readyocr-0.0.9/src/readyocr/entities/key.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/line.py` & `readyocr-0.0.9/src/readyocr/entities/line.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/merged_cell.py` & `readyocr-0.0.9/src/readyocr/entities/merged_cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/page.py` & `readyocr-0.0.9/src/readyocr/entities/page.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/page_entity.py` & `readyocr-0.0.9/src/readyocr/entities/page_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,9 +182,9 @@
         """
         return {
             "id": self.id,
             "class": self.__class__.__name__,
             "boundingBox": self.bbox.export_json(),
             "metadata": self.metadata,
             "tags": [tag for tag in self.tags],
-            "childrendIds": [child.id for child in self.children]
+            "childrenIds": [child.id for child in self.children]
         }
```

### Comparing `readyocr-0.0.8/src/readyocr/entities/paragraph.py` & `readyocr-0.0.9/src/readyocr/entities/paragraph.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/table.py` & `readyocr-0.0.9/src/readyocr/entities/table.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/textbox.py` & `readyocr-0.0.9/src/readyocr/entities/textbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/value.py` & `readyocr-0.0.9/src/readyocr/entities/value.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/entities/word.py` & `readyocr-0.0.9/src/readyocr/entities/word.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/exceptions.py` & `readyocr-0.0.9/src/readyocr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/parsers/google_document_ai_parser.py` & `readyocr-0.0.9/src/readyocr/parsers/google_document_ai_parser.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/parsers/readyocr_parser.py` & `readyocr-0.0.9/src/readyocr/parsers/readyocr_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #                             "x": 0.052512288093566895,
 #                             "y": 0.8079520590823819,
 #                             "width": 0.05254054814577103,
 #                             "height": 0.009167630081129974
 #                         },
 #                         "metadata": {},
 #                         "tags": [],
-#                         "childrendIds": [
+#                         "childrenIds": [
 #                             "2aced2b4-a20a-427a-83d4-732f79ef378f",
 #                             "1bb89b44-7a35-4466-bb21-0d0c6145c850"
 #                         ],
 #                         "text": "order of:",
 #                         "confidence": 0.9911622619628906,
 #                         "language": null
 #                     },
@@ -66,15 +66,15 @@
                     "x": 0.052512288093566895,
                     "y": 0.8079520590823819,
                     "width": 0.05254054814577103,
                     "height": 0.009167630081129974
                 },
                 "metadata": {},
                 "tags": [],
-                "childrendIds": [
+                "childrenIds": [
                     "2aced2b4-a20a-427a-83d4-732f79ef378f",
                     "1bb89b44-7a35-4466-bb21-0d0c6145c850"
                 ],
                 "text": "order of:",
                 "confidence": 0.9911622619628906,
                 "language": null
             }
@@ -85,15 +85,15 @@
                     "x": 0.4973248541355133,
                     "y": 0.23672433135340398,
                     "width": 0.03262513503432274,
                     "height": 0.009943900668560324
                 },
                 "metadata": {},
                 "tags": [],
-                "childrendIds": [],
+                "childrenIds": [],
                 "text": "date",
                 "confidence": 0.9994115447998047,
                 "language": null
             }
     -> Key: {
                 "id": "ba26e843-759d-4abb-8f45-b75faf577553",
                 "class": "Key",
@@ -101,15 +101,15 @@
                     "x": 0.5765600800514221,
                     "y": 0.3129917424933737,
                     "width": 0.0572432205080986,
                     "height": 0.010077135449113594
                 },
                 "metadata": {},
                 "tags": [],
-                "childrendIds": [
+                "childrenIds": [
                     "b222e6e9-ba9a-47cb-acf9-7845d9ad3c11",
                     "890cbbcd-66d4-4d8d-a4f5-d6ee69c59288",
                     "b3929a99-ee32-4b64-8069-28fc7a822a81",
                     "aec8fc85-e5eb-4f12-af9a-b94c8e0c18a3"
                 ],
                 "text": "key",
                 "confidence": 0.41478912353515623,
@@ -122,15 +122,15 @@
                     "x": 0.24050265550613403,
                     "y": 0.18935537547556613,
                     "width": 0.008100352250039577,
                     "height": 0.008480351599044478
                 },
                 "metadata": {},
                 "tags": [],
-                "childrendIds": [
+                "childrenIds": [
                     "8f6bf718-d569-4941-b74e-f094a86a59dd"
                 ],
                 "text": "value",
                 "confidence": 0.882987060546875,
                 "language": null
             }
     :type entity_json: json
```

### Comparing `readyocr-0.0.8/src/readyocr/parsers/textract_parser.py` & `readyocr-0.0.9/src/readyocr/parsers/textract_parser.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/utils/languages.py` & `readyocr-0.0.9/src/readyocr/utils/languages.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr/utils/visualize.py` & `readyocr-0.0.9/src/readyocr/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.8/src/readyocr.egg-info/PKG-INFO` & `readyocr-0.0.9/src/readyocr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.8
+Version: 0.0.9
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -101,39 +101,40 @@
     cell.tags.add('COLUMN_HEADER')
     table.children.add(cell)
 
     # Get all table cell which is column header
     table.children.filter_by_tags('COLUMN_HEADER') 
     ```
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    # python object -> python dict
+    dict_resp = document.export_json()
+
+    # python dict -> python object
+    same_document = load(dict_resp)
+    ```
+
 * ReadyOCR support visualize for bounding box and textbox
 
     ```
     for item in page.descendants.filter_by_class(Line):
         visualize_image = draw_textbox(
             image=visualize_image, 
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
-* ReadyOCR support export json object and also load from same json object
-
-    ```
-    from readyocr.parsers.readyocr_parser import load
-
-    ...
-    dict_resp = document.export_json()
-
-    #TODO: finish load function, please refer to Textract Package
-    same_document = load(dict_resp)
-    ```
-
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.8/src/readyocr.egg-info/SOURCES.txt` & `readyocr-0.0.9/src/readyocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

