# Comparing `tmp/lzokay-1.1.3.tar.gz` & `tmp/lzokay-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzokay-1.1.3.tar", last modified: Thu Jul 13 17:43:36 2023, max compression
+gzip compressed data, was "lzokay-1.1.4.tar", last modified: Mon Jul 24 18:57:33 2023, max compression
```

## Comparing `lzokay-1.1.3.tar` & `lzokay-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/.github/
--rw-rw-rw-   0        0        0      730 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/.github/workflows/
--rw-rw-rw-   0        0        0      618 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/workflows/dependabot.yml
--rw-rw-rw-   0        0        0     4572 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/workflows/python.yml
--rw-rw-rw-   0        0        0     1992 2023-07-13 17:41:58.000000 lzokay-1.1.3/.gitignore
--rw-rw-rw-   0        0        0       96 2023-07-13 17:41:58.000000 lzokay-1.1.3/.gitmodules
--rw-rw-rw-   0        0        0      432 2023-07-13 17:41:58.000000 lzokay-1.1.3/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1108 2023-07-13 17:41:58.000000 lzokay-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-13 17:41:58.000000 lzokay-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      786 2023-07-13 17:43:36.973441 lzokay-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-07-13 17:41:58.000000 lzokay-1.1.3/README.md
--rw-rw-rw-   0        0        0   438357 2023-07-13 17:43:34.000000 lzokay-1.1.3/_lzokay.cpp
--rw-rw-rw-   0        0        0     2329 2023-07-13 17:41:58.000000 lzokay-1.1.3/_lzokay.pyx
--rw-rw-rw-   0        0        0      541 2023-07-13 17:41:58.000000 lzokay-1.1.3/lzokay_wrap.pxd
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.942191 lzokay-1.1.3/native/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/native/lzokay/
--rw-rw-rw-   0        0        0       41 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/.git
--rw-rw-rw-   0        0        0     1705 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/CMakeLists.txt
--rw-rw-rw-   0        0        0      111 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/Config.cmake.in
--rw-rw-rw-   0        0        0     1097 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/LICENSE
--rw-rw-rw-   0        0        0     1892 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/native/lzokay/lzokay-c/
--rw-rw-rw-   0        0        0      204 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/CMakeLists.txt
--rw-rw-rw-   0        0        0     1084 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.cpp
--rw-rw-rw-   0        0        0      566 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.h
--rw-rw-rw-   0        0        0    21184 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay.cpp
--rw-rw-rw-   0        0        0     2558 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay.hpp
--rw-rw-rw-   0        0        0     1305 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/test.cpp
--rw-rw-rw-   0        0        0     1455 2023-07-13 17:41:58.000000 lzokay-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      137 2023-07-13 17:43:36.973441 lzokay-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     5173 2023-07-13 17:41:58.000000 lzokay-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.942191 lzokay-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/src/lzokay/
--rw-rw-rw-   0        0        0      275 2023-07-13 17:41:58.000000 lzokay-1.1.3/src/lzokay/__init__.py
--rw-rw-rw-   0        0        0      164 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay/version.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/src/lzokay.egg-info/
--rw-rw-rw-   0        0        0      786 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/tests/
--rw-rw-rw-   0        0        0      493 2023-07-13 17:41:58.000000 lzokay-1.1.3/tests/test_native.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/.github/
+-rw-rw-rw-   0        0        0      730 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/.github/workflows/
+-rw-rw-rw-   0        0        0      618 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/workflows/dependabot.yml
+-rw-rw-rw-   0        0        0     4572 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/workflows/python.yml
+-rw-rw-rw-   0        0        0     1992 2023-07-24 18:55:58.000000 lzokay-1.1.4/.gitignore
+-rw-rw-rw-   0        0        0       96 2023-07-24 18:55:58.000000 lzokay-1.1.4/.gitmodules
+-rw-rw-rw-   0        0        0      432 2023-07-24 18:55:58.000000 lzokay-1.1.4/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1108 2023-07-24 18:55:58.000000 lzokay-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-24 18:55:58.000000 lzokay-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      786 2023-07-24 18:57:33.831189 lzokay-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-24 18:55:58.000000 lzokay-1.1.4/README.md
+-rw-rw-rw-   0        0        0   438217 2023-07-24 18:57:31.000000 lzokay-1.1.4/_lzokay.cpp
+-rw-rw-rw-   0        0        0     2329 2023-07-24 18:55:58.000000 lzokay-1.1.4/_lzokay.pyx
+-rw-rw-rw-   0        0        0      541 2023-07-24 18:55:58.000000 lzokay-1.1.4/lzokay_wrap.pxd
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.815564 lzokay-1.1.4/native/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/native/lzokay/
+-rw-rw-rw-   0        0        0       41 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/.git
+-rw-rw-rw-   0        0        0     1705 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/CMakeLists.txt
+-rw-rw-rw-   0        0        0      111 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/Config.cmake.in
+-rw-rw-rw-   0        0        0     1097 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/native/lzokay/lzokay-c/
+-rw-rw-rw-   0        0        0      204 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1084 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.cpp
+-rw-rw-rw-   0        0        0      566 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.h
+-rw-rw-rw-   0        0        0    21184 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay.cpp
+-rw-rw-rw-   0        0        0     2558 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay.hpp
+-rw-rw-rw-   0        0        0     1305 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/test.cpp
+-rw-rw-rw-   0        0        0     1495 2023-07-24 18:55:58.000000 lzokay-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      137 2023-07-24 18:57:33.831189 lzokay-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-07-24 18:55:58.000000 lzokay-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.815564 lzokay-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/src/lzokay/
+-rw-rw-rw-   0        0        0      275 2023-07-24 18:55:58.000000 lzokay-1.1.4/src/lzokay/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay/version.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/src/lzokay.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/tests/
+-rw-rw-rw-   0        0        0      493 2023-07-24 18:55:58.000000 lzokay-1.1.4/tests/test_native.py
```

### Comparing `lzokay-1.1.3/.github/dependabot.yml` & `lzokay-1.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/.github/workflows/dependabot.yml` & `lzokay-1.1.4/.github/workflows/dependabot.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/.github/workflows/python.yml` & `lzokay-1.1.4/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/.gitignore` & `lzokay-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/LICENSE` & `lzokay-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/PKG-INFO` & `lzokay-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lzokay
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lzokay-1.1.3/_lzokay.cpp` & `lzokay-1.1.4/_lzokay.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-/* Generated by Cython 3.0.0rc2 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "cmake_options": {
-            "dir": "D:\\a\\py-lzokay\\py-lzokay\\native\\lzokay",
-            "targets": {
-                "lzokay": "lib"
-            }
-        },
+        "cmake_project": "D:\\a\\py-lzokay\\py-lzokay\\native\\lzokay",
+        "cmake_targets": [
+            "lzokay"
+        ],
         "depends": [],
         "extra_compile_args": [
             "-DUNICODE",
             "/std:c++17",
             "/MD"
         ],
         "language": "c++",
@@ -57,18 +55,18 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0rc2"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000C2
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -1882,30 +1880,30 @@
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0rc2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0rc2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0rc2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0rc2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0rc2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0rc2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0rc2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0rc2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
@@ -5615,35 +5613,35 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 69, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_0(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8267,18 +8265,18 @@
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0rc2
-#define __PYX_HAVE_RT_ImportType_3_0_0rc2
-static PyTypeObject *__Pyx_ImportType_3_0_0rc2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0rc2 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -8324,23 +8322,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0rc2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0rc2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `lzokay-1.1.3/_lzokay.pyx` & `lzokay-1.1.4/_lzokay.pyx`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/lzokay_wrap.pxd` & `lzokay-1.1.4/lzokay_wrap.pxd`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/CMakeLists.txt` & `lzokay-1.1.4/native/lzokay/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/LICENSE` & `lzokay-1.1.4/native/lzokay/LICENSE`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/README.md` & `lzokay-1.1.4/native/lzokay/README.md`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.cpp` & `lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.h` & `lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.h`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/lzokay.cpp` & `lzokay-1.1.4/native/lzokay/lzokay.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/lzokay.hpp` & `lzokay-1.1.4/native/lzokay/lzokay.hpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/native/lzokay/test.cpp` & `lzokay-1.1.4/native/lzokay/test.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.3/pyproject.toml` & `lzokay-1.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=61.2",
     "Cython>=3.0a10",
-    "setuptools_scm[toml]>=3.4"
+    "setuptools_scm[toml]>=3.4",
+    "setuptools-cmake-helper>=0.1.1",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lzokay"
 description = "Python bindings for LZ👌, a LZO compression/decompression algorithm."
```

### Comparing `lzokay-1.1.3/src/lzokay.egg-info/PKG-INFO` & `lzokay-1.1.4/src/lzokay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lzokay
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lzokay-1.1.3/src/lzokay.egg-info/SOURCES.txt` & `lzokay-1.1.4/src/lzokay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

