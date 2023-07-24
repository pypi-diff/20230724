# Comparing `tmp/nonebot-plugin-blocker-0.3.0.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.3.0.tar", last modified: Mon Jul 24 20:23:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.0.post1.tar", last modified: Mon Jul 24 21:21:43 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.3.0.tar` & `nonebot_plugin_blocker-0.3.0.post1.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.079993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/setup.cfg
+-rw-r--r--   0        0        0     1074 2023-07-24 18:35:05.396383 nonebot_plugin_blocker-0.3.0.post1/LICENSE
+-rw-r--r--   0        0        0     2447 2023-07-24 21:18:46.257130 nonebot_plugin_blocker-0.3.0.post1/README.md
+-rw-r--r--   0        0        0     3062 2023-07-24 20:18:13.529731 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     5176 2023-07-24 20:17:03.641783 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2436 2023-07-24 19:49:40.333436 nonebot_plugin_blocker-0.3.0.post1/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      682 2023-07-24 21:21:43.655767 nonebot_plugin_blocker-0.3.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.0.post1/PKG-INFO
```

### Comparing `nonebot-plugin-blocker-0.3.0/LICENSE` & `nonebot_plugin_blocker-0.3.0.post1/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2023 MerCuJerry
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+MIT License
+
+Copyright (c) 2023 MerCuJerry
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `nonebot-plugin-blocker-0.3.0/PKG-INFO` & `nonebot_plugin_blocker-0.3.0.post1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-blocker
-Version: 0.3.0
-Summary: Message Blocker
-Author-email: MerCuJerry <mercujerry@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
-Keywords: nonebot,nonebot2,qqbot,bot
-Requires-Python: <4.0,>=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-blocker
 
 _✨ NoneBot Plugin Blocker ✨_
 
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-blocker.svg" alt="license">
+    <img src="https://img.shields.io/github/license/MerCuJerry/nonebot-plugin-blocker.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
@@ -80,13 +68,13 @@
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
-### 如果你设置了blocker_trigger项那么指令将会是你设置文本，如果仍然只能使用.bot on|off说明配置写错了请检查
+### 如果你在WebUI设置了指令那么指令将会是你设置的文本
 
 ## TODO && 碎碎念
 
  * 准备接着改改配置项
  * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
```

#### html2text {}

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.0 Summary:
-Message Blocker Author-email: MerCuJerry
-gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
-nonebot-plugin-blocker Keywords: nonebot,nonebot2,qqbot,bot Requires-Python:
-<4.0,>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
@@ -21,12 +16,10 @@
 BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
 æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
-###
-å¦æä½ è®¾ç½®äºblocker_triggeré¡¹é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®ææ¬ï¼å¦æä»ç¶åªè½ä½¿ç¨.bot
-on|offè¯´æéç½®åéäºè¯·æ£æ¥ ## TODO && ç¢ç¢å¿µ *
-åå¤æ¥çæ¹æ¹éç½®é¡¹ *
+### å¦æä½ å¨WebUIè®¾ç½®äºæä»¤é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®çææ¬ ##
+TODO && ç¢ç¢å¿µ * åå¤æ¥çæ¹æ¹éç½®é¡¹ *
 ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
```

