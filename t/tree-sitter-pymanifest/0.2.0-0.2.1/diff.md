# Comparing `tmp/tree_sitter_pymanifest-0.2.0-cp38-abi3-macosx_10_9_universal2.whl.zip` & `tmp/tree_sitter_pymanifest-0.2.1-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 13983 bytes, number of entries: 8
--rw-r--r--  2.0 unx      189 b- defN 22-Sep-14 22:27 tree_sitter_pymanifest/__init__.py
--rw-r--r--  2.0 unx      884 b- defN 22-Sep-14 22:27 tree_sitter_pymanifest/_core.py
--rwxr-xr-x  2.0 unx    99422 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest/pymanifest.so
--rw-rw-r--  2.0 unx      733 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest-0.2.0.dist-info/RECORD
--rw-r--r--  2.0 unx     1058 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      113 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest-0.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1442 b- defN 22-Sep-14 22:30 tree_sitter_pymanifest-0.2.0.dist-info/METADATA
-8 files, 103864 bytes uncompressed, 12683 bytes compressed:  87.8%
+Zip file size: 13603 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      198 b- defN 23-Jul-24 08:26 tree_sitter_pymanifest/__init__.py
+-rw-rw-rw-  2.0 fat      914 b- defN 23-Jul-24 08:26 tree_sitter_pymanifest/_core.py
+-rw-rw-rw-  2.0 fat    22016 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest/pymanifest.dll
+-rw-rw-rw-  2.0 fat      799 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest/pymanifest.exp
+-rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest/pymanifest.lib
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1490 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      921 b- defN 23-Jul-24 08:29 tree_sitter_pymanifest-0.2.1.dist-info/RECORD
+10 files, 29346 bytes uncompressed, 12001 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: tree_sitter_pymanifest/__init__.py
 Comment: 
 
 Filename: tree_sitter_pymanifest/_core.py
 Comment: 
 
-Filename: tree_sitter_pymanifest/pymanifest.so
+Filename: tree_sitter_pymanifest/pymanifest.dll
 Comment: 
 
-Filename: tree_sitter_pymanifest-0.2.0.dist-info/RECORD
+Filename: tree_sitter_pymanifest/pymanifest.exp
 Comment: 
 
-Filename: tree_sitter_pymanifest-0.2.0.dist-info/LICENSE
+Filename: tree_sitter_pymanifest/pymanifest.lib
 Comment: 
 
-Filename: tree_sitter_pymanifest-0.2.0.dist-info/WHEEL
+Filename: tree_sitter_pymanifest-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: tree_sitter_pymanifest-0.2.0.dist-info/top_level.txt
+Filename: tree_sitter_pymanifest-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: tree_sitter_pymanifest-0.2.0.dist-info/METADATA
+Filename: tree_sitter_pymanifest-0.2.1.dist-info/WHEEL
+Comment: 
+
+Filename: tree_sitter_pymanifest-0.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: tree_sitter_pymanifest-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_pymanifest/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-"""PyPA manifest parser"""
-
-from ._core import parse, query, highlights
-
-__author__ = 'ObserverOfTime'
-__version__ = '0.2.0'
-__license__ = 'MIT'
-
-__all__ = ['parse', 'query', 'highlights']
+"""PyPA manifest parser"""
+
+from ._core import parse, query, highlights
+
+__author__ = 'ObserverOfTime'
+__version__ = '0.2.0'
+__license__ = 'MIT'
+
+__all__ = ['parse', 'query', 'highlights']
```

## tree_sitter_pymanifest/_core.py

 * *Ordering differences only*

```diff
@@ -1,30 +1,30 @@
-from pathlib import PurePath
-from pkg_resources import resource_filename
-from sys import platform
-
-from tree_sitter import Language, Parser
-
-_language = Language(
-    PurePath(__file__).with_name('pymanifest') \
-        .with_suffix('.dll' if platform == 'win32' else '.so'),
-    'pymanifest'
-)
-
-_parser = Parser()
-_parser.set_language(_language)
-
-def parse(source):
-    """Parse the given source code"""
-    if isinstance(source, str):
-        source = source.encode()
-    return _parser.parse(source, keep_text=True)
-
-def query(query, node):
-    """Run an arbitrary query on the given source node"""
-    return _language.query(query).captures(node)
-
-def highlights(tree):
-    """Return the highlight groups for the given source tree"""
-    res = resource_filename(__package__, 'queries/highlights.scm')
-    with open(res, 'r') as hl:
-        return query(hl.read(), tree.root_node)
+from pathlib import PurePath
+from pkg_resources import resource_filename
+from sys import platform
+
+from tree_sitter import Language, Parser
+
+_language = Language(
+    PurePath(__file__).with_name('pymanifest') \
+        .with_suffix('.dll' if platform == 'win32' else '.so'),
+    'pymanifest'
+)
+
+_parser = Parser()
+_parser.set_language(_language)
+
+def parse(source):
+    """Parse the given source code"""
+    if isinstance(source, str):
+        source = source.encode()
+    return _parser.parse(source, keep_text=True)
+
+def query(query, node):
+    """Run an arbitrary query on the given source node"""
+    return _language.query(query).captures(node)
+
+def highlights(tree):
+    """Return the highlight groups for the given source tree"""
+    res = resource_filename(__package__, 'queries/highlights.scm')
+    with open(res, 'r') as hl:
+        return query(hl.read(), tree.root_node)
```

## Comparing `tree_sitter_pymanifest-0.2.0.dist-info/LICENSE` & `tree_sitter_pymanifest-0.2.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2022 ObserverOfTime
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2022 ObserverOfTime
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `tree_sitter_pymanifest-0.2.0.dist-info/METADATA` & `tree_sitter_pymanifest-0.2.1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-Metadata-Version: 2.1
-Name: tree-sitter-pymanifest
-Version: 0.2.0
-Summary: A tree-sitter parser for MANIFEST.in files
-Author-email: ObserverOfTime <chronobserver@disroot.org>
-License: MIT
-Project-URL: Homepage, https://github.com/ObserverOfTime/tree-sitter-pymanifest
-Project-URL: Issues, https://github.com/ObserverOfTime/tree-sitter-pymanifest/issues
-Project-URL: Sponsor, https://github.com/sponsors/ObserverOfTime
-Keywords: tree-sitter,parser,lexer
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: tree-sitter (~=0.20)
-
-======================
-tree-sitter-pymanifest
-======================
-
-A tree-sitter parser for PyPA manifest files.
-
-Python package
---------------
-
-Installation
-^^^^^^^^^^^^
-
-.. code-block:: bash
-
-   pip install tree-sitter-pymanifest
-
-
-Usage
-^^^^^
-
-.. code-block:: python
-
-   import tree_sitter_pymanifest as pymanifest
-
-   with open('MANIFEST.in', 'r') as mf:
-      # parse a MANIFEST.in file
-      tree = pymanifest.parse(mf.read())
-      # get the highlight groups
-      hl_groups = pymanifest.highlights(tree)
-      # run an arbitrary query
-      dir_patterns = pymanifest.query("""
-      ((command dir_pattern: (pattern) @dir_pattern))
-      """, tree.root_node)
+Metadata-Version: 2.1
+Name: tree-sitter-pymanifest
+Version: 0.2.1
+Summary: A tree-sitter parser for MANIFEST.in files
+Author-email: ObserverOfTime <chronobserver@disroot.org>
+License: MIT
+Project-URL: Homepage, https://github.com/ObserverOfTime/tree-sitter-pymanifest
+Project-URL: Issues, https://github.com/ObserverOfTime/tree-sitter-pymanifest/issues
+Project-URL: Sponsor, https://github.com/sponsors/ObserverOfTime
+Keywords: tree-sitter,parser,lexer
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: tree-sitter (~=0.20)
+
+======================
+tree-sitter-pymanifest
+======================
+
+A tree-sitter parser for PyPA manifest files.
+
+Python package
+--------------
+
+Installation
+^^^^^^^^^^^^
+
+.. code-block:: bash
+
+   pip install tree-sitter-pymanifest
+
+Usage
+^^^^^
+
+.. code-block:: python
+
+   import tree_sitter_pymanifest as pymanifest
+
+   with open('MANIFEST.in', 'r') as mf:
+      # parse a MANIFEST.in file
+      tree = pymanifest.parse(mf.read())
+      # get the highlight groups
+      hl_groups = pymanifest.highlights(tree)
+      # run an arbitrary query
+      dir_patterns = pymanifest.query("""
+      (command dir_pattern: (pattern) @dir_pattern)
+      """, tree.root_node)
```

