# Comparing `tmp/svcs-23.3.1.dev23-py3-none-any.whl.zip` & `tmp/svcs-23.3.1.dev24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7731 bytes, number of entries: 9
+Zip file size: 7751 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      476 b- defN 20-Feb-02 00:00 svcs/__init__.py
 -rw-r--r--  2.0 unx     6879 b- defN 20-Feb-02 00:00 svcs/_core.py
 -rw-r--r--  2.0 unx      234 b- defN 20-Feb-02 00:00 svcs/exceptions.py
 -rw-r--r--  2.0 unx     2365 b- defN 20-Feb-02 00:00 svcs/flask.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 svcs/py.typed
-?rw-r--r--  2.0 unx     5284 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev23.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev23.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev23.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      672 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev23.dist-info/RECORD
-9 files, 17069 bytes uncompressed, 6585 bytes compressed:  61.4%
+?rw-r--r--  2.0 unx     5334 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev24.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev24.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev24.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      672 b- defN 20-Feb-02 00:00 svcs-23.3.1.dev24.dist-info/RECORD
+9 files, 17119 bytes uncompressed, 6605 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: svcs/flask.py
 Comment: 
 
 Filename: svcs/py.typed
 Comment: 
 
-Filename: svcs-23.3.1.dev23.dist-info/METADATA
+Filename: svcs-23.3.1.dev24.dist-info/METADATA
 Comment: 
 
-Filename: svcs-23.3.1.dev23.dist-info/WHEEL
+Filename: svcs-23.3.1.dev24.dist-info/WHEEL
 Comment: 
 
-Filename: svcs-23.3.1.dev23.dist-info/licenses/LICENSE
+Filename: svcs-23.3.1.dev24.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: svcs-23.3.1.dev23.dist-info/RECORD
+Filename: svcs-23.3.1.dev24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `svcs-23.3.1.dev23.dist-info/METADATA` & `svcs-23.3.1.dev24.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.3.1.dev23
+Version: 23.3.1.dev24
 Summary: A Service Locator for Python
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
@@ -33,15 +33,15 @@
 Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
 
 
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="docs/_static/logo.svg" width="25%" alt="svcs" />
+    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="25%" alt="svcs" />
   </a>
 </p>
 
 
 # *svcs*: A Service Locator for Python
 
 > **Warning**
```

## Comparing `svcs-23.3.1.dev23.dist-info/licenses/LICENSE` & `svcs-23.3.1.dev24.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

