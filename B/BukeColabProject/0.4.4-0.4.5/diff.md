# Comparing `tmp/BukeColabProject-0.4.4.tar.gz` & `tmp/BukeColabProject-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BukeColabProject-0.4.4.tar", last modified: Mon Jul 24 12:44:07 2023, max compression
+gzip compressed data, was "dist\BukeColabProject-0.4.5.tar", last modified: Mon Jul 24 12:50:10 2023, max compression
```

## Comparing `BukeColabProject-0.4.4.tar` & `BukeColabProject-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:44:07.000000 BukeColabProject-0.4.4/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:44:07.000000 BukeColabProject-0.4.4/BukeColabProject/
--rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.4/BukeColabProject/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.4/BukeColabProject/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8920 2023-07-24 12:27:22.000000 BukeColabProject-0.4.4/BukeColabProject/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-0.4.4/BukeColabProject/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.4/BukeColabProject/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.4/BukeColabProject/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.4/BukeColabProject/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.4/BukeColabProject/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.4/BukeColabProject/generate_trading_days.py
--rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.4/BukeColabProject/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.4/BukeColabProject/parameter.py
--rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.4/BukeColabProject/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.4/BukeColabProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:44:07.000000 BukeColabProject-0.4.4/BukeColabProject.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 12:44:06.000000 BukeColabProject-0.4.4/BukeColabProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 12:44:06.000000 BukeColabProject-0.4.4/BukeColabProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-07-24 12:44:06.000000 BukeColabProject-0.4.4/BukeColabProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 12:44:06.000000 BukeColabProject-0.4.4/BukeColabProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 12:44:07.000000 BukeColabProject-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 12:44:07.000000 BukeColabProject-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-24 12:43:56.000000 BukeColabProject-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/BukeColabProject/
+-rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8928 2023-07-24 12:49:56.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.5/BukeColabProject/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.5/BukeColabProject/generate_day_price.py
+-rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.5/BukeColabProject/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.5/BukeColabProject/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.5/BukeColabProject/generate_trading_days.py
+-rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.5/BukeColabProject/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.5/BukeColabProject/parameter.py
+-rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.5/BukeColabProject/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.5/BukeColabProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-24 12:49:56.000000 BukeColabProject-0.4.5/setup.py
```

### Comparing `BukeColabProject-0.4.4/BukeColabProject/Buke_S002_buy_list.py` & `BukeColabProject-0.4.5/BukeColabProject/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/Buke_S002_sell_list.py` & `BukeColabProject-0.4.5/BukeColabProject/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/Buke_S004_buy_list.py` & `BukeColabProject-0.4.5/BukeColabProject/Buke_S004_buy_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 import pandas as pd
 from pandas import DataFrame
 
 from BukeColabProject.indicator import sma, ibs, pivot_standard, stochastic_fast_d, stochastic_fast_k, 순거래대금
-from BukeColabProject.function import rank
+from BukeColabProject.function import rank, ts_min
 from BukeColabProject.parameter import Market, MovingAverage
 from BukeColabProject.tools import get_ask_price
 
 
 def str_to_date(trading_day: str) -> date:
     return date(int(trading_day[:4]), int(trading_day[5:7]), int(trading_day[8:]))
```

### Comparing `BukeColabProject-0.4.4/BukeColabProject/Buke_S004_sell_list.py` & `BukeColabProject-0.4.5/BukeColabProject/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/function.py` & `BukeColabProject-0.4.5/BukeColabProject/function.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/generate_day_price.py` & `BukeColabProject-0.4.5/BukeColabProject/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/generate_index_day_price.py` & `BukeColabProject-0.4.5/BukeColabProject/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/generate_stock_list.py` & `BukeColabProject-0.4.5/BukeColabProject/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/generate_trading_days.py` & `BukeColabProject-0.4.5/BukeColabProject/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/indicator.py` & `BukeColabProject-0.4.5/BukeColabProject/indicator.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/parameter.py` & `BukeColabProject-0.4.5/BukeColabProject/parameter.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject/tools.py` & `BukeColabProject-0.4.5/BukeColabProject/tools.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/BukeColabProject.egg-info/SOURCES.txt` & `BukeColabProject-0.4.5/BukeColabProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.4/setup.py` & `BukeColabProject-0.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BukeColabProject", # Replace with your own username
-    version="0.4.4",
+    version="0.4.5",
     author="Example Author",
     author_email="yesben214@gamil.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

