# Comparing `tmp/syntaxlight-0.0.4.tar.gz` & `tmp/syntaxlight-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.4.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.5.tar", max compression
```

## Comparing `syntaxlight-0.0.4.tar` & `syntaxlight-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.4/LICENSE
--rw-r--r--   0        0        0      464 2023-07-21 06:02:06.182590 syntaxlight-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1632 2023-07-20 09:56:07.920078 syntaxlight-0.0.4/README.md
--rw-r--r--   0        0        0      191 2023-07-19 07:19:43.518938 syntaxlight-0.0.4/syntaxlight/__init__.py
--rw-r--r--   0        0        0    13864 2023-07-20 09:35:37.730553 syntaxlight-0.0.4/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.4/syntaxlight/css/all.css
--rw-r--r--   0        0        0     2081 2023-07-19 08:12:53.632477 syntaxlight-0.0.4/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.4/syntaxlight/css/index.css
--rw-r--r--   0        0        0      485 2023-07-19 08:11:30.544637 syntaxlight-0.0.4/syntaxlight/css/json.css
--rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.4/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.4/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.4/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.4/syntaxlight/error.py
--rw-r--r--   0        0        0     1995 2023-07-21 06:00:15.010137 syntaxlight-0.0.4/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.4/syntaxlight/export.py
--rw-r--r--   0        0        0      406 2023-07-20 13:32:30.588909 syntaxlight-0.0.4/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0    12379 2023-07-19 02:03:36.729775 syntaxlight-0.0.4/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     2219 2023-07-04 09:22:19.741835 syntaxlight-0.0.4/syntaxlight/lexers/ebnf_lexer.py
--rw-r--r--   0        0        0     1864 2023-07-04 09:20:59.243201 syntaxlight-0.0.4/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    19627 2023-07-19 02:25:52.820410 syntaxlight-0.0.4/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.4/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.4/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3538 2023-07-06 06:05:23.042009 syntaxlight-0.0.4/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4578 2023-07-20 13:32:30.928035 syntaxlight-0.0.4/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      205 2023-07-12 06:09:50.252799 syntaxlight-0.0.4/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0   100677 2023-07-21 05:59:31.524515 syntaxlight-0.0.4/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0      989 2023-07-04 09:23:16.797987 syntaxlight-0.0.4/syntaxlight/parsers/ebnf_parser.py
--rw-r--r--   0        0        0     5758 2023-07-10 15:27:05.012220 syntaxlight-0.0.4/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0     8881 2023-07-21 05:50:20.656491 syntaxlight-0.0.4/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.4/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11786 2023-07-16 15:52:23.224969 syntaxlight-0.0.4/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-15 15:57:39.737127 syntaxlight-0.0.4/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     3835 2023-07-21 05:48:12.460063 syntaxlight-0.0.4/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.4/syntaxlight/template.html
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 syntaxlight-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.5/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-24 08:09:12.714704 syntaxlight-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.5/README.md
+-rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.5/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    14933 2023-07-24 07:57:41.164021 syntaxlight-0.0.5/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.5/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.5/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.5/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.5/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.5/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.5/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.5/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.5/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.5/syntaxlight/error.py
+-rw-r--r--   0        0        0     2009 2023-07-24 08:05:40.440581 syntaxlight-0.0.5/syntaxlight/example.py
+-rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.5/syntaxlight/export.py
+-rw-r--r--   0        0        0     2725 2023-07-23 15:16:02.280132 syntaxlight-0.0.5/syntaxlight/gdt.py
+-rw-r--r--   0        0        0      388 2023-07-22 13:46:05.416059 syntaxlight-0.0.5/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     1923 2023-07-22 13:45:56.258345 syntaxlight-0.0.5/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12472 2023-07-24 01:14:51.430992 syntaxlight-0.0.5/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     1997 2023-07-21 12:49:29.104139 syntaxlight-0.0.5/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    19933 2023-07-24 06:59:03.624407 syntaxlight-0.0.5/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.5/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.5/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     2870 2023-07-22 13:41:57.282224 syntaxlight-0.0.5/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4578 2023-07-20 13:32:30.928035 syntaxlight-0.0.5/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      240 2023-07-21 14:12:28.396351 syntaxlight-0.0.5/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     6858 2023-07-24 01:35:24.029532 syntaxlight-0.0.5/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   100128 2023-07-24 08:05:22.752514 syntaxlight-0.0.5/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.5/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0     9682 2023-07-24 07:47:18.356056 syntaxlight-0.0.5/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.5/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.5/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.5/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     3906 2023-07-24 01:38:00.242828 syntaxlight-0.0.5/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.5/syntaxlight/template.html
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.5/PKG-INFO
```

### Comparing `syntaxlight-0.0.4/LICENSE` & `syntaxlight-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/README.md` & `syntaxlight-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -30,12 +30,31 @@
 dot -Tpng ./ast.dot -o ast.png
 ```
 
 ## 文档和 API
 
 关于详细的 API 使用方法, 以及对于默认配置的修改情况请参阅 [syntaxlight 使用文档](https://luzhixing12345.github.io/syntaxlight/)
 
+## 开发功能
+
+本仓库的 Makefile 与 test.py 提供了对于测试用例的渲染预览, 运行后打开 syntaxlight_example/index.html 即可
+
+```bash
+# 浏览所有 C 测试用例集合渲染结果
+make 
+
+# 浏览所有 json 测试用例集合渲染结果
+make t=json
+
+# 浏览 json 第一个 test/json/1.json 测试用例渲染结果
+make t=json i=1
+
+# 浏览 toml 第一个 test/toml/1.json 测试用例在 one-dark-pro 风格下的渲染结果
+make t=toml i=1 s=one-dark-pro
+```
+
 ## 参考
 
 - [Let's Build A Simple Interpreter](https://ruslanspivak.com/lsbasi-part1/)
+- [tree-sitter](https://github.com/tree-sitter/tree-sitter)
 - [pygments](https://pygments.org/)
 - [carbon](https://carbon.now.sh/)
```

### Comparing `syntaxlight-0.0.4/syntaxlight/ast.py` & `syntaxlight-0.0.5/syntaxlight/ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,32 @@
 import textwrap
-
+from enum import Enum
 from .lexers import Token
-from typing import List, Union
+from typing import List, Union, Dict, Tuple
+from .gdt import Enum
 
 AST_CREATED_INDEX = 0
 
 
-class GlobalDescriptorTable:
-    def __init__(self) -> None:
-        self.descriptors = {}
-
-    def register_id(self, name, class_name):
-        if self.descriptors.get(name) is None:
-            self.descriptors[name] = class_name
-
-    def reset(self):
-        self.descriptors = {}
-
-    def __getitem__(self, index):
-        return self.descriptors[index]
-
-    def __contains__(self, item):
-        return item in self.descriptors
-
-
 class AST(object):
     def __init__(self) -> None:
         # 节点被创建的顺序
         global AST_CREATED_INDEX
-        self.created_index = AST_CREATED_INDEX
+        self._created_index = AST_CREATED_INDEX
         AST_CREATED_INDEX = AST_CREATED_INDEX + 1
 
         self.class_name: str = self.__class__.__name__
-        self._node_info: str = f"[{self.class_name}:{self.created_index}]"
+        self.node_info: str = f"[{self.class_name}:{self._created_index}]"
 
-        self.indent = " " * 4
+        self._indent = " " * 4
         # AST 树包含的 Token
         self._tokens: List[Token] = []
-        self.depth = 0  # 节点深度
-        self.is_bottom_ast = False  # 底层 AST
+        self._depth = 0  # 节点深度
+        self.is_leaf_ast = False  # 底层 AST, 叶节点
+        self.update_subnode = False  # update 时将 class_name 传递到所有的子 AST 节点中
 
     def register_token(self, tokens: List[Token], extra_class_name: str = None):
         """
         将 token 注册到 AST 树中以更新 token 的属性
         """
         for token in tokens:
             token.class_list.add(self.class_name)
@@ -51,41 +35,67 @@
             self._tokens.append(token)
             token.ast = self
 
     def update(self, **kwargs):
         """
         对于一些后续才可以获取的属性, 或者子 AST 节点的注册, 调用此方法更新子 AST 对象内部的元素
         """
-        for key, value in kwargs.items():
-            setattr(self, key, value)
+        for key, node in kwargs.items():
+            setattr(self, key, node)
             # update 的时候将子元素的 token 也添加当前 AST 的 class
-            if isinstance(value, AST):
-                for token in value._tokens:
+            if isinstance(node, AST):
+                for token in node._tokens:
                     token.class_list.add(self.class_name)
+            if self.update_subnode:
+                self._update_sub_ast(node, self.class_name)
+
+    def _update_sub_ast(self, node: "AST", class_name: str):
+        """
+        为叶节点补充添加类名信息, 但 token 会有很复杂的 class name, 不宜采用
+        """
+        if node is None:
+            return
+        if type(node) == list:
+            for nod in node:
+                self._update_sub_ast(nod, class_name)
+            return
+        if node.is_leaf_ast:
+            node.class_name = class_name
+            for token in node._tokens:
+                token.class_list.add(class_name)
+            return
+        else:
+            for _, attribute_value in vars(node).items():
+                if isinstance(attribute_value, AST):
+                    self._update_sub_ast(attribute_value, class_name)
+                elif type(attribute_value) == list:
+                    if len(attribute_value) > 0 and isinstance(attribute_value[0], AST):
+                        for a_v in attribute_value:
+                            self._update_sub_ast(a_v, class_name)
 
     def visit(self, node_visitor: "NodeVisitor" = None):
         """
         由 node visitor 访问时递归调用
         """
         node_visitor.depth -= 1  # 到达叶节点, 退出到上一层
         # print(f'visit {self.class_name}, depth = {self.depth}')
 
     def formatter(self, depth: int = 0):
         raise NotImplementedError(self.class_name + " should override format function to display")
 
-    def __str__(self) -> str:
-        return self.formatter()
+    # def __str__(self) -> str:
+    #     return self.formatter()
 
-    def __repr__(self) -> str:
-        return self.__str__()
+    # def __repr__(self) -> str:
+    #     return self.__str__()
 
     def get_node_info(self):
         # f'depth={self.depth}\\n'
-        node_content = self._node_info + "\\n" + f"depth={self.depth}"
-        return f'node{self.created_index} [label="{node_content}"]'
+        node_content = self.node_info + "\\n" + f"depth={self._depth}"
+        return f'node{self._created_index} [label="{node_content}"]'
 
 
 class Object(AST):
     """
     { pair1, pair2, ...}
     """
 
@@ -106,19 +116,19 @@
         if self._inside_array:
             depth += 1
         result = "{"
         if len(self.pairs) == 0:
             result += " }"
         else:
             result += "\n"
-            result += self.indent * (depth + 1) + f"{self.pairs[0].formatter(depth)}"
+            result += self._indent * (depth + 1) + f"{self.pairs[0].formatter(depth)}"
             for i in range(1, len(self.pairs)):
                 member = self.pairs[i]
-                result += f",\n{self.indent * (depth+1)}{member.formatter(depth)}"
-            result += "\n" + self.indent * depth + "}"
+                result += f",\n{self._indent * (depth+1)}{member.formatter(depth)}"
+            result += "\n" + self._indent * depth + "}"
         return result
 
 
 class Array(AST):
     """
     [ element1, elements2, ...]
     """
@@ -141,107 +151,115 @@
         for e in self.elements:
             if e.class_name == "Object":
                 e._inside_array = True
         if len(self.elements) == 0:
             result += " ]"
         else:
             result += "\n"
-            result += self.indent * (depth + 1) + f"{self.elements[0].formatter(depth)}"
+            result += self._indent * (depth + 1) + f"{self.elements[0].formatter(depth)}"
             for i in range(1, len(self.elements)):
                 element = self.elements[i]
-                result += f",\n{self.indent * (depth+1)}{element.formatter(depth)}"
-            result += "\n" + self.indent * depth + "]"
+                result += f",\n{self._indent * (depth+1)}{element.formatter(depth)}"
+            result += "\n" + self._indent * depth + "]"
         return result
 
 
 class Pair(AST):
     def __init__(self, key: AST = None, value: AST = None) -> None:
         super().__init__()
         self.key: AST = key
         self.value: AST = value
 
-    def update(self, **kwargs):
-        return super().update(**kwargs)
-
     def visit(self, node_visitor: "NodeVisitor" = None):
         node_visitor.link(self, self.key)
         node_visitor.link(self, self.value)
         return super().visit(node_visitor)
 
     def formatter(self, depth: int = 0):
         return f"{self.key.formatter(depth+1)}: {self.value.formatter(depth+1)}"
 
 
 class Keyword(AST):
     def __init__(self, name) -> None:
         super().__init__()
         self.name: str = name
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.name}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.name}"
 
     def formatter(self, depth: int = 0):
         return self.name
 
 
 class Identifier(AST):
     def __init__(self, id) -> None:
         super().__init__()
         self.id: str = id
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.id}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.id}"
+
+
+class Punctuator(AST):
+    def __init__(self) -> None:
+        super().__init__()
+        self.op = self.op
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.op}"
 
 
 class Constant(AST):
     def __init__(self, constant) -> None:
         super().__init__()
         self.constant = constant
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.constant}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.constant}"
 
 
 class String(AST):
     def __init__(self, string) -> None:
         super().__init__()
         self.string: str = string
-        self.is_bottom_ast = True
+        self.is_leaf_ast = True
 
         string_info = self.string.replace("\\", "\\\\").replace('"', '\\"')
-        self._node_info += f"\\n{string_info}"
+        self.node_info += f"\\n{string_info}"
+
+    def __str__(self) -> str:
+        return self.string
 
     def formatter(self, depth: int = 0):
         return self.string
 
 
 class Char(AST):
     def __init__(self, string) -> None:
         super().__init__()
         self.string = string
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.string}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.string}"
 
     def formatter(self, depth: int = 0):
         return self.string
 
 
 class Number(AST):
     def __init__(self, value) -> None:
         super().__init__()
         self.value = value
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.value}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.value}"
 
     def formatter(self, depth: int = 0):
         return self.value
 
 
 class Punctuator(AST):
     def __init__(self, op) -> None:
         super().__init__()
         self.op = op
-        self.is_bottom_ast = True
+        self.is_leaf_ast = True
 
     def formatter(self, depth: int = 0):
         return self.op
 
 
 class UnaryOp(AST):
     def __init__(self, expr: AST = None, op: str = None) -> None:
@@ -270,16 +288,16 @@
         return super().visit(node_visitor)
 
 
 class AssignOp(AST):
     def __init__(self, op: str = None) -> None:
         super().__init__()
         self.op = op
-        self.is_bottom_ast = True
-        self._node_info += f"\\n{self.op}"
+        self.is_leaf_ast = True
+        self.node_info += f"\\n{self.op}"
 
     def visit(self, node_visitor: "NodeVisitor" = None):
         return super().visit(node_visitor)
 
 
 class ConditionalExpression(AST):
     def __init__(self) -> None:
@@ -338,15 +356,15 @@
 
     def register(self, node: AST, depth: int):
         if node in self.visit_node_list:
             print("visit the same node!!!")
             exit(1)
         else:
             # 更新 AST 节点的深度
-            node.depth = depth
+            node._depth = depth
             self.visit_node_list.append(node)
 
         self.dot_body.append(node.get_node_info())
 
     def link(self, root: AST, node: AST):
         """
         usage inside AST : node_visitor.link(self, self.xxx)
@@ -363,15 +381,15 @@
         if type(node) == list:
             for n in node:
                 self.link(root, n)
             return
         if node not in self.visit_node_list:
             self.register(node, self.depth + 1)
 
-        self.dot_body.append(f"node{root.created_index} -> node{node.created_index}")
+        self.dot_body.append(f"node{root._created_index} -> node{node._created_index}")
         self.depth += 1
         node.visit(self)
 
     def save(self):
         """
         save in graphviz pic
         """
@@ -381,72 +399,74 @@
             graphviz_content += f"    {dot}\n"
         graphviz_content += self.dot_footer
         with open(self.image_name, "w", encoding="utf-8") as f:
             f.write(graphviz_content)
         print(f"ast tree saved in [{self.image_name}], view by grpahviz")
 
 
-def display_ast(node: AST, save_ast_tree = False):
+def display_ast(node: AST, sub_roots: List[AST], save_ast_tree=False):
     node_visitor = NodeVisitor()
     node.visit(node_visitor)
+    for sub_root in sub_roots:
+        node_visitor.depth += 1
+        sub_root.visit(node_visitor)
 
     if save_ast_tree:
         node_visitor.save()
     # node.formatter()
-
     assert node_visitor.depth == -1
 
 
-def add_ast_type(node: AST, class_name: str):
+def add_ast_type(node: AST, css_type: Enum):
     """
-    为节点补充添加类名信息, 比如返回值 ReturnValue
+    为叶节点补充添加类名信息
     """
     if node is None:
         return
     if type(node) == list:
         for nod in node:
-            add_ast_type(nod, class_name)
+            add_ast_type(nod, css_type)
         return
 
-    if node.is_bottom_ast:
-        node.class_name = class_name
+    if node.is_leaf_ast:
+        node.class_name = css_type.value
         for token in node._tokens:
-            token.class_list.add(class_name)
+            token.class_list.add(css_type.value)
             # print(token, f"[{class_name}]")
         return
     else:
         # 遍历对象的所有属性
         for _, attribute_value in vars(node).items():
             if isinstance(attribute_value, AST):
-                add_ast_type(attribute_value, class_name)
+                add_ast_type(attribute_value, css_type)
             elif type(attribute_value) == list:
                 if len(attribute_value) > 0 and isinstance(attribute_value[0], AST):
                     for a_v in attribute_value:
-                        add_ast_type(a_v, class_name)
+                        add_ast_type(a_v, css_type)
+
 
-def delete_ast_type(node: AST, class_name: str):
+def delete_ast_type(node: AST, css_type: Enum):
     """
-    为节点补充去除类名信息
+    为叶节点补充去除类名信息
     """
-    # print(node.class_name)
     if node is None:
         return
     if type(node) == list:
         for nod in node:
-            delete_ast_type(nod, class_name)
+            delete_ast_type(nod, css_type)
         return
 
-    if node.is_bottom_ast:
+    if node.is_leaf_ast:
         for token in node._tokens:
-            if class_name in token.class_list:
-                token.class_list.remove(class_name)
+            if css_type.value in token.class_list:
+                token.class_list.remove(css_type.value)
             # print(token, f"[{class_name}]")
         return
     else:
         # 遍历对象的所有属性
         for _, attribute_value in vars(node).items():
             if isinstance(attribute_value, AST):
-                delete_ast_type(attribute_value, class_name)
+                delete_ast_type(attribute_value, css_type)
             elif type(attribute_value) == list:
                 if len(attribute_value) > 0 and isinstance(attribute_value[0], AST):
                     for a_v in attribute_value:
-                        delete_ast_type(a_v, class_name)
+                        delete_ast_type(a_v, css_type)
```

### Comparing `syntaxlight-0.0.4/syntaxlight/css/all.css` & `syntaxlight-0.0.5/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/css/c.css` & `syntaxlight-0.0.5/syntaxlight/css/c.css`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 .Token.TRUE,
 .Token.FALSE,
 .Token.NULL {
     color: --type;
 }
 
 .Token.STRING,
-.Token.STR {
+.Token.CHARACTER {
     color: --string;
 }
 
 .Token.STRING.Format {
     color: --format;
 }
 
@@ -108,15 +108,16 @@
 }
 
 .Token.FunctionName.ID,
 .Token.FunctionCall.ID {
     color: --function;
 }
 
-.Token.DefineName.ID,
+.Token.MacroDefine.ID,
+.Token.MarcroFunction.ID,
 .Token.BACK_SLASH {
     color: --type;
 }
 
 .Token.FunctionP.ID {
     color: --variant;
 }
@@ -125,15 +126,15 @@
     color: --define;
 }
 
 .Token.Enumerator.ID {
     color: --enum;
 }
 
-.Token.StructClass,
+.Token.StructureClass,
 .Token.EnumID,
 .Token.Typedefine {
     color: --struct;
 }
 
 .Token.LT,
 .Token.GT,
```

### Comparing `syntaxlight-0.0.4/syntaxlight/css/index.css` & `syntaxlight-0.0.5/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/css/themes.json` & `syntaxlight-0.0.5/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/css/toml.css` & `syntaxlight-0.0.5/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/error.py` & `syntaxlight-0.0.5/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/example.py` & `syntaxlight-0.0.5/syntaxlight/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .export import export_css
 from typing import Union, List
 
 
 def example_display(
     file_path: Union[str, List[str]] = None,
     style="vscode",
-    save_ast_tree=True,
+    save_ast_tree=False,
     language: str = "guess",
 ):
     example_folder_name = os.path.join(os.getcwd(), "syntaxlight_example")
     if language == "guess":
         if type(file_path) == list:
             language = guess_language(file_path[0])
         else:
@@ -33,22 +33,22 @@
         file_path = [file_path]
 
     code_html = ""
     for fp in file_path:
         html = parse_file(fp, language, save_ast_tree=save_ast_tree)
         if html is None:
             continue
-        code_html += f'<pre class="language-{language}"><code>{html}</code></pre>'
+        code_html += f'<p>{fp}</p><pre class="language-{language}"><code>{html}</code></pre>'
 
     code_html = f'<div class="markdown-body">{code_html}</div>'
     with open(html_template_file, "r", encoding="utf-8") as f:
         content = f.read().replace("html-scope", code_html).replace("css-scope", css_scope)
 
     with open(os.path.join(example_folder_name, example_html_file), "w", encoding="utf-8") as f:
         f.write(content)
 
     for file in css_files:
         shutil.copyfile(file, os.path.join(example_folder_name, file.split(os.sep)[-1]))
 
     export_name = os.path.join(example_folder_name, f"{language}.css")
     export_css([language], export_name, style)
-    print(f"open syntaxlight_example/inedx.html in browser")
+    # print(f"open syntaxlight_example/inedx.html in browser")
```

### Comparing `syntaxlight-0.0.4/syntaxlight/export.py` & `syntaxlight-0.0.5/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/c_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,18 +124,18 @@
         self.advance()
         result = "'" + self.current_char
         if self.current_char == "\\":
             self.advance()
             result += self.current_char
         self.advance()
         if self.current_char != "'":
-            token = Token(TokenType.CHAR, result, self.line, self.column)
+            token = Token(TokenType.CHARACTER, result, self.line, self.column)
             self.error(ErrorCode.MULTICHARACTER_CONSTANT, token)
         result += "'"
-        token = Token(TokenType.CHAR, result, self.line, self.column)
+        token = Token(TokenType.CHARACTER, result, self.line, self.column)
         self.advance()
         return token
 
     def get_next_token(self):
         while self.current_char is not None:
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
@@ -262,15 +262,15 @@
         )
 
         self.identifier = TokenSet(TokenType.ID)
         self.parameter_declaration = TokenSet(self.declaration_specifier)
         self.parameter_list = TokenSet(self.parameter_declaration)
         self.constant = TokenSet(TokenType.NUMBER, CTokenType.TRUE, CTokenType.FALSE)
         self.primary_expression = TokenSet(
-            TokenType.ID, TokenType.STRING, TokenType.LPAREN, TokenType.CHAR, self.constant
+            TokenType.ID, TokenType.STRING, TokenType.LPAREN, TokenType.CHARACTER, self.constant
         )
         self.postfix_expression = TokenSet(self.primary_expression, TokenType.LPAREN)
         # postfix_expression 内部的
         self.postfix_expression_inside = TokenSet(
             TokenType.LSQUAR_PAREN,
             TokenType.LPAREN,
             TokenType.DOT,
@@ -295,14 +295,15 @@
         self.assignment_expression = TokenSet(self.unary_expression, self.conditinal_expression)
         self.expression = TokenSet(self.assignment_expression)
         self.direct_abstract_declarator = TokenSet(TokenType.LPAREN, TokenType.LSQUAR_PAREN)
         self.abstract_declarator = TokenSet(TokenType.MUL, self.direct_abstract_declarator)
         self.initializer = TokenSet(self.assignment_expression, TokenType.LCURLY_BRACE)
         self.designator = TokenSet(TokenType.LSQUAR_PAREN, TokenType.DOT)
         self.designation = TokenSet(self.designator)
+        self.initializer_list = TokenSet(self.designation, self.initializer)
 
         self.labeled_statement = TokenSet(self.identifier, CTokenType.CASE, CTokenType.DEFAULT)
         self.expression_statement = TokenSet(self.expression, TokenType.SEMI)
         self.compound_statement = TokenSet(TokenType.LCURLY_BRACE)
         self.selection_statement = TokenSet(CTokenType.IF, CTokenType.SWITCH)
         self.iteration_statement = TokenSet(CTokenType.WHILE, CTokenType.DO, CTokenType.FOR)
         self.jump_statement = TokenSet(
```

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/ebnf_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/json_lexer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,59 @@
 from .lexer import Lexer, Token, TokenType
+from ..error import ErrorCode
 from enum import Enum
 
 
-class EBNFTokenType(Enum):
-    S = "SEPARATOR"
-    GRAMMAR = "GRAMMAR"
-    RULE = "RULE"
-    LHS = "LHS"
-    RHS = "RHS"
-    TERMINATOR = "TERMINATOR"
-    ALTERNATION = "ALTERNATION"
-    IDENTIFIER = "IDENTIFIER"
-    CONCATENATION = "CONCATENATION"
-    FACTOR = "FACTOR"
-    LETTER = "LETTER"
-    DIGIT = "DIGIT"
-    TERM = "TERM"
-    SYMBOL = "SYMBOL"
-    CHARACTER = "CHARACTER"
-    TERMINAL = "TERMINAL"
-    RESERVED_KEYWORD_START = ""
-    RESERVED_KEYWORD_END = ""
-
-
-class EBNFErrorCode(Enum):
-    UNEXPECTED_TOKEN = "Unexpected token"  # 不匹配的 Token 类型
-    ID_NOT_FOUND = "Identifier not found"
-    DUPLICATE_ID = "Duplicate id found"
-    PARAMETERS_NOT_MATCH = "parameter number not match"
-
-
-class EBNFLexer(Lexer):
-    def __init__(self, text: str, LanguageTokenType: Enum = EBNFTokenType):
-        super().__init__(text, LanguageTokenType)
+class JsonTokenType(Enum):
+    # single-character token types
+    RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
 
-    def get_next_token(self) -> Token:
+    # keyword
+    TRUE = "true"
+    FALSE = "false"
+    NULL = "null"
+
+    RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
+
+
+class JsonLexer(Lexer):
+    def __init__(self, text: str, TokenType: Enum = JsonTokenType):
+        super().__init__(text, TokenType)
+
+    def get_next_token(self):
         while self.current_char is not None:
+            # json 仅支持 ""
+            if self.current_char == TokenType.QUOTO.value:
+                return self.get_string()
+
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
-            if self.current_char.isalpha():
-                return self.get_id()
-
-            if self.current_char in ("'", '"'):
-                return self.get_str()
+            if self.current_char.isdigit():
+                return self.get_number()
 
+            if self.current_char.isalnum() or self.current_char == '_':
+                return self.get_id()
+            
+            if self.current_char == '/' and self.peek() == '/':
+                return self.get_comment(('//','\n'))
+            
             try:
-                # get enum member by value, e.g.
-                # TokenType(';') --> TokenType.SEMI
                 token_type = TokenType(self.current_char)
-            except ValueError:
-                # no enum member with value equal to self.current_char
-                self.error()
+            except ValueError: # pragma: no cover
+                token = Token(None, self.current_char, self.line, self.column)
+                self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
-                # create a token with a single-character lexeme as its value
                 token = Token(
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
                 self.advance()
                 return token
-
-        return Token(type=TokenType.EOF, value=None)
+        
+        # End of File
+        return Token(type=TokenType.EOF, value='EOF', line=self.line, column=self.column)
```

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/bnf_lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-from .lexer import Lexer, Token, TokenType
-from ..error import ErrorCode
-from enum import Enum
 
+from .lexer import Lexer, Token, TokenType, TokenSet, ErrorCode
+from enum import Enum
 
-class JsonTokenType(Enum):
-    # single-character token types
+class BNFTokenType(Enum):
     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
-
-    # keyword
-    TRUE = "true"
-    FALSE = "false"
-    NULL = "null"
-
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
 
-class JsonLexer(Lexer):
-    def __init__(self, text: str, TokenType: Enum = JsonTokenType):
-        super().__init__(text, TokenType)
+class BNFLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = BNFTokenType):
+        super().__init__(text, LanguageTokenType)
+        self.build_long_op_dict(["::="])
 
-    def get_next_token(self):
+    def get_next_token(self) -> Token:
+        
         while self.current_char is not None:
-            # json 仅支持 ""
-            if self.current_char == TokenType.QUOTO.value:
-                return self.get_string()
-
-            if self.current_char == TokenType.SPACE.value:
-                return self.skip_whitespace()
-
+            
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
+            
+            if self.current_char == ' ':
+                return self.skip_whitespace()
 
-            if self.current_char.isdigit():
-                return self.get_number()
-
+            if self.current_char in ("'", '"'):
+                return self.get_str()
+            
             if self.current_char.isalnum() or self.current_char == '_':
-                return self.get_id()
+                return self.get_id(extend_chars=['_','-'])
+            
+            if self.current_char == '#':
+                return self.get_comment(("#",'\n'))
+            
+            if self.current_char in self.long_op_dict:
+                return self.get_long_op()
             
             try:
                 token_type = TokenType(self.current_char)
             except ValueError: # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
@@ -47,10 +44,10 @@
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
                 self.advance()
                 return token
-        
-        # End of File
-        return Token(type=TokenType.EOF, value='EOF', line=self.line, column=self.column)
+            
+
+        return Token(type=TokenType.EOF, value='EOF', line=self.line, column=self.column)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     BANG = "!"
     BACKTICK = "`"
     TILDE = "~"
     AT_SIGN = "@"
     EOF = "EOF"
     ID = "ID"
     STRING = "STRING"  # STRING 表示严格意义上的字符串, 即 "" 两个双引号包裹的
-    CHAR = "CHAR"  # CHAR 表示单个字符, 即 'a'
+    CHARACTER = "CHARACTER"  # CHARACTER 表示单个字符, 即 'a'
     STR = "STR"  # STR 表示 "" | '' 包裹的字符串
     NUMBER = "NUMBER"  # 整数 | 小数 | 科学计数法
     INT = "INT"  # 整数
     FLOAT = "FLOAT"  # 小数
     COMMENT = "COMMENT"
     SHL = "<<"
     SHR = ">>"
@@ -84,14 +84,16 @@
     VARARGS = "..."
     DB_COLON = "::"
     INC = "++"
     DEC = "--"
     OR = "||"
     AND = "&&"
     POINT = "->"
+    PRODUCTION_SYMBOL = "::="
+    DOUBLE_HASH = "##"
 
 
 class TTYColor(Enum):
     BLACK = 30
     RED = 31
     GREEN = 32
     YELLOW = 33
@@ -125,21 +127,20 @@
         return css_class
 
     def __str__(self):
         """
         ID 指创建的索引值
         column 指该 token 最后一个字符的位置
         """
-        return "Token[id:{ID}]({type}, {value}, position={lineno}:{column}) {AST_type}".format(
+        return "Token[{ID}]({type}, {value}, position={lineno}:{column})".format(
             ID=self._id,
             type=self.type,
             value=repr(self.value),
             lineno=self.line,
-            column=self.column,
-            AST_type=self.get_css_class(),
+            column=self.column
         )
 
     def __repr__(self):
         return self.__str__()
 
 
 class Lexer:
@@ -156,14 +157,15 @@
         self.pos: int = 0  # 当前指针指向的字符
         self.current_char: str = self.text[self.pos]  # 当前指针指向的字符
         self.line: int = 1
         self.column: int = 1  # 指向 token 的 value 中最后出现的字符的位置
         self.LanguageTokenType: Enum = LanguageTokenType
         self.context_bias = 10  # 发生错误时 token 的前后文行数
         self.file_path = None  # 手动修改文件路径, 用于后期错误处理的输出
+        self._status_stack = [] # 状态栈
 
         # 获取 RESERVED_KEYWORD_START - RESERVED_KEYWORD_END 之间的保留关键字
         tt_list = list(LanguageTokenType)
         start_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_START)
         end_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_END)
         self.reserved_keywords = {
             token_type.value: token_type for token_type in tt_list[start_index + 1 : end_index]
@@ -184,16 +186,16 @@
         #     return self.get_long_op()
         self.long_op_dict: Dict[str, List] = {}
 
     def build_long_op_dict(self, supported_long_op: List[str]):
         """
         构造长运算符的匹配模式
         """
-        self.long_ops = sorted(supported_long_op, key=len, reverse=True)
-        for long_op in self.long_ops:
+        self._long_ops = sorted(supported_long_op, key=len, reverse=True)
+        for long_op in self._long_ops:
             assert len(long_op) >= 2, f"{long_op} should be longer"
             if self.long_op_dict.get(long_op[0]) is None:
                 self.long_op_dict[long_op[0]] = []
             self.long_op_dict[long_op[0]].append(long_op[1:])
 
     def ttyinfo(self, text: str, color: TTYColor = TTYColor.RED) -> str:
         """
@@ -205,26 +207,28 @@
 
     def _record(self):
         """
         用于 parser 中 peek_next_token
 
         记录当前 lexer 解析状态, 被 _reset 调用时恢复
         """
-        self._clone_status = {"pos": self.pos, "line": self.line, "column": self.column}
+        # 采用栈的方式保存数据状态, 避免由于 peek_next_token 中的 eat 导致多次嵌套调用覆盖数据
+        self._status_stack.append({"pos": self.pos, 'c':self.current_char, "line": self.line, "column": self.column})
 
     def _reset(self):
         """
         用于 parser 中 peek_next_token
 
         恢复为 lexer 之前的状态
         """
-        self.pos = self._clone_status["pos"]
-        self.line = self._clone_status["line"]
-        self.column = self._clone_status["column"]
-        self.current_char = self.text[self.pos]
+        status = self._status_stack.pop()
+        self.pos = status["pos"]
+        self.current_char = status['c']
+        self.line = status["line"]
+        self.column = status["column"]
 
     def error(self, error_code: ErrorCode = None, token: Token = None, message: str = ""):
         raise LexerError(
             error_code=error_code,
             token=token,
             context=self.get_error_token_context(token),
             file_path=self.file_path,
@@ -442,21 +446,22 @@
                             ErrorCode.UNEXPECTED_TOKEN,
                             Token(TokenType.STRING, result, self.line, self.column),
                         )
                     count = 0
                     result += self.current_char
                 self.advance()
 
-        token = Token(TokenType.STR, result, self.line, self.column-1)
+        token = Token(TokenType.STR, result, self.line, self.column - 1)
         return token
 
-    def get_id(self, ignore_case=False, extend_chars=["_"]):
+    def get_id(self, ignore_case=False, extend_chars: List[str] = ["_"]):
         """
         获取标识符, 留给后续的语法分析处理
         @ignore_case : 是否忽略大小写
+        @extend_chars: 扩展字符, 默认扩展 "_", 一般还可修改为 ["_", "-"]
 
         <letter> ::= [A-Za-z]
          <digit> ::= [0-9]
             <id> ::= (<letter>|_)(<letter>|_|<digit>)*
 
         此函数应次于 get_number 调用
         """
@@ -492,39 +497,39 @@
 
         start_symbol, end_symbol = comment_symbol
         assert start_symbol[0] == self.current_char
 
         result = start_symbol
         for _ in range(len(start_symbol)):
             self.advance()
-        
+
         end_symbol_length = len(end_symbol)
         while self.current_char is not None:
             if self.current_char == end_symbol[0]:
                 if end_symbol_length == 1:
                     # 单行注释不包括最后的换行
                     result += self.current_char
                     break
-                elif self.peek(end_symbol_length-1) == end_symbol[1:]:
+                elif self.peek(end_symbol_length - 1) == end_symbol[1:]:
                     result += self.current_char
-                    for _ in range(end_symbol_length-1):
+                    for _ in range(end_symbol_length - 1):
                         self.advance()
                         result += self.current_char
                     break
             result += self.current_char
             self.advance()
 
         # 除单行注释外抛异常
         if self.current_char is None and end_symbol != "\n":
             token = Token(TokenType.COMMENT, result, self.line, self.column - 1)
             self.error(ErrorCode.UNTERMINATED_COMMENT, token)
 
-        if end_symbol == '\n':
+        if end_symbol == "\n":
             result = result[:-1]
-            token = Token(TokenType.COMMENT, result, self.line, self.column-1)
+            token = Token(TokenType.COMMENT, result, self.line, self.column - 1)
         else:
             token = Token(TokenType.COMMENT, result, self.line, self.column)
             self.advance()
         return token
 
     def get_long_op(self):
         """
@@ -538,15 +543,15 @@
         for long_op in self.long_op_dict[self.current_char]:
             if self.peek(len(long_op)) == long_op:
                 result = self.current_char + long_op
                 token_type = TokenType(result)
                 for _ in range(len(long_op)):
                     self.advance()
                 break
-        
+
         token = Token(token_type, result, self.line, self.column)
         self.advance()
         return token
 
     def get_next_token(self) -> Token:
         """
         while self.current_char is not None:
```

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/toml_lexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,32 +12,14 @@
     DATE = "DATE"
 
 
 class TomlLexer(Lexer):
     def __init__(self, text: str, LanguageTokenType: Enum = TomlTokenType):
         super().__init__(text, LanguageTokenType)
 
-    def get_id(self):
-        """Handle identifiers and reserved keywords"""
-        value = ""
-        while self.current_char is not None and (
-            self.current_char.isalnum() or self.current_char == "_" or self.current_char == '-'
-        ):
-            value += self.current_char
-            self.advance()
-
-        token_type = self.reserved_keywords.get(value)
-
-        if token_type is None:
-            token = Token(type=TokenType.ID, value=value, line=self.line, column=self.column - 1)
-        else:
-            # reserved keyword
-            token = Token(type=token_type, value=value, line=self.line, column=self.column - 1)
-        return token
-
     def get_next_token(self):
         while self.current_char is not None:
             # TOML 单双引号都可以
             if (
                 self.current_char == TokenType.QUOTO.value
                 or self.current_char == TokenType.APOSTROPHE.value
             ):
@@ -67,15 +49,15 @@
                         result += self.current_char
                         self.advance()
                     return Token(TomlTokenType.DATE, result, self.line, self.column - 1)
                 else:
                     return token
 
             if self.current_char.isalpha():
-                return self.get_id()
+                return self.get_id(extend_chars=['_'])
 
             try:
                 token_type = TokenType(self.current_char)
             except ValueError: # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
```

### Comparing `syntaxlight-0.0.4/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.5/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.4/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.5/syntaxlight/parsers/c_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,27 +20,40 @@
     UnaryOp,
     BinaryOp,
     ConditionalExpression,
     Identifier,
     Constant,
     Expression,
     AssignOp,
-    GlobalDescriptorTable,
     NodeVisitor,
     Char,
     add_ast_type,
     delete_ast_type,
 )
-from typing import List, Union, Optional
+from typing import List, Union
 from enum import Enum
-
+from ..gdt import *
 
 GDT = GlobalDescriptorTable()
 
 
+class C_CSS(Enum):
+    BASE_TYPE = "BaseType"
+    STORAGE_TYPE = "StorageType"
+    TYPE_SPECIFIER = "TypeSpecifier"
+    FUNCTION_TYPE = "FunctionType"
+    STRUCTURE_TYPE = "StructureType"
+    QUALIFY_TYPE = "QualifyType"
+    HEADER_NAME = "HeaderName"
+    ALIGN_SPECIFIER = "AlignSpecifier"
+    ATOMAIC_TYPE_SPECIFIER = "AtomicTypeSpecifier"
+    STRUCTURE_CLASS = "StructureClass"
+    GOTO_LABEL = "GotoLabel"
+
+
 class TranslationUnit(AST):
     def __init__(self, declarations) -> None:
         super().__init__()
         self.declarations = declarations
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.declarations)
@@ -243,15 +256,15 @@
         node_visitor.link(self, self.sub_nodes)
         return super().visit(node_visitor)
 
 
 class PrimaryExpression(AST):
     def __init__(self) -> None:
         super().__init__()
-        self.sub_node = None
+        self.sub_node: Union[Identifier, Constant, Expression, Char, GenericSelection] = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.sub_node)
         return super().visit(node_visitor)
 
 
 class TypeSpecifier(AST):
@@ -419,18 +432,18 @@
         node_visitor.link(self, self.initializer)
         return super().visit(node_visitor)
 
 
 class Designation(AST):
     def __init__(self) -> None:
         super().__init__()
-        self.designator = None
+        self.designators = None
 
     def visit(self, node_visitor: NodeVisitor = None):
-        node_visitor.link(self, self.designator)
+        node_visitor.link(self, self.designators)
         return super().visit(node_visitor)
 
 
 class Designator(AST):
     def __init__(self) -> None:
         super().__init__()
         self.const_expr = None
@@ -530,15 +543,14 @@
         super().__init__()
         self.group_parts = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.group_parts)
         return super().visit(node_visitor)
 
-
 class IfSection(AST):
     def __init__(self) -> None:
         super().__init__()
         self.group = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.group)
@@ -546,15 +558,15 @@
 
 
 class IfGroup(AST):
     def __init__(self) -> None:
         super().__init__()
         self.keyword = None
         self.const_expr = None
-        self.id = None
+        self.id: Identifier = None
         self.group = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.keyword)
         node_visitor.link(self, self.const_expr)
         node_visitor.link(self, self.id)
         node_visitor.link(self, self.group)
@@ -598,22 +610,24 @@
 
 
 class ControlLine(AST):
     def __init__(self) -> None:
         super().__init__()
         self.keyword = None
         self.id: Identifier = None
-        self.paramters = None
+        self.header_name = None
+        self.paramters: List[Identifier] = None
         self.parameterization = None
         self.pp_tokens = None
         self.group = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.keyword)
         node_visitor.link(self, self.id)
+        node_visitor.link(self, self.header_name)
         node_visitor.link(self, self.paramters)
         node_visitor.link(self, self.parameterization)
         node_visitor.link(self, self.pp_tokens)
         node_visitor.link(self, self.group)
         return super().visit(node_visitor)
 
 
@@ -627,17 +641,17 @@
         return super().visit(node_visitor)
 
 
 class PPtoken(AST):
     def __init__(self, value) -> None:
         super().__init__()
         self.value: str = value
-        self.is_bottom_ast = True
+        self.is_leaf_ast = True
         value = self.value.replace("\\", "\\\\").replace('"', '\\"')
-        self._node_info += f"\\n{value}"
+        self.node_info += f"\\n{value}"
 
 
 class CParser(Parser):
     def __init__(self, lexer, skip_invisible_characters=True, skip_space=True):
         super().__init__(lexer, skip_invisible_characters, skip_space)
         self.cfirst_set = CTokenSet()
         self.in_preprocessing = False  # 进入预处理阶段, 影响 after_eat
@@ -649,22 +663,23 @@
             "include",
             "define",
             "undef",
             "line",
             "error",
             "pragma",
         ]
+        self.after_eat()
 
     def parse(self):
-        self.node = self.translation_unit()
+        self.root = self.translation_unit()
         self.skip_crlf()
         if self.current_token.type != TokenType.EOF:
             self.error(error_code=ErrorCode.UNEXPECTED_TOKEN, message="should match EOF")
         GDT.reset()
-        return self.node
+        return self.root
 
     def translation_unit(self):
         """
         <translation-unit> ::= {<external-declaration>}*
         """
         declarations = []
         while self.current_token.type in self.cfirst_set.external_declaration:
@@ -679,76 +694,26 @@
                                  | <statement>
 
         在这里没有办法区分, 需要查看 <declarator> 后面是否有<declaration>* 和 <compound-statement> 才可以确定是 <function-definition>
 
         @扩展文法
         添加 <group> <statement> 以适配宏定义与开头的陈述语句. C 默认不支持 if for 作为陈述语句, 这里添加对于代码段的扩展支持
         """
-        # @修改文法
-        # 当无 <declaration-specifier>* (无类型) 只有 <declarator> 的时候匹配 <function_definition>
+        # function-definition 在 declaration 中被检验和修正
         self._unknown_typedef_id_guess()
-        if self.current_token.type in self.cfirst_set.group:
-            return self.group()
-        elif self.current_token.type in self.cfirst_set.declaration:
+        if self.current_token.type in self.cfirst_set.declaration:
             return self.declaration()
         elif self.current_token.type in self.cfirst_set.statement:
             return self.statement()
         else:  # pragma: no cover
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN,
                 "token type should inside function definition and declaration",
             )
 
-    def function_definition(self):
-        """
-        <function-definition> ::= <declaration-specifier>* <declarator> <declaration>* <compound-statement>
-        """
-        node = Function()
-        declaration_specifiers = []
-        
-        self._unknown_typedef_id_guess()
-        while self.current_token.type in self.cfirst_set.declaration_specifier:
-            declaration_specifiers.append(self.declaration_sepcifier())
-            # @扩展文法
-            # 对于 static clock_t ticks = 10; 判定双 ID 则将前一个 clock_t 置为 TYPEDEF_ID
-            if self.current_token.type == TokenType.ID and self.peek_next_token().type == TokenType.ID:
-                self.current_token.type = CTokenType.TYPEDEF_ID
-                GDT.register_id(self.current_token.value, "Typedefine")
-
-        node.update(declaration_specifiers=declaration_specifiers)
-        declarator = self.declarator()
-        declarations = []
-        while self.current_token.type in self.cfirst_set.declaration:
-            declarations.append(self.declaration())
-
-        # 正常情况
-        if self.current_token.type in self.cfirst_set.compound_statement:
-            node.update(declarator=declarator)
-            node.update(declarations=declarations)
-            node.update(compound_statement=self.compound_statement())
-        elif self.current_token.type in self.cfirst_set.assignment_operator:
-            # @扩展文法
-            # 对于 x += 10 这种外部非初始化的赋值表达式, 从 <function-definition> 转为 <expression>
-            node = Expression()
-            assign_exprs = []
-            assign_expr = AssignmentExpression()
-            assign_expr.update(expr=declarator)
-            assign_expr.update(assign_op=self.assignment_operator())
-            assign_expr.update(assignment_expr=self.assignment_expression())
-            assign_exprs.append(assign_expr)
-            while self.current_token.type == TokenType.COMMA:
-                node.register_token(self.eat(TokenType.COMMA))
-                assign_exprs.append(self.assignment_expression())
-            node.update(exprs=assign_exprs)
-            return node
-
-        add_ast_type(node.declaration_specifiers, "ReturnValue")
-        add_ast_type(node.declarator.direct_declarator.id, "FunctionName")
-        return node
-
     def declaration_sepcifier(self) -> AST:
         """
         <declaration-specifier> ::= <storage-class-specifier>
                                   | <type-specifier>
                                   | <type-qualifier>
                                   | <function-specifier>
                                   | <alignment-specifier>
@@ -767,31 +732,34 @@
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be StorageType or BaseType or QualifyType"
             )
 
         return node
 
     def _unknown_typedef_id_guess(self):
-        '''
+        """
         @扩展文法
         对于 static clock_t ticks = 10; 判定双 ID 则将前一个 clock_t 置为 TYPEDEF_ID
-        '''
-        if self.current_token.type == TokenType.ID and self.peek_next_token().type in (TokenType.ID, TokenType.MUL):
+        """
+        if self.current_token.type == TokenType.ID and self.peek_next_token().type in (
+            TokenType.ID,
+            TokenType.MUL,
+        ):
             self.current_token.type = CTokenType.TYPEDEF_ID
-            GDT.register_id(self.current_token.value, "Typedefine")
+            GDT.register_id(self.current_token.value, CSS.TYPEDEF)
 
     def storage_class_specifier(self):
         """
         <storage-class-specifier> ::= 'auto'
                                     | 'register'
                                     | 'static'
                                     | 'extern'
                                     | 'typedef'
         """
-        return self.keyword(class_name="StorageType")
+        return self.keyword(css_type=C_CSS.STORAGE_TYPE)
 
     def type_specifier(self):
         """
         <type-specifier> ::= void
                            | char
                            | short
                            | int
@@ -816,26 +784,26 @@
         elif self.current_token.type in self.cfirst_set.struct_or_union_specifier:
             node = self.struct_or_union_specifier()
         elif self.current_token.type in self.cfirst_set.enum_specifier:
             node = self.enum_specifier()
         elif self.current_token.type in self.cfirst_set.typedef_name:
             node = self.typedef_name()
         elif self.current_token.type in self.cfirst_set.type_specifier:
-            node = self.keyword(class_name="BaseType")
+            node = self.keyword(css_type=C_CSS.BASE_TYPE)
         else:  # pragma: no cover
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be type specifier")
-        add_ast_type(node, "TypeSpecifier")
+        add_ast_type(node, C_CSS.TYPE_SPECIFIER)
         return node
 
     def function_specifier(self):
         """
         <function-specifier> ::= inline
                                | _Noreturn
         """
-        return self.keyword(class_name="FunctionType")
+        return self.keyword(css_type=C_CSS.FUNCTION_TYPE)
 
     def alignment_specifier(self):
         """
         <alignment-specifier> ::= _Alignas "(" <type-name> ")"
                                 | _Alignas "(" <constant-expression> ")"
         """
         node = TypeSpecifier()
@@ -845,27 +813,27 @@
             node.update(sub_node=self.type_name())
             node.register_token(self.eat(TokenType.RPAREN))
         elif self.current_token.type in self.cfirst_set.constant_expression:
             node.update(sub_node=self.constant_expression())
             node.register_token(self.eat(TokenType.RPAREN))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be type-name or constant-expression")
-        add_ast_type(node, "AlignSpecifier")
+        add_ast_type(node, C_CSS.ALIGN_SPECIFIER)
         return node
 
     def atomic_type_specifier(self):
         """
         <atomic-type-specifier> ::= _Atomic "(" <type-name> ")"
         """
         node = TypeSpecifier()
         node.update(keyword=self.keyword(CTokenType._ATOMIC))
         node.register_token(self.eat(TokenType.LPAREN))
         node.update(sub_node=self.type_name())
         node.register_token(self.eat(TokenType.RPAREN))
-        add_ast_type(node, "AtomicTypeSpecifier")
+        add_ast_type(node, C_CSS.ATOMAIC_TYPE_SPECIFIER)
         return node
 
     def struct_or_union_specifier(self):
         """
         <struct-or-union-specifier> ::= <struct-or-union> <identifier> ("{" {<struct-declaration>}* "}")?
                                       | <struct-or-union>              "{" {<struct-declaration>}* "}"
         """
@@ -893,23 +861,23 @@
                 self._unknown_typedef_id_guess()
             node.update(declarations=struct_declarations)
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
 
             # 匿名 struct 且未定义成员
             if len(struct_declarations) == 0 and node.id is None:
                 self.warning("unnamed struct/union that defines no instances", node)
-        add_ast_type(node.id, "StructClass")
+        add_ast_type(node.id, C_CSS.STRUCTURE_CLASS)
         return node
 
     def struct_or_union(self):
         """
         <struct-or-union> ::= "struct"
                             | "union"
         """
-        return self.keyword(class_name="StructureType")
+        return self.keyword(css_type=C_CSS.STRUCTURE_TYPE)
 
     def struct_declaration(self):
         """
         <struct-declaration> ::= <specifier-qualifier-list> <struct-declarator-list>? ";"
                                | <static_assert-declaration>
         """
         node = StructDeclaration()
@@ -933,25 +901,30 @@
                 result.append(self.type_specifier())
             else:
                 result.append(self.type_qualifier())
         return result
 
     def after_eat(self):
         if self.current_token.type == TokenType.ID and self.current_token.value in GDT:
-            if GDT[self.current_token.value] == "Typedefine":
+            if GDT[self.current_token.value] == CSS.TYPEDEF:
                 self.current_token.type = CTokenType.TYPEDEF_ID
         
         if self.in_preprocessing:
             if self.current_token.type == CTokenType.IF:
                 self.current_token.type = CTokenType.IF_P
             elif self.current_token.type == CTokenType.ELSE:
                 self.current_token.type = CTokenType.ELSE_P
             elif self.current_token.value in self.preprocessing_keywords:
                 self.current_token.type = CTokenType(self.current_token.value)
-
+                
+        elif self.current_token.type == TokenType.HASH:
+            # 多根节点树
+            # TODO: 考虑如何格式化
+            self.group()
+            
 
     def struct_declarator_list(self) -> List[AST]:
         """
         <struct-declarator-list> ::= <struct-declarator> ("," <struct-declarator>)*
         """
         result = [self.struct_declarator()]
         while self.current_token.type == TokenType.COMMA:
@@ -1016,15 +989,15 @@
     def type_qualifier(self):
         """
         <type-qualifier> ::= const
                            | volatile
                            | restrict
                            | _Atomic
         """
-        return self.keyword(class_name="QualifyType")
+        return self.keyword(css_type=C_CSS.QUALIFY_TYPE)
 
     def direct_declaractor(self):
         """
         <direct-declarator> ::= <identifier>
                               | "(" <declarator> ")"
                               | <direct-declarator> "[" <type-qualifier-list>? <assignment-expression>? "]"
                               | <direct-declarator> "[" static <type-qualifier-list>? <assignment-expression> "]"
@@ -1032,14 +1005,18 @@
                               | <direct-declarator> "[" <type-qualifier-list>? "*" "]"
                               | <direct-declarator> "(" <parameter-list> ")"
                               | <direct-declarator> "(" (<identifier-list>)? ")"
         """
         node = DirectDeclaractor()
         if self.current_token.type == TokenType.ID:
             node.update(id=self.identifier())
+            # 对于初始化的变量去掉其 DefineName 的 tag
+            if node.id.id in GDT and GDT[node.id.id] == CSS.MACRO_DEFINE:
+                delete_ast_type(node.id, CSS.MACRO_DEFINE)
+                GDT.delete_id(node.id.id)
         elif (
             self.current_token.type == TokenType.LPAREN
             and self.peek_next_token().type in self.cfirst_set.declarator
         ):
             node.register_token(self.eat(TokenType.LPAREN))
             node.update(declarator=self.declarator())
             node.register_token(self.eat(TokenType.RPAREN))
@@ -1055,45 +1032,46 @@
         sub_nodes = []
         while self.current_token.type in (TokenType.LPAREN, TokenType.LSQUAR_PAREN):
             sub_node = DirectDeclaractorPostfix()
             if self.current_token.type == TokenType.LSQUAR_PAREN:
                 sub_node.register_token(self.eat(TokenType.LSQUAR_PAREN))
 
                 if self.current_token.type == CTokenType.STATIC:
-                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, "StorageType"))
+                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
 
                 if self.current_token.type in self.cfirst_set.type_qualifier:
                     sub_node.update(type_qualifiers=self.type_qualifier_list())
 
                 if self.current_token.type == CTokenType.STATIC:
                     if sub_node.static_head is not None:
                         self.error(ErrorCode.UNEXPECTED_TOKEN, "multi static")
-                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, "StorageType"))
+                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
 
                 if self.current_token.type == TokenType.MUL:
                     self.current_token.type = CTokenType.STAR
                     sub_node.register_token(self.eat(CTokenType.STAR))
                 elif self.current_token.type in self.cfirst_set.assignment_expression:
                     sub_node.update(assignment_expr=self.assignment_expression())
 
                 sub_node.register_token(self.eat(TokenType.RSQUAR_PAREN))
 
             if self.current_token.type == TokenType.LPAREN:
                 # 可以确定是一个函数名
                 if node.id is not None:
                     node.is_function = True
-                    add_ast_type(node, "FunctionName")
-                    GDT.register_id(node.id.id, "FunctionName")
+                    add_ast_type(node, CSS.FUNCTION_NAME)
+                    # TODO
+                    GDT.register_id(node.id.id, CSS.FUNCTION_NAME)
                 else:
                     # 函数指针 "(" <declarator> ")"
-                    add_ast_type(node, "FunctionP")
+                    add_ast_type(node, CSS.FUNCTION_POINTER)
                     _node = node
                     while _node.declarator is not None:
                         _node = _node.declarator.direct_declarator
-                    GDT.register_id(_node.id.id, "FunctionP")
+                    GDT.register_id(_node.id.id, CSS.FUNCTION_POINTER)
 
                 node.register_token(self.eat(TokenType.LPAREN))
                 self._unknown_typedef_id_guess()
                 if self.current_token.type in self.cfirst_set.parameter_list:
                     sub_node.update(parameter_list=self.parameter_list())
                 # elif self.current_token.type == TokenType.ID:
                 #     # @扩展文法
@@ -1407,28 +1385,24 @@
                 sub_nodes.append(self.expression())
                 node.register_token(self.eat(TokenType.RSQUAR_PAREN))
             elif self.current_token.type == TokenType.LPAREN:
                 node.register_token(self.eat(TokenType.LPAREN))
                 # function call
                 # 对于函数指针, 不视为 FunctionCall
                 func_node = node.primary_expr.sub_node
-                if (
-                    type(func_node) == Identifier
-                    and func_node.id in GDT
-                    and GDT[func_node.id] == "FunctionP"
-                ):
+                if type(func_node) == Identifier and GDT[func_node.id] == CSS.FUNCTION_POINTER:
                     pass
                 elif len(sub_nodes) >= 1:
                     # 间接调用不视为 FunctionCall
                     #
                     # person.printInfo = printPersonInfo;
                     # person.printInfo(person.name, person.age);
                     pass
                 else:
-                    add_ast_type(node.primary_expr, "FunctionCall")
+                    add_ast_type(node.primary_expr, CSS.FUNCTION_CALL)
                 if self.current_token.type in self.cfirst_set.assignment_expression:
                     sub_nodes.append(self.assignment_expression())
                     while self.current_token.type == TokenType.COMMA:
                         node.register_token(self.eat(TokenType.COMMA))
                         sub_nodes.append(self.assignment_expression())
                 node.register_token(self.eat(TokenType.RPAREN))
             elif self.current_token.type == TokenType.DOT:
@@ -1460,15 +1434,15 @@
             # @扩展文法
             # Constant 包含了 true, false
             # 该关键字由 C23 引入, 但非常常用, 一般会 define 为 1 和 0, 所以这里引入为 Constant
             sub_node = Constant(self.current_token.value)
             sub_node.register_token(self.eat(self.current_token.type))
         elif self.current_token.type == TokenType.STRING:
             sub_node = self.string()
-        elif self.current_token.type == TokenType.CHAR:
+        elif self.current_token.type == TokenType.CHARACTER:
             sub_node = Char(self.current_token.value)
             sub_node.register_token(self.eat(self.current_token.type))
         elif self.current_token.type == TokenType.LPAREN:
             node.register_token(self.eat(TokenType.LPAREN))
             sub_node = self.expression()
             node.register_token(self.eat(TokenType.RPAREN))
         elif self.current_token.type in self.cfirst_set.generic_selection:
@@ -1536,15 +1510,15 @@
         """
         # <conditional-expression> => <cast-expression> => ("(" <type-name> ")")* <unary-expression>
         # 无法 LL1 判断, 需要额外处理
         if self.current_token.type not in self.cfirst_set.assignment_expression:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be unary expression or conditional expression"
             )
-
+        
         node = AssignmentExpression()
         expr = self.conditional_expression()
         if isinstance(expr.condition_expr, BinaryOp):
             # 含双目运算符, 必为 conditional expression
             node.update(expr=expr)
         elif isinstance(expr.condition_expr, CastExpression):
             # CastExpression 含 type_names 必为 conditional expression
@@ -1659,22 +1633,22 @@
                     self.current_token.type = CTokenType.STAR
                     sub_node.register_token(self.eat(CTokenType.STAR))
                     sub_node.register_token(self.eat(TokenType.RSQUAR_PAREN))
                     sub_nodes.append(sub_node)
                     continue
 
                 if self.current_token.type == CTokenType.STATIC:
-                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, "StorageType"))
+                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
                 if self.current_token.type in self.cfirst_set.type_qualifier:
                     sub_node.update(type_qualifiers=self.type_qualifier_list())
 
                 if self.current_token.type == CTokenType.STATIC:
                     if sub_node.static_head is not None:
                         self.error(ErrorCode.UNEXPECTED_TOKEN, "multi static")
-                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, "StorageType"))
+                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
 
                 if self.current_token.type in self.cfirst_set.assignment_expression:
                     sub_node.update(assignment_expr=self.assignment_expression())
 
                 sub_node.register_token(self.eat(TokenType.RSQUAR_PAREN))
                 sub_nodes.append(sub_node)
 
@@ -1686,15 +1660,17 @@
         <enum-specifier> ::= enum (<identifier>)? "{" <enumerator> ("," <enumerator>)* ","? "}"
                            | enum <identifier>
         """
         node = EnumSpecifier()
         node.update(keyword=self.keyword(CTokenType.ENUM))
         if self.current_token.type in self.cfirst_set.identifier:
             node.update(id=self.identifier())
-            add_ast_type(node.id, "EnumID")
+            delete_ast_type(node.id, CSS.MACRO_DEFINE)
+            add_ast_type(node.id, CSS.ENUM_ID)
+            GDT.register_id(node.id.id, CSS.ENUM_ID)
         if self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
             enumerators = [self.enumerator()]
             while self.current_token.type == TokenType.COMMA:
                 node.register_token(self.eat(TokenType.COMMA))
                 if self.current_token.type == TokenType.RCURLY_BRACE:
                     break
@@ -1706,25 +1682,26 @@
 
     def enumerator(self):
         """
         <enumerator> ::= <identifier> ("=" <constant-expression>)?
         """
         node = Enumerator()
         node.update(id=self.identifier())
-        GDT.register_id(node.id.id, "Enumerator")
+        add_ast_type(node.id, CSS.ENUMERATOR)
+        GDT.register_id(node.id.id, CSS.ENUMERATOR)
         if self.current_token.type == TokenType.ASSIGN:
             node.register_token(self.eat(TokenType.ASSIGN))
             node.update(const_expr=self.constant_expression())
         return node
 
     def typedef_name(self):
         """
         <typedef-name> ::= <identifier>
         """
-        node = self.keyword(CTokenType.TYPEDEF_ID, class_name="Typedefine")
+        node = self.keyword(CTokenType.TYPEDEF_ID, css_type=CSS.TYPEDEF)
         return node
 
     def declaration(self):
         """
         <declaration> ::= <declaration-specifier>+ (<init-declarator-list>)? ";"
                         | <static-assert-declaration>
 
@@ -1735,37 +1712,37 @@
         node = Declaration()
         if self.current_token.type in self.cfirst_set.static_assert_declaration:
             node.update(static_assert=self.static_assert_declaration())
             return node
 
         declaration_specifiers: List[AST] = [self.declaration_sepcifier()]
         self._unknown_typedef_id_guess()
-            
+
         while self.current_token.type in self.cfirst_set.declaration_specifier:
             declaration_specifiers.append(self.declaration_sepcifier())
             self._unknown_typedef_id_guess()
 
         if self.current_token.type in self.cfirst_set.init_declarator_list:
             init_declarator_list = self.init_declarator_list()
             if self.current_token.type == TokenType.SEMI:
                 node.update(declaration_specifiers=declaration_specifiers)
                 node.update(init_declarator_list=init_declarator_list)
                 node.register_token(self.eat(TokenType.SEMI))
                 if self._is_C_function(init_declarator_list):
-                    add_ast_type(declaration_specifiers, "ReturnValue")
+                    add_ast_type(declaration_specifiers, CSS.FUNCTION_RETURN_TYPE)
                 # @扩展文法
                 # 对于 typedef 重命名的符号, 加入 GDT 中
                 if (
                     type(node.declaration_specifiers[0]) == Keyword
                     and node.declaration_specifiers[0].name == "typedef"
                 ):
                     for init_declarator in node.init_declarator_list:
-                        add_ast_type(init_declarator.declarator.direct_declarator.id, "Typedefine")
+                        add_ast_type(init_declarator.declarator.direct_declarator.id, CSS.TYPEDEF)
                         GDT.register_id(
-                            init_declarator.declarator.direct_declarator.id.id, "Typedefine"
+                            init_declarator.declarator.direct_declarator.id.id, CSS.TYPEDEF
                         )
 
                 return node
             elif self._is_C_function(init_declarator_list) and (
                 self.current_token.type in self.cfirst_set.compound_statement
                 or self.current_token.type in self.cfirst_set.declaration
             ):
@@ -1816,19 +1793,19 @@
         # }
         declarations = []
         while self.current_token.type in self.cfirst_set.declaration:
             declarations.append(self.declaration())
         node.update(declarations=declarations)
         node.update(compound_statement=self.compound_statement())
 
-        add_ast_type(node.declaration_specifiers, "ReturnValue")
-        add_ast_type(node.declarator.declarator.direct_declarator.id, "FunctionName")
+        add_ast_type(node.declaration_specifiers, CSS.FUNCTION_RETURN_TYPE)
+        add_ast_type(node.declarator.declarator.direct_declarator.id, CSS.FUNCTION_NAME)
         # 对于含 <declaration> 的情况取消其参数的 Typedefine
         if len(node.declarations) != 0:
-            delete_ast_type(node.declarator, "Typedefine")
+            delete_ast_type(node.declarator, CSS.TYPEDEF)
         return node
 
     def init_declarator_list(self) -> List[InitDeclarator]:
         """
         <init-declarator-list> ::= <init-declarator> ("," <init-declarator>)*
         """
         result = [self.init_declarator()]
@@ -1855,50 +1832,61 @@
                         | "{" <initializer-list> "," "}"
         """
         node = Initializer()
         if self.current_token.type in self.cfirst_set.assignment_expression:
             node.update(assignment_expr=self.assignment_expression())
         elif self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
-            node.update(initializer_list=self.initializer_list())
+            if self.current_token.type in self.cfirst_set.initializer_list:
+                node.update(initializer_list=self.initializer_list())
+                
             if self.current_token.type == TokenType.COMMA:
                 node.register_token(self.eat(TokenType.COMMA))
+                
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
         else:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be initializer list or assignment expression"
             )
         return node
 
     def initializer_list(self) -> List[AST]:
         """
         <initializer-list> ::= <designation>? <initializer> ("," <designation>? <initializer>)*
         """
         node = DesignationInitializer()
         if self.current_token.type in self.cfirst_set.designation:
             node.update(designation=self.designation())
+        
         node.update(initializer=self.initializer())
-
         result = [node]
-
         while self.current_token.type == TokenType.COMMA:
+            next_token_type = self.peek_next_token().type
+            if (
+                next_token_type not in self.cfirst_set.designation
+                and next_token_type not in self.cfirst_set.initializer
+            ):
+                break
             self.eat(TokenType.COMMA)
             node = DesignationInitializer()
             if self.current_token.type in self.cfirst_set.designation:
                 node.update(designation=self.designation())
             node.update(initializer=self.initializer())
             result.append(node)
         return result
 
     def designation(self):
         """
         <designation> ::= <designator>+ "="
         """
         node = Designation()
-        node.update(designator=self.designator())
+        designators = [self.designator()]
+        while self.current_token.type in self.cfirst_set.designator:
+            designators.append(self.designator())
+        node.update(designators=designators)
         node.register_token(self.eat(TokenType.ASSIGN))
         return node
 
     def designator(self):
         """
         <designator> ::= "[" <constant-expression> "]"
                        | "." <identifier>
@@ -1917,40 +1905,25 @@
 
     def compound_statement(self):
         """
         <compound-statement> ::= "{" (<block-item>)* "}"
 
         <block-item> ::= <declaration>
                        | <statement>
-                       | <group>
         """
         node = CompoundStatement()
         node.register_token(self.eat(TokenType.LCURLY_BRACE))
         sub_nodes = []
         self._unknown_typedef_id_guess()
         while self.current_token.type in self.cfirst_set.block_item:
             if self.current_token.type in self.cfirst_set.declaration:
                 sub_nodes.append(self.declaration())
-            elif (
-                self.current_token.type == TokenType.ID
-                and self.peek_next_token().type == TokenType.ID
-            ):
-                # @扩展文法
-                # 对于未声明类但直接使用的情况, 判断一下后面仍然是一个 ID 或者是 <declaration_specifier>
-                # 继续选择 declaration
-                # int main() {
-                #     Person person = { "Alice", 25, { 30, 40 } };
-                # }
-                self.current_token.type = CTokenType.TYPEDEF_ID
-                sub_nodes.append(self.declaration())
             elif self.current_token.type in self.cfirst_set.statement:
                 sub_nodes.append(self.statement())
-            else:
-                # group
-                sub_nodes.append(self.group())
+            self._unknown_typedef_id_guess()
         node.update(sub_nodes=sub_nodes)
         node.register_token(self.eat(TokenType.RCURLY_BRACE))
         return node
 
     def statement(self):
         """
         <statement> ::= <labeled-statement>
@@ -1992,16 +1965,16 @@
                               | default ":" <statement>
         """
         node = LabeledStatement()
 
         if self.current_token.type in self.cfirst_set.identifier:
             node.update(id=self.identifier())
             # goto 的标签
-            add_ast_type(node.id, "GotoLabel")
-            GDT.register_id(node.id.id, "GotoLabel")
+            add_ast_type(node.id, C_CSS.GOTO_LABEL)
+            GDT.register_id(node.id.id, C_CSS.GOTO_LABEL)
         elif self.current_token.type == CTokenType.CASE:
             node.update(keyword=self.keyword(CTokenType.CASE))
             node.update(const_expr=self.constant_expression())
         elif self.current_token.type == CTokenType.DEFAULT:
             node.update(keyword=self.keyword(CTokenType.DEFAULT))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be id or case or default")
@@ -2101,90 +2074,93 @@
                            | return {<expression>}? ";"
         """
         node = JumpStatement()
         if self.current_token.type in self.cfirst_set.jump_statement:
             if self.current_token.type == CTokenType.GOTO:
                 node.update(keyword=self.keyword())
                 node.update(expr=self.identifier())
-                add_ast_type(node.expr, "GotoLabel")
+                add_ast_type(node.expr, C_CSS.GOTO_LABEL)
             elif self.current_token.type == CTokenType.RETURN:
                 node.update(keyword=self.keyword())
                 if self.current_token.type in self.cfirst_set.expression:
                     node.update(expr=self.expression())
             else:
                 node.update(keyword=self.keyword())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be goto continue break return")
         node.register_token(self.eat(TokenType.SEMI))
         return node
 
     def identifier(self):
         """
-        id
+        <ID>
         """
         node = Identifier(self.current_token.value)
         token_value = self.current_token.value
         node.register_token(self.eat(TokenType.ID))
 
         # 判断一下 ID 的 class_name
         if token_value in GDT:
             add_ast_type(node, GDT[token_value])
         elif bool(re.match(r"^[A-Z0-9_]+$", token_value)):
             # ID 全部为 大写/数字/下划线, 很可能为宏
-            add_ast_type(node, "DefineName")
+            add_ast_type(node, CSS.MACRO_DEFINE)
+            GDT.register_id(node.id, CSS.MACRO_DEFINE)
 
         return node
 
-    def keyword(self, token_type: Enum = None, class_name: str = None):
+    def keyword(self, token_type: Enum = None, css_type: Enum = None):
         """
         keyword
 
         @token_type: keyword 的类型,默认为 current_token.type
         @class_name: 修改 Keyword 的类名
         """
         keyword = Keyword(self.current_token.value)
         if token_type:
             keyword.register_token(self.eat(token_type))
         else:
             keyword.register_token(self.eat())
-        if class_name is not None:
-            add_ast_type(keyword, class_name)
+        if css_type is not None:
+            add_ast_type(keyword, css_type)
         return keyword
 
     def string(self):
         """
         string
         """
         return self._string_inside_format(self.current_token)
 
     def _string_inside_format(self, token: Token):
         """
         取出其中格式化字符 %d %x \n 并新建 token
         """
-        pattern = r"(%[0-9diufFeEgGxXoscpaAn]+|(?:\\\\|\\n|\\t|\\v|\\f))"
+        pattern = r"(%[0-9ldiufFeEgGxXoscpaAn]+|(?:\\\\|\\n|\\t|\\v|\\f))"
         sub_strings = re.split(pattern, token.value)
         new_asts = []
         line = token.line
         column = token.column - len(token.value)
         for sub_string in sub_strings:
             if len(sub_string) == 0:
                 continue
             column += len(sub_string)
             token = Token(TokenType.STRING, sub_string, line, column)
-            if bool(re.match(r"%[0-9diufFeEgGxXoscpaAn]+", sub_string)):
+            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAn]+", sub_string)):
                 token.class_list.add("Format")
             elif sub_string in ["\\n", "\\t", "\\f", "\\v", "\\a", "\\b", "\\\\"]:
                 token.class_list.add("Control")
 
             self._register_token(token)
             node = String(token.value)
             node.register_token([token])
             new_asts.append(node)
 
         self.current_token = self.lexer.get_next_token()
+        self._skip()
+        self.after_eat()
         return new_asts
 
     def static_assert_declaration(self):
         """
         <static_assert-declaration> ::= _Static_assert "(" <constant-expression> "," <string> ")"
         """
         node = StaticAssertDeclaration()
@@ -2202,14 +2178,17 @@
         node = Group()
         group_parts = []
         while self.current_token.type == TokenType.HASH:
             self._begin_preprocessing()
             group_parts.append(self.group_part())
         node.update(group_parts=group_parts)
         self._end_preprocessing()
+
+        # 添加至 sub_roots
+        self.sub_roots.append(node)
         return node
 
     def _begin_preprocessing(self):
         """
         开始预处理
         """
         # 考虑换行
@@ -2271,77 +2250,72 @@
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "preprocess keyword error")
         node.update(group=group)
         return node
 
     def if_group(self):
         """
-        <if-group> ::= "#" if <constant-expression> <CRLF> <group>?
-                     | "#" ifdef <identifier> <CRLF> <group>?
-                     | "#" ifndef <identifier> <CRLF> <group>?
+        <if-group> ::= "#" if <constant-expression> <CRLF>
+                     | "#" ifdef <identifier> <CRLF
+                     | "#" ifndef <identifier> <CRLF>
         """
         self.eat(TokenType.HASH)
         node = IfGroup()
         if self.current_token.type == CTokenType.IF_P:
-            node.update(keyword=self.keyword(CTokenType.IF_P, "Preprocess"))
+            node.update(keyword=self.keyword(CTokenType.IF_P, CSS.PREPROCESS))
             node.update(const_expr=self.constant_expression())
         elif self.current_token.type in (CTokenType.IFDEF, CTokenType.IFNDEF):
-            node.update(keyword=self.keyword(class_name="Preprocess"))
+            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
+            add_ast_type(node.id, CSS.MACRO_DEFINE)
+            GDT.register_id(node.id.id, CSS.MACRO_DEFINE)
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be if ifdef ifndef")
-        add_ast_type(node.id, "DefineName")
         self.eat_lf()
         self._end_preprocessing()
-        if self.current_token.type in self.cfirst_set.external_declaration:
-            node.update(group=self.external_declaration())
         return node
 
     def elif_group(self):
         """
-        <elif-group> ::= "#" elif <constant-expression> <CRLF> <group>?
+        <elif-group> ::= "#" elif <constant-expression> <CRLF>
         """
         self.eat(TokenType.HASH)
         node = ElifGroup()
-        node.update(keyword=self.keyword(CTokenType.ELIF, class_name="Preprocess"))
+        node.update(keyword=self.keyword(CTokenType.ELIF, css_type=CSS.PREPROCESS))
         node.update(const_expr=self.constant_expression())
         self.eat_lf()
         self._end_preprocessing()
-        if self.current_token.type in self.cfirst_set.external_declaration:
-            node.update(group=self.external_declaration())
         return node
 
     def else_group(self):
         """
-        <else-group> ::= "#" else <CRLF> <group>?
+        <else-group> ::= "#" else <CRLF>
         """
         self.eat(TokenType.HASH)
         node = ElseGroup()
         if self.current_token.type == CTokenType.ELSE:
             self.current_token.type == CTokenType.ELSE_P
-            node.update(keyword=self.keyword(CTokenType.ELSE_P, class_name="Preprocess"))
+            node.update(keyword=self.keyword(CTokenType.ELSE_P, css_type=CSS.PREPROCESS))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be else")
         self.eat_lf()
         self._end_preprocessing()
-        if self.current_token.type in self.cfirst_set.external_declaration:
-            node.update(group=self.external_declaration())
         return node
 
     def endif_line(self):
         """
         <endif-line> ::= "#" endif <CRLF>
         """
         self.eat(TokenType.HASH)
         node = EndifLine()
-        node.update(keyword=self.keyword(CTokenType.ENDIF, class_name="Preprocess"))
+        node.update(keyword=self.keyword(CTokenType.ENDIF, css_type=CSS.PREPROCESS))
         self.eat_lf()
         self._end_preprocessing()
-        if self.current_token.type in self.cfirst_set.external_declaration:
-            node.update(group=self.external_declaration())
+        # if self.current_token.type in self.cfirst_set.external_declaration:
+        #     node.update(group=self.external_declaration())
         return node
 
     def control_line(self):
         """
         <control-line> ::= "#" include <header-name> <CRLF>
                          | "#" define <identfier> <pp-token>* <CRLF>
                          | "#" define <identifier> "(" <identifier-list>? ")" <pp-token>* <CRLF>
@@ -2350,26 +2324,34 @@
                          | "#" undef <identifier> <CRLF>
                          | "#" line <pp-token>+ <CRLF>
                          | "#" error <pp-token>* <CRLF>
                          | "#" pragma <pp-token>* <CRLF>
                          | "#" <CRLF>
 
         <pp-token> ::= any
-
-        括号要求前面无空格, 不过这里不做处理
         """
         self.eat(TokenType.HASH)
         node = ControlLine()
         if self.current_token.type == CTokenType.INCLUDE:
-            node.update(keyword=self.keyword(class_name="Preprocess"))
+            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
             node.update(header_name=self.header_name())
         elif self.current_token.type == CTokenType.DEFINE:
-            node.update(keyword=self.keyword(class_name="Preprocess"))
+            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            # define 这里需要考虑空格的影响, 作为函数括号要求前面无空格
+            # define A(a,b) 1
+            # define A (a,b)
+            #
+            # 这里禁用skip_space和skip_invisible_characters以单步匹配下一个 token
+            self.skip_space = False
+            self.skip_invisible_characters = False
             node.update(id=self.identifier())
+            self.skip_invisible_characters = True
+            self.skip_space = True
             if self.current_token.type == TokenType.LPAREN:
+                # paramters 或 parameterization 被定义了说明是函数
                 node.register_token(self.eat(TokenType.LPAREN))
                 if self.current_token.type in self.cfirst_set.identifier_list:
                     node.update(paramters=self.identifier_list())
                 if self.current_token.type == TokenType.COMMA:
                     node.register_token(self.eat())
                 if self.current_token.type == TokenType.VARARGS:
                     node.update(parameterization=self.keyword(TokenType.VARARGS))
@@ -2379,34 +2361,44 @@
             while self.current_token.type not in (TokenType.EOF, TokenType.LF):
                 if self.current_token.type == TokenType.BACK_SLASH:
                     pp_tokens.append(self.pp_token())
                 pp_tokens.append(self.pp_token())
             node.update(pp_tokens=pp_tokens)
 
         elif self.current_token.type == CTokenType.UNDEF:
-            node.update(keyword=self.keyword(class_name="Preprocess"))
+            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
         elif self.current_token.type in (CTokenType.LINE, CTokenType.ERROR, CTokenType.PRAGMA):
-            node.update(keyword=self.keyword(class_name="Preprocess"))
+            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
 
         if node.id is not None:
-            add_ast_type(node.id, "DefineName")
-            GDT.register_id(node.id.id, "DefineName")
+            if node.paramters is not None:
+                # paramters 被定义了说明是函数
+                # TODO: parameterization
+                add_ast_type(node.id, CSS.MACRO_FUNCTION)
+                arguments = []
+                for i_node in node.paramters:
+                    arguments.append(Argument(name=i_node.id, type=None))
+                GDT.register_function(node.id.id, arguments, (), CSS.MACRO_FUNCTION)
+            else:
+                # 常规宏定义变量
+                add_ast_type(node.id, CSS.MACRO_DEFINE)
+                GDT.register_id(node.id.id, CSS.MACRO_DEFINE)
+
         self.eat_lf()
         self._end_preprocessing()
-        if self.current_token.type in self.cfirst_set.external_declaration:
-            node.update(group=self.external_declaration())
+        # if self.current_token.type in self.cfirst_set.external_declaration:
+        #     node.update(group=self.external_declaration())
         return node
 
     def pp_token(self):
         """
         any
         """
-
         if self.current_token.type == TokenType.LANGLE_BRACE:
             self.current_token.type = TokenType.LT
         elif self.current_token.type == TokenType.RANGLE_BRACE:
             self.current_token.type = TokenType.GT
 
         if self.current_token.type == TokenType.ID:
             return self.identifier()
@@ -2424,27 +2416,29 @@
         any member of the source character set except the new-line character and >
 
         <string>
         """
         node = HeaderName()
         if self.current_token.type == TokenType.STRING:
             node.update(file_path=self.string())
-            add_ast_type(node.file_path, "HeaderName")
+            add_ast_type(node.file_path, C_CSS.HEADER_NAME)
         elif self.current_token.type == TokenType.LANGLE_BRACE:
             node.register_token(self.eat(TokenType.LANGLE_BRACE))
             result = ""
             line = -1
             column = -1
             while self.current_token.type != TokenType.RANGLE_BRACE:
                 if self.current_token.type in (TokenType.EOF, TokenType.LF):
                     break
                 result += self.current_token.value
                 line = self.current_token.line
                 column = self.current_token.column
                 self.current_token = self.lexer.get_next_token()
+                self._skip()
+                self.after_eat()
             if self.current_token.type == TokenType.EOF:
                 self.error(ErrorCode.UNEXPECTED_TOKEN, "miss >")
             if self.current_token.type == TokenType.LF:
                 self.error(ErrorCode.UNEXPECTED_TOKEN, "\\n inside include <>")
 
             new_token = Token(TokenType.STRING, result, line, column)
             file_path = String(new_token.value)
```

### Comparing `syntaxlight-0.0.4/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.5/syntaxlight/parsers/json_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
             TokenType.LCURLY_BRACE,
             JsonTokenType.TRUE,
             JsonTokenType.FALSE,
             JsonTokenType.NULL,
         ]
 
     def parse(self):
-        self.node = self.json()
+        self.root = self.json()
         if self.current_token.type != TokenType.EOF:
             self.error(error_code=ErrorCode.UNEXPECTED_TOKEN, message="should match EOF")
         # print(self.node)
-        return self.node
+        return self.root
 
     def json(self):
         """
         <Json> ::= <Object>
                  | <Array>
         """
         if self.current_token.type == TokenType.LCURLY_BRACE:
@@ -80,42 +80,42 @@
         elements = []
         if self.current_token.type in self.value_first_set:
             elements.append(self.value())
             while self.current_token.type == TokenType.COMMA:
                 comma = self.current_token
                 node.register_token(self.eat(TokenType.COMMA))
                 if self.current_token.type == TokenType.RSQUAR_PAREN:
-                    self.error(ErrorCode.TRAILING_COMMA, token= comma,message= TokenType.COMMA.value)
+                    self.error(ErrorCode.TRAILING_COMMA, token=comma, message=TokenType.COMMA.value)
                 elements.append(self.value())
 
             if self.current_token.type != TokenType.RSQUAR_PAREN:
-                self.error(ErrorCode.MISS_EXPECTED_TOKEN,message= TokenType.COMMA.value)
+                self.error(ErrorCode.MISS_EXPECTED_TOKEN, message=TokenType.COMMA.value)
 
         node.update(elements=elements)
         node.register_token(self.eat(TokenType.RSQUAR_PAREN))
         return node
 
     def pair(self):
         """
-        <Pair> ::= String ':' <Value>
+        <Pair> ::= <STRING> ':' <Value>
         """
         node = Pair()
 
         key = String(self.current_token.value)
-        key.register_token(self.eat(TokenType.STRING), 'Key')
-        
-        node.update(key = key)
+        key.register_token(self.eat(TokenType.STRING), "Key")
+
+        node.update(key=key)
         node.register_token(self.eat(TokenType.COLON))
         node.update(value=self.value())
         return node
 
     def value(self):
         """
-        <Value> ::= String
-                  | Number
+        <Value> ::= <STRING>
+                  | '-'? <NUMBER>
                   | <Object>
                   | <Array>
                   | true
                   | false
                   | null
         """
         # print(self.current_token.type)
```

### Comparing `syntaxlight-0.0.4/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.5/syntaxlight/parsers/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ..error import ParserError, ErrorCode
 from enum import Enum
 from ..ast import AST
 from typing import List
 import sys
 import html
 import traceback
+import copy
 
 DEBUG = False
 DEBUG = True
 
 
 class Parser:
     def __init__(
@@ -28,15 +29,17 @@
             TokenType.RSQUAR_PAREN,
             TokenType.LCURLY_BRACE,
             TokenType.RCURLY_BRACE,
             TokenType.LANGLE_BRACE,
             TokenType.RANGLE_BRACE,
         ]
         self.brace_max_depth = 3  # 深度循环轮次
-        self.node: AST = None
+        self.root: AST = None  # 主根节点
+        self.sub_roots: List[AST] = []  # 其他根节点, 例如预处理命令
+        self._status_stack = []  # 状态栈
         self.current_token: Token = self.lexer.get_next_token()
         self._skip()
 
     def error(
         self,
         error_code: ErrorCode,
         message: str = "",
@@ -74,41 +77,47 @@
 
     def _log_trace(self):
         """
         查看 python 函数调用栈
         """
         if DEBUG:
             stack_trace = traceback.extract_stack()
+            function_length = 0
+            line_length = 0
+            for stack in stack_trace:
+                _, line_number, function_name, _ = stack
+                function_length = max(function_length, len(function_name))
+                line_length = max(line_length, len(str(line_number)))
             for stack in stack_trace:
                 _, line_number, function_name, line_of_code = stack
-                print(f"[{function_name:<25}][{line_number}]: {line_of_code.strip()}")
-    def after_eat(self):
-        """
-        eat 之后对于 current_token 的一些操作
-        """
-        return
+                print(
+                    f"[{function_name:>{function_length}}][{line_number:<{line_length}}]: {line_of_code.strip()}"
+                )
 
     def eat(self, token_type: Enum = None) -> List[Token]:
         """
         匹配一个 token_type 类型的 token, 并获取下一个 token 更新 current_token
 
         token_type 默认值为 None, 表示匹配当前 current_token.type
         """
-        # print(self.current_token)
+        # print(token_type, self.current_token)
         # self._log_trace()
         # if DEBUG:
         #     import inspect
         #     frame = inspect.currentframe().f_back
         #     lineno = frame.f_lineno
         #     print(f"The 'eat' method was called from line {lineno}.")
         tokens = [self.current_token]
         if token_type is None or self.current_token.type == token_type:
             self._register_token()
             self.current_token = self.lexer.get_next_token()
             tokens.extend(self._skip())
+            self.after_eat()
+            return tokens
+
         else:
             current_value = self.current_token.value
             expected_value = token_type.value
             if current_value in self.lexer.invisible_characters:
                 current_value = self.current_token.type.name
             if self.current_token.type == TokenType.EOF:
                 current_value = "EOF"
@@ -116,20 +125,27 @@
                 expected_value = token_type.name
             self.error(
                 error_code=ErrorCode.UNEXPECTED_TOKEN,
                 token=self.current_token,
                 message=f"should match {expected_value} but got {current_value}",
             )
 
-        self.after_eat()
-        return tokens
+    def after_eat(self):
+        """
+        eat 之后对于 current_token 的一些操作
+        """
+        return
 
     def _skip(self) -> List[Token]:
+        """
+        跳过不可见字符和空格
+
+        由 self.skip_invisible_characters 与 self.skip_space 控制
+        """
         tokens = []
-        # 跳过不可见字符和空格
         if self.skip_invisible_characters and self.skip_space:
             while (
                 self.current_token.value in self.lexer.invisible_characters
                 or self.current_token.type == TokenType.SPACE
             ):
                 self._register_token()
                 tokens.append(self.current_token)
@@ -168,37 +184,40 @@
         跳过最后的空白和换行
         """
         while self.current_token.type != TokenType.EOF:
             self._skip()
 
     def eat_lf(self):
         """
-        跳过一个换行
+        跳过一个换行, 如果是结尾 EOF 则不跳过
         """
         if self.current_token.type == TokenType.CR:
             self.eat(self.current_token.type)
         if self.current_token.type == TokenType.EOF:
             return
         self.eat(TokenType.LF)
         self.skip_crlf()
 
     def peek_next_token(self) -> Token:
         """
         查看下一个 token 的类型
         """
+        # 保存程序状态
         self.lexer._record()
         token_list_length = len(self._token_list)
+        sub_roots_length = len(self.sub_roots)
         current_token = self.current_token
 
-        self.eat(self.current_token.type)
+        self.eat()
         next_token = self.current_token
 
+        self.lexer._reset()
         self._token_list = self._token_list[:token_list_length]
+        self.sub_roots = self.sub_roots[:sub_roots_length]
         self.current_token = current_token
-        self.lexer._reset()
         return next_token
 
     def _register_token(self, token=None):
         """
         将一个 token 注册到 token_list 当中
 
         每一个 token 都需要间接的执行此过程, 以便最终恢复高亮文本信息
```

### Comparing `syntaxlight-0.0.4/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.5/syntaxlight/parsers/toml_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,19 +138,19 @@
             TomlTokenType.FALSE,
             TokenType.LSQUAR_PAREN,
             TokenType.LCURLY_BRACE,
         ]
         self.path_first_set = [TokenType.ID, TokenType.STR]
 
     def parse(self):
-        self.node = self.toml()
+        self.root = self.toml()
         if self.current_token.type != TokenType.EOF:
             self.error(ErrorCode.UNEXPECTED_TOKEN)
         # print(self.node)
-        return self.node
+        return self.root
 
     def toml(self):
         """
         <toml> ::= <expression> ( <CRLF> expression )*
         """
         expressions = []
         self.skip_crlf()
@@ -186,15 +186,15 @@
         node.register_token(self.eat(TokenType.ASSIGN))
         value = self.value()
         node.update(value=value)
         return node
 
     def path(self):
         """
-        <path> ::= (<ID> | <str>) ('.' (<ID> | <str>)) *
+        <path> ::= (<ID> | <STRING>) ( '.' (<ID> | <STRING>)) *
         """
         if self.current_token.type not in self.path_first_set:  # pragma: no cover
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be ID or str")
 
         node = Path()
         path = self.current_token.value
         node.register_token(self.eat(self.current_token.type))
@@ -244,28 +244,28 @@
         self.eat_lf()
         entries = self.table_entry()
         node.update(entries=entries)
         return node
 
     def table_entry(self):
         """
-        <table_entry> ::= ( <pair> )*
+        <table_entry> ::= (<pair>)? ( <CRLF> <pair> )*
         """
         pairs = []
         accepted_token_types = [TokenType.ID, TokenType.STR]
         while self.current_token.type in accepted_token_types:
             pairs.append(self.pair())
             self.eat_lf()
             self.skip_crlf()
 
         return TableEntry(pairs)
 
     def value(self):
         """
-        <value> ::= <str> | <number> | <date> | 'true' | 'false' | <array> | <inline_table>
+        <value> ::= <STRING> | <NUMBER> | <DATE> | true | false | <array> | <inline_table>
         """
 
         if self.current_token.type not in self.value_first_set:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN,
                 f"should be a value",
             )
@@ -286,15 +286,15 @@
                 number.register_token(self.eat(TokenType.NUMBER))
             else:
                 self.error(ErrorCode.UNEXPECTED_TOKEN, f"should match number")
             node.update(expr=number)
 
         elif self.current_token.type == TomlTokenType.DATE:
             node = Number(self.current_token.value)
-            node.register_token(self.eat(TomlTokenType.DATE),'Date')
+            node.register_token(self.eat(TomlTokenType.DATE), "Date")
 
         elif self.current_token.type in (TomlTokenType.TRUE, TomlTokenType.FALSE):
             node = Keyword(self.current_token.value)
             node.register_token(self.eat(self.current_token.type))
 
         elif self.current_token.type == TokenType.LSQUAR_PAREN:
             node = self.array()
```

### Comparing `syntaxlight-0.0.4/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.5/syntaxlight/parsers/xml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,26 +77,26 @@
 class XmlParser(Parser):
     def __init__(
         self, lexer, skip_invisible_characters=True, skip_space=True, display_warning=True
     ):
         super().__init__(lexer, skip_invisible_characters, skip_space, display_warning)
 
     def parse(self):
-        self.node = self.XML()
+        self.root = self.XML()
         if self.current_token.type == XmlTokenType.CONTENT:
             eat_flag = True
             for char in self.current_token.value:
-                if char not in self.lexer.invisible_characters or char != ' ':
+                if char not in self.lexer.invisible_characters or char != " ":
                     eat_flag = False
                     break
             if eat_flag:
                 self.eat(self.current_token.type)
         if self.current_token.type != TokenType.EOF:
             self.error(error_code=ErrorCode.UNEXPECTED_TOKEN, message="should match EOF")
-        return self.node
+        return self.root
 
     def XML(self):
         """
         <XML> ::= (<prolog>)? (<element>)?
         """
         node = XML()
         if self.current_token.type == XmlTokenType.PROLOG_START:
```

### Comparing `syntaxlight-0.0.4/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.5/syntaxlight/syntax_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from .lexers import *
 from .error import Error
 from .parsers import *
 from .ast import display_ast
 import sys
 
 
-def parse(text: str, language: str = "guess", file_path=None, show_error_context=True, save_ast_tree = False) -> str:
+def parse(
+    text: str, language: str = "guess", file_path=None, show_error_context=True, save_ast_tree=False
+) -> str:
     assert type(text) == str
     assert type(language) == str
 
     if len(text) == 0:
         return ""
 
     language = language.lower()
@@ -22,15 +24,15 @@
     try:
         parser.parse()
     except Error as e:
         sys.stderr.write(e.message)
         if show_error_context:
             sys.stderr.write(e.context)
     else:
-        display_ast(parser.node, save_ast_tree = save_ast_tree)
+        display_ast(parser.root,parser.sub_roots, save_ast_tree=save_ast_tree)
         # print(parser.node)
         return parser.to_html()
 
 
 def parse_file(
     file_path: str, language: str = "guess", show_error_context=True, save_ast_tree=False
 ) -> str:
@@ -52,17 +54,17 @@
         file_path=file_path,
         show_error_context=show_error_context,
         save_ast_tree=save_ast_tree,
     )
 
 
 def guess_language(file_path: str) -> str:
-    '''
+    """
     通过文件名猜测文法类型
-    '''
+    """
     file_name = file_path.split(os.sep)[-1]
 
     languages = {
         "json": ["json"],
         "c": ["c", "h"],
         "lua": ["lua"],
         "bnf": ["bnf"],
@@ -71,14 +73,15 @@
         "rust": ["rs"],
         "javascript": ["js"],
         "typescript": ["ts", "tsx", "tsc"],
         "pascal": ["pas"],
         "toml": ["toml"],
         "xml": ["xml"],
         "shell": ["sh"],
+        "bnf": ["bnf"],
     }
 
     if "." in file_name:
         suffix = file_name.split(".")[-1]
         for language, suffix_names in languages.items():
             if suffix in suffix_names:
                 return language
@@ -110,18 +113,18 @@
 def get_lexer(code: str, language: str) -> Lexer:
     language = language.lower()
 
     lexers = {
         "c": CLexer,
         "lua": LuaLexer,
         "json": JsonLexer,
-        "ebnf": EBNFLexer,
         "toml": TomlLexer,
         "xml": XmlLexer,
         "shell": ShellLexer,
+        "bnf": BNFLexer,
     }
 
     lexer_class = lexers.get(language, None)
     if lexer_class is None:
         print("unknown language type: ", language)
         exit(1)
 
@@ -131,14 +134,15 @@
 def get_parser(lexer: Lexer) -> Parser:
     parsers = {
         "json": JsonParser,
         "toml": TomlParser,
         "c": CParser,
         "xml": XmlParser,
         "shell": ShellParser,
+        "bnf": BNFParser,
     }
 
     syntax_type = lexer.__class__.__name__.replace("Lexer", "").lower()
     parser_class = parsers.get(syntax_type, None)
 
     if parser_class is None:
         print("unknown lexer type: ", lexer.__class__.__name__)
```

### Comparing `syntaxlight-0.0.4/PKG-INFO` & `syntaxlight-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.4
+Version: 0.0.5
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -47,12 +47,31 @@
 dot -Tpng ./ast.dot -o ast.png
 ```
 
 ## 文档和 API
 
 关于详细的 API 使用方法, 以及对于默认配置的修改情况请参阅 [syntaxlight 使用文档](https://luzhixing12345.github.io/syntaxlight/)
 
+## 开发功能
+
+本仓库的 Makefile 与 test.py 提供了对于测试用例的渲染预览, 运行后打开 syntaxlight_example/index.html 即可
+
+```bash
+# 浏览所有 C 测试用例集合渲染结果
+make 
+
+# 浏览所有 json 测试用例集合渲染结果
+make t=json
+
+# 浏览 json 第一个 test/json/1.json 测试用例渲染结果
+make t=json i=1
+
+# 浏览 toml 第一个 test/toml/1.json 测试用例在 one-dark-pro 风格下的渲染结果
+make t=toml i=1 s=one-dark-pro
+```
+
 ## 参考
 
 - [Let's Build A Simple Interpreter](https://ruslanspivak.com/lsbasi-part1/)
+- [tree-sitter](https://github.com/tree-sitter/tree-sitter)
 - [pygments](https://pygments.org/)
 - [carbon](https://carbon.now.sh/)
```

