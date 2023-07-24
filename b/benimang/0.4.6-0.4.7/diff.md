# Comparing `tmp/benimang-0.4.6.tar.gz` & `tmp/benimang-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.6.tar", last modified: Mon Jul 24 03:57:08 2023, max compression
+gzip compressed data, was "benimang-0.4.7.tar", last modified: Mon Jul 24 06:34:29 2023, max compression
```

## Comparing `benimang-0.4.6.tar` & `benimang-0.4.7.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.390165 benimang-0.4.6/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-24 03:57:08.389164 benimang-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.384164 benimang-0.4.6/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.6/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.6/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bexecute.py
--rw-rw-rw-   0        0        0     2706 2023-07-24 03:53:29.000000 benimang-0.4.6/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.6/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-22 08:10:55.000000 benimang-0.4.6/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.6/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.6/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.6/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/btable.py
--rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.6/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.6/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.6/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.387164 benimang-0.4.6/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-24 03:54:05.000000 benimang-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 03:57:08.390165 benimang-0.4.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.388165 benimang-0.4.6/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.6/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.204159 benimang-0.4.7/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-24 06:34:29.203158 benimang-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.199158 benimang-0.4.7/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.7/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6313 2023-07-24 06:29:19.000000 benimang-0.4.7/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2762 2023-07-24 06:21:16.000000 benimang-0.4.7/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.7/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-22 08:10:55.000000 benimang-0.4.7/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.7/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.7/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.7/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/btable.py
+-rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.7/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.7/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.7/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.202159 benimang-0.4.7/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-24 06:30:49.000000 benimang-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:34:29.204159 benimang-0.4.7/setup.cfg
```

### Comparing `benimang-0.4.6/beni/bbyte.py` & `benimang-0.4.7/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bcache.py` & `benimang-0.4.7/beni/bcache.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from beni.bfunc import getWrapped
 
 _foreverDatetime = datetime(9999, 9, 9)
 
 
 class BCacheFileManager:
 
-    def __init__(self, cacheDir: Path) -> None:
-        self._cacheDir = cacheDir
+    def __init__(self, cachePath: Path) -> None:
+        self._cachePath = cachePath
         self._waitingWriteDeadlineFile = False
-        self._deadlineFile = cacheDir.joinpath('deadline.dat')
+        self._deadlineFile = cachePath.joinpath('deadline.dat')
         if self._deadlineFile.exists():
             try:
                 with open(self._deadlineFile, 'rb') as f:
                     self._deadlineDict = pickle.loads(f.read())
             except:
                 self._deadlineDict = {}
         else:
@@ -73,15 +73,15 @@
         else:
             await bpath.remove(file)
 
     async def clear(self, key: str):
         await bpath.remove(self._getFile(key))
 
     def _getFile(self, key: str):
-        return bpath.get(self._cacheDir, bfunc.crcStr(key))
+        return bpath.get(self._cachePath, bfunc.crcStr(key))
 
     async def _updateDeadlineFile(self):
         if not self._waitingWriteDeadlineFile:
             self._waitingWriteDeadlineFile = True
             asyncio.create_task(
                 self._writeDeadlineFile()
             )
```

### Comparing `benimang-0.4.6/beni/bcolor.py` & `benimang-0.4.7/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bexecute.py` & `benimang-0.4.7/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bfile.py` & `benimang-0.4.7/beni/bfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,8 +96,10 @@
     ary.sort()
     for substr in ary:
         subAry = substr.replace('\r\n', '\n').split('\n')
         fileName = subAry.pop(0)
         if subAry:
             file = output / fileName
             bcolor.printYellow(file)
-            await bfile.writeText(file, '\n'.join(subAry))
+            msg = '\n'.join(subAry).strip()
+            if msg:
+                await bfile.writeText(file, msg)
```

### Comparing `benimang-0.4.6/beni/bfunc.py` & `benimang-0.4.7/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bhttp.py` & `benimang-0.4.7/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/binput.py` & `benimang-0.4.7/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/block.py` & `benimang-0.4.7/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/blog.py` & `benimang-0.4.7/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bpath.py` & `benimang-0.4.7/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bplaywright.py` & `benimang-0.4.7/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bprogress.py` & `benimang-0.4.7/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bqiniu.py` & `benimang-0.4.7/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bsqlite.py` & `benimang-0.4.7/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bstorage.py` & `benimang-0.4.7/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/btable.py` & `benimang-0.4.7/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/btask.py` & `benimang-0.4.7/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/btime.py` & `benimang-0.4.7/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.6/beni/bzip.py` & `benimang-0.4.7/beni/bzip.py`

 * *Files identical despite different names*

