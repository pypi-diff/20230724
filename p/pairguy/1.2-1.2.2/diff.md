# Comparing `tmp/pairguy-1.2.tar.gz` & `tmp/pairguy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pairguy-1.2.tar", last modified: Fri Jul 21 01:42:43 2023, max compression
+gzip compressed data, was "pairguy-1.2.2.tar", last modified: Mon Jul 24 04:35:54 2023, max compression
```

## Comparing `pairguy-1.2.tar` & `pairguy-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.430554 pairguy-1.2/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-07-21 01:42:43.430326 pairguy-1.2/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 pairguy-1.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.428817 pairguy-1.2/pairguy/
--rw-r--r--   0 cmw        (501) staff       (20)    26742 2023-07-20 23:24:02.000000 pairguy-1.2/pairguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    17010 2023-07-20 23:24:02.000000 pairguy-1.2/pairguy/pairguy_Aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    71232 2023-07-21 01:25:59.000000 pairguy-1.2/pairguy/pairguy_Components.py
--rw-r--r--   0 cmw        (501) staff       (20)    32787 2023-07-21 01:34:12.000000 pairguy-1.2/pairguy/pairguy_EquityCurves.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.430047 pairguy-1.2/pairguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      283 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-21 01:42:43.430626 pairguy-1.2/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      830 2023-07-21 01:42:07.000000 pairguy-1.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 04:35:54.177077 pairguy-1.2.2/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-07-24 04:35:54.176818 pairguy-1.2.2/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 pairguy-1.2.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 04:35:54.175460 pairguy-1.2.2/pairguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    26742 2023-07-20 23:24:02.000000 pairguy-1.2.2/pairguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    17010 2023-07-20 23:24:02.000000 pairguy-1.2.2/pairguy/pairguy_Aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    71425 2023-07-24 04:33:56.000000 pairguy-1.2.2/pairguy/pairguy_Components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    32787 2023-07-21 01:34:12.000000 pairguy-1.2.2/pairguy/pairguy_EquityCurves.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 04:35:54.176632 pairguy-1.2.2/pairguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-07-24 04:35:53.000000 pairguy-1.2.2/pairguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      283 2023-07-24 04:35:53.000000 pairguy-1.2.2/pairguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-07-24 04:35:53.000000 pairguy-1.2.2/pairguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-07-24 04:35:53.000000 pairguy-1.2.2/pairguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-07-24 04:35:53.000000 pairguy-1.2.2/pairguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-24 04:35:54.177125 pairguy-1.2.2/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-07-24 04:35:13.000000 pairguy-1.2.2/setup.py
```

### Comparing `pairguy-1.2/pairguy/__init__.py` & `pairguy-1.2.2/pairguy/__init__.py`

 * *Files identical despite different names*

### Comparing `pairguy-1.2/pairguy/pairguy_Aggregate.py` & `pairguy-1.2.2/pairguy/pairguy_Aggregate.py`

 * *Files identical despite different names*

### Comparing `pairguy-1.2/pairguy/pairguy_Components.py` & `pairguy-1.2.2/pairguy/pairguy_Components.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,27 +292,32 @@
 
 
 
         per_col_1_1.append(html.Div('Number of Trade'))
         per_col_1_1.append(html.Div('Net Profit'))
         per_col_1_1.append(html.Div('Net Profit/MDD'))
         per_col_1_1.append(html.Div('Return on Capital'))
+        per_col_1_1.append(html.Div(html.Img()))
         per_col_1_1.append(html.Div('Ann. Return'))
         per_col_1_1.append(html.Div('Ann. Std'))
         per_col_1_1.append(html.Div('Ann. Sharpe Ratio'))
         per_col_1_1.append(html.Div('MDD Dollar'))
         per_col_1_1.append(html.Div('MDD Percentage'))
+        per_col_1_1.append(html.Div(html.Img()))
         per_col_1_1.append(html.Div('Win Rate'))
         per_col_1_1.append(html.Div('COV (Count)'))
         per_col_1_1.append(html.Div('COV (Return)'))
         per_col_1_1.append(html.Div('Total Commission'))
         per_col_1_1.append(html.Div('Risk Free Rate'))
 
         for i in range(13):
             per_col_1_2.append(html.Div(df[keys[i]], style={'text-align': 'center'}))
+            if (i == 3) or (i == 8):
+                per_col_1_2.append(html.Div(html.Img()))
+
         try:
             per_col_1_2.append(html.Div( "{:.2%}".format(risk_free_rate / 100) , style={'text-align': 'center'}))
         except:
             per_col_1_2.append(html.Div('-----', style={'text-align': 'center'}))
 
         # for i in range(7, 13):
         #     per_col_2_2.append(html.Div(str(df[keys[i]]), style={'text-align': 'center'}))
```

### Comparing `pairguy-1.2/pairguy/pairguy_EquityCurves.py` & `pairguy-1.2.2/pairguy/pairguy_EquityCurves.py`

 * *Files identical despite different names*

### Comparing `pairguy-1.2/setup.py` & `pairguy-1.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pairguy",
-    version="1.2",
+    version="1.2.2",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Pairguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas==1.5.3',
```

