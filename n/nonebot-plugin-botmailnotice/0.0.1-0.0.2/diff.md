# Comparing `tmp/nonebot-plugin-BotMailNotice-0.0.1.tar.gz` & `tmp/nonebot-plugin-BotMailNotice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-BotMailNotice-0.0.1.tar", max compression
+gzip compressed data, was "nonebot-plugin-BotMailNotice-0.0.2.tar", max compression
```

## Comparing `nonebot-plugin-BotMailNotice-0.0.1.tar` & `nonebot-plugin-BotMailNotice-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2023-07-24 15:03:51.823628 nonebot-plugin-BotMailNotice-0.0.1/LICENSE
--rw-r--r--   0        0        0     2471 2023-07-24 15:04:07.847740 nonebot-plugin-BotMailNotice-0.0.1/nonebot_plugin_BotMailNotice/__init__.py
--rw-r--r--   0        0        0      476 2023-07-24 15:09:13.199030 nonebot-plugin-BotMailNotice-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2854 2023-07-24 14:56:54.031826 nonebot-plugin-BotMailNotice-0.0.1/README.md
--rw-r--r--   0        0        0     3587 1970-01-01 00:00:00.000000 nonebot-plugin-BotMailNotice-0.0.1/setup.py
--rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 nonebot-plugin-BotMailNotice-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-24 15:03:51.823628 nonebot-plugin-BotMailNotice-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2471 2023-07-24 15:04:07.847740 nonebot-plugin-BotMailNotice-0.0.2/nonebot_plugin_BotMailNotice/__init__.py
+-rw-r--r--   0        0        0      476 2023-07-24 15:16:59.586852 nonebot-plugin-BotMailNotice-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-07-24 15:16:15.103027 nonebot-plugin-BotMailNotice-0.0.2/README.md
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 nonebot-plugin-BotMailNotice-0.0.2/setup.py
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 nonebot-plugin-BotMailNotice-0.0.2/PKG-INFO
```

### Comparing `nonebot-plugin-BotMailNotice-0.0.1/LICENSE` & `nonebot-plugin-BotMailNotice-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-BotMailNotice-0.0.1/nonebot_plugin_BotMailNotice/__init__.py` & `nonebot-plugin-BotMailNotice-0.0.2/nonebot_plugin_BotMailNotice/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-BotMailNotice-0.0.1/README.md` & `nonebot-plugin-BotMailNotice-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -69,29 +69,29 @@
     
 
 </details>
 
 <details>
 <summary>使用第二种方式安装看此方法</summary>
 
-- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`
+- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["nonebot_plugin_BotMailNotice"]`
 
 </details>
 
 
 
 ##  配置
 运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中配置项
 
-| 配置项 | 必填 | 值类型 | 默认值 | 说明 |
-|:------:|:----:|:---:|:---:|:--:|
-| username | 是 | str | ""  | 邮箱账号 |
-| password | 是 | str | ""  | 邮箱密码或授权码 |
-| hostname | 是 | str | ""  | 邮箱服务器地址 |
-| port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
+|  配置项  | 必填  | 值类型 | 默认值 |            说明            |
+| :------: | :---: | :----: | :----: | :------------------------: |
+| username |  是   |  str   |   ""   |          邮箱账号          |
+| password |  是   |  str   |   ""   |      邮箱密码或授权码      |
+| hostname |  是   |  str   |   ""   |       邮箱服务器地址       |
+|   port   |  是   |  int   |  465   | 邮箱端口号，ssl模式时为465 |
 
 ## 示例配置
   
 ```env
 mail_notice='{
 "username":"xxx@qq.com",
 "password":"qflgxxxxxx",
```

#### html2text {}

```diff
@@ -15,16 +15,17 @@
 ä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³ -
 å°`nonebot_plugin_BotMailNotice`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯
 - æä»¶ç»æå¦ä¸ ```py ð¦ AweSome-Bot âââ ð awesome_bot â
 âââ ð plugins | âââ ð nonebot_plugin_BotMailNotice |
 âââ ð __init__.py âââ ð .env.prod âââ ð .gitignore
 âââ ð pyproject.toml âââ ð README.md ```
 ä½¿ç¨ç¬¬äºç§æ¹å¼å®è£çæ­¤æ¹æ³ - å¨`pyproject.toml`éç`
-[tool.nonebot]`ä¸­æ·»å `plugins = ["TeenStudy"]`  ## éç½®
+[tool.nonebot]`ä¸­æ·»å `plugins = ["nonebot_plugin_BotMailNotice"]`  ## éç½®
 è¿è¡æä»¶åï¼éè¦å¨ nonebot2
 é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­éç½®é¡¹ | éç½®é¡¹ | å¿å¡« |
-å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| | username
-| æ¯ | str | "" | é®ç®±è´¦å· | | password | æ¯ | str | "" |
-é®ç®±å¯ç æææç  | | hostname | æ¯ | str | "" | é®ç®±æå¡å¨å°å
-| | port | æ¯ | int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | ##
-ç¤ºä¾éç½® ```env mail_notice='{ "username":"xxx@qq.com", "password":
-"qflgxxxxxx", "hostname":"smtp.qq.com", "port":587 }' ```
+å¼ç±»å | é»è®¤å¼ | è¯´æ | | :------: | :---: | :----: | :----: | :------
+------------------: | | username | æ¯ | str | "" | é®ç®±è´¦å· | | password |
+æ¯ | str | "" | é®ç®±å¯ç æææç  | | hostname | æ¯ | str | "" |
+é®ç®±æå¡å¨å°å | | port | æ¯ | int | 465 |
+é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | ## ç¤ºä¾éç½® ```env mail_notice='
+{ "username":"xxx@qq.com", "password":"qflgxxxxxx", "hostname":"smtp.qq.com",
+"port":587 }' ```
```

### Comparing `nonebot-plugin-BotMailNotice-0.0.1/setup.py` & `nonebot-plugin-BotMailNotice-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiosmtplib>=2.0.0,<3.0.0', 'nonebot2>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-botmailnotice',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '基于nonebot2bot断连时的Mail通知插件',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-BotMailNotice\n\n_✨ bot断连时的Mail通知插件 ✨_\n\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ZM25XC/BotMailNotice.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-BotMailNotice">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-BotMailNotice.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n\n</div>\n\n\n## 介绍\n\n- 可以在bot断开与nonebot2的连接时向指定邮箱发送邮件通知，用来通知是否掉线\n  \n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/BotMailNotice.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n- 使用`pip install nonebot-plugin-BotMailNotice`来进行安装,使用`pip install nonebot-plugin-BotMailNotice -U`进行更新\n- 使用`nb plugin install nonebot-plugin-BotMailNotice`来进行安装,使用`nb plugin install nonebot-plugin-BotMailNotice -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`nonebot_plugin_BotMailNotice`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 nonebot_plugin_BotMailNotice\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n\n\n##  配置\n运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中配置项\n\n| 配置项 | 必填 | 值类型 | 默认值 | 说明 |\n|:------:|:----:|:---:|:---:|:--:|\n| username | 是 | str | ""  | 邮箱账号 |\n| password | 是 | str | ""  | 邮箱密码或授权码 |\n| hostname | 是 | str | ""  | 邮箱服务器地址 |\n| port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |\n\n## 示例配置\n  \n```env\nmail_notice=\'{\n"username":"xxx@qq.com",\n"password":"qflgxxxxxx",\n"hostname":"smtp.qq.com",\n"port":587\n}\'\n```',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-BotMailNotice\n\n_✨ bot断连时的Mail通知插件 ✨_\n\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ZM25XC/BotMailNotice.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-BotMailNotice">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-BotMailNotice.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n\n</div>\n\n\n## 介绍\n\n- 可以在bot断开与nonebot2的连接时向指定邮箱发送邮件通知，用来通知是否掉线\n  \n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/BotMailNotice.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n- 使用`pip install nonebot-plugin-BotMailNotice`来进行安装,使用`pip install nonebot-plugin-BotMailNotice -U`进行更新\n- 使用`nb plugin install nonebot-plugin-BotMailNotice`来进行安装,使用`nb plugin install nonebot-plugin-BotMailNotice -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`nonebot_plugin_BotMailNotice`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 nonebot_plugin_BotMailNotice\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["nonebot_plugin_BotMailNotice"]`\n\n</details>\n\n\n\n##  配置\n运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中配置项\n\n|  配置项  | 必填  | 值类型 | 默认值 |            说明            |\n| :------: | :---: | :----: | :----: | :------------------------: |\n| username |  是   |  str   |   ""   |          邮箱账号          |\n| password |  是   |  str   |   ""   |      邮箱密码或授权码      |\n| hostname |  是   |  str   |   ""   |       邮箱服务器地址       |\n|   port   |  是   |  int   |  465   | 邮箱端口号，ssl模式时为465 |\n\n## 示例配置\n  \n```env\nmail_notice=\'{\n"username":"xxx@qq.com",\n"password":"qflgxxxxxx",\n"hostname":"smtp.qq.com",\n"port":587\n}\'\n```',
     'author': 'ZM25XC',
     'author_email': 'xingling25@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ZM25XC/BotMailNotice',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_botmailnotice'] package_data = \ {'': ['*']} install_requires
 = \ ['aiosmtplib>=2.0.0,<3.0.0', 'nonebot2>=2.0.0,<3.0.0'] setup_kwargs =
-{ 'name': 'nonebot-plugin-botmailnotice', 'version': '0.0.1', 'description':
+{ 'name': 'nonebot-plugin-botmailnotice', 'version': '0.0.2', 'description':
 'åºäºnonebot2botæ­è¿æ¶çMailéç¥æä»¶', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
   \n\n# nonebot-plugin-BotMailNotice\n\n_â¨ botæ­è¿æ¶çMailéç¥æä»¶
@@ -24,19 +24,21 @@
 å°`nonebot_plugin_BotMailNotice`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯\n\n-
 æä»¶ç»æå¦ä¸\n\n ```py\n ð¦ AweSome-Bot\n âââ ð awesome_bot\n
 â âââ ð plugins\n | âââ ð nonebot_plugin_BotMailNotice\n |
 âââ ð __init__.py\n âââ ð .env.prod\n âââ ð
 .gitignore\n âââ ð pyproject.toml\n âââ ð README.md\n ```\n\n
 \n\n\n\n\nä½¿ç¨ç¬¬äºç§æ¹å¼å®è£çæ­¤æ¹æ³\n\n-
 å¨`pyproject.toml`éç`[tool.nonebot]`ä¸­æ·»å `plugins =
-["TeenStudy"]`\n\n\n\n\n\n## éç½®\nè¿è¡æä»¶åï¼éè¦å¨ nonebot2
+["nonebot_plugin_BotMailNotice"]`\n\n\n\n\n\n##
+éç½®\nè¿è¡æä»¶åï¼éè¦å¨ nonebot2
 é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­éç½®é¡¹\n\n| éç½®é¡¹ | å¿å¡« |
-å¼ç±»å | é»è®¤å¼ | è¯´æ |\n|:------:|:----:|:---:|:---:|:--:|\n|
-username | æ¯ | str | "" | é®ç®±è´¦å· |\n| password | æ¯ | str | "" |
-é®ç®±å¯ç æææç  |\n| hostname | æ¯ | str | "" | é®ç®±æå¡å¨å°å
-|\n| port | æ¯ | int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 |\n\n##
-ç¤ºä¾éç½®\n \n```env\nmail_notice=\'{\n"username":"xxx@qq.com",\n"password":
+å¼ç±»å | é»è®¤å¼ | è¯´æ |\n| :------: | :---: | :----: | :----: | :-----
+-------------------: |\n| username | æ¯ | str | "" | é®ç®±è´¦å· |\n|
+password | æ¯ | str | "" | é®ç®±å¯ç æææç  |\n| hostname | æ¯ | str
+| "" | é®ç®±æå¡å¨å°å |\n| port | æ¯ | int | 465 |
+é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 |\n\n## ç¤ºä¾éç½®\n
+\n```env\nmail_notice=\'{\n"username":"xxx@qq.com",\n"password":
 "qflgxxxxxx",\n"hostname":"smtp.qq.com",\n"port":587\n}\'\n```', 'author':
 'ZM25XC', 'author_email': 'xingling25@qq.com', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'https://github.com/ZM25XC/BotMailNotice',
 'packages': packages, 'package_data': package_data, 'install_requires':
 install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot-plugin-BotMailNotice-0.0.1/PKG-INFO` & `nonebot-plugin-BotMailNotice-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-botmailnotice
-Version: 0.0.1
+Version: 0.0.2
 Summary: 基于nonebot2bot断连时的Mail通知插件
 Home-page: https://github.com/ZM25XC/BotMailNotice
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -87,29 +87,29 @@
     
 
 </details>
 
 <details>
 <summary>使用第二种方式安装看此方法</summary>
 
-- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`
+- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["nonebot_plugin_BotMailNotice"]`
 
 </details>
 
 
 
 ##  配置
 运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中配置项
 
-| 配置项 | 必填 | 值类型 | 默认值 | 说明 |
-|:------:|:----:|:---:|:---:|:--:|
-| username | 是 | str | ""  | 邮箱账号 |
-| password | 是 | str | ""  | 邮箱密码或授权码 |
-| hostname | 是 | str | ""  | 邮箱服务器地址 |
-| port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
+|  配置项  | 必填  | 值类型 | 默认值 |            说明            |
+| :------: | :---: | :----: | :----: | :------------------------: |
+| username |  是   |  str   |   ""   |          邮箱账号          |
+| password |  是   |  str   |   ""   |      邮箱密码或授权码      |
+| hostname |  是   |  str   |   ""   |       邮箱服务器地址       |
+|   port   |  是   |  int   |  465   | 邮箱端口号，ssl模式时为465 |
 
 ## 示例配置
   
 ```env
 mail_notice='{
 "username":"xxx@qq.com",
 "password":"qflgxxxxxx",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-botmailnotice Version: 0.0.1
+Metadata-Version: 2.1 Name: nonebot-plugin-botmailnotice Version: 0.0.2
 Summary: åºäºnonebot2botæ­è¿æ¶çMailéç¥æä»¶ Home-page: https://
 github.com/ZM25XC/BotMailNotice License: MIT Author: ZM25XC Author-email:
 xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiosmtplib (>=2.0.0,<3.0.0) Requires-Dist: nonebot2
@@ -24,16 +24,17 @@
 ä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³ -
 å°`nonebot_plugin_BotMailNotice`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯
 - æä»¶ç»æå¦ä¸ ```py ð¦ AweSome-Bot âââ ð awesome_bot â
 âââ ð plugins | âââ ð nonebot_plugin_BotMailNotice |
 âââ ð __init__.py âââ ð .env.prod âââ ð .gitignore
 âââ ð pyproject.toml âââ ð README.md ```
 ä½¿ç¨ç¬¬äºç§æ¹å¼å®è£çæ­¤æ¹æ³ - å¨`pyproject.toml`éç`
-[tool.nonebot]`ä¸­æ·»å `plugins = ["TeenStudy"]`  ## éç½®
+[tool.nonebot]`ä¸­æ·»å `plugins = ["nonebot_plugin_BotMailNotice"]`  ## éç½®
 è¿è¡æä»¶åï¼éè¦å¨ nonebot2
 é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­éç½®é¡¹ | éç½®é¡¹ | å¿å¡« |
-å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| | username
-| æ¯ | str | "" | é®ç®±è´¦å· | | password | æ¯ | str | "" |
-é®ç®±å¯ç æææç  | | hostname | æ¯ | str | "" | é®ç®±æå¡å¨å°å
-| | port | æ¯ | int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | ##
-ç¤ºä¾éç½® ```env mail_notice='{ "username":"xxx@qq.com", "password":
-"qflgxxxxxx", "hostname":"smtp.qq.com", "port":587 }' ```
+å¼ç±»å | é»è®¤å¼ | è¯´æ | | :------: | :---: | :----: | :----: | :------
+------------------: | | username | æ¯ | str | "" | é®ç®±è´¦å· | | password |
+æ¯ | str | "" | é®ç®±å¯ç æææç  | | hostname | æ¯ | str | "" |
+é®ç®±æå¡å¨å°å | | port | æ¯ | int | 465 |
+é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | ## ç¤ºä¾éç½® ```env mail_notice='
+{ "username":"xxx@qq.com", "password":"qflgxxxxxx", "hostname":"smtp.qq.com",
+"port":587 }' ```
```

