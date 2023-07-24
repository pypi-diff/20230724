# Comparing `tmp/BukeColabProject-0.4.2.tar.gz` & `tmp/BukeColabProject-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BukeColabProject-0.4.2.tar", last modified: Sun Apr 23 08:47:01 2023, max compression
+gzip compressed data, was "dist\BukeColabProject-0.4.3.tar", last modified: Mon Jul 24 12:28:25 2023, max compression
```

## Comparing `BukeColabProject-0.4.2.tar` & `BukeColabProject-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/
-drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/BukeColabProject/
--rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.2/BukeColabProject/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.2/BukeColabProject/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.2/BukeColabProject/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.2/BukeColabProject/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.2/BukeColabProject/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.2/BukeColabProject/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.2/BukeColabProject/generate_trading_days.py
--rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.2/BukeColabProject/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.2/BukeColabProject/parameter.py
--rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.2/BukeColabProject/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.2/BukeColabProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      472 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-04-23 08:46:17.000000 BukeColabProject-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:28:25.000000 BukeColabProject-0.4.3/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:28:25.000000 BukeColabProject-0.4.3/BukeColabProject/
+-rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.3/BukeColabProject/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.3/BukeColabProject/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8920 2023-07-24 12:27:22.000000 BukeColabProject-0.4.3/BukeColabProject/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17289 2023-07-24 12:27:22.000000 BukeColabProject-0.4.3/BukeColabProject/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.3/BukeColabProject/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.3/BukeColabProject/generate_day_price.py
+-rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.3/BukeColabProject/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.3/BukeColabProject/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.3/BukeColabProject/generate_trading_days.py
+-rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.3/BukeColabProject/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.3/BukeColabProject/parameter.py
+-rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.3/BukeColabProject/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.3/BukeColabProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:28:25.000000 BukeColabProject-0.4.3/BukeColabProject.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:28:24.000000 BukeColabProject-0.4.3/BukeColabProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 12:28:24.000000 BukeColabProject-0.4.3/BukeColabProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:28:24.000000 BukeColabProject-0.4.3/BukeColabProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 12:28:24.000000 BukeColabProject-0.4.3/BukeColabProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 12:28:25.000000 BukeColabProject-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:28:25.000000 BukeColabProject-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-24 12:27:22.000000 BukeColabProject-0.4.3/setup.py
```

### Comparing `BukeColabProject-0.4.2/BukeColabProject/Buke_S002_buy_list.py` & `BukeColabProject-0.4.3/BukeColabProject/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/Buke_S002_sell_list.py` & `BukeColabProject-0.4.3/BukeColabProject/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/function.py` & `BukeColabProject-0.4.3/BukeColabProject/function.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/generate_day_price.py` & `BukeColabProject-0.4.3/BukeColabProject/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/generate_index_day_price.py` & `BukeColabProject-0.4.3/BukeColabProject/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/generate_stock_list.py` & `BukeColabProject-0.4.3/BukeColabProject/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/generate_trading_days.py` & `BukeColabProject-0.4.3/BukeColabProject/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/indicator.py` & `BukeColabProject-0.4.3/BukeColabProject/indicator.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/parameter.py` & `BukeColabProject-0.4.3/BukeColabProject/parameter.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject/tools.py` & `BukeColabProject-0.4.3/BukeColabProject/tools.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.2/BukeColabProject.egg-info/SOURCES.txt` & `BukeColabProject-0.4.3/BukeColabProject.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 README.md
 setup.py
 BukeColabProject/Buke_S002_buy_list.py
 BukeColabProject/Buke_S002_sell_list.py
+BukeColabProject/Buke_S004_buy_list.py
+BukeColabProject/Buke_S004_sell_list.py
 BukeColabProject/__init__.py
 BukeColabProject/function.py
 BukeColabProject/generate_day_price.py
 BukeColabProject/generate_index_day_price.py
 BukeColabProject/generate_stock_list.py
 BukeColabProject/generate_trading_days.py
 BukeColabProject/indicator.py
```

### Comparing `BukeColabProject-0.4.2/setup.py` & `BukeColabProject-0.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BukeColabProject", # Replace with your own username
-    version="0.4.2",
+    version="0.4.3",
     author="Example Author",
     author_email="yesben214@gamil.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

