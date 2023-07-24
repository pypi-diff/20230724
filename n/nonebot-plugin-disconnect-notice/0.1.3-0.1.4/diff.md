# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.3.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.3.tar` & `nonebot_plugin_disconnect_notice-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-24 14:36:09.664898 nonebot_plugin_disconnect_notice-0.1.3/LICENSE
--rw-r--r--   0        0        0     3678 2023-07-24 14:36:09.664898 nonebot_plugin_disconnect_notice-0.1.3/README.md
--rw-r--r--   0        0        0     2243 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      688 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      586 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2134 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      445 2023-07-24 14:36:09.668899 nonebot_plugin_disconnect_notice-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4298 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3680 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/README.md
+-rw-r--r--   0        0        0     2497 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      784 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2099 2023-07-24 16:24:22.722401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      445 2023-07-24 16:24:22.722401 nonebot_plugin_disconnect_notice-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/LICENSE` & `nonebot_plugin_disconnect_notice-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/README.md` & `nonebot_plugin_disconnect_notice-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 </div>
 
 
 ## 📖 介绍
 
 - 可以在bot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人bot可能被风控掉线
 - 目前支持全部适配器协议，通知方式支持邮件通知
-- 如果有其他通知方式的需求，欢迎提issus或pr
+- 如果有其他通知方式的需求，欢迎提issues或pr
 
 >断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -83,17 +83,17 @@
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
-| 指令 | 权限 | 需要@ | 范围  |           说明            |
-|:-----:|:----:|:----:|:---:|:-----------------------:|
-| 断连通知测试 | 主人 | 否 | 私聊/群聊 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
+| 指令 | 权限 | 需要@ |  范围  |           说明            |
+|:-----:|:----:|:----:|:----:|:-----------------------:|
+| 断连通知测试 | 主人 | 否 | 所有会话 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
 ### 效果图
 <details>
 <summary>邮件通知</summary>
 
 ![mail.png](images/mail.png)
 
 </details>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # nonebot-plugin-disconnect-notice _â¨ botæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
 å¯ä»¥å¨botæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººbotå¯è½è¢«é£æ§æçº¿
 - ç®åæ¯æå¨é¨ééå¨åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissuesæpr
 >æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
@@ -28,12 +28,12 @@
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
-å¦ | ç§è/ç¾¤è |
+----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
+å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # onebot11 协议
 from nonebot.adapters.onebot.v11 import Bot as V11Bot
 from nonebot import on_command
 from nonebot.permission import SUPERUSER
 
 from .config import driver, plugin_config, global_config
+from .dataClass import BotParams
 from .utils import send_notice, mail_config, send_mail
 
 __plugin_meta__ = PluginMetadata(
     name="bot断连通知",
     description="bot断连时的通知插件，当前支持邮件通知",
     usage="""
     超级用户指令:
@@ -27,33 +28,41 @@
 notice_test = on_command("断连通知测试", permission=SUPERUSER)
 
 
 @notice_test.handle()
 async def _(matcher: Matcher):
     """主动触发掉线通知测试"""
     msg = "已发送测试邮件，如未收到请检查邮件垃圾箱"
-    res = await send_mail("114514", test=True)
+    bot_params = BotParams(
+        adapter_name="114514",
+        bot_id="114514"
+    )
+    res = await send_mail(bot_params, test=True)
     if res is not None:
         msg = f"测试邮件发送失败，请重新检查配置项参数正确性，错误信息为: {res}"
     await matcher.finish(msg)
 
 
 @driver.on_bot_disconnect
 async def disconnect(bot: Bot):
     """bot断连触发器"""
     # 开发者模式下不生效
     if not plugin_config.disconnect_notice_dev_mode:
-        await send_notice(bot)
+        bot_params = BotParams(
+            adapter_name=bot.adapter.get_name(),
+            bot_id=bot.self_id
+        )
+        await send_notice(bot_params)
 
 
 @driver.on_bot_connect
 async def connect(bot: Bot):
     """bot接入时检测配置完整性"""
     if isinstance(bot, V11Bot):
         if not mail_config.check_params():
             # 缺少参数,私聊通知主人
             super_user: str = list(global_config.superusers)[0]
             if super_user:
                 msg = "【插件nonebot-plugin-disconnect-notice】\n缺少mail配置项，请按照" \
-                      "https://github.com/Cypas/nonebot_plugin_disconnect_notice#%EF%B8%8F-%E9%85%8D%E7%BD%AE"\
+                      "https://github.com/Cypas/nonebot_plugin_disconnect_notice#%EF%B8%8F-%E9%85%8D%E7%BD%AE" \
                       "\n添加配置项后，再重新载入插件"
                 await bot.send_private_msg(user_id=int(super_user), message=msg)
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,7 +13,16 @@
 
     def check_params(self) -> bool:
         """检查参数是否填写完整"""
         if self.user and self.password and self.server and self.port and self.notice_email:
             return True
         else:
             return False
+
+
+class BotParams:
+    def __init__(self,
+                 adapter_name: str,
+                 bot_id: str,
+                 ):
+        self.adapter_name = adapter_name
+        self.bot_id = bot_id
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 import aiosmtplib
 
 from nonebot import logger, Bot
 from .config import plugin_config
-from .dataClass import MailConfig
+from .dataClass import MailConfig, BotParams
 
 mail_config: MailConfig = MailConfig(
     user=plugin_config.disconnect_notice_smtp_user,
     password=plugin_config.disconnect_notice_smtp_password,
     server=plugin_config.disconnect_notice_smtp_server,
     port=plugin_config.disconnect_notice_smtp_port,
     notice_email=plugin_config.disconnect_notice_notice_email,
 )
 
 
-async def send_notice(bot: Bot):
+async def send_notice(bot_params: BotParams):
     """整合发送通知消息"""
-    bot_id = get_bot_id(bot)
-    await send_mail(bot_id)
+    await send_mail(bot_params)
 
 
-async def send_mail(bot_id: str, test: bool = False):
+async def send_mail(bot_params: BotParams, test: bool = False):
     """发送邮件通知"""
     # 邮箱凭据
     global mail_config
     # 参数校验
     if not mail_config.check_params():
         error = "邮件通知缺少配置参数，无法进行通知"
         logger.error(error)
         return error
     # 邮件正文
     subject = f"你的bot掉线了"
-    content = f"你的bot账号: {bot_id} 掉线了，可能是被风控了，赶快去看看吧"
+    content = f"你的 {bot_params.adapter_name} 适配器的bot账号: {bot_params.bot_id} 掉线了，可能是被风控了，赶快去看看吧"
     if test:
         subject = f"掉线通知测试"
         content = f"这是一封掉线通知测试邮件，你bot并没有掉线"
 
     # 构造邮件内容
     message = MIMEMultipart("alternative")
     message["Subject"] = Header(subject, 'utf-8')
@@ -46,20 +45,15 @@
     message.attach(MIMEText(content))
     # 连接SMTP服务器并发送邮件
     use_tls = False
     if mail_config.port == 465:
         use_tls = True
     try:
         async with aiosmtplib.SMTP(hostname=mail_config.server, port=mail_config.port, use_tls=use_tls) as smtp:
-            await smtp.login(mail_config.user,mail_config.password)
+            await smtp.login(mail_config.user, mail_config.password)
             await smtp.send_message(message)
     except Exception as e:
         logger.error(f"邮件发送失败，错误信息如下{e}")
         return e
     logger.info("通知邮件发送成功!")
     return
 
-
-def get_bot_id(bot) -> str:
-    """获取bot_id"""
-    bot_id = bot.self_id
-    return bot_id
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.3/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.3
+Version: 0.1.4
 Summary: bot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -39,15 +39,15 @@
 </div>
 
 
 ## 📖 介绍
 
 - 可以在bot断开与nonebot的连接时向主人发送例如邮件的通知，用来通知主人bot可能被风控掉线
 - 目前支持全部适配器协议，通知方式支持邮件通知
-- 如果有其他通知方式的需求，欢迎提issus或pr
+- 如果有其他通知方式的需求，欢迎提issues或pr
 
 >断连事件是通过判断nb与bot端的ws连接状态来实现的，当主动停止nonebot框架时，会先断开ws连接，随后再退出,这意味着主动停止nonebot框架时，也会收到插件发送的离线通知消息，这个无法避免，属于正常情况
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -100,17 +100,17 @@
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
-| 指令 | 权限 | 需要@ | 范围  |           说明            |
-|:-----:|:----:|:----:|:---:|:-----------------------:|
-| 断连通知测试 | 主人 | 否 | 私聊/群聊 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
+| 指令 | 权限 | 需要@ |  范围  |           说明            |
+|:-----:|:----:|:----:|:----:|:-----------------------:|
+| 断连通知测试 | 主人 | 否 | 所有会话 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
 ### 效果图
 <details>
 <summary>邮件通知</summary>
 
 ![mail.png](images/mail.png)
 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.4
 Summary: botæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-
 onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-
@@ -10,15 +10,15 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # nonebot-plugin-disconnect-notice _â¨ botæ­è¿æ¶çéç¥æä»¶ â¨_
                            [license] [pypi] [python]
 ## ð ä»ç» -
 å¯ä»¥å¨botæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººbotå¯è½è¢«é£æ§æçº¿
 - ç®åæ¯æå¨é¨ééå¨åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
-å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissusæpr
+å¦ææå¶ä»éç¥æ¹å¼çéæ±ï¼æ¬¢è¿æissuesæpr
 >æ­è¿äºä»¶æ¯éè¿å¤æ­nbä¸botç«¯çwsè¿æ¥ç¶ææ¥å®ç°çï¼å½ä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¼åæ­å¼wsè¿æ¥ï¼éååéåº,è¿æå³çä¸»å¨åæ­¢nonebotæ¡æ¶æ¶ï¼ä¹ä¼æ¶å°æä»¶åéçç¦»çº¿éç¥æ¶æ¯ï¼è¿ä¸ªæ æ³é¿åï¼å±äºæ­£å¸¸æåµ
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
@@ -37,12 +37,12 @@
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
 ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
-å¦ | ç§è/ç¾¤è |
+----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
+å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

