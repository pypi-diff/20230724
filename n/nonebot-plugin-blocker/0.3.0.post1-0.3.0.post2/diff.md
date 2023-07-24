# Comparing `tmp/nonebot_plugin_blocker-0.3.0.post1.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.0.post1.tar", last modified: Mon Jul 24 21:21:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.0.post2.tar", last modified: Mon Jul 24 21:25:19 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.0.post1.tar` & `nonebot_plugin_blocker-0.3.0.post2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-07-24 18:35:05.396383 nonebot_plugin_blocker-0.3.0.post1/LICENSE
--rw-r--r--   0        0        0     2447 2023-07-24 21:18:46.257130 nonebot_plugin_blocker-0.3.0.post1/README.md
--rw-r--r--   0        0        0     3062 2023-07-24 20:18:13.529731 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     5176 2023-07-24 20:17:03.641783 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2436 2023-07-24 19:49:40.333436 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      682 2023-07-24 21:21:43.655767 nonebot_plugin_blocker-0.3.0.post1/pyproject.toml
--rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-24 18:35:05.396383 nonebot_plugin_blocker-0.3.0.post2/LICENSE
+-rw-r--r--   0        0        0     2447 2023-07-24 21:18:46.257130 nonebot_plugin_blocker-0.3.0.post2/README.md
+-rw-r--r--   0        0        0     3062 2023-07-24 20:18:13.529731 nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     5176 2023-07-24 20:17:03.641783 nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2436 2023-07-24 19:49:40.333436 nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      721 2023-07-24 21:25:19.638877 nonebot_plugin_blocker-0.3.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.0.post2/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.0.post1/LICENSE` & `nonebot_plugin_blocker-0.3.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.0.post1/README.md` & `nonebot_plugin_blocker-0.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.0.post2/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.0.post1/pyproject.toml` & `nonebot_plugin_blocker-0.3.0.post2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.0.post1"
+version = "0.3.0.post2"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
@@ -22,14 +22,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 homepage = "https://github.com/MerCuJerry/nonebot-plugin-blocker"
 
 [tool.pdm.build]
+package-dir = "nonebot_plugin_blocker"
 includes = [
     "nonebot_plugin_blocker/web/webpage",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `nonebot_plugin_blocker-0.3.0.post1/PKG-INFO` & `nonebot_plugin_blocker-0.3.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.0.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.0.post2
 Summary: Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https:
 //github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

