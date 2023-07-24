# Comparing `tmp/shareddata-2.1.1.tar.gz` & `tmp/shareddata-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.1.1.tar", last modified: Mon Jul 24 01:28:50 2023, max compression
+gzip compressed data, was "shareddata-2.1.2.tar", last modified: Mon Jul 24 01:30:52 2023, max compression
```

## Comparing `shareddata-2.1.1.tar` & `shareddata-2.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:28:50.049148 shareddata-2.1.1/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.1/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:28:50.049148 shareddata-2.1.1/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.1/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.1/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-24 01:28:50.049148 shareddata-2.1.1/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:28:50.049148 shareddata-2.1.1/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:28:50.049148 shareddata-2.1.1/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.1/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/SeriesLib.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.1/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.1/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/SharedDataAWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.1/src/SharedData/SharedDataFeeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.1/src/SharedData/SharedDataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14997 2023-07-24 01:04:18.000000 shareddata-2.1.1/src/SharedData/SharedDataPeriod.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.1/src/SharedData/SharedDataRealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28691 2023-07-18 17:59:43.000000 shareddata-2.1.1/src/SharedData/SharedDataTable.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.1/src/SharedData/SharedDataTableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.1/src/SharedData/SharedDataTableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21252 2023-07-24 01:28:24.000000 shareddata-2.1.1/src/SharedData/SharedDataTimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.1/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.1/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.1/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:28:50.049148 shareddata-2.1.1/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:28:50.000000 shareddata-2.1.1/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-24 01:28:50.000000 shareddata-2.1.1/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-24 01:28:50.000000 shareddata-2.1.1/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-24 01:28:50.000000 shareddata-2.1.1/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-24 01:28:50.000000 shareddata-2.1.1/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.2/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:30:52.823783 shareddata-2.1.2/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.2/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.2/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-24 01:30:52.823783 shareddata-2.1.2/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.2/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SeriesLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.2/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.2/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SharedDataAWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.2/src/SharedData/SharedDataFeeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.2/src/SharedData/SharedDataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14997 2023-07-24 01:04:18.000000 shareddata-2.1.2/src/SharedData/SharedDataPeriod.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.2/src/SharedData/SharedDataRealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28691 2023-07-18 17:59:43.000000 shareddata-2.1.2/src/SharedData/SharedDataTable.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.2/src/SharedData/SharedDataTableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.2/src/SharedData/SharedDataTableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21114 2023-07-24 01:30:39.000000 shareddata-2.1.2/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.2/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.2/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.2/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:30:52.823783 shareddata-2.1.2/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-24 01:30:52.000000 shareddata-2.1.2/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.1.1/LICENSE` & `shareddata-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/PKG-INFO` & `shareddata-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.1
+Version: 2.1.2
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.1/README.md` & `shareddata-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/setup.cfg` & `shareddata-2.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.1.1
+version = 2.1.2
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.1.1/src/SharedData/Defaults.py` & `shareddata-2.1.2/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/Logger.py` & `shareddata-2.1.2/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.1.2/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/Metadata.py` & `shareddata-2.1.2/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/MultiProc.py` & `shareddata-2.1.2/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SeriesLib.py` & `shareddata-2.1.2/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedData.py` & `shareddata-2.1.2/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.1.2/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.1.2/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataFeeder.py` & `shareddata-2.1.2/src/SharedData/SharedDataFeeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataFrame.py` & `shareddata-2.1.2/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataPeriod.py` & `shareddata-2.1.2/src/SharedData/SharedDataPeriod.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataRealTime.py` & `shareddata-2.1.2/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.1.2/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataTable.py` & `shareddata-2.1.2/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataTableIndex.py` & `shareddata-2.1.2/src/SharedData/SharedDataTableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataTableIndexJit.py` & `shareddata-2.1.2/src/SharedData/SharedDataTableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.1.2/src/SharedData/SharedDataTimeSeries.py`

 * *Files 7% similar despite different names*

```diff
@@ -299,95 +299,95 @@
         sidx = np.array([self.get_loc_symbol(s) for s in _cols])
         ts = _idx.values.astype(np.int64)/10**9 #seconds
         tidx = self.get_loc_timestamp(ts)
         self.setValuesJit(self.data.values,tidx,sidx,_data)
         data_io.close()
         return _header[4]
  
-    # # WRITE
-    # def write(self, startDate=None):
-    #     firstdate = self.data.first_valid_index()
-    #     if not startDate is None:
-    #         firstdate = startDate
+    # WRITE
+    def write(self, startDate=None):
+        firstdate = self.data.first_valid_index()
+        if not startDate is None:
+            firstdate = startDate
         
-    #     path, shm_name = self.get_path()
+        path, shm_name = self.get_path()
         
-    #     partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
-    #     threads = []
+        partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
+        threads = []
 
-    #     mtime = datetime.now().timestamp()        
-    #     if firstdate<partdate:
-    #         # write head
-    #         threads = [*threads , \
-    #             Thread(target=SharedDataTimeSeries.write_timeseries_df,\
-    #                 args=(self,self.data.loc[:partdate], str(path / (self.tag+'_head.bin')), mtime) )]
-    #     # write tail
-    #     threads = [*threads , \
-    #             Thread(target=SharedDataTimeSeries.write_timeseries_df,\
-    #                 args=(self,self.data.loc[partdate:], str(path / (self.tag+'_tail.bin')), mtime) )]
+        mtime = datetime.now().timestamp()        
+        if firstdate<partdate:
+            # write head
+            threads = [*threads , \
+                Thread(target=SharedDataTimeSeries.write_timeseries_df,\
+                    args=(self,self.data.loc[:partdate], str(path / (self.tag+'_head.bin')), mtime) )]
+        # write tail
+        threads = [*threads , \
+                Thread(target=SharedDataTimeSeries.write_timeseries_df,\
+                    args=(self,self.data.loc[partdate:], str(path / (self.tag+'_tail.bin')), mtime) )]
 
-    #     for i in range(len(threads)):
-    #         threads[i].start()
+        for i in range(len(threads)):
+            threads[i].start()
 
-    #     for i in range(len(threads)):
-    #         threads[i].join()
+        for i in range(len(threads)):
+            threads[i].join()
         
-    # def write_timeseries_df(self,df,tag_path,mtime):
-    #     ts_io = SharedDataTimeSeries.create_timeseries_io(df)        
-    #     threads=[]
-    #     if self.sharedData.s3write:
-    #         ts_io.seek(0)
-    #         gzip_io = io.BytesIO()
-    #         with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
-    #             shutil.copyfileobj(ts_io, gz)
-
-    #         threads = [*threads , \
-    #             Thread(target=S3Upload,args=(gzip_io, tag_path+'.gzip', mtime) )]
-
-    #     if self.sharedData.save_local:
-    #         threads = [*threads , \
-    #             Thread(target=SharedDataTimeSeries.write_file, args=(ts_io, tag_path, mtime) )]
+    def write_timeseries_df(self,df,tag_path,mtime):
+        ts_io = SharedDataTimeSeries.create_timeseries_io(df)        
+        threads=[]
+        if self.sharedData.s3write:
+            ts_io.seek(0)
+            gzip_io = io.BytesIO()
+            with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
+                shutil.copyfileobj(ts_io, gz)
+
+            threads = [*threads , \
+                Thread(target=S3Upload,args=(gzip_io, tag_path+'.gzip', mtime) )]
+
+        if self.sharedData.save_local:
+            threads = [*threads , \
+                Thread(target=SharedDataTimeSeries.write_file, args=(ts_io, tag_path, mtime) )]
                             
-    #     for i in range(len(threads)):
-    #         threads[i].start()
+        for i in range(len(threads)):
+            threads[i].start()
 
-    #     for i in range(len(threads)):
-    #         threads[i].join()
+        for i in range(len(threads)):
+            threads[i].join()
 
-    # def create_timeseries_io(df):
-    #     df = df.dropna(how='all',axis=0)
-    #     r, c = df.shape
-    #     idx = (df.index.astype(np.int64))
-    #     idx_b = idx.values.tobytes()
-    #     cols = df.columns.values
-    #     colscsv = ','.join(cols)
-    #     colscsv_b = str.encode(colscsv,encoding='UTF-8',errors='ignore')
-    #     nbidx = len(idx_b)
-    #     nbcols = len(colscsv_b)
-    #     data = np.ascontiguousarray(df.values.astype(np.float64))
-    #     header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
-    #     #calculate hash
-    #     m = hashlib.md5(idx_b)
-    #     m.update(colscsv_b)
-    #     m.update(data)
-    #     md5hash_b = m.digest()
-    #     # allocate memory
-    #     io_obj = io.BytesIO()
-    #     io_obj.write(header)
-    #     io_obj.write(idx_b)
-    #     io_obj.write(colscsv_b)
-    #     io_obj.write(data)
-    #     io_obj.write(md5hash_b)
-    #     return io_obj
-
-    # def write_file(io_obj,path,mtime):
-    #     with open(path, 'wb') as f:
-    #         f.write(io_obj.getbuffer())
-    #         f.flush()
-    #     os.utime(path, (mtime, mtime))
+    def create_timeseries_io(df):
+        df = df.dropna(how='all',axis=0)
+        r, c = df.shape
+        idx = (df.index.astype(np.int64))
+        idx_b = idx.values.tobytes()
+        cols = df.columns.values
+        colscsv = ','.join(cols)
+        colscsv_b = str.encode(colscsv,encoding='UTF-8',errors='ignore')
+        nbidx = len(idx_b)
+        nbcols = len(colscsv_b)
+        data = np.ascontiguousarray(df.values.astype(np.float64))
+        header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
+        #calculate hash
+        m = hashlib.md5(idx_b)
+        m.update(colscsv_b)
+        m.update(data)
+        md5hash_b = m.digest()
+        # allocate memory
+        io_obj = io.BytesIO()
+        io_obj.write(header)
+        io_obj.write(idx_b)
+        io_obj.write(colscsv_b)
+        io_obj.write(data)
+        io_obj.write(md5hash_b)
+        return io_obj
+
+    def write_file(io_obj,path,mtime):
+        with open(path, 'wb') as f:
+            f.write(io_obj.getbuffer())
+            f.flush()
+        os.utime(path, (mtime, mtime))
 
     # MESSAGES
     def broadcast(self,idx,col):
         SharedDataRealTime.broadcast(
             self.sharedData,
             self.feeder,
             self.period,
```

### Comparing `shareddata-2.1.1/src/SharedData/SharedNumpy.py` & `shareddata-2.1.2/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/SharedData/Utils.py` & `shareddata-2.1.2/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.1/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.1.2/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.1
+Version: 2.1.2
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.1/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.1.2/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

