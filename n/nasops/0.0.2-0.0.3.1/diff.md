# Comparing `tmp/nasops-0.0.2.tar.gz` & `tmp/nasops-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasops-0.0.2.tar", last modified: Wed Dec 14 03:37:00 2022, max compression
+gzip compressed data, was "nasops-0.0.3.1.tar", last modified: Mon Jul 24 11:16:39 2023, max compression
```

## Comparing `nasops-0.0.2.tar` & `nasops-0.0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      214 2022-12-14 03:37:00.646726 nasops-0.0.2/PKG-INFO
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      344 2022-09-29 09:30:19.000000 nasops-0.0.2/README.md
-drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/dtools/
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        0 2022-05-18 10:40:46.000000 nasops-0.0.2/dtools/__init__.py
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     1447 2022-12-14 02:46:13.000000 nasops-0.0.2/dtools/__main__.py
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     2413 2022-12-14 03:32:08.000000 nasops-0.0.2/dtools/main.py
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     7560 2022-12-14 03:29:37.000000 nasops-0.0.2/dtools/util.py
-drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/nasops.egg-info/
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      214 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/PKG-INFO
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      278 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/SOURCES.txt
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        1 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/dependency_links.txt
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       44 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/entry_points.txt
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       27 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/requires.txt
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        7 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/top_level.txt
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       38 2022-12-14 03:37:00.646726 nasops-0.0.2/setup.cfg
--rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      506 2022-12-14 03:16:00.000000 nasops-0.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:16:39.717678 nasops-0.0.3.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:16:39.717678 nasops-0.0.3.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      434 2023-07-20 07:48:38.000000 nasops-0.0.3.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:16:39.713678 nasops-0.0.3.1/dtools/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-18 10:40:46.000000 nasops-0.0.3.1/dtools/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2957 2023-07-24 11:09:42.000000 nasops-0.0.3.1/dtools/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2957 2023-07-24 11:09:23.000000 nasops-0.0.3.1/dtools/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9013 2023-07-20 07:51:24.000000 nasops-0.0.3.1/dtools/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:16:39.713678 nasops-0.0.3.1/nasops.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      268 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       44 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       27 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-07-24 11:16:39.000000 nasops-0.0.3.1/nasops.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 11:16:39.717678 nasops-0.0.3.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      508 2023-07-24 11:15:45.000000 nasops-0.0.3.1/setup.py
```

### Comparing `nasops-0.0.2/dtools/main.py` & `nasops-0.0.3.1/dtools/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import argparse as arg
 import os
 import configparser
-from .util import download_from_nas, list_file, upload, init
+from util import download_from_nas, list_file, upload, init, uploadshare, share
 
 def bmcompiler_parser():
     parser = arg.ArgumentParser(description     = "handle nas with command line",
                                 formatter_class = arg.ArgumentDefaultsHelpFormatter,
                                 prog            = "python -m dtools")
     
-    parser.add_argument("method", choices=["download", "upload", "list", "init"], help="download or upload, you can do init first to avoid enter username and passwd  everytime")
+    parser.add_argument("method", choices=["download", "upload", "list", "init", "share", "upshare"], help="download or upload, you can do init first to avoid enter username and passwd  everytime")
     
     # upload file argments : name, password, local_dir, nas_dir
     parser.add_argument("--name", type=str,help="username")
     parser.add_argument("--password", type=str,help="password")
     parser.add_argument("--local_dir", type=str,help="local dir")
     parser.add_argument("--nas_dir", type=str,help="nas dir. Attention : \n \
         1. if the nas_dir is not exist, it will be created automatically. \n \
         2. And usually you should set nas_dir as /home/xxxx. \n \
         3. upload mode and target name is not support now. ")
     parser.add_argument('--verbose', type=bool, default=False, help='verbose')
+    parser.add_argument("--sharetime", type=int, default=30, help="the share link available time : \n \
+                        1. if the sharetime is not set, the default time is 30 days. \n \
+                        2. the sharetime will be 1000 days if you set -1.")
     return parser
 
 def check_user_info(parser):
     if parser.password and parser.name:
         pw = parser.password
         un = parser.name
     elif os.path.exists(os.path.expanduser("~/.nasops.ini")):
@@ -40,15 +43,23 @@
 
     if a.method == 'download':
         download_from_nas(a.url)
     
     if a.method == 'upload':
         un, pw = check_user_info(a)
         upload(un, pw, a.local_dir, a.nas_dir)
-        
+
+    if a.method == 'upshare':
+        un, pw = check_user_info(a)
+        uploadshare(un, pw, a.local_dir, a.nas_dir, a.sharetime)
+
+    if a.method == 'share':
+        un, pw = check_user_info(a)
+        share(un, pw, a.nas_dir, a.sharetime)
+
     if a.method == 'list':
         un, pw = check_user_info(a)
         list_file(un, pw, a.nas_dir)
     
     if a.method == 'init': 
         if os.name == "posix":
             if a.name and a.password:
```

### Comparing `nasops-0.0.2/dtools/util.py` & `nasops-0.0.3.1/dtools/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json 
 import os
-
+import time
 import requests
 from tqdm import tqdm
 import configparser
 PUBLIC_PREFIX = "http://219.142.246.77:65000"
 def fix_url(url):
     return url.replace("https://disk.sophgo.vip", PUBLIC_PREFIX)
 
@@ -133,16 +133,53 @@
                 'overwrite': 'true'
             } 
             files = {'file': (local_file_name, payload, 'application/octet-stream')}      
             uri=PUBLIC_PREFIX + r'/webapi/entry.cgi?api=SYNO.FileStation.Upload&version=2&method=upload&_sid=' + sid
             req=requests.post(uri, data=args, files=files, verify=True)
             # print("Success: \t",req.json())
     except Exception as e:
-        print('upload %s error：%s' % (local_file_name,e))
-        
+        print('upload %s error:%s' % (local_file_name,e))
+
+def generate_data_expired(timelong=3600*24*30):
+    current_time = int(time.time())
+    end_time = current_time + timelong
+     # return "YYYY-MM-DD"
+    format_time = time.strftime("%Y-%m-%d", time.localtime(end_time))
+    return format_time
+
+def share(username, password, nas_dir, sharetime=30):
+    sid = get_sid(username, password)
+    sharetime = 1000 if sharetime == -1 else sharetime
+    timelong  = 3600*24*sharetime
+    try:
+        payload={
+            "api":"SYNO.FileStation.Sharing",
+            "version":3,
+            "method":"create",
+            "path": nas_dir,
+            "date_expired": generate_data_expired(timelong),
+        }
+        url=PUBLIC_PREFIX + r'/webapi/entry.cgi'
+        # 构造cookies
+        cookies = {
+            "id":sid
+        }
+        req=requests.get(url, params=payload, verify=True, cookies=cookies)
+        req = req.json()
+        print(req['data']['links'][0]['url'])
+    except Exception as e:
+        print(e)
+
+def uploadshare(username, password, local_dir, nas_dir):
+    # upload local_dir to nas_dir
+    sid = get_sid(username, password)
+    upload_dir(sid, local_dir, nas_dir)
+    share(sid, nas_dir)
+    print("upload success")
+
 def upload_dir(sid, local_dir, nas_dir):
     # local_dir is file path, use upload_file to upload it
     # local_dir is dir path, use upload_dir to upload it
     if os.path.isfile(local_dir):
         upload_file(sid, local_dir, nas_dir)
     else:
         for each_file in tqdm(os.listdir(local_dir), leave=False):
@@ -172,14 +209,21 @@
 
 def upload(username, password, local_dir, nas_dir):
     # upload local_dir to nas_dir
     sid = get_sid(username, password)
     upload_dir(sid, local_dir, nas_dir)
     print("upload success")
 
+def uploadshare(username, password, local_dir, nas_dir, sharetime):
+    # upload local_dir to nas_dir
+    sid = get_sid(username, password)
+    upload_dir(sid, local_dir, nas_dir)
+    print("upload success! start to share")
+    share(sid, nas_dir, sharetime)
+
 def list_file(username, password, nas_dir="/home"):
     # list all files in nas_dir
     sid = get_sid(username, password)
     list_nas_files(sid, nas_dir)
 
 def init(un, pw):
     config = configparser.ConfigParser()
```

