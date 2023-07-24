# Comparing `tmp/rst-to-myst-0.3.4.tar.gz` & `tmp/rst_to_myst-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst-to-myst-0.3.4.tar", last modified: Mon Jan 16 23:29:26 2023, max compression
+gzip compressed data, was "rst_to_myst-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rst-to-myst-0.3.4.tar` & `rst_to_myst-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       66 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/.gitattributes
--rw-r--r--   0        0        0     1744 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/.gitignore
--rw-r--r--   0        0        0      710 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      174 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/.readthedocs.yml
--rw-r--r--   0        0        0     1069 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/LICENSE
--rw-r--r--   0        0        0     2464 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/README.md
--rw-r--r--   0        0        0      609 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/docs/source/api.rst
--rw-r--r--   0        0        0       97 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/docs/source/cli.rst
--rw-r--r--   0        0        0     1360 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/docs/source/conf.py
--rw-r--r--   0        0        0     1145 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/docs/source/index.md
--rw-r--r--   0        0        0     4804 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/docs/source/usage.md
--rw-r--r--   0        0        0     1490 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      219 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/rst_to_myst/__init__.py
--rw-r--r--   0        0        0    11307 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/rst_to_myst/cli.py
--rw-r--r--   0        0        0        0 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/rst_to_myst/data/__init__.py
--rw-r--r--   0        0        0     7405 2023-01-16 23:29:20.420723 rst-to-myst-0.3.4/rst_to_myst/data/directives.yml
--rw-r--r--   0        0        0    37675 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/inliner.py
--rw-r--r--   0        0        0    25379 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/markdownit.py
--rw-r--r--   0        0        0     9019 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/mdformat_render.py
--rw-r--r--   0        0        0     8868 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/namespace.py
--rw-r--r--   0        0        0     1134 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/nodes.py
--rw-r--r--   0        0        0     7716 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/parser.py
--rw-r--r--   0        0        0    17826 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/states.py
--rw-r--r--   0        0        0     1169 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/rst_to_myst/utils.py
--rw-r--r--   0        0        0      601 2023-01-16 23:29:20.424723 rst-to-myst-0.3.4/tox.ini
--rw-r--r--   0        0        0     3840 1970-01-01 00:00:00.000000 rst-to-myst-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1744 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/.gitignore
+-rw-r--r--   0        0        0      710 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      174 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1069 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2464 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/README.md
+-rw-r--r--   0        0        0      162 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/codecov.yml
+-rw-r--r--   0        0        0      609 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/docs/source/api.rst
+-rw-r--r--   0        0        0       97 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/docs/source/cli.rst
+-rw-r--r--   0        0        0     1360 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1145 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/docs/source/index.md
+-rw-r--r--   0        0        0     4804 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/docs/source/usage.md
+-rw-r--r--   0        0        0     1516 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/__init__.py
+-rw-r--r--   0        0        0    11305 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/cli.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/data/__init__.py
+-rw-r--r--   0        0        0     7405 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/data/directives.yml
+-rw-r--r--   0        0        0    37674 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/inliner.py
+-rw-r--r--   0        0        0    25378 2023-07-24 18:07:35.410006 rst_to_myst-0.4.0/rst_to_myst/markdownit.py
+-rw-r--r--   0        0        0     9019 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/mdformat_render.py
+-rw-r--r--   0        0        0     8865 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/namespace.py
+-rw-r--r--   0        0        0     1136 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/nodes.py
+-rw-r--r--   0        0        0     7716 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/parser.py
+-rw-r--r--   0        0        0    17825 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/states.py
+-rw-r--r--   0        0        0      494 2023-07-24 18:07:35.414006 rst_to_myst-0.4.0/rst_to_myst/utils.py
+-rw-r--r--   0        0        0      573 2023-07-24 18:07:35.418007 rst_to_myst-0.4.0/tox.ini
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 rst_to_myst-0.4.0/PKG-INFO
```

### Comparing `rst-to-myst-0.3.4/.gitignore` & `rst_to_myst-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/.pre-commit-config.yaml` & `rst_to_myst-0.4.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     exclude: |
         (?x)^(
             tests/fixtures/.*
         )$
   - id: check-yaml
   - id: check-toml
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
   - id: python-check-blanket-noqa
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.7.0
   hooks:
   - id: black
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
```

### Comparing `rst-to-myst-0.3.4/LICENSE` & `rst_to_myst-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/README.md` & `rst_to_myst-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/docs/source/api.rst` & `rst_to_myst-0.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/docs/source/conf.py` & `rst_to_myst-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/docs/source/index.md` & `rst_to_myst-0.4.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/docs/source/usage.md` & `rst_to_myst-0.4.0/docs/source/usage.md`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/pyproject.toml` & `rst_to_myst-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,38 +17,39 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 readme = "README.md"
 keywords = ["restructuredtext","markdown", "myst"]
 
 requires-python=">=3.7"
 dependencies=[
-    "docutils>=0.15,<0.18",
+    "docutils>=0.17,<0.20",
     "importlib_resources~=3.1;python_version<'3.9'",
     "pyyaml",
-    "markdown-it-py~=1.0",
-    "mdformat~=0.7.6",
-    "mdformat-myst~=0.1.4",
-    "mdformat-deflist~=0.1.0",
+    "markdown-it-py~=2.0",
+    "mdformat~=0.7.16",
+    "mdformat-myst~=0.1.5",
+    "mdformat-deflist~=0.1.2",
     "click>=7.1,<9"
 ]
 
 [project.urls]
 Home = "https://github.com/executablebooks/rst-to-myst"
 Documentation = "https://rst-to-myst.readthedocs.io"
 
 [project.scripts]
 rst2myst = "rst_to_myst.cli:main"
 
 [project.optional-dependencies]
-sphinx = ["sphinx>=3.2,<5"]
+sphinx = ["sphinx>=5,<7"]
 test = [
     "pytest~=6.0",
     "coverage",
     "pytest-cov",
-    "pytest-regressions"
+    "pytest-regressions",
+    "pytest-param-files",
 ]
 docs = [
     "myst-parser",
     "sphinx-book-theme",
     "sphinx-click",
     "sphinx-design"
 ]
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/cli.py` & `rst_to_myst-0.4.0/rst_to_myst/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         try:
             with path.open("r") as handle:
                 data = yaml.safe_load(handle)
         except Exception as exc:
             raise click.BadOptionUsage(
                 "--conversions", f"Error reading conversions file: {exc}", ctx
             )
-    if not isinstance(value, Mapping):
-        raise click.BadOptionUsage("--conversions", f"Not a mapping: {value!r}", ctx)
+    if not isinstance(data, Mapping):
+        raise click.BadOptionUsage("--conversions", f"Not a mapping: {data!r}", ctx)
     return data
 
 
 OPT_CONVERSIONS = click.option(
     "--conversions",
     "-c",
     default=None,
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/data/directives.yml` & `rst_to_myst-0.4.0/rst_to_myst/data/directives.yml`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/rst_to_myst/inliner.py` & `rst_to_myst-0.4.0/rst_to_myst/inliner.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         return regexp
 
 
 class Regexes:
     """Initialise and store compiled regexes."""
 
     def __init__(self, start_string_prefix: str, end_string_suffix: str):
-
         # Define inline object recognitions
         # ---------------------------------
         non_whitespace_before = r"(?<!\s)"
         non_whitespace_escape_before = r"(?<![\s\x00])"
         non_unescaped_whitespace_escape_before = r"(?<!(?<!\x00)[\s\x00])"
         non_whitespace_after = r"(?!\s)"
         # Alphanumerics with isolated internal [-._+:] chars (i.e. not 2 together):
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/markdownit.py` & `rst_to_myst-0.4.0/rst_to_myst/markdownit.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,14 @@
         # each body row should have the full amount of columns
         for row in tbody.children:
             if len(row.children) != ncolumns:
                 return False
         return True
 
     def visit_table(self, node):
-
         if not self.parse_gfm_table(node):
             text = node.rawsource
             if not text.endswith("\n"):
                 text += "\n"
             self.add_token(
                 "fence", "code", 0, content=text, markup="```", info="{eval-rst}"
             )
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/mdformat_render.py` & `rst_to_myst-0.4.0/rst_to_myst/mdformat_render.py`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/rst_to_myst/namespace.py` & `rst_to_myst-0.4.0/rst_to_myst/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         if domain not in self.domains:
             raise KeyError(f"domain {domain} not yet registered")
         self.domains[domain].roles[name] = role
 
     # additional methods
 
     def get_element(self, attr: str, name: str):
-
         # convert to standardised name
         canonicalname = name.lower()
         # try translation
         if self.language_module is not None:
             try:
                 canonicalname = getattr(self.language_module, attr)[canonicalname]
             except (AttributeError, KeyError):
@@ -214,20 +213,18 @@
     from sphinx.application import builtin_extensions
     from sphinx.errors import ExtensionError
     from sphinx.extension import Extension
     from sphinx.registry import EXTENSION_BLACKLIST
 
     LOCK.acquire()
     try:
-
         directives._directives = app.directives
         roles._roles = app.roles
 
         for extname in chain(builtin_extensions, extensions):
-
             if extname in app.extensions or extname in EXTENSION_BLACKLIST:
                 continue
 
             try:
                 mod = import_module(extname)
             except ImportError as err:
                 raise ImportError(f"Could not import extension {extname}", err) from err
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/nodes.py` & `rst_to_myst-0.4.0/rst_to_myst/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
         self,
         rawsource,
         *,
         name: str,
         module: str,
         conversion: str,
         options_list: List[Tuple[str, Any]],
-        **kwargs
+        **kwargs,
     ) -> None:
         super().__init__(
             rawsource,
             name=name,
             module=module,
             conversion=conversion,
             options_list=options_list,
-            **kwargs
+            **kwargs,
         )
 
 
 class ArgumentNode(nodes.Element):
     """The parsed argument of a directive."""
```

### Comparing `rst-to-myst-0.3.4/rst_to_myst/parser.py` & `rst_to_myst-0.4.0/rst_to_myst/parser.py`

 * *Files identical despite different names*

### Comparing `rst-to-myst-0.3.4/rst_to_myst/states.py` & `rst_to_myst-0.4.0/rst_to_myst/states.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,14 @@
         )
 
         blank_finish = blank_finish or self.state_machine.is_next_line_blank()
 
         return block_text, indented, indent, lineno, line_offset, blank_finish
 
     def parse_directive_block(self, indented, line_offset, directive):
-
         if indented and not indented[0].strip():
             indented.trim_start()
             line_offset += 1
 
         while indented and not indented[-1].strip():
             indented.trim_end()
```

### Comparing `rst-to-myst-0.3.4/tox.ini` & `rst_to_myst-0.4.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [tox]
 envlist = py38
 
 [testenv]
 usedevelop = true
 
 [testenv:py{37,38,39,310,311}]
-deps =
-    black
-    flake8
 extras =
     sphinx
     test
 commands = pytest {posargs}
 
 [testenv:cli]
 extras = sphinx
```

### Comparing `rst-to-myst-0.3.4/PKG-INFO` & `rst_to_myst-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: rst-to-myst
-Version: 0.3.4
+Version: 0.4.0
 Summary: Convert RST to MyST-Markdown.
 Keywords: restructuredtext,markdown,myst
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: docutils>=0.15,<0.18
+Requires-Dist: docutils>=0.17,<0.20
 Requires-Dist: importlib_resources~=3.1;python_version<'3.9'
 Requires-Dist: pyyaml
-Requires-Dist: markdown-it-py~=1.0
-Requires-Dist: mdformat~=0.7.6
-Requires-Dist: mdformat-myst~=0.1.4
-Requires-Dist: mdformat-deflist~=0.1.0
+Requires-Dist: markdown-it-py~=2.0
+Requires-Dist: mdformat~=0.7.16
+Requires-Dist: mdformat-myst~=0.1.5
+Requires-Dist: mdformat-deflist~=0.1.2
 Requires-Dist: click>=7.1,<9
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: sphinx-book-theme ; extra == "docs"
 Requires-Dist: sphinx-click ; extra == "docs"
 Requires-Dist: sphinx-design ; extra == "docs"
-Requires-Dist: sphinx>=3.2,<5 ; extra == "sphinx"
+Requires-Dist: sphinx>=5,<7 ; extra == "sphinx"
 Requires-Dist: pytest~=6.0 ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-regressions ; extra == "test"
+Requires-Dist: pytest-param-files ; extra == "test"
 Project-URL: Documentation, https://rst-to-myst.readthedocs.io
 Project-URL: Home, https://github.com/executablebooks/rst-to-myst
 Provides-Extra: docs
 Provides-Extra: sphinx
 Provides-Extra: test
 
 # rst-to-myst
```

