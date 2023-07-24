# Comparing `tmp/nasops-0.0.3.2.tar.gz` & `tmp/nasops-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasops-0.0.3.2.tar", last modified: Mon Jul 24 11:24:59 2023, max compression
+gzip compressed data, was "nasops-0.0.3.3.tar", last modified: Mon Jul 24 11:34:04 2023, max compression
```

## Comparing `nasops-0.0.3.2.tar` & `nasops-0.0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:24:59.677688 nasops-0.0.3.2/
--rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:24:59.677688 nasops-0.0.3.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      493 2023-07-24 11:24:24.000000 nasops-0.0.3.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:24:59.677688 nasops-0.0.3.2/dtools/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-18 10:40:46.000000 nasops-0.0.3.2/dtools/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2958 2023-07-24 11:23:37.000000 nasops-0.0.3.2/dtools/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2958 2023-07-24 11:23:33.000000 nasops-0.0.3.2/dtools/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     9013 2023-07-20 07:51:24.000000 nasops-0.0.3.2/dtools/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:24:59.677688 nasops-0.0.3.2/nasops.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      268 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       44 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       27 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-07-24 11:24:59.000000 nasops-0.0.3.2/nasops.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 11:24:59.677688 nasops-0.0.3.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      508 2023-07-24 11:24:47.000000 nasops-0.0.3.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:34:04.657699 nasops-0.0.3.3/
+-rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:34:04.657699 nasops-0.0.3.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      493 2023-07-24 11:24:24.000000 nasops-0.0.3.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:34:04.657699 nasops-0.0.3.3/dtools/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-18 10:40:46.000000 nasops-0.0.3.3/dtools/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2958 2023-07-24 11:23:37.000000 nasops-0.0.3.3/dtools/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2958 2023-07-24 11:23:33.000000 nasops-0.0.3.3/dtools/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9139 2023-07-24 11:33:03.000000 nasops-0.0.3.3/dtools/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 11:34:04.657699 nasops-0.0.3.3/nasops.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      171 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      268 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       44 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       27 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-07-24 11:34:04.000000 nasops-0.0.3.3/nasops.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 11:34:04.657699 nasops-0.0.3.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      508 2023-07-24 11:33:24.000000 nasops-0.0.3.3/setup.py
```

### Comparing `nasops-0.0.3.2/dtools/__main__.py` & `nasops-0.0.3.3/dtools/__main__.py`

 * *Files identical despite different names*

### Comparing `nasops-0.0.3.2/dtools/main.py` & `nasops-0.0.3.3/dtools/main.py`

 * *Files identical despite different names*

### Comparing `nasops-0.0.3.2/dtools/util.py` & `nasops-0.0.3.3/dtools/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,20 @@
 def generate_data_expired(timelong=3600*24*30):
     current_time = int(time.time())
     end_time = current_time + timelong
      # return "YYYY-MM-DD"
     format_time = time.strftime("%Y-%m-%d", time.localtime(end_time))
     return format_time
 
-def share(username, password, nas_dir, sharetime=30):
-    sid = get_sid(username, password)
+def share(username=None, password=None, nas_dir=None, sharetime=30,sid=None):
+    if not sid:
+        assert username and password
+        sid = get_sid(username, password)
+    else:
+        pass
     sharetime = 1000 if sharetime == -1 else sharetime
     timelong  = 3600*24*sharetime
     try:
         payload={
             "api":"SYNO.FileStation.Sharing",
             "version":3,
             "method":"create",
@@ -214,15 +218,15 @@
     print("upload success")
 
 def uploadshare(username, password, local_dir, nas_dir, sharetime):
     # upload local_dir to nas_dir
     sid = get_sid(username, password)
     upload_dir(sid, local_dir, nas_dir)
     print("upload success! start to share")
-    share(sid, nas_dir, sharetime)
+    share(sid=sid, nas_dir=nas_dir, sharetime=sharetime)
 
 def list_file(username, password, nas_dir="/home"):
     # list all files in nas_dir
     sid = get_sid(username, password)
     list_nas_files(sid, nas_dir)
 
 def init(un, pw):
```

