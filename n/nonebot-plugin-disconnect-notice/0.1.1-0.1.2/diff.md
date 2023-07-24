# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.1.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.1.tar` & `nonebot_plugin_disconnect_notice-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-24 05:55:20.591489 nonebot_plugin_disconnect_notice-0.1.1/LICENSE
--rw-r--r--   0        0        0     3164 2023-07-24 05:55:20.591489 nonebot_plugin_disconnect_notice-0.1.1/README.md
--rw-r--r--   0        0        0     2240 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      649 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      586 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2316 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      425 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-24 11:10:51.700522 nonebot_plugin_disconnect_notice-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3689 2023-07-24 11:10:51.700522 nonebot_plugin_disconnect_notice-0.1.2/README.md
+-rw-r--r--   0        0        0     2328 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      586 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2316 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      425 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/LICENSE` & `nonebot_plugin_disconnect_notice-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/README.md` & `nonebot_plugin_disconnect_notice-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 
 ## 📖 介绍
 
-- 可以在qqbot断开与nonebot连接时向主人进行例如邮件的通知
+- 可以在qqbot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人QQbot可能被风控掉线
 - 目前支持onebotv11协议，通知方式支持邮件通知
 - 如果有其他协议或通知方式的需求，欢迎提issus或pr
 
+>断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-disconnect-notice
@@ -63,14 +65,15 @@
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
+| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下QQbot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
```

#### html2text {}

```diff
@@ -1,32 +1,37 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-disconnect-notice _â¨ QQbotæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
-å¯ä»¥å¨qqbotæ­å¼ä¸nonebotè¿æ¥æ¶åä¸»äººè¿è¡ä¾å¦é®ä»¶çéç¥ -
-ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr ## ð¿
-å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-disconnect-
-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pdm pdm add nonebot-plugin-disconnect-notice   poetry poetry add nonebot-
-plugin-disconnect-notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨
-nonebot2 é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
+å¯ä»¥å¨qqbotæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººQQbotå¯è½è¢«é£æ§æçº¿
+- ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
+å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+>æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
+## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
+nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
+notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨ nonebot2
+é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
 éç½®é¡¹ | å¿å¡« | å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:-
 --:|:--:| | disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦
 114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
 é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
 int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
 disconnect_notice_notice_email | æ¯ | str | "" |
-æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ |  ç¤ºä¾éç½® ```env #
-disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user = "114514@yeah.net"
-#é®ç®±è´¦å· disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
+æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
+| bool | False |
+å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸QQbotæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+|  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
+disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
+disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
 ----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
 å¦ | ç§è/ç¾¤è |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,20 +37,22 @@
         msg = f"测试邮件发送失败，请重新检查配置项参数正确性，错误信息为: {res}"
     await matcher.finish(msg)
 
 
 @driver.on_bot_disconnect
 async def disconnect(bot: Union[V11Bot]):
     """bot断连触发器"""
-    send_notice(bot)
+    # 开发者模式下不生效
+    if not plugin_config.disconnect_notice_dev_mode:
+        send_notice(bot)
 
 
 @driver.on_bot_connect
 async def connect(bot: V11Bot):
-    """插件载入时检测配置完整性"""
+    """bot接入时检测配置完整性"""
     if not mail_config.check_params():
         # 缺少参数,私聊通知主人
         super_user: str = list(global_config.superusers)[0]
         if super_user:
             await bot.send_private_msg(user_id=int(super_user), message="【插件nonebot-plugin-disconnect-notice】\n"
                                                                         "缺少mail配置项，请按照https://github.com"
                                                                         "/Cypas/nonebot_plugin_disconnect_notice#%EF%B8%8F-%E9%85%8D%E7%BD%AE"
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
 class Config(BaseModel):
     disconnect_notice_smtp_user = ""
     disconnect_notice_smtp_password = ""
     disconnect_notice_smtp_server = ""
     disconnect_notice_smtp_port = 465
     disconnect_notice_notice_email = ""
+    disconnect_notice_dev_mode = False
 
 
 driver = get_driver()
 # 本地测试时由于不启动 driver，需要将下面两行注释并取消再下一行的注释
 global_config = driver.config
 plugin_config = Config.parse_obj(global_config)
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.1/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.1
+Version: 0.1.2
 Summary: QQbot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,18 +36,20 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 
 ## 📖 介绍
 
-- 可以在qqbot断开与nonebot连接时向主人进行例如邮件的通知
+- 可以在qqbot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人QQbot可能被风控掉线
 - 目前支持onebotv11协议，通知方式支持邮件通知
 - 如果有其他协议或通知方式的需求，欢迎提issus或pr
 
+>断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-disconnect-notice
@@ -79,14 +81,15 @@
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
+| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下QQbot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
```

#### html2text {}

```diff
@@ -1,40 +1,45 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.1
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.2
 Summary: QQbotæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2
 (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-disconnect-notice _â¨ QQbotæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
-å¯ä»¥å¨qqbotæ­å¼ä¸nonebotè¿æ¥æ¶åä¸»äººè¿è¡ä¾å¦é®ä»¶çéç¥ -
-ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr ## ð¿
-å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-disconnect-
-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pdm pdm add nonebot-plugin-disconnect-notice   poetry poetry add nonebot-
-plugin-disconnect-notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨
-nonebot2 é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
+å¯ä»¥å¨qqbotæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººQQbotå¯è½è¢«é£æ§æçº¿
+- ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
+å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+>æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
+## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
+nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
+notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨ nonebot2
+é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
 éç½®é¡¹ | å¿å¡« | å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:-
 --:|:--:| | disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦
 114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
 é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
 int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
 disconnect_notice_notice_email | æ¯ | str | "" |
-æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ |  ç¤ºä¾éç½® ```env #
-disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user = "114514@yeah.net"
-#é®ç®±è´¦å· disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
+æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
+| bool | False |
+å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸QQbotæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+|  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
+disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
+disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
 ----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
 å¦ | ç§è/ç¾¤è |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
```

