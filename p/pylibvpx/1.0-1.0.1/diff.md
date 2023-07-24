# Comparing `tmp/pylibvpx-1.0.tar.gz` & `tmp/pylibvpx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibvpx-1.0.tar", last modified: Mon Jun 12 22:35:26 2023, max compression
+gzip compressed data, was "pylibvpx-1.0.1.tar", last modified: Mon Jul 24 20:01:13 2023, max compression
```

## Comparing `pylibvpx-1.0.tar` & `pylibvpx-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:35:26.266349 pylibvpx-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 22:35:00.000000 pylibvpx-1.0/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-12 22:35:00.000000 pylibvpx-1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 22:35:00.000000 pylibvpx-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-12 22:35:26.266349 pylibvpx-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 22:35:00.000000 pylibvpx-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-12 22:35:00.000000 pylibvpx-1.0/pylibvpx.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:35:26.262349 pylibvpx-1.0/pylibvpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-12 22:35:26.000000 pylibvpx-1.0/pylibvpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 22:35:26.000000 pylibvpx-1.0/pylibvpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:35:26.000000 pylibvpx-1.0/pylibvpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 22:35:26.000000 pylibvpx-1.0/pylibvpx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 22:35:00.000000 pylibvpx-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:35:26.266349 pylibvpx-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 22:35:00.000000 pylibvpx-1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxcommon.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxcommon_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxdecoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxdecoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxencoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-12 22:35:00.000000 pylibvpx-1.0/vpxencoder.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:01:13.051897 pylibvpx-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 20:01:13.051897 pylibvpx-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/pylibvpx.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:01:13.051897 pylibvpx-1.0.1/pylibvpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 20:01:13.000000 pylibvpx-1.0.1/pylibvpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-24 20:01:13.000000 pylibvpx-1.0.1/pylibvpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:01:13.000000 pylibvpx-1.0.1/pylibvpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 20:01:13.000000 pylibvpx-1.0.1/pylibvpx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:01:13.051897 pylibvpx-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxcommon.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxcommon_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxdecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxdecoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxencoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 20:00:47.000000 pylibvpx-1.0.1/vpxencoder.hpp
```

### Comparing `pylibvpx-1.0/CMakeLists.txt` & `pylibvpx-1.0.1/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.16)
-project(pylibvpx LANGUAGES CXX VERSION "1.0")
+project(pylibvpx LANGUAGES CXX VERSION "1.0.1")
 
 # Default to Release build type
 if (NOT CMAKE_BUILD_TYPE OR CMAKE_BUILD_TYPE STREQUAL "")
   set(CMAKE_BUILD_TYPE "Release" CACHE STRING "" FORCE)
 endif()
 
 # Fetch conan.cmake
@@ -12,14 +12,20 @@
 if(NOT EXISTS "${CMAKE_BINARY_DIR}/conan.cmake")
   message(STATUS "Downloading conan.cmake from https://github.com/conan-io/cmake-conan")
   file(DOWNLOAD "https://raw.githubusercontent.com/conan-io/cmake-conan/0.18.1/conan.cmake"
        "${CMAKE_BINARY_DIR}/conan.cmake" TLS_VERIFY ON)
 endif()
 include(${CMAKE_BINARY_DIR}/conan.cmake)
 
+if(WIN32)
+  # Prevent pybind11 from sharing resources with other, potentially ABI incompatible modules
+  # https://github.com/pybind/pybind11/issues/2898
+  add_definitions(-DPYBIND11_COMPILER_TYPE="_${PROJECT_NAME}_abi")
+endif()
+
 # Get pybind11 and libvpx from conan
 conan_cmake_configure(
   REQUIRES pybind11/2.10.4 libvpx/1.11.0
   GENERATORS cmake_find_package
 )
 conan_cmake_autodetect(settings)
 if (CMAKE_CXX_COMPILER_ID MATCHES "MSVC")
```

### Comparing `pylibvpx-1.0/LICENSE` & `pylibvpx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibvpx-1.0/pylibvpx.cpp` & `pylibvpx-1.0.1/pylibvpx.cpp`

 * *Files identical despite different names*

### Comparing `pylibvpx-1.0/setup.py` & `pylibvpx-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = pathlib.Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type="text/markdown"
 
 setup(
     name="pylibvpx",
-    version="1.0",
+    version="1.0.1",
     author="Peter Würtz",
     author_email="pwuertz@gmail.com",
     url="https://github.com/pwuertz/libvpx-bindings",
     description="Python bindings for libvpx",
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     ext_modules=[CMakeExtension(
```

### Comparing `pylibvpx-1.0/vpxcommon_impl.hpp` & `pylibvpx-1.0.1/vpxcommon_impl.hpp`

 * *Files identical despite different names*

### Comparing `pylibvpx-1.0/vpxdecoder.cpp` & `pylibvpx-1.0.1/vpxdecoder.cpp`

 * *Files identical despite different names*

### Comparing `pylibvpx-1.0/vpxencoder.cpp` & `pylibvpx-1.0.1/vpxencoder.cpp`

 * *Files identical despite different names*

### Comparing `pylibvpx-1.0/vpxencoder.hpp` & `pylibvpx-1.0.1/vpxencoder.hpp`

 * *Files identical despite different names*

