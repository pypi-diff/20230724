# Comparing `tmp/chromedriver-autoinstaller-0.6.0.tar.gz` & `tmp/chromedriver-autoinstaller-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-autoinstaller-0.6.0.tar", last modified: Mon Jul 24 04:10:33 2023, max compression
+gzip compressed data, was "chromedriver-autoinstaller-0.6.1.tar", last modified: Mon Jul 24 04:18:02 2023, max compression
```

## Comparing `chromedriver-autoinstaller-0.6.0.tar` & `chromedriver-autoinstaller-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.092650 chromedriver-autoinstaller-0.6.0/
--rw-r--r--   0 crysbe     (501) staff       (20)     1068 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/LICENSE
--rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:10:33.092703 chromedriver-autoinstaller-0.6.0/PKG-INFO
--rw-r--r--   0 crysbe     (501) staff       (20)      847 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/README.md
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.091954 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/
--rw-r--r--   0 crysbe     (501) staff       (20)     1422 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/__init__.py
--rw-r--r--   0 crysbe     (501) staff       (20)    11777 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/utils.py
-drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:10:33.092548 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/
--rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/PKG-INFO
--rw-r--r--   0 crysbe     (501) staff       (20)      364 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 crysbe     (501) staff       (20)        1 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       95 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/entry_points.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       27 2023-07-24 04:10:33.000000 chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/top_level.txt
--rw-r--r--   0 crysbe     (501) staff       (20)       79 2023-07-24 04:10:33.092883 chromedriver-autoinstaller-0.6.0/setup.cfg
--rw-r--r--   0 crysbe     (501) staff       (20)     1984 2023-07-24 04:10:27.000000 chromedriver-autoinstaller-0.6.0/setup.py
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:18:02.386473 chromedriver-autoinstaller-0.6.1/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1068 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.1/LICENSE
+-rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:18:02.386520 chromedriver-autoinstaller-0.6.1/PKG-INFO
+-rw-r--r--   0 crysbe     (501) staff       (20)      847 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.1/README.md
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:18:02.385890 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1422 2023-07-24 04:08:55.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller/__init__.py
+-rw-r--r--   0 crysbe     (501) staff       (20)    12156 2023-07-24 04:17:52.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller/utils.py
+drwxr-xr-x   0 crysbe     (501) staff       (20)        0 2023-07-24 04:18:02.386383 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/
+-rw-r--r--   0 crysbe     (501) staff       (20)     1883 2023-07-24 04:18:02.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 crysbe     (501) staff       (20)      364 2023-07-24 04:18:02.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)        1 2023-07-24 04:18:02.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       95 2023-07-24 04:18:02.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/entry_points.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       27 2023-07-24 04:18:02.000000 chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/top_level.txt
+-rw-r--r--   0 crysbe     (501) staff       (20)       79 2023-07-24 04:18:02.386676 chromedriver-autoinstaller-0.6.1/setup.cfg
+-rw-r--r--   0 crysbe     (501) staff       (20)     1984 2023-07-24 04:17:59.000000 chromedriver-autoinstaller-0.6.1/setup.py
```

### Comparing `chromedriver-autoinstaller-0.6.0/LICENSE` & `chromedriver-autoinstaller-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.6.0/PKG-INFO` & `chromedriver-autoinstaller-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.6.0
+Version: 0.6.1
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
 Keywords: chromedriver chrome chromium selenium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-autoinstaller-0.6.0/README.md` & `chromedriver-autoinstaller-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/__init__.py` & `chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller/utils.py` & `chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,22 @@
         version = (
             process.communicate()[0]
             .decode("UTF-8")
             .replace("Google Chrome", "")
             .strip()
         )
     elif platform == "win":
+        # check both of Program Files and Program Files (x86).
+        # if the version isn't found on both of them, version is an empty string.
         dirs = [f.name for f in os.scandir("C:\\Program Files\\Google\\Chrome\\Application") if f.is_dir() and re.match("^[0-9.]+$", f.name)]
-        version = max(dirs)
+        if dirs:
+            version = max(dir)
+        else:
+            dirs = [f.name for f in os.scandir("C:\\Program Files (x86)\\Google\\Chrome\\Application") if f.is_dir() and re.match("^[0-9.]+$", f.name)]
+            version = max(dirs) if dirs else ''
     else:
         return
     return version
 
 
 def get_linux_executable_path():
     """
```

### Comparing `chromedriver-autoinstaller-0.6.0/chromedriver_autoinstaller.egg-info/PKG-INFO` & `chromedriver-autoinstaller-0.6.1/chromedriver_autoinstaller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.6.0
+Version: 0.6.1
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
 Keywords: chromedriver chrome chromium selenium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-autoinstaller-0.6.0/setup.py` & `chromedriver-autoinstaller-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         shutil.rmtree("dist")
     if os.path.isdir("chromedriver_autoinstaller.egg-info"):
         shutil.rmtree("chromedriver_autoinstaller.egg-info")
 
 
 setup(
     name="chromedriver-autoinstaller",
-    version="0.6.0",
+    version="0.6.1",
     author="Yeongbin Jo",
     author_email="iam.yeongbin.jo@gmail.com",
     description="Automatically install chromedriver that supports the currently installed version of chrome.",
     license="MIT",
     keywords="chromedriver chrome chromium selenium",
     url="https://github.com/yeongbin-jo/python-chromedriver-autoinstaller",
     packages=["chromedriver_autoinstaller"],
```

