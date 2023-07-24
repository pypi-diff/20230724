# Comparing `tmp/render_engine_tailwindcss-2023.1.2a2.tar.gz` & `tmp/render_engine_tailwindcss-2023.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_tailwindcss-2023.1.2a2.tar", last modified: Wed Feb 22 05:30:59 2023, max compression
+gzip compressed data, was "render_engine_tailwindcss-2023.7.1a2.tar", last modified: Mon Jul 24 05:08:46 2023, max compression
```

## Comparing `render_engine_tailwindcss-2023.1.2a2.tar` & `render_engine_tailwindcss-2023.7.1a2.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-22 05:30:59.384261 render_engine_tailwindcss-2023.1.2a2/
--rw-r--r--   0 jaymiller   (501) staff       (20)     1067 2023-01-22 04:33:07.000000 render_engine_tailwindcss-2023.1.2a2/LICENSE
--rw-r--r--   0 jaymiller   (501) staff       (20)     1606 2023-02-22 05:30:59.383818 render_engine_tailwindcss-2023.1.2a2/PKG-INFO
--rw-r--r--   0 jaymiller   (501) staff       (20)     1240 2023-01-22 18:50:54.000000 render_engine_tailwindcss-2023.1.2a2/README.md
--rw-r--r--   0 jaymiller   (501) staff       (20)      598 2023-02-22 05:30:39.000000 render_engine_tailwindcss-2023.1.2a2/pyproject.toml
--rw-r--r--   0 jaymiller   (501) staff       (20)       38 2023-02-22 05:30:59.384308 render_engine_tailwindcss-2023.1.2a2/setup.cfg
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-22 05:30:59.377281 render_engine_tailwindcss-2023.1.2a2/src/
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-22 05:30:59.380187 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss/
--rw-r--r--   0 jaymiller   (501) staff       (20)       33 2023-01-22 00:46:13.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss/__init__.py
--rw-r--r--   0 jaymiller   (501) staff       (20)     1033 2023-02-22 05:29:12.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss/plugins.py
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-22 05:30:59.382839 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/
--rw-r--r--   0 jaymiller   (501) staff       (20)     1606 2023-02-22 05:30:59.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/PKG-INFO
--rw-r--r--   0 jaymiller   (501) staff       (20)      403 2023-02-22 05:30:59.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/SOURCES.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)        1 2023-02-22 05:30:59.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/dependency_links.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)       54 2023-02-22 05:30:59.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/requires.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)       26 2023-02-22 05:30:59.000000 render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/top_level.txt
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-22 05:30:59.383321 render_engine_tailwindcss-2023.1.2a2/tests/
--rw-r--r--   0 jaymiller   (501) staff       (20)     1914 2023-01-23 12:29:00.000000 render_engine_tailwindcss-2023.1.2a2/tests/test_css_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-24 05:08:45.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 05:08:46.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:08:45.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 05:08:45.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 05:08:45.000000 render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:08:46.012564 render_engine_tailwindcss-2023.7.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 05:08:31.000000 render_engine_tailwindcss-2023.7.1a2/tests/test_css_files.py
```

### Comparing `render_engine_tailwindcss-2023.1.2a2/LICENSE` & `render_engine_tailwindcss-2023.7.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine_tailwindcss-2023.1.2a2/PKG-INFO` & `render_engine_tailwindcss-2023.7.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine_tailwindcss
-Version: 2023.1.2a2
+Version: 2023.7.1a2
 Summary: tailwindcss-parser for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_tailwindcss/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_tailwindcss/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_tailwindcss-2023.1.2a2/README.md` & `render_engine_tailwindcss-2023.7.1a2/README.md`

 * *Files identical despite different names*

### Comparing `render_engine_tailwindcss-2023.1.2a2/pyproject.toml` & `render_engine_tailwindcss-2023.7.1a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+local_scheme = "no-local-version"
+
 [project]
 name = "render_engine_tailwindcss"
-version = "2023.1.2a2"
+dynamic = ["version"]
 description = "tailwindcss-parser for Render Engine"
 readme = "README.md"
 
 dependencies = ["render-engine>=2023.1.3a1", "pytailwindcss"]
 
 [project.optional-dependencies]
 dev = ["pytest"]
```

### Comparing `render_engine_tailwindcss-2023.1.2a2/src/render_engine_tailwindcss.egg-info/PKG-INFO` & `render_engine_tailwindcss-2023.7.1a2/src/render_engine_tailwindcss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine-tailwindcss
-Version: 2023.1.2a2
+Version: 2023.7.1a2
 Summary: tailwindcss-parser for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_tailwindcss/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_tailwindcss/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_tailwindcss-2023.1.2a2/tests/test_css_files.py` & `render_engine_tailwindcss-2023.7.1a2/tests/test_css_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pathlib
-import dataclasses
-
-import pytest
+import logging
 
 from render_engine_tailwindcss.plugins import parse_css_files
 
 css_text = """
 @tailwind base;
 @tailwind components;
 @tailwind utilities;
@@ -17,19 +15,24 @@
     static_path = tmp_path.joinpath("static")
     static_path.mkdir()
 
     static_path.joinpath("style1.css").write_text(css_text)
     static_path.joinpath("style2.css").write_text(css_text)
 
     # Create an output folder
-    output_path = tmp_path.joinpath("output")
-
+    output_path = tmp_path / "output"
+    logging.info(f"{static_path=}, {output_path=}")
+    result_path = output_path.joinpath("/" / static_path)
+    logging.info(f"{result_path=}")
     # Create a site object
-    parse_css_files(static_path, output_path) 
-    assert len(list(output_path.joinpath('static').iterdir())) == 2
+    parse_css_files(
+        static_path=static_path,
+        output_path=output_path,
+    ) 
+    assert len(list(pathlib.Path(output_path).joinpath("static").iterdir())) ==2
 
 
 def test_files_are_recursive(tmp_path):
     """Tests that each .css file creates a corresponding .css file in the output directory."""
     static_path = tmp_path.joinpath("static")
     static_path2 = static_path.joinpath("pre")
     static_path.mkdir()
@@ -39,15 +42,15 @@
     static_path2.joinpath("style2.css").write_text(css_text)
 
     # Create an output folder
     output_path = tmp_path.joinpath("output")
     
     # Create a site object
     parse_css_files(static_path, output_path) 
-    assert len(list(output_path.glob("*.css"))) == 1
+    assert len(list(output_path.rglob("*.css"))) == 2
     assert len(list(pathlib.Path(output_path / "static" / "pre").glob("*.css"))) == 1
 
 
 def test_non_css_files_are_ignored(tmp_path):
     """Tests that non .css files are ignored."""
     static_path = tmp_path.joinpath("static")
     output_path = tmp_path.joinpath("output")
```

