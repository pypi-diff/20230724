# Comparing `tmp/shareddata-2.1.2.tar.gz` & `tmp/shareddata-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.1.2.tar", last modified: Mon Jul 24 01:30:52 2023, max compression
+gzip compressed data, was "shareddata-2.1.3.tar", last modified: Mon Jul 24 10:10:43 2023, max compression
```

## Comparing `shareddata-2.1.2.tar` & `shareddata-2.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.2/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:30:52.823783 shareddata-2.1.2/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.2/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.2/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-24 01:30:52.823783 shareddata-2.1.2/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.2/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SeriesLib.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.2/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.2/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SharedDataAWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.2/src/SharedData/SharedDataFeeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.2/src/SharedData/SharedDataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14997 2023-07-24 01:04:18.000000 shareddata-2.1.2/src/SharedData/SharedDataPeriod.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.2/src/SharedData/SharedDataRealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28691 2023-07-18 17:59:43.000000 shareddata-2.1.2/src/SharedData/SharedDataTable.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.2/src/SharedData/SharedDataTableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.2/src/SharedData/SharedDataTableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21114 2023-07-24 01:30:39.000000 shareddata-2.1.2/src/SharedData/SharedDataTimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.2/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.2/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 10:10:43.220617 shareddata-2.1.3/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.3/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 10:10:43.220617 shareddata-2.1.3/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.3/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.3/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-24 10:10:43.220617 shareddata-2.1.3/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 10:10:43.216617 shareddata-2.1.3/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 10:10:43.220617 shareddata-2.1.3/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.3/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/SeriesLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.3/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.3/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/SharedDataAWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.3/src/SharedData/SharedDataFeeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.3/src/SharedData/SharedDataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15137 2023-07-24 01:42:34.000000 shareddata-2.1.3/src/SharedData/SharedDataPeriod.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.3/src/SharedData/SharedDataRealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28691 2023-07-18 17:59:43.000000 shareddata-2.1.3/src/SharedData/SharedDataTable.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.3/src/SharedData/SharedDataTableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.3/src/SharedData/SharedDataTableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21114 2023-07-24 01:30:39.000000 shareddata-2.1.3/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.3/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.3/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.3/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 10:10:43.220617 shareddata-2.1.3/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 10:10:43.000000 shareddata-2.1.3/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-24 10:10:43.000000 shareddata-2.1.3/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-24 10:10:43.000000 shareddata-2.1.3/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-24 10:10:43.000000 shareddata-2.1.3/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-24 10:10:43.000000 shareddata-2.1.3/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.1.2/LICENSE` & `shareddata-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/PKG-INFO` & `shareddata-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.2
+Version: 2.1.3
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.2/README.md` & `shareddata-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/setup.cfg` & `shareddata-2.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.1.2
+version = 2.1.3
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.1.2/src/SharedData/Defaults.py` & `shareddata-2.1.3/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/Logger.py` & `shareddata-2.1.3/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.1.3/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/Metadata.py` & `shareddata-2.1.3/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/MultiProc.py` & `shareddata-2.1.3/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SeriesLib.py` & `shareddata-2.1.3/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedData.py` & `shareddata-2.1.3/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.1.3/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.1.3/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataFeeder.py` & `shareddata-2.1.3/src/SharedData/SharedDataFeeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataFrame.py` & `shareddata-2.1.3/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataPeriod.py` & `shareddata-2.1.3/src/SharedData/SharedDataPeriod.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,34 +35,42 @@
         elif self.period=='M15':
             self.periodSeconds = 60*15
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M1':
             self.periodSeconds = 60
             self.default_startDate = pd.Timestamp('2010-01-01')
         self.getContinousTimeIndex(self.default_startDate)
+        self.loaded = False
+
+        
+    def load(self):
         # read if not loaded
         shdatalist = self.sharedData.list()   
         path, shm_name = self.get_path()
         idx = [shm_name in str(s) for s in shdatalist.index]
         if not np.any(idx):
             self.read()
 
+
     def __setitem__(self, tag, df):
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 self.tags[tag] = SharedDataFrame(self, tag, df)
             else:
                 self.tags[tag] = SharedDataTimeSeries(self, tag, df)
         elif isinstance(df, pd.DataFrame):
             data = self.tags[tag].data
             iidx = df.index.intersection(data.index)
             icol = df.columns.intersection(data.columns)
             data.loc[iidx, icol] = df.loc[iidx, icol].copy()
 
-    def __getitem__(self, tag):        
+    def __getitem__(self, tag):     
+        if not self.loaded:
+            self.load()   
+            self.loaded=True
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 df = SharedDataFrame(self, tag)
                 if not df.data.empty:
                     self.tags[tag] = df
                 else:
                     return pd.DataFrame([])
```

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataRealTime.py` & `shareddata-2.1.3/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.1.3/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataTable.py` & `shareddata-2.1.3/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataTableIndex.py` & `shareddata-2.1.3/src/SharedData/SharedDataTableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataTableIndexJit.py` & `shareddata-2.1.3/src/SharedData/SharedDataTableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.1.3/src/SharedData/SharedDataTimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/SharedNumpy.py` & `shareddata-2.1.3/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/SharedData/Utils.py` & `shareddata-2.1.3/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.2/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.1.3/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.2
+Version: 2.1.3
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.2/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.1.3/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

