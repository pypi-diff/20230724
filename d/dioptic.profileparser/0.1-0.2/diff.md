# Comparing `tmp/dioptic.profileparser-0.1.tar.gz` & `tmp/dioptic.profileparser-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptic.profileparser-0.1.tar", last modified: Sat Jun 17 01:02:53 2023, max compression
+gzip compressed data, was "dioptic.profileparser-0.2.tar", last modified: Mon Jul 24 19:43:37 2023, max compression
```

## Comparing `dioptic.profileparser-0.1.tar` & `dioptic.profileparser-0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.006757 dioptic.profileparser-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/.github/workflows/pypi-packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)   154785 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/cpp/peglib.h
--rw-r--r--   0 runner    (1001) docker     (123)    28701 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/cpp/processprofile.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/dioptic.profileparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 01:02:52.000000 dioptic.profileparser-0.1/dioptic.profileparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-17 01:02:53.000000 dioptic.profileparser-0.1/dioptic.profileparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:02:52.000000 dioptic.profileparser-0.1/dioptic.profileparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 01:02:52.000000 dioptic.profileparser-0.1/dioptic.profileparser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/js/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/js/profile_parser_js.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/python/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/python/pyprofileparser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:02:53.010757 dioptic.profileparser-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-17 01:02:41.000000 dioptic.profileparser-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.565196 dioptic.profileparser-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.561196 dioptic.profileparser-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.561196 dioptic.profileparser-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/.github/workflows/pypi-packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-24 19:43:37.565196 dioptic.profileparser-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.561196 dioptic.profileparser-0.2/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)   154785 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/cpp/peglib.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28701 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/cpp/processprofile.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.561196 dioptic.profileparser-0.2/dioptic.profileparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-24 19:43:37.000000 dioptic.profileparser-0.2/dioptic.profileparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 19:43:37.000000 dioptic.profileparser-0.2/dioptic.profileparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:43:37.000000 dioptic.profileparser-0.2/dioptic.profileparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:43:37.000000 dioptic.profileparser-0.2/dioptic.profileparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.565196 dioptic.profileparser-0.2/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/js/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/js/profile_parser_js.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:37.565196 dioptic.profileparser-0.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/python/pyprofileparser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:43:37.565196 dioptic.profileparser-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 19:43:23.000000 dioptic.profileparser-0.2/setup.py
```

### Comparing `dioptic.profileparser-0.1/.github/workflows/pypi-packages.yml` & `dioptic.profileparser-0.2/.github/workflows/pypi-packages.yml`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/.gitlab-ci.yml` & `dioptic.profileparser-0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/LICENSE` & `dioptic.profileparser-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/cpp/peglib.h` & `dioptic.profileparser-0.2/cpp/peglib.h`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/cpp/processprofile.hpp` & `dioptic.profileparser-0.2/cpp/processprofile.hpp`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/js/CMakeLists.txt` & `dioptic.profileparser-0.2/js/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/js/profile_parser_js.cpp` & `dioptic.profileparser-0.2/js/profile_parser_js.cpp`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.1/python/pyprofileparser.cpp` & `dioptic.profileparser-0.2/python/pyprofileparser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include "pybind11/pybind11.h"
 #include "pybind11/stl.h"
 #include "../cpp/processprofile.hpp"
 
 using namespace std::string_view_literals;
 namespace py = pybind11;
 
-constexpr auto VERSION = "0.1"sv;
+constexpr auto VERSION = "0.2"sv;
 
 struct Convert {
     // Profile data types to python conversion
     // TODO: pybind11 converts all basic types -> add converters for custom types only
 
     template<typename T>
     static inline py::object to_py(const std::shared_ptr<T>& v)
```

### Comparing `dioptic.profileparser-0.1/setup.py` & `dioptic.profileparser-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = pathlib.Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type="text/markdown"
 
 setup(
     name="dioptic.profileparser",
-    version="0.1",
+    version="0.2",
     author="Peter Würtz",
     author_email="pwuertz@gmail.com",
     url="https://github.com/dioptic/profileparser",
     description="Parser library for ARGOS declarative profiles.",
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     #namespace_packages=["dioptic"],
```

