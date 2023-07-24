# Comparing `tmp/editables-0.4.tar.gz` & `tmp/editables-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editables-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "editables-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `editables-0.4.tar` & `editables-0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1072 2021-04-08 16:24:47.187184 editables-0.4/LICENSE.txt
--rw-r--r--   0        0        0     1996 2022-04-09 15:49:08.690254 editables-0.4/README.md
--rw-r--r--   0        0        0      658 2022-04-09 15:49:08.691217 editables-0.4/docs/Makefile
--rwxr-xr-x   0        0        0      799 2022-04-09 15:49:08.692220 editables-0.4/docs/make.bat
--rw-r--r--   0        0        0       27 2022-04-09 15:49:08.692220 editables-0.4/docs/requirements.txt
--rw-r--r--   0        0        0     1957 2023-07-06 14:58:12.743793 editables-0.4/docs/source/conf.py
--rw-r--r--   0        0        0     6485 2023-06-29 15:09:33.531062 editables-0.4/docs/source/implementation.md
--rw-r--r--   0        0        0      427 2023-07-06 14:57:18.057853 editables-0.4/docs/source/index.md
--rw-r--r--   0        0        0     4707 2023-07-06 14:57:18.106888 editables-0.4/docs/source/usage.md
--rw-r--r--   0        0        0     5962 2023-07-06 14:57:18.111892 editables-0.4/docs/source/use-cases.md
--rw-r--r--   0        0        0     1304 2023-07-06 14:58:12.742811 editables-0.4/pyproject.toml
--rw-r--r--   0        0        0     3645 2023-07-06 14:58:12.742811 editables-0.4/src/editables/__init__.py
--rw-r--r--   0        0        0     1122 2023-06-28 16:25:44.327179 editables-0.4/src/editables/redirector.py
--rw-r--r--   0        0        0       76 2023-06-28 12:32:00.757014 editables-0.4/tests/requirements.txt
--rw-r--r--   0        0        0     5070 2023-06-29 15:09:33.532063 editables-0.4/tests/test_editable.py
--rw-r--r--   0        0        0     2130 2021-06-12 11:40:39.885457 editables-0.4/tests/test_redirects.py
--rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 editables-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-04-08 16:24:47.187184 editables-0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1996 2022-04-09 15:49:08.690254 editables-0.5/README.md
+-rw-r--r--   0        0        0      658 2022-04-09 15:49:08.691217 editables-0.5/docs/Makefile
+-rwxr-xr-x   0        0        0      799 2022-04-09 15:49:08.692220 editables-0.5/docs/make.bat
+-rw-r--r--   0        0        0       27 2022-04-09 15:49:08.692220 editables-0.5/docs/requirements.txt
+-rw-r--r--   0        0        0     1957 2023-07-24 18:24:48.387946 editables-0.5/docs/source/conf.py
+-rw-r--r--   0        0        0     6485 2023-06-29 15:09:33.531062 editables-0.5/docs/source/implementation.md
+-rw-r--r--   0        0        0      427 2023-07-06 14:57:18.057853 editables-0.5/docs/source/index.md
+-rw-r--r--   0        0        0     4707 2023-07-06 14:57:18.106888 editables-0.5/docs/source/usage.md
+-rw-r--r--   0        0        0     5962 2023-07-06 14:57:18.111892 editables-0.5/docs/source/use-cases.md
+-rw-r--r--   0        0        0     1326 2023-07-24 18:24:48.387425 editables-0.5/pyproject.toml
+-rw-r--r--   0        0        0     3645 2023-07-24 18:24:48.386392 editables-0.5/src/editables/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 13:47:17.334124 editables-0.5/src/editables/py.typed
+-rw-r--r--   0        0        0     1487 2023-07-24 18:23:20.448231 editables-0.5/src/editables/redirector.py
+-rw-r--r--   0        0        0       76 2023-06-28 12:32:00.757014 editables-0.5/tests/requirements.txt
+-rw-r--r--   0        0        0     5070 2023-06-29 15:09:33.532063 editables-0.5/tests/test_editable.py
+-rw-r--r--   0        0        0     2357 2023-07-24 18:23:20.453198 editables-0.5/tests/test_redirects.py
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 editables-0.5/PKG-INFO
```

### Comparing `editables-0.4/LICENSE.txt` & `editables-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `editables-0.4/README.md` & `editables-0.5/README.md`

 * *Files identical despite different names*

### Comparing `editables-0.4/docs/Makefile` & `editables-0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `editables-0.4/docs/make.bat` & `editables-0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `editables-0.4/docs/source/conf.py` & `editables-0.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "editables"
 copyright = "2021, Paul Moore"
 author = "Paul Moore"
 
 # The full version, including alpha/beta/rc tags
-release = "0.4"
+release = "0.5"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `editables-0.4/docs/source/implementation.md` & `editables-0.5/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `editables-0.4/docs/source/usage.md` & `editables-0.5/docs/source/usage.md`

 * *Files identical despite different names*

### Comparing `editables-0.4/docs/source/use-cases.md` & `editables-0.5/docs/source/use-cases.md`

 * *Files identical despite different names*

### Comparing `editables-0.4/pyproject.toml` & `editables-0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "editables"
-version = "0.4"
+version = "0.5"
 description = "Editable installations"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [{name = "Paul Moore", email = "p.f.moore@gmail.com"}]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Libraries",
   "Topic :: Utilities",
+  "Typing :: Typed",
 ]
 dependencies = []
 
 [project.urls]
 Documentation = "https://editables.readthedocs.io"
 Source = "https://github.com/pfmoore/editables"
 Tracker = "https://github.com/pfmoore/editables/issues"
```

### Comparing `editables-0.4/src/editables/__init__.py` & `editables-0.5/src/editables/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Iterable, List, Tuple, Union
 
 __all__ = (
     "EditableProject",
     "__version__",
 )
 
-__version__ = "0.4"
+__version__ = "0.5"
 
 
 # Check if a project name is valid, based on PEP 426:
 # https://peps.python.org/pep-0426/#name
 def is_valid(name: str) -> bool:
     return (
         re.match(r"^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", name, re.IGNORECASE)
```

### Comparing `editables-0.4/src/editables/redirector.py` & `editables-0.5/src/editables/redirector.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,7 +33,15 @@
     @classmethod
     def install(cls) -> None:
         for f in sys.meta_path:
             if f == cls:
                 break
         else:
             sys.meta_path.append(cls)
+
+    @classmethod
+    def invalidate_caches(cls) -> None:
+        # importlib.invalidate_caches calls finders' invalidate_caches methods,
+        # and since we install this meta path finder as a class rather than an instance,
+        # we have to override the inherited invalidate_caches method (using self)
+        # as a classmethod instead
+        pass
```

### Comparing `editables-0.4/tests/test_editable.py` & `editables-0.5/tests/test_editable.py`

 * *Files identical despite different names*

### Comparing `editables-0.4/tests/test_redirects.py` & `editables-0.5/tests/test_redirects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import importlib
 import sys
 
 from editables.redirector import RedirectingFinder as F
 
 
 @contextlib.contextmanager
 def save_import_state():
@@ -77,7 +78,14 @@
         assert mod.val == 42
         import pkg
 
         assert pkg.val == 42
         import pkg.sub
 
         assert pkg.sub.val == 42
+
+
+def test_cache_invalidation():
+    F.install()
+    # assert that the finder matches importlib's expectations
+    # see https://github.com/pfmoore/editables/issues/31
+    importlib.invalidate_caches()
```

### Comparing `editables-0.4/PKG-INFO` & `editables-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: editables
-Version: 0.4
+Version: 0.5
 Summary: Editable installations
 Author-email: Paul Moore <p.f.moore@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Project-URL: Documentation, https://editables.readthedocs.io
 Project-URL: Source, https://github.com/pfmoore/editables
 Project-URL: Tracker, https://github.com/pfmoore/editables/issues
 
 # A Python library for creating "editable wheels"
 
 This library supports the building of wheels which, when installed, will
```

