# Comparing `tmp/dolang-0.0.8.tar.gz` & `tmp/dolang-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolang-0.0.8.tar", last modified: Mon Apr 27 10:12:09 2020, max compression
+gzip compressed data, was "dolang-0.0.9.tar", last modified: Thu Aug 27 20:50:24 2020, max compression
```

## Comparing `dolang-0.0.8.tar` & `dolang-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      172 2020-04-09 10:30:41.074278 dolang-0.0.8/dolang/__init__.py
--rw-r--r--   0        0        0    17796 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/codegen.py
--rw-r--r--   0        0        0    35628 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/dataclasses.py
--rw-r--r--   0        0        0     3177 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/factory.py
--rw-r--r--   0        0        0     4081 2020-04-27 08:12:56.398961 dolang-0.0.8/dolang/function_compiler.py
--rw-r--r--   0        0        0      328 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/language.py
--rw-r--r--   0        0        0     8726 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/latex.py
--rw-r--r--   0        0        0     4049 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/objects.py
--rw-r--r--   0        0        0     6312 2020-04-09 10:30:41.078278 dolang-0.0.8/dolang/pattern.py
--rw-r--r--   0        0        0     9728 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/symbolic.py
--rw-r--r--   0        0        0     5876 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/symbolic_old.py
--rw-r--r--   0        0        0     1172 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/symbols.py
--rw-r--r--   0        0        0        0 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/tests/test.py
--rw-r--r--   0        0        0      758 2020-04-27 08:34:38.481942 dolang-0.0.8/dolang/tests/test_compiler.py
--rw-r--r--   0        0        0     2739 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/tests/test_make_function.py
--rw-r--r--   0        0        0      639 2020-04-27 08:30:01.713890 dolang-0.0.8/dolang/tests/test_patterns.py
--rw-r--r--   0        0        0     2940 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/tests/test_symbolic.py
--rw-r--r--   0        0        0      708 2020-04-27 08:29:53.357768 dolang-0.0.8/dolang/tests/test_symbols.py
--rw-r--r--   0        0        0     3431 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/triangular_solver.py
--rw-r--r--   0        0        0     4092 2020-04-09 10:30:41.082278 dolang-0.0.8/dolang/vectorize.py
--rw-r--r--   0        0        0      425 2020-04-27 09:09:04.926787 dolang-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      698 2020-04-27 10:12:09.994860 dolang-0.0.8/setup.py
--rw-r--r--   0        0        0      596 2020-04-27 10:12:09.995157 dolang-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/__init__.py
+-rw-r--r--   0        0        0    17796 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/codegen.py
+-rw-r--r--   0        0        0    35628 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/dataclasses.py
+-rw-r--r--   0        0        0     3129 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/factory.py
+-rw-r--r--   0        0        0     4158 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/function_compiler.py
+-rw-r--r--   0        0        0    10936 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/grammar.py
+-rw-r--r--   0        0        0      328 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/language.py
+-rw-r--r--   0        0        0     8941 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/latex.py
+-rw-r--r--   0        0        0     4049 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/objects.py
+-rw-r--r--   0        0        0     6312 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/pattern.py
+-rw-r--r--   0        0        0    10770 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/symbolic.py
+-rw-r--r--   0        0        0     5876 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/symbolic_old.py
+-rw-r--r--   0        0        0     1172 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/symbols.py
+-rw-r--r--   0        0        0      762 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/tests/test_compiler.py
+-rw-r--r--   0        0        0      322 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/tests/test_latex.py
+-rw-r--r--   0        0        0      741 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/tests/test_patterns.py
+-rw-r--r--   0        0        0     3361 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/tests/test_symbolic.py
+-rw-r--r--   0        0        0      816 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/tests/test_symbols.py
+-rw-r--r--   0        0        0     3431 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/triangular_solver.py
+-rw-r--r--   0        0        0     4092 2020-08-27 20:50:13.845900 dolang-0.0.9/dolang/vectorize.py
+-rw-r--r--   0        0        0      446 2020-08-27 20:50:13.845900 dolang-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      693 2020-08-27 20:50:24.583701 dolang-0.0.9/setup.py
+-rw-r--r--   0        0        0      591 2020-08-27 20:50:24.584004 dolang-0.0.9/PKG-INFO
```

### Comparing `dolang-0.0.8/dolang/codegen.py` & `dolang-0.0.9/dolang/codegen.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/dataclasses.py` & `dolang-0.0.9/dolang/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/factory.py` & `dolang-0.0.9/dolang/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,19 @@
 
 def substitute_preamble(ff: FlatFunctionFactory):
     import dolang
     import copy
     from .symbolic import NameSubstituter
     pr = copy.copy(ff.preamble)
     for k in pr.keys():
-        pr[k] = dolang.parse_string(pr[k]).value
+        pr[k] = dolang.parse_string(pr[k])
     st = NameSubstituter(pr)
     dd = copy.copy(ff.content)
     for k in dd.keys():
-        eq = dolang.parse_string(dd[k]).value
-        dd[k] = to_source(st.visit(eq))
+        dd[k] = to_source(st.transform(eq))
     return FlatFunctionFactory({}, dd, ff.arguments, ff.funname)
 
 
 def get_symbolic_derivatives(fff: FlatFunctionFactory, max_order=1):
 
     eqs = [symlib.sympify(eq) for eq in fff.content.values()]
     varname = [*fff.arguments.keys()][0]
```

### Comparing `dolang-0.0.8/dolang/function_compiler.py` & `dolang-0.0.9/dolang/function_compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 from ast import Assign, arg, FunctionDef, Module, Store, Subscript, Name, Load, Index, Num
 from ast import arguments as ast_arguments
 
+from dolang.grammar import tree_to_ast
 from dolang.factory import FlatFunctionFactory
 from dolang.symbolic import parse_string
 from dolang.codegen import to_source
 
 import sys
 
 def compile_factory(fff: FlatFunctionFactory):
@@ -19,21 +20,22 @@
                             slice=Index(Num(pos)), ctx=Load())
             val = Assign(targets=[Name(id=sym, ctx=Store())], value=rhs)
             unpacking.append(val)
 
     body = []
 
     for (k, neq) in fff.preamble.items():
-        val = parse_string(neq).value
+        tree = parse_string(neq)
+        val = tree_to_ast(tree).value
         line = Assign(targets=[Name(id=k, ctx=Store())], value=val)
         body.append(line)
 
     for n, (k, neq) in enumerate(fff.content.items()):
-        # should the result of parse_string always of type Expr ?
-        val = parse_string(neq).value
+        tree = parse_string(neq)
+        val = tree_to_ast(tree).value
         line = Assign(targets=[Name(id=k, ctx=Store())], value=val)
         body.append(line)
     #
     for n, (lhs, neq) in enumerate(fff.content.items()):
         line = Assign(targets=[Subscript(value=Name(id='out', ctx=Load()),
                                          slice=Index(Num(n)), ctx=Store())], value=Name(id=lhs, ctx=Load()))
         body.append(line)
@@ -47,22 +49,22 @@
     else:
         f = FunctionDef(name=funname,
                         args=ast_arguments(args=[arg(arg=a) for a in arguments] + [arg(arg='out')],
                                            vararg=None, kwarg=None, kwonlyargs=[], kw_defaults=[], defaults=[]),
                         body=unpacking + body, decorator_list=[])
         mod = Module(body=[f])
 
-
     mmod = ast.fix_missing_locations(mod)
     return mmod
 
 def make_method_from_factory(fff: FlatFunctionFactory, vectorize=True, use_file=False, debug=False):
     mod = compile_factory(fff)
 
     if debug:
+        from .codegen import to_source
         print(to_source(mod))
 
     if vectorize:
         coredims = [len(v) for k, v in fff.arguments.items()]
         signature = str.join(',', ['(n_{})'.format(d) for d in coredims])
         n_out = len(fff.content)
         if n_out in coredims:
```

### Comparing `dolang-0.0.8/dolang/latex.py` & `dolang-0.0.9/dolang/latex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 import re
 import ast
-from .symbolic import eval_scalar
+
+def eval_scalar(tree):
+    try:
+        if isinstance(tree, ast.Num):
+            return tree.n
+        elif isinstance(tree, ast.UnaryOp):
+            if isinstance(tree.op, ast.USub):
+                return -tree.operand.n
+            elif isinstance(tree.op, ast.UAdd):
+                return tree.operand.n
+        else:
+            raise Exception("Don't know how to do that.")
+    except:
+        raise Exception("Don't know how to do that.")
+
 
 def parse(s): return ast.parse(s).body[0].value
 
 class ExprVisitor(ast.NodeVisitor):
 
     def __init__(self, variables):
         self.variables = variables
@@ -95,17 +109,17 @@
     else:
         suffix = None
     if expr in greek_letters:
         res = greek_letters[expr]
     else:
         res = expr
     if suffix=='bar':
-        res = "\overline{{{}}}".format(res)
+        res = "\\overline{{{}}}".format(res)
     elif suffix == 'star':
-        res = "{}^{{\star}}".format(res)
+        res = "{}^{{\\star}}".format(res)
     return res
 # greekify('zbar')
 
 
 def split_name_into_parts(a):
     s = a.replace('__','&')
     m = reg_rad.findall(a)
@@ -169,15 +183,15 @@
     def visit_Variable(self, tvar):
         return name_to_latex(tvar[0], tvar[1])
 
     def visit_RCall(self, n):
         func = self.visit(n.func)
         args = ', '.join(map(self.visit, n.args))
         if func == 'sqrt':
-            return '\sqrt{%s}' % args
+            return '\\sqrt{%s}' % args
         else:
             return r'\operatorname{%s}\left(%s\right)' % (func, args)
 
     def prec_Call(self, n):
         return 1000
     def prec_RCall(self, n):
         return 1000
@@ -317,16 +331,7 @@
     expr = s.replace('==', '=').replace('=','==')
     if '==' in expr:
         lhs, rhs = [expr2tex(variables,str.strip(e)) for e in str.split(expr,'==')]
         return "{} = {}".format(lhs, rhs)
     else: return expr2tex(variables,expr)
 
 # ast.dump(ast.parse("a == b"))
-
-if __name__ == "__main__":
-
-    s = '(a + w_1__y)/2 + 1'
-    s =  "-(1+2)"
-    s = "a*x(2) + b*y(-1)"
-    print( expr2tex(['x','y'], s) )
-    eq = "l = a*x(2) + b*y(-1)"
-    print( eq2tex(['x','y'], eq))
```

### Comparing `dolang-0.0.8/dolang/objects.py` & `dolang-0.0.9/dolang/objects.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/pattern.py` & `dolang-0.0.9/dolang/pattern.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/symbolic.py` & `dolang-0.0.9/dolang/symbolic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,343 +1,364 @@
-from dolang.language import functions as functions_dict
-from dolang.codegen import to_source
-from typing import Tuple, List, Dict, Set, TypeVar, Union
-from ast import NodeTransformer, Name, UnaryOp, UAdd, USub, Load, Call
-
-try:
-    from .dataclasses import dataclass
-except:
-    from dataclasses import dataclass
-
-import ast
-from ast import Expr
-from functools import wraps
-import re
-
-T = TypeVar('T')
-
-Expression = ast.Expr
-
-functions = list(functions_dict.keys())
-
-__regex_eq__ = re.compile("([^=]*)=([^=]*)")
-
-
-def parse_string(s: str) -> ast.Expr:
-    ss = s.replace("^", "**")
-    m = re.match(__regex_eq__, ss)
-    if m:
-        ss = str.join('==', m.groups())
-    return ast.parse(ss).body[0]
-
-
-def dedup(l: List[T]) -> List[T]:
-    return list(dict.fromkeys(l))
-
-
-def stringify_variable(arg: Tuple[str, int]) -> str:
-    s = arg[0]
-    date = arg[1]
-    if date == 0:
-        return '{}__0_'.format(s)
-    elif date <= 0:
-        return '{}_m{}_'.format(s, str(-date))
-    elif date >= 0:
-        return '{}__{}_'.format(s, str(date))
-
-
-def stringify_parameter(p: str) -> str:
-    return '{}_'.format(p)
-
-
-def stringify_symbol(arg) -> str:
-    if isinstance(arg, str):
-        return stringify_parameter(arg)
-    elif isinstance(arg, tuple):
-        if len(arg) == 2 and isinstance(arg[0], str) and isinstance(
-                arg[1], int):
-            return stringify_variable(arg)
-    raise Exception("Unknown canonical form: {}".format(arg))
-
-
-def destringify_variable(s: str) -> Tuple[str, int]:
-    raise Exception("Not implemented.")
-
-
-def destringify_parameter(s: str) -> Tuple[str, int]:
-    raise Exception("Not implemented.")
-
-
-def destringify(s: str):
-    raise Exception("Not implemented.")
-
-
-###
-# The following function can take a string or an expression as the first argument, and return an argument of the same type.
-###
-
-
-def expression_or_string(f):
-    @wraps(f)
-    def wrapper(*args, **kwds):
-        if not isinstance(args[0], str):
-            return f(*args, **kwds)
-        else:
-            a = parse_string(args[0])
-            nargs = tuple([a]) + args[1:]
-            res = f(*nargs, **kwds)
-            return to_source(res)
-
-    return wrapper
-
-
-@expression_or_string
-def stringify(expr: Expression, variables: List[str] = []) -> Expression:
-    import copy
-    en = ExpressionStringifier(variables=variables)
-    return en.visit(copy.deepcopy(expr))
-
-
-# shift timing in equations
-# time_shift(:(a+b(1)+c),1,[:b,:c]) == :(a+b(2)+c(1))
-
-
-@expression_or_string
-def time_shift(expr: Expression, n) -> Expression:
-    import copy
-    eexpr = copy.deepcopy(expr)
-    variables = [e[0] for e in list_variables(eexpr)]
-    return TimeShiftTransformer(shift=n, variables=variables).visit(eexpr)
-
-
-@expression_or_string
-def steady_state(expr: Expression) -> Expression:
-    import copy
-    eexpr = copy.deepcopy(expr)
-    variables = [e[0] for e in list_variables(eexpr)]
-    return TimeShiftTransformer(shift='S', variables=variables).visit(eexpr)
+from .grammar import *
+parse_string = parser.parse
 
 
-@expression_or_string
-def sanitize(expr: Expression, variables=None, functions=None):
-    # special functions ?
-    es = ExpressionSanitizer(variables=variables)
-    return es.visit(expr)
-
-
-def list_variables(expr: Expression,
-                   funs: List[str] = None) -> List[Tuple[str, int]]:
-
-    if funs is None:
-        funs = []
-    ll = ListSymbols(known_functions=functions + funs)
-    ll.visit(expr)
-    if ll.problems:
-        e = Exception('Symbolic error.')
-        e.problems = ll.problems
-        raise e
-    return dedup([v[0] for v in ll.variables])
-
-
-@dataclass
-class SymbolList(dict):
-    variables: Set[Tuple[str, int]]
-    parameters: Set[str]
-    functions: Set[str]
-
-
-def list_symbols(expr: Expression, funs: List[str] = None) -> SymbolList:
-    if funs is None:
-        funs = []
-    ll = ListSymbols(known_functions=functions + funs)
-    ll.visit(expr)
-    if ll.problems:
-        e = Exception('Symbolic error.')
-        e.problems = ll.problems
-        print(e.problems)
-        raise e
-
-    def head(v):
-        return [i[0] for i in v]
-
-    return SymbolList(
-        dedup(head(ll.variables)), dedup(head(ll.constants)),
-        dedup(head(ll.functions)))
-
-
-### Tree manipulation functions
-
+import ast
 
-def eval_scalar(tree: Expression) -> Union[int, float]:
+def eval_scalar(tree):
     try:
         if isinstance(tree, ast.Num):
             return tree.n
         elif isinstance(tree, ast.UnaryOp):
             if isinstance(tree.op, ast.USub):
                 return -tree.operand.n
             elif isinstance(tree.op, ast.UAdd):
                 return tree.operand.n
         else:
             raise Exception("Don't know how to do that.")
     except:
         raise Exception("Don't know how to do that.")
 
 
-class ListSymbols(ast.NodeVisitor):
-    def __init__(self, known_functions=[], known_variables=[]):
-        self.known_functions = known_functions
-        self.known_variables = known_variables
-        self.functions = []
-        self.variables = []
-        self.constants = []
-        self.problems = []
-
-    def visit_Call(self, call):
-        name = call.func.id
-        colno = call.func.col_offset
-        if name in self.known_functions:
-            self.functions.append((name, colno))
-            [self.visit(e) for e in call.args]
-        else:
-            try:
-                assert (len(call.args) == 1)
-                n = int(eval_scalar(call.args[0]))
-                self.variables.append(((name, n), colno))
-            except Exception as e:
-                self.problems.append([name, 0, colno, 'incorrect subscript'])
-                # [self.visit(e) for e in call.args]
-
-    def visit_Name(self, name):
-        # colno = name.colno
-        colno = name.col_offset
-        n = 0
-        name = name.id
-        if name in self.known_functions:
-            self.problems.append([name, colno, 'function_not_called'])
-        else:
-            self.constants.append((name, colno))
-
-
-class ExpressionStringifier(NodeTransformer):
-
-    # replaces calls to variables by time subscripts
-
-    def __init__(self, variables=None, functions=None, constants=None):
-
-        self.variables = variables if variables is not None else []
-        if functions is None:
-            self.functions = [e for e in functions_dict.keys()]
-        else:
-            self.functions = functions
-        if constants is None:
-            self.constants = ['pi', 'e', 'inf']
-        else:
-            self.constants = constants
-        # self.variables = tvariables # ???
-
-    def visit_Name(self, node):
-
-        name = node.id
-        # if name self.functions:
-        #     return node
-        if name in self.constants:
-            return node
-        elif name in self.variables:
-            return Name(id=stringify_variable((name, 0)), ctx=Load())
-        else:
-            return Name(id=stringify_parameter(name), ctx=Load())
-
-    def visit_Call(self, node):
-
-        name = node.func.id
-        args = node.args[0]
-
-        if name in self.variables or name not in self.functions:
-            try:
-                date = eval_scalar(args)
-            except:
-                raise Exception("Unrecognized subscript.")
-            newname = stringify_variable((name, date))
-            if newname is not None:
-                return Name(newname, Load())
-        else:
-            return Call(
-                func=node.func,
-                args=[self.visit(e) for e in node.args],
-                keywords=[])
-
-
-class TimeShiftTransformer(ast.NodeTransformer):
-    def __init__(self, shift=0, variables=None):
-
-        self.variables = variables if variables is not None else []
-        self.shift = shift
-
-    def visit_Call(self, node):
-
-        name = node.func.id
-        args = node.args[0]
-
-        if name in self.variables:
-            if isinstance(args, UnaryOp):
-                # we have s(+1)
-                if (isinstance(args.op, UAdd)):
-                    args = args.operand
-                    date = args.n
-                elif (isinstance(args.op, USub)):
-                    args = args.operand
-                    date = -args.n
-                else:
-                    raise Exception("Unrecognized subscript.")
-            else:
-                date = args.n
-            if self.shift == 'S':
-                new_date = 0
-            else:
-                new_date = date + self.shift
-            return ast.parse('{}({})'.format(name, new_date)).body[0].value
-        else:
-
-            # , keywords=node.keywords,  kwargs=node.kwargs)
-            return Call(
-                func=node.func,
-                args=[self.visit(e) for e in node.args],
-                keywords=[])
-
-
-class ExpressionSanitizer(NodeTransformer):
-
-    # replaces calls to variables by time subscripts
-    def __init__(self, variables=None):
-        self.variables = variables if variables is not None else []
-
-    def visit_Name(self, node):
-        name = node.id
-        if name in self.variables:
-            return ast.parse('{}(0)'.format(name)).body[0].value
-        else:
-            return node
-
-    def visit_Call(self, node):
-        name = node.func.id
-        if name in self.variables:
-            t = eval_scalar(node.args[0])
-            return ast.parse('{}({})'.format(name, t)).body[0].value
-        else:
-            return Call(
-                func=node.func,
-                args=[self.visit(e) for e in node.args],
-                keywords=[])
-
-
-class NameSubstituter(ast.NodeTransformer):
-
-    # substitutes a name by an expression
-    def __init__(self, substitutions: Dict[str, Expr]):
-        self.substitutions = substitutions
-
-    def visit_Name(self, node):
-        name = node.id
-        if name in self.substitutions:
-            return self.substitutions[name]
-        else:
-            return node
+# from dolang.language import functions as functions_dict
+# from dolang.codegen import to_source
+# from typing import Tuple, List, Dict, Set, TypeVar, Union
+# from ast import NodeTransformer, Name, UnaryOp, UAdd, USub, Load, Call
+
+# try:
+#     from .dataclasses import dataclass
+# except:
+#     from dataclasses import dataclass
+
+# import ast
+# from ast import Expr
+# from functools import wraps
+# import re
+
+# T = TypeVar('T')
+
+# Expression = ast.Expr
+
+# functions = list(functions_dict.keys())
+
+# __regex_eq__ = re.compile("([^=]*)=([^=]*)")
+
+
+# def parse_string(s: str) -> ast.Expr:
+#     ss = s.replace("^", "**")
+#     m = re.match(__regex_eq__, ss)
+#     if m:
+#         ss = str.join('==', m.groups())
+#     return ast.parse(ss).body[0]
+
+
+# def dedup(l: List[T]) -> List[T]:
+#     return list(dict.fromkeys(l))
+
+
+# def stringify_variable(arg: Tuple[str, int]) -> str:
+#     s = arg[0]
+#     date = arg[1]
+#     if date == 0:
+#         return '{}__0_'.format(s)
+#     elif date <= 0:
+#         return '{}_m{}_'.format(s, str(-date))
+#     elif date >= 0:
+#         return '{}__{}_'.format(s, str(date))
+
+
+# def stringify_parameter(p: str) -> str:
+#     return '{}_'.format(p)
+
+
+# def stringify_symbol(arg) -> str:
+#     if isinstance(arg, str):
+#         return stringify_parameter(arg)
+#     elif isinstance(arg, tuple):
+#         if len(arg) == 2 and isinstance(arg[0], str) and isinstance(
+#                 arg[1], int):
+#             return stringify_variable(arg)
+#     raise Exception("Unknown canonical form: {}".format(arg))
+
+
+# def destringify_variable(s: str) -> Tuple[str, int]:
+#     raise Exception("Not implemented.")
+
+
+# def destringify_parameter(s: str) -> Tuple[str, int]:
+#     raise Exception("Not implemented.")
+
+
+# def destringify(s: str):
+#     raise Exception("Not implemented.")
+
+
+# ###
+# # The following function can take a string or an expression as the first argument, and return an argument of the same type.
+# ###
+
+
+# def expression_or_string(f):
+#     @wraps(f)
+#     def wrapper(*args, **kwds):
+#         if not isinstance(args[0], str):
+#             return f(*args, **kwds)
+#         else:
+#             a = parse_string(args[0])
+#             nargs = tuple([a]) + args[1:]
+#             res = f(*nargs, **kwds)
+#             return to_source(res)
+
+#     return wrapper
+
+
+# @expression_or_string
+# def stringify(expr: Expression, variables: List[str] = []) -> Expression:
+#     import copy
+#     en = ExpressionStringifier(variables=variables)
+#     return en.visit(copy.deepcopy(expr))
+
+
+# # shift timing in equations
+# # time_shift(:(a+b(1)+c),1,[:b,:c]) == :(a+b(2)+c(1))
+
+
+# @expression_or_string
+# def time_shift(expr: Expression, n) -> Expression:
+#     import copy
+#     eexpr = copy.deepcopy(expr)
+#     variables = [e[0] for e in list_variables(eexpr)]
+#     return TimeShiftTransformer(shift=n, variables=variables).visit(eexpr)
+
+
+# @expression_or_string
+# def steady_state(expr: Expression) -> Expression:
+#     import copy
+#     eexpr = copy.deepcopy(expr)
+#     variables = [e[0] for e in list_variables(eexpr)]
+#     return TimeShiftTransformer(shift='S', variables=variables).visit(eexpr)
+
+
+# @expression_or_string
+# def sanitize(expr: Expression, variables=None, functions=None):
+#     # special functions ?
+#     es = ExpressionSanitizer(variables=variables)
+#     return es.visit(expr)
+
+
+# def list_variables(expr: Expression,
+#                    funs: List[str] = None) -> List[Tuple[str, int]]:
+
+#     if funs is None:
+#         funs = []
+#     ll = ListSymbols(known_functions=functions + funs)
+#     ll.visit(expr)
+#     if ll.problems:
+#         e = Exception('Symbolic error.')
+#         e.problems = ll.problems
+#         raise e
+#     return dedup([v[0] for v in ll.variables])
+
+
+# @dataclass
+# class SymbolList(dict):
+#     variables: Set[Tuple[str, int]]
+#     parameters: Set[str]
+#     functions: Set[str]
+
+
+# def list_symbols(expr: Expression, funs: List[str] = None) -> SymbolList:
+#     if funs is None:
+#         funs = []
+#     ll = ListSymbols(known_functions=functions + funs)
+#     ll.visit(expr)
+#     if ll.problems:
+#         e = Exception('Symbolic error.')
+#         e.problems = ll.problems
+#         print(e.problems)
+#         raise e
+
+#     def head(v):
+#         return [i[0] for i in v]
+
+#     return SymbolList(
+#         dedup(head(ll.variables)), dedup(head(ll.constants)),
+#         dedup(head(ll.functions)))
+
+
+# ### Tree manipulation functions
+
+
+# def eval_scalar(tree: Expression) -> Union[int, float]:
+#     try:
+#         if isinstance(tree, ast.Num):
+#             return tree.n
+#         elif isinstance(tree, ast.UnaryOp):
+#             if isinstance(tree.op, ast.USub):
+#                 return -tree.operand.n
+#             elif isinstance(tree.op, ast.UAdd):
+#                 return tree.operand.n
+#         else:
+#             raise Exception("Don't know how to do that.")
+#     except:
+#         raise Exception("Don't know how to do that.")
+
+
+# class ListSymbols(ast.NodeVisitor):
+#     def __init__(self, known_functions=[], known_variables=[]):
+#         self.known_functions = known_functions
+#         self.known_variables = known_variables
+#         self.functions = []
+#         self.variables = []
+#         self.constants = []
+#         self.problems = []
+
+#     def visit_Call(self, call):
+#         name = call.func.id
+#         colno = call.func.col_offset
+#         if name in self.known_functions:
+#             self.functions.append((name, colno))
+#             [self.visit(e) for e in call.args]
+#         else:
+#             try:
+#                 assert (len(call.args) == 1)
+#                 n = int(eval_scalar(call.args[0]))
+#                 self.variables.append(((name, n), colno))
+#             except Exception as e:
+#                 self.problems.append([name, 0, colno, 'incorrect subscript'])
+#                 # [self.visit(e) for e in call.args]
+
+#     def visit_Name(self, name):
+#         # colno = name.colno
+#         colno = name.col_offset
+#         n = 0
+#         name = name.id
+#         if name in self.known_functions:
+#             self.problems.append([name, colno, 'function_not_called'])
+#         else:
+#             self.constants.append((name, colno))
+
+
+# class ExpressionStringifier(NodeTransformer):
+
+#     # replaces calls to variables by time subscripts
+
+#     def __init__(self, variables=None, functions=None, constants=None):
+
+#         self.variables = variables if variables is not None else []
+#         if functions is None:
+#             self.functions = [e for e in functions_dict.keys()]
+#         else:
+#             self.functions = functions
+#         if constants is None:
+#             self.constants = ['pi', 'e', 'inf']
+#         else:
+#             self.constants = constants
+#         # self.variables = tvariables # ???
+
+#     def visit_Name(self, node):
+
+#         name = node.id
+#         # if name self.functions:
+#         #     return node
+#         if name in self.constants:
+#             return node
+#         elif name in self.variables:
+#             return Name(id=stringify_variable((name, 0)), ctx=Load())
+#         else:
+#             return Name(id=stringify_parameter(name), ctx=Load())
+
+#     def visit_Call(self, node):
+
+#         name = node.func.id
+#         args = node.args[0]
+
+#         if name in self.variables or name not in self.functions:
+#             try:
+#                 date = eval_scalar(args)
+#             except:
+#                 raise Exception("Unrecognized subscript.")
+#             newname = stringify_variable((name, date))
+#             if newname is not None:
+#                 return Name(newname, Load())
+#         else:
+#             return Call(
+#                 func=node.func,
+#                 args=[self.visit(e) for e in node.args],
+#                 keywords=[])
+
+
+# class TimeShiftTransformer(ast.NodeTransformer):
+#     def __init__(self, shift=0, variables=None):
+
+#         self.variables = variables if variables is not None else []
+#         self.shift = shift
+
+#     def visit_Call(self, node):
+
+#         name = node.func.id
+#         args = node.args[0]
+
+#         if name in self.variables:
+#             if isinstance(args, UnaryOp):
+#                 # we have s(+1)
+#                 if (isinstance(args.op, UAdd)):
+#                     args = args.operand
+#                     date = args.n
+#                 elif (isinstance(args.op, USub)):
+#                     args = args.operand
+#                     date = -args.n
+#                 else:
+#                     raise Exception("Unrecognized subscript.")
+#             else:
+#                 date = args.n
+#             if self.shift == 'S':
+#                 new_date = 0
+#             else:
+#                 new_date = date + self.shift
+#             return ast.parse('{}({})'.format(name, new_date)).body[0].value
+#         else:
+
+#             # , keywords=node.keywords,  kwargs=node.kwargs)
+#             return Call(
+#                 func=node.func,
+#                 args=[self.visit(e) for e in node.args],
+#                 keywords=[])
+
+
+# class ExpressionSanitizer(NodeTransformer):
+
+#     # replaces calls to variables by time subscripts
+#     def __init__(self, variables=None):
+#         self.variables = variables if variables is not None else []
+
+#     def visit_Name(self, node):
+#         name = node.id
+#         if name in self.variables:
+#             return ast.parse('{}(0)'.format(name)).body[0].value
+#         else:
+#             return node
+
+#     def visit_Call(self, node):
+#         name = node.func.id
+#         if name in self.variables:
+#             t = eval_scalar(node.args[0])
+#             return ast.parse('{}({})'.format(name, t)).body[0].value
+#         else:
+#             return Call(
+#                 func=node.func,
+#                 args=[self.visit(e) for e in node.args],
+#                 keywords=[])
+
+
+# class NameSubstituter(ast.NodeTransformer):
+
+#     # substitutes a name by an expression
+#     def __init__(self, substitutions: Dict[str, Expr]):
+#         self.substitutions = substitutions
+
+#     def visit_Name(self, node):
+#         name = node.id
+#         if name in self.substitutions:
+#             return self.substitutions[name]
+#         else:
+#             return node
```

### Comparing `dolang-0.0.8/dolang/symbolic_old.py` & `dolang-0.0.9/dolang/symbolic_old.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/symbols.py` & `dolang-0.0.9/dolang/symbols.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/tests/test_compiler.py` & `dolang-0.0.9/dolang/tests/test_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,9 +24,11 @@
     fun = make_method_from_factory(fff)[0]
 
     import numpy as np
     out = np.array([0.3, 0.1])
 
     fun(np.array([0.1, 0.2]), np.array([10]), np.array([0.5, 0.3]), out)
 
-    print( abs(out[0] - 4.45168907)<1e-8 )
-    print( abs(out[1] - 8.2)<1e-8 )
+    assert( abs(out[0] - 4.45168907)<1e-8 )
+    assert( abs(out[1] - 8.2)<1e-8 )
+
+
```

### Comparing `dolang-0.0.8/dolang/tests/test_patterns.py` & `dolang-0.0.9/dolang/tests/test_patterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import dolang
-from dolang.pattern import compare_strings
-import yaml
-
-class bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-tests = yaml.safe_load(open('tests/patterns.yaml'))
-
-pattern_tests = tests['patterns']
-
-for l in pattern_tests:
-
-    res = compare_strings(l[0], l[1])
-    expected = l[2]
-    ok = (res==expected)
-    msg = bcolors.OKBLUE+'✓'+bcolors.ENDC if ok else bcolors.FAIL+'✗'+bcolors.ENDC
-    print('{} : {} : {} : ({} instead of {})'.format(msg,l[0],l[1],res,expected))
+def test_patterns():
+
+    import dolang
+    from dolang.pattern import compare_strings
+    import yaml
+
+    class bcolors:
+        HEADER = '\033[95m'
+        OKBLUE = '\033[94m'
+        OKGREEN = '\033[92m'
+        WARNING = '\033[93m'
+        FAIL = '\033[91m'
+        ENDC = '\033[0m'
+        BOLD = '\033[1m'
+        UNDERLINE = '\033[4m'
+
+    tests = yaml.safe_load(open('tests/patterns.yaml'))
+
+    pattern_tests = tests['patterns']
+
+    for l in pattern_tests:
+
+        res = compare_strings(l[0], l[1])
+        expected = l[2]
+        ok = (res==expected)
+        msg = bcolors.OKBLUE+'✓'+bcolors.ENDC if ok else bcolors.FAIL+'✗'+bcolors.ENDC
+        print('{} : {} : {} : ({} instead of {})'.format(msg,l[0],l[1],res,expected))
```

### Comparing `dolang-0.0.8/dolang/tests/test_symbols.py` & `dolang-0.0.9/dolang/tests/test_symbols.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from dolang.symbols import Symbol
-import yaml
+def test_symbols():
+    from dolang.symbols import Symbol
+    import yaml
 
-class bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
+    class bcolors:
+        HEADER = '\033[95m'
+        OKBLUE = '\033[94m'
+        OKGREEN = '\033[92m'
+        WARNING = '\033[93m'
+        FAIL = '\033[91m'
+        ENDC = '\033[0m'
+        BOLD = '\033[1m'
+        UNDERLINE = '\033[4m'
 
 
-txt = yaml.safe_load(open("tests/symbols.yaml"))
+    txt = yaml.safe_load(open("tests/symbols.yaml"))
 
-summary = []
-for short_sym, long_sym in txt['symbols'].items():
+    summary = []
+    for short_sym, long_sym in txt['symbols'].items():
 
 
-    sym = eval(long_sym)
-    result = (short_sym == (str(sym)))
-    summary.append([sym, long_sym, result])
+        sym = eval(long_sym)
+        result = (short_sym == (str(sym)))
+        summary.append([sym, long_sym, result])
 
-    # try the other direction (match short symbol)
+        # try the other direction (match short symbol)
 
-for l in summary:
-    ok = l[2]
-    msg = bcolors.OKBLUE+'✓'+bcolors.ENDC if ok else bcolors.FAIL+'✗'+bcolors.ENDC
-    print('{} | {:<50} -> {}'.format(msg, str(l[1]), l[0]))
+    for l in summary:
+        ok = l[2]
+        msg = bcolors.OKBLUE+'✓'+bcolors.ENDC if ok else bcolors.FAIL+'✗'+bcolors.ENDC
+        print('{} | {:<50} -> {}'.format(msg, str(l[1]), l[0]))
```

### Comparing `dolang-0.0.8/dolang/triangular_solver.py` & `dolang-0.0.9/dolang/triangular_solver.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/dolang/vectorize.py` & `dolang-0.0.9/dolang/vectorize.py`

 * *Files identical despite different names*

### Comparing `dolang-0.0.8/setup.py` & `dolang-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['dolang', 'dolang.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numba>=0.49.0,<0.50.0',
+['lark-parser>=0.9.0,<0.10.0',
+ 'numba>=0.50',
  'numpy>=1.18.3,<2.0.0',
- 'sympy>=1.5.1,<2.0.0',
- 'tempita>=0.5.2,<0.6.0']
+ 'sympy>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'dolang',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Dolo Modeling Language',
     'long_description': None,
     'author': 'Winant Pablo',
     'author_email': 'pablo.winant@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dolang-0.0.8/PKG-INFO` & `dolang-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dolang
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dolo Modeling Language
 License: BSD-2-Clause
 Author: Winant Pablo
 Author-email: pablo.winant@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: numba (>=0.49.0,<0.50.0)
+Requires-Dist: lark-parser (>=0.9.0,<0.10.0)
+Requires-Dist: numba (>=0.50)
 Requires-Dist: numpy (>=1.18.3,<2.0.0)
 Requires-Dist: sympy (>=1.5.1,<2.0.0)
-Requires-Dist: tempita (>=0.5.2,<0.6.0)
```

