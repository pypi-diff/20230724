# Comparing `tmp/nasops-0.0.1.tar.gz` & `tmp/nasops-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasops-0.0.1.tar", last modified: Thu Sep 29 09:44:31 2022, max compression
+gzip compressed data, was "nasops-0.0.2.tar", last modified: Wed Dec 14 03:37:00 2022, max compression
```

## Comparing `nasops-0.0.1.tar` & `nasops-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-29 09:44:31.583545 nasops-0.0.1/
--rw-rw-rw-   0        0        0      175 2022-09-29 09:44:31.582546 nasops-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      344 2022-09-29 09:30:19.000000 nasops-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-29 09:44:31.557550 nasops-0.0.1/dtools/
--rw-rw-rw-   0        0        0        0 2022-05-18 10:40:46.000000 nasops-0.0.1/dtools/__init__.py
--rw-rw-rw-   0        0        0     1447 2022-09-29 09:08:26.000000 nasops-0.0.1/dtools/__main__.py
--rw-rw-rw-   0        0        0     1770 2022-09-29 09:28:10.000000 nasops-0.0.1/dtools/main.py
--rw-rw-rw-   0        0        0     7245 2022-09-29 09:32:38.000000 nasops-0.0.1/dtools/util.py
-drwxrwxrwx   0        0        0        0 2022-09-29 09:44:31.579548 nasops-0.0.1/nasops.egg-info/
--rw-rw-rw-   0        0        0      175 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-29 09:44:31.000000 nasops-0.0.1/nasops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-29 09:44:31.584545 nasops-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      490 2022-09-29 09:44:18.000000 nasops-0.0.1/setup.py
+drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      214 2022-12-14 03:37:00.646726 nasops-0.0.2/PKG-INFO
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      344 2022-09-29 09:30:19.000000 nasops-0.0.2/README.md
+drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/dtools/
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        0 2022-05-18 10:40:46.000000 nasops-0.0.2/dtools/__init__.py
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     1447 2022-12-14 02:46:13.000000 nasops-0.0.2/dtools/__main__.py
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     2413 2022-12-14 03:32:08.000000 nasops-0.0.2/dtools/main.py
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)     7560 2022-12-14 03:29:37.000000 nasops-0.0.2/dtools/util.py
+drwxrwxr-x   0 yifeigao  (1000) yifeigao  (1000)        0 2022-12-14 03:37:00.646726 nasops-0.0.2/nasops.egg-info/
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      214 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/PKG-INFO
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      278 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/SOURCES.txt
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        1 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/dependency_links.txt
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       44 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/entry_points.txt
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       27 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/requires.txt
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)        7 2022-12-14 03:37:00.000000 nasops-0.0.2/nasops.egg-info/top_level.txt
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)       38 2022-12-14 03:37:00.646726 nasops-0.0.2/setup.cfg
+-rw-rw-r--   0 yifeigao  (1000) yifeigao  (1000)      506 2022-12-14 03:16:00.000000 nasops-0.0.2/setup.py
```

### Comparing `nasops-0.0.1/dtools/__main__.py` & `nasops-0.0.2/dtools/__main__.py`

 * *Files identical despite different names*

### Comparing `nasops-0.0.1/dtools/util.py` & `nasops-0.0.2/dtools/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import requests
-from tqdm import tqdm
 import json 
 import os
+
+import requests
+from tqdm import tqdm
+import configparser
 PUBLIC_PREFIX = "http://219.142.246.77:65000"
 def fix_url(url):
     return url.replace("https://disk.sophgo.vip", PUBLIC_PREFIX)
 
 def judge(url):
     return url.split("/")[3] == "sharing"
 
@@ -100,17 +102,14 @@
     else:
         url = PUBLIC_PREFIX + '/fsdownload/webapi/file_download.cgi/' + file_name
         post_data = "api=SYNO.FolderSharing.Download&method=download&version=2&mode=download&stdhtml=false&dlname=%22" \
                 + file_name + "%22&path=%5B%22%2F" + file_name.split(".")[0] + "%22%5D&_sharing_id=%22" + id + "%22&codepage=chs"
         resp = requests.post( url = url,cookies = cookie, data = post_data, stream=True)
         download(resp, fixed_url)
 
-# 上传功能的编写 
-
-
 def get_sid(username, password):
     ret = requests.get(f'{PUBLIC_PREFIX}/webapi/auth.cgi?api=SYNO.API.Auth&version=3&method=login&account={username}&passwd={password}&session=FileStation&format=sid')
     ret = json.loads(ret.content)
     if not ret['success']:
         ValueError("Login Failed! Please check your username and password!")
     _sid =ret['data']['sid']
     return _sid
@@ -148,15 +147,15 @@
     else:
         for each_file in tqdm(os.listdir(local_dir), leave=False):
             if os.path.isdir(os.path.join(local_dir,each_file)):
                 upload_dir(sid, os.path.join(local_dir,each_file), nas_dir+"/"+each_file)
             else:
                 upload_file(sid, os.path.join(local_dir,each_file), nas_dir)
     
-def list_nas_files(sid, nas_dir="home/Drive"):
+def list_nas_files(sid, nas_dir="home"):
     # list all files in nas_dir
     uri=PUBLIC_PREFIX + r'/webapi/entry.cgi?api=SYNO.FileStation.List&version=2&method=list&_sid=' + sid
     args = {
         'folder_path': nas_dir,
         'additional': 'real_path,owner,time,perm,real_path',
         'limit': 1000,
         'offset': 0
@@ -173,18 +172,29 @@
 
 def upload(username, password, local_dir, nas_dir):
     # upload local_dir to nas_dir
     sid = get_sid(username, password)
     upload_dir(sid, local_dir, nas_dir)
     print("upload success")
 
-def list_file(username, password, nas_dir="home/Drive"):
+def list_file(username, password, nas_dir="/home"):
     # list all files in nas_dir
     sid = get_sid(username, password)
     list_nas_files(sid, nas_dir)
 
+def init(un, pw):
+    config = configparser.ConfigParser()
+    config["SophonNas"] = {
+        "username" : un,
+        "password" : pw
+    }
+    # with open(os.path.expanduser("~/.nasops.ini"), 'wb+') as cfg:
+    with open(os.path.expanduser("~/.nasops.ini"), 'w') as cfg:
+        config.write(cfg)
+    print("init successfully")
+
 if __name__ == "__main__":
     single = "http://219.142.246.77:65000/sharing/lLojTQ9xW"
     multi = "https://disk.sophgo.vip/fsdownload/eqwC92lRU/vit"
     multi_o = "https://disk.sophgo.vip/sharing/qHL626Irz"
     # print(get_sid("wangyang.zuo","ZWYdomain0905"))
     # print(fix_url(single))
```

