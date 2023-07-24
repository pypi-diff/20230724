# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.0.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.0.tar` & `nonebot_plugin_disconnect_notice-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/LICENSE
--rw-r--r--   0        0        0     2864 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/README.md
--rw-r--r--   0        0        0     1494 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      649 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      583 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2085 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      425 2023-07-24 03:55:13.714954 nonebot_plugin_disconnect_notice-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-24 05:55:20.591489 nonebot_plugin_disconnect_notice-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3164 2023-07-24 05:55:20.591489 nonebot_plugin_disconnect_notice-0.1.1/README.md
+-rw-r--r--   0        0        0     2240 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      586 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2316 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      425 2023-07-24 05:55:20.595489 nonebot_plugin_disconnect_notice-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.0/LICENSE` & `nonebot_plugin_disconnect_notice-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.0/README.md` & `nonebot_plugin_disconnect_notice-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -66,25 +66,33 @@
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
 
 <details>
 <summary>示例配置</summary>
+  
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 ```
+
 </details>
 
 ## 🎉 使用
+### 指令表
+| 指令 | 权限 | 需要@ | 范围  |           说明            |
+|:-----:|:----:|:----:|:---:|:-----------------------:|
+| 断连通知测试 | 主人 | 否 | 私聊/群聊 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
 ### 效果图
 <details>
 <summary>邮件通知</summary>
 
+![mail.png](images/mail.png)
+
 </details>
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -22,9 +22,13 @@
 disconnect_notice_notice_email | æ¯ | str | "" |
 æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ |  ç¤ºä¾éç½® ```env #
 disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user = "114514@yeah.net"
 #é®ç®±è´¦å· disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
-ä½¿ç¨ ### ææå¾  é®ä»¶éç¥  ##
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
+----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
+å¦ | ç§è/ç¾¤è |
+ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
+ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.0/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.1.1/nonebot_plugin_disconnect_notice/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import smtplib
 from email.mime import text
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.header import Header
+from typing import Union
+
 # onebot11 协议
 from nonebot.adapters.onebot.v11 import Bot as V11Bot
 
 from nonebot import logger
 from .config import plugin_config
 from .dataClass import MailConfig
 
@@ -15,50 +17,55 @@
     password=plugin_config.disconnect_notice_smtp_password,
     server=plugin_config.disconnect_notice_smtp_server,
     port=plugin_config.disconnect_notice_smtp_port,
     notice_email=plugin_config.disconnect_notice_notice_email,
 )
 
 
-def send_notice(bot: V11Bot):
+def send_notice(bot: Union[V11Bot]):
     """整合发送通知消息"""
     bot_id = get_bot_id(bot)
     send_mail(bot_id)
 
 
-def send_mail(bot_id: str):
+def send_mail(bot_id: str, test: bool = False):
     """发送邮件通知"""
     # 邮箱凭据
     global mail_config
     # 参数校验
     if not mail_config.check_params():
-        logger.error("邮件通知缺少配置参数，无法进行通知")
-        return
+        error = "邮件通知缺少配置参数，无法进行通知"
+        logger.error(error)
+        return error
     # 邮件正文
     subject = f"你的QQbot掉线了"
     content = f"你的QQbot账号: {bot_id} 掉线了，可能是被风控了，赶快去看看吧"
+    if test:
+        subject = f"掉线通知测试"
+        content = f"这是一封掉线通知测试邮件，你bot并没有掉线"
 
     # 构造邮件内容
     message = MIMEMultipart("alternative")
     message["Subject"] = Header(subject, 'utf-8')
     message["From"] = mail_config.user
     message["To"] = mail_config.notice_email
     message.attach(MIMEText(content))
     # 连接SMTP服务器并发送邮件
-    if mail_config.smtp_port == 465:
+    if mail_config.port == 465:
         server = smtplib.SMTP_SSL(mail_config.server, mail_config.port)
     else:
         # 25或其他
         server = smtplib.SMTP(mail_config.server, mail_config.port)
     try:
         server.login(mail_config.user, mail_config.password)
         server.sendmail(mail_config.user, mail_config.notice_email, message.as_string())
     except Exception as e:
         logger.error(f"邮件发送失败，错误信息如下{e}")
-        return
+        return e
     logger.info("通知邮件发送成功!")
+    return
 
 
-def get_bot_id(bot: V11Bot) -> str:
+def get_bot_id(bot: Union[V11Bot]) -> str:
     """获取bot_id"""
     bot_id = bot.self_id
     return bot_id
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.0/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.0
+Version: 0.1.1
 Summary: QQbot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -82,26 +82,34 @@
 | disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
 
 <details>
 <summary>示例配置</summary>
+  
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 ```
+
 </details>
 
 ## 🎉 使用
+### 指令表
+| 指令 | 权限 | 需要@ | 范围  |           说明            |
+|:-----:|:----:|:----:|:---:|:-----------------------:|
+| 断连通知测试 | 主人 | 否 | 私聊/群聊 | 主动触发掉线通知测试，用来测试通知是否正常可用 |
 ### 效果图
 <details>
 <summary>邮件通知</summary>
 
+![mail.png](images/mail.png)
+
 </details>
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.0
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.1
 Summary: QQbotæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2
 (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
@@ -30,9 +30,13 @@
 disconnect_notice_notice_email | æ¯ | str | "" |
 æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ |  ç¤ºä¾éç½® ```env #
 disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user = "114514@yeah.net"
 #é®ç®±è´¦å· disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
-ä½¿ç¨ ### ææå¾  é®ä»¶éç¥  ##
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
+----:|:----:|:---:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
+å¦ | ç§è/ç¾¤è |
+ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
+ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

