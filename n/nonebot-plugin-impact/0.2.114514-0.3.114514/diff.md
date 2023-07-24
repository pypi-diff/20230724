# Comparing `tmp/nonebot_plugin_impact-0.2.114514.tar.gz` & `tmp/nonebot_plugin_impact-0.3.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.2.114514.tar", last modified: Mon Jul 24 16:07:12 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.3.114514.tar", last modified: Mon Jul 24 16:22:05 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.2.114514.tar` & `nonebot_plugin_impact-0.3.114514.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.186682 nonebot_plugin_impact-0.2.114514/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.2.114514/LICENSE
--rw-rw-rw-   0        0        0      306 2023-07-24 16:07:12.185680 nonebot_plugin_impact-0.2.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.137789 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     2047 2023-07-24 16:03:28.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0     9171 2023-07-24 16:00:38.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/draw_img.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.144760 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/fonts/
--rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
--rw-rw-rw-   0        0        0    20206 2023-07-24 15:51:35.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2205 2023-07-24 16:03:09.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8628 2023-07-24 15:22:41.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.143788 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      306 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-24 16:07:12.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 16:07:12.186682 nonebot_plugin_impact-0.2.114514/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-07-24 16:07:02.000000 nonebot_plugin_impact-0.2.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:22:05.378227 nonebot_plugin_impact-0.3.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.3.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-07-24 16:22:05.377227 nonebot_plugin_impact-0.3.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 16:22:05.361258 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2093 2023-07-24 16:19:40.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0     9171 2023-07-24 16:00:38.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/draw_img.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:22:05.369228 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/fonts/
+-rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
+-rw-rw-rw-   0        0        0    20206 2023-07-24 15:51:35.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2205 2023-07-24 16:03:09.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8628 2023-07-24 15:22:41.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:22:05.368228 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-07-24 16:22:05.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-24 16:22:05.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 16:22:05.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-24 16:22:05.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 16:22:05.000000 nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 16:22:05.378227 nonebot_plugin_impact-0.3.114514/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-07-24 16:21:57.000000 nonebot_plugin_impact-0.3.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.2.114514/LICENSE` & `nonebot_plugin_impact-0.3.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     priority=20,
     block=False,
     handlers=[impart.pk],
 )
 
 on_regex(
     "^(打胶|开导)$", 
-    priority=20, block=True, 
+    priority=20, 
+    block=True, 
     handlers=[impart.dajiao]
 )
 
 on_command(
     "嗦牛子", 
     priority=20, 
     block=True, 
@@ -68,26 +69,27 @@
     block=True,
     handlers=[impart.query_injection],
 )
 
 on_command(
     "淫趴介绍", 
     priority=20, 
-    block=True
+    block=True,
+    handlers=[impart.yinpa_introduce]
 )
 
 with contextlib.suppress(Exception):
     from nonebot.plugin import PluginMetadata
 
     __plugin_meta__ = PluginMetadata(
         name="impact",
         description="让群友们眼前一黑的nonebot2淫趴插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_impact",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
-            "version": "0.02.114514",
+            "version": "0.03.114514",
             "priority": 20,
         },
     )
```

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/draw_img.py` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/draw_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.3.114514/nonebot_plugin_impact/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.2.114514/setup.py` & `nonebot_plugin_impact-0.3.114514/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_impact",
-    version="0.02.114514",
+    version="0.03.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="让群友们眼前一黑的nonebot2淫趴插件",
     python_requires=">=3.8.0",
     packages=find_packages(),
     url="https://github.com/Special-Week/nonebot_plugin_impact",
     package_data={"nonebot_plugin_impact": ["fonts/*"]},
```

