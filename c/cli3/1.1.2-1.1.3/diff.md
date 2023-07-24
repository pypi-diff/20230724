# Comparing `tmp/cli3-1.1.2.tar.gz` & `tmp/cli3-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli3-1.1.2.tar", last modified: Wed Jun 28 01:53:24 2023, max compression
+gzip compressed data, was "cli3-1.1.3.tar", last modified: Mon Jul 24 17:28:56 2023, max compression
```

## Comparing `cli3-1.1.2.tar` & `cli3-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:53:24.901958 cli3-1.1.2/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1064 2020-10-21 03:10:04.000000 cli3-1.1.2/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-06-28 01:53:24.901958 cli3-1.1.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.1.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:53:24.901958 cli3-1.1.2/cli/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1343 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    13821 2023-06-26 05:51:15.000000 cli3-1.1.2/cli/abc.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6825 2023-06-26 05:50:21.000000 cli3-1.1.2/cli/app.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4660 2023-05-09 00:41:40.000000 cli3-1.1.2/cli/argument.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     7041 2023-05-09 00:53:27.000000 cli3-1.1.2/cli/command.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4504 2023-06-26 05:52:32.000000 cli3-1.1.2/cli/flag.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4997 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/help.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     7434 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/parser.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:53:24.901958 cli3-1.1.2/cli/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      111 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5816 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/tests/app.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:53:24.901958 cli3-1.1.2/cli/tests/content/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/tests/content/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2599 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/tests/content/v1.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2002 2023-05-03 02:43:51.000000 cli3-1.1.2/cli/tests/content/v2.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    14056 2023-05-09 00:39:09.000000 cli3-1.1.2/cli/wraps.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:53:24.901958 cli3-1.1.2/cli3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-06-28 01:53:24.000000 cli3-1.1.2/cli3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      402 2023-06-28 01:53:24.000000 cli3-1.1.2/cli3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-28 01:53:24.000000 cli3-1.1.2/cli3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       17 2023-06-28 01:53:24.000000 cli3-1.1.2/cli3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2023-06-28 01:53:24.000000 cli3-1.1.2/cli3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-28 01:53:24.901958 cli3-1.1.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      775 2023-06-26 05:52:58.000000 cli3-1.1.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:28:56.322196 cli3-1.1.3/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1064 2020-10-21 03:10:04.000000 cli3-1.1.3/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-07-24 17:28:56.322196 cli3-1.1.3/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.1.3/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:28:56.318196 cli3-1.1.3/cli/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1343 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    13821 2023-06-26 05:51:15.000000 cli3-1.1.3/cli/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6825 2023-06-26 05:50:21.000000 cli3-1.1.3/cli/app.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4660 2023-05-09 00:41:40.000000 cli3-1.1.3/cli/argument.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7041 2023-05-09 00:53:27.000000 cli3-1.1.3/cli/command.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4619 2023-07-24 17:25:50.000000 cli3-1.1.3/cli/flag.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4997 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/help.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7434 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/parser.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:28:56.322196 cli3-1.1.3/cli/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      111 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5816 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/tests/app.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:28:56.322196 cli3-1.1.3/cli/tests/content/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/tests/content/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2599 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/tests/content/v1.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2002 2023-05-03 02:43:51.000000 cli3-1.1.3/cli/tests/content/v2.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    14056 2023-05-09 00:39:09.000000 cli3-1.1.3/cli/wraps.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:28:56.322196 cli3-1.1.3/cli3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-07-24 17:28:56.000000 cli3-1.1.3/cli3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      402 2023-07-24 17:28:56.000000 cli3-1.1.3/cli3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-24 17:28:56.000000 cli3-1.1.3/cli3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       56 2023-07-24 17:28:56.000000 cli3-1.1.3/cli3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2023-07-24 17:28:56.000000 cli3-1.1.3/cli3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-07-24 17:28:56.322196 cli3-1.1.3/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      848 2023-07-24 17:28:09.000000 cli3-1.1.3/setup.py
```

### Comparing `cli3-1.1.2/LICENSE` & `cli3-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/PKG-INFO` & `cli3-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.1.2
+Version: 1.1.3
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cli3-1.1.2/README.md` & `cli3-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/__init__.py` & `cli3-1.1.3/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/abc.py` & `cli3-1.1.3/cli/abc.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/app.py` & `cli3-1.1.3/cli/app.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/argument.py` & `cli3-1.1.3/cli/argument.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/command.py` & `cli3-1.1.3/cli/command.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/flag.py` & `cli3-1.1.3/cli/flag.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,22 +71,25 @@
 @dataclass(slots=True)
 class BoolFlag(Flag[bool]):
     """implementation for supporting boolean flags"""
     type:      ClassVar[Type] = bool
     default:   bool           = False
     has_value: bool           = False
 
+@dataclass(slots=True)
 class IntFlag(Flag[int]):
     """implementation for supporting integer flags"""
     type: ClassVar[Type] = int
 
+@dataclass(slots=True)
 class StringFlag(Flag[str]):
     """implementation for supporting string flags"""
     type: ClassVar[Type] = str
 
+@dataclass(slots=True)
 class FloatFlag(Flag[float]):
     """implementation for supporting flag flags"""
     type: ClassVar[Type] = float
 
 @dataclass(slots=True)
 class DecimalFlag(Flag[float]):
     """
@@ -98,23 +101,25 @@
     decimal: int            = 2
 
     def parse(self, value: str):
         """handle float founding based on decimal setting"""
         with capture_errors():
             return parse_decimal(value, self.decimal)
 
+@dataclass(slots=True)
 class ListFlag(Flag[List[str]]):
     """implementatin for supporting list flags"""
     type: ClassVar[Type] = list
 
     def parse(self, value: str):
         """convert value into list object"""
         with capture_errors():
             return [c.strip() for c in value.split(',')]
 
+@dataclass(slots=True)
 class DurationFlag(Flag[timedelta]):
     """implementation for supporting time-duration flags"""
     type: ClassVar[Type] = timedelta
 
     def parse(self, value: str):
         """convert string-value into timedelta"""
         with capture_errors():
```

### Comparing `cli3-1.1.2/cli/help.py` & `cli3-1.1.3/cli/help.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/parser.py` & `cli3-1.1.3/cli/parser.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/tests/app.py` & `cli3-1.1.3/cli/tests/app.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/tests/content/v1.py` & `cli3-1.1.3/cli/tests/content/v1.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/tests/content/v2.py` & `cli3-1.1.3/cli/tests/content/v2.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli/wraps.py` & `cli3-1.1.3/cli/wraps.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.2/cli3.egg-info/PKG-INFO` & `cli3-1.1.3/cli3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.1.2
+Version: 1.1.3
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cli3-1.1.2/setup.py` & `cli3-1.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='cli3',
-    version='1.1.2',
+    version='1.1.3',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/cli',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description=(
         'A highly configurable, dynamic, fast, and easy '
         'solution to managing a command-line application.'
     ),
     python_requires='>=3.7',
     long_description=readme,
     long_description_content_type="text/markdown",
-    install_requires=['jinja2', 'pyderive3'],
+    install_requires=[
+        'jinja2>=3.1.2',
+        'pyderive3>=0.0.6',
+        'typing_extensions>=4.7.1',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

