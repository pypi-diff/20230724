# Comparing `tmp/pymtpng-1.0.tar.gz` & `tmp/pymtpng-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymtpng-1.0.tar", last modified: Mon Jun 12 23:19:50 2023, max compression
+gzip compressed data, was "pymtpng-1.0.1.tar", last modified: Mon Jul 24 19:33:51 2023, max compression
```

## Comparing `pymtpng-1.0.tar` & `pymtpng-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:19:50.093278 pymtpng-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:19:50.089278 pymtpng-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:19:50.093278 pymtpng-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-12 23:19:38.000000 pymtpng-1.0/.github/workflows/pypi-packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 23:19:38.000000 pymtpng-1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-12 23:19:38.000000 pymtpng-1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 23:19:38.000000 pymtpng-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-12 23:19:50.093278 pymtpng-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 23:19:38.000000 pymtpng-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-12 23:19:38.000000 pymtpng-1.0/mtpng.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-06-12 23:19:38.000000 pymtpng-1.0/pymtpng.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:19:50.093278 pymtpng-1.0/pymtpng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-12 23:19:50.000000 pymtpng-1.0/pymtpng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 23:19:50.000000 pymtpng-1.0/pymtpng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:19:50.000000 pymtpng-1.0/pymtpng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 23:19:50.000000 pymtpng-1.0/pymtpng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 23:19:38.000000 pymtpng-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:19:50.093278 pymtpng-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 23:19:38.000000 pymtpng-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:19:50.093278 pymtpng-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-12 23:19:38.000000 pymtpng-1.0/tests/test_mtpng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:51.294373 pymtpng-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:51.286373 pymtpng-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:51.290373 pymtpng-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 19:33:39.000000 pymtpng-1.0.1/.github/workflows/pypi-packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 19:33:39.000000 pymtpng-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-24 19:33:39.000000 pymtpng-1.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 19:33:39.000000 pymtpng-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 19:33:51.294373 pymtpng-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 19:33:39.000000 pymtpng-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-24 19:33:39.000000 pymtpng-1.0.1/mtpng.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-07-24 19:33:39.000000 pymtpng-1.0.1/pymtpng.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:51.294373 pymtpng-1.0.1/pymtpng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 19:33:51.000000 pymtpng-1.0.1/pymtpng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 19:33:51.000000 pymtpng-1.0.1/pymtpng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:33:51.000000 pymtpng-1.0.1/pymtpng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:33:51.000000 pymtpng-1.0.1/pymtpng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 19:33:39.000000 pymtpng-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:33:51.294373 pymtpng-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 19:33:39.000000 pymtpng-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:51.294373 pymtpng-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 19:33:39.000000 pymtpng-1.0.1/tests/test_mtpng.py
```

### Comparing `pymtpng-1.0/.github/workflows/pypi-packages.yml` & `pymtpng-1.0.1/.github/workflows/pypi-packages.yml`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0/CMakeLists.txt` & `pymtpng-1.0.1/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 cmake_minimum_required(VERSION 3.16)
 project(pymtpng CXX)
 
 include(FetchContent)
 
+if(WIN32)
+  # Prevent pybind11 from sharing resources with other, potentially ABI incompatible modules
+  # https://github.com/pybind/pybind11/issues/2898
+  add_definitions(-DPYBIND11_COMPILER_TYPE="_${PROJECT_NAME}_abi")
+endif()
+
 # Fetch pybind11 library
 FetchContent_Declare(
   pybind11
   GIT_REPOSITORY https://github.com/pybind/pybind11
-  GIT_TAG        v2.10.4
+  GIT_TAG        v2.11.1
   GIT_SHALLOW    True
 )
 FetchContent_MakeAvailable(pybind11)
 
 # Fetch mtpng source
 FetchContent_Declare(
   mtpng
```

### Comparing `pymtpng-1.0/LICENSE` & `pymtpng-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0/PKG-INFO` & `pymtpng-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymtpng
-Version: 1.0
+Version: 1.0.1
 Summary: Python bindings for MTPNG library
 Home-page: https://github.com/pwuertz/pymtpng
 Author: Peter Würtz
 Author-email: pwuertz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymtpng-1.0/README.md` & `pymtpng-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0/mtpng.hpp` & `pymtpng-1.0.1/mtpng.hpp`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0/pymtpng.cpp` & `pymtpng-1.0.1/pymtpng.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "mtpng.hpp"
 
 
 using namespace std::string_view_literals;
 namespace py = pybind11;
 
-constexpr auto VERSION = "1.0"sv;
+constexpr auto VERSION = "1.0.1"sv;
 
 using stringv_map = std::map<std::string_view, std::string_view>;
 
 using np_uint8_array_t = py::array_t<uint8_t, py::array::c_style>;
 using np_uint16_array_t = py::array_t<uint16_t, py::array::c_style>;
 
 using write_fn_t = std::function<size_t(const uint8_t* bytes, const size_t len)>;
```

### Comparing `pymtpng-1.0/pymtpng.egg-info/PKG-INFO` & `pymtpng-1.0.1/pymtpng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymtpng
-Version: 1.0
+Version: 1.0.1
 Summary: Python bindings for MTPNG library
 Home-page: https://github.com/pwuertz/pymtpng
 Author: Peter Würtz
 Author-email: pwuertz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymtpng-1.0/setup.py` & `pymtpng-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = pathlib.Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type="text/markdown"
 
 setup(
     name="pymtpng",
-    version="1.0",
+    version="1.0.1",
     author="Peter Würtz",
     author_email="pwuertz@gmail.com",
     url="https://github.com/pwuertz/pymtpng",
     description="Python bindings for MTPNG library",
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     ext_modules=[CMakeExtension(
```

### Comparing `pymtpng-1.0/tests/test_mtpng.py` & `pymtpng-1.0.1/tests/test_mtpng.py`

 * *Files identical despite different names*

