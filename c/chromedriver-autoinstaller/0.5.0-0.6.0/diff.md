# Comparing `tmp/chromedriver-autoinstaller-0.5.0.tar.gz` & `tmp/chromedriver-autoinstaller-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-autoinstaller-0.5.0.tar", last modified: Mon Jul 24 04:09:58 2023, max compression
+gzip compressed data, was "chromedriver-autoinstaller-0.6.0.tar", last modified: Mon Jul 24 04:10:33 2023, max compression
```

## Comparing `chromedriver-autoinstaller-0.5.0.tar` & `chromedriver-autoinstaller-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:09:58.374864 chromedriver-autoinstaller-0.5.0/
--rw-r--r--   0 crysbe     (501) staff       (20)     1068 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.5.0/LICENSE
--rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:09:58.374918 chromedriver-autoinstaller-0.5.0/PKG-INFO
--rw-r--r--   0 crysbe     (501) staff       (20)      847 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.5.0/README.md
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:09:58.374285 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller/
--rw-r--r--   0 crysbe     (501) staff       (20)     1422 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller/__init__.py
--rw-r--r--   0 crysbe     (501) staff       (20)    11777 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller/utils.py
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:09:58.374776 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/
--rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:09:58.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/PKG-INFO
--rw-r--r--   0 crysbe     (501) staff       (20)      364 2023-07-24 04:09:58.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 crysbe     (501) staff       (20)        1 2023-07-24 04:09:58.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       95 2023-07-24 04:09:58.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/entry_points.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       27 2023-07-24 04:09:58.000000 chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/top_level.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       79 2023-07-24 04:09:58.375074 chromedriver-autoinstaller-0.5.0/setup.cfg
--rw-r--r--   0 crysbe     (501) staff       (20)     1984 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.5.0/setup.py
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.092650 chromedriver-autoinstaller-0.6.0/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1068 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/LICENSE
+-rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:10:33.092703 chromedriver-autoinstaller-0.6.0/PKG-INFO
+-rw-r--r--   0 crysbe     (501) staff       (20)      847 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/README.md
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.091954 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1422 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/__init__.py
+-rw-r--r--   0 crysbe     (501) staff       (20)    11777 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/utils.py
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.092548 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 crysbe     (501) staff       (20)      364 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)        1 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       95 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/entry_points.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       27 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/top_level.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       79 2023-07-24 04:10:33.092883 chromedriver-autoinstaller-0.6.0/setup.cfg
+-rw-r--r--   0 crysbe     (501) staff       (20)     1984 2023-07-24 04:10:27.000000 chromedriver-autoinstaller-0.6.0/setup.py
```

### Comparing `chromedriver-autoinstaller-0.5.0/LICENSE` & `chromedriver-autoinstaller-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.5.0/PKG-INFO` & `chromedriver-autoinstaller-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.5.0
+Version: 0.6.0
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
 Keywords: chromedriver chrome chromium selenium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-autoinstaller-0.5.0/README.md` & `chromedriver-autoinstaller-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller/__init__.py` & `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller/utils.py` & `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.5.0/chromedriver_autoinstaller.egg-info/PKG-INFO` & `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.5.0
+Version: 0.6.0
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
 Keywords: chromedriver chrome chromium selenium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-autoinstaller-0.5.0/setup.py` & `chromedriver-autoinstaller-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         shutil.rmtree("dist")
     if os.path.isdir("chromedriver_autoinstaller.egg-info"):
         shutil.rmtree("chromedriver_autoinstaller.egg-info")
 
 
 setup(
     name="chromedriver-autoinstaller",
-    version="0.5.0",
+    version="0.6.0",
     author="Yeongbin Jo",
     author_email="iam.yeongbin.jo@gmail.com",
     description="Automatically install chromedriver that supports the currently installed version of chrome.",
     license="MIT",
     keywords="chromedriver chrome chromium selenium",
     url="https://github.com/yeongbin-jo/python-chromedriver-autoinstaller",
     packages=["chromedriver_autoinstaller"],
```

