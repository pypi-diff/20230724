# Comparing `tmp/benimang-0.4.5.tar.gz` & `tmp/benimang-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.5.tar", last modified: Sat Jul 22 07:58:56 2023, max compression
+gzip compressed data, was "benimang-0.4.6.tar", last modified: Mon Jul 24 03:57:08 2023, max compression
```

## Comparing `benimang-0.4.5.tar` & `benimang-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 07:58:56.414405 benimang-0.4.5/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-22 07:58:56.413405 benimang-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 07:58:56.406404 benimang-0.4.5/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.5/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.5/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.5/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.5/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.5/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.5/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.5/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.5/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.5/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.5/beni/btable.py
--rw-rw-rw-   0        0        0     4616 2023-07-22 07:57:11.000000 benimang-0.4.5/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.5/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.5/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.5/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-22 07:58:56.411404 benimang-0.4.5/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-22 07:58:56.000000 benimang-0.4.5/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-22 07:58:56.000000 benimang-0.4.5/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 07:58:56.000000 benimang-0.4.5/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 07:58:56.000000 benimang-0.4.5/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-22 07:57:45.000000 benimang-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 07:58:56.414405 benimang-0.4.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 07:58:56.412405 benimang-0.4.5/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.5/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.390165 benimang-0.4.6/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-24 03:57:08.389164 benimang-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.384164 benimang-0.4.6/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.6/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.6/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2706 2023-07-24 03:53:29.000000 benimang-0.4.6/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.6/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-22 08:10:55.000000 benimang-0.4.6/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.6/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.6/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.6/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.6/beni/btable.py
+-rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.6/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.6/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.6/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.6/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.387164 benimang-0.4.6/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 03:57:08.000000 benimang-0.4.6/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-24 03:54:05.000000 benimang-0.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 03:57:08.390165 benimang-0.4.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 03:57:08.388165 benimang-0.4.6/test/
+-rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.6/test/test_sample.py
```

### Comparing `benimang-0.4.5/beni/bbyte.py` & `benimang-0.4.6/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bcache.py` & `benimang-0.4.6/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bcolor.py` & `benimang-0.4.6/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bexecute.py` & `benimang-0.4.6/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bfile.py` & `benimang-0.4.6/beni/bfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import os
 from pathlib import Path
 from typing import Any
 
 import aiofiles
 
-from beni import bfunc, block, bpath
+from beni import bcolor, bfile, bfunc, block, bpath
+from beni.btype import Null
 
 _limit = 50
 
 
 @block.useLimit(_limit)
 async def writeText(file: Path | str, content: str, encoding: str = 'utf8', newline: str = '\n'):
     file = bpath.get(file)
@@ -69,17 +71,33 @@
 async def readToml(file: Path | str):
     import tomllib
     return tomllib.loads(
         await readText(file)
     )
 
 
-async def md5File(file: Path | str):
+async def md5(file: Path | str):
     return bfunc.md5Bytes(
         await readBytes(file)
     )
 
 
-async def crcFile(file: Path | str):
+async def crc(file: Path | str):
     return bfunc.crcBytes(
         await readBytes(file)
     )
+
+
+async def makeFiles(content: str, output: Path = Null):
+    if output is Null:
+        output = Path(os.curdir).absolute()
+    ary = content.split('>>>')
+    ary = [x.strip() for x in ary]
+    ary = [x for x in ary if x]
+    ary.sort()
+    for substr in ary:
+        subAry = substr.replace('\r\n', '\n').split('\n')
+        fileName = subAry.pop(0)
+        if subAry:
+            file = output / fileName
+            bcolor.printYellow(file)
+            await bfile.writeText(file, '\n'.join(subAry))
```

### Comparing `benimang-0.4.5/beni/bfunc.py` & `benimang-0.4.6/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bhttp.py` & `benimang-0.4.6/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/binput.py` & `benimang-0.4.6/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/block.py` & `benimang-0.4.6/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/blog.py` & `benimang-0.4.6/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bpath.py` & `benimang-0.4.6/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bplaywright.py` & `benimang-0.4.6/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bprogress.py` & `benimang-0.4.6/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bqiniu.py` & `benimang-0.4.6/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bsqlite.py` & `benimang-0.4.6/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bstorage.py` & `benimang-0.4.6/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/btable.py` & `benimang-0.4.6/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/btask.py` & `benimang-0.4.6/beni/btask.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             eval(f'{module}.{cmd}')(*args, **kwargs)
     asyncio.run(func())
 
 
 @asynccontextmanager
 async def _task():
     _checkVscodeVenv()
-    bfunc.sysUtf8()
+    # bfunc.sysUtf8() # 由于不是每次都需要用到，界面显示了不美观 Active code page: 65001
     if options.binPath:
         bfunc.addEnvPath(options.binPath)
     async with block.useFileLock(options.lock):
         start_time = Datetime.now()
         bfunc.initErrorFormat()
         if options.logPath:
             logFile = bpath.get(options.logPath, btime.datetimeStr('%Y%m%d_%H%M%S.log'))
```

### Comparing `benimang-0.4.5/beni/btime.py` & `benimang-0.4.6/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/beni/bzip.py` & `benimang-0.4.6/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/benimang.egg-info/SOURCES.txt` & `benimang-0.4.6/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.4.5/test/test_sample.py` & `benimang-0.4.6/test/test_sample.py`

 * *Files identical despite different names*

