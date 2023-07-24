# Comparing `tmp/nonebot-plugin-blocker-0.2.1.tar.gz` & `tmp/nonebot-plugin-blocker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.2.1.tar", last modified: Sat Jul 15 18:18:57 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.3.0.tar", last modified: Mon Jul 24 20:23:13 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.2.1.tar` & `nonebot-plugin-blocker-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.079993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:23:13.000000 nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-24 20:22:50.000000 nonebot-plugin-blocker-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:23:13.083993 nonebot-plugin-blocker-0.3.0/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.2.1/PKG-INFO` & `nonebot-plugin-blocker-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-blocker
-Version: 0.2.1
-Summary: Message Blocker
-Author-email: MerCuJerry <mercujerry@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
-Requires-Python: <4.0,>=3.8
-Description-Content-Type: text/markdown
-
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -31,14 +21,16 @@
 
 </div>
 
 ## 📖 介绍
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
+插件提供了一个简单的WebUI来让你配置Bot的开关指令以及对指令做出的回复。
+
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
@@ -50,43 +42,39 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
+### 请注意，曾经使用过低版本本插件的请重新在WebUI里进行配置
+
 ### 常规配置项，位于.env文件里
 
 ```ini
-#本配置项不是必填配置项
-blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+#WebUI的登录凭证，不设置即不进行验证
+BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD=""
 ```
 
 ### 其他配置项
-插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
-```jsonc
-    {
-        "reply_on":{
-            "type":"text"
-            "data":{
-                "text":"在本群开启"
-            }
-        },
-        "reply_off":{
-            "type":"text"
-            "data":{
-                "text":"在本群关闭"
-            }
-        }
-    }
-```
+
+插件的回复配置文件位于 `data/blocker/reply_config.json` 里，不建议手动更改
+
 `data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+
+### 如果你设置了blocker_trigger项那么指令将会是你设置文本，如果仍然只能使用.bot on|off说明配置写错了请检查
+
+## TODO && 碎碎念
+
+ * 准备接着改改配置项
+ * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.1 Summary:
-Message Blocker Author-email: MerCuJerry
-gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
-nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
-text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
-æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
+æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
+## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
-å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
-blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
-``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
-blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+è¯·æ³¨æï¼æ¾ç»ä½¿ç¨è¿ä½çæ¬æ¬æä»¶çè¯·éæ°å¨WebUIéè¿è¡éç½®
+### å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini
+#WebUIçç»å½å­è¯ï¼ä¸è®¾ç½®å³ä¸è¿è¡éªè¯ BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
+æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
+éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
+###
+å¦æä½ è®¾ç½®äºblocker_triggeré¡¹é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®ææ¬ï¼å¦æä»ç¶åªè½ä½¿ç¨.bot
+on|offè¯´æéç½®åéäºè¯·æ£æ¥ ## TODO && ç¢ç¢å¿µ *
+åå¤æ¥çæ¹æ¹éç½®é¡¹ *
+ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
```

### Comparing `nonebot-plugin-blocker-0.2.1/README.md` & `nonebot-plugin-blocker-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-blocker
+Version: 0.3.0
+Summary: Message Blocker
+Author-email: MerCuJerry <mercujerry@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
+Keywords: nonebot,nonebot2,qqbot,bot
+Requires-Python: <4.0,>=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -21,14 +33,16 @@
 
 </div>
 
 ## 📖 介绍
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
+插件提供了一个简单的WebUI来让你配置Bot的开关指令以及对指令做出的回复。
+
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
@@ -40,43 +54,39 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
+### 请注意，曾经使用过低版本本插件的请重新在WebUI里进行配置
+
 ### 常规配置项，位于.env文件里
 
 ```ini
-#本配置项不是必填配置项
-blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+#WebUI的登录凭证，不设置即不进行验证
+BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD=""
 ```
 
 ### 其他配置项
-插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
-```jsonc
-    {
-        "reply_on":{
-            "type":"text"
-            "data":{
-                "text":"在本群开启"
-            }
-        },
-        "reply_off":{
-            "type":"text"
-            "data":{
-                "text":"在本群关闭"
-            }
-        }
-    }
-```
+
+插件的回复配置文件位于 `data/blocker/reply_config.json` 里，不建议手动更改
+
 `data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
-### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+
+### 如果你设置了blocker_trigger项那么指令将会是你设置文本，如果仍然只能使用.bot on|off说明配置写错了请检查
+
+## TODO && 碎碎念
+
+ * 准备接着改改配置项
+ * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
```

#### html2text {}

```diff
@@ -1,21 +1,32 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.0 Summary:
+Message Blocker Author-email: MerCuJerry
+gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
+nonebot-plugin-blocker Keywords: nonebot,nonebot2,qqbot,bot Requires-Python:
+<4.0,>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
-æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
+æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
+## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
-å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
-blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
-``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
-blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+è¯·æ³¨æï¼æ¾ç»ä½¿ç¨è¿ä½çæ¬æ¬æä»¶çè¯·éæ°å¨WebUIéè¿è¡éç½®
+### å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini
+#WebUIçç»å½å­è¯ï¼ä¸è®¾ç½®å³ä¸è¿è¡éªè¯ BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
+æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
+éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
+###
+å¦æä½ è®¾ç½®äºblocker_triggeré¡¹é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®ææ¬ï¼å¦æä»ç¶åªè½ä½¿ç¨.bot
+on|offè¯´æéç½®åéäºè¯·æ£æ¥ ## TODO && ç¢ç¢å¿µ *
+åå¤æ¥çæ¹æ¹éç½®é¡¹ *
+ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
```

### Comparing `nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.3.0/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.2.1
+Version: 0.3.0
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
+Keywords: nonebot,nonebot2,qqbot,bot
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
@@ -31,14 +33,16 @@
 
 </div>
 
 ## 📖 介绍
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
+插件提供了一个简单的WebUI来让你配置Bot的开关指令以及对指令做出的回复。
+
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
@@ -50,43 +54,39 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
+### 请注意，曾经使用过低版本本插件的请重新在WebUI里进行配置
+
 ### 常规配置项，位于.env文件里
 
 ```ini
-#本配置项不是必填配置项
-blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+#WebUI的登录凭证，不设置即不进行验证
+BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD=""
 ```
 
 ### 其他配置项
-插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
-```jsonc
-    {
-        "reply_on":{
-            "type":"text"
-            "data":{
-                "text":"在本群开启"
-            }
-        },
-        "reply_off":{
-            "type":"text"
-            "data":{
-                "text":"在本群关闭"
-            }
-        }
-    }
-```
+
+插件的回复配置文件位于 `data/blocker/reply_config.json` 里，不建议手动更改
+
 `data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+
+### 如果你设置了blocker_trigger项那么指令将会是你设置文本，如果仍然只能使用.bot on|off说明配置写错了请检查
+
+## TODO && 碎碎念
+
+ * 准备接着改改配置项
+ * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
```

#### html2text {}

```diff
@@ -1,26 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.0 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
-nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
-text/markdown
+nonebot-plugin-blocker Keywords: nonebot,nonebot2,qqbot,bot Requires-Python:
+<4.0,>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
-æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
+æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
+## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
-å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
-blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
-``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
-blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
-"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+è¯·æ³¨æï¼æ¾ç»ä½¿ç¨è¿ä½çæ¬æ¬æä»¶çè¯·éæ°å¨WebUIéè¿è¡éç½®
+### å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini
+#WebUIçç»å½å­è¯ï¼ä¸è®¾ç½®å³ä¸è¿è¡éªè¯ BLOCKER_WEBUI_USERNAME=""
+BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
+æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
+éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
+###
+å¦æä½ è®¾ç½®äºblocker_triggeré¡¹é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®ææ¬ï¼å¦æä»ç¶åªè½ä½¿ç¨.bot
+on|offè¯´æéç½®åéäºè¯·æ£æ¥ ## TODO && ç¢ç¢å¿µ *
+åå¤æ¥çæ¹æ¹éç½®é¡¹ *
+ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
```

