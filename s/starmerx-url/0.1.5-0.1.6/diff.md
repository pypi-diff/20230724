# Comparing `tmp/starmerx_url-0.1.5.tar.gz` & `tmp/starmerx_url-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmerx_url-0.1.5.tar", last modified: Mon Jul 24 03:20:12 2023, max compression
+gzip compressed data, was "starmerx_url-0.1.6.tar", last modified: Mon Jul 24 03:25:29 2023, max compression
```

## Comparing `starmerx_url-0.1.5.tar` & `starmerx_url-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:20:12.231707 starmerx_url-0.1.5/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.5/LICENSE
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-07-24 03:20:12.231707 starmerx_url-0.1.5/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      570 2023-07-24 03:19:47.000000 starmerx_url-0.1.5/README.md
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-07-24 03:20:12.231707 starmerx_url-0.1.5/setup.cfg
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-07-24 03:19:04.000000 starmerx_url-0.1.5/setup.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:20:12.231707 starmerx_url-0.1.5/starmerx_url/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.5/starmerx_url/__init__.py
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     2461 2023-07-24 03:16:44.000000 starmerx_url-0.1.5/starmerx_url/verify_url.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:20:12.231707 starmerx_url-0.1.5/starmerx_url.egg-info/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-07-24 03:20:12.000000 starmerx_url-0.1.5/starmerx_url.egg-info/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-07-24 03:20:12.000000 starmerx_url-0.1.5/starmerx_url.egg-info/SOURCES.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-07-24 03:20:12.000000 starmerx_url-0.1.5/starmerx_url.egg-info/dependency_links.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-07-24 03:20:12.000000 starmerx_url-0.1.5/starmerx_url.egg-info/top_level.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.5/starmerx_url.egg-info/zip-safe
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:25:29.766940 starmerx_url-0.1.6/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.6/LICENSE
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-07-24 03:25:29.766940 starmerx_url-0.1.6/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      570 2023-07-24 03:19:47.000000 starmerx_url-0.1.6/README.md
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-07-24 03:25:29.766940 starmerx_url-0.1.6/setup.cfg
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-07-24 03:25:07.000000 starmerx_url-0.1.6/setup.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:25:29.766940 starmerx_url-0.1.6/starmerx_url/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.6/starmerx_url/__init__.py
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     2528 2023-07-24 03:24:58.000000 starmerx_url-0.1.6/starmerx_url/verify_url.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-07-24 03:25:29.766940 starmerx_url-0.1.6/starmerx_url.egg-info/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-07-24 03:25:29.000000 starmerx_url-0.1.6/starmerx_url.egg-info/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-07-24 03:25:29.000000 starmerx_url-0.1.6/starmerx_url.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-07-24 03:25:29.000000 starmerx_url-0.1.6/starmerx_url.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-07-24 03:25:29.000000 starmerx_url-0.1.6/starmerx_url.egg-info/top_level.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.6/starmerx_url.egg-info/zip-safe
```

### Comparing `starmerx_url-0.1.5/LICENSE` & `starmerx_url-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerx_url-0.1.5/README.md` & `starmerx_url-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `starmerx_url-0.1.5/setup.py` & `starmerx_url-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="starmerx_url",
-    version="0.1.5",
+    version="0.1.6",
     author="yang",
     author_email="yangjuan@starmerx.com",
     description="starmerx verify url",
     license="MIT",
     url="",  # github
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `starmerx_url-0.1.5/starmerx_url/verify_url.py` & `starmerx_url-0.1.6/starmerx_url/verify_url.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         referer = request.META.get("HTTP_REFERER", "")
         reg2 = re.compile(reg2_compile)
         reg1 = re.compile(reg1_compile)
         print(f"remote_addr--{remote_addr}")
         print(f"remote_addr_real--{remote_addr_real}")
         print(f"referer--{referer}")
         if remote_addr_real_host_skip:
-            return False
+            if remote_addr_real in remote_addr_real_host_skip:
+                return False
 
         if referer_host:
             return re.match(reg2, remote_addr) or \
                    re.match(reg1, remote_addr_real) or \
                    remote_addr_real == remote_addr_real_host or \
                    referer_host in referer
```

