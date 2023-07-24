# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.2.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.2.tar` & `nonebot_plugin_disconnect_notice-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-24 11:10:51.700522 nonebot_plugin_disconnect_notice-0.1.2/LICENSE
--rw-r--r--   0        0        0     3689 2023-07-24 11:10:51.700522 nonebot_plugin_disconnect_notice-0.1.2/README.md
--rw-r--r--   0        0        0     2328 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      688 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      586 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2316 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      425 2023-07-24 11:10:51.704522 nonebot_plugin_disconnect_notice-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-24 14:36:09.664898 nonebot_plugin_disconnect_notice-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3678 2023-07-24 14:36:09.664898 nonebot_plugin_disconnect_notice-0.1.3/README.md
+-rw-r--r--   0        0        0     2243 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      586 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2134 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      445 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4298 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/LICENSE` & `nonebot_plugin_disconnect_notice-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/README.md` & `nonebot_plugin_disconnect_notice-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-disconnect-notice
 
-_✨ QQbot断连时的通知插件 ✨_
+_✨ bot断连时的通知插件 ✨_
 
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/Skyminers/Bot-Splatoon3.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-disconnect-notice">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-disconnect-notice.svg" alt="pypi">
@@ -20,17 +20,17 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 
 ## 📖 介绍
 
-- 可以在qqbot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人QQbot可能被风控掉线
-- 目前支持onebotv11协议，通知方式支持邮件通知
-- 如果有其他协议或通知方式的需求，欢迎提issus或pr
+- 可以在bot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人bot可能被风控掉线
+- 目前支持全部适配器协议，通知方式支持邮件通知
+- 如果有其他通知方式的需求，欢迎提issus或pr
 
 >断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -65,15 +65,15 @@
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
-| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下QQbot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
-  # nonebot-plugin-disconnect-notice _â¨ QQbotæ­è¿æ¶çéç¥æä»¶ â¨_
+   # nonebot-plugin-disconnect-notice _â¨ botæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
-å¯ä»¥å¨qqbotæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººQQbotå¯è½è¢«é£æ§æçº¿
-- ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+å¯ä»¥å¨botæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººbotå¯è½è¢«é£æ§æçº¿
+- ç®åæ¯æå¨é¨ééå¨åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
+å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
 >æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
@@ -20,15 +20,15 @@
 114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
 é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
 int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
 disconnect_notice_notice_email | æ¯ | str | "" |
 æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
 | bool | False |
-å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸QQbotæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import Union
-
 from nonebot.internal.matcher import Matcher
 from nonebot.plugin import PluginMetadata
+from nonebot import Bot
 
 # onebot11 协议
 from nonebot.adapters.onebot.v11 import Bot as V11Bot
 from nonebot import on_command
 from nonebot.permission import SUPERUSER
 
 from .config import driver, plugin_config, global_config
 from .utils import send_notice, mail_config, send_mail
 
 __plugin_meta__ = PluginMetadata(
-    name="QQbot断连通知",
-    description="QQbot断连时的通知插件",
+    name="bot断连通知",
+    description="bot断连时的通知插件，当前支持邮件通知",
     usage="""
     超级用户指令:
         断连通知测试:主动触发掉线通知测试
     """,
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
     homepage="https://github.com/Cypas/nonebot_plugin_disconnect_notice",
     # 发布必填。
-    supported_adapters={"~onebot.v11"},
+    supported_adapters=None,
 )
 
 notice_test = on_command("断连通知测试", permission=SUPERUSER)
 
 
 @notice_test.handle()
 async def _(matcher: Matcher):
     """主动触发掉线通知测试"""
     msg = "已发送测试邮件，如未收到请检查邮件垃圾箱"
-    res = send_mail("114514", test=True)
+    res = await send_mail("114514", test=True)
     if res is not None:
         msg = f"测试邮件发送失败，请重新检查配置项参数正确性，错误信息为: {res}"
     await matcher.finish(msg)
 
 
 @driver.on_bot_disconnect
-async def disconnect(bot: Union[V11Bot]):
+async def disconnect(bot: Bot):
     """bot断连触发器"""
     # 开发者模式下不生效
     if not plugin_config.disconnect_notice_dev_mode:
-        send_notice(bot)
+        await send_notice(bot)
 
 
 @driver.on_bot_connect
-async def connect(bot: V11Bot):
+async def connect(bot: Bot):
     """bot接入时检测配置完整性"""
-    if not mail_config.check_params():
-        # 缺少参数,私聊通知主人
-        super_user: str = list(global_config.superusers)[0]
-        if super_user:
-            await bot.send_private_msg(user_id=int(super_user), message="【插件nonebot-plugin-disconnect-notice】\n"
-                                                                        "缺少mail配置项，请按照https://github.com"
-                                                                        "/Cypas/nonebot_plugin_disconnect_notice#%EF%B8%8F-%E9%85%8D%E7%BD%AE"
-                                                                        "\n添加配置项后，再重新载入插件")
+    if isinstance(bot, V11Bot):
+        if not mail_config.check_params():
+            # 缺少参数,私聊通知主人
+            super_user: str = list(global_config.superusers)[0]
+            if super_user:
+                msg = "【插件nonebot-plugin-disconnect-notice】\n缺少mail配置项，请按照" \
+                      "https://github.com/Cypas/nonebot_plugin_disconnect_notice#%EF%B8%8F-%E9%85%8D%E7%BD%AE"\
+                      "\n添加配置项后，再重新载入插件"
+                await bot.send_private_msg(user_id=int(super_user), message=msg)
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,65 @@
-import smtplib
-from email.mime import text
-from email.mime.text import MIMEText
-from email.mime.multipart import MIMEMultipart
 from email.header import Header
-from typing import Union
-
-# onebot11 协议
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+import aiosmtplib
 
-from nonebot import logger
+from nonebot import logger, Bot
 from .config import plugin_config
 from .dataClass import MailConfig
 
 mail_config: MailConfig = MailConfig(
     user=plugin_config.disconnect_notice_smtp_user,
     password=plugin_config.disconnect_notice_smtp_password,
     server=plugin_config.disconnect_notice_smtp_server,
     port=plugin_config.disconnect_notice_smtp_port,
     notice_email=plugin_config.disconnect_notice_notice_email,
 )
 
 
-def send_notice(bot: Union[V11Bot]):
+async def send_notice(bot: Bot):
     """整合发送通知消息"""
     bot_id = get_bot_id(bot)
-    send_mail(bot_id)
+    await send_mail(bot_id)
 
 
-def send_mail(bot_id: str, test: bool = False):
+async def send_mail(bot_id: str, test: bool = False):
     """发送邮件通知"""
     # 邮箱凭据
     global mail_config
     # 参数校验
     if not mail_config.check_params():
         error = "邮件通知缺少配置参数，无法进行通知"
         logger.error(error)
         return error
     # 邮件正文
-    subject = f"你的QQbot掉线了"
-    content = f"你的QQbot账号: {bot_id} 掉线了，可能是被风控了，赶快去看看吧"
+    subject = f"你的bot掉线了"
+    content = f"你的bot账号: {bot_id} 掉线了，可能是被风控了，赶快去看看吧"
     if test:
         subject = f"掉线通知测试"
         content = f"这是一封掉线通知测试邮件，你bot并没有掉线"
 
     # 构造邮件内容
     message = MIMEMultipart("alternative")
     message["Subject"] = Header(subject, 'utf-8')
     message["From"] = mail_config.user
     message["To"] = mail_config.notice_email
     message.attach(MIMEText(content))
     # 连接SMTP服务器并发送邮件
+    use_tls = False
     if mail_config.port == 465:
-        server = smtplib.SMTP_SSL(mail_config.server, mail_config.port)
-    else:
-        # 25或其他
-        server = smtplib.SMTP(mail_config.server, mail_config.port)
+        use_tls = True
     try:
-        server.login(mail_config.user, mail_config.password)
-        server.sendmail(mail_config.user, mail_config.notice_email, message.as_string())
+        async with aiosmtplib.SMTP(hostname=mail_config.server, port=mail_config.port, use_tls=use_tls) as smtp:
+            await smtp.login(mail_config.user,mail_config.password)
+            await smtp.send_message(message)
     except Exception as e:
         logger.error(f"邮件发送失败，错误信息如下{e}")
         return e
     logger.info("通知邮件发送成功!")
     return
 
 
-def get_bot_id(bot: Union[V11Bot]) -> str:
+def get_bot_id(bot) -> str:
     """获取bot_id"""
     bot_id = bot.self_id
     return bot_id
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.2/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.2
-Summary: QQbot断连时的通知插件
+Version: 0.1.3
+Summary: bot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-disconnect-notice
 
-_✨ QQbot断连时的通知插件 ✨_
+_✨ bot断连时的通知插件 ✨_
 
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/Skyminers/Bot-Splatoon3.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-disconnect-notice">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-disconnect-notice.svg" alt="pypi">
@@ -36,17 +37,17 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 
 ## 📖 介绍
 
-- 可以在qqbot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人QQbot可能被风控掉线
-- 目前支持onebotv11协议，通知方式支持邮件通知
-- 如果有其他协议或通知方式的需求，欢迎提issus或pr
+- 可以在bot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人bot可能被风控掉线
+- 目前支持全部适配器协议，通知方式支持邮件通知
+- 如果有其他通知方式的需求，欢迎提issus或pr
 
 >断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -81,15 +82,15 @@
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
-| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下QQbot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.2
-Summary: QQbotæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.3
+Summary: botæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2
-(>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
+Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-
+onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-
+Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
-  # nonebot-plugin-disconnect-notice _â¨ QQbotæ­è¿æ¶çéç¥æä»¶ â¨_
+   # nonebot-plugin-disconnect-notice _â¨ botæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
-å¯ä»¥å¨qqbotæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººQQbotå¯è½è¢«é£æ§æçº¿
-- ç®åæ¯æonebotv11åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»åè®®æéç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+å¯ä»¥å¨botæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººbotå¯è½è¢«é£æ§æçº¿
+- ç®åæ¯æå¨é¨ééå¨åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
+å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
 >æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
@@ -28,15 +29,15 @@
 114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
 é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
 int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
 disconnect_notice_notice_email | æ¯ | str | "" |
 æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
 | bool | False |
-å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸QQbotæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
```

