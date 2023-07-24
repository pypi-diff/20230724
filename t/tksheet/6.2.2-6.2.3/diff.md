# Comparing `tmp/tksheet-6.2.2.tar.gz` & `tmp/tksheet-6.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.2.2.tar", last modified: Mon Jul 10 09:13:21 2023, max compression
+gzip compressed data, was "tksheet-6.2.3.tar", last modified: Mon Jul 24 07:29:53 2023, max compression
```

## Comparing `tksheet-6.2.2.tar` & `tksheet-6.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.217928 tksheet-6.2.2/
--rw-rw-rw-   0        0        0     1101 2023-07-09 07:20:56.000000 tksheet-6.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-07-10 09:13:21.217928 tksheet-6.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-07-09 07:20:56.000000 tksheet-6.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-07-10 09:13:21.218930 tksheet-6.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-07-09 07:23:02.000000 tksheet-6.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.207333 tksheet-6.2.2/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/__init__.py
--rw-rw-rw-   0        0        0   165253 2023-07-09 18:18:57.000000 tksheet-6.2.2/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   112139 2023-07-09 17:19:23.000000 tksheet-6.2.2/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8880 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   334327 2023-07-09 17:31:47.000000 tksheet-6.2.2/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12733 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   109067 2023-07-09 17:20:47.000000 tksheet-6.2.2/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5784 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    60025 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.217928 tksheet-6.2.2/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2023-07-24 07:29:53.819976 tksheet-6.2.3/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2023-05-23 12:03:48.000000 tksheet-6.2.3/LICENSE.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3601 2023-07-24 07:29:53.819976 tksheet-6.2.3/PKG-INFO
+-rw-r--r--   0 rg        (1000) rg        (1000)     3007 2023-07-23 17:32:48.000000 tksheet-6.2.3/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)       79 2023-07-24 07:29:53.819976 tksheet-6.2.3/setup.cfg
+-rw-r--r--   0 rg        (1000) rg        (1000)     1027 2023-07-24 07:23:48.000000 tksheet-6.2.3/setup.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2023-07-24 07:29:53.819976 tksheet-6.2.3/tksheet/
+-rw-r--r--   0 rg        (1000) rg        (1000)     1989 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/__init__.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   165250 2023-07-23 17:33:54.000000 tksheet-6.2.3/tksheet/_tksheet.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   112139 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_column_headers.py
+-rw-r--r--   0 rg        (1000) rg        (1000)     9211 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_formatters.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   334327 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_main_table.py
+-rw-r--r--   0 rg        (1000) rg        (1000)    12733 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_other_classes.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   109067 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_row_index.py
+-rw-r--r--   0 rg        (1000) rg        (1000)     5784 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_top_left_rectangle.py
+-rw-r--r--   0 rg        (1000) rg        (1000)    60025 2023-07-23 17:32:48.000000 tksheet-6.2.3/tksheet/_tksheet_vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2023-07-24 07:29:53.819976 tksheet-6.2.3/tksheet.egg-info/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3601 2023-07-24 07:29:53.000000 tksheet-6.2.3/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      429 2023-07-24 07:29:53.000000 tksheet-6.2.3/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2023-07-24 07:29:53.000000 tksheet-6.2.3/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2023-07-24 07:29:53.000000 tksheet-6.2.3/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.2.2/LICENSE.txt` & `tksheet-6.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/PKG-INFO` & `tksheet-6.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-Metadata-Version: 2.1
-Name: tksheet
-Version: 6.2.2
-Summary: Tkinter table / sheet widget
-Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.2.tar.gz
-Author: ragardner
-Author-email: github@ragardner.simplelogin.com
-License: MIT
-Keywords: tkinter,table,widget,sheet,grid,tk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
-
-## **Python tkinter table widget**
-
-----
-
-```python
-#To install using pip
-pip install tksheet
-
-#To update using pip
-pip install tksheet --upgrade
-```
-
-## **Help**
-
-----
-
-- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
-- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
-- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
-- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
-- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
-
-### **NOTICE:** 
-With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
-
-## **Features**
-
-----
-
-- Display and modify tabular data
-- Stores its display data as a Python list of lists, sublists being rows
-- Runs smoothly even with millions of rows/columns
-- Edit cells directly
-- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
-- Drag and drop columns and rows
-- Multiple line header and index cells
-- Expand row heights and column widths
-- Change fonts and font size (not for individual cells)
-- Change any colors in the sheet
-- Create an unlimited number of high performance dropdown and check boxes
-- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
-- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
-
-### **light blue theme**
-
-----
-
-![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
-
-### **black theme**
-
-----
-
-![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+Metadata-Version: 2.1
+Name: tksheet
+Version: 6.2.3
+Summary: Tkinter table / sheet widget
+Home-page: https://github.com/ragardner/tksheet
+Author: ragardner
+Author-email: github@ragardner.simplelogin.com
+License: MIT
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.3.tar.gz
+Keywords: tkinter,table,widget,sheet,grid,tk
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
+
+## **Python tkinter table widget**
+
+----
+
+```python
+#To install using pip
+pip install tksheet
+
+#To update using pip
+pip install tksheet --upgrade
+```
+
+## **Help**
+
+----
+
+- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
+- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
+- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
+
+### **NOTICE:** 
+With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
+
+## **Features**
+
+----
+
+- Display and modify tabular data
+- Stores its display data as a Python list of lists, sublists being rows
+- Runs smoothly even with millions of rows/columns
+- Edit cells directly
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
+- Drag and drop columns and rows
+- Multiple line header and index cells
+- Expand row heights and column widths
+- Change fonts and font size (not for individual cells)
+- Change any colors in the sheet
+- Create an unlimited number of high performance dropdown and check boxes
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
+- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
+
+### **light blue theme**
+
+----
+
+![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
+
+### **black theme**
+
+----
+
+![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+
```

### Comparing `tksheet-6.2.2/README.md` & `tksheet-6.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/__init__.py` & `tksheet-6.2.3/tksheet/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# ruff: noqa: F401
-# ruff: noqa: F403
-from ._tksheet import Sheet, Sheet_Dropdown
-from ._tksheet_column_headers import ColumnHeaders
-from ._tksheet_formatters import (
-    Formatter,
-    bool_formatter,
-    bool_to_str,
-    data_to_str,
-    float_formatter,
-    float_to_str,
-    format_data,
-    formatter,
-    get_clipboard_data,
-    get_data_with_valid_check,
-    int_formatter,
-    is_bool_like,
-    is_none_like,
-    percentage_formatter,
-    percentage_to_str,
-    to_bool,
-    to_float,
-    to_int,
-    to_str,
-    try_to_bool,
-)
-from ._tksheet_main_table import MainTable
-from ._tksheet_other_classes import (
-    BeginDragDropEvent,
-    CtrlKeyEvent,
-    CurrentlySelectedClass,
-    DeleteRowColumnEvent,
-    DeselectionEvent,
-    DraggedRowColumn,
-    DrawnItem,
-    DropDownModifiedEvent,
-    EditCellEvent,
-    EditHeaderEvent,
-    EditIndexEvent,
-    EndDragDropEvent,
-    GeneratedMouseEvent,
-    InsertEvent,
-    PasteEvent,
-    ResizeEvent,
-    SelectCellEvent,
-    SelectColumnEvent,
-    SelectionBoxEvent,
-    SelectRowEvent,
-    TextCfg,
-    TextEditor,
-    TextEditor_,
-    UndoEvent,
-    _ProgBar,
-    dropdown_search_function,
-    get_checkbox_dict,
-    get_checkbox_kwargs,
-    get_dropdown_dict,
-    get_dropdown_kwargs,
-    get_index_of_gap_in_sorted_integer_seq_forward,
-    get_index_of_gap_in_sorted_integer_seq_reverse,
-    get_n2a,
-    get_seq_without_gaps_at_index,
-    is_iterable,
-    num2alpha,
-)
-from ._tksheet_row_index import RowIndex
-from ._tksheet_top_left_rectangle import TopLeftRectangle
-from ._tksheet_vars import (
-    USER_OS,
-    Color_Map_,
-    arrowkey_bindings_helper,
-    ctrl_key,
-    emitted_events,
-    falsy,
-    get_font,
-    get_heading_font,
-    get_index_font,
-    nonelike,
-    rc_binding,
-    symbols_set,
-    theme_black,
-    theme_dark,
-    theme_dark_blue,
-    theme_dark_green,
-    theme_light_blue,
-    theme_light_green,
-    truthy,
-)
+# ruff: noqa: F401
+# ruff: noqa: F403
+from ._tksheet import Sheet, Sheet_Dropdown
+from ._tksheet_column_headers import ColumnHeaders
+from ._tksheet_formatters import (
+    Formatter,
+    bool_formatter,
+    bool_to_str,
+    data_to_str,
+    float_formatter,
+    float_to_str,
+    format_data,
+    formatter,
+    get_clipboard_data,
+    get_data_with_valid_check,
+    int_formatter,
+    is_bool_like,
+    is_none_like,
+    percentage_formatter,
+    percentage_to_str,
+    to_bool,
+    to_float,
+    to_int,
+    to_str,
+    try_to_bool,
+)
+from ._tksheet_main_table import MainTable
+from ._tksheet_other_classes import (
+    BeginDragDropEvent,
+    CtrlKeyEvent,
+    CurrentlySelectedClass,
+    DeleteRowColumnEvent,
+    DeselectionEvent,
+    DraggedRowColumn,
+    DrawnItem,
+    DropDownModifiedEvent,
+    EditCellEvent,
+    EditHeaderEvent,
+    EditIndexEvent,
+    EndDragDropEvent,
+    GeneratedMouseEvent,
+    InsertEvent,
+    PasteEvent,
+    ResizeEvent,
+    SelectCellEvent,
+    SelectColumnEvent,
+    SelectionBoxEvent,
+    SelectRowEvent,
+    TextCfg,
+    TextEditor,
+    TextEditor_,
+    UndoEvent,
+    _ProgBar,
+    dropdown_search_function,
+    get_checkbox_dict,
+    get_checkbox_kwargs,
+    get_dropdown_dict,
+    get_dropdown_kwargs,
+    get_index_of_gap_in_sorted_integer_seq_forward,
+    get_index_of_gap_in_sorted_integer_seq_reverse,
+    get_n2a,
+    get_seq_without_gaps_at_index,
+    is_iterable,
+    num2alpha,
+)
+from ._tksheet_row_index import RowIndex
+from ._tksheet_top_left_rectangle import TopLeftRectangle
+from ._tksheet_vars import (
+    USER_OS,
+    Color_Map_,
+    arrowkey_bindings_helper,
+    ctrl_key,
+    emitted_events,
+    falsy,
+    get_font,
+    get_heading_font,
+    get_index_font,
+    nonelike,
+    rc_binding,
+    symbols_set,
+    theme_black,
+    theme_dark,
+    theme_dark_blue,
+    theme_dark_green,
+    theme_light_blue,
+    theme_light_green,
+    truthy,
+)
```

### Comparing `tksheet-6.2.2/tksheet/_tksheet.py` & `tksheet-6.2.3/tksheet/_tksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -3678,15 +3678,15 @@
         formatter_options={},
         formatter_class=None,
         redraw=True,
         **kwargs,
     ):
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(len(self.MT.data)):
-                self.MT.format_column(r_, **{"formatter": formatter_class, **formatter_options, **kwargs})
+                self.MT.format_row(r_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         elif is_iterable(r):
             for r_ in r:
                 self.MT.format_row(r_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         else:
             self.MT.format_row(r, **{"formatter": formatter_class, **formatter_options, **kwargs})
         self.set_refresh_timer(redraw)
```

### Comparing `tksheet-6.2.2/tksheet/_tksheet_column_headers.py` & `tksheet-6.2.3/tksheet/_tksheet_column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/_tksheet_formatters.py` & `tksheet-6.2.3/tksheet/_tksheet_formatters.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-from __future__ import annotations
-
-from typing import Any, Union, Dict
-
-from ._tksheet_vars import (
-    falsy,
-    nonelike,
-    truthy,
-)
-
-
-def is_none_like(n: Any):
-    if (isinstance(n, str) and n.lower().replace(" ", "") in nonelike) or n in nonelike:
-        return True
-    return False
-
-
-def to_int(x: Any, **kwargs):
-    if isinstance(x, int):
-        return x
-    return int(float(x))
-
-
-def to_float(x: Any, **kwargs):
-    if isinstance(x, float):
-        return x
-    if isinstance(x, str) and x.endswith("%"):
-        return float(x.replace("%", "")) / 100
-    return float(x)
-
-
-def to_bool(val: Any, **kwargs):
-    if type(val) == bool:
-        return val
-    if isinstance(val, str):
-        v = val.lower()
-    else:
-        v = val
-    if "truthy" in kwargs:
-        _truthy = kwargs["truthy"]
-    else:
-        _truthy = truthy
-    if "falsy" in kwargs:
-        _falsy = kwargs["falsy"]
-    else:
-        _falsy = falsy
-    if v in _truthy:
-        return True
-    elif v in _falsy:
-        return False
-    raise ValueError(f'Cannot map "{val}" to bool.')
-
-
-def try_to_bool(val: Any, **kwargs):
-    try:
-        return to_bool(val)
-    except Exception:
-        return val
-
-
-def is_bool_like(v: Any, **kwargs):
-    try:
-        to_bool(v)
-        return True
-    except Exception:
-        return False
-
-
-def to_str(v: Any, **kwargs: Dict) -> str:
-    return f"{v}"
-
-
-def float_to_str(v: Union[int, float], **kwargs: Dict) -> str:
-    if isinstance(v, float):
-        if v.is_integer():
-            return f"{int(v)}"
-        if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
-            if kwargs["decimals"]:
-                return f"{round(v, kwargs['decimals'])}"
-            return f"{int(round(v, kwargs['decimals']))}"
-    return f"{v}"
-
-
-def percentage_to_str(v: Union[int, float], **kwargs: Dict) -> str:
-    if isinstance(v, (int, float)):
-        x = v * 100
-        if isinstance(x, float):
-            if x.is_integer():
-                return f"{int(x)}%"
-            if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
-                if kwargs["decimals"]:
-                    return f"{round(x, kwargs['decimals'])}%"
-                return f"{int(round(x, kwargs['decimals']))}%"
-    return f"{x}%"
-
-
-def bool_to_str(v: Any, **kwargs: Dict) -> str:
-    return f"{v}"
-
-
-def int_formatter(
-    datatypes=int,
-    format_function=to_int,
-    to_str_function=to_str,
-    **kwargs,
-) -> Dict:
-    return formatter(
-        datatypes=datatypes,
-        format_function=format_function,
-        to_str_function=to_str_function,
-        **kwargs,
-    )
-
-
-def float_formatter(
-    datatypes=float,
-    format_function=to_float,
-    to_str_function=float_to_str,
-    decimals=2,
-    **kwargs,
-) -> Dict:
-    return formatter(
-        datatypes=datatypes,
-        format_function=format_function,
-        to_str_function=to_str_function,
-        decimals=decimals,
-        **kwargs,
-    )
-
-
-def percentage_formatter(
-    datatypes=float,
-    format_function=to_float,
-    to_str_function=percentage_to_str,
-    decimals=2,
-    **kwargs,
-) -> Dict:
-    return formatter(
-        datatypes=datatypes,
-        format_function=format_function,
-        to_str_function=to_str_function,
-        decimals=decimals,
-        **kwargs,
-    )
-
-
-def bool_formatter(
-    datatypes=bool,
-    format_function=to_bool,
-    to_str_function=bool_to_str,
-    invalid_value="NA",
-    truthy_values=truthy,
-    falsy_values=falsy,
-    **kwargs,
-) -> Dict:
-    return formatter(
-        datatypes=datatypes,
-        format_function=format_function,
-        to_str_function=to_str_function,
-        invalid_value=invalid_value,
-        truthy_values=truthy_values,
-        falsy_values=falsy_values,
-        **kwargs,
-    )
-
-
-def formatter(
-    datatypes,
-    format_function,
-    to_str_function=to_str,
-    invalid_value="NaN",
-    nullable=True,
-    pre_format_function=None,
-    post_format_function=None,
-    clipboard_function=None,
-    **kwargs,
-) -> Dict:
-    return {
-        **dict(
-            datatypes=datatypes,
-            format_function=format_function,
-            to_str_function=to_str_function,
-            invalid_value=invalid_value,
-            nullable=nullable,
-            pre_format_function=pre_format_function,
-            post_format_function=post_format_function,
-            clipboard_function=clipboard_function,
-        ),
-        **kwargs,
-    }
-
-
-def format_data(
-    value="",
-    datatypes=int,
-    nullable=True,
-    pre_format_function=None,
-    format_function=to_int,
-    post_format_function=None,
-    **kwargs,
-) -> Any:
-    if pre_format_function:
-        value = pre_format_function(value)
-    if nullable and is_none_like(value):
-        value = None
-    else:
-        try:
-            value = format_function(value, **kwargs)
-        except Exception:
-            pass
-    if post_format_function and isinstance(value, datatypes):
-        value = post_format_function(value)
-    return value
-
-
-def data_to_str(
-    value="",
-    datatypes=int,
-    nullable=True,
-    invalid_value="NaN",
-    to_str_function=None,
-    **kwargs,
-) -> str:
-    if not isinstance(value, datatypes):
-        return invalid_value
-    if value is None and nullable:
-        return ""
-    return to_str_function(value, **kwargs)
-
-
-def get_data_with_valid_check(value="", datatypes=tuple(), invalid_value="NA"):
-    if isinstance(value, datatypes):
-        return value
-    return invalid_value
-
-
-def get_clipboard_data(value="", clipboard_function=None, **kwargs):
-    if clipboard_function is not None:
-        return clipboard_function(value, **kwargs)
-    if isinstance(value, (str, int, float, bool)):
-        return value
-    return data_to_str(value, **kwargs)
-
-
-class Formatter:
-    def __init__(
-        self,
-        value,
-        datatypes=int,
-        format_function=to_int,
-        to_str_function=to_str,
-        nullable=True,
-        invalid_value="NaN",
-        pre_format_function=None,
-        post_format_function=None,
-        clipboard_function=None,
-        **kwargs,
-    ):
-        if nullable:
-            if isinstance(datatypes, (list, tuple)):
-                datatypes = tuple({type_ for type_ in datatypes} | {type(None)})
-            else:
-                datatypes = (datatypes, type(None))
-        elif isinstance(datatypes, (list, tuple)) and type(None) in datatypes:
-            raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
-        elif datatypes is type(None):
-            raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
-        self.kwargs = kwargs
-        self.valid_datatypes = datatypes
-        self.format_function = format_function
-        self.to_str_function = to_str_function
-        self.nullable = nullable
-        self.invalid_value = invalid_value
-        self.pre_format_function = pre_format_function
-        self.post_format_function = post_format_function
-        self.clipboard_function = clipboard_function
-        try:
-            self.value = self.format_data(value)
-        except Exception:
-            self.value = f"{value}"
-
-    def __str__(self):
-        if not self.valid():
-            return self.invalid_value
-        if self.value is None and self.nullable:
-            return ""
-        return self.to_str_function(self.value, **self.kwargs)
-
-    def valid(self, value=None) -> bool:
-        if value is None:
-            value = self.value
-        if isinstance(value, self.valid_datatypes):
-            return True
-        return False
-
-    def format_data(self, value):
-        if self.pre_format_function:
-            value = self.pre_format_function(value)
-        value = None if (self.nullable and is_none_like(value)) else self.format_function(value, **self.kwargs)
-        if self.post_format_function and self.valid(value):
-            value = self.post_format_function(value)
-        return value
-
-    def get_data_with_valid_check(self):
-        if self.valid():
-            return self.value
-        return self.invalid_value
-
-    def get_clipboard_data(self):
-        if self.clipboard_function is not None:
-            return self.clipboard_function(self.value, **self.kwargs)
-        if isinstance(self.value, (int, float, bool)):
-            return self.value
-        return self.__str__()
-
-    def __eq__(self, __value) -> bool:
-        # in case of custom formatter class
-        # compare the values
-        try:
-            if hasattr(__value, "value"):
-                return self.value == __value.value
-        except Exception:
-            pass
-        # if comparing to a string, format the string and compare
-        if isinstance(__value, str):
-            try:
-                return self.value == self.format_data(__value)
-            except Exception:
-                pass
-        # if comparing to anything else, compare the values
-        return self.value == __value
+from __future__ import annotations
+
+from typing import Any, Union, Dict
+
+from ._tksheet_vars import (
+    falsy,
+    nonelike,
+    truthy,
+)
+
+
+def is_none_like(n: Any):
+    if (isinstance(n, str) and n.lower().replace(" ", "") in nonelike) or n in nonelike:
+        return True
+    return False
+
+
+def to_int(x: Any, **kwargs):
+    if isinstance(x, int):
+        return x
+    return int(float(x))
+
+
+def to_float(x: Any, **kwargs):
+    if isinstance(x, float):
+        return x
+    if isinstance(x, str) and x.endswith("%"):
+        return float(x.replace("%", "")) / 100
+    return float(x)
+
+
+def to_bool(val: Any, **kwargs):
+    if type(val) == bool:
+        return val
+    if isinstance(val, str):
+        v = val.lower()
+    else:
+        v = val
+    if "truthy" in kwargs:
+        _truthy = kwargs["truthy"]
+    else:
+        _truthy = truthy
+    if "falsy" in kwargs:
+        _falsy = kwargs["falsy"]
+    else:
+        _falsy = falsy
+    if v in _truthy:
+        return True
+    elif v in _falsy:
+        return False
+    raise ValueError(f'Cannot map "{val}" to bool.')
+
+
+def try_to_bool(val: Any, **kwargs):
+    try:
+        return to_bool(val)
+    except Exception:
+        return val
+
+
+def is_bool_like(v: Any, **kwargs):
+    try:
+        to_bool(v)
+        return True
+    except Exception:
+        return False
+
+
+def to_str(v: Any, **kwargs: Dict) -> str:
+    return f"{v}"
+
+
+def float_to_str(v: Union[int, float], **kwargs: Dict) -> str:
+    if isinstance(v, float):
+        if v.is_integer():
+            return f"{int(v)}"
+        if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
+            if kwargs["decimals"]:
+                return f"{round(v, kwargs['decimals'])}"
+            return f"{int(round(v, kwargs['decimals']))}"
+    return f"{v}"
+
+
+def percentage_to_str(v: Union[int, float], **kwargs: Dict) -> str:
+    if isinstance(v, (int, float)):
+        x = v * 100
+        if isinstance(x, float):
+            if x.is_integer():
+                return f"{int(x)}%"
+            if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
+                if kwargs["decimals"]:
+                    return f"{round(x, kwargs['decimals'])}%"
+                return f"{int(round(x, kwargs['decimals']))}%"
+    return f"{x}%"
+
+
+def bool_to_str(v: Any, **kwargs: Dict) -> str:
+    return f"{v}"
+
+
+def int_formatter(
+    datatypes=int,
+    format_function=to_int,
+    to_str_function=to_str,
+    **kwargs,
+) -> Dict:
+    return formatter(
+        datatypes=datatypes,
+        format_function=format_function,
+        to_str_function=to_str_function,
+        **kwargs,
+    )
+
+
+def float_formatter(
+    datatypes=float,
+    format_function=to_float,
+    to_str_function=float_to_str,
+    decimals=2,
+    **kwargs,
+) -> Dict:
+    return formatter(
+        datatypes=datatypes,
+        format_function=format_function,
+        to_str_function=to_str_function,
+        decimals=decimals,
+        **kwargs,
+    )
+
+
+def percentage_formatter(
+    datatypes=float,
+    format_function=to_float,
+    to_str_function=percentage_to_str,
+    decimals=2,
+    **kwargs,
+) -> Dict:
+    return formatter(
+        datatypes=datatypes,
+        format_function=format_function,
+        to_str_function=to_str_function,
+        decimals=decimals,
+        **kwargs,
+    )
+
+
+def bool_formatter(
+    datatypes=bool,
+    format_function=to_bool,
+    to_str_function=bool_to_str,
+    invalid_value="NA",
+    truthy_values=truthy,
+    falsy_values=falsy,
+    **kwargs,
+) -> Dict:
+    return formatter(
+        datatypes=datatypes,
+        format_function=format_function,
+        to_str_function=to_str_function,
+        invalid_value=invalid_value,
+        truthy_values=truthy_values,
+        falsy_values=falsy_values,
+        **kwargs,
+    )
+
+
+def formatter(
+    datatypes,
+    format_function,
+    to_str_function=to_str,
+    invalid_value="NaN",
+    nullable=True,
+    pre_format_function=None,
+    post_format_function=None,
+    clipboard_function=None,
+    **kwargs,
+) -> Dict:
+    return {
+        **dict(
+            datatypes=datatypes,
+            format_function=format_function,
+            to_str_function=to_str_function,
+            invalid_value=invalid_value,
+            nullable=nullable,
+            pre_format_function=pre_format_function,
+            post_format_function=post_format_function,
+            clipboard_function=clipboard_function,
+        ),
+        **kwargs,
+    }
+
+
+def format_data(
+    value="",
+    datatypes=int,
+    nullable=True,
+    pre_format_function=None,
+    format_function=to_int,
+    post_format_function=None,
+    **kwargs,
+) -> Any:
+    if pre_format_function:
+        value = pre_format_function(value)
+    if nullable and is_none_like(value):
+        value = None
+    else:
+        try:
+            value = format_function(value, **kwargs)
+        except Exception:
+            pass
+    if post_format_function and isinstance(value, datatypes):
+        value = post_format_function(value)
+    return value
+
+
+def data_to_str(
+    value="",
+    datatypes=int,
+    nullable=True,
+    invalid_value="NaN",
+    to_str_function=None,
+    **kwargs,
+) -> str:
+    if not isinstance(value, datatypes):
+        return invalid_value
+    if value is None and nullable:
+        return ""
+    return to_str_function(value, **kwargs)
+
+
+def get_data_with_valid_check(value="", datatypes=tuple(), invalid_value="NA"):
+    if isinstance(value, datatypes):
+        return value
+    return invalid_value
+
+
+def get_clipboard_data(value="", clipboard_function=None, **kwargs):
+    if clipboard_function is not None:
+        return clipboard_function(value, **kwargs)
+    if isinstance(value, (str, int, float, bool)):
+        return value
+    return data_to_str(value, **kwargs)
+
+
+class Formatter:
+    def __init__(
+        self,
+        value,
+        datatypes=int,
+        format_function=to_int,
+        to_str_function=to_str,
+        nullable=True,
+        invalid_value="NaN",
+        pre_format_function=None,
+        post_format_function=None,
+        clipboard_function=None,
+        **kwargs,
+    ):
+        if nullable:
+            if isinstance(datatypes, (list, tuple)):
+                datatypes = tuple({type_ for type_ in datatypes} | {type(None)})
+            else:
+                datatypes = (datatypes, type(None))
+        elif isinstance(datatypes, (list, tuple)) and type(None) in datatypes:
+            raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
+        elif datatypes is type(None):
+            raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
+        self.kwargs = kwargs
+        self.valid_datatypes = datatypes
+        self.format_function = format_function
+        self.to_str_function = to_str_function
+        self.nullable = nullable
+        self.invalid_value = invalid_value
+        self.pre_format_function = pre_format_function
+        self.post_format_function = post_format_function
+        self.clipboard_function = clipboard_function
+        try:
+            self.value = self.format_data(value)
+        except Exception:
+            self.value = f"{value}"
+
+    def __str__(self):
+        if not self.valid():
+            return self.invalid_value
+        if self.value is None and self.nullable:
+            return ""
+        return self.to_str_function(self.value, **self.kwargs)
+
+    def valid(self, value=None) -> bool:
+        if value is None:
+            value = self.value
+        if isinstance(value, self.valid_datatypes):
+            return True
+        return False
+
+    def format_data(self, value):
+        if self.pre_format_function:
+            value = self.pre_format_function(value)
+        value = None if (self.nullable and is_none_like(value)) else self.format_function(value, **self.kwargs)
+        if self.post_format_function and self.valid(value):
+            value = self.post_format_function(value)
+        return value
+
+    def get_data_with_valid_check(self):
+        if self.valid():
+            return self.value
+        return self.invalid_value
+
+    def get_clipboard_data(self):
+        if self.clipboard_function is not None:
+            return self.clipboard_function(self.value, **self.kwargs)
+        if isinstance(self.value, (int, float, bool)):
+            return self.value
+        return self.__str__()
+
+    def __eq__(self, __value) -> bool:
+        # in case of custom formatter class
+        # compare the values
+        try:
+            if hasattr(__value, "value"):
+                return self.value == __value.value
+        except Exception:
+            pass
+        # if comparing to a string, format the string and compare
+        if isinstance(__value, str):
+            try:
+                return self.value == self.format_data(__value)
+            except Exception:
+                pass
+        # if comparing to anything else, compare the values
+        return self.value == __value
```

### Comparing `tksheet-6.2.2/tksheet/_tksheet_main_table.py` & `tksheet-6.2.3/tksheet/_tksheet_main_table.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/_tksheet_other_classes.py` & `tksheet-6.2.3/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/_tksheet_row_index.py` & `tksheet-6.2.3/tksheet/_tksheet_row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.2.3/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet/_tksheet_vars.py` & `tksheet-6.2.3/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.2/tksheet.egg-info/PKG-INFO` & `tksheet-6.2.3/tksheet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-Metadata-Version: 2.1
-Name: tksheet
-Version: 6.2.2
-Summary: Tkinter table / sheet widget
-Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.2.tar.gz
-Author: ragardner
-Author-email: github@ragardner.simplelogin.com
-License: MIT
-Keywords: tkinter,table,widget,sheet,grid,tk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
-
-## **Python tkinter table widget**
-
-----
-
-```python
-#To install using pip
-pip install tksheet
-
-#To update using pip
-pip install tksheet --upgrade
-```
-
-## **Help**
-
-----
-
-- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
-- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
-- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
-- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
-- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
-
-### **NOTICE:** 
-With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
-
-## **Features**
-
-----
-
-- Display and modify tabular data
-- Stores its display data as a Python list of lists, sublists being rows
-- Runs smoothly even with millions of rows/columns
-- Edit cells directly
-- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
-- Drag and drop columns and rows
-- Multiple line header and index cells
-- Expand row heights and column widths
-- Change fonts and font size (not for individual cells)
-- Change any colors in the sheet
-- Create an unlimited number of high performance dropdown and check boxes
-- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
-- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
-
-### **light blue theme**
-
-----
-
-![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
-
-### **black theme**
-
-----
-
-![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+Metadata-Version: 2.1
+Name: tksheet
+Version: 6.2.3
+Summary: Tkinter table / sheet widget
+Home-page: https://github.com/ragardner/tksheet
+Author: ragardner
+Author-email: github@ragardner.simplelogin.com
+License: MIT
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.3.tar.gz
+Keywords: tkinter,table,widget,sheet,grid,tk
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
+
+## **Python tkinter table widget**
+
+----
+
+```python
+#To install using pip
+pip install tksheet
+
+#To update using pip
+pip install tksheet --upgrade
+```
+
+## **Help**
+
+----
+
+- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
+- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
+- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
+
+### **NOTICE:** 
+With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
+
+## **Features**
+
+----
+
+- Display and modify tabular data
+- Stores its display data as a Python list of lists, sublists being rows
+- Runs smoothly even with millions of rows/columns
+- Edit cells directly
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
+- Drag and drop columns and rows
+- Multiple line header and index cells
+- Expand row heights and column widths
+- Change fonts and font size (not for individual cells)
+- Change any colors in the sheet
+- Create an unlimited number of high performance dropdown and check boxes
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
+- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
+
+### **light blue theme**
+
+----
+
+![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
+
+### **black theme**
+
+----
+
+![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+
```

