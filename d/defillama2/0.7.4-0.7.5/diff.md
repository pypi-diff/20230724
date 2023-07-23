# Comparing `tmp/defillama2-0.7.4.tar.gz` & `tmp/defillama2-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillama2-0.7.4.tar", last modified: Fri May 19 23:19:20 2023, max compression
+gzip compressed data, was "defillama2-0.7.5.tar", last modified: Sun Jul 23 23:20:31 2023, max compression
```

## Comparing `defillama2-0.7.4.tar` & `defillama2-0.7.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.955956 defillama2-0.7.4/
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.931118 defillama2-0.7.4/.github/
--rw-r--r--   0 gmlang     (501) staff       (20)       70 2023-01-16 09:23:00.000000 defillama2-0.7.4/.github/FUNDING.yml
--rw-r--r--   0 gmlang     (501) staff       (20)       36 2022-10-05 00:39:49.000000 defillama2-0.7.4/.gitignore
--rw-r--r--   0 gmlang     (501) staff       (20)     1073 2022-10-05 00:37:39.000000 defillama2-0.7.4/LICENSE
--rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-05-19 23:19:20.955559 defillama2-0.7.4/PKG-INFO
--rw-r--r--   0 gmlang     (501) staff       (20)     4745 2023-01-16 09:23:00.000000 defillama2-0.7.4/README.md
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.932647 defillama2-0.7.4/defillama2/
--rw-r--r--   0 gmlang     (501) staff       (20)       33 2022-10-05 02:49:32.000000 defillama2-0.7.4/defillama2/__init__.py
--rw-r--r--   0 gmlang     (501) staff       (20)    48782 2023-05-19 23:09:12.000000 defillama2-0.7.4/defillama2/defillama2.py
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.936743 defillama2-0.7.4/defillama2/deprecated/
--rw-r--r--   0 gmlang     (501) staff       (20)     2580 2022-12-25 02:07:22.000000 defillama2-0.7.4/defillama2/deprecated/get_daily_open_close.py
--rw-r--r--   0 gmlang     (501) staff       (20)     3548 2022-12-25 02:07:35.000000 defillama2-0.7.4/defillama2/deprecated/get_tokens_hist_prices.py
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.935711 defillama2-0.7.4/defillama2.egg-info/
--rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/PKG-INFO
--rw-r--r--   0 gmlang     (501) staff       (20)      713 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/SOURCES.txt
--rw-r--r--   0 gmlang     (501) staff       (20)        1 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/dependency_links.txt
--rw-r--r--   0 gmlang     (501) staff       (20)       45 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/requires.txt
--rw-r--r--   0 gmlang     (501) staff       (20)       11 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/top_level.txt
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.952210 defillama2-0.7.4/notebooks/
--rw-r--r--   0 gmlang     (501) staff       (20)    37377 2022-12-29 06:01:51.000000 defillama2-0.7.4/notebooks/defillama_api_bridges.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    66566 2022-12-29 06:07:03.000000 defillama2-0.7.4/notebooks/defillama_api_coins.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    86058 2022-12-29 06:10:14.000000 defillama2-0.7.4/notebooks/defillama_api_fees_and_revenue.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    74996 2022-12-29 06:12:00.000000 defillama2-0.7.4/notebooks/defillama_api_stablecoins.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)     1443 2023-04-28 00:46:34.000000 defillama2-0.7.4/notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py
--rw-r--r--   0 gmlang     (501) staff       (20)  1281090 2022-12-29 06:39:00.000000 defillama2-0.7.4/notebooks/defillama_api_tvl.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    69598 2022-12-29 06:41:14.000000 defillama2-0.7.4/notebooks/defillama_api_volumes.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)   363834 2022-12-29 06:55:51.000000 defillama2-0.7.4/notebooks/defillama_api_yields.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)       38 2023-05-19 23:19:20.956065 defillama2-0.7.4/setup.cfg
--rw-r--r--   0 gmlang     (501) staff       (20)     1080 2023-05-19 23:10:11.000000 defillama2-0.7.4/setup.py
--rw-r--r--   0 gmlang     (501) staff       (20)   305716 2022-10-05 03:53:55.000000 defillama2-0.7.4/splash.png
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.103190 defillama2-0.7.5/
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.050670 defillama2-0.7.5/.github/
+-rw-r--r--   0 gmlang     (501) staff       (20)       70 2023-01-16 09:23:00.000000 defillama2-0.7.5/.github/FUNDING.yml
+-rw-r--r--   0 gmlang     (501) staff       (20)       36 2022-10-05 00:39:49.000000 defillama2-0.7.5/.gitignore
+-rw-r--r--   0 gmlang     (501) staff       (20)     1073 2022-10-05 00:37:39.000000 defillama2-0.7.5/LICENSE
+-rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-07-23 23:20:31.102437 defillama2-0.7.5/PKG-INFO
+-rw-r--r--   0 gmlang     (501) staff       (20)     4745 2023-01-16 09:23:00.000000 defillama2-0.7.5/README.md
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.051592 defillama2-0.7.5/defillama2/
+-rw-r--r--   0 gmlang     (501) staff       (20)       33 2022-10-05 02:49:32.000000 defillama2-0.7.5/defillama2/__init__.py
+-rw-r--r--   0 gmlang     (501) staff       (20)    48752 2023-07-23 23:17:00.000000 defillama2-0.7.5/defillama2/defillama2.py
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.055259 defillama2-0.7.5/defillama2/deprecated/
+-rw-r--r--   0 gmlang     (501) staff       (20)     2580 2022-12-25 02:07:22.000000 defillama2-0.7.5/defillama2/deprecated/get_daily_open_close.py
+-rw-r--r--   0 gmlang     (501) staff       (20)     3548 2022-12-25 02:07:35.000000 defillama2-0.7.5/defillama2/deprecated/get_tokens_hist_prices.py
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.054088 defillama2-0.7.5/defillama2.egg-info/
+-rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-07-23 23:20:30.000000 defillama2-0.7.5/defillama2.egg-info/PKG-INFO
+-rw-r--r--   0 gmlang     (501) staff       (20)      713 2023-07-23 23:20:30.000000 defillama2-0.7.5/defillama2.egg-info/SOURCES.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)        1 2023-07-23 23:20:30.000000 defillama2-0.7.5/defillama2.egg-info/dependency_links.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)       45 2023-07-23 23:20:30.000000 defillama2-0.7.5/defillama2.egg-info/requires.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)       11 2023-07-23 23:20:30.000000 defillama2-0.7.5/defillama2.egg-info/top_level.txt
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-07-23 23:20:31.090540 defillama2-0.7.5/notebooks/
+-rw-r--r--   0 gmlang     (501) staff       (20)    37377 2022-12-29 06:01:51.000000 defillama2-0.7.5/notebooks/defillama_api_bridges.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    66566 2022-12-29 06:07:03.000000 defillama2-0.7.5/notebooks/defillama_api_coins.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    86058 2022-12-29 06:10:14.000000 defillama2-0.7.5/notebooks/defillama_api_fees_and_revenue.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    74996 2022-12-29 06:12:00.000000 defillama2-0.7.5/notebooks/defillama_api_stablecoins.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)     1443 2023-04-28 00:46:34.000000 defillama2-0.7.5/notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py
+-rw-r--r--   0 gmlang     (501) staff       (20)  1281090 2022-12-29 06:39:00.000000 defillama2-0.7.5/notebooks/defillama_api_tvl.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    69598 2022-12-29 06:41:14.000000 defillama2-0.7.5/notebooks/defillama_api_volumes.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)   363834 2022-12-29 06:55:51.000000 defillama2-0.7.5/notebooks/defillama_api_yields.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)       38 2023-07-23 23:20:31.103362 defillama2-0.7.5/setup.cfg
+-rw-r--r--   0 gmlang     (501) staff       (20)     1080 2023-07-23 23:18:22.000000 defillama2-0.7.5/setup.py
+-rw-r--r--   0 gmlang     (501) staff       (20)   305716 2022-10-05 03:53:55.000000 defillama2-0.7.5/splash.png
```

### Comparing `defillama2-0.7.4/LICENSE` & `defillama2-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/PKG-INFO` & `defillama2-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillama2
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python client for DefiLlama API
 Home-page: https://github.com/coindataschool/defillama2
 Author: Coin Data School
 Author-email: <coindataschool@gmail.com>
 Keywords: python 3,defillama,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama2-0.7.4/README.md` & `defillama2-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/defillama2/defillama2.py` & `defillama2-0.7.5/defillama2/defillama2.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,16 +774,15 @@
             index=range(1))
         # volume by dex
         df = pd.DataFrame(resp['protocols'])\
             .query("latestFetchIsOk == True & disabled == False")
         ha = df['breakdown24h']
         volume_by_dex = df.drop(columns=[
             'latestFetchIsOk', 'disabled', 'module', 'logo', 'protocolType', 
-            'displayName', 'methodology', 'methodologyURL', 'breakdown24h', 
-            'protocolsStats'])
+            'displayName', 'methodology', 'methodologyURL', 'breakdown24h',])
         # volume by dex by chain
         volume_by_dex_by_chain = \
             pd.concat([pd.DataFrame(ha.iloc[i]) for i in range(len(ha))])\
             .stack().reset_index()
         volume_by_dex_by_chain.columns = ['protocol', 'chain', 'total24h']
         # daily volume of all dexes
         daily_volume = pd.DataFrame(resp['totalDataChart'])
```

### Comparing `defillama2-0.7.4/defillama2/deprecated/get_daily_open_close.py` & `defillama2-0.7.5/defillama2/deprecated/get_daily_open_close.py`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/defillama2/deprecated/get_tokens_hist_prices.py` & `defillama2-0.7.5/defillama2/deprecated/get_tokens_hist_prices.py`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/defillama2.egg-info/PKG-INFO` & `defillama2-0.7.5/defillama2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillama2
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python client for DefiLlama API
 Home-page: https://github.com/coindataschool/defillama2
 Author: Coin Data School
 Author-email: <coindataschool@gmail.com>
 Keywords: python 3,defillama,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama2-0.7.4/defillama2.egg-info/SOURCES.txt` & `defillama2-0.7.5/defillama2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_bridges.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_bridges.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_coins.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_coins.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_fees_and_revenue.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_fees_and_revenue.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_stablecoins.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_stablecoins.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py` & `defillama2-0.7.5/notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_tvl.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_tvl.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_volumes.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_volumes.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/notebooks/defillama_api_yields.ipynb` & `defillama2-0.7.5/notebooks/defillama_api_yields.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.4/setup.py` & `defillama2-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
-VERSION = '0.7.4'
+VERSION = '0.7.5'
 
 packages = ['defillama2']
 requires = ['requests>=2.28.1', 'pandas>=1.4.4', 'numpy>=1.22.4']
 
 with open('README.md', mode='r') as f:
     readme = f.read()
```

### Comparing `defillama2-0.7.4/splash.png` & `defillama2-0.7.5/splash.png`

 * *Files identical despite different names*

