# Comparing `tmp/bcmd-0.0.7.tar.gz` & `tmp/bcmd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.7.tar", last modified: Sat Jul 22 09:27:29 2023, max compression
+gzip compressed data, was "bcmd-0.0.8.tar", last modified: Mon Jul 24 06:41:18 2023, max compression
```

## Comparing `bcmd-0.0.7.tar` & `bcmd-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:27:29.520556 bcmd-0.0.7/
--rw-rw-rw-   0        0        0      233 2023-07-22 09:27:29.520556 bcmd-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-22 09:27:29.509554 bcmd-0.0.7/bcmd/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.7/bcmd/__init__.py
--rw-rw-rw-   0        0        0      473 2023-07-22 06:56:21.000000 bcmd-0.0.7/bcmd/dev.py
--rw-rw-rw-   0        0        0      259 2023-07-22 02:11:10.000000 bcmd-0.0.7/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:27:29.519556 bcmd-0.0.7/bcmd/tasks/
--rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.7/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-22 09:04:30.000000 bcmd-0.0.7/bcmd/tasks/mirrors.py
--rw-rw-rw-   0        0        0     2380 2023-07-22 09:24:15.000000 bcmd-0.0.7/bcmd/tasks/time.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:27:29.516556 bcmd-0.0.7/bcmd.egg-info/
--rw-rw-rw-   0        0        0      233 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      149 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 09:27:29.000000 bcmd-0.0.7/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      616 2023-07-22 09:27:04.000000 bcmd-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 09:27:29.520556 bcmd-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.798607 bcmd-0.0.8/
+-rw-rw-rw-   0        0        0      233 2023-07-24 06:41:18.798607 bcmd-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.784828 bcmd-0.0.8/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.8/bcmd/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-07-24 03:57:58.000000 bcmd-0.0.8/bcmd/dev.py
+-rw-rw-rw-   0        0        0      259 2023-07-24 01:26:53.000000 bcmd-0.0.8/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.797608 bcmd-0.0.8/bcmd/tasks/
+-rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.8/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-07-24 03:16:35.000000 bcmd-0.0.8/bcmd/tasks/bin.py
+-rw-rw-rw-   0        0        0      451 2023-07-24 02:24:56.000000 bcmd-0.0.8/bcmd/tasks/json.py
+-rw-rw-rw-   0        0        0     1328 2023-07-24 01:44:47.000000 bcmd-0.0.8/bcmd/tasks/mirrors.py
+-rw-rw-rw-   0        0        0      598 2023-07-24 01:55:47.000000 bcmd-0.0.8/bcmd/tasks/proxy.py
+-rw-rw-rw-   0        0        0     2368 2023-07-22 09:34:39.000000 bcmd-0.0.8/bcmd/tasks/time.py
+-rw-rw-rw-   0        0        0     2292 2023-07-22 10:03:50.000000 bcmd-0.0.8/bcmd/tasks/venv.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.791606 bcmd-0.0.8/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      149 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      617 2023-07-24 06:39:06.000000 bcmd-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:41:18.799608 bcmd-0.0.8/setup.cfg
```

### Comparing `bcmd-0.0.7/bcmd/tasks/mirrors.py` & `bcmd-0.0.8/bcmd/tasks/mirrors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,13 @@
+from __future__ import annotations
+
 from enum import StrEnum
-from beni import bpath, bfile
 
 import typer
-from beni import bcolor, bfunc, btask
-
-
-class _MirrorsType(StrEnum):
-    pip = 'pip'
-    npm = 'npm'
-
-
-_mirrorsFiles = {
-    _MirrorsType.pip: {
-        bpath.getUser('pip/pip.ini'): [
-            '[global]',
-            'index-url = https://mirrors.aliyun.com/pypi/simple',
-        ],
-    },
-    _MirrorsType.npm: {
-        bpath.getUser('.bashrc'): [
-            'registry=https://registry.npm.taobao.org/',
-            'electron_mirror=https://npm.taobao.org/mirrors/electron/',
-        ],
-    },
-}
+from beni import bcolor, bfile, bfunc, bpath, btask
 
 
 @btask.app.command()
 @bfunc.syncCall
 async def mirrors(
     types: list[_MirrorsType] = typer.Argument(None, help="镜像的类型"),
     disabled: bool = typer.Option(False, help="是否禁用"),
@@ -43,8 +23,28 @@
                 bcolor.printRed('删除文件', file)
             else:
                 print()
                 bcolor.printYellow(file)
                 msg = '\n'.join(msgAry)
                 await bfile.writeText(file, msg)
                 bcolor.printMagenta(msg)
-    print()
+
+
+class _MirrorsType(StrEnum):
+    pip = 'pip'
+    npm = 'npm'
+
+
+_mirrorsFiles = {
+    _MirrorsType.pip: {
+        bpath.getUser('pip/pip.ini'): [
+            '[global]',
+            'index-url = https://mirrors.aliyun.com/pypi/simple',
+        ],
+    },
+    _MirrorsType.npm: {
+        bpath.getUser('.bashrc'): [
+            'registry=https://registry.npm.taobao.org/',
+            'electron_mirror=https://npm.taobao.org/mirrors/electron/',
+        ],
+    },
+}
```

### Comparing `bcmd-0.0.7/bcmd/tasks/time.py` & `bcmd-0.0.8/bcmd/tasks/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,8 +67,7 @@
     for tzname in tzname_list:
         datetime_tz = datetime_utc.astimezone(ZoneInfo(tzname))
         dstStr = ''
         dst = datetime_tz.dst()
         if dst:
             dstStr = f'(DST+{dst})'
         print(f'{datetime_tz} {tzname} {dstStr}')
-    print()
```

### Comparing `bcmd-0.0.7/pyproject.toml` & `bcmd-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "bcmd"
-version = "0.0.7"
+version = "0.0.8"
 description = "Commands for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni", "bcmd"]
 authors = [
   {email = "benimang@126.com"},
-  {name = "Beni Mang"}
+  {name = "Beni Mang"},
 ]
 maintainers = [
   {name = "Beni Mang", email = "benimang@126.com"}
 ]
 
 dependencies = [
   'aioconsole',
   'aiofiles',
   'aiohttp',
   'autopep8',
-  'benimang==0.4.5',
+  'benimang>=0.4.7',
   'build',
   'colorama',
   'nest-asyncio',
   'orjson',
   'portalocker',
   'pretty_errors',
   'pyperclip',
```

