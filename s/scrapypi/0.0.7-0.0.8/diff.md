# Comparing `tmp/scrapypi-0.0.7.tar.gz` & `tmp/scrapypi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapypi-0.0.7.tar", last modified: Thu Jul 20 17:53:04 2023, max compression
+gzip compressed data, was "scrapypi-0.0.8.tar", last modified: Mon Jul 24 01:21:23 2023, max compression
```

## Comparing `scrapypi-0.0.7.tar` & `scrapypi-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-20 17:53:04.930780 scrapypi-0.0.7/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      700 2023-07-20 16:34:55.000000 scrapypi-0.0.7/CHANGELOG.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-07-17 13:44:26.000000 scrapypi-0.0.7/LICENCE.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.7/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2617 2023-07-20 17:53:04.930780 scrapypi-0.0.7/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2043 2023-07-20 17:51:30.000000 scrapypi-0.0.7/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-20 17:53:04.926780 scrapypi-0.0.7/scrapypi/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-20 17:50:01.000000 scrapypi-0.0.7/scrapypi/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     4733 2023-07-20 15:59:41.000000 scrapypi-0.0.7/scrapypi/handler.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     4172 2023-07-20 17:48:28.000000 scrapypi-0.0.7/scrapypi/scrapypi.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-20 17:53:04.930780 scrapypi-0.0.7/scrapypi/stubs/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-17 12:33:53.000000 scrapypi-0.0.7/scrapypi/stubs/__init__.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      230 2023-07-17 15:49:11.000000 scrapypi-0.0.7/scrapypi/stubs/scrapypi.pyi
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-20 17:53:04.930780 scrapypi-0.0.7/scrapypi.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2617 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      367 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       24 2023-07-20 17:53:04.000000 scrapypi-0.0.7/scrapypi.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-20 17:53:04.930780 scrapypi-0.0.7/setup.cfg
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1900 2023-07-20 17:50:12.000000 scrapypi-0.0.7/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-24 01:21:23.367544 scrapypi-0.0.8/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      700 2023-07-20 16:34:55.000000 scrapypi-0.0.8/CHANGELOG.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-07-17 13:44:26.000000 scrapypi-0.0.8/LICENCE.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.8/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2433 2023-07-24 01:21:23.367544 scrapypi-0.0.8/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1859 2023-07-24 01:16:53.000000 scrapypi-0.0.8/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-24 01:21:23.359543 scrapypi-0.0.8/scrapypi/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-24 01:17:43.000000 scrapypi-0.0.8/scrapypi/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     4733 2023-07-20 15:59:41.000000 scrapypi-0.0.8/scrapypi/handler.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     4172 2023-07-20 21:03:55.000000 scrapypi-0.0.8/scrapypi/scrapypi.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-24 01:21:23.367544 scrapypi-0.0.8/scrapypi/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-17 12:33:53.000000 scrapypi-0.0.8/scrapypi/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      230 2023-07-17 15:49:11.000000 scrapypi-0.0.8/scrapypi/stubs/scrapypi.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-24 01:21:23.367544 scrapypi-0.0.8/scrapypi.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2433 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      367 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       14 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       24 2023-07-24 01:21:22.000000 scrapypi-0.0.8/scrapypi.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-24 01:21:23.367544 scrapypi-0.0.8/setup.cfg
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1912 2023-07-24 01:18:06.000000 scrapypi-0.0.8/setup.py
```

### Comparing `scrapypi-0.0.7/CHANGELOG.md` & `scrapypi-0.0.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.7/LICENCE.txt` & `scrapypi-0.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.7/PKG-INFO` & `scrapypi-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -29,26 +29,27 @@
 
 ```bash
 $ scrapypi
 ```
 
 Below are examples and functions and classes in scrapypi for data fetching.
 
-- stats
 - info
+- stats
 - version
 
 ### **info**
 
 Get package information. You can either get information using package name or package pypi url.
 
 ```python
 from scrapypi import info, stats, licence
 
-info(<package_name>) # returns a dictionary of information.
+# returns a dictionary of information.
+info(<package_name>)
 ```
 
 values returned by info() is listed below:
 
 - name
 - author
 - licence
@@ -62,43 +63,34 @@
 Get package full statistics, including download values everyday of package upload, date and number of downloads.
 
 ```python
 from scrapypi import stats
 
 statistics = stats(<package_name>)
 
-statistics.dataset() # get all daily download counts of package in the year.
+# get all daily download counts of package in the year.
+statistics.dataset()
 
-statistics.get_total() # get total number of downloads.
+# get total number of downloads.
+statistics.get_total()
 ```
 
 ### **version**
 
 You can also get package name and version using the version function.
 
 ```python
 from scrapypi import version
 
-version(<package_name>) # returns package name and version in a tuple. (name, version)
+# returns package name and version in a tuple. (name, version)
+version(<package_name>)
 ```
 
 > Use the version function if you need to get those information fast. But i recommend using the info function.
 
 ### **main**
 
 The main function is to get a statics view of packages and also compare the statistics of multiple packages. Use the **main()** function to run the scrapypi script for statistics fetcher. Fetching multiple packages needs to be seperated with a comma (,)
 
 ```
 Package Name(s): package_one, package_two
 ```
-
-> ### **CHANGELOG**
->
-> **0.0.7** -- [ 20 JULY 2023 ]  
-> [ ADDED ]  
-> [+] Previous version
->
-> [ FIXED ]  
-> [+] Total amount of package downloads
->
-> [ CHANGED ]  
-> [+] Interface
```

### Comparing `scrapypi-0.0.7/README.md` & `scrapypi-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 
 ```bash
 $ scrapypi
 ```
 
 Below are examples and functions and classes in scrapypi for data fetching.
 
-- stats
 - info
+- stats
 - version
 
 ### **info**
 
 Get package information. You can either get information using package name or package pypi url.
 
 ```python
 from scrapypi import info, stats, licence
 
-info(<package_name>) # returns a dictionary of information.
+# returns a dictionary of information.
+info(<package_name>)
 ```
 
 values returned by info() is listed below:
 
 - name
 - author
 - licence
@@ -45,43 +46,34 @@
 Get package full statistics, including download values everyday of package upload, date and number of downloads.
 
 ```python
 from scrapypi import stats
 
 statistics = stats(<package_name>)
 
-statistics.dataset() # get all daily download counts of package in the year.
+# get all daily download counts of package in the year.
+statistics.dataset()
 
-statistics.get_total() # get total number of downloads.
+# get total number of downloads.
+statistics.get_total()
 ```
 
 ### **version**
 
 You can also get package name and version using the version function.
 
 ```python
 from scrapypi import version
 
-version(<package_name>) # returns package name and version in a tuple. (name, version)
+# returns package name and version in a tuple. (name, version)
+version(<package_name>)
 ```
 
 > Use the version function if you need to get those information fast. But i recommend using the info function.
 
 ### **main**
 
 The main function is to get a statics view of packages and also compare the statistics of multiple packages. Use the **main()** function to run the scrapypi script for statistics fetcher. Fetching multiple packages needs to be seperated with a comma (,)
 
 ```
 Package Name(s): package_one, package_two
 ```
-
-> ### **CHANGELOG**
->
-> **0.0.7** -- [ 20 JULY 2023 ]  
-> [ ADDED ]  
-> [+] Previous version
->
-> [ FIXED ]  
-> [+] Total amount of package downloads
->
-> [ CHANGED ]  
-> [+] Interface
```

### Comparing `scrapypi-0.0.7/scrapypi/handler.py` & `scrapypi-0.0.8/scrapypi/handler.py`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.7/scrapypi/scrapypi.py` & `scrapypi-0.0.8/scrapypi/scrapypi.py`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.7/scrapypi.egg-info/PKG-INFO` & `scrapypi-0.0.8/scrapypi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -29,26 +29,27 @@
 
 ```bash
 $ scrapypi
 ```
 
 Below are examples and functions and classes in scrapypi for data fetching.
 
-- stats
 - info
+- stats
 - version
 
 ### **info**
 
 Get package information. You can either get information using package name or package pypi url.
 
 ```python
 from scrapypi import info, stats, licence
 
-info(<package_name>) # returns a dictionary of information.
+# returns a dictionary of information.
+info(<package_name>)
 ```
 
 values returned by info() is listed below:
 
 - name
 - author
 - licence
@@ -62,43 +63,34 @@
 Get package full statistics, including download values everyday of package upload, date and number of downloads.
 
 ```python
 from scrapypi import stats
 
 statistics = stats(<package_name>)
 
-statistics.dataset() # get all daily download counts of package in the year.
+# get all daily download counts of package in the year.
+statistics.dataset()
 
-statistics.get_total() # get total number of downloads.
+# get total number of downloads.
+statistics.get_total()
 ```
 
 ### **version**
 
 You can also get package name and version using the version function.
 
 ```python
 from scrapypi import version
 
-version(<package_name>) # returns package name and version in a tuple. (name, version)
+# returns package name and version in a tuple. (name, version)
+version(<package_name>)
 ```
 
 > Use the version function if you need to get those information fast. But i recommend using the info function.
 
 ### **main**
 
 The main function is to get a statics view of packages and also compare the statistics of multiple packages. Use the **main()** function to run the scrapypi script for statistics fetcher. Fetching multiple packages needs to be seperated with a comma (,)
 
 ```
 Package Name(s): package_one, package_two
 ```
-
-> ### **CHANGELOG**
->
-> **0.0.7** -- [ 20 JULY 2023 ]  
-> [ ADDED ]  
-> [+] Previous version
->
-> [ FIXED ]  
-> [+] Total amount of package downloads
->
-> [ CHANGED ]  
-> [+] Interface
```

### Comparing `scrapypi-0.0.7/setup.py` & `scrapypi-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     LONG_DESCRIPTION = readme.read()
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Get PyPi Package information.'
 KEYWORDS = ['pypi', 'information', 'package', 'module', 'stats', 'info', 'scrape']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
@@ -55,13 +55,13 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     licence='GNU LGPLv3',
     long_description=LONG_DESCRIPTION,
     packages=[data for data in data_ref],
     package_data=data_ref,
     python_requires='>=3.7',
-    install_requires=['wget'],
+    install_requires=['wget', 'requests'],
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
     py_modules=['scrapypi'],
     entry_points = {'console_scripts':['scrapypi = scrapypi:main']},
 )
```

