# Comparing `tmp/avirtech_spraying_jiyi_lib-0.0.1.tar.gz` & `tmp/avirtech_spraying_jiyi_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avirtech_spraying_jiyi_lib-0.0.1.tar", last modified: Mon Jul 24 06:33:59 2023, max compression
+gzip compressed data, was "avirtech_spraying_jiyi_lib-0.0.3.tar", last modified: Mon Jul 24 08:59:23 2023, max compression
```

## Comparing `avirtech_spraying_jiyi_lib-0.0.1.tar` & `avirtech_spraying_jiyi_lib-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:33:59.456773 avirtech_spraying_jiyi_lib-0.0.1/
--rw-rw-rw-   0        0        0      934 2023-07-24 06:33:59.455818 avirtech_spraying_jiyi_lib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-01-10 06:21:10.000000 avirtech_spraying_jiyi_lib-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 06:33:59.408101 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib/
--rw-rw-rw-   0        0        0       47 2023-07-24 06:25:07.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib/__init__.py
--rw-rw-rw-   0        0        0    31165 2023-07-24 06:14:24.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:33:59.452780 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/
--rw-rw-rw-   0        0        0      934 2023-07-24 06:33:57.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-07-24 06:33:59.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:33:58.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-24 06:33:58.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-24 06:33:58.000000 avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 06:33:59.456773 avirtech_spraying_jiyi_lib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-07-24 06:22:30.000000 avirtech_spraying_jiyi_lib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:59:23.912001 avirtech_spraying_jiyi_lib-0.0.3/
+-rw-rw-rw-   0        0        0     1193 2023-07-24 08:59:23.912001 avirtech_spraying_jiyi_lib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-07-24 08:58:08.000000 avirtech_spraying_jiyi_lib-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 08:59:23.895047 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib/
+-rw-rw-rw-   0        0        0       47 2023-07-24 08:46:59.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib/__init__.py
+-rw-rw-rw-   0        0        0    31181 2023-07-24 08:55:43.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:59:23.910006 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/
+-rw-rw-rw-   0        0        0     1193 2023-07-24 08:59:23.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-07-24 08:59:23.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 08:59:23.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-24 08:59:23.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-24 08:59:23.000000 avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 08:59:23.912998 avirtech_spraying_jiyi_lib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-07-24 06:56:22.000000 avirtech_spraying_jiyi_lib-0.0.3/setup.py
```

### Comparing `avirtech_spraying_jiyi_lib-0.0.1/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py` & `avirtech_spraying_jiyi_lib-0.0.3/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 from matplotlib.ticker import (MultipleLocator, AutoMinorLocator)
 
 class autocorrect:
     @staticmethod
     def process_all():
 
         mxd = arcpy.mapping.MapDocument("Current")
-        arcpy.env.workspace = "Current"
-        global df
+        mxd.author = "Avirtech"
+        arcpy.env.workspace = "CURRENT"
         df = arcpy.mapping.ListDataFrames(mxd)[0]
 
+
         ws = Tk()
         ws.title('Input Data')
         ws.geometry('380x450')
 
         ##  Mode Data
         label1 = Label(ws, text="Pilih Mode Data", font= ('Helvetica 12'))
         label1.pack(pady=5)
```

### Comparing `avirtech_spraying_jiyi_lib-0.0.1/setup.py` & `avirtech_spraying_jiyi_lib-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup( 
     name="avirtech_spraying_jiyi_lib",
-    version="0.0.1",
-    description="Avirtech Python Library to Generate track drone spraying FC JIYI",
+    version="0.0.3",
+    description="Avirtech Python Library to Generate drone spraying error with palm location",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Mohammad ILham R",
     author_email="ilhamr.mohammad@gmail.com",
     license="MIT",
     classifiers=[
@@ -32,9 +32,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["avirtech_spraying_jiyi_lib"],
     include_package_data=True,
-    install_requires=["simpledbf","matplotlib", "numpy","pathlib"]
+    install_requires=["simpledbf","numpy","matplotlib","pathlib"]
 )
```

