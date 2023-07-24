# Comparing `tmp/dauricum-0.3.tar.gz` & `tmp/dauricum-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauricum-0.3.tar", last modified: Wed Jul 19 15:08:27 2023, max compression
+gzip compressed data, was "dauricum-0.4.tar", last modified: Mon Jul 24 12:33:55 2023, max compression
```

## Comparing `dauricum-0.3.tar` & `dauricum-0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.526213 dauricum-0.3/
--rw-rw-rw-   0        0        0     1669 2023-07-19 15:08:27.526213 dauricum-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2023-07-07 16:58:20.000000 dauricum-0.3/README.md
--rw-rw-rw-   0        0        0      535 2023-07-19 15:07:34.000000 dauricum-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 15:08:27.526213 dauricum-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.497231 dauricum-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.503226 dauricum-0.3/src/dauricum/
--rw-rw-rw-   0        0        0     3314 2023-07-19 15:07:49.000000 dauricum-0.3/src/dauricum/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-07-19 15:03:19.000000 dauricum-0.3/src/dauricum/__main__.py
--rw-rw-rw-   0        0        0     1046 2023-07-07 15:13:01.000000 dauricum-0.3/src/dauricum/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.524212 dauricum-0.3/src/dauricum/transformers/
--rw-rw-rw-   0        0        0     5359 2023-07-07 15:09:19.000000 dauricum-0.3/src/dauricum/transformers/ControlFlowTransformer.py
--rw-rw-rw-   0        0        0     6058 2023-07-07 15:50:07.000000 dauricum-0.3/src/dauricum/transformers/InOutlineTransformer.py
--rw-rw-rw-   0        0        0    18409 2023-07-07 15:31:39.000000 dauricum-0.3/src/dauricum/transformers/MBAExprTransformer.py
--rw-rw-rw-   0        0        0     1849 2023-07-07 13:21:14.000000 dauricum-0.3/src/dauricum/transformers/MemoryTransformer.py
--rw-rw-rw-   0        0        0     2684 2023-07-16 09:22:58.000000 dauricum-0.3/src/dauricum/transformers/OpaqueTransformer.py
--rw-rw-rw-   0        0        0    15070 2023-07-19 14:53:26.000000 dauricum-0.3/src/dauricum/transformers/RenamerTransformer.py
--rw-rw-rw-   0        0        0     5165 2023-07-07 15:09:52.000000 dauricum-0.3/src/dauricum/transformers/TryCatchTransformer.py
--rw-rw-rw-   0        0        0     3728 2023-07-07 15:11:46.000000 dauricum-0.3/src/dauricum/transformers/TryNormalizerTransformer.py
--rw-rw-rw-   0        0        0        0 2023-07-07 13:55:08.000000 dauricum-0.3/src/dauricum/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.509221 dauricum-0.3/src/dauricum.egg-info/
--rw-rw-rw-   0        0        0     1669 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 12:33:55.701792 dauricum-0.4/
+-rw-rw-rw-   0        0        0     1822 2023-07-24 12:33:55.700793 dauricum-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1298 2023-07-24 12:33:35.000000 dauricum-0.4/README.md
+-rw-rw-rw-   0        0        0      535 2023-07-24 11:56:05.000000 dauricum-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:33:55.701792 dauricum-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 12:33:55.674810 dauricum-0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:33:55.681804 dauricum-0.4/src/dauricum/
+-rw-rw-rw-   0        0        0     3541 2023-07-24 12:17:29.000000 dauricum-0.4/src/dauricum/__init__.py
+-rw-rw-rw-   0        0        0     4280 2023-07-24 12:30:46.000000 dauricum-0.4/src/dauricum/__main__.py
+-rw-rw-rw-   0        0        0     1046 2023-07-07 15:13:01.000000 dauricum-0.4/src/dauricum/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:33:55.699797 dauricum-0.4/src/dauricum/transformers/
+-rw-rw-rw-   0        0        0     5359 2023-07-07 15:09:19.000000 dauricum-0.4/src/dauricum/transformers/ControlFlowTransformer.py
+-rw-rw-rw-   0        0        0     6140 2023-07-24 12:26:07.000000 dauricum-0.4/src/dauricum/transformers/InOutlineTransformer.py
+-rw-rw-rw-   0        0        0    18409 2023-07-07 15:31:39.000000 dauricum-0.4/src/dauricum/transformers/MBAExprTransformer.py
+-rw-rw-rw-   0        0        0     1849 2023-07-07 13:21:14.000000 dauricum-0.4/src/dauricum/transformers/MemoryTransformer.py
+-rw-rw-rw-   0        0        0     2684 2023-07-16 09:22:58.000000 dauricum-0.4/src/dauricum/transformers/OpaqueTransformer.py
+-rw-rw-rw-   0        0        0    15076 2023-07-24 12:24:40.000000 dauricum-0.4/src/dauricum/transformers/RenamerTransformer.py
+-rw-rw-rw-   0        0        0     3534 2023-07-24 12:21:04.000000 dauricum-0.4/src/dauricum/transformers/StringTransformer.py
+-rw-rw-rw-   0        0        0     5165 2023-07-07 15:09:52.000000 dauricum-0.4/src/dauricum/transformers/TryCatchTransformer.py
+-rw-rw-rw-   0        0        0     3728 2023-07-07 15:11:46.000000 dauricum-0.4/src/dauricum/transformers/TryNormalizerTransformer.py
+-rw-rw-rw-   0        0        0        0 2023-07-07 13:55:08.000000 dauricum-0.4/src/dauricum/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:33:55.686803 dauricum-0.4/src/dauricum.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-24 12:33:55.000000 dauricum-0.4/src/dauricum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-24 12:33:55.000000 dauricum-0.4/src/dauricum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:33:55.000000 dauricum-0.4/src/dauricum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 12:33:55.000000 dauricum-0.4/src/dauricum.egg-info/top_level.txt
```

### Comparing `dauricum-0.3/PKG-INFO` & `dauricum-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauricum
-Version: 0.3
+Version: 0.4
 Summary: Python 3.10+ obfuscator with many obfuscation methods.
 Author-email: nighty1337 <mg938436@gmail.com>
 Project-URL: Homepage, https://github.com/Maxdsdsdsd/dauricum
 Project-URL: Bug Tracker, https://github.com/Maxdsdsdsd/dauricum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,14 +24,17 @@
 
 ## Features
  * MBA Expressions
  * In Outline
  * Control Flow
  * Try Catch
  * Try Catch Normalizer
+ * Opaque
+ * Renamer (Classes, fields, functions)
+ * String Obscure
 
 ## Examples
 Check out examples folder
 
 ## How to
 ### Installation
 
@@ -51,18 +54,18 @@
 ```
 
 ### Use
 
 Obfuscate .py file
 
 ```bash
-  py -m dauricum -input example1-unobf.py -output a.py --mba-expression
-  --mba-expression-mode true --in-outline
-  --control-flow --try-catch --try-catch-mode true
-  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5
+  py -m dauricum -input example1-unobf.py -output example1-obf-0.4.py --mba-expression
+  --mba-expression-mode true --in-outline --control-flow --try-catch --try-catch-mode true
+  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5 --rename --rename-mode 3
+  --opaque --opaque-iter 5 --string-obscure
 ```
 
 Get help
 
 ```bash
   py -m dauricum --help
 ```
```

### Comparing `dauricum-0.3/README.md` & `dauricum-0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 ## Features
  * MBA Expressions
  * In Outline
  * Control Flow
  * Try Catch
  * Try Catch Normalizer
+ * Opaque
+ * Renamer (Classes, fields, functions)
+ * String Obscure
 
 ## Examples
 Check out examples folder
 
 ## How to
 ### Installation
 
@@ -38,18 +41,18 @@
 ```
 
 ### Use
 
 Obfuscate .py file
 
 ```bash
-  py -m dauricum -input example1-unobf.py -output a.py --mba-expression
-  --mba-expression-mode true --in-outline
-  --control-flow --try-catch --try-catch-mode true
-  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5
+  py -m dauricum -input example1-unobf.py -output example1-obf-0.4.py --mba-expression
+  --mba-expression-mode true --in-outline --control-flow --try-catch --try-catch-mode true
+  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5 --rename --rename-mode 3
+  --opaque --opaque-iter 5 --string-obscure
 ```
 
 Get help
 
 ```bash
   py -m dauricum --help
 ```
```

### Comparing `dauricum-0.3/pyproject.toml` & `dauricum-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dauricum"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="nighty1337", email="mg938436@gmail.com" },
 ]
 description = "Python 3.10+ obfuscator with many obfuscation methods."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dauricum-0.3/src/dauricum/__init__.py` & `dauricum-0.4/src/dauricum/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 dauricum.
 
 Python 3.10+ obfuscator with many obfuscation methods.
 
 """
 
-__version__ = "0.3"
+__version__ = "0.4"
 __author__ = 'nighty1337'
 __credits__ = 'POP_JUMP_FORWARD_IF_FALSE'
 
 import ast
 
 from io import TextIOWrapper
 from dauricum.transformers import TryCatchTransformer
 from dauricum.transformers import TryNormalizerTransformer
 from dauricum.transformers import MemoryTransformer
 from dauricum.transformers import InOutlineTransformer
 from dauricum.transformers import ControlFlowTransformer
 from dauricum.transformers import MBAExprTransformer
 from dauricum.transformers import OpaqueTransformer
 from dauricum.transformers import RenamerTransformer
+from dauricum.transformers import StringTransformer
 from dauricum.logger import Logger
 
 class ObfuscatorSettings():
     def __init__(self):
         self.transformers = []
         self.logger_enabled = True
     def addTransformer(self, transformer):
@@ -85,14 +86,21 @@
     def Renamer(self, mode: int):
         """ 
         
         Renamer Transformer
         
         """
         self.addTransformer(RenamerTransformer.RenamerTransformer(mode))
+    def ObscureString(self):
+        """ 
+        
+        Renamer Transformer
+        
+        """
+        self.addTransformer(StringTransformer.StringTransformer())
 
 class Obfuscator:
     def obfuscate(input_file: TextIOWrapper, out_file: TextIOWrapper, settings: ObfuscatorSettings):
         Logger.init(settings.logger_enabled)
         Logger.logger.name = __class__.__name__
         
         Logger.logger.info(f"Obfuscating \"{input_file.name}\" ")
```

### Comparing `dauricum-0.3/src/dauricum/__main__.py` & `dauricum-0.4/src/dauricum/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,14 +92,19 @@
     )
     parser.add_argument(
         "--rename-mode",
         type=int,
         default=0,
         help="Change Renamer mode (0 - random sequence of 32 characters, 1 - random misleading word, 2 - random sequence of 64 characters, 3 - random word of misleading characters)"
     )
+    parser.add_argument(
+        "--string-obscure",
+        action='store_true',
+        help="Enables String Tranformer"
+    )
     
     args = parser.parse_args()
     return args
 
 def main():
     args = handle_args()
     
@@ -110,14 +115,17 @@
     
     settings = ObfuscatorSettings()
     settings.setLoggerEnabled(args.logging)
     
     if (args.mba_expression):
         settings.MBAExpression(args.mba_expression_mode)
         
+    if (args.string_obscure):
+        settings.ObscureString()
+        
     if (args.rename):
         settings.Renamer(args.rename_mode)
         
     if (args.in_outline):
         settings.InOutline()
     
     if (args.opaque):
```

### Comparing `dauricum-0.3/src/dauricum/logger.py` & `dauricum-0.4/src/dauricum/logger.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/ControlFlowTransformer.py` & `dauricum-0.4/src/dauricum/transformers/ControlFlowTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/InOutlineTransformer.py` & `dauricum-0.4/src/dauricum/transformers/InOutlineTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
     def setTree(self, tree):
         self.tree = tree
         
     class InOutlineTransformer(ast.NodeTransformer):
         def visit_Call(self, node : ast.Call):
             if (isinstance(node.func, ast.Attribute)):
                 return node
+            if (isinstance(node.func, ast.Lambda)):
+                return node
             
             if (not node.func.id in default_names):
                 return node
             
             if (not node.func.id in InOutlineTransformer.call_lambdas):
                 InOutlineTransformer.call_lambdas.update( 
                     {
```

### Comparing `dauricum-0.3/src/dauricum/transformers/MBAExprTransformer.py` & `dauricum-0.4/src/dauricum/transformers/MBAExprTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/MemoryTransformer.py` & `dauricum-0.4/src/dauricum/transformers/MemoryTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/OpaqueTransformer.py` & `dauricum-0.4/src/dauricum/transformers/OpaqueTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/RenamerTransformer.py` & `dauricum-0.4/src/dauricum/transformers/RenamerTransformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,16 +152,16 @@
         Logger.logger.info(f"Transforming {self.__class__.__name__}...")
         
         RenamerController.instantiate_parents(self.tree)
         
         newTree = RenamerTransformer.RenamerTransformer().visit(self.tree)
         ast.fix_missing_locations(newTree)
         
-        newTree = RenamerTransformer.FieldRenamerTransformer().visit(newTree)
-        ast.fix_missing_locations(newTree)
+        # newTree = RenamerTransformer.FieldRenamerTransformer().visit(newTree)
+        # ast.fix_missing_locations(newTree)
         newTree = RenamerTransformer.FunctionRenamerTranformer().visit(newTree)
         ast.fix_missing_locations(newTree)
         newTree = RenamerTransformer.PreClassRenamerTransformer().visit(newTree)
         ast.fix_missing_locations(newTree)
         newTree = RenamerTransformer.ClassRenamerTransformer().visit(newTree)
         ast.fix_missing_locations(newTree)
         
@@ -195,15 +195,15 @@
                 
                 RenamerController.field_mappings.update(
                     {
                         target.id + str(RenamerTransformer.proceeded_fields): [generated_name, parent, node, enumerate(RenamerController.field_mappings)]
                     }
                 )
                 
-                node.targets[node.targets.index(target)].id = generated_name
+                # node.targets[node.targets.index(target)].id = generated_name
                 
                 RenamerTransformer.proceeded_fields += 1
             
                 RenamerTransformer.proceeded += 1
             
             return node
```

### Comparing `dauricum-0.3/src/dauricum/transformers/TryCatchTransformer.py` & `dauricum-0.4/src/dauricum/transformers/TryCatchTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum/transformers/TryNormalizerTransformer.py` & `dauricum-0.4/src/dauricum/transformers/TryNormalizerTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.3/src/dauricum.egg-info/PKG-INFO` & `dauricum-0.4/src/dauricum.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauricum
-Version: 0.3
+Version: 0.4
 Summary: Python 3.10+ obfuscator with many obfuscation methods.
 Author-email: nighty1337 <mg938436@gmail.com>
 Project-URL: Homepage, https://github.com/Maxdsdsdsd/dauricum
 Project-URL: Bug Tracker, https://github.com/Maxdsdsdsd/dauricum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,14 +24,17 @@
 
 ## Features
  * MBA Expressions
  * In Outline
  * Control Flow
  * Try Catch
  * Try Catch Normalizer
+ * Opaque
+ * Renamer (Classes, fields, functions)
+ * String Obscure
 
 ## Examples
 Check out examples folder
 
 ## How to
 ### Installation
 
@@ -51,18 +54,18 @@
 ```
 
 ### Use
 
 Obfuscate .py file
 
 ```bash
-  py -m dauricum -input example1-unobf.py -output a.py --mba-expression
-  --mba-expression-mode true --in-outline
-  --control-flow --try-catch --try-catch-mode true
-  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5
+  py -m dauricum -input example1-unobf.py -output example1-obf-0.4.py --mba-expression
+  --mba-expression-mode true --in-outline --control-flow --try-catch --try-catch-mode true
+  --try-catch-iter 3 --try-normalizer --try-normalizer-iter 5 --rename --rename-mode 3
+  --opaque --opaque-iter 5 --string-obscure
 ```
 
 Get help
 
 ```bash
   py -m dauricum --help
 ```
```

### Comparing `dauricum-0.3/src/dauricum.egg-info/SOURCES.txt` & `dauricum-0.4/src/dauricum.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 src/dauricum.egg-info/top_level.txt
 src/dauricum/transformers/ControlFlowTransformer.py
 src/dauricum/transformers/InOutlineTransformer.py
 src/dauricum/transformers/MBAExprTransformer.py
 src/dauricum/transformers/MemoryTransformer.py
 src/dauricum/transformers/OpaqueTransformer.py
 src/dauricum/transformers/RenamerTransformer.py
+src/dauricum/transformers/StringTransformer.py
 src/dauricum/transformers/TryCatchTransformer.py
 src/dauricum/transformers/TryNormalizerTransformer.py
 src/dauricum/transformers/__init__.py
```

