# Comparing `tmp/q2report-0.1.31.tar.gz` & `tmp/q2report-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.31.tar", max compression
+gzip compressed data, was "q2report-0.1.32.tar", max compression
```

## Comparing `q2report-0.1.31.tar` & `q2report-0.1.32.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.31/LICENSE
--rw-r--r--   0        0        0      536 2023-07-21 16:11:28.919106 q2report-0.1.31/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.31/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.31/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.31/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.31/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.31/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.31/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20677 2023-07-21 15:58:27.016880 q2report-0.1.31/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.31/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    30319 2023-07-13 08:40:44.679410 q2report-0.1.31/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.31/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-07-21 16:11:34.573524 q2report-0.1.31/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.31/README.md
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.32/LICENSE
+-rw-r--r--   0        0        0      536 2023-07-24 20:54:04.029178 q2report-0.1.32/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.32/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.32/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.32/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.32/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.32/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.32/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20677 2023-07-21 15:58:27.016880 q2report-0.1.32/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.32/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    31040 2023-07-24 20:45:33.537327 q2report-0.1.32/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.32/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-07-24 20:54:06.238873 q2report-0.1.32/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.32/README.md
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.32/PKG-INFO
```

### Comparing `q2report-0.1.31/LICENSE` & `q2report-0.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/pyproject.toml` & `q2report-0.1.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.31"
+version = "0.1.32"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pillow = "^9.4.0"
```

### Comparing `q2report-0.1.31/q2report/q2printer/docx_parts.py` & `q2report-0.1.32/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2printer/q2printer.py` & `q2report-0.1.32/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.32/q2report/q2printer/q2printer_docx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2printer/q2printer_html.py` & `q2report-0.1.32/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.32/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.32/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/q2report/q2report.py` & `q2report-0.1.32/q2report/q2report.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,16 +242,18 @@
     default_cell = {
         "data": "",
         "style": {},
         "rowspan": 0,
         "colspan": 0,
     }
 
-    def __init__(self):
+    def __init__(self, style={}):
         self.report_content = {}
+        if style:
+            self.set_style(style)
         self.printer = None
         self.params = {}
         self.prevrowdata = {}
         self.use_prevrowdata = False
         self.mydata = mydata(self)
         self.table_aggregators = {}
         self.table_group_aggregators = []
@@ -283,14 +285,15 @@
         font_family=None,
         font_size=None,
         font_weight=None,
         border_width=None,
         padding=None,
         text_align=None,
         vertical_align=None,
+        alignment=None,
     ):
         """_summary_
 
         Args:
             font_family (str, optional): e.g. "Arial". Defaults to None.
             font_size (str, int, float, optional): font size in pt, e.g. 12, 12.5, "12.5" . Defaults to None.
             font_weight str, optional): "bold" or "". Defaults to None.
@@ -313,14 +316,30 @@
             style["border-width"] = border_width
         if padding:
             style["padding"] = padding
         if text_align:
             style["text-align"] = text_align
         if vertical_align:
             style["vertical-align"] = vertical_align
+        if alignment is not None:
+            alignment = num(alignment)
+            if alignment in (7, 4, 1, 0, -1):
+                style["text-align"] = "left"
+            elif alignment in (9, 6, 3):
+                style["text-align"] = "right"
+            else:
+                style["text-align"] = "center"
+
+            if alignment in (7, 8, 9, 0, -1):
+                style["vertical-align"] = "top"
+            elif alignment in (1, 2, 3):
+                style["vertical-align"] = "bottom"
+            else:
+                style["vertical-align"] = "middle"
+
         return style
 
     def set_style(self, style=None):
         if style is None or not isinstance(style, dict):
             return
         if "style" not in self.report_content:
             self.report_content["style"] = deepcopy(self.default_style)
@@ -651,15 +670,16 @@
                             self.render_table_groups(rows_section, column_style)
                             self.aggregators_calc()
                             self.outline_level += 1
                             self.render_rows_section(rows_section, column_style)
                             self.outline_level -= 1
                             self.prevrowdata.update(data_row)
 
-                            self.data_step()
+                            if self.data_step():
+                                break
                         self.data_stop()
 
                         self.render_table_groups(rows_section, column_style, True)
                         self.render_table_footer(rows_section, column_style)
                     else:  # Free rows
                         self.render_rows_section(rows_section, column_style)
```

### Comparing `q2report-0.1.31/q2report/q2utils.py` & `q2report-0.1.32/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/README.md` & `q2report-0.1.32/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.31/PKG-INFO` & `q2report-0.1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.31
+Version: 0.1.32
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

