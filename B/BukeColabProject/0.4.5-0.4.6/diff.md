# Comparing `tmp/BukeColabProject-0.4.5.tar.gz` & `tmp/BukeColabProject-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BukeColabProject-0.4.5.tar", last modified: Mon Jul 24 12:50:10 2023, max compression
+gzip compressed data, was "dist\BukeColabProject-0.4.6.tar", last modified: Mon Jul 24 13:11:46 2023, max compression
```

## Comparing `BukeColabProject-0.4.5.tar` & `BukeColabProject-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/BukeColabProject/
--rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8928 2023-07-24 12:49:56.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-0.4.5/BukeColabProject/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.5/BukeColabProject/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.5/BukeColabProject/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.5/BukeColabProject/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.5/BukeColabProject/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.5/BukeColabProject/generate_trading_days.py
--rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.5/BukeColabProject/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.5/BukeColabProject/parameter.py
--rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.5/BukeColabProject/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.5/BukeColabProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 12:50:09.000000 BukeColabProject-0.4.5/BukeColabProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 12:50:10.000000 BukeColabProject-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-24 12:49:56.000000 BukeColabProject-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/
+drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject/
+-rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8974 2023-07-24 13:11:32.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.6/BukeColabProject/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.6/BukeColabProject/generate_day_price.py
+-rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.6/BukeColabProject/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.6/BukeColabProject/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.6/BukeColabProject/generate_trading_days.py
+-rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.6/BukeColabProject/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.6/BukeColabProject/parameter.py
+-rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.6/BukeColabProject/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.6/BukeColabProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-24 13:11:32.000000 BukeColabProject-0.4.6/setup.py
```

### Comparing `BukeColabProject-0.4.5/BukeColabProject/Buke_S002_buy_list.py` & `BukeColabProject-0.4.6/BukeColabProject/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/Buke_S002_sell_list.py` & `BukeColabProject-0.4.6/BukeColabProject/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/Buke_S004_buy_list.py` & `BukeColabProject-0.4.6/BukeColabProject/Buke_S004_buy_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
                 pre_buy_list.append(ticker_data)
         except:
             continue
 
     pre_buy_list.sort(reverse=True)
 
     pre_buy_list = pre_buy_list[:10]
+    print(pre_buy_list)
 
     basket = {'종목코드': [],'종목명':[], '매수가격1': []}
 
     for priority_value, ticker in pre_buy_list:
 
         try:
             yesterday_low = int(day_price[ticker]['저가'].loc[trading_days_list[-1]])
@@ -209,9 +210,11 @@
             basket['종목코드'].append(ticker)
             basket['종목명'].append(ticker_name)
             basket['매수가격1'].append(f"{buy_price1}원")
 
         except:
             continue
 
+    print(basket)
+
     df = pd.DataFrame(basket)
     df.to_csv(f"{path}/buy_4_{str(day)[-5:]}.txt")
```

### Comparing `BukeColabProject-0.4.5/BukeColabProject/Buke_S004_sell_list.py` & `BukeColabProject-0.4.6/BukeColabProject/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/function.py` & `BukeColabProject-0.4.6/BukeColabProject/function.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/generate_day_price.py` & `BukeColabProject-0.4.6/BukeColabProject/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/generate_index_day_price.py` & `BukeColabProject-0.4.6/BukeColabProject/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/generate_stock_list.py` & `BukeColabProject-0.4.6/BukeColabProject/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/generate_trading_days.py` & `BukeColabProject-0.4.6/BukeColabProject/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/indicator.py` & `BukeColabProject-0.4.6/BukeColabProject/indicator.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/parameter.py` & `BukeColabProject-0.4.6/BukeColabProject/parameter.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject/tools.py` & `BukeColabProject-0.4.6/BukeColabProject/tools.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/BukeColabProject.egg-info/SOURCES.txt` & `BukeColabProject-0.4.6/BukeColabProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.5/setup.py` & `BukeColabProject-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BukeColabProject", # Replace with your own username
-    version="0.4.5",
+    version="0.4.6",
     author="Example Author",
     author_email="yesben214@gamil.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

