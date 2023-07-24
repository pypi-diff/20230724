# Comparing `tmp/ML-Algo-1.3.tar.gz` & `tmp/ML-Algo-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.3.tar", last modified: Tue Jul 18 13:09:31 2023, max compression
+gzip compressed data, was "ML-Algo-1.3.1.tar", last modified: Mon Jul 24 06:33:52 2023, max compression
```

## Comparing `ML-Algo-1.3.tar` & `ML-Algo-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:09:31.469804 ML-Algo-1.3/
-drwxrwxrwx   0        0        0        0 2023-07-18 13:09:31.464800 ML-Algo-1.3/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.3/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     2364 2023-07-17 06:12:40.000000 ML-Algo-1.3/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.3/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2649 2023-07-18 13:08:47.000000 ML-Algo-1.3/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.3/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0     2517 2023-07-13 11:01:26.000000 ML-Algo-1.3/ML_Algo/TestRun.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.3/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:09:31.468798 ML-Algo-1.3/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0     2237 2023-07-18 13:09:31.000000 ML-Algo-1.3/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-18 13:09:31.000000 ML-Algo-1.3/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:09:31.000000 ML-Algo-1.3/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 13:09:31.000000 ML-Algo-1.3/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 13:09:31.000000 ML-Algo-1.3/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2237 2023-07-18 13:09:31.469804 ML-Algo-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 13:09:31.470802 ML-Algo-1.3/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-07-18 13:08:53.000000 ML-Algo-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:33:52.225114 ML-Algo-1.3.1/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:33:52.214255 ML-Algo-1.3.1/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.3.1/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     2364 2023-07-17 06:12:40.000000 ML-Algo-1.3.1/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.3.1/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2616 2023-07-24 06:02:33.000000 ML-Algo-1.3.1/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.3.1/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0     2517 2023-07-13 11:01:26.000000 ML-Algo-1.3.1/ML_Algo/TestRun.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.3.1/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:33:52.222729 ML-Algo-1.3.1/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0     2239 2023-07-24 06:33:51.000000 ML-Algo-1.3.1/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-24 06:33:51.000000 ML-Algo-1.3.1/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:33:51.000000 ML-Algo-1.3.1/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-24 06:33:51.000000 ML-Algo-1.3.1/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 06:33:51.000000 ML-Algo-1.3.1/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2239 2023-07-24 06:33:52.225114 ML-Algo-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:33:52.226124 ML-Algo-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-24 06:32:03.000000 ML-Algo-1.3.1/setup.py
```

### Comparing `ML-Algo-1.3/ML_Algo/DataCleaning.py` & `ML-Algo-1.3.1/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.3/ML_Algo/FetchData.py` & `ML-Algo-1.3.1/ML_Algo/FetchData.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.3/ML_Algo/Predictions.py` & `ML-Algo-1.3.1/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.3/ML_Algo/Series_Data.py` & `ML-Algo-1.3.1/ML_Algo/Series_Data.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
 
 
 def combine_json_data(json_files):
     combined_df = pd.DataFrame()
 
     for index, json_data in enumerate(json_files):
-        print(index, json_data)
         if 'data' not in json_data:
             continue  # Skip this iteration if 'data' key is not present
 
         data = json_data['data']['10751']
         df = pd.DataFrame(data)
         df['ts'] = pd.to_datetime(df['ts'], format="%m/%d/%Y %I:%M:%S %p")
         df['ts'] = df['ts'].dt.strftime('%H:%M')
```

### Comparing `ML-Algo-1.3/ML_Algo/Series_Time.py` & `ML-Algo-1.3.1/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.3/ML_Algo/TestRun.py` & `ML-Algo-1.3.1/ML_Algo/TestRun.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.3/ML_Algo.egg-info/PKG-INFO` & `ML-Algo-1.3.1/ML_Algo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.3
+Version: 1.3.1
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.3 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.3.1 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
```

### Comparing `ML-Algo-1.3/PKG-INFO` & `ML-Algo-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.3
+Version: 1.3.1
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.3 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.3.1 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
```

### Comparing `ML-Algo-1.3/setup.py` & `ML-Algo-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ML-Algo',
-    version='1.3',
+    version='1.3.1',
     author='Mr Raj',
     author_email='arunraj14092002@gmail.com',
     description='A package for calculating Series Time Data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['ML_Algo'],
     install_requires=['pandas','requests'],
```

