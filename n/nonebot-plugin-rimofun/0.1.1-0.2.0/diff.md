# Comparing `tmp/nonebot_plugin_rimofun-0.1.1.tar.gz` & `tmp/nonebot_plugin_rimofun-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rimofun-0.1.1.tar", last modified: Sun Jun  4 17:17:47 2023, max compression
+gzip compressed data, was "nonebot_plugin_rimofun-0.2.0.tar", last modified: Mon Jul 24 03:24:15 2023, max compression
```

## Comparing `nonebot_plugin_rimofun-0.1.1.tar` & `nonebot_plugin_rimofun-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      575 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/LICENSE
--rw-r--r--   0        0        0     3619 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/README.md
--rw-r--r--   0        0        0     1326 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__init__.py
--rw-r--r--   0        0        0     5444 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__main__.py
--rw-r--r--   0        0        0       57 2023-06-04 17:17:25.575806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/.git
--rw-r--r--   0        0        0      147 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/LICENSE
--rw-r--r--   0        0        0     2590 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py
--rw-r--r--   0        0        0     6002 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json
--rw-r--r--   0        0        0   608988 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json
--rw-r--r--   0        0        0     4455 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json
--rw-r--r--   0        0        0     7480 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json
--rw-r--r--   0        0        0       69 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/莉沫词库.json
--rw-r--r--   0        0        0     5934 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/img/s.jpg
--rw-r--r--   0        0        0     1233 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/readme.md
--rw-r--r--   0        0        0      642 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/setup.py
--rw-r--r--   0        0        0     1635 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/config.py
--rw-r--r--   0        0        0     1997 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/data_source.py
--rw-r--r--   0        0        0       65 2023-06-04 17:17:26.239807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/.git
--rw-r--r--   0        0        0     2332 2023-06-04 17:17:26.259807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py
--rw-r--r--   0        0        0  3180205 2023-06-04 17:17:26.279807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt
--rw-r--r--   0        0        0  1369263 2023-06-04 17:17:26.287807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt
--rw-r--r--   0        0        0     6002 2023-06-04 17:17:26.287807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json
--rw-r--r--   0        0        0    31239 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json
--rw-r--r--   0        0        0     4498 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/readme.md
--rw-r--r--   0        0        0    29473 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json
--rw-r--r--   0        0        0     1191 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/数据.py
--rw-r--r--   0        0        0     1740 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/超.py
--rw-r--r--   0        0        0      660 2023-06-04 17:17:47.614089 nonebot_plugin_rimofun-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 nonebot_plugin_rimofun-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4181 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/README.md
+-rw-r--r--   0        0        0     1513 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/__init__.py
+-rw-r--r--   0        0        0     5380 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/__main__.py
+-rw-r--r--   0        0        0       57 2023-07-24 03:23:55.166107 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/.git
+-rw-r--r--   0        0        0      147 2023-07-24 03:23:55.834109 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/LICENSE
+-rw-r--r--   0        0        0     2590 2023-07-24 03:23:55.834109 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py
+-rw-r--r--   0        0        0     6002 2023-07-24 03:23:55.834109 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json
+-rw-r--r--   0        0        0   608988 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json
+-rw-r--r--   0        0        0     4455 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json
+-rw-r--r--   0        0        0     7480 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json
+-rw-r--r--   0        0        0       69 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/莉沫词库.json
+-rw-r--r--   0        0        0     5934 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/img/s.jpg
+-rw-r--r--   0        0        0     1233 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/readme.md
+-rw-r--r--   0        0        0      642 2023-07-24 03:23:55.842110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/setup.py
+-rw-r--r--   0        0        0     1664 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/config.py
+-rw-r--r--   0        0        0     1997 2023-07-24 03:23:54.494105 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/data_source.py
+-rw-r--r--   0        0        0       65 2023-07-24 03:23:55.826110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/.git
+-rw-r--r--   0        0        0     2332 2023-07-24 03:23:55.850109 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py
+-rw-r--r--   0        0        0  3180205 2023-07-24 03:23:55.870110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt
+-rw-r--r--   0        0        0  1369263 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt
+-rw-r--r--   0        0        0     6002 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json
+-rw-r--r--   0        0        0    31239 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json
+-rw-r--r--   0        0        0     4498 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/readme.md
+-rw-r--r--   0        0        0    29473 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json
+-rw-r--r--   0        0        0     1191 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/数据.py
+-rw-r--r--   0        0        0     1740 2023-07-24 03:23:55.878110 nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/超.py
+-rw-r--r--   0        0        0      647 2023-07-24 03:24:15.774373 nonebot_plugin_rimofun-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 nonebot_plugin_rimofun-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_rimofun-0.1.1/LICENSE` & `nonebot_plugin_rimofun-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/README.md` & `nonebot_plugin_rimofun-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 
 <div align="center">
 
 # NoneBot-Plugin-RimoFun
 
 _✨ 基于 [RimoChan](https://github.com/RimoChan) 开发的工具的有趣插件~ ✨_
 
+[幼女 Code](https://github.com/RimoChan/unvcode) | [不能好好说话](https://github.com/RimoChan/bnhhsh) | [淫语翻译机](https://github.com/RimoChan/yinglish) | [不会翻译机](https://github.com/RimoChan/not_translator)
+
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<a href="https://pdm.fming.dev">
+  <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
+</a>
+<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157">
+  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157.svg" alt="wakatime">
+</a>
+
+<br />
+
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-rimofun.svg" alt="license">
+  <img src="https://img.shields.io/github/license/lgc-NB2Dev/nonebot-plugin-rimofun.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
+  <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-rimofun" alt="pypi download">
 </a>
-<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157">
-  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157.svg" alt="wakatime">
-</a>
 
 </div>
 
 ## 📖 介绍
 
 把一些 [RimoChan](https://github.com/RimoChan) 的有趣的项目揉在了一起，做出了这个插件！
 
@@ -97,18 +105,22 @@
 
 ## ⚙️ 配置
 
 我真的懒得写文档了，请自行查看 [config.py](nonebot_plugin_rimofun/config.py)，感谢您的配合……
 
 ## 🎉 使用
 
+![help](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/-6cb8f68366e0b5f5.png)
+
+<!--
 ### 指令表
 
-不想写文档了……累了……  
+不想写文档了……累了……
 看看 [\_\_init\_\_.py](nonebot_plugin_rimofun/__init__.py) 吧，谢谢您了……
+-->
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -129,8 +141,14 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.0
+
+- 使用 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 兼容多平台消息发送
+
+### 0.1.1
+
+- 🎉 NoneBot 2.0 🚀
```

#### html2text {}

```diff
@@ -1,32 +1,36 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-RimoFun _â¨ åºäº [RimoChan](https://github.com/RimoChan)
-å¼åçå·¥å·çæè¶£æä»¶~ â¨_ [license] [pypi] [python] [pypi_download]
-                                  [wakatime]
+å¼åçå·¥å·çæè¶£æä»¶~ â¨_ [å¹¼å¥³ Code](https://github.com/RimoChan/
+    unvcode) | [ä¸è½å¥½å¥½è¯´è¯](https://github.com/RimoChan/bnhhsh) |
+  [æ·«è¯­ç¿»è¯æº](https://github.com/RimoChan/yinglish) | [ä¸ä¼ç¿»è¯æº]
+(https://github.com/RimoChan/not_translator) [python] [pdm-managed] [wakatime]
+                       [license] [pypi] [pypi_download]
 ## ð ä»ç» æä¸äº [RimoChan](https://github.com/RimoChan)
 çæè¶£çé¡¹ç®æå¨äºä¸èµ·ï¼ååºäºè¿ä¸ªæä»¶ï¼ ## ð¿ å®è£
 ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-rimofun
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-rimofun ```   pdm ```bash pdm add
 nonebot-plugin-rimofun ```   poetry ```bash poetry add nonebot-plugin-rimofun
 ```   conda ```bash conda install nonebot-plugin-rimofun ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_rimofun" ] ```  ## âï¸ éç½®
 æççæå¾åææ¡£äºï¼è¯·èªè¡æ¥ç [config.py]
-(nonebot_plugin_rimofun/config.py)ï¼æè°¢æ¨çéåâ¦â¦ ## ð ä½¿ç¨
-### æä»¤è¡¨ ä¸æ³åææ¡£äºâ¦â¦ç´¯äºâ¦â¦ çç [\_\_init\_\_.py]
-(nonebot_plugin_rimofun/__init__.py) å§ï¼è°¢è°¢æ¨äºâ¦â¦ ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+(nonebot_plugin_rimofun/config.py)ï¼æè°¢æ¨çéåâ¦â¦ ## ð ä½¿ç¨ !
+[help](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/-
+6cb8f68366e0b5f5.png)  ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
+(https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RimoChan](https://github.com/RimoChan) -
 æè°¢è¿ä½å¤§ä½¬ååºäºè¿äºæè¶£çé¡¹ç®ï¼ï¼ï¼æ²¡æè¿ä½å¤§ä½¬çè¿äºç²¾å½©ä½åå°±ä¸ä¼æè¿ä¸ªæä»¶ï¼æ¬
 fw å¨è¿éè¡·å¿æè°¢â¦â¦ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - ä½¿ç¨ [SAA](https://
+github.com/felinae98/nonebot-plugin-send-anything-anywhere)
+å¼å®¹å¤å¹³å°æ¶æ¯åé ### 0.1.1 - ð NoneBot 2.0 ð
```

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__main__.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import random
 import re
 from typing import List, Literal, Type
 
-from nonebot import get_driver, on_command, on_message
-from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment
+from nonebot import on_command, on_message
+from nonebot.internal.adapter import Event, Message
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg
 from nonebot.typing import T_State
+from nonebot_plugin_saa import MessageFactory
 
 from .config import config
 from .data_source import (
     bnhhsh_trans,
     not_translate,
     parse_yinglish_param,
     unvcode_convert,
     yinglish_trans,
 )
 
-nickname = n[0] if (n := list(get_driver().config.nickname)) else "我"
+nickname = list(config.nickname)[0] if config.nickname else "咱"
 
 
 def get_command_matcher(commands: List[str], *args, **kwargs) -> Type[Matcher]:
     return on_command(commands[0], *args, aliases=set(commands[1:]), **kwargs)
 
 
 matcher_unvcode = get_command_matcher(config.rimofun_unvcode_commands)
@@ -86,15 +87,15 @@
 
 @matcher_translate.handle()
 async def _(matcher: Matcher, arg: str = ArgPlainText("arg")):
     result = not_translate(arg)
     await matcher.finish(f"请您看看{nickname}的翻译厉不厉害！嘿嘿~\n{result}")
 
 
-async def trigger_rule(event: MessageEvent, state: T_State):
+async def trigger_rule(event: Event, state: T_State):
     msg_txt = event.get_plaintext().strip()
     if not msg_txt:
         return False
 
     is_english = re.fullmatch(r"^[a-zA-Z0-9@$!%*?&#^-_.+\s]+$", msg_txt)
     random_val = random.random()
 
@@ -131,24 +132,23 @@
     rule=trigger_rule,
     block=False,
     priority=config.rimofun_initiative_priority,
 )
 
 
 @matcher_initiative.handle()
-async def _(matcher: Matcher, event: MessageEvent, state: T_State):
+async def _(event: Event, state: T_State):
     msg_txt = event.get_plaintext().strip()
     trigger_type: Literal["bnhhsh", "yinglish", "translator"] = state["type"]
-    reply_seg = MessageSegment.reply(event.message_id)
 
     if trigger_type == "bnhhsh":
         result = bnhhsh_trans(msg_txt)
         reply = "\n".join([f"{k}：{v}" for k, v in result.items()])
-        await matcher.finish(reply_seg + f"让{nickname}解释一下消息里出现的神秘字母吧~\n{reply}")
+        await MessageFactory(f"让{nickname}解释一下消息里出现的神秘字母吧~\n{reply}").finish(reply=True)
 
     if trigger_type == "yinglish":
         reply = yinglish_trans(msg_txt)
-        await matcher.finish(reply_seg + f"让{nickname}来把你说的话变得更涩一点~\n{reply}")
+        await MessageFactory(f"让{nickname}来把你说的话变得更涩一点~\n{reply}").finish(reply=True)
 
     if trigger_type == "translator":
         reply = not_translate(msg_txt)
-        await matcher.finish(reply_seg + f"让{nickname}把这条消息翻译一下吧！\n{reply}")
+        await MessageFactory(f"让{nickname}把这条消息翻译一下吧！\n{reply}").finish(reply=True)
```

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/img/s.jpg` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/img/s.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/readme.md` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/readme.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/setup.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/bnhhsh/setup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/config.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import List
+from typing import List, Set
 
 from nonebot import get_driver
 from pydantic import BaseModel
 
 
 class ConfigModel(BaseModel):
+    nickname: Set[str]
+
     # unvcode
     rimofun_unvcode_mse: float = 0.2
     """unvcode 的全局字符串不同阈值，比如 0.2 代表匹配 80% 相同的字符"""
 
     rimofun_unvcode_commands: List[str] = ["unvcode", "幼女码"]
     """手动触发 bnhhsh 的命令"""
```

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/data_source.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/readme.md` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/readme.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/数据.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/数据.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/超.py` & `nonebot_plugin_rimofun-0.2.0/nonebot_plugin_rimofun/not_translator/训练代码/超.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.1/pyproject.toml` & `nonebot_plugin_rimofun-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "nonebot-plugin-rimofun"
-version = "0.1.1"
+version = "0.2.0"
 description = "Use RimoChan's stuff to do some interesting things"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
-    "nonebot-adapter-onebot<3.0.0,>=2.2.1",
+    "nonebot-plugin-send-anything-anywhere>=0.2.7",
     "pydantic<2.0.0,>=1.10.6",
-    "pypinyin<1.0.0,>=0.48.0",
-    "yinglish<2.0.0,>=1.0.1",
-    "unvcode<2.0.0,>=1.0.0",
+    "pypinyin>=0.48.0",
+    "yinglish>=1.0.1",
+    "unvcode>=1.0.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_rimofun-0.1.1/PKG-INFO` & `nonebot_plugin_rimofun-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rimofun
-Version: 0.1.1
+Version: 0.2.0
 Summary: Use RimoChan's stuff to do some interesting things
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-rimofun
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-rimofun
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
 Requires-Dist: pydantic<2.0.0,>=1.10.6
-Requires-Dist: pypinyin<1.0.0,>=0.48.0
-Requires-Dist: yinglish<2.0.0,>=1.0.1
-Requires-Dist: unvcode<2.0.0,>=1.0.0
+Requires-Dist: pypinyin>=0.48.0
+Requires-Dist: yinglish>=1.0.1
+Requires-Dist: unvcode>=1.0.0
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/rimofun.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
@@ -25,27 +25,35 @@
 
 <div align="center">
 
 # NoneBot-Plugin-RimoFun
 
 _✨ 基于 [RimoChan](https://github.com/RimoChan) 开发的工具的有趣插件~ ✨_
 
+[幼女 Code](https://github.com/RimoChan/unvcode) | [不能好好说话](https://github.com/RimoChan/bnhhsh) | [淫语翻译机](https://github.com/RimoChan/yinglish) | [不会翻译机](https://github.com/RimoChan/not_translator)
+
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<a href="https://pdm.fming.dev">
+  <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
+</a>
+<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157">
+  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157.svg" alt="wakatime">
+</a>
+
+<br />
+
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-rimofun.svg" alt="license">
+  <img src="https://img.shields.io/github/license/lgc-NB2Dev/nonebot-plugin-rimofun.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
+  <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-rimofun" alt="pypi download">
 </a>
-<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157">
-  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/4a5fe67b-9572-412a-84b8-064ca20f9157.svg" alt="wakatime">
-</a>
 
 </div>
 
 ## 📖 介绍
 
 把一些 [RimoChan](https://github.com/RimoChan) 的有趣的项目揉在了一起，做出了这个插件！
 
@@ -114,18 +122,22 @@
 
 ## ⚙️ 配置
 
 我真的懒得写文档了，请自行查看 [config.py](nonebot_plugin_rimofun/config.py)，感谢您的配合……
 
 ## 🎉 使用
 
+![help](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/-6cb8f68366e0b5f5.png)
+
+<!--
 ### 指令表
 
-不想写文档了……累了……  
+不想写文档了……累了……
 看看 [\_\_init\_\_.py](nonebot_plugin_rimofun/__init__.py) 吧，谢谢您了……
+-->
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -146,8 +158,14 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.0
+
+- 使用 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 兼容多平台消息发送
+
+### 0.1.1
+
+- 🎉 NoneBot 2.0 🚀
```

#### html2text {}

```diff
@@ -1,41 +1,45 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rimofun Version: 0.1.1 Summary: Use
+Metadata-Version: 2.1 Name: nonebot-plugin-rimofun Version: 0.2.0 Summary: Use
 RimoChan's stuff to do some interesting things Home-page: https://github.com/
 lgc-NB2Dev/nonebot-plugin-rimofun Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-rimofun Requires-Python: <4.0,>=3.8 Requires-Dist:
-nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1 Requires-
-Dist: pydantic<2.0.0,>=1.10.6 Requires-Dist: pypinyin<1.0.0,>=0.48.0 Requires-
-Dist: yinglish<2.0.0,>=1.0.1 Requires-Dist: unvcode<2.0.0,>=1.0.0 Description-
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
+Requires-Dist: pydantic<2.0.0,>=1.10.6 Requires-Dist: pypinyin>=0.48.0
+Requires-Dist: yinglish>=1.0.1 Requires-Dist: unvcode>=1.0.0 Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-RimoFun _â¨ åºäº [RimoChan](https://github.com/RimoChan)
-å¼åçå·¥å·çæè¶£æä»¶~ â¨_ [license] [pypi] [python] [pypi_download]
-                                  [wakatime]
+å¼åçå·¥å·çæè¶£æä»¶~ â¨_ [å¹¼å¥³ Code](https://github.com/RimoChan/
+    unvcode) | [ä¸è½å¥½å¥½è¯´è¯](https://github.com/RimoChan/bnhhsh) |
+  [æ·«è¯­ç¿»è¯æº](https://github.com/RimoChan/yinglish) | [ä¸ä¼ç¿»è¯æº]
+(https://github.com/RimoChan/not_translator) [python] [pdm-managed] [wakatime]
+                       [license] [pypi] [pypi_download]
 ## ð ä»ç» æä¸äº [RimoChan](https://github.com/RimoChan)
 çæè¶£çé¡¹ç®æå¨äºä¸èµ·ï¼ååºäºè¿ä¸ªæä»¶ï¼ ## ð¿ å®è£
 ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-rimofun
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-rimofun ```   pdm ```bash pdm add
 nonebot-plugin-rimofun ```   poetry ```bash poetry add nonebot-plugin-rimofun
 ```   conda ```bash conda install nonebot-plugin-rimofun ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_rimofun" ] ```  ## âï¸ éç½®
 æççæå¾åææ¡£äºï¼è¯·èªè¡æ¥ç [config.py]
-(nonebot_plugin_rimofun/config.py)ï¼æè°¢æ¨çéåâ¦â¦ ## ð ä½¿ç¨
-### æä»¤è¡¨ ä¸æ³åææ¡£äºâ¦â¦ç´¯äºâ¦â¦ çç [\_\_init\_\_.py]
-(nonebot_plugin_rimofun/__init__.py) å§ï¼è°¢è°¢æ¨äºâ¦â¦ ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+(nonebot_plugin_rimofun/config.py)ï¼æè°¢æ¨çéåâ¦â¦ ## ð ä½¿ç¨ !
+[help](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/-
+6cb8f68366e0b5f5.png)  ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
+(https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RimoChan](https://github.com/RimoChan) -
 æè°¢è¿ä½å¤§ä½¬ååºäºè¿äºæè¶£çé¡¹ç®ï¼ï¼ï¼æ²¡æè¿ä½å¤§ä½¬çè¿äºç²¾å½©ä½åå°±ä¸ä¼æè¿ä¸ªæä»¶ï¼æ¬
 fw å¨è¿éè¡·å¿æè°¢â¦â¦ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - ä½¿ç¨ [SAA](https://
+github.com/felinae98/nonebot-plugin-send-anything-anywhere)
+å¼å®¹å¤å¹³å°æ¶æ¯åé ### 0.1.1 - ð NoneBot 2.0 ð
```

