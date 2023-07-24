# Comparing `tmp/langchain_plantuml-0.0.4.tar.gz` & `tmp/langchain_plantuml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_plantuml-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "langchain_plantuml-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `langchain_plantuml-0.0.4.tar` & `langchain_plantuml-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11356 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/LICENSE
--rw-r--r--   0        0        0     3006 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/README.md
--rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/__init__.py
--rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/__init__.py
--rw-r--r--   0        0        0     9487 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
--rw-r--r--   0        0        0    13343 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
--rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/core/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/core/plantuml_callback_handler.py
--rw-r--r--   0        0        0     1255 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/diagram.py
--rw-r--r--   0        0        0     1749 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3006 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/README.md
+-rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/__init__.py
+-rw-r--r--   0        0        0     9487 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
+-rw-r--r--   0        0        0    13343 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
+-rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/core/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/core/plantuml_callback_handler.py
+-rw-r--r--   0        0        0     1255 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/diagram.py
+-rw-r--r--   0        0        0     1749 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.5/PKG-INFO
```

### Comparing `langchain_plantuml-0.0.4/LICENSE` & `langchain_plantuml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/README.md` & `langchain_plantuml-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/__init__.py` & `langchain_plantuml-0.0.5/langchain_plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/__init__.py` & `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py` & `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py` & `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/core/__init__.py` & `langchain_plantuml-0.0.5/langchain_plantuml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/core/plantuml_callback_handler.py` & `langchain_plantuml-0.0.5/langchain_plantuml/core/plantuml_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/langchain_plantuml/diagram.py` & `langchain_plantuml-0.0.5/langchain_plantuml/diagram.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.4/pyproject.toml` & `langchain_plantuml-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 [build-system]
 requires = ["flit_core==3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "langchain-plantuml"
-version = "0.0.4"
+version = "0.0.5"
 description = "Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze."
 authors = [{ name = "Lei Zhang", email = "zhanglei@apache.org" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "langchain==0.0.228"
+    "langchain>=0.0.228"
 ]
 
 [tool.flit.module]
 name = "langchain_plantuml"
 
 [project.optional-dependencies]
 lint = [
```

### Comparing `langchain_plantuml-0.0.4/PKG-INFO` & `langchain_plantuml-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: langchain-plantuml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 Author-email: Lei Zhang <zhanglei@apache.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: langchain==0.0.228
+Requires-Dist: langchain>=0.0.228
 Requires-Dist: flake8==5.0.4 ; extra == "lint"
 Requires-Dist: pyproject-flake8==5.0.4 ; extra == "lint"
 Requires-Dist: isort>=5,<6 ; extra == "lint"
 Requires-Dist: black>=23,<24 ; extra == "lint"
 Requires-Dist: flit==3.9.0 ; extra == "package"
 Requires-Dist: openai==0.27.8 ; extra == "test"
 Requires-Dist: chromadb==0.3.26 ; extra == "test"
```

