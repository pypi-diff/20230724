# Comparing `tmp/SloppyV3-0.0.0.0.20230724.2.tar.gz` & `tmp/SloppyV3-0.0.0.0.20230724.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SloppyV3-0.0.0.0.20230724.2.tar", last modified: Mon Jul 24 02:21:13 2023, max compression
+gzip compressed data, was "SloppyV3-0.0.0.0.20230724.3.tar", last modified: Mon Jul 24 05:45:32 2023, max compression
```

## Comparing `SloppyV3-0.0.0.0.20230724.2.tar` & `SloppyV3-0.0.0.0.20230724.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 02:21:13.408101 SloppyV3-0.0.0.0.20230724.2/
--rw-r--r--   0 h2noda     (501) staff       (20)      328 2023-07-24 02:21:13.407720 SloppyV3-0.0.0.0.20230724.2/PKG-INFO
--rw-r--r--   0 h2noda     (501) staff       (20)       58 2023-02-03 02:12:55.000000 SloppyV3-0.0.0.0.20230724.2/README.md
-drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 02:21:13.404859 SloppyV3-0.0.0.0.20230724.2/SloppyV3/
--rw-r--r--   0 h2noda     (501) staff       (20)    11152 2023-07-24 02:20:39.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3/common.py
--rw-r--r--   0 h2noda     (501) staff       (20)      377 2023-07-03 09:25:52.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3/database.py
--rw-r--r--   0 h2noda     (501) staff       (20)     1123 2023-02-07 00:53:47.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3/error.py
--rw-r--r--   0 h2noda     (501) staff       (20)     5486 2023-07-03 09:30:44.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3/excel.py
-drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 02:21:13.407170 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/
--rw-r--r--   0 h2noda     (501) staff       (20)      328 2023-07-24 02:21:13.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/PKG-INFO
--rw-r--r--   0 h2noda     (501) staff       (20)      253 2023-07-24 02:21:13.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/SOURCES.txt
--rw-r--r--   0 h2noda     (501) staff       (20)        1 2023-07-24 02:21:13.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/dependency_links.txt
--rw-r--r--   0 h2noda     (501) staff       (20)       67 2023-07-24 02:21:13.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/requires.txt
--rw-r--r--   0 h2noda     (501) staff       (20)       64 2023-07-24 02:21:13.000000 SloppyV3-0.0.0.0.20230724.2/SloppyV3.egg-info/top_level.txt
--rw-r--r--   0 h2noda     (501) staff       (20)       38 2023-07-24 02:21:13.408281 SloppyV3-0.0.0.0.20230724.2/setup.cfg
--rw-r--r--   0 h2noda     (501) staff       (20)     1186 2023-07-24 02:20:51.000000 SloppyV3-0.0.0.0.20230724.2/setup.py
+drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 05:45:32.762636 SloppyV3-0.0.0.0.20230724.3/
+-rw-r--r--   0 h2noda     (501) staff       (20)      328 2023-07-24 05:45:32.762226 SloppyV3-0.0.0.0.20230724.3/PKG-INFO
+-rw-r--r--   0 h2noda     (501) staff       (20)       58 2023-02-03 02:12:55.000000 SloppyV3-0.0.0.0.20230724.3/README.md
+drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 05:45:32.758872 SloppyV3-0.0.0.0.20230724.3/SloppyV3/
+-rw-r--r--   0 h2noda     (501) staff       (20)    11152 2023-07-24 02:20:39.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3/common.py
+-rw-r--r--   0 h2noda     (501) staff       (20)      377 2023-07-03 09:25:52.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3/database.py
+-rw-r--r--   0 h2noda     (501) staff       (20)     1123 2023-02-07 00:53:47.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3/error.py
+-rw-r--r--   0 h2noda     (501) staff       (20)     5749 2023-07-24 05:44:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3/excel.py
+drwxr-xr-x   0 h2noda     (501) staff       (20)        0 2023-07-24 05:45:32.761550 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/
+-rw-r--r--   0 h2noda     (501) staff       (20)      328 2023-07-24 05:45:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/PKG-INFO
+-rw-r--r--   0 h2noda     (501) staff       (20)      253 2023-07-24 05:45:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/SOURCES.txt
+-rw-r--r--   0 h2noda     (501) staff       (20)        1 2023-07-24 05:45:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/dependency_links.txt
+-rw-r--r--   0 h2noda     (501) staff       (20)       67 2023-07-24 05:45:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/requires.txt
+-rw-r--r--   0 h2noda     (501) staff       (20)       64 2023-07-24 05:45:32.000000 SloppyV3-0.0.0.0.20230724.3/SloppyV3.egg-info/top_level.txt
+-rw-r--r--   0 h2noda     (501) staff       (20)       38 2023-07-24 05:45:32.762853 SloppyV3-0.0.0.0.20230724.3/setup.cfg
+-rw-r--r--   0 h2noda     (501) staff       (20)     1186 2023-07-24 05:45:03.000000 SloppyV3-0.0.0.0.20230724.3/setup.py
```

### Comparing `SloppyV3-0.0.0.0.20230724.2/SloppyV3/common.py` & `SloppyV3-0.0.0.0.20230724.3/SloppyV3/common.py`

 * *Files identical despite different names*

### Comparing `SloppyV3-0.0.0.0.20230724.2/SloppyV3/error.py` & `SloppyV3-0.0.0.0.20230724.3/SloppyV3/error.py`

 * *Files identical despite different names*

### Comparing `SloppyV3-0.0.0.0.20230724.2/SloppyV3/excel.py` & `SloppyV3-0.0.0.0.20230724.3/SloppyV3/excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,28 +42,29 @@
 
     def SideStyle(border_style=borders.NONE, color="000000"):
         side = Side(border_style=border_style, color=color)
         return side
 
     @dataclass
     class CellStyle:
+        # #000000 #FFFFFF
         # row: int
         # column: int
         # cellvalue: str = None
         font: Font = Font(
             name="D2Coding",
             size="10",
             color="000000",
             underline=None,
             bold=False,
             italic=False,
             strikethrough=False,
         )
         alignment: Alignment = Alignment(horizontal="center", vertical="center")
-        side: Side(border_style=borders.NONE, color="000000")
+        side: Side = Side(border_style=borders.NONE, color="000000")
         border: Border = Border(left=side, right=side, top=side, bottom=side)
         fill: PatternFill = PatternFill(
             fill_type="solid", start_color=None, end_color=None
         )
 
         def set_font(
             name="D2Coding",
@@ -89,14 +90,20 @@
             alignment = Alignment(horizontal=horizontal, vertical=vertical)
             return alignment
 
         def set_side(border_style=borders.BORDER_NONE, color="000000") -> Side:
             side = Side(border_style=border_style, color=color)
             return side
 
+        def set_patternfill(
+            type="solid", sbgcolor="000000", ebgcolor="000000"
+        ) -> PatternFill:
+            fill = PatternFill(type="solid", start_color=sbgcolor, end_color=ebgcolor)
+            return fill
+
         # def set_border()
 
     def set_font(
         fontname="D2Coding",
         fontsize="10",
         fontcolor="000000",
         fontunderline=None,
```

### Comparing `SloppyV3-0.0.0.0.20230724.2/setup.py` & `SloppyV3-0.0.0.0.20230724.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="SloppyV3",
-    version="0.0.0.0.20230724.2",
+    version="0.0.0.0.20230724.3",
     author="Chungman Kim",
     author_email="h2noda@gmail.com",
     description="Python module - SloppyV3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "beautifulsoup4",
```

