# Comparing `tmp/pyfeyn2-2.3.4.tar.gz` & `tmp/pyfeyn2-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.3.4.tar", max compression
+gzip compressed data, was "pyfeyn2-2.3.5.tar", max compression
```

## Comparing `pyfeyn2-2.3.4.tar` & `pyfeyn2-2.3.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-07-21 11:06:02.341584 pyfeyn2-2.3.4/LICENSE
--rw-r--r--   0        0        0     3115 2023-07-21 11:06:02.341584 pyfeyn2-2.3.4/README.md
--rw-r--r--   0        0        0      154 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2838 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      647 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/diagram.py
--rw-r--r--   0        0        0      768 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     3068 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0     3336 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2734 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      279 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0     2911 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3626 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3596 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5926 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1617 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     7120 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     7036 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13245 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41394 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12740 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     9146 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     8914 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      863 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2364 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1701 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     2114 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      527 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3850 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1976 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2630 2023-07-21 11:06:04.625616 pyfeyn2-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.4/setup.py
--rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 07:08:04.637394 pyfeyn2-2.3.5/LICENSE
+-rw-r--r--   0        0        0     3115 2023-07-24 07:08:04.641394 pyfeyn2-2.3.5/README.md
+-rw-r--r--   0        0        0      154 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2838 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      647 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/diagram.py
+-rw-r--r--   0        0        0      768 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0    10564 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0     3279 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2734 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      279 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2924 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3626 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5926 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1617 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     7120 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7036 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12740 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9146 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     8914 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2114 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3850 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2630 2023-07-24 07:08:07.933416 pyfeyn2-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.5/setup.py
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.5/PKG-INFO
```

### Comparing `pyfeyn2-2.3.4/LICENSE` & `pyfeyn2-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/README.md` & `pyfeyn2-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/auto/bend.py` & `pyfeyn2-2.3.5/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/auto/diagram.py` & `pyfeyn2-2.3.5/pyfeyn2/auto/diagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/auto/label.py` & `pyfeyn2-2.3.5/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.3.5/pyfeyn2/feynmandiagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Moved to :py:mod:`feynml`"""
 from importlib.metadata import version
 
-from feynml.connector import Connector as Connector_
-from feynml.feynmandiagram import FeynmanDiagram as FeynmanDiagram_
-from feynml.feynml import FeynML as FeynML_
-from feynml.head import Head as Head_
-
 # from feynml.feynml import Tool as Tool_
-from feynml.leg import Leg as Leg_
-from feynml.meta import Meta as Meta_
-from feynml.momentum import Momentum as Momentum_
-from feynml.pdgid import PDG as PDG_
-from feynml.point import Point as Point_
-from feynml.propagator import Propagator as Propagator_
-from feynml.styled import Styled as Styled_
-from feynml.vertex import Vertex as Vertex_
+from feynml import PDG as PDG_
+from feynml import Connector as Connector_
+from feynml import FeynmanDiagram as FeynmanDiagram_
+from feynml import FeynML as FeynML_
+from feynml import Head as Head_
+from feynml import Leg as Leg_
+from feynml import Meta as Meta_
+from feynml import Point as Point_
+from feynml import Propagator as Propagator_
+from feynml import Styled as Styled_
+from feynml import Vertex as Vertex_
+from feynml.momentum import Momentum as Momentum_  # TODO fix to feynml only
 from smpl_doc import doc
 
 
 class Head(Head_):
     class Meta(Head_.Meta):
         pass
```

### Comparing `pyfeyn2-2.3.4/pyfeyn2/interface/dot.py` & `pyfeyn2-2.3.5/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/mkfeyndiag.py` & `pyfeyn2-2.3.5/pyfeyn2/mkfeyndiag.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     return c
 
 
 def renderer_from_string(s):
     return class_for_name(".".join(s.split(".")[0:-1]), s.split(".")[-1])
 
 
-def main():
+def main(argv=None):
     # parse command line options with argparse
     parser = argparse.ArgumentParser(
         prog="pyfeyn2.mkfeyndiag",
         description="Draw FeynML diagrams with pyfeyn2.",
     )
     parser.add_argument(
         "input",
@@ -68,15 +68,15 @@
         "--diagram",
         metavar="DIAGRAM",
         default=None,
         type=str,
         help="Diagram id to render.",
     )
 
-    args = parser.parse_args()
+    args = parser.parse_args(argv)
 
     arenderer = args.renderer
     renderer = None
     if arenderer is None:
         pass
     elif arenderer.lower() == "ascii":
         renderer = ASCIIRender
```

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/all.py` & `pyfeyn2-2.3.5/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.3.5/pyfeyn2/render/latex/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.3.5/pyfeyn2/render/latex/feynmp.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.3.5/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.3.5/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.3.5/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.3.5/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/lines.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/pyxrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.3.5/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/render.py` & `pyfeyn2-2.3.5/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/label.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/line.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/point.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/point.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/style.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.3.5/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.4/pyproject.toml` & `pyfeyn2-2.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.3.4"
+version = "2.3.5"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -25,15 +25,15 @@
 ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 cssselect ="*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
-feynml = {version = ">=0.1.6", extras = ["interfaces"]}
+feynml = {version = ">=0.2.8", extras = ["interfaces"]}
 #feynml= {path= "../feynml", develop = true, extras = ["interfaces"]}
 
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pyfeyn2-2.3.4/setup.py` & `pyfeyn2-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['Wand',
  'cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'dot2tex',
  'feynman>=2.0,<3.0',
- 'feynml[interfaces]>=0.1.6',
+ 'feynml[interfaces]>=0.2.8',
  'graphviz',
  'ipyparallel',
  'matplotlib>=1.4.0,<4.0.0',
  'numpy>=1.6,<1.24',
  'particle',
  'pydot',
  'pygments',
@@ -39,15 +39,15 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.3.4',
+    'version': '2.3.5',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.3.4/PKG-INFO` & `pyfeyn2-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.3.4
+Version: 2.3.5
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 Requires-Dist: Wand
 Requires-Dist: cssselect
 Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: dot2tex
 Requires-Dist: feynman (>=2.0,<3.0)
-Requires-Dist: feynml[interfaces] (>=0.1.6)
+Requires-Dist: feynml[interfaces] (>=0.2.8)
 Requires-Dist: graphviz
 Requires-Dist: ipyparallel
 Requires-Dist: matplotlib (>=1.4.0,<4.0.0)
 Requires-Dist: numpy (>=1.6,<1.24)
 Requires-Dist: particle
 Requires-Dist: pydot
 Requires-Dist: pygments
```

