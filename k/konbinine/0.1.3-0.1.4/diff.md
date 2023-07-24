# Comparing `tmp/konbinine-0.1.3.tar.gz` & `tmp/konbinine-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konbinine-0.1.3.tar", last modified: Mon Jul 24 09:52:07 2023, max compression
+gzip compressed data, was "konbinine-0.1.4.tar", last modified: Mon Jul 24 10:12:24 2023, max compression
```

## Comparing `konbinine-0.1.3.tar` & `konbinine-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.519967 konbinine-0.1.3/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.3/LICENSE
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:52:07.519967 konbinine-0.1.3/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1408 2023-07-24 08:53:23.000000 konbinine-0.1.3/README.md
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.509967 konbinine-0.1.3/konbinine/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    27357 2023-07-24 09:26:46.000000 konbinine-0.1.3/konbinine/__init__.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.3/konbinine/enums.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.3/konbinine/exceptions.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.3/konbinine/logs.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7084 2023-07-24 08:53:23.000000 konbinine-0.1.3/konbinine/models.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      487 2023-06-29 09:15:35.000000 konbinine-0.1.3/konbinine/utils.py
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.519967 konbinine-0.1.3/konbinine.egg-info/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      382 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/SOURCES.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/dependency_links.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/requires.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/top_level.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/zip-safe
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1325 2023-07-24 09:52:01.000000 konbinine-0.1.3/pyproject.toml
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.3/requirements.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-07-24 09:52:07.519967 konbinine-0.1.3/setup.cfg
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.3/setup.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.4/LICENSE
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-07-24 10:12:24.949967 konbinine-0.1.4/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     2128 2023-07-24 10:10:35.000000 konbinine-0.1.4/README.md
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/konbinine/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    27357 2023-07-24 10:11:47.000000 konbinine-0.1.4/konbinine/__init__.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.4/konbinine/enums.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.4/konbinine/exceptions.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.4/konbinine/logs.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7084 2023-07-24 08:53:23.000000 konbinine-0.1.4/konbinine/models.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      487 2023-06-29 09:15:35.000000 konbinine-0.1.4/konbinine/utils.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/konbinine.egg-info/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      382 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/SOURCES.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/dependency_links.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/requires.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/top_level.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.4/konbinine.egg-info/zip-safe
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1268 2023-07-24 09:56:01.000000 konbinine-0.1.4/pyproject.toml
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.4/requirements.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-07-24 10:12:24.949967 konbinine-0.1.4/setup.cfg
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.4/setup.py
```

### Comparing `konbinine-0.1.3/LICENSE` & `konbinine-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.3/PKG-INFO` & `konbinine-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.3
+Version: 0.1.4
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
@@ -64,18 +64,43 @@
 **konbinine** is designed to be use with web framework (such as Django, Flask, etc) that interacts with ShotGrid. This
 library has not been tested inside Digital Content Creation (DCC) software such as Maya, 3ds Max or Houdini.
 
 Technically it should just work but that is outside the scope of this library.
 
 ### New Project
 
+#### First time setup
+
 1. Add `konbinine` to your project's `requirements.txt`.
 2. ???
 3. Profit (in improving code readability and debugging)
 
+#### Using konbinine
+
+I recommend configuring the environment variables before running the following code.
+
+Set it using your `.env` file or through the shell session etc.
+
+```shell
+# if your studio subscribed to Shotgun prior to the ShotGrid rename, the URL should
+# looks like https://yourstudioname.shotgunstudio.com or something 
+KONBINI_BASE_URL=https://yourstudioname.shotgrid.autodesk.com
+KONBINI_SCRIPT_NAME=YOURSHOTGRIDAPISCRIPTNAMEHERE
+KONBINI_API_KEY=YOURSHOTGRIDAPIKEYHERE
+```
+
+```python
+from konbinine import Konbini
+from konbinine.enums import SgEntity
+
+kon = Konbini()
+booking_schemas = kon.get_sg_entity_schema_fields(SgEntity.BOOKING)
+# whatever booking schemas results here
+```
+
 ### Existing Project that Uses shotgun_api3
 
 You will need to... rewrite/refactor your code to use **konbinine**! Pretty much the main reason why **konbinine** was
 created is to improve the Developer Experience (DX) when interacting with ShotGrid.
 
 ## Quickstart for Developers
```

### Comparing `konbinine-0.1.3/konbinine/__init__.py` & `konbinine-0.1.4/konbinine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 import calendar
 import datetime
 import logging
 import os
 from typing import List, Optional, Set, Union
```

### Comparing `konbinine-0.1.3/konbinine/enums.py` & `konbinine-0.1.4/konbinine/enums.py`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.3/konbinine/models.py` & `konbinine-0.1.4/konbinine/models.py`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.3/konbinine.egg-info/PKG-INFO` & `konbinine-0.1.4/konbinine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.3
+Version: 0.1.4
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
@@ -64,18 +64,43 @@
 **konbinine** is designed to be use with web framework (such as Django, Flask, etc) that interacts with ShotGrid. This
 library has not been tested inside Digital Content Creation (DCC) software such as Maya, 3ds Max or Houdini.
 
 Technically it should just work but that is outside the scope of this library.
 
 ### New Project
 
+#### First time setup
+
 1. Add `konbinine` to your project's `requirements.txt`.
 2. ???
 3. Profit (in improving code readability and debugging)
 
+#### Using konbinine
+
+I recommend configuring the environment variables before running the following code.
+
+Set it using your `.env` file or through the shell session etc.
+
+```shell
+# if your studio subscribed to Shotgun prior to the ShotGrid rename, the URL should
+# looks like https://yourstudioname.shotgunstudio.com or something 
+KONBINI_BASE_URL=https://yourstudioname.shotgrid.autodesk.com
+KONBINI_SCRIPT_NAME=YOURSHOTGRIDAPISCRIPTNAMEHERE
+KONBINI_API_KEY=YOURSHOTGRIDAPIKEYHERE
+```
+
+```python
+from konbinine import Konbini
+from konbinine.enums import SgEntity
+
+kon = Konbini()
+booking_schemas = kon.get_sg_entity_schema_fields(SgEntity.BOOKING)
+# whatever booking schemas results here
+```
+
 ### Existing Project that Uses shotgun_api3
 
 You will need to... rewrite/refactor your code to use **konbinine**! Pretty much the main reason why **konbinine** was
 created is to improve the Developer Experience (DX) when interacting with ShotGrid.
 
 ## Quickstart for Developers
```

### Comparing `konbinine-0.1.3/pyproject.toml` & `konbinine-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -39,13 +39,10 @@
 "Bug Reports" = "https://github.com/hueyyeng/konbini/issues"
 "Source" = "https://github.com/hueyyeng/konbini"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
-#[tool.setuptools.packages.find]
-#where = ["konbinine"]
-
 [tool.setuptools.dynamic]
 version = {attr = "konbinine.__version__"}
 dependencies = {file = "requirements.txt"}
```

### Comparing `konbinine-0.1.3/setup.cfg` & `konbinine-0.1.4/setup.cfg`

 * *Files identical despite different names*

