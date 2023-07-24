# Comparing `tmp/orbit_component_zerodocs-1.0.17.tar.gz` & `tmp/orbit_component_zerodocs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_zerodocs-1.0.17.tar", max compression
+gzip compressed data, was "orbit_component_zerodocs-1.0.9.tar", max compression
```

## Comparing `orbit_component_zerodocs-1.0.17.tar` & `orbit_component_zerodocs-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.17/LICENSE.md
--rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.17/README.md
--rw-r--r--   0        0        0       97 2023-07-10 09:48:58.739070 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/__init__.py
--rwxr-xr-x   0        0        0    22584 2023-07-13 12:44:58.370278 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/doc_python.py
--rw-r--r--   0        0        0     3876 2023-07-21 17:06:43.646581 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/plugin.py
--rw-r--r--   0        0        0     3117 2023-07-21 16:48:16.496392 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/APIs.py
--rw-r--r--   0        0        0    14028 2023-07-21 17:04:52.192674 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/Cache.py
--rw-r--r--   0        0        0     1868 2023-07-13 12:27:27.754789 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/Project.py
--rw-r--r--   0        0        0      270 2023-07-13 17:20:37.712326 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/Versions.py
--rw-r--r--   0        0        0        0 2023-07-24 15:01:06.590511 orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/version.py
--rw-r--r--   0        0        0     1401 2023-07-24 15:01:06.590511 orbit_component_zerodocs-1.0.17/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.17/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.9/README.md
+-rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/__init__.py
+-rwxr-xr-x   0        0        0    19748 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py
+-rw-r--r--   0        0        0     1599 2023-06-08 11:28:29.403019 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/plugin.py
+-rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py
+-rw-r--r--   0        0        0    11017 2023-06-02 18:29:55.867494 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py
+-rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py
+-rw-r--r--   0        0        0      270 2023-06-08 11:36:09.568981 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Versions.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/version.py
+-rw-r--r--   0        0        0     1404 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.9/PKG-INFO
```

### Comparing `orbit_component_zerodocs-1.0.17/LICENSE.md` & `orbit_component_zerodocs-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/doc_python.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,27 @@
 #   WORK IN PROGRESS
 #
 #   Experimentation re; generating API documentation automatically from code
 #   Designed specifically to cope with P3 typing
 #   This was pulled from the original - needs a rewrite really, mostly works for now
 #
 import ast
-from typing import Any
 from ujson import dumps
 from loguru import logger as log
-from orbit_database import ObjectId
 
 class MethodVisitor(ast.NodeVisitor):
 
     def __init__(self, root):
         self._root = root
         super().__init__()
 
-    def visit_AsyncFunctionDef(self, node):
-        return self.visit_FunctionDef(node)
-
     def visit_FunctionDef(self, node):
         args = []
         anns = []
         defs = []
-        
-        # log.error(f'Name={node.name} ret={node.returns}')
-        
         for default in node.args.defaults:
             if isinstance(default, ast.NameConstant):
                 v = str(default.value)
             elif isinstance(default, ast.Num):
                 v = str(default.n)
             elif isinstance(default, ast.Attribute):
                 v = f'{default.value.id}.{default.attr}'
@@ -48,27 +40,21 @@
             else:
                 print("Unknown type: ", type(default))
 
             defs.append(v)
 
         defs = [None for i in range(len(node.args.args) - len(node.args.defaults))] + defs
 
-        # log.debug("--")
-        # for attr in ['args', 'defaults', 'kw_defaults', 'kwarg', 'kwonlyargs', 'posonlyargs', 'vararg']:
-        #     log.error(f'{attr} == {getattr(node.args, attr)}')
-            
         for x in node.args.args:
             args.append(x.arg)
             if isinstance(x.annotation, ast.Name):
                 anns.append(x.annotation.id)
             elif isinstance(x.annotation, ast.Subscript):
                 if isinstance(x.annotation.slice, ast.Name):
                     anns.append(x.annotation.slice.id)
-                elif hasattr(x.annotation.slice, 'op'):
-                    anns.append(self.recurse_ops(x.annotation.slice))
                 elif hasattr(x.annotation.slice, 'value'):
                     if isinstance(x.annotation.slice.value, ast.Name):
                         anns.append(x.annotation.slice.value.id)
                     elif isinstance(x.annotation.slice.value, ast.Subscript):
                         anns.append(x.annotation.slice.value)
                     else:
                         lst = []
@@ -78,84 +64,38 @@
                             else:
                                 if not isinstance(elt, ast.List):
                                     lst.append(elt.value.id)
                                 else:
                                     print(">>>", lst)
                         anns.append((x.annotation.value.id, lst))
                 else:
-                    print("Not sure what to do with: (", type(x.annotation.slice), ') ||', type(x.annotation.value), x.arg)
+                    print("Not sure what to do with: (", type(x.annotation.slice), ') ||', type(x.annotation), x.arg)
                     anns.append(None)
             else:
                 anns.append(None)
-        rets = self.recurse_subscript([node.returns])
-        if node.args.vararg:
-            args.append(f'*{node.args.vararg.arg}')
-            anns.append(None)
-
-        if node.args.kwarg:
-            args.append(f'**{node.args.kwarg.arg}')
-            anns.append(None)
+
+        if isinstance(node.returns, ast.Name):
+            rets = node.returns.id
+        elif isinstance(node.returns, ast.NameConstant):
+            rets = node.returns.value
+        else:
+            rets = None
 
         self._root['args'] = args
         self._root['anns'] = anns
         self._root['defs'] = defs
         self._root['rets'] = rets
         self._root['line'] = node.lineno
         self._root['docs'] = ast.get_docstring(node, clean=True) or ''
         for item in node.decorator_list:
             if item.id == 'property':
                 self._root['prop'] = True
 
-    def recurse_ops (self, param):
-        ret = ''
-        for p in [param.left, param.op, param.right]:
-            if isinstance(p, ast.BinOp):
-                ret += self.recurse_ops(p)
-                continue
-            elif isinstance(p, ast.BitOr):
-                ret += "|"
-                continue
-            elif isinstance(p, ast.Name):
-                ret += str(p.id)
-            elif isinstance(p, ast.NameConstant):
-                ret += str(p.value)
-        return ret
-
-    def recurse_subscript(self, params):
-        ret = ''
-        for param in params:               
-            if ret: ret += ', '    
-            if isinstance(param, ast.Name):
-                ret += str(param.id)
-            elif isinstance(param, ast.NameConstant):
-                ret += str(param.value)
-            elif isinstance(param, ast.Subscript):
-                if hasattr(param.slice, 'elts'):
-                    ret += f'{param.value.id}[{self.recurse_subscript(param.slice.elts)}]'
-                elif hasattr(param.slice, 'op'):
-                    ret += self.recurse_ops(param.slice)
-                else:
-                    log.error(f"Don't know what to do with {param.slice} {dir(param.slice)}")
-                    ret = f'{param.value.id}[{param.slice.id}]'
-            elif isinstance(param, ast.List):
-                ret += f'[{self.recurse_subscript(param.elts)}]'
-            elif param == None:
-                pass
-            else:
-                ret = ''
-                log.error(f"Failed: {param}, {type(param)} {dir(param)}")
-            
-        return ret
-                
-
     def generic_visit(self, node):
-        if isinstance(node, ast.FunctionDef):
-            return self.visit_FunctionDef(node)
-        else:
-            print(f"B> Unhandled node: {node}")            
+        print(f"B> Unhandled node: {node}")
 
 
 class ClassVisitor(ast.NodeVisitor):
 
     def __init__(self, root):
         self._root = root
         super().__init__()
@@ -173,26 +113,26 @@
         elif isinstance(val, ast.Bytes):
             return val.s
 
         print("Unknown type: ", type(val))
         return None
 
     def visit_ClassDef(self, node):
-        # log.error(f"BASES: {node.bases} node: {node.name} line: {node.lineno}")
+        log.error(f"BASES: {node.bases} node: {node.name} line: {node.lineno}")
         self._root[node.name] = {
             'base': [base.id for base in node.bases],
             'name': node.name,
             'defs': {},
             'docs': ast.get_docstring(node, clean=True) or '',
             'cdef': {},
             'line': node.lineno
         }
         root = self._root[node.name]
         for method_node in ast.iter_child_nodes(node):
-            if isinstance(method_node, ast.FunctionDef) or isinstance(method_node, ast.AsyncFunctionDef):
+            if isinstance(method_node, ast.FunctionDef):
                 root['defs'][method_node.name] = {}
                 MethodVisitor(root['defs'][method_node.name]).visit(method_node)
             elif isinstance(method_node, ast.Name):
                 pass
             elif isinstance(method_node, ast.Pass):
                 pass
             elif isinstance(method_node, ast.Assign):
@@ -235,15 +175,15 @@
 
 
 class Documentation:
 
     BASE_URL = 'https://gitlab.com/oddjobz/pynndb2/-/blob/master/pynndb'
     EXAMPLE_URL = 'https://gitlab.com/oddjobz/pynndb2-examples/-/blob/master'
 
-    def present(self, module_root):
+    def present(self):
         css_module = '<div class="moduledef">'
         css_module_doc = '<div class="moduledoc">'
         css_module_doc_end = '</div>'
         css_module_end = '</div>'
         css_class_end = '</div>'
         css_klass = '<span class="klass">'
         css_klass_end = '</span>'
@@ -276,27 +216,36 @@
         def function_href(k, f):
             f = f.replace("_", "")
             return f'<div class="function" id="item-{k}-{f}">'
 
         def class_href(k):
             return f'<div class="classdef" id="section-{k}">'
 
-        def format_doc(text):
+        def format_docstringmod(text):
+            lines = text.split('\n')
+            section1 = ''
+            section2 = ''
+
+            while len(lines):
+                line = lines.pop(0)
+                if not len(line):
+                    break
+                section1 += line + '\n'
+            while len(lines):
+                line = lines.pop(0)
+                section2 += line
+
+            return f'{css_module_doc}{section1}\n<div>{section2}</div>{css_module_doc_end}'
+
+        def format_docstring(text):
             result = ''
             lines = text.split('\n')
             out = ''
-            ret = ''
             while len(lines):
                 line = lines.pop(0)
-                if len(line) and line[0] == '>':
-                    ret += f"<div class='doc-note'>{line.replace('> ', '📌 ')}</div>"
-                    continue
-                if len(line) and line[0] == '!':
-                    ret += f"<div class='doc-note'>{line.replace('! ', '😶 ')}</div>"
-                    continue
                 if not len(line):
                     result += out + '\n'
                     out = ''
                 elif line == '---':
                     result += out + '\n'
                     out = ''
                     while len(lines):
@@ -310,40 +259,22 @@
                     result += out
                     out = ''
                     while len(lines):
                         line = lines.pop(0)
                         if line == '```':
                             break
                         out += f'{line}\n'
-                    out = f'<div class="docs-code-block"><pre class="shadow-lg rounded"><code class="python">{out}</code></pre></div>'
+                    out = f'<div class="docs-code-block"><pre class="shadow-lg rounded"><code class="python hljs">{out}</code></pre></div>'
                 elif line[:2] in ['  ', 'o ', '- ', '* ']:
                     result += '\n' + line.replace('* ', '📌 ')
                     out = ''
                 else:
                     out += line + ' '
             result += '\n' + out
-            if ret:
-                result =result.strip() + ret            
-            return result
-        
-        def format_docstringmod(text):
-            lines = text.split('\n')
-            section1 = ''
-            section2 = ''
-            while len(lines):
-                line = lines.pop(0)
-                if not len(line):
-                    break
-                section1 += line + '\n'
-
-            section2 = format_doc("\n".join(lines)).strip()
-            return f'{css_module_doc}{section1}<div>{section2}</div>{css_module_doc_end}'
-        
-        def format_docstring(text):
-            return f'{docstring}{format_doc(text).strip()}{docstring_end}'
+            return f'{docstring}{result.strip()}{docstring_end}'
 
         def parse_tuple(text):
             items = ''
             for item in text:
                 if len(items):
                     items += ' | '
                 items += (item.id if isinstance(item, ast.Name) else item)
@@ -386,45 +317,36 @@
                 print(type(text))
                 return '???'
 
         def function_definition(module, klass, name):
             fn = klass['defs'][name]
             # base = self.BASE_URL if self._name == 'pynndb' else f'{self.EXAMPLE_URL}/{self._name}'
             # url = f'{base}/{module_name}.py#L{fn.get("line")}'
-            # url = 'need a module url'
-            # s = f'<a href="{url}" target="_blank">{method}{name}{method_end} </a>'
+            url = 'need a module url'
+            s = f'<a href="{url}" target="_blank">{method}{name}{method_end} </a>'
 
             docs = fn.get('docs')
             anns = fn.get('anns')
             args = fn.get('args')
             defs = fn.get('defs')
             line = fn.get('line')
-            
-            s= f'<a onclick="window.zd_gotoSource({line})">{method}{name}{method_end} </a>'
 
             text = ''
             look = {}
             newa = []
-            if args:
-                for arg in args:
-                    look[arg] = {
-                        'ann': anns.pop(0) if len(anns) else None,
-                        'def': defs.pop(0) if len(defs) else None
-                    }
-                    a = look[arg]['def']
-                    if isinstance(a, str):
-                        arg = f'[{css_arg}{arg}{css_arg_end}]'
-                    else:
-                        arg = f'{css_arg}{arg}{css_arg_end}'
-                    newa.append(arg)
-            else:
-                print("ERROR:", docs,anns,args,defs,line)
-                return
+            for arg in args:
+                look[arg] = {'ann': anns.pop(0), 'def': defs.pop(0)}
+                a = look[arg]['def']
+                if isinstance(a, str):
+                    arg = f'[{css_arg}{arg}{css_arg_end}]'
+                else:
+                    arg = f'{css_arg}{arg}{css_arg_end}'
+                newa.append(arg)
 
-            s += f'({", ".join(newa)})' + (f' -> {css_return}{fn.get("rets")}{css_return_end}' if fn.get("rets") else '')
+            s += f'({", ".join(newa)}) -> {css_return}{fn.get("rets")}{css_return_end}'
             p = ''
             pcount = 0
             p += f'{params}'
             for line in docs.split("\n"):
                 parts = line.split(" ")
                 if len(parts) > 1 and parts[1] == '-':
                     pcount += 1
@@ -447,107 +369,115 @@
             if pcount:
                 s += f'{paramslabel}PARAMETERS{paramslabel_end}{p}'
             else:
                 s += f'{params}{params_end}'
             return s
 
         def module_definition(module):
+            # module = self._modules.get(module_name)
             docs = module.get('__doc__') if '__doc__' in module else None
+            # if not module:
+            #     print(f'Module not found: {module_name}')
+            #     return ''
             s = f'{format_docstringmod(docs)}' if docs else ''
             for klass_name in module.keys():
                 if klass_name in ['__doc__']:
                     continue
-                               
                 klass = module[klass_name]
+                # base = self.BASE_URL if self._name == 'pynndb' else f'{self.EXAMPLE_URL}/{self._name}'
+                # url = f'{base}/{module_name}.py#L{klass.get("line")}'
+                url = 'need url'
+
+                # sidebar.write(f'<li class="nav-item section-title mt-3">\n')
+                # sidebar.write(f' <a class="nav-link scrollto" href="#section-{klass_name}">\n')
+                # sidebar.write(f'{CLASS_ICON}{klass_name}')
+                # sidebar.write(f' </a></li>\n')
+
                 s += f'{class_href(klass_name)}\n'
-                line = klass.get("line")
-                s += f'{keyword}class{keyword_end} <a onclick="window.zd_gotoSource({line})">{css_klass}{klass_name}{css_klass_end}</a>\n'
-                
+                s += f'{keyword}class{keyword_end} <a href="{url}" target="_blank">{css_klass}{klass_name}{css_klass_end}</a>\n'
                 if klass.get('base'):
                     params = ", ".join([f"{css_arg}{base}{css_arg_end}\n" for base in klass["base"]])
                     s += f'({params})'
                     s += ':'
                 s += format_docstring(klass.get("docs"))
+
+                # sidebar.write(f'<ul class="section-items list-unstyled nav flex-column pb3">')
                 if 'cdef' in klass:
                     cdef = klass.get('cdef')
                     if len(cdef):
                         s += f'{methodslabel}CLASS PROPERTIES{methodslabel_end}\n'
                         for item in sorted(cdef):
                             href = f'#item-{klass_name}-{item}'
+                            # sidebar.write(f'<li class="nav-item"><a class="nav-link scrollto" href="{href}">{item}</a></li>')
                             s += f'<div class="cdef" id="item-{klass_name}-{item}">{method}{item}{method_end} =\n'
                             if isinstance(cdef[item], dict):
                                 s += f'<pre>{dumps(cdef[item], indent=4)}'
                             else:
                                 s += f'"{css_literal}{cdef[item]}{css_literal_end}"'
                             s += f'</div>'
 
                 if klass.get('defs'):
                     p = f'{methodslabel}PROPERTIES{methodslabel_end}\n'
                     found = False
                     for fn in sorted(klass['defs']):
                         if klass['defs'][fn].get('prop'):
                             found = True
                             href = f'item-{klass_name}-{fn.replace("_", "")}'
+
                             line = klass['defs'][fn].get('line')
+
                             self.addIndex('property', href, fn, line)
+                            # sidebar.write(f'<li class="nav-item"><a class="nav-link scrollto" href="{href}">{fn}</a></li>')
                             p += f'{function_href(klass_name, fn)}{function_definition(self._module, klass, fn)}{css_function_end}\n'
                     if found:
                         s += p
 
                 if klass.get('defs'):
                     m = f'{methodslabel}METHODS{methodslabel_end}\n'
                     found = False
-                    for fn in klass['defs']:
+                    for fn in sorted(klass['defs']):
                         if not klass['defs'][fn].get('prop'):
                             found = True
                             href = f'item-{klass_name}-{fn.replace("_", "")}'
+
                             line = klass['defs'][fn].get('line')
+
                             self.addIndex('method', href, fn, line)
+                            # sidebar.write(f'<li class="nav-item"><a class="nav-link scrollto" href="{href}">{fn}</a></li>')
                             m += f'{function_href(klass_name, fn)}{function_definition(self._module, klass, fn)}{css_function_end}\n'
                     s += m
+
                 s += f'{css_class_end}\n'
+                # sidebar.write(f'</ul>')
             return s
-        fns = "".join([function_definition(None, {'defs': module_root}, fn) for fn in module_root.keys()])
-        return f'{css_module}{module_definition(self._module)}{fns}{css_module_end}'
+
+        return f'{css_module}{module_definition(self._module)}{css_module_end}'
 
     def addIndex (self, typ, href, fn, ln):
         node = {
             'parent': self._key,
             'type': typ,
             'label': fn,
             'isLeaf': True,
             'line': ln,
-            '_id': str(ObjectId()),
-            'uri': href
+            '_id': href,
         }
         self._index.append(node)
 
     def __init__(self):
         self._module = {}
         self._index = []
         self._key = None
 
     def run(self, key, text):
         self._key = key
         tree = ast.parse(text)
         self._module['__doc__'] = ast.get_docstring(tree)
         ClassVisitor(self._module).visit(tree)
-        root = {}
-        for item in tree.body:
-            if isinstance(item, ast.FunctionDef) or isinstance(item, ast.AsyncFunctionDef):
-                root[item.name] = {'defs': {item.name: {
-                    'base': [],
-                    'name': 'module',
-                    'defs': {},
-                    'docs': '',
-                    'cdef': {},
-                    'line': item.lineno
-                }}}
-                MethodVisitor(root[item.name]).visit(item)
-        return self._index, self.present(root)
+        return self._index, self.present()
 
 
 if __name__ == '__main__':
     with open('test1.py') as io:
         text = io.read()
     print(Documentation().run(text))
```

### Comparing `orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/APIs.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,18 +54,15 @@
     def get_api_remote (self, provider, api, branch, path):
         files = []
         folders = []
         if provider == 'gitlab':
             project = [p for p in gitlab.projects.list(search=api, ref=branch) if p.path == api]
             if not project:
                 return {'ok': False, 'error': f'unable to find project: {api}'}
-            # log.error(f'{project[0]}=>{str(dir(project[0]))}')
-            # log.error(f'URL={project[0].web_url}')
-            # log.error(f'Path={project[0].path}')
-            for file in project[0].repository_tree(path=path, recursive=False, ref=branch, get_all=True):
+            for file in project[0].repository_tree(path=path, recursive=False, ref=branch):
                 item = {
                     'key': f"{branch}|{file['id']}",
                     'label': file['name'],
                     'path': file['path'],
                     'type': file['type'],
                     'isLeaf': file['type'] == 'blob',
                     'provider': provider,
```

### Comparing `orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/Cache.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,42 @@
 from orbit_component_base.src.orbit_orm import BaseTable, BaseCollection, register_class, register_method
 from orbit_component_zerodocs.doc_python import Documentation
 from orbit_database import SerialiserType, Doc
 from hashlib import md5
 from orbit_component_base.src.orbit_shared import world
 from loguru import logger as log
 from gitlab import Gitlab
-from gitlab.exceptions import GitlabHeadError
 from base64 import b64decode
 from asyncio import ensure_future
 from datetime import datetime
 from cmarkgfm import github_flavored_markdown_to_html
 from cmarkgfm.cmark import Options as opts
 from asyncio import ensure_future
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name, get_lexer_for_filename
 from pygments.formatters import HtmlFormatter
 from pygments.util import ClassNotFound
 from bs4 import BeautifulSoup
 from asyncio import get_running_loop as loop
 from orbit_component_zerodocs.schema.Project import ProjectTable
-from re import sub as substitute
-from nltk import word_tokenize
-from nltk.corpus import stopwords
-from collections import Counter
-from io import StringIO
-import tokenize
-
-STOP = set(stopwords.words('english'))
-STOP.add('none')
 
 gitlab = Gitlab()
-remove_whitespace = {ord('\r'): 32, ord('\n'): 32, ord('\t'): 32}
 
 
 class CacheTable (BaseTable):
 
     norm_table_name = 'cache'
     norm_auditing = True
     norm_codec = SerialiserType.UJSON
     norm_ensure = [
-        {'index_name': 'by_params'  , 'duplicates': False, 'func': '{root}|{provider}|{project}|{branch}|{path}'},
-        {'index_name': 'by_root'    , 'duplicates': True, 'func': '{root}|{path}'},
-        {'index_name': 'by_words'   , 'iwx': True }
+        {'index_name': 'by_params', 'duplicates': False, 'func': '{root}|{provider}|{project}|{branch}|{path}'},
+        {'index_name': 'by_root', 'duplicates': True, 'func': '{root}|{path}'}
     ]
 
     def _cache_path (self, name):
-        # log.warning(f"Construct: {self._provider}|{self._project}|{self._path}|{name}")
         return world.conf.tmp / md5(f'{self._provider}|{self._project}|{self._path}|{name}'.encode()).hexdigest()
 
     def from_cache (self, params):
         result = {'ok': True, 'loading': True, '_id': self.key, 'stamp': 0}
         for mode in params.get('modes', ['html']):
             try:
                 with open(self._cache_path(mode), 'r') as io:
@@ -74,116 +61,80 @@
             project = gitlab.projects.get(self._project_id)
             if not project:
                 raise Exception(f'unknown project id: {self._project_id}')
             data = project.files.get(self._path, ref=self._branch)
             if not data:
                 raise Exception(f'unable to find path: {self._provider}/{self._path}')
             self._badges = [(badge.rendered_link_url, badge.rendered_image_url) for badge in project.badges.list()]
-            self._prefix = project.web_url
             return b64decode(data.content) if data.encoding == 'base64' else data.content
         except Exception as e:
             log.exception(e)
 
     def thread_head (self):
         try:
             project = gitlab.projects.get(self._project_id)
             if not project:
                 raise Exception(f'unknown project id: {self._project_id}')
             data = project.files.head(self._path, ref=self._branch)
             if not data:
                 raise Exception(f'unable to find path: {self._provider}/{self._path}')
             return data
-        except GitlabHeadError:
-            log.error(f'Unable to find proj={self._project_id} prov={self._provider} path={self._path}')
         except Exception as e:
             log.exception(e)
 
+    # def from_id (self, root, provider, project, branch, path, transaction=None):
+    #     doc = Doc({'root': root, 'provider': provider, 'project': project, 'branch': branch, 'uri': id})
+    #     self.set(self.norm_tb.seek_one('by_params', doc, txn=transaction))
+    #     if not self.isValid:
+    #         self._root = root
+    #         self._provider = provider
+    #         self._project = project
+    #         self._branch = branch
+    #         self._path = path
+    #     return self
+
     def from_params (self, params, transaction=None):
         doc = Doc(params)
         self.set(self.norm_tb.seek_one('by_params', doc, txn=transaction))
         if not self.isValid:
             self.set(doc)
-            # log.error(f'Missing doc: {doc.doc}')
         return self
 
 
 @register_class
 class CacheCollection (BaseCollection):
 
     table_class = CacheTable
     table_methods = []
 
     MD_OPTIONS = (opts.CMARK_OPT_UNSAFE | opts.CMARK_OPT_LIBERAL_HTML_TAG | opts.CMARK_OPT_DEFAULT)
 
-    async def search (self, text):
-        ids = []
-        text = text.split(' ')
-        if not len(text):
-            return {'ok': True, 'count': 0}
-        
-        words = text[:-1]
-        matches = self.table_class().norm_tb.lexicon('by_words', text, 9999)
-        if len(matches):
-            word, count = matches[0]
-            words.append(word)
-
-        if not len(words):
-            return {'ok': True, 'count': 0}
-
-        count, results = self.table_class().norm_tb.match('by_words', words)
-        if not count:
-            return {'ok': True, 'count': 0}
-        
-        for oid in results:
-            ids.append(oid.decode())
-        
-        return {'ok': True, 'ids': ids, 'count': count, 'partial': words, 'matches': [word[0] for word in matches]}
-
-    async def local_update (self, params, text):
-        doc = self.table_class().from_params(params)
-        if doc.isValid:
-            return await self.update(doc, text)
-
     async def fetch (self, params, force=False):
         # log.error(f'Force={force}')
         doc = self.table_class().from_params(params)
-        if not doc.isValid:
-            ensure_future(self.check(doc))
+        ensure_future(self.check(doc))
         # log.success(f'Doc={doc.doc}, {doc.isValid}')
         if force:
             doc._etag = None
-        ret = doc.from_cache(params)
-        if doc.isValid and doc._refresh:
-            ensure_future(self.check(doc))
-        return ret
+        return doc.from_cache(params)
 
     async def update (self, doc, text):
         if text and isinstance(text, bytes): text = text.decode()
         with open(doc._cache_path('text'), 'w') as io:
             io.write(text)
         if doc._path.endswith('.md') or doc._label in ['LICENSE', 'README']:
             html = github_flavored_markdown_to_html(text, self.MD_OPTIONS)
             formatter = HtmlFormatter(style='manni')
             soup = BeautifulSoup(html, 'html.parser')
-            
-            text = " ".join(soup.get_text(separator=" ").translate(remove_whitespace).split()).strip()
-            text = word_tokenize(substitute(r'&\w+;\s?', '', substitute('[^0-9a-zA-Z]+', ' ', text).lower().strip()))
-            doc.words = Counter([word for word in filter(lambda word: len(word) > 1 and word not in STOP, text)])
-
             for tag in soup.find_all('pre'):
                 try:
                     lexer = get_lexer_by_name(tag.get('lang'), stripall=True)
                     tag.replace_with(BeautifulSoup(highlight(tag.find('code').text, lexer, formatter), 'html.parser'))
                 except ClassNotFound:
                     pass
-                
-            for tag in soup.find_all('img'):
-                src = tag.get('src')
-                if src.startswith('../'): src = src[3:]
-                tag['src'] = f"{doc._prefix}/-/raw/{doc._branch}/{src}"
             html = '<style>' + formatter.get_style_defs() + '</style>' + str(soup)
         else:
             try:
                 lexer = get_lexer_for_filename(doc._path, stripall=True)
             except ClassNotFound:
                 lexer = get_lexer_by_name('text', stripall=True)
 
@@ -192,58 +143,46 @@
 
         with open(doc._cache_path('html'), 'w') as io:
             io.write(html)
 
         if doc._path.endswith('.py'):
             index, html = Documentation().run(doc.key, text)
             doc._children = index
-            formatter = HtmlFormatter(style='manni')
+            formatter = HtmlFormatter(style='tango')
             soup = BeautifulSoup(html, 'html.parser')
-
             for tag in soup.find_all('pre'):
                 try:
                     lexer = get_lexer_for_filename(doc._path, stripall=True)
                     hlight = tag.find('code')
-                    if hlight:
-                        tag.replace_with(BeautifulSoup(highlight(hlight.text, lexer, formatter), 'html.parser'))
-                except ClassNotFound:
-                    pass
+                    try:
+                        if hlight:
+                            tag.replace_with(BeautifulSoup(hlight.text, lexer, formatter), 'html.parser')
+                    except AttributeError as e:
+                        log.error(str(e))
+                        log.error(f'Text> {hlight.text}')
                 except ClassNotFound:
                     pass
             html = '<style>' + formatter.get_style_defs() + '</style>' + str(soup)
 
             with open(doc._cache_path('api'), 'w') as io:
                 io.write(html)
                 doc._children = index
 
-            words = Counter()
-            with StringIO(text) as io:
-                tokens = tokenize.generate_tokens(io.readline)
-                for token in tokens:
-                    word = token.string.strip()
-                    if not word.startswith('"') and not word.startswith("'") and not word.startswith("#"):
-                        if len(word) > 1:
-                            words.update([word])
-                    for word in word.replace('"', '').replace("'", '').replace("\n", " ").replace('#', '').split(" "):
-                        if len(word) > 1 and word[0] >= '0' and word[0] <= 'z':
-                            words.update([word])
-            doc.words = words
-            print(words)
         doc.update({'stamp': datetime.now().timestamp()})
         doc.save() if doc.isValid else doc.append()
 
     async def check (self, doc):
         try:
             project = ProjectTable().from_params(doc)
             doc._project_id = project._project_id
             head = await doc.head()
             if head:
                 etag = head.get('Etag')
-                log.success(f'Etag={etag} Old={doc._etag}')
                 if etag == doc._etag and not doc._refresh:
+                    # log.debug(f'Serving "{doc._path}" from cache based on Etag')
                     return
                 log.warning(f"Check did an update, new etag={etag}, old={doc._etag}")
                 doc.update({'etag': etag, 'refresh': False})
                 text = await doc.fetch()
                 return await self.update(doc, text)
             else:
                 log.error(f'Unable to load file: {doc.doc}')
@@ -263,28 +202,26 @@
                     project = gitlab.projects.get(project_id)
                     for branch in project.branches.list():
                         branches.append(branch.name)
                     return {'ok': True, 'id': project_id, 'branches': branches }
             return {'ok': False, 'error': f'Project not found: {params.get("project")}'}
         raise Exception(f'unknown provider: {params.get("provider")}')
     
-    async def put (self, params):
-        old_data = params.get('old_data')
-        new_data = params.get('new_data')
+    async def put (self, old_data, new_data):
         # log.success(f'Create> {new_data}')
         # log.warning(f'Delete> {old_data}')
         for item in new_data:
             doc = self.table_class().from_params(item)
             if '_id' in doc:
                 doc.pop('_id')
             if 'children' in doc:
                 doc.pop('children')
 
-            # if '|' in item.get('key'):
-            #     item['key'] = item.get('key').split('|')[1]
+            if '|' in item.get('key'):
+                item['key'] = item.get('key').split('|')[1]
 
             if doc.isValid:
                 # log.debug(f'Update')
                 doc.update(item).save()
             else:
                 # log.debug(f'Append')
                 doc.update(item).append()
@@ -313,30 +250,17 @@
             if entry._provider != provider or entry._project != project or entry._root != root or entry._branch != branch:
                 break
             entry.delete()
 
     @register_method
     def get_ids(cls, session, params, transaction=None):
         ids, data = [], []
-        if 'ids' in params:
-            for id in params['ids']:
-                doc = cls.table_class().from_key(id)
-                if doc.isValid:
-                    session.append(params, doc.key, ids, data, doc, strip=cls.table_strip)
-        else:
-            duds = []
-            limit = Doc(params.get('filter'))
-            for result in cls().filter(index_name='by_root', lower=limit):
-                doc = result.doc
-                if doc._root != limit._root:
-                    break
-                if not doc._key:
-                    duds.append(doc.key)
-                    continue
-                session.append(params, result.oid.decode(), ids, data, doc, strip=cls.table_strip)
+        limit = Doc(params.get('filter'))
+        for result in cls().filter(index_name='by_root', lower=limit):
+            doc = result.doc
+            if doc._root != limit._root:
+                break
+            doc._key = f'{doc._branch}|{doc._key}'
+            session.append(params, result.oid.decode(), ids, data, doc, strip=cls.table_strip)
         session.update(ids, params)
-        if duds:
-            log.error(f'Excluded duds: {len(duds)}')
-            cls().delete(duds)
-            
         return {'ok': True, 'ids': ids, 'data': data}
```

### Comparing `orbit_component_zerodocs-1.0.17/orbit_component_zerodocs/schema/Project.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             log.debug(f'Append')
             doc.update(params).append()
         return {'ok': True}
 
     async def remove (self, params):
         doc = self.table_class().from_params(params)
         if not doc.isValid:
-            log.error(f"Project not found: {params}")
             return {'ok': False, 'error': f'Project entry not found: {id}'}
         doc.delete()
         return {'ok': True}
     
     @register_method
     def get_ids(cls, session, params, transaction=None):
         ids, data = [], []
```

### Comparing `orbit_component_zerodocs-1.0.17/pyproject.toml` & `orbit_component_zerodocs-1.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-zerodocs"
-version = "1.0.17"
+version = "1.0.9"
 description = "Orbit Component for inline documentation"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_zerodocs"}]
 classifiers = [
@@ -22,22 +22,21 @@
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-zerodocs"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-zerodocs/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-orbit-database = ">=1.0"
+orbit-database = "^0.99.91"
 loguru = "^0.7.0"
 pygments = "^2.15.1"
 bs4 = "^0.0.1"
 cmarkgfm = "^2022.10.27"
 python-gitlab = "^3.14.0"
-lxml = "^4.9.3"
-nltk = "^3.8.1"
+orbit-component-base = "^0.99.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `orbit_component_zerodocs-1.0.17/PKG-INFO` & `orbit_component_zerodocs-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-zerodocs
-Version: 1.0.17
+Version: 1.0.9
 Summary: Orbit Component for inline documentation
 Home-page: https://gitlab.com/madpenguin/orbit-component-zerodocs
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: cmarkgfm (>=2022.10.27,<2023.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: lxml (>=4.9.3,<5.0.0)
-Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: orbit-database (>=1.0)
+Requires-Dist: orbit-component-base (>=0.99.9,<0.100.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Description-Content-Type: text/markdown
 
 # Orbit Component :: ZeroDocs
```

