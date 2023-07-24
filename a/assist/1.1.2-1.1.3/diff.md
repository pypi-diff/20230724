# Comparing `tmp/assist-1.1.2.tar.gz` & `tmp/assist-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assist-1.1.2.tar", last modified: Thu Jul 20 17:49:51 2023, max compression
+gzip compressed data, was "assist-1.1.3.tar", last modified: Mon Jul 24 13:43:24 2023, max compression
```

## Comparing `assist-1.1.2.tar` & `assist-1.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.152630 assist-1.1.2/
--rw-r--r--   0 mholman    (501) staff       (20)    35147 2023-03-16 20:41:43.000000 assist-1.1.2/LICENSE
--rw-r--r--   0 mholman    (501) staff       (20)      264 2023-07-20 17:44:53.000000 assist-1.1.2/MANIFEST.in
--rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-20 17:49:51.152454 assist-1.1.2/PKG-INFO
--rw-r--r--   0 mholman    (501) staff       (20)     5345 2023-07-20 17:49:30.000000 assist-1.1.2/README.md
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.149949 assist-1.1.2/assist/
--rw-r--r--   0 mholman    (501) staff       (20)     1813 2023-07-20 17:44:53.000000 assist-1.1.2/assist/__init__.py
--rw-r--r--   0 mholman    (501) staff       (20)     2829 2023-07-20 17:44:53.000000 assist-1.1.2/assist/ephem.py
--rw-r--r--   0 mholman    (501) staff       (20)     3601 2023-07-20 17:44:53.000000 assist-1.1.2/assist/extras.py
--rw-r--r--   0 mholman    (501) staff       (20)        0 2023-07-20 17:44:53.000000 assist-1.1.2/assist/py.typed
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.150935 assist-1.1.2/assist.egg-info/
--rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/PKG-INFO
--rw-r--r--   0 mholman    (501) staff       (20)      411 2023-07-20 17:49:51.000000 assist-1.1.2/assist.egg-info/SOURCES.txt
--rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/dependency_links.txt
--rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/not-zip-safe
--rw-r--r--   0 mholman    (501) staff       (20)       22 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/requires.txt
--rw-r--r--   0 mholman    (501) staff       (20)       17 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/top_level.txt
--rw-r--r--   0 mholman    (501) staff       (20)       81 2023-03-16 20:41:43.000000 assist-1.1.2/pyproject.toml
--rw-r--r--   0 mholman    (501) staff       (20)       38 2023-07-20 17:49:51.152678 assist-1.1.2/setup.cfg
--rw-r--r--   0 mholman    (501) staff       (20)     4818 2023-07-20 17:49:30.000000 assist-1.1.2/setup.py
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.152232 assist-1.1.2/src/
--rw-r--r--   0 mholman    (501) staff       (20)    21697 2023-07-20 17:49:30.000000 assist-1.1.2/src/assist.c
--rw-r--r--   0 mholman    (501) staff       (20)     6849 2023-07-20 17:44:53.000000 assist-1.1.2/src/assist.h
--rw-r--r--   0 mholman    (501) staff       (20)    84761 2023-07-20 17:44:53.000000 assist-1.1.2/src/forces.c
--rw-r--r--   0 mholman    (501) staff       (20)     1383 2023-03-16 20:41:43.000000 assist-1.1.2/src/forces.h
--rw-r--r--   0 mholman    (501) staff       (20)    12771 2023-03-16 20:41:43.000000 assist-1.1.2/src/planets.c
--rw-r--r--   0 mholman    (501) staff       (20)     3161 2023-03-16 20:41:43.000000 assist-1.1.2/src/planets.h
--rw-r--r--   0 mholman    (501) staff       (20)     8181 2023-03-16 20:41:43.000000 assist-1.1.2/src/spk.c
--rw-r--r--   0 mholman    (501) staff       (20)     1135 2023-03-16 20:41:43.000000 assist-1.1.2/src/spk.h
--rw-r--r--   0 mholman    (501) staff       (20)        7 2023-07-20 17:49:02.000000 assist-1.1.2/version.txt
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-24 13:43:24.728346 assist-1.1.3/
+-rw-r--r--   0 mholman    (501) staff       (20)    35147 2023-07-21 19:36:10.000000 assist-1.1.3/LICENSE
+-rw-r--r--   0 mholman    (501) staff       (20)      264 2023-07-21 19:36:10.000000 assist-1.1.3/MANIFEST.in
+-rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-24 13:43:24.728243 assist-1.1.3/PKG-INFO
+-rw-r--r--   0 mholman    (501) staff       (20)     5345 2023-07-24 13:43:14.000000 assist-1.1.3/README.md
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-24 13:43:24.725795 assist-1.1.3/assist/
+-rw-r--r--   0 mholman    (501) staff       (20)     1813 2023-07-21 19:36:10.000000 assist-1.1.3/assist/__init__.py
+-rw-r--r--   0 mholman    (501) staff       (20)     2829 2023-07-21 19:36:10.000000 assist-1.1.3/assist/ephem.py
+-rw-r--r--   0 mholman    (501) staff       (20)     3601 2023-07-21 19:36:10.000000 assist-1.1.3/assist/extras.py
+-rw-r--r--   0 mholman    (501) staff       (20)        0 2023-07-21 19:36:10.000000 assist-1.1.3/assist/py.typed
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-24 13:43:24.726542 assist-1.1.3/assist.egg-info/
+-rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-24 13:43:24.000000 assist-1.1.3/assist.egg-info/PKG-INFO
+-rw-r--r--   0 mholman    (501) staff       (20)      411 2023-07-24 13:43:24.000000 assist-1.1.3/assist.egg-info/SOURCES.txt
+-rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-24 13:43:24.000000 assist-1.1.3/assist.egg-info/dependency_links.txt
+-rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-21 20:08:31.000000 assist-1.1.3/assist.egg-info/not-zip-safe
+-rw-r--r--   0 mholman    (501) staff       (20)       22 2023-07-24 13:43:24.000000 assist-1.1.3/assist.egg-info/requires.txt
+-rw-r--r--   0 mholman    (501) staff       (20)       17 2023-07-24 13:43:24.000000 assist-1.1.3/assist.egg-info/top_level.txt
+-rw-r--r--   0 mholman    (501) staff       (20)       81 2023-07-21 19:36:10.000000 assist-1.1.3/pyproject.toml
+-rw-r--r--   0 mholman    (501) staff       (20)       38 2023-07-24 13:43:24.728378 assist-1.1.3/setup.cfg
+-rw-r--r--   0 mholman    (501) staff       (20)     4835 2023-07-24 13:43:14.000000 assist-1.1.3/setup.py
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-24 13:43:24.728074 assist-1.1.3/src/
+-rw-r--r--   0 mholman    (501) staff       (20)    21697 2023-07-24 13:43:14.000000 assist-1.1.3/src/assist.c
+-rw-r--r--   0 mholman    (501) staff       (20)     6792 2023-07-24 00:23:15.000000 assist-1.1.3/src/assist.h
+-rw-r--r--   0 mholman    (501) staff       (20)    84761 2023-07-21 19:36:10.000000 assist-1.1.3/src/forces.c
+-rw-r--r--   0 mholman    (501) staff       (20)     1383 2023-07-21 19:36:10.000000 assist-1.1.3/src/forces.h
+-rw-r--r--   0 mholman    (501) staff       (20)    12771 2023-07-21 19:36:10.000000 assist-1.1.3/src/planets.c
+-rw-r--r--   0 mholman    (501) staff       (20)     3161 2023-07-21 19:36:10.000000 assist-1.1.3/src/planets.h
+-rw-r--r--   0 mholman    (501) staff       (20)     8181 2023-07-21 19:36:10.000000 assist-1.1.3/src/spk.c
+-rw-r--r--   0 mholman    (501) staff       (20)     1135 2023-07-21 19:36:10.000000 assist-1.1.3/src/spk.h
+-rw-r--r--   0 mholman    (501) staff       (20)        7 2023-07-24 13:42:20.000000 assist-1.1.3/version.txt
```

### Comparing `assist-1.1.2/LICENSE` & `assist-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/PKG-INFO` & `assist-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assist
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library high accuracy ephemeris in REBOUND
 Home-page: https://github.com/matthewholman/assist
 Author: Matthew Holman
 Author-email: mholman@cfa.harvard.edu
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Version](https://img.shields.io/badge/assist-v1.1.2-green.svg?style=flat)](https://assist.readthedocs.org)
+[![Version](https://img.shields.io/badge/assist-v1.1.3-green.svg?style=flat)](https://assist.readthedocs.org)
 [![GPL](https://img.shields.io/badge/license-GPL-green.svg?style=flat)](https://github.com/matthewholman/blob/main/LICENSE)
 [![Python unit tests)](https://github.com/matthewholman/assist/actions/workflows/python.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/python.yml)
 [![C unit tests](https://github.com/matthewholman/assist/actions/workflows/c.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/c.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7778016.svg)](https://doi.org/10.5281/zenodo.7778016)
```

### Comparing `assist-1.1.2/README.md` & `assist-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b21 5b56 6572 7369 6f6e 5d28 6874 7470  [![Version](http
 00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 00000020: 696f 2f62 6164 6765 2f61 7373 6973 742d  io/badge/assist-
-00000030: 7631 2e31 2e32 2d67 7265 656e 2e73 7667  v1.1.2-green.svg
+00000030: 7631 2e31 2e33 2d67 7265 656e 2e73 7667  v1.1.3-green.svg
 00000040: 3f73 7479 6c65 3d66 6c61 7429 5d28 6874  ?style=flat)](ht
 00000050: 7470 733a 2f2f 6173 7369 7374 2e72 6561  tps://assist.rea
 00000060: 6474 6865 646f 6373 2e6f 7267 290a 5b21  dthedocs.org).[!
 00000070: 5b47 504c 5d28 6874 7470 733a 2f2f 696d  [GPL](https://im
 00000080: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
 00000090: 6765 2f6c 6963 656e 7365 2d47 504c 2d67  ge/license-GPL-g
 000000a0: 7265 656e 2e73 7667 3f73 7479 6c65 3d66  reen.svg?style=f
```

### Comparing `assist-1.1.2/assist/__init__.py` & `assist-1.1.3/assist/__init__.py`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/assist/ephem.py` & `assist-1.1.3/assist/ephem.py`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/assist/extras.py` & `assist-1.1.3/assist/extras.py`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/assist.egg-info/PKG-INFO` & `assist-1.1.3/assist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assist
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library high accuracy ephemeris in REBOUND
 Home-page: https://github.com/matthewholman/assist
 Author: Matthew Holman
 Author-email: mholman@cfa.harvard.edu
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Version](https://img.shields.io/badge/assist-v1.1.2-green.svg?style=flat)](https://assist.readthedocs.org)
+[![Version](https://img.shields.io/badge/assist-v1.1.3-green.svg?style=flat)](https://assist.readthedocs.org)
 [![GPL](https://img.shields.io/badge/license-GPL-green.svg?style=flat)](https://github.com/matthewholman/blob/main/LICENSE)
 [![Python unit tests)](https://github.com/matthewholman/assist/actions/workflows/python.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/python.yml)
 [![C unit tests](https://github.com/matthewholman/assist/actions/workflows/c.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/c.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7778016.svg)](https://doi.org/10.5281/zenodo.7778016)
```

### Comparing `assist-1.1.2/setup.py` & `assist-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DASSISTGITHASH="+ghash
 except:
-    ghash_arg = "-DASSISTGITHASH=14a8eee16015ce67506db3c69a060428d026ffaa" #GITHASHAUTOUPDATE
+    ghash_arg = "-DASSISTGITHASH=52acc4b057a6c26f4a8f324651c3d9b19cbaf6b5" #GITHASHAUTOUPDATE
 
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
 
         try:
             import rebound
@@ -64,24 +64,24 @@
 libassistmodule = Extension('libassist',
                   sources = [ 'src/assist.c','src/spk.c', 'src/planets.c', 'src/forces.c'],
                     include_dirs = ['src'],
                     library_dirs = [],
                     runtime_library_dirs = ["."],
                     libraries=['rebound'+suffix[:suffix.rfind('.')]],
                     define_macros=[ ('LIBASSIST', None) ],
-                    extra_compile_args=['-fstrict-aliasing', '-O3','-std=c99', '-fPIC', '-Wpointer-arith', ghash_arg],
+                    extra_compile_args=['-fstrict-aliasing', '-O3','-std=c99', '-fPIC', '-D_GNU_SOURCE', '-Wpointer-arith', ghash_arg],
                     extra_link_args=extra_link_args,
                     )
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='assist',
-    version='1.1.2',
+    version='1.1.3',
     description='A library high accuracy ephemeris in REBOUND',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/matthewholman/assist',
     author='Matthew Holman',
     author_email='mholman@cfa.harvard.edu',
     license='GPL',
```

### Comparing `assist-1.1.2/src/assist.c` & `assist-1.1.3/src/assist.c`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 const int reb_max_messages_length = 1024;   // needs to be constant expression for array size
 const int reb_max_messages_N = 10;
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* assist_build_str = __DATE__ " " __TIME__;   // Date and time build string. 
-const char* assist_version_str = "1.1.2";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* assist_version_str = "1.1.3";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* assist_githash_str = STRINGIFY(ASSISTGITHASH);// This line gets updated automatically. Do not edit manually.
 
 
 // These correspond to ASSIST_STATUS enum.
 
 const char* assist_error_messages[] = {
     "No error has occured.", // ASSIST_SUCCESS
```

### Comparing `assist-1.1.2/src/assist.h` & `assist-1.1.3/src/assist.h`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,14 @@
  * You should have received a copy of the GNU General Public License
  * along with ASSIST. If not, see <http://www.gnu.org/licenses/>.
  *
  */
 #ifndef _ASSIST_ASSIST_H_H
 #define _ASSIST_ASSIST_H_H
 
-#ifndef M_PI 
-#define M_PI 3.1415926535879323846
-#endif
-
 #include <stdint.h>
 #include <limits.h>
 #include "rebound.h"
 #ifndef ASSISTGITHASH
 #define ASSISTGITHASH notavailable0000000000000000000000000001 
 #endif // ASSISTGITHASH
```

### Comparing `assist-1.1.2/src/forces.c` & `assist-1.1.3/src/forces.c`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/src/forces.h` & `assist-1.1.3/src/forces.h`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/src/planets.c` & `assist-1.1.3/src/planets.c`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/src/planets.h` & `assist-1.1.3/src/planets.h`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/src/spk.c` & `assist-1.1.3/src/spk.c`

 * *Files identical despite different names*

### Comparing `assist-1.1.2/src/spk.h` & `assist-1.1.3/src/spk.h`

 * *Files identical despite different names*

