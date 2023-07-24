# Comparing `tmp/nonebot_plugin_arkgacha-0.3.0.tar.gz` & `tmp/nonebot_plugin_arkgacha-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arkgacha-0.3.0.tar", last modified: Thu Jun  1 09:28:49 2023, max compression
+gzip compressed data, was "nonebot_plugin_arkgacha-0.4.0.tar", last modified: Mon Jul 24 13:55:27 2023, max compression
```

## Comparing `nonebot_plugin_arkgacha-0.3.0.tar` & `nonebot_plugin_arkgacha-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    34522 2021-09-10 07:59:22.042000 nonebot_plugin_arkgacha-0.3.0/LICENSE
--rw-r--r--   0        0        0     2131 2023-05-13 08:16:56.047078 nonebot_plugin_arkgacha-0.3.0/README.md
--rw-r--r--   0        0        0     6180 2023-06-01 09:16:45.506306 nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/__init__.py
--rw-r--r--   0        0        0      250 2023-05-13 08:21:01.844002 nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/config.py
--rw-r--r--   0        0        0      679 2023-06-01 09:28:49.656286 nonebot_plugin_arkgacha-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2591 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2021-09-10 07:59:22.042000 nonebot_plugin_arkgacha-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2216 2023-07-24 13:55:11.128396 nonebot_plugin_arkgacha-0.4.0/README.md
+-rw-r--r--   0        0        0     6205 2023-07-24 12:53:25.968613 nonebot_plugin_arkgacha-0.4.0/nonebot_plugin_arkgacha/__init__.py
+-rw-r--r--   0        0        0     2771 2023-07-24 12:53:25.977252 nonebot_plugin_arkgacha-0.4.0/nonebot_plugin_arkgacha/__main__.py
+-rw-r--r--   0        0        0      250 2023-05-13 08:21:01.844002 nonebot_plugin_arkgacha-0.4.0/nonebot_plugin_arkgacha/config.py
+-rw-r--r--   0        0        0      765 2023-07-24 13:55:27.097333 nonebot_plugin_arkgacha-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_arkgacha-0.3.0/LICENSE` & `nonebot_plugin_arkgacha-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.3.0/README.md` & `nonebot_plugin_arkgacha-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,33 @@
 $ nb plugin install nonebot-plugin-arkgacha
 ```
 
 **在使用该插件之前，需要先初始化资源**
 
 命令行输入：
 ```bash
-$ arkkit init -SIMG
+nb arkgacha init
+```
+
+或
+
+```bash
+arkkit init -SIMG
 ```
 
 ## 配置
 
 - ARKGACHA_POOL_FILE: 抽卡池文件路径, 不填则使用 [`localstore`](https://github.com/nonebot/plugin-localstore) 保存抽卡池
 - ARKGACHA_MAX: 抽卡最大次数, 默认为 300
 - ARKGACHA_PURE_TEXT: 是否使用纯文本, 默认为 False (十连模拟必须使用图片)
 - ARKGACHA_AUTO_UPDATE: 是否自动更新，默认为 True
 
 ## 注意事项
-1. `方舟抽卡` 不需要图片资源, 可在不经过 `arkkit init` 的情况下使用
-2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `arkkit init -SIMG` 初始化资源，否则会出现错误
+1. `方舟抽卡` 不需要图片资源, 可在不经过 `nb arkgacha init` 或 `arkkit init` 的情况下使用
+2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `nb arkgacha init` 或 `arkkit init -SIMG` 初始化资源，否则会出现错误
 3. 若配置，每天 16 点将自动更新卡池资源
 4. 如果获取资源时出现网络错误，请检查代理设置，或尝试访问 PRTS
 
 ## 使用方法
 
 指令如下: 
 > 方舟抽卡
```

#### html2text {}

```diff
@@ -2,20 +2,21 @@
         # NoneBot Plugin Arkgacha _â¨ ææ¥æ¹èæ½å¡æ¨¡æå¨ â¨_
                            [license] [pypi] [python]
 è¯¥æä»¶æä¾äºæ¨¡æææ¥æ¹èæ½å¡çåè½ï¼åæ¬æ å¤´å½¢å¼çæ½å¡æ¨¡æä¸æ¨¡æåè¿
 éè¿ä½¿ç¨ [`saa`](https://github.com/felinae98/nonebot-plugin-send-anything-
 anywhere) æä»¶ééå¤å¹³å° ## å®è£ ```bash $ pip install nonebot-plugin-
 arkgacha ``` ```bash $ nb plugin install nonebot-plugin-arkgacha ```
 **å¨ä½¿ç¨è¯¥æä»¶ä¹åï¼éè¦ååå§åèµæº** å½ä»¤è¡è¾å¥ï¼
-```bash $ arkkit init -SIMG ``` ## éç½® - ARKGACHA_POOL_FILE:
-æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`](https://github.com/
-nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX: æ½å¡æå¤§æ¬¡æ°,
-é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬, é»è®¤ä¸º False
-(åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
+```bash nb arkgacha init ``` æ ```bash arkkit init -SIMG ``` ## éç½® -
+ARKGACHA_POOL_FILE: æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`]
+(https://github.com/nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX:
+æ½å¡æå¤§æ¬¡æ°, é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬,
+é»è®¤ä¸º False (åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
 æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
-ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `arkkit init` çæåµä¸ä½¿ç¨ 2.
-`æ¹èåè¿` éè¦å¾çèµæº, éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `arkkit init
--SIMG` åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
+ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `nb arkgacha init` æ `arkkit init`
+çæåµä¸ä½¿ç¨ 2. `æ¹èåè¿` éè¦å¾çèµæº,
+éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `nb arkgacha init` æ `arkkit init -SIMG`
+åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
 ç¹å°èªå¨æ´æ°å¡æ± èµæº 4.
 å¦æè·åèµæºæ¶åºç°ç½ç»éè¯¯ï¼è¯·æ£æ¥ä»£çè®¾ç½®ï¼æå°è¯è®¿é®
 PRTS ## ä½¿ç¨æ¹æ³ æä»¤å¦ä¸: > æ¹èæ½å¡ > > æ¹èæ½å¡ 200 > >
 æ¹èåè¿ > > æ¹èå¡æ± æ´æ° ## ææ > æ¹èåè¿ ![res](./test.png)
```

### Comparing `nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/__init__.py` & `nonebot_plugin_arkgacha-0.4.0/nonebot_plugin_arkgacha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from nonebot_plugin_apscheduler import scheduler
 
 from .config import Config
 
 driver = get_driver()
 global_config = driver.config
 config = Config.parse_obj(global_config)
-
+__version__ = "0.4.0"
 __plugin_meta__ = PluginMetadata(
     name="明日方舟抽卡模拟",
     description="明模拟日方舟抽卡功能，支持模拟十连",
     usage="""\
 方舟抽卡 [count = 10]
 方舟十连
 方舟抽卡帮助
@@ -39,15 +39,15 @@
 """,
     homepage="https://github.com/RF-Tar-Railt/nonebot-plugin-arkgacha",
     type="application",
     config=Config,
     extra={
         "author": "RF-Tar-Railt",
         'priority': 3,
-        "version": "0.3.0",
+        "version": __version__,
     }
 )
 
 
 gacha = ArknightsGacha(config.arkgacha_pool_file or get_data_file("arkgacha", "pool.json"))
 user_cache_file = get_cache_file("arkgacha", "user.json")
 if not user_cache_file.exists():
```

### Comparing `nonebot_plugin_arkgacha-0.3.0/pyproject.toml` & `nonebot_plugin_arkgacha-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-arkgacha"
-version = "0.3.0"
+version = "0.4.0"
 description = "Plugin for Arknights gacha, support multi platform"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-plugin-alconna>=0.7.0",
@@ -15,14 +15,17 @@
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
+[project.entry-points.nb_scripts]
+arkgacha = "nonebot_plugin_arkgacha.__main__:main"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
```

### Comparing `nonebot_plugin_arkgacha-0.3.0/PKG-INFO` & `nonebot_plugin_arkgacha-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-arkgacha
-Version: 0.3.0
+Version: 0.4.0
 Summary: Plugin for Arknights gacha, support multi platform
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-alconna>=0.7.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
@@ -49,27 +49,33 @@
 $ nb plugin install nonebot-plugin-arkgacha
 ```
 
 **在使用该插件之前，需要先初始化资源**
 
 命令行输入：
 ```bash
-$ arkkit init -SIMG
+nb arkgacha init
+```
+
+或
+
+```bash
+arkkit init -SIMG
 ```
 
 ## 配置
 
 - ARKGACHA_POOL_FILE: 抽卡池文件路径, 不填则使用 [`localstore`](https://github.com/nonebot/plugin-localstore) 保存抽卡池
 - ARKGACHA_MAX: 抽卡最大次数, 默认为 300
 - ARKGACHA_PURE_TEXT: 是否使用纯文本, 默认为 False (十连模拟必须使用图片)
 - ARKGACHA_AUTO_UPDATE: 是否自动更新，默认为 True
 
 ## 注意事项
-1. `方舟抽卡` 不需要图片资源, 可在不经过 `arkkit init` 的情况下使用
-2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `arkkit init -SIMG` 初始化资源，否则会出现错误
+1. `方舟抽卡` 不需要图片资源, 可在不经过 `nb arkgacha init` 或 `arkkit init` 的情况下使用
+2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `nb arkgacha init` 或 `arkkit init -SIMG` 初始化资源，否则会出现错误
 3. 若配置，每天 16 点将自动更新卡池资源
 4. 如果获取资源时出现网络错误，请检查代理设置，或尝试访问 PRTS
 
 ## 使用方法
 
 指令如下: 
 > 方舟抽卡
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.4.0 Summary:
 Plugin for Arknights gacha, support multi platform Author-Email: RF-Tar-Railt
 qq.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-alconna>=0.7.0 Requires-Dist: nonebot-plugin-
 send-anything-anywhere>=0.2.4 Requires-Dist: arknights-toolkit<0.6.0,>=0.5.8
 Requires-Dist: nonebot-plugin-localstore>=0.4.1 Requires-Dist: nonebot-plugin-
 apscheduler>=0.2.0 Description-Content-Type: text/markdown
                                    [nonebot]
         # NoneBot Plugin Arkgacha _â¨ ææ¥æ¹èæ½å¡æ¨¡æå¨ â¨_
                            [license] [pypi] [python]
 è¯¥æä»¶æä¾äºæ¨¡æææ¥æ¹èæ½å¡çåè½ï¼åæ¬æ å¤´å½¢å¼çæ½å¡æ¨¡æä¸æ¨¡æåè¿
 éè¿ä½¿ç¨ [`saa`](https://github.com/felinae98/nonebot-plugin-send-anything-
 anywhere) æä»¶ééå¤å¹³å° ## å®è£ ```bash $ pip install nonebot-plugin-
 arkgacha ``` ```bash $ nb plugin install nonebot-plugin-arkgacha ```
 **å¨ä½¿ç¨è¯¥æä»¶ä¹åï¼éè¦ååå§åèµæº** å½ä»¤è¡è¾å¥ï¼
-```bash $ arkkit init -SIMG ``` ## éç½® - ARKGACHA_POOL_FILE:
-æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`](https://github.com/
-nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX: æ½å¡æå¤§æ¬¡æ°,
-é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬, é»è®¤ä¸º False
-(åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
+```bash nb arkgacha init ``` æ ```bash arkkit init -SIMG ``` ## éç½® -
+ARKGACHA_POOL_FILE: æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`]
+(https://github.com/nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX:
+æ½å¡æå¤§æ¬¡æ°, é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬,
+é»è®¤ä¸º False (åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
 æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
-ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `arkkit init` çæåµä¸ä½¿ç¨ 2.
-`æ¹èåè¿` éè¦å¾çèµæº, éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `arkkit init
--SIMG` åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
+ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `nb arkgacha init` æ `arkkit init`
+çæåµä¸ä½¿ç¨ 2. `æ¹èåè¿` éè¦å¾çèµæº,
+éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `nb arkgacha init` æ `arkkit init -SIMG`
+åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
 ç¹å°èªå¨æ´æ°å¡æ± èµæº 4.
 å¦æè·åèµæºæ¶åºç°ç½ç»éè¯¯ï¼è¯·æ£æ¥ä»£çè®¾ç½®ï¼æå°è¯è®¿é®
 PRTS ## ä½¿ç¨æ¹æ³ æä»¤å¦ä¸: > æ¹èæ½å¡ > > æ¹èæ½å¡ 200 > >
 æ¹èåè¿ > > æ¹èå¡æ± æ´æ° ## ææ > æ¹èåè¿ ![res](./test.png)
```

