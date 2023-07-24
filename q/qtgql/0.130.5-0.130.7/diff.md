# Comparing `tmp/qtgql-0.130.5.tar.gz` & `tmp/qtgql-0.130.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.130.5.tar", max compression
+gzip compressed data, was "qtgql-0.130.7.tar", max compression
```

## Comparing `qtgql-0.130.5.tar` & `qtgql-0.130.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-23 19:15:21.979142 qtgql-0.130.5/LICENSE
--rw-r--r--   0        0        0     1116 2023-07-23 19:15:21.979142 qtgql-0.130.5/README.md
--rw-r--r--   0        0        0     4337 2023-07-23 19:15:56.455094 qtgql-0.130.5/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-23 19:16:00.155086 qtgql-0.130.5/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     2116 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3393 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1216 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3855 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16149 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4441 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2208 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4600 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0     2019 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3629 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2985 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1137 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4791 2023-07-23 19:15:21.991142 qtgql-0.130.5/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4157 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5052 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     6692 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18386 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1579 2023-07-23 19:15:21.995142 qtgql-0.130.5/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.130.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 05:26:15.207449 qtgql-0.130.7/LICENSE
+-rw-r--r--   0        0        0     1116 2023-07-24 05:26:15.207449 qtgql-0.130.7/README.md
+-rw-r--r--   0        0        0     4337 2023-07-24 05:26:43.023320 qtgql-0.130.7/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-24 05:26:43.827318 qtgql-0.130.7/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     2116 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3393 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1216 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3855 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16149 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4441 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2208 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4600 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0     2019 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3629 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2985 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1137 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4791 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4157 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5052 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     6692 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18386 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1579 2023-07-24 05:26:15.219449 qtgql-0.130.7/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.130.7/PKG-INFO
```

### Comparing `qtgql-0.130.5/LICENSE` & `qtgql-0.130.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/README.md` & `qtgql-0.130.7/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/pyproject.toml` & `qtgql-0.130.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.130.5"
+version = "0.130.7"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.130.5/qtgqlcodegen/cli.py` & `qtgql-0.130.7/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/config.py` & `qtgql-0.130.7/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/core/cppref.py` & `qtgql-0.130.7/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.130.7/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/core/template.py` & `qtgql-0.130.7/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/generator.py` & `qtgql-0.130.7/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/operation/definitions.py` & `qtgql-0.130.7/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.130.7/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.130.7/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/operation/template.py` & `qtgql-0.130.7/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/operation/utils.py` & `qtgql-0.130.7/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/schema/definitions.py` & `qtgql-0.130.7/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.130.7/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/schema/template.py` & `qtgql-0.130.7/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/CMakeLists.jinja.cmake` & `qtgql-0.130.7/qtgqlcodegen/templates/CMakeLists.jinja.cmake`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.130.7/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.130.7/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.130.7/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/types.py` & `qtgql-0.130.7/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/qtgqlcodegen/utils.py` & `qtgql-0.130.7/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.5/PKG-INFO` & `qtgql-0.130.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.130.5
+Version: 0.130.7
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

