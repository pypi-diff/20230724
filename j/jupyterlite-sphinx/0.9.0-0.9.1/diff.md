# Comparing `tmp/jupyterlite_sphinx-0.9.0.tar.gz` & `tmp/jupyterlite_sphinx-0.9.1.tar.gz`

## Comparing `jupyterlite_sphinx-0.9.0.tar` & `jupyterlite_sphinx-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.css
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.js
--rw-r--r--   0        0        0    13888 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/LICENSE
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/README.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.css
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.js
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/LICENSE
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/README.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.1/PKG-INFO
```

### Comparing `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.css` & `jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.css`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.js` & `jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.py` & `jupyterlite_sphinx-0.9.1/jupyterlite_sphinx/jupyterlite_sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 from docutils.nodes import SkipNode, Element
 
 from sphinx.application import Sphinx
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.fileutil import copy_asset
 from sphinx.parsers import RSTParser
 
+try:
+    import voici
+except ImportError:
+    voici = None
+
 HERE = Path(__file__).parent
 
 CONTENT_DIR = "_contents"
 JUPYTERLITE_DIR = "lite"
-# Using a global variable, is there a better way?
-APPS = []
 
 
 # Used for nodes that do not need to be rendered
 def skip(self, node):
     raise SkipNode
 
 
@@ -192,17 +195,14 @@
         "toolbar": directives.unchanged,
         "theme": directives.unchanged,
         "prompt": directives.unchanged,
         "prompt_color": directives.unchanged,
     }
 
     def run(self):
-        if not "repl" in APPS:
-            APPS.append("repl")
-
         width = self.options.pop("width", "100%")
         height = self.options.pop("height", "100%")
 
         prompt = self.options.pop("prompt", False)
         prompt_color = self.options.pop("prompt_color", None)
 
         prefix = os.path.relpath(
@@ -285,55 +285,38 @@
     """The ``.. jupyterlite::`` directive.
 
     Renders a Notebook with JupyterLite in the docs.
     """
 
     iframe_cls = JupyterLiteIframe
 
-    def run(self):
-        if not "lab" in APPS:
-            APPS.append("lab")
-
-        return super().run()
-
 
 class RetroLiteDirective(_LiteDirective):
     """The ``.. retrolite::`` directive.
 
     Renders a Notebook with RetroLite in the docs.
     """
 
     iframe_cls = RetroLiteIframe
 
-    def run(self):
-        if not "retro" in APPS:
-            APPS.append("retro")
-
-        return super().run()
-
 
 class VoiciDirective(_LiteDirective):
     """The ``.. voici::`` directive.
 
     Renders a Notebook with Voici in the docs.
     """
 
     iframe_cls = VoiciIframe
 
     def run(self):
-        try:
-            import voici
-        except ImportError:
+        if voici is None:
             raise RuntimeError(
                 "Voici must be installed if you want to make use of the voici directive: pip install voici"
             )
 
-        if not "voici" in APPS:
-            APPS.append("voici")
-
         return super().run()
 
 
 class RetroLiteParser(RSTParser):
     """Sphinx source parser for Jupyter notebooks.
 
     Shows the Notebook using retrolite."""
@@ -389,30 +372,34 @@
             for match in glob.glob(pattern, recursive=True)
         ]
 
         contents = []
         for content in jupyterlite_contents:
             contents.extend(["--contents", content])
 
-        apps = []
-        for jlite_app in APPS:
-            apps.extend(["--apps", jlite_app])
+        voici_option = [] if voici is None else ["--apps", "voici"]
 
         command = [
             "jupyter",
             "lite",
             "build",
             "--debug",
             *config,
-            *apps,
             *contents,
             "--contents",
             os.path.join(app.srcdir, CONTENT_DIR),
             "--output-dir",
             os.path.join(app.outdir, JUPYTERLITE_DIR),
+            "--apps",
+            "lab",
+            "--apps",
+            "retro",
+            "--apps",
+            "repl",
+            *voici_option,
             "--lite-dir",
             jupyterlite_dir,
         ]
 
         subprocess.run(command, cwd=app.srcdir, check=True)
 
         print("[jupyterlite-sphinx] JupyterLite build done")
```

### Comparing `jupyterlite_sphinx-0.9.0/LICENSE` & `jupyterlite_sphinx-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.0/pyproject.toml` & `jupyterlite_sphinx-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.0/PKG-INFO` & `jupyterlite_sphinx-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite-sphinx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sphinx extension for deploying JupyterLite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
```

