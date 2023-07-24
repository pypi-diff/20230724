# Comparing `tmp/py7za-0.2.8.tar.gz` & `tmp/py7za-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py7za-0.2.8.tar", last modified: Thu Aug  4 07:07:27 2022, max compression
+gzip compressed data, was "py7za-0.2.9.tar", last modified: Mon Jul 24 05:01:00 2023, max compression
```

## Comparing `py7za-0.2.8.tar` & `py7za-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-08-04 07:07:27.095668 py7za-0.2.8/
--rw-rw-rw-   0        0        0      121 2021-12-14 05:08:19.000000 py7za-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4052 2022-08-04 07:07:27.095668 py7za-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2851 2022-01-14 00:29:03.000000 py7za-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-08-04 07:07:27.085667 py7za-0.2.8/py7za/
--rw-rw-rw-   0        0        0      206 2021-12-16 08:00:39.000000 py7za-0.2.8/py7za/__init__.py
--rw-rw-rw-   0        0        0     3070 2022-01-13 22:52:47.000000 py7za-0.2.8/py7za/_asyncio_pool.py
--rw-rw-rw-   0        0        0     3530 2021-10-27 05:27:59.000000 py7za-0.2.8/py7za/_cpu_count.py
--rw-rw-rw-   0        0        0     1932 2021-12-16 08:07:49.000000 py7za-0.2.8/py7za/_nice_size.py
--rw-rw-rw-   0        0        0     6363 2021-11-15 00:06:11.000000 py7za-0.2.8/py7za/_py7za.py
--rw-rw-rw-   0        0        0       23 2022-08-04 07:06:44.000000 py7za-0.2.8/py7za/_version.py
-drwxrwxrwx   0        0        0        0 2022-08-04 07:07:27.092667 py7za-0.2.8/py7za/bin/
--rw-rw-rw-   0        0        0     1288 2020-12-03 01:25:23.000000 py7za-0.2.8/py7za/bin/7za-license.txt
--rwxrwxrwx   0        0        0  1152000 2019-02-21 16:00:00.000000 py7za-0.2.8/py7za/bin/7za.exe
--rw-rw-rw-   0        0        0    27023 2021-10-15 03:25:18.000000 py7za-0.2.8/py7za/bin/GNU_LGPL.txt
--rw-rw-rw-   0        0        0      261 2021-12-14 05:08:19.000000 py7za-0.2.8/py7za/groups.json
--rw-rw-rw-   0        0        0    24544 2022-08-04 06:50:08.000000 py7za-0.2.8/py7za/py7za_box.py
-drwxrwxrwx   0        0        0        0 2022-08-04 07:07:27.089667 py7za-0.2.8/py7za.egg-info/
--rw-rw-rw-   0        0        0     4052 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-04 07:07:26.000000 py7za-0.2.8/py7za.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-08-04 07:07:27.095668 py7za-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2102 2022-01-13 22:48:00.000000 py7za-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-04 07:07:27.094667 py7za-0.2.8/test/
--rw-rw-rw-   0        0        0     1808 2022-01-13 22:48:00.000000 py7za-0.2.8/test/test_asyncio_pool.py
--rw-rw-rw-   0        0        0     1465 2021-12-16 08:06:31.000000 py7za-0.2.8/test/test_nice_size.py
--rw-rw-rw-   0        0        0    19224 2022-01-13 11:57:56.000000 py7za-0.2.8/test/test_py7za_box.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:01:00.830297 py7za-0.2.9/
+-rw-rw-rw-   0        0        0      121 2021-12-14 05:08:19.000000 py7za-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4052 2023-07-24 05:01:00.849731 py7za-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2851 2022-01-14 00:29:03.000000 py7za-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 05:01:00.805108 py7za-0.2.9/py7za/
+-rw-rw-rw-   0        0        0      206 2021-12-16 08:00:39.000000 py7za-0.2.9/py7za/__init__.py
+-rw-rw-rw-   0        0        0     3070 2022-01-13 22:52:47.000000 py7za-0.2.9/py7za/_asyncio_pool.py
+-rw-rw-rw-   0        0        0     3530 2021-10-27 05:27:59.000000 py7za-0.2.9/py7za/_cpu_count.py
+-rw-rw-rw-   0        0        0     1932 2021-12-16 08:07:49.000000 py7za-0.2.9/py7za/_nice_size.py
+-rw-rw-rw-   0        0        0     6363 2021-11-15 00:06:11.000000 py7za-0.2.9/py7za/_py7za.py
+-rw-rw-rw-   0        0        0       23 2023-07-24 05:00:22.000000 py7za-0.2.9/py7za/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:01:00.813149 py7za-0.2.9/py7za/bin/
+-rw-rw-rw-   0        0        0     1288 2020-12-03 01:25:23.000000 py7za-0.2.9/py7za/bin/7za-license.txt
+-rwxrwxrwx   0        0        0  1152000 2019-02-21 16:00:00.000000 py7za-0.2.9/py7za/bin/7za.exe
+-rw-rw-rw-   0        0        0    27023 2021-10-15 03:25:18.000000 py7za-0.2.9/py7za/bin/GNU_LGPL.txt
+-rw-rw-rw-   0        0        0      261 2021-12-14 05:08:19.000000 py7za-0.2.9/py7za/groups.json
+-rw-rw-rw-   0        0        0    24544 2022-08-04 06:50:08.000000 py7za-0.2.9/py7za/py7za_box.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:01:00.810149 py7za-0.2.9/py7za.egg-info/
+-rw-rw-rw-   0        0        0     4052 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 05:01:00.000000 py7za-0.2.9/py7za.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-24 05:01:00.850738 py7za-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2102 2022-01-13 22:48:00.000000 py7za-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:01:00.830297 py7za-0.2.9/test/
+-rw-rw-rw-   0        0        0     1808 2022-01-13 22:48:00.000000 py7za-0.2.9/test/test_asyncio_pool.py
+-rw-rw-rw-   0        0        0     1465 2021-12-16 08:06:31.000000 py7za-0.2.9/test/test_nice_size.py
+-rw-rw-rw-   0        0        0    19224 2022-01-13 11:57:56.000000 py7za-0.2.9/test/test_py7za_box.py
```

### Comparing `py7za-0.2.8/PKG-INFO` & `py7za-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py7za
-Version: 0.2.8
+Version: 0.2.9
 Summary: Description
 Home-page: https://gitlab.com/Jaap.vanderVelde/py7za
 Author: BMT, Jaap van der Velde
 Author-email: jaap.vandervelde@bmtglobal.com
 License: MIT
-Download-URL: https://gitlab.com/Jaap.vanderVelde/py7za/repository/archive.zip?ref=0.2.8
+Download-URL: https://gitlab.com/Jaap.vanderVelde/py7za/repository/archive.zip?ref=0.2.9
 Description: # Py7za ("pizza")
         
         Python wrapper for running the 7za.exe utility from https://www.7-zip.org/
         
         The wrapper simply runs the application in a separate process and added functionality primarily aimed at running the tool in several parallel processes from the command-line.
         
         Other than providing that utility, the wrapper tries to provide users Python API access to 7za in a way as simple, and as close to the original as possible. See some documentation for the command line options here https://sevenzip.osdn.jp/chm/cmdline/index.htm (no affiliation).
```

### Comparing `py7za-0.2.8/README.md` & `py7za-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/_asyncio_pool.py` & `py7za-0.2.9/py7za/_asyncio_pool.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/_cpu_count.py` & `py7za-0.2.9/py7za/_cpu_count.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/_nice_size.py` & `py7za-0.2.9/py7za/_nice_size.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/_py7za.py` & `py7za-0.2.9/py7za/_py7za.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/bin/7za-license.txt` & `py7za-0.2.9/py7za/bin/7za-license.txt`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/bin/7za.exe` & `py7za-0.2.9/py7za/bin/7za.exe`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/bin/GNU_LGPL.txt` & `py7za-0.2.9/py7za/bin/GNU_LGPL.txt`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za/py7za_box.py` & `py7za-0.2.9/py7za/py7za_box.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/py7za.egg-info/PKG-INFO` & `py7za-0.2.9/py7za.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py7za
-Version: 0.2.8
+Version: 0.2.9
 Summary: Description
 Home-page: https://gitlab.com/Jaap.vanderVelde/py7za
 Author: BMT, Jaap van der Velde
 Author-email: jaap.vandervelde@bmtglobal.com
 License: MIT
-Download-URL: https://gitlab.com/Jaap.vanderVelde/py7za/repository/archive.zip?ref=0.2.8
+Download-URL: https://gitlab.com/Jaap.vanderVelde/py7za/repository/archive.zip?ref=0.2.9
 Description: # Py7za ("pizza")
         
         Python wrapper for running the 7za.exe utility from https://www.7-zip.org/
         
         The wrapper simply runs the application in a separate process and added functionality primarily aimed at running the tool in several parallel processes from the command-line.
         
         Other than providing that utility, the wrapper tries to provide users Python API access to 7za in a way as simple, and as close to the original as possible. See some documentation for the command line options here https://sevenzip.osdn.jp/chm/cmdline/index.htm (no affiliation).
```

### Comparing `py7za-0.2.8/setup.py` & `py7za-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/test/test_asyncio_pool.py` & `py7za-0.2.9/test/test_asyncio_pool.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/test/test_nice_size.py` & `py7za-0.2.9/test/test_nice_size.py`

 * *Files identical despite different names*

### Comparing `py7za-0.2.8/test/test_py7za_box.py` & `py7za-0.2.9/test/test_py7za_box.py`

 * *Files identical despite different names*

