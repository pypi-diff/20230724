# Comparing `tmp/impunity-1.0.1.tar.gz` & `tmp/impunity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impunity-1.0.1.tar", max compression
+gzip compressed data, was "impunity-1.0.2.tar", max compression
```

## Comparing `impunity-1.0.1.tar` & `impunity-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2023-03-17 15:25:08.762240 impunity-1.0.1/license.txt
--rw-r--r--   0        0        0     1363 2023-07-21 10:47:02.546507 impunity-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       54 2022-12-15 08:10:37.693666 impunity-1.0.1/src/impunity/__init__.py
--rw-r--r--   0        0        0      520 2023-04-26 09:32:15.372322 impunity-1.0.1/src/impunity/exception.py
--rw-r--r--   0        0        0        0 2023-03-17 15:25:08.762240 impunity-1.0.1/src/impunity/py.typed
--rw-r--r--   0        0        0      859 2023-06-20 08:36:00.376797 impunity-1.0.1/src/impunity/quantityNode.py
--rw-r--r--   0        0        0    38267 2023-07-21 10:57:01.761738 impunity-1.0.1/src/impunity/visitor.py
--rw-r--r--   0        0        0     9530 2023-07-12 08:34:02.847488 impunity-1.0.1/src/impunity/wrapper.py
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 impunity-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-03-03 23:02:21.617620 impunity-1.0.2/license.txt
+-rw-r--r--   0        0        0     1363 2023-07-24 12:50:28.083889 impunity-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-12-14 22:12:52.000000 impunity-1.0.2/src/impunity/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-03 12:48:13.573198 impunity-1.0.2/src/impunity/exception.py
+-rw-r--r--   0        0        0        0 2023-02-08 08:48:46.044417 impunity-1.0.2/src/impunity/py.typed
+-rw-r--r--   0        0        0      859 2023-06-20 12:24:15.987401 impunity-1.0.2/src/impunity/quantityNode.py
+-rw-r--r--   0        0        0    38823 2023-07-24 12:47:46.611310 impunity-1.0.2/src/impunity/visitor.py
+-rw-r--r--   0        0        0     9530 2023-07-20 13:23:10.648860 impunity-1.0.2/src/impunity/wrapper.py
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 impunity-1.0.2/PKG-INFO
```

### Comparing `impunity-1.0.1/license.txt` & `impunity-1.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `impunity-1.0.1/pyproject.toml` & `impunity-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "impunity"
-version = "1.0.1"
+version = "1.0.2"
 description = "Static checking for consistency of physical units"
 authors = [
   "Antoine Chevrot <antoine.chevrot@gmail.com>",
   "Xavier Olive <git@xoolive.org>"
 ]
 license = "MIT"
 include = [
```

### Comparing `impunity-1.0.1/src/impunity/exception.py` & `impunity-1.0.2/src/impunity/exception.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0.1/src/impunity/quantityNode.py` & `impunity-1.0.2/src/impunity/quantityNode.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0.1/src/impunity/visitor.py` & `impunity-1.0.2/src/impunity/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
                         f"In function {self.fun.__module__}/"
                         + f"{self.fun.__name__}: "
                         + "Signature of annotated functions must be "
                         + "of type string or typing.Annotated"
                     )
 
         # Check units in the return node
-        node = self.generic_visit(node)  # type: ignore
+        node = cast(ast.FunctionDef, self.generic_visit(node))
         return node
 
     def get_node_unit(self, node: Optional[ast.expr]) -> QuantityNode:
         """Method to induce the unit of a node through recursive
         calls on children if any.
 
         Args:
@@ -705,18 +705,22 @@
                 else ast.Call(
                     func=node.func,
                     args=new_args,
                     keywords=node.keywords,
                 )
             )
 
-            return QuantityNode(
-                ast.copy_location(new_node, node), return_signature[1]
+            return_unit = (
+                return_signature[1].__metadata__[0]  # type: ignore
+                if is_annotated(return_signature[1])
+                else return_signature[1]
             )
 
+            return QuantityNode(ast.copy_location(new_node, node), return_unit)
+
         elif isinstance(node, ast.Attribute):
             if isinstance(node.value, ast.Name):
                 if node.value.id == "self":
                     return QuantityNode(node, self.class_attr[node.attr])
             return QuantityNode(node, None)
 
         else:
@@ -822,14 +826,15 @@
 
         value = self.get_node_unit(node.value)
 
         if value.node is None:
             expected = cast(annotation_node, node.annotation)
             expected_unit = get_annotation_unit(expected)
             self.vars[node.target.id] = expected_unit  # type: ignore
+            return node
 
         if value.node != node.value:
             new_node = ast.AnnAssign(
                 target=node.target,
                 annotation=node.annotation,
                 value=value.node,
                 simple=node.simple,
@@ -863,15 +868,15 @@
                     self.class_attr[node.target.attr] = value.unit
         else:
             if isinstance(node.target, ast.Name):
                 annotation = get_annotation_unit(
                     cast(annotation_node, node.annotation)
                 )
                 self.vars[node.target.id] = annotation
-        # ast.fix_missing_locations(new_node)
+
         return ast.copy_location(new_node, node)
 
     def visit_BinOp(self, node: ast.BinOp) -> ast.BinOp:
         """Method called by the visitor if the visited node is an
         Binary Operation node.
         Checks the units in the node and returns it eventually modified.
 
@@ -969,15 +974,25 @@
                     if isinstance(elem, ast.Name):
                         if isinstance(received[i], typing.ForwardRef):
                             self.vars[elem.id] = received[i].__forward_arg__
                         else:
                             self.vars[elem.id] = received[i]
 
             elif isinstance(target, ast.Name):
-                self.vars[target.id] = value.unit
+                if target.id in self.vars:
+                    expected = self.vars[target.id]
+                    new_value = self.node_convert(
+                        expected, value.unit, value.node
+                    )
+                    new_node = ast.Assign(
+                        targets=node.targets,
+                        value=new_value,
+                    )
+                else:
+                    self.vars[target.id] = value.unit
             elif isinstance(target, ast.Attribute):
                 if isinstance(target.value, ast.Name):
                     if target.value.id == "self":
                         self.class_attr[target.attr] = value.unit
 
         return ast.copy_location(new_node, node)
```

### Comparing `impunity-1.0.1/src/impunity/wrapper.py` & `impunity-1.0.2/src/impunity/wrapper.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0.1/PKG-INFO` & `impunity-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impunity
-Version: 1.0.1
+Version: 1.0.2
 Summary: Static checking for consistency of physical units
 License: MIT
 Author: Antoine Chevrot
 Author-email: antoine.chevrot@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

