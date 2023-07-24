# Comparing `tmp/PyQt6_sip-13.5.1.tar.gz` & `tmp/PyQt6_sip-13.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_sip-13.5.1.tar", last modified: Thu Apr 13 15:05:22 2023, max compression
+gzip compressed data, was "PyQt6_sip-13.5.2.tar", last modified: Fri Jul 21 16:58:20 2023, max compression
```

## Comparing `PyQt6_sip-13.5.1.tar` & `PyQt6_sip-13.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-13 15:05:22.851240 PyQt6_sip-13.5.1/
--rw-r--r--   0 phil       (501) staff       (20)     2766 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)    18161 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE-GPL2
--rw-r--r--   0 phil       (501) staff       (20)    35297 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE-GPL3
--rw-r--r--   0 phil       (501) staff       (20)       56 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-13 15:05:22.851324 PyQt6_sip-13.5.1/PKG-INFO
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-13 15:05:22.851032 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      389 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        6 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)      108 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/README
--rw-r--r--   0 phil       (501) staff       (20)       57 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)      296 2023-04-13 15:05:22.851799 PyQt6_sip-13.5.1/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1630 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/setup.py
--rw-r--r--   0 phil       (501) staff       (20)    49929 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip.h
--rw-r--r--   0 phil       (501) staff       (20)    21140 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_array.c
--rw-r--r--   0 phil       (501) staff       (20)     1285 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_array.h
--rw-r--r--   0 phil       (501) staff       (20)      859 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_bool.cpp
--rw-r--r--   0 phil       (501) staff       (20)   312458 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_core.c
--rw-r--r--   0 phil       (501) staff       (20)     5397 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_core.h
--rw-r--r--   0 phil       (501) staff       (20)    13975 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_descriptors.c
--rw-r--r--   0 phil       (501) staff       (20)    14690 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_enum.c
--rw-r--r--   0 phil       (501) staff       (20)     1296 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_enum.h
--rw-r--r--   0 phil       (501) staff       (20)     5650 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_int_convertors.c
--rw-r--r--   0 phil       (501) staff       (20)    13795 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_object_map.c
--rw-r--r--   0 phil       (501) staff       (20)     4788 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_threads.c
--rw-r--r--   0 phil       (501) staff       (20)    19169 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_voidptr.c
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-21 16:58:20.322716 PyQt6_sip-13.5.2/
+-rw-r--r--   0 phil       (501) staff       (20)     2766 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)    18161 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/LICENSE-GPL2
+-rw-r--r--   0 phil       (501) staff       (20)    35297 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/LICENSE-GPL3
+-rw-r--r--   0 phil       (501) staff       (20)       56 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      505 2023-07-21 16:58:20.322810 PyQt6_sip-13.5.2/PKG-INFO
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-21 16:58:20.322501 PyQt6_sip-13.5.2/PyQt6_sip.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      505 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/PyQt6_sip.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      389 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/PyQt6_sip.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/PyQt6_sip.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        6 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/PyQt6_sip.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)      108 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/README
+-rw-r--r--   0 phil       (501) staff       (20)       57 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)      296 2023-07-21 16:58:20.323258 PyQt6_sip-13.5.2/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1630 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/setup.py
+-rw-r--r--   0 phil       (501) staff       (20)    49930 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip.h
+-rw-r--r--   0 phil       (501) staff       (20)    21256 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_array.c
+-rw-r--r--   0 phil       (501) staff       (20)     1285 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_array.h
+-rw-r--r--   0 phil       (501) staff       (20)      859 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_bool.cpp
+-rw-r--r--   0 phil       (501) staff       (20)   312546 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_core.c
+-rw-r--r--   0 phil       (501) staff       (20)     5397 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_core.h
+-rw-r--r--   0 phil       (501) staff       (20)    13975 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_descriptors.c
+-rw-r--r--   0 phil       (501) staff       (20)    14690 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_enum.c
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_enum.h
+-rw-r--r--   0 phil       (501) staff       (20)     5650 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_int_convertors.c
+-rw-r--r--   0 phil       (501) staff       (20)    13795 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_object_map.c
+-rw-r--r--   0 phil       (501) staff       (20)     4788 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_threads.c
+-rw-r--r--   0 phil       (501) staff       (20)    19169 2023-07-21 16:58:20.000000 PyQt6_sip-13.5.2/sip_voidptr.c
```

### Comparing `PyQt6_sip-13.5.1/LICENSE` & `PyQt6_sip-13.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/LICENSE-GPL2` & `PyQt6_sip-13.5.2/LICENSE-GPL2`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/LICENSE-GPL3` & `PyQt6_sip-13.5.2/LICENSE-GPL3`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/setup.py` & `PyQt6_sip-13.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,12 +34,12 @@
     module_src.append('sip_bool.cpp')
 
 module = Extension('PyQt6.sip', module_src)
 
 # Do the setup.
 setup(
         name='PyQt6_sip',
-        version='13.5.1',
+        version='13.5.2',
         license='SIP',
         python_requires='>=3.7',
         ext_modules=[module]
      )
```

### Comparing `PyQt6_sip-13.5.1/sip.h` & `PyQt6_sip-13.5.2/sip.h`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 extern "C" {
 #endif
 
 
 /* The version of the ABI. */
 #define SIP_ABI_MAJOR_VERSION       13
 #define SIP_ABI_MINOR_VERSION       5
-#define SIP_MODULE_PATCH_VERSION    1
+#define SIP_MODULE_PATCH_VERSION    2
 
 
 /*
  * The change history of the ABI.
  *
  * v13.5
  *  - Added the '#' conversion character to the argument parsers.
@@ -70,16 +70,16 @@
  *
  * v13.1
  *  - Added sipNextExceptionHandler().
  */
 
 
 /* The version of the code generator. */
-#define SIP_VERSION                 0x60709
-#define SIP_VERSION_STR             "6.7.9"
+#define SIP_VERSION                 0x6070a
+#define SIP_VERSION_STR             "6.7.10"
 
 /* These are all dependent on the user-specified name of the sip module. */
 #define _SIP_MODULE_FQ_NAME         "PyQt6.sip"
 #define _SIP_MODULE_NAME            "sip"
 #define _SIP_MODULE_SHARED          1
 #define _SIP_MODULE_ENTRY           PyInit_sip
```

### Comparing `PyQt6_sip-13.5.1/sip_array.c` & `PyQt6_sip-13.5.2/sip_array.c`

 * *Files 3% similar despite different names*

```diff
@@ -280,44 +280,51 @@
 
 /*
  * The buffer implementation.
  */
 static int sipArray_getbuffer(PyObject *self, Py_buffer *view, int flags)
 {
     sipArrayObject *array = (sipArrayObject *)self;
+    const char *format;
+    Py_ssize_t itemsize;
 
     if (view == NULL)
         return 0;
 
     if (((flags & PyBUF_WRITABLE) == PyBUF_WRITABLE) && (array->flags & SIP_READ_ONLY))
     {
         PyErr_SetString(PyExc_BufferError, "object is not writable");
         return -1;
     }
 
     view->obj = self;
     Py_INCREF(self);
 
+    /*
+     * If there is no format, ie. it is a wrapped type, then present it as
+     * bytes.
+     */
+    if ((format = array->format) == NULL)
+    {
+        format = "B";
+        itemsize = sizeof (unsigned char);
+    }
+    else
+    {
+        itemsize = array->stride;
+    }
+
     view->buf = array->data;
     view->len = array->len * array->stride;
     view->readonly = (array->flags & SIP_READ_ONLY);
-    view->itemsize = array->stride;
+    view->itemsize = itemsize;
 
     view->format = NULL;
     if ((flags & PyBUF_FORMAT) == PyBUF_FORMAT)
-    {
-        if (array->format == NULL)
-        {
-            PyErr_SetString(PyExc_BufferError,
-                    "format has not been specified");
-            return -1;
-        }
-
-        view->format = (char *)array->format;
-    }
+        view->format = format;
 
     view->ndim = 1;
 
     view->shape = NULL;
     if ((flags & PyBUF_ND) == PyBUF_ND)
         view->shape = &view->len;
```

### Comparing `PyQt6_sip-13.5.1/sip_array.h` & `PyQt6_sip-13.5.2/sip_array.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_bool.cpp` & `PyQt6_sip-13.5.2/sip_bool.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_core.c` & `PyQt6_sip-13.5.2/sip_core.c`

 * *Files 0% similar despite different names*

```diff
@@ -1886,27 +1886,27 @@
  * A wrapper around the Python memory allocater that will raise an exception if
  * if the allocation fails.
  */
 void *sip_api_malloc(size_t nbytes)
 {
     void *mem;
 
-    if ((mem = PyMem_Malloc(nbytes)) == NULL)
+    if ((mem = PyMem_RawMalloc(nbytes)) == NULL)
         PyErr_NoMemory();
 
     return mem;
 }
 
 
 /*
  * A wrapper around the Python memory de-allocater.
  */
 void sip_api_free(void *mem)
 {
-    PyMem_Free(mem);
+    PyMem_RawFree(mem);
 }
 
 
 /*
  * Extend a Python slot by looking in other modules to see if there is an
  * extender function that can handle the arguments.
  */
@@ -11125,15 +11125,19 @@
 
 
 /*
  * Get the dict of a Python type (on behalf of the limited API).
  */
 static PyObject *sip_api_py_type_dict(const PyTypeObject *py_type)
 {
+#if PY_VERSION_HEX >= 0x030c0000
+    return PyType_GetDict(py_type);
+#else
     return py_type->tp_dict;
+#endif
 }
 
 
 /*
  * Get the name of a Python type (on behalf of the limited API).
  */
 static const char *sip_api_py_type_name(const PyTypeObject *py_type)
```

### Comparing `PyQt6_sip-13.5.1/sip_core.h` & `PyQt6_sip-13.5.2/sip_core.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_descriptors.c` & `PyQt6_sip-13.5.2/sip_descriptors.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_enum.c` & `PyQt6_sip-13.5.2/sip_enum.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_enum.h` & `PyQt6_sip-13.5.2/sip_enum.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_int_convertors.c` & `PyQt6_sip-13.5.2/sip_int_convertors.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_object_map.c` & `PyQt6_sip-13.5.2/sip_object_map.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_threads.c` & `PyQt6_sip-13.5.2/sip_threads.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.1/sip_voidptr.c` & `PyQt6_sip-13.5.2/sip_voidptr.c`

 * *Files identical despite different names*

