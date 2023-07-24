# Comparing `tmp/docrawl-1.0.1.tar.gz` & `tmp/docrawl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.0.1.tar", last modified: Mon Jul 24 17:57:04 2023, max compression
+gzip compressed data, was "docrawl-1.0.2.tar", last modified: Mon Jul 24 18:01:23 2023, max compression
```

## Comparing `docrawl-1.0.1.tar` & `docrawl-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.801751 docrawl-1.0.1/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      568 2023-07-24 17:57:04.801751 docrawl-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.786791 docrawl-1.0.1/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-1.0.1/docrawl/__init__.py
--rw-rw-rw-   0        0        0    11453 2023-07-13 10:34:35.000000 docrawl-1.0.1/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    36466 2023-07-24 17:55:36.000000 docrawl-1.0.1/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2023-07-13 10:34:35.000000 docrawl-1.0.1/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-1.0.1/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-1.0.1/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.800753 docrawl-1.0.1/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 17:57:04.801751 docrawl-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-07-24 17:57:00.000000 docrawl-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:01:23.594891 docrawl-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-07-24 18:01:23.594891 docrawl-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 18:01:23.583920 docrawl-1.0.2/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-1.0.2/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    11453 2023-07-13 10:34:35.000000 docrawl-1.0.2/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    36561 2023-07-24 18:01:02.000000 docrawl-1.0.2/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2023-07-13 10:34:35.000000 docrawl-1.0.2/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-1.0.2/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-1.0.2/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:01:23.594891 docrawl-1.0.2/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-24 18:01:22.000000 docrawl-1.0.2/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-24 18:01:23.000000 docrawl-1.0.2/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:01:23.000000 docrawl-1.0.2/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-24 18:01:23.000000 docrawl-1.0.2/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 18:01:23.000000 docrawl-1.0.2/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 18:01:23.595888 docrawl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-07-24 18:01:20.000000 docrawl-1.0.2/setup.py
```

### Comparing `docrawl-1.0.1/LICENSE` & `docrawl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.1/PKG-INFO` & `docrawl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-1.0.1/docrawl/docrawl_client.py` & `docrawl-1.0.2/docrawl/docrawl_client.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.1/docrawl/docrawl_core.py` & `docrawl-1.0.2/docrawl/docrawl_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,18 +111,19 @@
             if self.headless:
                 self.options.add_argument("--headless")
 
                 # For headless mode different width of window is needed
                 window_size_x = 1450
 
             try:
-                self.browser = webdriver.Chrome(options=self.options, desired_capabilities=capabilities,
+                self.browser = webdriver.Chrome(options=self.options,#, desired_capabilities=capabilities,
                                                 executable_path=ChromeDriverManager().install())
-            except:
-                pass
+            except Exception as e:
+                docrawl_logger.error("Error: Browser could not be intialized",e)
+                
 
         window_size_x = 1820
 
         self.browser.set_window_size(window_size_x, 980)
 
         return self.browser
```

### Comparing `docrawl-1.0.1/docrawl/docrawl_launcher.py` & `docrawl-1.0.2/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.1/docrawl/docrawl_logger.py` & `docrawl-1.0.2/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.1/docrawl/elements.py` & `docrawl-1.0.2/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.1/docrawl.egg-info/PKG-INFO` & `docrawl-1.0.2/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-1.0.1/setup.py` & `docrawl-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.0.1',
+    version='1.0.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

