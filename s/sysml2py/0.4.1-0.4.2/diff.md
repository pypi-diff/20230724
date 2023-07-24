# Comparing `tmp/sysml2py-0.4.1.tar.gz` & `tmp/sysml2py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.4.1.tar", max compression
+gzip compressed data, was "sysml2py-0.4.2.tar", max compression
```

## Comparing `sysml2py-0.4.1.tar` & `sysml2py-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-07-24 03:17:52.536772 sysml2py-0.4.1/LICENSE
--rw-r--r--   0        0        0     3757 2023-07-24 03:17:52.536772 sysml2py-0.4.1/README.md
--rw-r--r--   0        0        0     1576 2023-07-24 03:17:53.308792 sysml2py-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3297 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/__init__.py
--rw-r--r--   0        0        0     8052 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/definition.py
--rw-r--r--   0        0        0     2297 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/formatting.py
--rw-r--r--   0        0        0    22296 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0        0        0    10762 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0        0        0    48820 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0        0        0   105604 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/grammar/classes.py
--rw-r--r--   0        0        0    28524 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/textx/KerML.xtext
--rw-r--r--   0        0        0    14284 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/textx/KerMLExpressions.xtext
--rw-r--r--   0        0        0    60663 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/textx/SysML.xtext
--rw-r--r--   0        0        0     6279 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0        0        0    22976 2023-07-24 03:17:52.536772 sysml2py-0.4.1/src/sysml2py/usage.py
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-24 16:53:35.802486 sysml2py-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-24 16:53:35.806486 sysml2py-0.4.2/README.md
+-rw-r--r--   0        0        0     1576 2023-07-24 16:53:36.630487 sysml2py-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3297 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/__init__.py
+-rw-r--r--   0        0        0     8299 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/definition.py
+-rw-r--r--   0        0        0     2297 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/formatting.py
+-rw-r--r--   0        0        0    22296 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0        0        0    10762 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0        0        0    48820 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0        0        0   105604 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/classes.py
+-rw-r--r--   0        0        0    28524 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/KerML.xtext
+-rw-r--r--   0        0        0    14284 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/KerMLExpressions.xtext
+-rw-r--r--   0        0        0    60663 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/SysML.xtext
+-rw-r--r--   0        0        0     6279 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0        0        0    22976 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/usage.py
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.2/PKG-INFO
```

### Comparing `sysml2py-0.4.1/LICENSE` & `sysml2py-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/README.md` & `sysml2py-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/pyproject.toml` & `sysml2py-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #requires = ["setuptools>=61.0"]
 #build-backend = "setuptools.build_meta"
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "sysml2py"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -47,15 +47,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
 
 [tool.poetry]
 name = "sysml2py"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Christopher Cox <chris.cox@westfall.io>"]
 readme = "README.md"
 packages = [{ include = "sysml2py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sysml2py-0.4.1/src/sysml2py/__init__.py` & `sysml2py-0.4.2/src/sysml2py/__init__.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/definition.py` & `sysml2py-0.4.2/src/sysml2py/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
                 if de["ownedRelatedElement"]["name"] == "Package":
                     p = Package().load_from_grammar(
                         PackageGrammar(de["ownedRelatedElement"])
                     )
                     self.children.append(p)
                     member_grammar.append(p._get_definition(child="PackageBody"))
                 else:
-                    raise NotImplementedError
+                    raise ValueError("Base Model must be encapsulated by a package.")
+            else:
+                raise ValueError("Base Model must be encapsulated by a package.")
 
         self.grammar = RootNamespace(
             {"name": "PackageBodyElement", "ownedRelationship": member_grammar}
         )
 
         return self
 
@@ -92,14 +94,17 @@
 
         return self
 
     def _get_definition(self):
         return self.grammar.get_definition()
 
     def dump(self):
+        if len(self.children) == 0:
+            raise ValueError("Base Model has no elements to output.")
+
         self._ensure_body()
         return classtree(self._get_definition()).dump()
 
     def _set_child(self, child):
         self.children.append(child)
         return self
```

### Comparing `sysml2py-0.4.1/src/sysml2py/formatting.py` & `sysml2py-0.4.2/src/sysml2py/formatting.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.4.2/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.4.2/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.4.2/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/grammar/classes.py` & `sysml2py-0.4.2/src/sysml2py/grammar/classes.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/textx/KerML.xtext` & `sysml2py-0.4.2/src/sysml2py/textx/KerML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/textx/KerMLExpressions.xtext` & `sysml2py-0.4.2/src/sysml2py/textx/KerMLExpressions.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/textx/SysML.xtext` & `sysml2py-0.4.2/src/sysml2py/textx/SysML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.4.2/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/src/sysml2py/usage.py` & `sysml2py-0.4.2/src/sysml2py/usage.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.1/PKG-INFO` & `sysml2py-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Christopher Cox
 Author-email: chris.cox@westfall.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

