# Comparing `tmp/recometrics-0.1.6.post8.tar.gz` & `tmp/recometrics-0.1.6.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recometrics-0.1.6.post8.tar", last modified: Tue Jul 18 19:52:20 2023, max compression
+gzip compressed data, was "recometrics-0.1.6.post9.tar", last modified: Mon Jul 24 16:44:38 2023, max compression
```

## Comparing `recometrics-0.1.6.post8.tar` & `recometrics-0.1.6.post9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post8/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post8/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       99 2023-07-18 19:49:29.000000 recometrics-0.1.6.post8/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/recometrics/
--rw-r--r--   0 david     (1000) david     (1000)    38717 2023-07-03 18:56:28.000000 recometrics-0.1.6.post8/recometrics/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     2269 2023-07-18 19:51:03.000000 recometrics-0.1.6.post8/recometrics/wrapper.h
--rw-r--r--   0 david     (1000) david     (1000)    27792 2023-07-18 19:48:20.000000 recometrics-0.1.6.post8/recometrics/wrapper.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/recometrics.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      371 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       26 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    13598 2023-07-18 19:48:02.000000 recometrics-0.1.6.post8/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/src/
--rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post8/src/recometrics.hpp
--rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post8/src/recometrics_instantiated.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post8/src/recometrics_signatures.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post9/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       99 2023-07-18 19:49:29.000000 recometrics-0.1.6.post9/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/recometrics/
+-rw-r--r--   0 david     (1000) david     (1000)    38717 2023-07-03 18:56:28.000000 recometrics-0.1.6.post9/recometrics/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     2269 2023-07-18 19:51:03.000000 recometrics-0.1.6.post9/recometrics/wrapper.h
+-rw-r--r--   0 david     (1000) david     (1000)    27792 2023-07-18 19:48:20.000000 recometrics-0.1.6.post9/recometrics/wrapper.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/recometrics.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-24 16:44:38.000000 recometrics-0.1.6.post9/recometrics.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      371 2023-07-24 16:44:38.000000 recometrics-0.1.6.post9/recometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-24 16:44:38.000000 recometrics-0.1.6.post9/recometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       26 2023-07-24 16:44:38.000000 recometrics-0.1.6.post9/recometrics.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-24 16:44:38.000000 recometrics-0.1.6.post9/recometrics.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    13653 2023-07-24 16:43:52.000000 recometrics-0.1.6.post9/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-24 16:44:38.767694 recometrics-0.1.6.post9/src/
+-rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post9/src/recometrics.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post9/src/recometrics_instantiated.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post9/src/recometrics_signatures.hpp
```

### Comparing `recometrics-0.1.6.post8/LICENSE` & `recometrics-0.1.6.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/MANIFEST.in` & `recometrics-0.1.6.post9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/recometrics/__init__.py` & `recometrics-0.1.6.post9/recometrics/__init__.py`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/recometrics/wrapper.h` & `recometrics-0.1.6.post9/recometrics/wrapper.h`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/recometrics/wrapper.pyx` & `recometrics-0.1.6.post9/recometrics/wrapper.pyx`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/setup.py` & `recometrics-0.1.6.post9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 except AttributeError:
     EXIT_SUCCESS = 0
 
 class build_ext_subclass( build_ext ):
     def build_extensions(self):
         is_msvc = self.compiler.compiler_type == "msvc"
         is_clang = hasattr(self.compiler, 'compiler_cxx') and ("clang++" in self.compiler.compiler_cxx)
+        is_windows = sys.platform[:3].lower() == "win"
 
         compiler = self.compiler.compiler_type
         if is_msvc:
             for e in self.extensions:
                 e.extra_compile_args += ['/O2', '/openmp', '/GL', '/std:c++14', '/fp:contract', '/fp:except-']
         else:
             if not self.check_for_variable_dont_set_march() and not self.check_cflags_contain_arch():
@@ -280,15 +281,15 @@
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 
 setup(
     name  = "recometrics",
     packages = ["recometrics"],
-    version = '0.1.6-8',
+    version = '0.1.6-9',
     cmdclass = {'build_ext': build_ext_subclass},
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/recometrics',
     install_requires = ['numpy', 'scipy', 'cython', 'pandas'],
     description = 'Library-agnostic evaluation framework for implicit-feedback recommender systems',
     ext_modules = [
         Extension("recometrics.cpp_funs",
```

### Comparing `recometrics-0.1.6.post8/src/recometrics.hpp` & `recometrics-0.1.6.post9/src/recometrics.hpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/src/recometrics_instantiated.cpp` & `recometrics-0.1.6.post9/src/recometrics_instantiated.cpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post8/src/recometrics_signatures.hpp` & `recometrics-0.1.6.post9/src/recometrics_signatures.hpp`

 * *Files identical despite different names*

