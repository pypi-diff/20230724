# Comparing `tmp/pygetsource-0.0.0.tar.gz` & `tmp/pygetsource-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetsource-0.0.0.tar", last modified: Sun Jul 23 21:37:25 2023, max compression
+gzip compressed data, was "pygetsource-0.1.0.tar", last modified: Sun Jul 23 22:00:58 2023, max compression
```

## Comparing `pygetsource-0.0.0.tar` & `pygetsource-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-07-23 21:37:25.864240 pygetsource-0.0.0/
--rw-r--r--   0 perceval   (501) staff       (20)     1074 2023-07-23 09:08:25.000000 pygetsource-0.0.0/LICENSE
--rw-r--r--   0 perceval   (501) staff       (20)     7652 2023-07-23 21:37:25.864117 pygetsource-0.0.0/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)     5993 2023-07-23 21:29:18.000000 pygetsource-0.0.0/README.md
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-07-23 21:37:25.862664 pygetsource-0.0.0/pygetsource/
--rw-r--r--   0 perceval   (501) staff       (20)       96 2023-07-23 21:37:15.000000 pygetsource-0.0.0/pygetsource/__init__.py
--rw-r--r--   0 perceval   (501) staff       (20)     6263 2023-07-23 21:29:42.000000 pygetsource-0.0.0/pygetsource/ast_utils.py
--rw-r--r--   0 perceval   (501) staff       (20)    48349 2023-07-23 00:28:42.000000 pygetsource-0.0.0/pygetsource/decompiler.new.py
--rw-r--r--   0 perceval   (501) staff       (20)    75980 2023-07-23 21:34:31.000000 pygetsource-0.0.0/pygetsource/decompiler.py
--rw-r--r--   0 perceval   (501) staff       (20)     1998 2023-07-23 21:29:42.000000 pygetsource-0.0.0/pygetsource/factory.py
--rw-r--r--   0 perceval   (501) staff       (20)    66667 2023-07-23 19:52:30.000000 pygetsource-0.0.0/pygetsource/old.py
--rw-r--r--   0 perceval   (501) staff       (20)     4120 2023-07-23 21:29:42.000000 pygetsource-0.0.0/pygetsource/utils.py
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-07-23 21:37:25.863299 pygetsource-0.0.0/pygetsource.egg-info/
--rw-r--r--   0 perceval   (501) staff       (20)     7652 2023-07-23 21:37:25.000000 pygetsource-0.0.0/pygetsource.egg-info/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)      433 2023-07-23 21:37:25.000000 pygetsource-0.0.0/pygetsource.egg-info/SOURCES.txt
--rw-r--r--   0 perceval   (501) staff       (20)        1 2023-07-23 21:37:25.000000 pygetsource-0.0.0/pygetsource.egg-info/dependency_links.txt
--rw-r--r--   0 perceval   (501) staff       (20)      105 2023-07-23 21:37:25.000000 pygetsource-0.0.0/pygetsource.egg-info/requires.txt
--rw-r--r--   0 perceval   (501) staff       (20)       12 2023-07-23 21:37:25.000000 pygetsource-0.0.0/pygetsource.egg-info/top_level.txt
--rw-r--r--   0 perceval   (501) staff       (20)     1876 2023-07-23 21:36:29.000000 pygetsource-0.0.0/pyproject.toml
--rw-r--r--   0 perceval   (501) staff       (20)       38 2023-07-23 21:37:25.864282 pygetsource-0.0.0/setup.cfg
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-07-23 21:37:25.863871 pygetsource-0.0.0/tests/
--rw-r--r--   0 perceval   (501) staff       (20)      494 2023-07-23 21:32:25.000000 pygetsource-0.0.0/tests/test_dev.py
--rw-r--r--   0 perceval   (501) staff       (20)    13105 2023-07-23 21:33:35.000000 pygetsource-0.0.0/tests/test_py37.py
--rw-r--r--   0 perceval   (501) staff       (20)     1055 2023-07-23 21:29:17.000000 pygetsource-0.0.0/tests/test_rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-23 22:00:43.000000 pygetsource-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-23 22:00:58.184706 pygetsource-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-23 22:00:43.000000 pygetsource-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/pygetsource/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75980 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/decompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/pygetsource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:00:58.184706 pygetsource-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_rebuild.py
```

### Comparing `pygetsource-0.0.0/LICENSE` & `pygetsource-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/PKG-INFO` & `pygetsource-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.0.0
+Version: 0.1.0
 Summary: Decompiler written in Python for Python
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,19 @@
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
+<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+
+
 # pygetsource
 
 `pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
```

### Comparing `pygetsource-0.0.0/README.md` & `pygetsource-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
+<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+
+
 # pygetsource
 
 `pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
```

### Comparing `pygetsource-0.0.0/pygetsource/ast_utils.py` & `pygetsource-0.1.0/pygetsource/ast_utils.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/pygetsource/decompiler.new.py` & `pygetsource-0.1.0/pygetsource/decompiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+import ast
 import dis
 import io
 import sys
-from typing import List, Optional, Set, Tuple, Type, Container
 import textwrap
+from types import CodeType
+from typing import List, Optional, Set, Tuple, Type
 
+from astunparse.unparser import Unparser
 from IPython.display import display
 
+from .ast_utils import RemoveLastContinue
 from .utils import (
-    hasjabs,
-    graph_sort,
+    binop_to_ast,
+    compareop_to_ast,
     get_origin,
-    lowest_common_successors, compareop_to_ast, binop_to_ast, inplace_to_ast, unaryop_to_ast,
+    graph_sort,
+    hasjabs,
+    inplace_to_ast,
+    lowest_common_successors,
+    unaryop_to_ast,
 )
-from .ast_utils import *
 
 try:
     import ast as astunparse
 
     assert hasattr(astunparse, "unparse")
     print("Using ast.unparse")
 except AssertionError:
     import astunparse
-from types import CodeType
 
 INDENT = 0
 DEBUG = False
 DRAW_PROG = "dot"
 
 
 class set_debug:
@@ -45,25 +51,88 @@
 
 def debug(*args, **kwargs):
     if DEBUG:
         buffer = io.StringIO()
         print(*args, **kwargs, file=buffer)
         print(textwrap.indent(buffer.getvalue(), "  " * INDENT), end="")
 
+
 def warn(*args):
     # debug but in red
     print("\033[91m", *args, "\033[0m")
 
 
+class Unpacking(ast.AST):
+    _attributes = ()
+    _fields = ("value",)
+
+    def __init__(self, value, counter, starred=False):
+        self.value = value
+        self.counter = counter
+        self.starred = starred
+
+
+class ForTargetPlaceholder(ast.AST):
+    _attributes = ()
+    _fields = ()
+
+
+def unparse_ForTargetPlaceholder(self, node):
+    self.write("[...]")
+
+
+Unparser._ForTargetPlaceholder = unparse_ForTargetPlaceholder
+
+
+class ExceptionMatch(ast.AST):
+    _attributes = ()
+    _fields = ("value",)
+
+    def __init__(self, value):
+        self.value = value
+
+
+class ExceptionPlaceholder(ast.AST):
+    _attributes = ()
+    _fields = ()
+
+
+class Reraise(ast.AST):
+    _attributes = ()
+    _fields = ()
+
+
+class ComprehensionBody(ast.AST):
+    _attributes = ()
+    _fields = ("value", "collection")
+
+    def __init__(self, value, collection):
+        self.collection = collection
+        self.value = value
+
+
+def unparse_ComprehensionBody(self, node):
+    """Produced by LIST_APPEND or SET_ADD and unparsed as collection.append/add(value)"""
+    self.fill()
+    self.write("append/add(")
+    self.dispatch(node.value)
+    self.write(")")
+
+
+Unparser._ComprehensionBody = unparse_ComprehensionBody
+
+
 class Node:
     def __init__(self, code: CodeType, op_idx: int, offset: int, opname: str, arg: int):
         # Two choices when walking the graph, either go to the next node or
         # jump to a different node in case of a (un)conditional jump
         self.next: Optional[Node] = None
+        self.next_is_virtual: bool = False
         self.jumps: Set[Node] = set()
+        self.virtual = None
 
         # Previous nodes
         self.prev: Set[Node] = set()
 
         # The node's code
         self.code = code
         self.opname = opname
@@ -84,137 +153,109 @@
 
     @property
     def container(self):
         if self._container is not self:
             self._container = self._container.container
         return self._container
 
-    def successors(self) -> Set["Node"]:
-        if self.next:
-            return {self.next, *self.jumps}
-        return self.jumps
-
     def add_stmt(self, stmt):
-        debug("Add stmt", self, ":", stmt)
+        if DEBUG:
+            debug("Add stmt", self, ":", stmt)
         try:
-            debug(
-                textwrap.indent(astunparse.unparse(ast.fix_missing_locations(stmt)), "  ")
-            )
-        except:
+            if DEBUG:
+                debug(
+                    textwrap.indent(
+                        astunparse.unparse(ast.fix_missing_locations(stmt)), "  "
+                    )
+                )
+        except Exception:
             warn("Could not unparse", stmt, "in", self)
         self.stmts.append(stmt)
 
-    def extend_stmts(self, stmts):
-        for stmt in stmts:
-            self.add_stmt(stmt)
-
     def add_stack(self, item):
         if self.stack is None:
             self.stack = []
-        debug("Add stack", self, ":", item)
+        if DEBUG:
+            debug("Add stack", self, ":", item)
         self.stack.append(item)
 
     def pop_stack(self):
         return self.stack.pop()
 
-    @property
-    def arg_value(self):
-        opname = self.opname
-        if opname.startswith('LOAD_') or opname.startswith('STORE_'):
-            opname = opname[5:] if opname.startswith('LOAD_') else opname[6:]
-
-            if opname == "FAST":
-                return self.code.co_varnames[self.arg]
-            elif opname in ("NAME", "GLOBAL"):
-                return self.code.co_names[self.arg]
-            elif opname == "DEREF":
-                return (self.code.co_cellvars + self.code.co_freevars)[self.arg]
-            elif opname == "CONST":
-                return repr(self.code.co_consts[self.arg])
-            elif opname in ("ATTR", "METHOD"):
-                return self.code.co_names[self.arg]
-        elif opname.startswith("COMPARE_OP"):
-            return dis.cmp_op[self.arg]
-        else:
-            return self.arg
-
     def contract_backward(self):
         """
         Merge the node with its predecessor
         """
 
         # If the node has a single predecessor, merge it with that node
 
         prev_node = next((n for n in self.prev if n.next is self), None)
         if not self.prev:
             self.loops = frozenset()
         if not (
             prev_node
             and (
-                (len(self.prev) == 1) or # and not prev_node.jumps) or
-                prev_node.opname in ("NOP",)
+                (len(self.prev) == 1)
+                or prev_node.opname in ("NOP",)  # and not prev_node.jumps) or
             )
         ):
-            debug(
-                "Could not contract", prev_node, "!<<<!", self, "| next:", self.next, "jumps:", self.jumps, "| prev:", self.prev,
-            )
+            if DEBUG:
+                debug(
+                    "Could not contract",
+                    prev_node,
+                    "!<<<!",
+                    self,
+                    "| next:",
+                    self.next,
+                    "jumps:",
+                    self.jumps,
+                    "| prev:",
+                    self.prev,
+                )
             return None
 
         prev_node._container = self._container
-        debug(
-            "Contract backward", prev_node, "<<<", self, "| next:", self.next, ", jumps:", self.jumps, "| prev:", self.prev,
-        )
+        if DEBUG:
+            debug(
+                "Contract backward",
+                prev_node,
+                "<<<",
+                self,
+                "|",
+                self.next,
+                self.jumps,
+                "|",
+                self.prev,
+            )
         self.prev.remove(prev_node)
         for pred_pred in prev_node.prev:
             if pred_pred.next is prev_node:
                 pred_pred.next = self
             pred_pred.jumps = {
                 self if jump is prev_node else jump for jump in pred_pred.jumps
             }
             self.prev.add(pred_pred)
 
         self.jumps = {
-            (self if n is prev_node else n)
-            for n in self.jumps | (prev_node.jumps - {self})
+            (self if n is prev_node else n) for n in (self.jumps | prev_node.jumps)
         }
 
         for succ in (self.next, *self.jumps):
             if not succ:
                 continue
             if prev_node in succ.prev:
                 succ.prev.remove(prev_node)
                 succ.prev.add(self)
 
         self.stmts = prev_node.stmts + self.stmts
-        debug("After contraction", self, "| next:", self.next, "jumps:", self.jumps, "| prev:", self.prev)
+        if DEBUG:
+            debug("After contraction", self, "|", self.next, self.jumps, "|", self.prev)
 
         return prev_node
 
-    def remove(self):
-        """
-        Remove the node from the graph
-        """
-        debug("Remove node", self, "|", self.next, self.jumps, "|", self.prev)
-        successors = set((self.next, *self.jumps) if self.next else self.jumps)
-        successors.discard(self)
-        for succ in successors:
-            if not succ:
-                continue
-            succ.prev.remove(self)
-            for pred in self.prev:
-                if pred is not self:
-                    succ.prev.add(pred)
-            print("Now", succ, "predecessors are", succ.prev)
-        for pred in self.prev:
-            pred.jumps |= successors
-            pred.jumps.discard(self)
-            if pred.next is self:
-                pred.next = self.next
-                pred.jumps.discard(self.next)
-
     @classmethod
     def from_code(cls, code: CodeType, prune: bool = False):
         bytes = code.co_code
         offset = 0
         graph = {}
 
         while offset < len(bytes):
@@ -235,16 +276,14 @@
             if sys.version_info >= (3, 10) and opname in hasjabs:
                 arg *= 2
 
             block = cls(code, op_idx, offset, opname=opname, arg=arg)
             for i in range(op_idx, offset, 2):
                 graph[i] = block
 
-        # graph[offset] = Block(code, offset, offset + 2, opname="END", arg=0, graph=graph)
-
         for block in graph.values():
             opname = block.opname
             arg = block.arg
 
             if opname in ("RETURN_VALUE",):
                 pass
             elif opname == "JUMP_FORWARD":
@@ -255,108 +294,170 @@
                 "POP_JUMP_IF_TRUE",
                 "POP_JUMP_IF_FALSE",
                 "JUMP_IF_NOT_EXC_MATCH",
             ):
                 block.next = graph[block.offset]
                 block.jumps.add(graph[arg])
             elif opname in (
-                  "FOR_ITER",
-                  "SETUP_FINALLY",
-                  "SETUP_LOOP",
+                "FOR_ITER",
+                "SETUP_FINALLY",
+                "SETUP_LOOP",
             ):
                 block.next = graph[block.offset]
 
                 if graph[block.offset + arg].opname == "POP_BLOCK":
                     block.jumps.add(graph[block.offset + arg + 2])
                 else:
                     block.jumps.add(graph[block.offset + arg])
             else:
                 if block.offset in graph:
                     block.next = graph[block.offset]
 
+            if (
+                # sys.version_info <= (3, 9)
+                block.offset in graph
+                and not block.next
+                and graph[block.offset] not in block.jumps
+                and not prune
+                and False
+            ):
+                block.next = graph[block.offset]
+                block.next_is_virtual = True
+
             if block.next:
                 block.next.prev.add(block)
             for jump in block.jumps:
                 jump.prev.add(block)
 
+            # block.is_virtual = True
+
         root = graph[0]
         root = rewire_break_loop(root)
 
+        if not prune:
+            prune_virtual_edges(root)
+        # seen = set()
+        # def unset_virtual(x):
+        #     if x in seen:
+        #         return
+        #     x.is_virtual = False
+        #     #for prev in tuple(x.prev):
+        #     #    if prev.next_is_virtual and prev.next is x:
+        #     #        prev.next = None
+        #     #        x.prev.remove(prev)
+        #     #        print("Removing prev from", x, ":", prev)
+        #     seen.add(x)
+        #     if not x.is_virtual:
+        #         for n in (x.next if not x.next_is_virtual else None, *x.jumps):
+        #             if n:
+        #                 unset_virtual(n)
+        # unset_virtual(graph[0])
+
         index = 0
         sorted_nodes = []
         for node in graph_sort(root):
             if (
-                  node.opname == "NOP" or
-                  node.opname == "RERAISE" and node.arg == 0 or
-                  node.opname == "POP_BLOCK" or
-                  node.opname == "SETUP_LOOP"
-
+                node.opname == "NOP"
+                or node.opname == "RERAISE"
+                and node.arg == 0
+                or node.opname == "POP_BLOCK"
+                or node.opname == "SETUP_LOOP"
             ):
                 if node.next:
                     for n in node.prev:
                         if n.next is node:
                             n.next = node.next
-                        n.jumps = {node.next if j is node else j for j in n.jumps} - {n.next}
+                        n.jumps = {node.next if j is node else j for j in n.jumps} - {
+                            n.next
+                        }
                     node.next.prev = (node.next.prev | node.prev) - {node}
             else:
                 node.index = index
                 index += 1
                 sorted_nodes.append(node)
 
         graph_nodes = set(sorted_nodes)
         for node in sorted_nodes:
             node.prev &= graph_nodes
-        #detect_loops(sorted_nodes[0])
+        # detect_loops(sorted_nodes[0])
 
         root = sorted_nodes[0]
 
         if prune:
             root = contract_jumps(root)
 
         return root
 
-
     def __repr__(self):
-        return f"[{self.op_idx}]{self.opname}({self.arg_value})"
+        return f"[{self.op_idx}]({self.opname}, {self.arg})"
+
+    @property
+    def arg_value(self):
+        opname = self.opname
+        if opname.startswith("LOAD_") or opname.startswith("STORE_"):
+            opname = opname[5:] if opname.startswith("LOAD_") else opname[6:]
+
+            if opname == "FAST":
+                return self.code.co_varnames[self.arg]
+            elif opname in ("NAME", "GLOBAL"):
+                return self.code.co_names[self.arg]
+            elif opname == "DEREF":
+                return (self.code.co_cellvars + self.code.co_freevars)[self.arg]
+            elif opname == "CONST":
+                return repr(self.code.co_consts[self.arg])
+            elif opname in ("ATTR", "METHOD"):
+                return self.code.co_names[self.arg]
+        elif opname.startswith("COMPARE_OP"):
+            return dis.cmp_op[self.arg]
+        else:
+            return self.arg
 
     def draw(self, prog=None):
-        from IPython.core.display import HTML
         import networkx as nx
+        from IPython.core.display import HTML
 
         g = nx.DiGraph()
 
         visited = set()
 
         def rec(node: Node, pos):
             if node in visited:
                 return
             visited.add(node)
             try:
                 source = node.to_source().split("\n")
-            except:
+            except Exception:
                 source = ["!ERROR!"]
             max_line = max(len(line) for line in source)
-            label = "\n".join([
-                f"[{node.op_idx}]{'✓' if node.visited else ''}|{len(node.stack) if node.stack else 0}☰|{len(node.prev)}↣",
-                #f"↺({','.join(str(i) for i in sorted(node.loops))})",
-                f"{node.opname}({node.arg_value})",
-                "------------",
-                *[line.ljust(max_line) for line in source],
-            ])
+            label = "\n".join(
+                [
+                    ("~({})".format(node.virtual) if node.virtual else "")
+                    + f"[{node.op_idx}]{'✓' if node.visited else ''}|"
+                    f"{len(node.stack) if node.stack else 0}☰|{len(node.prev)}↣",
+                    # f"↺({','.join(str(i) for i in sorted(node.loops))})",
+                    f"{node.opname}({node.arg_value})",
+                    "------------",
+                    *[line.ljust(max_line) for line in source],
+                ]
+            )
             g.add_node(
                 node,
                 pos=",".join(map(str, pos)) + "!",
                 label=label,
                 fontsize=10,
                 color="red" if node is self else "black",
             )
             # positions[node] = pos
-            if node.next:
+            if node.next and not node.next_is_virtual:
                 g.add_edge(node, node.next, label="next", fontsize=10)
                 rec(node.next, (pos[0], pos[1] + 1))
+            elif node.next:
+                g.add_edge(node, node.next, label="(next)", fontsize=10, style="dashed")
+                rec(node.next, (pos[0], pos[1] + 1))
+
             for jump in node.jumps:
                 g.add_edge(node, jump, label="jump", fontsize=10)
                 rec(jump, (pos[0], pos[1] + 1))
 
             # for p in node.prev:
             #     rec(p, (pos[0], pos[1] - 1))
 
@@ -364,15 +465,17 @@
         rec(first, (0, 0))
         agraph = nx.nx_agraph.to_agraph(g)
         # Update some global attrs like LR rankdir, box shape or monospace font
         agraph.graph_attr.update(rankdir="LR", fontname="Menlo")
         agraph.node_attr.update(shape="box", fontname="Menlo")
         agraph.edge_attr.update(fontname="Menlo")
         svg = agraph.draw(prog=DRAW_PROG if prog is None else prog, format="svg")
-        return HTML(f'<div style="max-height: 100%; max-width: initial">{svg.decode()}</div>')
+        return HTML(
+            f'<div style="max-height: 100%; max-width: initial">{svg.decode()}</div>'
+        )
 
     def to_source(self):
         res = []
         for stmt in self.stmts:
             try:
                 stmt = ast.fix_missing_locations(stmt)
             except AttributeError:
@@ -385,76 +488,517 @@
             return self.stmts
         prev_visited = [n for n in self.prev if n.visited]
         if len(prev_visited) != 1:
             return self.stmts
         prev = next(iter(prev_visited), None)
         return prev.last_stmts()
 
-    def can_process_node(self, stop_nodes: Container["Node"] = ()):
-        if self in stop_nodes:
-            return False
-        prev_visited = [n for n in self.prev if n.visited]
-        if len(prev_visited) > 1:
-            return False
-        return True
-
     # noinspection PyMethodParameters,PyMethodFirstArgAssignment
     def _run(
-          self: "Node",
-          loop_heads: Tuple["Node"] = (),
-          stop_nodes: Container["Node"] = (),
+        node: "Node",
+        stop_nodes: Set["Node"] = frozenset(),
+        loop_heads: Tuple["Node"] = (),
+        while_fusions={},
+        stop_on_jump: bool = False,
     ):
         """
         Convert the graph into an AST
         """
-        if not self.can_process_node(stop_nodes):
-            return
+        root = node
 
-        node = self
+        if node.visited or node in stop_nodes:
+            return None
 
         while True:
-            debug("-------------\nProcessing", node, "|", "next:", node.next, "| jumps:", node.jumps,
-                  "| prev:", node.prev, "| loops:", loop_heads)
+            if node.visited:
+                if DEBUG:
+                    debug("::: Already visited", node)
+                break
+            if DEBUG:
+                debug(
+                    "::: Processing",
+                    node,
+                    "|",
+                    node.next,
+                    node.jumps,
+                    "|",
+                    node.prev,
+                    "Ø",
+                    loop_heads,
+                )
             node.visited = True
             prev_visited = [n for n in node.prev if n.visited]
-            prev_unvisited = [n for n in node.prev if not n.visited]
-            assert len(prev_visited) <= 1, "Too many prev visited"
-
-            # This marks the start of a loop
-            if len(prev_unvisited):
-                loop_heads = (*loop_heads, node)
-
-            # Propagate the stack
+            if len(prev_visited) > 1:
+                if DEBUG:
+                    debug("Too many prev visited", prev_visited, "for", node)
+                raise Exception("Too many prev visited")
             if node.stack is None:
                 if prev_visited and prev_visited[0].stack is not None:
                     node.stack = list(prev_visited[0].stack)
                 else:
                     node.stack = []
 
-            # Process the node depending on its opname
+            prev_unvisited = [n for n in node.prev if not n.visited]
+            if len(prev_unvisited):
+                loop_heads = (*loop_heads, node)
+
             if node.opname == "LOAD_CLOSURE":
                 node.add_stack(None)
             elif node.opname.startswith("LOAD_"):
                 process_binding_(node)
             elif node.opname.startswith("STORE_"):
                 process_store_(node)
             elif node.opname.startswith("DELETE_") or node.opname.startswith("DEL_"):
                 process_binding_(node)
                 node.add_stmt(ast.Delete([node.pop_stack()]))
             elif node.opname == "RETURN_VALUE":
                 node.add_stmt(ast.Return(node.pop_stack()))
+            elif node.opname in ("JUMP_FORWARD", "JUMP_ABSOLUTE"):
+                jump = next(iter(node.jumps))
+
+                # If we don't leave any loop
+                loop_head = explore_until(jump, loop_heads)
+                same_context = (
+                    not loop_heads
+                    or loop_head is loop_heads[-1]
+                    or loop_head is None
+                    and len(jump.prev) == 1
+                )
+                if jump.visited:
+                    if same_context:
+                        node.add_stmt(ast.Continue(_loop_node=jump))
+                    else:
+                        node.add_stmt(ast.Break(_loop_node=jump))
+                else:
+                    if not same_context:
+                        node.add_stmt(ast.Break(_loop_node=jump))
+
+                if node.next and node.next_is_virtual:
+                    next_node = node.next
+                    print("NEXT VIRTUAL NODE", node, "->", next_node, next_node.virtual)
+                    if next_node.virtual:
+                        next_node = next_node._run(
+                            stop_nodes={*stop_nodes, *node.jumps},
+                            loop_heads=loop_heads,
+                            while_fusions=while_fusions,
+                        )
+                        if next_node is None:
+                            next_node = node.next
+                    print("...NEXT VIRTUAL NODE", node, "->", next_node)
+                    node.next = None
+                    next_node.prev.discard(node)
+                    node.stmts.extend(next_node.stmts)
+                    for succ in (next_node.next, *next_node.jumps):
+                        if succ and next_node in succ.prev:
+                            succ.prev.discard(next_node)
+                            succ.prev.add(node)
+                    node.jumps |= {next_node.next, *next_node.jumps} - {None}
+            elif node.opname in (
+                "POP_JUMP_IF_TRUE",
+                "POP_JUMP_IF_FALSE",
+                "JUMP_IF_NOT_EXC_MATCH",
+            ):
+                if node.opname == "JUMP_IF_NOT_EXC_MATCH":
+                    test = ExceptionMatch(node.pop_stack())
+                    node.pop_stack()
+                else:
+                    test = node.pop_stack()
+                node.jump_test = test
+
+                if_node = node.next
+                [else_node] = node.jumps
+
+                old_if_node = if_node
+
+                ################
+                # SPECIAL CASE #
+                ################
+                if DEBUG:
+                    debug(
+                        "IF/ELSE BLOCK",
+                        node,
+                        "LOOP HEADS",
+                        loop_heads,
+                        "IF",
+                        if_node,
+                        "ELSE",
+                        else_node,
+                    )
+
+                real_branch = (
+                    next(
+                        (n for n in loop_heads[-1].prev if n.next is loop_heads[-1]),
+                        None,
+                    )
+                    if loop_heads
+                    else None
+                )
+                if (
+                    real_branch
+                    and real_branch.jump_test
+                    and real_branch.opname
+                    == (
+                        "POP_JUMP_IF_FALSE"
+                        if node.opname == "POP_JUMP_IF_TRUE"
+                        else "POP_JUMP_IF_TRUE"
+                    )
+                    and ast.dump(real_branch.jump_test) == ast.dump(test)
+                ):
+                    real_head = get_origin(real_branch.jump_test)[0].container
+
+                    if DEBUG:
+                        debug("THIS SHOULD BE A CONDITIONAL WHILE LOOP", ast.dump(test))
+                    # node.add_stmt(ast.Continue())
+                    node.next.prev.discard(node)
+                    node.next = None
+                    node.jumps = {real_head}
+                    node.add_stmt(ast.Continue())
+                    else_node.prev.remove(node)
+                    real_head.prev.add(node)
+                    real_branch.is_conditional_while = True
+                    while_fusions[real_head] = else_node
+                    loop_heads = loop_heads[:-1]
+                    if loop_heads and loop_heads[-1] is not real_head:
+                        loop_heads = (*loop_heads, real_head)
+                ################
+                else:
+                    meet_nodes = lowest_common_successors(
+                        if_node,
+                        else_node,
+                        stop_nodes={*stop_nodes, node},
+                    )
+                    if DEBUG:
+                        debug(
+                            "IF/ELSE BLOCK",
+                            node,
+                            "MEET",
+                            meet_nodes,
+                            "(STOP at",
+                            {*stop_nodes, node},
+                            ")",
+                        )
+                    assert len(meet_nodes) <= 1
+
+                    before = (if_node, else_node)
+                    if_loop_head = (
+                        explore_until(if_node, loop_heads) if loop_heads else None
+                    )
+                    else_loop_head = (
+                        explore_until(else_node, loop_heads) if loop_heads else None
+                    )
+
+                    if_node = if_node._run(
+                        stop_nodes={*stop_nodes, *meet_nodes, node},
+                        loop_heads=loop_heads,
+                        while_fusions=while_fusions,
+                    )
+                    else_node = else_node._run(
+                        stop_nodes={*stop_nodes, *meet_nodes, node},
+                        loop_heads=loop_heads,
+                        while_fusions=while_fusions,
+                    )
+                    if DEBUG:
+                        debug("IF/ELSE", node, "MEET", meet_nodes)
+                    if DEBUG:
+                        debug(
+                            "IF/ELSE",
+                            node,
+                            "BEFORE succ",
+                            before,
+                            "-> AFTER succ",
+                            if_node,
+                            else_node,
+                        )
+                    if DEBUG:
+                        display(node.draw())
+
+                    if_item = (
+                        if_node.pop_stack()
+                        if if_node and len(if_node.stack) > len(node.stack)
+                        else None
+                    )
+                    else_item = (
+                        else_node.pop_stack()
+                        if else_node and len(else_node.stack) > len(node.stack)
+                        else None
+                    )
+
+                    test_origin = get_origin(test)[0].container
+                    has_been_unparsed = False
+                    if DEBUG:
+                        debug(
+                            "IS THIS A WHILE X LOOP ?",
+                            node,
+                            "LH",
+                            loop_heads,
+                            "IF NEXT",
+                            (if_node or old_if_node).next,
+                            "IF LOOP HEAD",
+                            if_loop_head,
+                            "TEST",
+                            test_origin,
+                            "ELSE LOOP HEAD",
+                            else_loop_head,
+                        )
+                    was_a_loop = False
+                    if (
+                        loop_heads
+                        and if_loop_head is loop_heads[-1]
+                        and test_origin is if_loop_head
+                        and (
+                            (if_node or old_if_node).next is if_loop_head
+                            or old_if_node.next is if_loop_head
+                        )
+                        and else_loop_head is not loop_heads[-1]
+                    ) or node.is_conditional_while:
+                        if DEBUG:
+                            debug(
+                                "THIS IS A WHILE X LOOP",
+                                node,
+                                "LOOP HEAD",
+                                if_loop_head,
+                            )
+                        # while node.contract_backward():
+                        #     print("NODE IS CONTRACTED", node, "==?", if_node.next)
+                        #     if DEBUG:
+                        #         display(node.draw())
+                        #     pass
+                        body_stmts = if_node.stmts if if_node else []
+                        if isinstance(body_stmts[-1], ast.Continue):
+                            body_stmts = body_stmts[:-1]
+                        body_stmts = body_stmts or [ast.Pass()]
+                        node.add_stmt(
+                            ast.While(
+                                test=(
+                                    test
+                                    if node.opname != "POP_JUMP_IF_TRUE"
+                                    else ast.UnaryOp(
+                                        op=ast.Not(),
+                                        operand=test,
+                                    )
+                                ),
+                                body=body_stmts,
+                                orelse=[],
+                                _loop_head=if_loop_head,
+                            )
+                        )
+                        if (
+                            else_node
+                            and else_node.stmts
+                            and not isinstance(else_node.stmts[-1], ast.Break)
+                        ):
+                            node.stmts.extend(else_node.stmts)
+                        if if_node.next:
+                            if_node.next.prev.discard(if_node)
+                            if_node.next = None
+                        has_been_unparsed = True
+                        was_a_loop = True
+                    if not has_been_unparsed:
+                        if if_item is None or not if_node or if_node.stmts:
+                            body_stmts = (
+                                if_node.stmts
+                                if if_node and if_node.stmts
+                                else [
+                                    ast.Continue()
+                                    if loop_heads and old_if_node is loop_heads[-1]
+                                    else ast.Pass()
+                                ]
+                                if not loop_heads
+                                or if_loop_head in (loop_heads[-1], None)
+                                # else [ast.Break(_loop_node=get_origin(test)[0])]
+                                else [ast.Break(_loop_node=if_loop_head)]
+                            )
+                            orelse_stmts = (
+                                else_node.stmts
+                                if else_node and else_node.stmts
+                                else []
+                                if meet_nodes
+                                or not loop_heads
+                                or else_loop_head is loop_heads[-1]
+                                else [ast.Break(_loop_node=else_loop_head)]
+                            )
+                            has_else = bool(meet_nodes) or else_loop_head is not None
+                            node.add_stmt(
+                                ast.If(
+                                    test=(
+                                        test
+                                        if node.opname != "POP_JUMP_IF_TRUE"
+                                        else ast.UnaryOp(
+                                            op=ast.Not(),
+                                            operand=test,
+                                        )
+                                    ),
+                                    body=body_stmts,
+                                    orelse=orelse_stmts if has_else else [],
+                                )
+                            )
+                            if not has_else:
+                                node.stmts.extend(orelse_stmts)
+                        if if_item:
+                            ternary_expr = ast.IfExp(
+                                test=(
+                                    test
+                                    if node.opname == "POP_JUMP_IF_FALSE"
+                                    else ast.UnaryOp(
+                                        op=ast.Not(),
+                                        operand=test,
+                                    )
+                                ),
+                                body=if_item,
+                                orelse=else_item,
+                            )
+                            # for item in if_node.stack:
+                            #    node.add_stack(item)
+                            node.add_stack(ternary_expr)
+
+                    # noinspection PyTypeChecker
+                    successors: Set[Node] = {
+                        *((if_node.next, *if_node.jumps) if if_node else (node.next,)),
+                        *(
+                            (else_node.next, *else_node.jumps)
+                            if else_node
+                            else node.jumps
+                        ),
+                    } - {
+                        None
+                    }  # type: ignore
+                    discarded_successors = {
+                        n
+                        for n in (if_node, else_node)
+                        + ((test_origin,) if was_a_loop else ())
+                        if n and n.visited
+                    }
+                    if DEBUG:
+                        debug(
+                            "IF/ELSE SUCC BEFORE CONTRACT",
+                            successors,
+                            "-",
+                            discarded_successors,
+                        )
+                    if DEBUG:
+                        debug("IF/ELSE PREV BEFORE CONTRACT", node.prev)
+                    successors = successors - discarded_successors
+
+                    jump_nodes = successors
+                    for succ in successors:
+                        if DEBUG:
+                            debug(
+                                "IF/ELSE",
+                                node,
+                                ": REBINDING SUCCESSOR",
+                                succ,
+                                "=>",
+                                succ.prev,
+                                "->",
+                                succ.prev - {if_node, else_node} | {node},
+                            )
+                        succ.prev = (succ.prev - discarded_successors) | {node}
+                    for n in discarded_successors:
+                        for p in n.prev:
+                            if p.next in discarded_successors:
+                                p.next = node
+                            p.jumps = {
+                                node if j in discarded_successors else j
+                                for j in p.jumps
+                            }
+                        n.prev = n.prev - discarded_successors
+                    node.next = None
+                    node.jumps = jump_nodes
+                    if DEBUG:
+                        debug("IF/ELSE", node, node.stack)
+                    if DEBUG:
+                        debug("IF/ELSE SUCC AFTER CONTRACT", successors)
+                    if DEBUG:
+                        debug(
+                            "IF/ELSE PREV AFTER CONTRACT",
+                            node.prev,
+                            "prevs successor:",
+                            [(n.next, *n.jumps) for n in node.prev],
+                        )
+
+                    if DEBUG:
+                        display(node.draw())
+
             elif node.opname == "SETUP_FINALLY":
-                raise NotImplementedError()
+                process_try_(node, loop_heads, stop_nodes, while_fusions)
             elif node.opname == "RERAISE":
+                # ("REMOVING RERAISE", node, "STOP NODES", stop_nodes)
+                # for n in node.prev:
+                #    if n.next is node:
+                #        n.next = node.next
+                #    n.jumps = {node.next if j is node else j for j in n.jumps} - {n.next}
+                # node.next.prev = (node.next.prev | node.prev) - {node}
                 node.add_stmt(Reraise())
             elif node.opname == "POP_BLOCK":
                 pass
             elif node.opname == "GET_ITER":
                 # During eval, pop and applies iter() to TOS
                 pass
+            elif node.opname == "FOR_ITER":
+                old_body_node = body_node = node.next
+                (jump_node,) = node.jumps
+
+                iter_item = node.pop_stack()
+                iter_item._dumped = True
+
+                placeholder = ForTargetPlaceholder()
+                placeholder._origin_offset = node.op_idx
+                placeholder._origin_node = node
+
+                body_node.stack = [*node.stack, iter_item, placeholder]
+                body_node = body_node._run(
+                    stop_nodes={*stop_nodes, node, jump_node},
+                    loop_heads=loop_heads,
+                    while_fusions=while_fusions,
+                )
+                body_loop_head = explore_until(
+                    body_node, (node, jump_node, *stop_nodes)
+                )
+                if DEBUG:
+                    debug("FOR LOOP HEAD", body_loop_head)
+                if DEBUG:
+                    debug("BODY", [ast.dump(x) for x in body_node.stmts])
+                target = body_node.stmts.pop(0).targets[0]
+
+                body_stmts = (body_node.stmts if body_node else []) + (
+                    [ast.Break()] if body_loop_head is not node else []
+                )
+                node.add_stmt(
+                    ast.For(
+                        target=target,
+                        iter=iter_item,
+                        body=body_stmts,
+                        orelse=[],  # TODO
+                        _loop_head=loop_heads[-1] if loop_heads else None,
+                    )
+                )
+                successors = {body_node.next, *body_node.jumps, *node.jumps} - {None}
+                discarded_successors = {
+                    n for n in (body_node, old_body_node, node) if n and n.visited
+                }
+                if DEBUG:
+                    debug("FOR SUCC", successors, "-", discarded_successors)
+                if DEBUG:
+                    debug("FOR PREV", node.prev)
+                successors = successors - discarded_successors
+                jump_nodes = successors
+                for succ in successors:
+                    succ.prev = (succ.prev - discarded_successors) | {node}
+                for n in discarded_successors:
+                    for p in n.prev:
+                        if p.next in discarded_successors:
+                            p.next = node
+                        p.jumps = {
+                            node if j in discarded_successors else j for j in p.jumps
+                        }
+                node.next.prev.discard(node)
+                node.next = None
+                node.jumps = jump_nodes
+                node.prev -= discarded_successors
+                loop_heads = loop_heads[:-1]
             elif node.opname == "COMPARE_OP":
                 if compareop_to_ast[node.arg] != "exception match":
                     right = node.pop_stack()
                     left = node.pop_stack()
                 else:
                     left = node.pop_stack()
                     # right = stack.pop()[1]
@@ -494,20 +1038,24 @@
                 )
             elif node.opname == "BINARY_SUBSCR":
                 slice = node.pop_stack()
                 value = node.pop_stack()
                 node.add_stack(ast.Subscript(value, slice))
             elif node.opname in unaryop_to_ast:
                 value = node.pop_stack()
-                node.add_stack(ast.UnaryOp(op=unaryop_to_ast[node.opname], operand=value))
+                node.add_stack(
+                    ast.UnaryOp(op=unaryop_to_ast[node.opname], operand=value)
+                )
             elif node.opname in inplace_to_ast:
                 right = node.pop_stack()
                 left = node.pop_stack()
                 node.add_stack(
-                    ast.AugAssign(target=left, op=inplace_to_ast[node.opname], value=right),
+                    ast.AugAssign(
+                        target=left, op=inplace_to_ast[node.opname], value=right
+                    ),
                 )
             elif node.opname == "BUILD_SLICE":
                 values = [node.pop_stack() for _ in range(node.arg)][::-1]
                 if node.arg == 2:
                     values = values + [None]
                 node.add_stack(ast.Slice(*values))
             elif node.opname == "BUILD_LIST":
@@ -547,54 +1095,64 @@
 
                 for i in reversed(range(before + after + 1)):
                     node.add_stack(Unpacking(value, counter=i, starred=i == before))
             elif node.opname in ("LIST_EXTEND", "SET_UPDATE"):
                 items = node.pop_stack()
                 if isinstance(items, ast.Constant):
                     items = [ast.Constant(x) for x in items.value]
-                elif hasattr(items, 'elts'):
+                elif hasattr(items, "elts"):
                     items = items.elts
                 else:
                     items = [ast.Starred(items)]
                 obj = node.stack[-node.arg]
                 obj = type(obj)(elts=[*obj.elts, *items])
                 node.stack[-node.arg] = obj
             elif node.opname in ("DICT_UPDATE", "DICT_MERGE"):
                 items = node.pop_stack()
                 if isinstance(items, ast.Constant):
-                    items = [(ast.Name(n), ast.Constant(v)) for n, v in items.value.items()]
-                #elif hasattr(items, 'keys'):
+                    items = [
+                        (ast.Name(n), ast.Constant(v)) for n, v in items.value.items()
+                    ]
+                # elif hasattr(items, 'keys'):
                 #    items = [(k, v) for k, v in zip(items.keys, items.values)]
                 else:
                     items = [(None, items)]
                 obj = node.stack[-node.arg]
                 assert isinstance(obj, ast.Dict)
-                obj = ast.Dict([*obj.keys, *(k for k, _ in items)],
-                               [*obj.values, *(v for _, v in items)])
+                obj = ast.Dict(
+                    [*obj.keys, *(k for k, _ in items)],
+                    [*obj.values, *(v for _, v in items)],
+                )
                 node.stack[-node.arg] = obj
             # TODO: check in for/while loop ?
             elif node.opname in ("LIST_APPEND", "SET_ADD"):
                 value = node.pop_stack()
                 collection = node.stack[-node.arg]
                 # if we can loop to the collection beginning
-                if loop_heads and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]:
+                if (
+                    loop_heads
+                    and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]
+                ):
                     node.add_stmt(ComprehensionBody(value, collection))
                 else:
-                    assert hasattr(collection, 'elts')
+                    assert hasattr(collection, "elts")
                     collection = type(collection)(elts=[*collection.elts, value])
                     node.stack[-node.arg] = collection
             elif node.opname == "MAP_ADD":
                 value = node.pop_stack()
                 key = node.pop_stack()
                 collection = node.stack[-node.arg]
                 # if we can loop to the collection beginning
-                if loop_heads and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]:
+                if (
+                    loop_heads
+                    and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]
+                ):
                     node.add_stmt(ComprehensionBody((key, value), collection))
                 else:
-                    assert hasattr(collection, 'elts')
+                    assert hasattr(collection, "elts")
                     collection = type(collection)(
                         keys=[*collection.keys, key],
                         values=[*collection.values, value],
                     )
                     node.stack[-node.arg] = collection
             elif node.opname == "YIELD_VALUE":
                 node.add_stmt(ast.Expr(ast.Yield(node.pop_stack())))
@@ -607,39 +1165,112 @@
                 assert isinstance(func_code, ast.Constant)
                 code = func_code.value
                 function_node = Node.from_code(code)
                 if DEBUG:
                     display(function_node.draw())
                 sub_function_body = function_node.run().stmts
 
-                node.add_stack(ast.FunctionDef(
-                    name=code.co_name,
-                    args=ast.arguments(
-                        args=[
-                            ast.arg(arg=arg, annotation=None)
-                            for arg in code.co_varnames[: code.co_argcount]
-                        ],
-                        vararg=None,
-                        kwonlyargs=[],
-                        kw_defaults=[],
-                        kwarg=None,
-                        defaults=[],
-                        posonlyargs=[],
-                    ),
-                    body=sub_function_body,
-                    decorator_list=[],
-                    returns=None,
-                ))
+                node.add_stack(
+                    ast.FunctionDef(
+                        name=code.co_name,
+                        args=ast.arguments(
+                            args=[
+                                ast.arg(arg=arg, annotation=None)
+                                for arg in code.co_varnames[: code.co_argcount]
+                            ],
+                            vararg=None,
+                            kwonlyargs=[],
+                            kw_defaults=[],
+                            kwarg=None,
+                            defaults=[],
+                            posonlyargs=[],
+                        ),
+                        body=sub_function_body,
+                        decorator_list=[],
+                        returns=None,
+                    )
+                )
             elif node.opname in ("CALL_FUNCTION", "CALL_METHOD"):
                 args = [node.pop_stack() for _ in range(node.arg)][::-1]
                 func = node.pop_stack()
                 if isinstance(func, ast.FunctionDef):
+
+                    class RewriteComprehensionArgs(ast.NodeTransformer):
+                        def visit_Name(self, node):
+                            if node.id.startswith("."):
+                                var_idx = int(node.id[1:])
+                                return args[var_idx]
+                            return node
+
+                        def visit_For(self, node: ast.For):
+                            nonlocal cls
+                            assert (
+                                len(node.body) == 1
+                                or len(node.body) == 2
+                                and isinstance(node.body[1], ast.Continue)
+                            )
+                            target = self.visit(node.target)
+                            elt = self.visit(node.body[0])
+                            iter = self.visit(node.iter)
+                            condition = None
+                            if isinstance(elt, ast.If):
+                                condition = elt.test
+                                assert (
+                                    len(elt.body) == 1
+                                    or len(elt.body) == 2
+                                    and isinstance(elt.body[1], ast.Continue)
+                                )
+                                elt = elt.body[0]
+                            generators = [
+                                ast.comprehension(
+                                    target=target,
+                                    iter=iter,
+                                    ifs=[condition]
+                                    if condition is not None
+                                    else [],  # TODO
+                                    is_async=False,  # TODO
+                                )
+                            ]
+                            if cls and isinstance(elt, cls):
+                                generators = generators + elt.generators
+                                elt = elt.elt
+                            elif isinstance(elt, ComprehensionBody):
+                                cls = {
+                                    ast.List: ast.ListComp,
+                                    ast.Set: ast.SetComp,
+                                    ast.Dict: ast.DictComp,
+                                }[type(elt.collection)]
+                                elt = elt.value
+                            elif isinstance(elt, ast.Expr) and isinstance(
+                                elt.value, ast.Yield
+                            ):
+                                cls = ast.GeneratorExp
+                                elt = elt.value.value
+                            else:
+                                raise Exception(
+                                    "Unexpected " + ast.dump(elt) + ", cls:" + str(cls)
+                                )
+
+                            if issubclass(cls, ast.DictComp):
+                                return ast.DictComp(
+                                    key=elt[0],
+                                    value=elt[1],
+                                    generators=generators,
+                                    ifs=[],
+                                )
+                            else:
+                                return cls(
+                                    elt=elt,
+                                    generators=generators,
+                                    ifs=[],
+                                )
+
                     assert len(func.body) == 2
                     cls: Optional[Type[ast.AST]] = None
-                    tree = RewriteComprehensionArgs(args, cls).visit(func)
+                    tree = RewriteComprehensionArgs().visit(func)
 
                     if len(func.body) == 1 or isinstance(func.body[1], ast.Return):
                         tree = func.body[0]
                     node.add_stack(tree)
                 else:
                     node.add_stack(
                         ast.Call(
@@ -704,15 +1335,15 @@
                 s = node.stack
                 s[-1], s[-2], s[-3] = s[-2], s[-3], s[-1]
             elif node.opname == "ROT_FOUR":
                 s = node.stack
                 s[-1], s[-2], s[-3], s[-4] = s[-2], s[-3], s[-4], s[-1]
             elif node.opname == "POP_TOP":
                 item = node.pop_stack()
-                if item and not getattr(item, '_dumped', False):
+                if item and not getattr(item, "_dumped", False):
                     node.add_stmt(ast.Expr(item))
             elif node.opname == "POP_EXCEPT":
                 node.pop_stack()
             elif node.opname == "FORMAT_VALUE":
                 fmt_spec = None
                 conversion = -1
                 if node.arg & 0x03 == 0x00:
@@ -752,178 +1383,57 @@
                 # of generator or coroutine. The legal kinds are 0 for generator, 1 f
                 # or coroutine, and 2 for async generator."
                 # However, there are no item in the stack (from the bytecode
                 # perspective) at the start of a generator comprehension function
                 # if node.index > 0:
                 #    node.pop_stack()
                 pass
-
-            elif node.opname in ("POP_JUMP_IF_TRUE", "POP_JUMP_IF_FALSE", "JUMP_IF_NOT_EXC_MATCH"):
-                test = node.pop_stack()
-                # node.jump_test = test
-
-                body_node = node.next
-                else_node: Node = next(iter(node.jumps))
-
-                meet_nodes = lowest_common_successors(
-                    body_node,
-                    else_node,
-                    stop_nodes={*stop_nodes, node},
-                )
-                assert len(meet_nodes) <= 1
-
-                # if loop_heads:
-                #     if_loop_head = explore_until(if_node, loop_heads)
-                #     else_loop_head = explore_until(else_node, loop_heads)
-                # else:
-                #     if_loop_head = else_loop_head = None
-
-                body_node = body_node._run(
-                    loop_heads=loop_heads,
-                    stop_nodes={*stop_nodes, *meet_nodes},
-                )
-                else_node = else_node._run(
-                    loop_heads=loop_heads,
-                    stop_nodes={*stop_nodes, *meet_nodes},
-                )
-
-                if DEBUG:
-                    display(node.draw())
-
-                # In case where in an inline condition, the branches stacks should
-                # contain more elements than the test stack
-                body_item = (
-                    body_node.pop_stack()
-                    if body_node and len(body_node.stack) > len(node.stack)
-                    else None
+            elif node.opname == "SETUP_LOOP":
+                # Python 3.7
+                raise Exception(
+                    "SETUP_LOOP code should have been removed during the "
+                    "graph initialization"
                 )
-                else_item = (
-                    else_node.pop_stack()
-                    if else_node and len(else_node.stack) > len(node.stack)
-                    else None
+            elif node.opname == "BREAK_LOOP":
+                # Python 3.7
+                raise Exception(
+                    "BREAK_LOOP code should have been removed during the "
+                    "graph initialization"
                 )
-                test_origin = get_origin(test)[0].container
-
-                if body_item:
-                    node.add_stack(ast.IfExp(
-                        test=(
-                            test
-                            if node.opname == "POP_JUMP_IF_FALSE"
-                            else ast.UnaryOp(
-                                op=ast.Not(),
-                                operand=test,
-                            )
-                        ),
-                        body=body_item,
-                        orelse=else_item,
-                    ))
-                else:
-                    # Multiple cases here:
-                    if body_node:
-                        # - if the body_node has been processed, then we can use its stmts
-                        body_stmts = body_node.stmts or [ast.Pass()]
-                    elif meet_nodes:
-                        print("MEET NODES", "=>", "pass")
-                        body_stmts = [ast.Pass()]
-                    else:
-                        next_node = node.next
-                        if loop_heads and next_node is loop_heads[-1]:
-                            # - if the test brings us back to the top of the last loop
-                            body_stmts = [ast.Continue()]
-                        elif loop_heads and next_node in loop_heads[:-1]:
-                            # - if the test brings us back to the top of a higher loop
-                            body_stmts = [ast.Break()]
-                        elif loop_heads:
-                            # - if we're in a loop but the test brings to a loop-free zone
-                            # TODO: should we check if a break brings us to the else node
-                            #       in case of while [...] loops ?
-                            body_stmts = [ast.Break()]
-                        else: # if not loop_heads
-                            # - if we're not in a loop
-                            body_stmts = [ast.Pass()]
-
-
-                    # Multiple cases here:
-                    if else_node:
-                        # - if the else_node has been processed, we can use its stmts
-                        else_stmts = else_node.stmts or [ast.Pass()]
-                    # - if this was a simple if without break or continue or return
-                    #   and else is empty, and does not have break/continue/... either
-                    #   (otherwise the two nodes would not meet), don't add an else
-                    #   statement
-                    elif meet_nodes:
-                        else_stmts = []
-                    else:
-                        # - if the body does not meet the else node due to a break,
-                        #   continue, return, or something else, then we need to
-                        #   inspect the various possible cases
-                        jump_node = next(iter(node.jumps))
-                        if loop_heads and jump_node is loop_heads[-1]:
-                            # - if fail brings us back to the top of the last loop
-                            else_stmts = [ast.Continue()]
-                        elif loop_heads and jump_node in loop_heads[:-1]:
-                            # - if fail brings us back to the top of a higher loop
-                            else_stmts = [ast.Break()]
-                        elif loop_heads:
-                            # - if we're in a loop but fail brings to a loop-free zone
-                            # TODO: should we check if a break brings us to the else
-                            #       node in case of while [...] loops ?
-                            else_stmts = [ast.Break()]
-                        else: # if not loop_heads
-                            # - if we're not in a loop
-                            else_stmts = []
-
-
-                    # To have a full if/else structure, we require that
-                    # the two branches meet again at some point
-                    has_else = bool(meet_nodes)  #  or else_loop_head is not None
-                    node.add_stmt(
-                        ast.If(
-                            test=(
-                                test
-                                if node.opname != "POP_JUMP_IF_TRUE"
-                                else ast.UnaryOp(
-                                    op=ast.Not(),
-                                    operand=test,
-                                )
-                            ),
-                            body=body_stmts,
-                            orelse=else_stmts if has_else else []
-                        )
-                    )
-                    if not has_else:
-                        node.stmts.extend(else_stmts)
-
-                if body_node:
-                    body_node.remove()
-                if else_node:
-                    else_node.remove()
-
-                if DEBUG:
-                    display(node.draw())
             else:
                 raise NotImplementedError(node.opname)
 
             # Handle while loops by detecting cycles of length 1
             prev_visited = [n for n in node.prev if n.visited]
-            debug("STACKS", "node", node, len(node.stack), node.stack, "prev", prev_visited, len(prev_visited[-1].stack) if prev_visited else 0, prev_visited[-1].stack if prev_visited else None)
-            debug("LOOP HEADS", "node", node, "PREV", node.prev, "=>", loop_heads)
+            if DEBUG:
+                debug(
+                    "STACKS",
+                    "node",
+                    node,
+                    len(node.stack),
+                    node.stack,
+                    "prev",
+                    prev_visited,
+                    len(prev_visited[-1].stack) if prev_visited else 0,
+                    prev_visited[-1].stack if prev_visited else None,
+                )
+            if DEBUG:
+                debug("LOOP HEADS", "node", node, "PREV", node.prev, "=>", loop_heads)
             while not prev_visited or len(node.stack) <= len(prev_visited[-1].stack):
-                if self.container is not node:
+                if root.container is not node:
                     prev = node.contract_backward()
                 else:
                     prev = None
                 if not prev and not node.prev == {node}:
                     break
                 if loop_heads and loop_heads[-1] is prev:
                     loop_heads = (*loop_heads[:-1], node)
                 if node in node.jumps:
                     node.jumps.remove(node)
                     node.prev.remove(node)
-
                     body = node.stmts
                     node.stmts = []
                     node.add_stmt(
                         ast.While(
                             test=ast.Constant(value=True, kind=None),
                             body=body,
                             orelse=[],
@@ -936,99 +1446,144 @@
 
                     prev_unvisited = [n for n in node.prev if not n.visited]
                     if len(prev_unvisited):
                         loop_heads = (*loop_heads, node)
                 prev_visited = [n for n in node.prev if n.visited]
                 if DEBUG:
                     display(node.draw())
-                debug("STACKS", "node", node, len(node.stack), "prev", prev_visited, len(prev_visited[-1].stack) if prev_visited else 0)
+                if DEBUG:
+                    debug(
+                        "STACKS",
+                        "node",
+                        node,
+                        len(node.stack),
+                        "prev",
+                        prev_visited,
+                        len(prev_visited[-1].stack) if prev_visited else 0,
+                    )
 
             if DEBUG:
                 display(node.draw())
 
-            debug("::: done", node, "|", node.next, node.jumps, "|", node.prev)
+            if DEBUG:
+                debug("::: done", node, "|", node.next, node.jumps, "|", node.prev)
 
-            if not node.next:
+            if not node.next and not stop_on_jump:
                 if loop_heads:
                     jump_to_head = {
                         n: explore_until(n, (*loop_heads, *stop_nodes))
                         for n in node.jumps
                     }
-                    debug("CANDIDATE JUMPS", node, "=>", jump_to_head, "LOOP HEADS", loop_heads)
+                    if DEBUG:
+                        debug(
+                            "CANDIDATE JUMPS",
+                            node,
+                            "=>",
+                            jump_to_head,
+                            "LOOP HEADS",
+                            loop_heads,
+                        )
                     same_level_jumps = [
-                        jump for jump, head in jump_to_head.items()
-                        if head is loop_heads[-1] or (head is None and len(jump.prev) == 1)
+                        jump
+                        for jump, head in jump_to_head.items()
+                        if head is loop_heads[-1]
+                        or (head is None and len(jump.prev) == 1)
                     ]
-                    debug("SAME LEVEL JUMPS", node, "=>", same_level_jumps, "LOOP HEADS", loop_heads)
+                    if DEBUG:
+                        debug(
+                            "SAME LEVEL JUMPS",
+                            node,
+                            "=>",
+                            same_level_jumps,
+                            "LOOP HEADS",
+                            loop_heads,
+                        )
                 else:
                     same_level_jumps = list(node.jumps)
 
                 if len(same_level_jumps) > 1:
                     warn("MULTIPLE CHOICE FOR JUMP", same_level_jumps)
                 if same_level_jumps:
-                    node.next = sorted(same_level_jumps,
-                                       key=lambda j: (0 if j.index > node.index else 1, j.index))[0]
+                    node.next = sorted(
+                        same_level_jumps,
+                        key=lambda j: (0 if j.index > node.index else 1, j.index),
+                    )[0]
                     node.jumps.remove(node.next)
                 # ARE WE SURE OF THIS ?
                 # If there is only one outgoing edge, jumping on a different level
                 # set it as next but don't continue exploring
                 elif len(node.jumps) == 1:
                     node.next = next(iter(node.jumps))
                     node.jumps.remove(node.next)
-                    #if node.is_virtual:
+                    # if node.is_virtual:
                     #    node.next.prev.discard(node)
-                    print("Stop after", node, "because not same level")
+                    if DEBUG:
+                        print("Stop after", node, "because not same level")
                     break
 
             # if node.is_virtual:
             #     for succ in node.jumps:
             #         succ.prev.discard(node)
-            if node.next and not node.next.visited and not node.next in stop_nodes:
+            if node.next and not node.next.visited and node.next not in stop_nodes:
                 node: Node = node.next
             else:
                 # if node.is_virtual and node.next:
                 #     node.next.prev.discard(node)
-                print("Stop after", node, ": next=", node.next, "is visited", node.next.visited if node.next else "-", "| stop nodes: ", stop_nodes)
-
-                if loop_heads and node.next is loop_heads[-1]:
-                    # we're brings us back to the top of the last loop
-                    node.add_stmt(ast.Continue())
-                elif node.next in loop_heads[:-1]:
-                    # we're brings us back to the top of a higher loop
-                    print("Next node is a loop head, break", node)
-                    node.add_stmt(ast.Break())
-                elif node.next in stop_nodes:
-                    # we're brings us back to a loop-free zone
-                    print("Next node is a stop node, break", node)
-                    node.add_stmt(ast.Break())
+                if DEBUG:
+                    print(
+                        "Stop after",
+                        node,
+                        ": next=",
+                        node.next,
+                        "is visited",
+                        node.next.visited if node.next else "-",
+                        "| stop nodes: ",
+                        stop_nodes,
+                    )
                 break
 
         return node
 
     def run(self) -> "Node":
         """Decompile a code object"""
         while_fusions = {}
-        node = self._run()
+        node = self._run(while_fusions=while_fusions)
+
+        class WhileBreakFixer(ast.NodeTransformer):
+            def visit_Break(self, node):
+                if hasattr(node, "_loop_node") and node._loop_node in while_fusions:
+                    if DEBUG:
+                        debug("NODE BREAK", node, node._loop_node)
+                    return ast.Continue()
+                return node
 
         node.stmts = [
-            #WhileBreakFixer(while_fusions).visit(
-            (RemoveLastContinue().visit(stmt))
+            WhileBreakFixer().visit(RemoveLastContinue().visit(stmt))
             for stmt in node.stmts
         ]
 
         return node
 
 
-def decompile(code: CodeType, prune: bool=False) -> str:
-    """Decompile a code object"""
-    node = Node.from_code(code, prune=prune)
-    if DEBUG:
-        print("DECOMPILE", node)
-        display(node.draw())
-    return node.run().to_source()
+def getsource(code: CodeType, debug: bool = False) -> str:
+    """
+    Decompile a code object
+
+    Parameters
+    ----------
+    code: CodeType
+        The code object to decompile
+    debug: bool
+        Whether to activate the debugging mode and visualize the graph reductions
+    """
+    with set_debug(debug):
+        node = Node.from_code(code)
+        if DEBUG:
+            display(node.draw())
+        return node.run().to_source()
 
 
 def detect_first_node(root):
     visited = set()
 
     best = root
 
@@ -1048,14 +1603,15 @@
                 continue
             rec(succ)
 
     rec(root)
 
     return best
 
+
 def explore_until(root, stops):
     if not stops:
         return None
 
     stops = list(stops)
     visited = set()
 
@@ -1064,118 +1620,143 @@
             return node
 
         if node in visited:
             return None
 
         visited.add(node)
 
-        results = [
-            rec(succ)
-            for succ in (node.next, *node.jumps)
-            if succ is not None
-        ]
+        results = [rec(succ) for succ in (node.next, *node.jumps) if succ is not None]
         res = min(filter(bool, results), key=stops.index, default=None)
         return res
 
     return rec(root)
 
 
 def process_binding_(node, save_origin=True):
     # assert len(block.pred) <= 1
     opname = node.opname
     arg = node.arg
     code = node.code
     idx = node.op_idx
     opname = opname.split("_")[1]
 
-    origin = (dict(
-        _origin_offset=idx,
-        _origin_node=node,
-    ) if save_origin else {})
+    origin = (
+        dict(
+            _origin_offset=idx,
+            _origin_node=node,
+        )
+        if save_origin
+        else {}
+    )
 
     if opname == "FAST":
         node.add_stack(
             ast.Name(
-                id=code.co_varnames[arg], **origin,
+                id=code.co_varnames[arg],
+                **origin,
             )
         )
     elif opname in ("NAME", "GLOBAL"):
         node.add_stack(
             ast.Name(
-                id=code.co_names[arg], **origin,
+                id=code.co_names[arg],
+                **origin,
             )
         )
     elif opname == "DEREF":
         node.add_stack(
             ast.Name(
-                id=(code.co_cellvars + code.co_freevars)[arg], **origin,
+                id=(code.co_cellvars + code.co_freevars)[arg],
+                **origin,
             )
         )
     elif opname == "CONST":
         const_value = code.co_consts[arg]
         if isinstance(const_value, frozenset):
             const_value = set(const_value)
         node.add_stack(
             ast.Constant(
                 value=const_value,
-                kind=None, **origin,
+                kind=None,
+                **origin,
             )
         )
     # ATTRIBUTES
     elif opname in ("ATTR", "METHOD"):
         value = node.pop_stack()
         node.add_stack(
             ast.Attribute(
                 value=value,
-                attr=code.co_names[arg], **origin,
+                attr=code.co_names[arg],
+                **origin,
             )
         )
     elif opname in ("SUBSCR",):
         value = node.pop_stack()
         node.add_stack(
             ast.Subscript(
                 slice=value,
-                value=node.pop_stack(), **origin,
+                value=node.pop_stack(),
+                **origin,
             )
         )
     else:
-        raise ValueError("Unknown opname", opname) # pragma: no cover
+        raise ValueError("Unknown opname", opname)  # pragma: no cover
 
 
 def process_store_(node: Node):
     process_binding_(node)
     target = node.pop_stack()
     value = node.pop_stack()
     if isinstance(value, ast.AugAssign):
         node.add_stmt(value)
     elif isinstance(value, ast.FunctionDef) and isinstance(target, ast.Name):
         node.add_stmt(value)
     else:
-        last_stmts = node.last_stmts()#next(iter(node.prev)).stmts if len(node.prev) == 1 else []
+        last_stmts = (
+            node.last_stmts()
+        )  # next(iter(node.prev)).stmts if len(node.prev) == 1 else []
 
         unpacking = value if isinstance(value, Unpacking) else None
         if unpacking:
             value = value.value
             target = ast.Starred(target) if unpacking.starred else target
             multi_targets = [ast.Tuple([target])]
         else:
             multi_targets = [target]
 
-
         try:
             is_multi_assignment = (
                 len(last_stmts)
                 and isinstance(last_stmts[-1], ast.Assign)
                 and get_origin(value)[1] <= get_origin(last_stmts[-1].targets)[1]
             )
-            debug(f"ORIGIN of {ast.dump(value)}", get_origin(value)[1], f"vs ORIGIN of last {ast.dump(last_stmts[-1])}", get_origin(last_stmts[-1].targets)[1])
-        except Exception as e:
+            if DEBUG:
+                debug(
+                    f"ORIGIN of {ast.dump(value)}",
+                    get_origin(value)[1],
+                    f"vs ORIGIN of last {ast.dump(last_stmts[-1])}",
+                    get_origin(last_stmts[-1].targets)[1],
+                )
+        except Exception:
             is_multi_assignment = False
 
-        debug("VALUE", value, "LAST", last_stmts, "MULTI", multi_targets, "UNPACKING", unpacking, "=> IS_MULTI:", is_multi_assignment)
+        if DEBUG:
+            debug(
+                "VALUE",
+                value,
+                "LAST",
+                last_stmts,
+                "MULTI",
+                multi_targets,
+                "UNPACKING",
+                unpacking,
+                "=> IS_MULTI:",
+                is_multi_assignment,
+            )
         if is_multi_assignment:
             prev = last_stmts.pop()
             prev_multi_targets = prev.targets
 
             if (
                 (not unpacking and prev.value is value)
                 or (
@@ -1209,18 +1790,240 @@
                 # value is value
 
         node.add_stmt(
             ast.Assign(
                 targets=multi_targets,
                 value=value,
             ),
-            # start=op_idx,
         )
 
 
+def process_try_(node, loop_heads, stop_nodes, while_fusions):
+    next_node = node.next
+    [jump_node] = node.jumps
+
+    old_next_node = next_node
+    old_jump_node = jump_node
+    jump_node.stack = [
+        *node.stack,
+        None,
+        None,
+        ExceptionPlaceholder(_dumped=True),
+        None,
+    ]
+
+    meet_nodes = list(
+        lowest_common_successors(
+            next_node,
+            jump_node,
+            stop_nodes={*stop_nodes, node},
+        )
+    )
+    if DEBUG:
+        debug(
+            "TRY BLOCK", node, "MEET", meet_nodes, "(STOP at", {*stop_nodes, node}, ")"
+        )
+    assert len(meet_nodes) <= 1
+
+    before = (next_node, jump_node)
+    next_node = next_node._run(
+        stop_nodes={*stop_nodes, *meet_nodes, node},
+        loop_heads=loop_heads,
+        while_fusions=while_fusions,
+    )
+    jump_node = jump_node._run(
+        stop_nodes={*stop_nodes, *meet_nodes, node},
+        loop_heads=loop_heads,
+        while_fusions=while_fusions,
+    )
+    if (
+        len(meet_nodes)
+        and meet_nodes[0].opname == "POP_BLOCK"
+        and meet_nodes[0] not in stop_nodes
+    ):
+        finally_node = meet_nodes[0]
+        old_finally_node = finally_node
+        old_prev, finally_node.prev = finally_node.prev, {node}
+        print("FOUND FINALLY", finally_node, "STOP AT", {*stop_nodes, node})
+        finally_node = finally_node._run(
+            stop_nodes={*stop_nodes, node},
+            loop_heads=loop_heads,
+            while_fusions=while_fusions,
+            stop_on_jump=True,
+        )
+        finally_node.prev = old_prev
+    else:
+        finally_node = old_finally_node = None
+
+    if DEBUG:
+        debug("TRY", node, "MEET", meet_nodes)
+    if DEBUG:
+        debug("TRY", node, "BEFORE succ", before, "-> AFTER succ", next_node, jump_node)
+
+    handlers = []
+    finalbody = []
+    if (
+        jump_node.stmts
+        and isinstance(jump_node.stmts[0], ast.If)
+        and isinstance(jump_node.stmts[0].test, ExceptionMatch)
+    ):
+        except_stmts = list(jump_node.stmts[0].body)
+        if isinstance(except_stmts[0], ast.Assign) and isinstance(
+            except_stmts[0].value, ExceptionPlaceholder
+        ):
+            name = except_stmts.pop(0).targets[0].id
+            # To handle auto-generated try/finally block
+            # with e = None; del e; instruction at the end of the generated try body
+            except_stmts = list(except_stmts[0].body)
+            i = next(
+                i
+                for i, s in enumerate(except_stmts)
+                if isinstance(s, ast.Delete) and s.targets[0].id == name
+            )
+            except_stmts = except_stmts[: i - 1] + except_stmts[i + 1 :]
+        else:
+            name = None
+        handlers.append(
+            ast.ExceptHandler(
+                type=jump_node.stmts[0].test.value,
+                name=name,
+                body=except_stmts,
+            )
+        )
+    elif isinstance(jump_node.stmts[-1], Reraise):
+        finalbody = jump_node.stmts[:-1]
+    else:
+        handlers.append(
+            ast.ExceptHandler(
+                type=None,
+                name=None,
+                body=jump_node.stmts,
+            )
+        )
+    if finally_node:
+        finalbody = finally_node.stmts
+
+    if (
+        next_node.stmts
+        and isinstance(next_node.stmts[0], ast.Try)
+        and not getattr(next_node.stmts[0], "_try_was_deduplicated", False)
+        and next_node.stmts[0].handlers
+        and next_node.stmts[0].finalbody
+    ):
+        print("DEDUPLICATING TRY", next_node.stmts[0], "WITH", node)
+        next_node.stmts[0]._try_was_deduplicated = True
+        node.stmts.extend(next_node.stmts)
+    else:
+        node.add_stmt(
+            ast.Try(
+                body=next_node.stmts if next_node else [ast.Pass()],
+                handlers=handlers,
+                orelse=[],  # TODO
+                finalbody=finalbody,  # TODO
+            )
+        )
+
+    # noinspection PyTypeChecker
+    successors: Set[Node] = {
+        *((next_node.next, *next_node.jumps) if next_node else (node.next,)),
+        *((jump_node.next, *jump_node.jumps) if jump_node else node.jumps),
+        *((finally_node.next, *finally_node.jumps) if finally_node else ()),
+    } - {
+        None
+    }  # type: ignore
+    discarded_successors = {
+        n
+        for n in (
+            next_node,
+            jump_node,
+            old_next_node,
+            old_jump_node,
+            finally_node,
+            old_finally_node,
+        )
+        if n and n.visited
+    }
+    if DEBUG:
+        debug("TRY SUCC", successors, "-", discarded_successors)
+    if DEBUG:
+        debug("TRY PREV", node.prev)
+    successors = successors - discarded_successors
+
+    jump_nodes = successors
+    for succ in successors:
+        if DEBUG:
+            debug(
+                "TRY",
+                node,
+                ": REBINDING SUCCESSOR",
+                succ,
+                "=>",
+                succ.prev,
+                "->",
+                succ.prev - {next_node, jump_node} | {node},
+            )
+        succ.prev = (succ.prev - discarded_successors) | {node}
+    for n in discarded_successors:
+        for p in n.prev:
+            if p.next in discarded_successors:
+                p.next = node
+            p.jumps = {node if j in discarded_successors else j for j in p.jumps}
+        n.prev = n.prev - discarded_successors
+    node.next = None
+    node.jumps = jump_nodes
+    if DEBUG:
+        debug("TRY", node, node.stack)
+
+    if DEBUG:
+        display(node.draw())
+
+
+def prune_virtual_edges(root):
+    queue = [(root, 0)]
+    graph = set()
+
+    while queue:
+        node, level = queue.pop(0)
+        graph.add(node)
+
+        if node.virtual is None:
+            node.virtual = level
+        else:
+            new_level = min(node.virtual, level)
+            if new_level == node.virtual:
+                continue
+            node.virtual = new_level
+        if node.next and node.next_is_virtual:
+            queue.append((node.next, level + 1))
+        elif node.next:
+            queue.append((node.next, level))
+        for succ in node.jumps:
+            queue.append((succ, level))
+
+    for node in graph:
+        for prev in tuple(node.prev):
+            if (
+                prev.virtual
+                and node.virtual
+                and prev.virtual > node.virtual
+                and prev.next is node
+            ):
+                node.prev.discard(prev)
+                prev.next = None
+            if (
+                prev.virtual
+                and node.virtual
+                and prev.virtual
+                and prev.virtual == node.virtual
+                and prev.next_is_virtual
+                and prev.next is node
+            ):
+                node.prev.discard(prev)
+                prev.next = None
+
 
 def contract_jumps(root):
     queue = [root]
     seen = set()
 
     while queue:
         node = queue.pop(0)
@@ -1251,28 +2054,28 @@
 
     while queue:
         node, loop_jumps = queue.pop(0)
         if not node or node in seen:
             continue
         seen.add(node)
         if node.opname == "SETUP_LOOP":
-            #jump_node = next(iter(node.jumps))
+            # jump_node = next(iter(node.jumps))
             jump_node = node.jumps.pop()
             jump_node.prev.discard(node)
             queue.append((node.next, [*loop_jumps, jump_node]))
             queue.append((jump_node, loop_jumps))
         elif node.opname == "BREAK_LOOP":
             node.opname = "JUMP_ABSOLUTE"
-            #node.next_is_virtual = True
+            # node.next_is_virtual = True
             if node.next:
                 node.next.prev.discard(node)
                 node.next = None
             node.arg = None
             loop_jumps[-1].prev.add(node)
             node.jumps = {loop_jumps[-1]}
             queue.append((node.next, loop_jumps))
         else:
             queue.append((node.next, loop_jumps))
             for jump in node.jumps:
                 queue.append((jump, loop_jumps))
 
-    return root
+    return root
```

### Comparing `pygetsource-0.0.0/pygetsource/factory.py` & `pygetsource-0.1.0/pygetsource/factory.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/pygetsource/utils.py` & `pygetsource-0.1.0/pygetsource/utils.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/pygetsource.egg-info/PKG-INFO` & `pygetsource-0.1.0/pygetsource.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.0.0
+Version: 0.1.0
 Summary: Decompiler written in Python for Python
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,19 @@
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
+<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+
+
 # pygetsource
 
 `pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
```

### Comparing `pygetsource-0.0.0/pyproject.toml` & `pygetsource-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/tests/test_py37.py` & `pygetsource-0.1.0/tests/test_py37.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.0.0/tests/test_rebuild.py` & `pygetsource-0.1.0/tests/test_rebuild.py`

 * *Files identical despite different names*

