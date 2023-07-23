# Comparing `tmp/pypkg_builder-0.1.tar.gz` & `tmp/pypkg_builder-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypkg_builder-0.1.tar", last modified: Sun Jul 23 21:54:27 2023, max compression
+gzip compressed data, was "pypkg_builder-1.0.tar", last modified: Sun Jul 23 23:33:56 2023, max compression
```

## Comparing `pypkg_builder-0.1.tar` & `pypkg_builder-1.0.tar`

### file list

```diff
@@ -1,14 +1,31 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 21:54:27.208665 pypkg_builder-0.1/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      349 2023-07-23 21:54:27.208665 pypkg_builder-0.1/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        5 2023-07-23 21:48:01.000000 pypkg_builder-0.1/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-23 21:54:27.208665 pypkg_builder-0.1/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      628 2023-07-23 21:53:09.000000 pypkg_builder-0.1/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 21:54:27.208665 pypkg_builder-0.1/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 21:54:27.208665 pypkg_builder-0.1/src/pypkg_builder/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-23 21:48:27.000000 pypkg_builder-0.1/src/pypkg_builder/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 21:54:27.208665 pypkg_builder-0.1/src/pypkg_builder.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      349 2023-07-23 21:54:27.000000 pypkg_builder-0.1/src/pypkg_builder.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      252 2023-07-23 21:54:27.000000 pypkg_builder-0.1/src/pypkg_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-23 21:54:27.000000 pypkg_builder-0.1/src/pypkg_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        7 2023-07-23 21:54:27.000000 pypkg_builder-0.1/src/pypkg_builder.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       14 2023-07-23 21:54:27.000000 pypkg_builder-0.1/src/pypkg_builder.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.413703 pypkg_builder-1.0/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-23 23:32:13.000000 pypkg_builder-1.0/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4267 2023-07-23 23:33:56.413703 pypkg_builder-1.0/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3861 2023-07-23 23:32:13.000000 pypkg_builder-1.0/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-23 23:33:56.413703 pypkg_builder-1.0/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      841 2023-07-23 23:32:13.000000 pypkg_builder-1.0/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.409703 pypkg_builder-1.0/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.413703 pypkg_builder-1.0/src/pypkg_builder/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/__init__.py
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3605 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/app.py
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      997 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/license.py
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1221 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/readme.py
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     2227 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/setuptoolfn.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.413703 pypkg_builder-1.0/src/pypkg_builder/templates/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       58 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/templates/help.html
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    10685 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/templates/index.html
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     2142 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/tree.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.413703 pypkg_builder-1.0/src/pypkg_builder/types/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/Apache Version 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/GNU GPLv3.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/MIT License.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/Mozilla Public License 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/The Unlicense.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:32:13.000000 pypkg_builder-1.0/src/pypkg_builder/types/user_defined.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-23 23:33:56.413703 pypkg_builder-1.0/src/pypkg_builder.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4267 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      789 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       72 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       25 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       14 2023-07-23 23:33:56.000000 pypkg_builder-1.0/src/pypkg_builder.egg-info/top_level.txt
```

### Comparing `pypkg_builder-0.1/setup.py` & `pypkg_builder-1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="pypkg_builder",
-    version="0.1",
-    description="Testing tool for package",
+    version="1.0",
+    description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
+    url="https://github.com/dipson94/packagemaker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dipson",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=['pandas'],
+    install_requires=['pyperclip','flask','datetime'],
     python_requires=">=3.10",
-   
+    entry_points={
+        'console_scripts': [
+            'pysetup=template_pypackage_builder.__init__:app.run',
+        ],
+    },
 )
```

