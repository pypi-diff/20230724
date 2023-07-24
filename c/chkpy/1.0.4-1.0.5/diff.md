# Comparing `tmp/chkpy-1.0.4.tar.gz` & `tmp/chkpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul 24 20:35:57 2022, from Unix
+gzip compressed data, was "chkpy-1.0.5.tar", last modified: Mon Jul 24 20:29:45 2023, max compression
```

## Comparing `chkpy-1.0.4.tar` & `chkpy-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    35149 2022-07-24 19:18:06.000000 chkpy-1.0.4/LICENSE
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1798 2022-07-24 20:35:41.000000 chkpy-1.0.4/PKG-INFO
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5409 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/test.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      561 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       47 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/entry_points.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      123 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1814 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/main.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1205 2022-07-24 19:18:06.000000 chkpy-1.0.4/README.md
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      341 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4077 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/modes.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      783 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/art.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1460 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/directory.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1689 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/filetest.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2022-07-24 20:33:56.000000 chkpy-1.0.4/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      371 2022-07-24 19:18:06.000000 chkpy-1.0.4/chkpy/__main__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1002 2022-07-24 20:33:43.000000 chkpy-1.0.4/setup.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2022-07-24 20:35:41.000000 chkpy-1.0.4/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       16 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        6 2022-07-24 20:33:56.000000 chkpy-1.0.4/chkpy.egg-info/top_level.txt
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-24 20:29:45.994937 chkpy-1.0.5/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    35149 2023-07-24 20:23:18.000000 chkpy-1.0.5/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      542 2023-07-24 20:29:45.994937 chkpy-1.0.5/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1205 2023-07-24 20:23:18.000000 chkpy-1.0.5/README.md
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-24 20:29:45.993937 chkpy-1.0.5/chkpy/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      123 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      371 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/__main__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      783 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/art.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1460 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/directory.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1689 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/filetest copy.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1689 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/filetest.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1832 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/main.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4037 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/modes.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5409 2023-07-24 20:23:18.000000 chkpy-1.0.5/chkpy/test.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-24 20:29:45.994937 chkpy-1.0.5/chkpy.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      542 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      364 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       46 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       16 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        6 2023-07-24 20:29:45.000000 chkpy-1.0.5/chkpy.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-07-24 20:29:45.994937 chkpy-1.0.5/setup.cfg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1002 2023-07-24 20:24:05.000000 chkpy-1.0.5/setup.py
```

### Comparing `chkpy-1.0.4/LICENSE` & `chkpy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chkpy-1.0.4/PKG-INFO` & `chkpy-1.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: chkpy
-Version: 1.0.4
-Summary: Wrapper for 3 python tools to aid in code development
-Home-page: https://github.com/nwc1020/ChkPy
-Author: Anthony Clark, Dylan Haus & Nick Cardin
-Author-email: <mail@unh.edu>
-License: GPLv3
-Keywords: python,wrapper,development
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChkPy!
  ```
     ChkPy! is a wrapper for 3 python development tools, pylint, pycodestyle & auopep8.
 
 Pylint provides syntax-error reporting, pycodestyle provides styling reporting & auopep8 provides enforcement of both.
 
 ChkPy! also has 3 options. these modes/options are explained below in detail.
@@ -57,9 +39,8 @@
 
     - chkpy Directory  (-r or -d )
 ```
 ### ChkPy will allow you to run BOTH modes simultaneously. THIS IS NOT RECOMENDED. DO NOT DO THIS.
 ```
 
     Created by Anthony Clark, Dylan Haus & Nick Cardin
-```
-
+```
```

### Comparing `chkpy-1.0.4/chkpy/test.py` & `chkpy-1.0.5/chkpy/test.py`

 * *Files identical despite different names*

### Comparing `chkpy-1.0.4/chkpy.egg-info/PKG-INFO` & `chkpy-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: chkpy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Wrapper for 3 python tools to aid in code development
 Home-page: https://github.com/nwc1020/ChkPy
 Author: Anthony Clark, Dylan Haus & Nick Cardin
 Author-email: <mail@unh.edu>
 License: GPLv3
 Keywords: python,wrapper,development
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 File: README.md
-
```

### Comparing `chkpy-1.0.4/chkpy/main.py` & `chkpy-1.0.5/chkpy/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     - the "-r" option which only runs reporting tools against,
       the given file/directory (reporting mode)
 
     - the "-d" option which runs reporting tools AFTER,
       attempting to fix styling/syntax (developer mode)
     '''
     opts, args = getopt.getopt(args, "dr")
-    file = args[0]
+    file = args[0].replace("\\","/")
     dir_mode_steps = ['directorymode']
     default_steps = ['pylint', 'pycode', 'auto8', 'pylint', 'pycode']
     dev_mode_steps = ['auto8', 'pylint', 'pycode']
     report_mode_steps = ['pylint', 'pycode']
 
     seperator = "\n=====================================================================\n"
     if os.path.isdir(file):
```

### Comparing `chkpy-1.0.4/chkpy/modes.py` & `chkpy-1.0.5/chkpy/modes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,16 @@
         description: This function calls pylint and
         runs it against an input file and returns the
         output in a tuple, first part of the tuple should be
         what we need most of the time however
         im returning both just in case
         '''
 
-        (pylint_stdout, pylint_stderr) = epylint.py_run("\"" + filename + "\"",
-        return_std=True)
-        return "\n OUTPUT FROM PYLINT! \n\n" + pylint_stdout.getvalue() + "\n"
+        pylint_stdout = os.popen("pylint " + "\"" + filename + "\"").read()
+        return "\n OUTPUT FROM PYLINT! \n\n" + pylint_stdout + "\n"
 
     def pycode(filename):  # F3
         '''
         date: 10/27/21
         edited: 02/13/22
         author: Dylan, MRegirouard
         description: This function calls pycodestyle
```

### Comparing `chkpy-1.0.4/chkpy/art.py` & `chkpy-1.0.5/chkpy/art.py`

 * *Files identical despite different names*

### Comparing `chkpy-1.0.4/chkpy/directory.py` & `chkpy-1.0.5/chkpy/directory.py`

 * *Files identical despite different names*

### Comparing `chkpy-1.0.4/chkpy/filetest.py` & `chkpy-1.0.5/chkpy/filetest copy.py`

 * *Files identical despite different names*

### Comparing `chkpy-1.0.4/setup.py` & `chkpy-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 
 # Setting up
 setup(
     name="chkpy",
-    version='1.0.4',
+    version='1.0.5',
     author="Anthony Clark, Dylan Haus & Nick Cardin",
     author_email="<mail@unh.edu>",
     description='Wrapper for 3 python tools to aid in code development',
     long_description='File: README.md',
     license='GPLv3',
     long_description_content_type="text/markdown",
     url="https://github.com/nwc1020/ChkPy",
```

