# Comparing `tmp/mdformat_mkdocs-1.0.3.tar.gz` & `tmp/mdformat_mkdocs-1.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-1.0.4rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-1.0.3.tar` & `mdformat_mkdocs-1.0.4rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1819 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.gitignore
--rw-r--r--   0        0        0     1756 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      571 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.pre-commit-test.yaml
--rw-r--r--   0        0        0       33 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.tool-versions
--rw-r--r--   0        0        0      979 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/LICENSE
--rw-r--r--   0        0        0     3265 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/README.md
--rw-r--r--   0        0        0      172 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0     3728 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0      402 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/README.md
--rw-r--r--   0        0        0     1063 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/docs/README.md
--rw-r--r--   0        0        0    78687 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdcs-demo-screenshot.png
--rw-r--r--   0        0        0       42 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdocs.yml
--rw-r--r--   0        0        0        0 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdocs_demo/__init__.py
--rw-r--r--   0        0        0    24503 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/poetry.lock
--rw-r--r--   0        0        0      372 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/pyproject.toml
--rw-r--r--   0        0        0     1630 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      789 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/tox.ini
--rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-06 01:58:46.525588 mdformat_mkdocs-1.0.4rc1/.gitignore
+-rw-r--r--   0        0        0     1756 2023-06-27 11:21:14.928646 mdformat_mkdocs-1.0.4rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      571 2023-07-18 22:26:29.357397 mdformat_mkdocs-1.0.4rc1/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       33 2023-04-06 01:58:46.526052 mdformat_mkdocs-1.0.4rc1/.tool-versions
+-rw-r--r--   0        0        0      979 2023-07-23 23:07:19.274542 mdformat_mkdocs-1.0.4rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-04-06 01:58:46.526311 mdformat_mkdocs-1.0.4rc1/LICENSE
+-rw-r--r--   0        0        0     3265 2023-07-23 23:07:19.381070 mdformat_mkdocs-1.0.4rc1/README.md
+-rw-r--r--   0        0        0      175 2023-07-23 23:14:30.380833 mdformat_mkdocs-1.0.4rc1/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0     3925 2023-07-23 23:03:42.317613 mdformat_mkdocs-1.0.4rc1/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0      402 2023-07-23 23:07:19.385206 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/README.md
+-rw-r--r--   0        0        0     1030 2023-07-23 23:06:49.565898 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/docs/README.md
+-rw-r--r--   0        0        0    78687 2023-06-27 11:17:33.074820 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdcs-demo-screenshot.png
+-rw-r--r--   0        0        0       42 2023-06-27 11:14:04.088218 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdocs.yml
+-rw-r--r--   0        0        0        0 2023-06-27 11:10:00.809267 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdocs_demo/__init__.py
+-rw-r--r--   0        0        0    24503 2023-06-27 11:08:15.516527 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/poetry.lock
+-rw-r--r--   0        0        0      372 2023-06-27 11:12:24.831270 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/pyproject.toml
+-rw-r--r--   0        0        0     1630 2023-06-27 23:43:24.286403 mdformat_mkdocs-1.0.4rc1/pyproject.toml
+-rw-r--r--   0        0        0      789 2023-04-06 02:58:30.440638 mdformat_mkdocs-1.0.4rc1/tox.ini
+-rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.4rc1/PKG-INFO
```

### Comparing `mdformat_mkdocs-1.0.3/.gitignore` & `mdformat_mkdocs-1.0.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/.pre-commit-config.yaml` & `mdformat_mkdocs-1.0.4rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/.pre-commit-test.yaml` & `mdformat_mkdocs-1.0.4rc1/.pre-commit-test.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/CONTRIBUTING.md` & `mdformat_mkdocs-1.0.4rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/LICENSE` & `mdformat_mkdocs-1.0.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/README.md` & `mdformat_mkdocs-1.0.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-1.0.4rc1/mdformat_mkdocs/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,23 +48,27 @@
     indent = " " * _MKDOCS_INDENT_COUNT
 
     rendered = ""
     last_indent = ""
     indent_counter = 0
     indent_lookup: Dict[str, int] = {}
     is_numbered = False
+    is_semantic_indent = False
     for line in text.split(eol):
         match = _RE_INDENT.match(line)
         assert match is not None  # for pylint
         list_match = _RE_LIST_ITEM.match(match["content"])
         new_line = line
         if list_match:
             is_numbered = list_match["bullet"] not in {"-", "*"}
             new_bullet = "1." if is_numbered else "-"
             new_line = f'{new_bullet} {list_match["item"]}'
+            is_semantic_indent = True
+        elif not line:
+            is_semantic_indent = False  # on line break, use non-semantic indents
 
         this_indent = match["indent"]
         if this_indent:
             indent_diff = len(this_indent) - len(last_indent)
             if not indent_diff:
                 ...
             elif indent_diff > 0:
@@ -74,15 +78,15 @@
                 indent_counter = indent_lookup[this_indent]
             else:
                 raise NotImplementedError(f"Error in indentation of: `{line}`")
         else:
             indent_counter = 0
         last_indent = this_indent
         new_indent = indent * indent_counter
-        if _ALIGN_SEMANTIC_BREAKS_IN_LISTS and not list_match:
+        if _ALIGN_SEMANTIC_BREAKS_IN_LISTS and not list_match and is_semantic_indent:
             removed_indents = -1 if is_numbered else -2
             new_indent = new_indent[:removed_indents]
         rendered += f"{new_indent}{new_line.strip()}{eol}"
     return rendered.rstrip()
 
 
 # A mapping from `RenderTreeNode.type` to a `Render` function that can
```

### Comparing `mdformat_mkdocs-1.0.3/mkdocs-demo/docs/README.md` & `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/docs/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,52 +2,46 @@
 
 Minimum example code to test MkDocs behavior
 
 ## Semantic Line Indents
 
 See discussion on: https://github.com/KyleKing/mdformat-mkdocs/issues/4
 
-### With proposed change
+### Default without Semantic Indents
 
 1. Here indent width is
-   three.
+    three (four).
 
     1. Here indent width is
-       three.
+        three (four).
 
 1. Here indent width is
-   five (three). The following indent needs to be four (but it is 3 with semantic change).
-
-   Otherwise this next paragraph doesn't belong in the same list item.
+    five (four). The following indent needs to be four.
 
----
+    Otherwise this next paragraph doesn't belong in the same list item.
 
-### With current behavior
+### With Smart Semantic Indents ON
 
 1. Here indent width is
-    three (four).
+   three.
 
     1. Here indent width is
-        three (four).
+       three.
 
 1. Here indent width is
-    five (four). The following indent needs to be four.
+   five (three). The following indent needs to be four (but it is 3 with semantic change).
 
     Otherwise this next paragraph doesn't belong in the same list item.
 
----
-
-### With proposed change for bullets
+#### For bullets
 
 1. Line
    semantic line 1 (3 spaces deep)
     - Bullet (4 spaces deep)
       semantic line 2 (6 spaces deep)
 
----
-
-### With proposed change for bullets nested in a numbered list
+#### For bullets nested in a numbered list
 
 - Line
   semantic line 1 (2 spaces deep)
     - Bullet (4 spaces deep)
       semantic line 2 (6 spaces deep)
```

### Comparing `mdformat_mkdocs-1.0.3/mkdocs-demo/mkdcs-demo-screenshot.png` & `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdcs-demo-screenshot.png`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/mkdocs-demo/poetry.lock` & `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/poetry.lock`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/pyproject.toml` & `mdformat_mkdocs-1.0.4rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/tox.ini` & `mdformat_mkdocs-1.0.4rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.3/PKG-INFO` & `mdformat_mkdocs-1.0.4rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 1.0.3
+Version: 1.0.4rc1
 Summary: An mdformat plugin for mkdocs.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

