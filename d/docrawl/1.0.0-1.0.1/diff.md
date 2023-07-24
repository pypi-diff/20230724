# Comparing `tmp/docrawl-1.0.0.tar.gz` & `tmp/docrawl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.0.0.tar", last modified: Thu Jul 13 10:36:04 2023, max compression
+gzip compressed data, was "docrawl-1.0.1.tar", last modified: Mon Jul 24 17:57:04 2023, max compression
```

## Comparing `docrawl-1.0.0.tar` & `docrawl-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.993735 docrawl-1.0.0/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      568 2023-07-13 10:36:04.993735 docrawl-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.974785 docrawl-1.0.0/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-1.0.0/docrawl/__init__.py
--rw-rw-rw-   0        0        0    11453 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    36374 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-1.0.0/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-1.0.0/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.992737 docrawl-1.0.0/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:36:04.993735 docrawl-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-07-13 10:35:43.000000 docrawl-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.801751 docrawl-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-07-24 17:57:04.801751 docrawl-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.786791 docrawl-1.0.1/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-1.0.1/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    11453 2023-07-13 10:34:35.000000 docrawl-1.0.1/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    36466 2023-07-24 17:55:36.000000 docrawl-1.0.1/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2023-07-13 10:34:35.000000 docrawl-1.0.1/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-1.0.1/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-1.0.1/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:57:04.800753 docrawl-1.0.1/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 17:57:04.000000 docrawl-1.0.1/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 17:57:04.801751 docrawl-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-07-24 17:57:00.000000 docrawl-1.0.1/setup.py
```

### Comparing `docrawl-1.0.0/LICENSE` & `docrawl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.0/PKG-INFO` & `docrawl-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-1.0.0/docrawl/docrawl_client.py` & `docrawl-1.0.1/docrawl/docrawl_client.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.0/docrawl/docrawl_core.py` & `docrawl-1.0.1/docrawl/docrawl_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
             if self.headless:
                 self.options.add_argument("--headless")
 
                 # For headless mode different width of window is needed
                 window_size_x = 1450
 
             try:
-                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities,
+                self.browser = webdriver.Firefox(options=self.options,#, capabilities=capabilities, #Capabilities deprecated in newest selenium
                                                  service=Service(GeckoDriverManager().install()))
             except Exception as e:
                 docrawl_logger.error(f'Error while creating Firefox instance {e}')
-                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities)
+                self.browser = webdriver.Firefox(options=self.options)#, capabilities=capabilities) #Capabilities deprecated in newest selenium
 
         elif self.driver_type == 'Chrome':
             capabilities = DesiredCapabilities.CHROME
             self.options = ChromeOptions()
 
             sw_options = self._set_proxy(proxy_info)
```

### Comparing `docrawl-1.0.0/docrawl/docrawl_launcher.py` & `docrawl-1.0.1/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.0/docrawl/docrawl_logger.py` & `docrawl-1.0.1/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.0/docrawl/elements.py` & `docrawl-1.0.1/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.0.0/docrawl.egg-info/PKG-INFO` & `docrawl-1.0.1/docrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-1.0.0/setup.py` & `docrawl-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.0.0',
+    version='1.0.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

