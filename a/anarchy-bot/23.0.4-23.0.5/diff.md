# Comparing `tmp/anarchy_bot-23.0.4.tar.gz` & `tmp/anarchy_bot-23.0.5.tar.gz`

## Comparing `anarchy_bot-23.0.4.tar` & `anarchy_bot-23.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/build.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/changlog.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/pyrightconfig.json
--rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/setup.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/__main__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/cb.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/chats.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/common.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/config.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/inline.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lang.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lists.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/main.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/msg.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lang/en.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/.gitignore
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/readme.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/build.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/changlog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/pyrightconfig.json
+-rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/setup.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/__main__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/cb.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/chats.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/common.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/inline.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/lang.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/lists.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/main.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/msg.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/anarchy_bot/lang/en.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/.gitignore
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/pyproject.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/readme.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 anarchy_bot-23.0.5/PKG-INFO
```

### Comparing `anarchy_bot-23.0.4/build.py` & `anarchy_bot-23.0.5/build.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/setup.py` & `anarchy_bot-23.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/cb.py` & `anarchy_bot-23.0.5/anarchy_bot/cb.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/chats.py` & `anarchy_bot-23.0.5/anarchy_bot/chats.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/common.py` & `anarchy_bot-23.0.5/anarchy_bot/common.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/config.py` & `anarchy_bot-23.0.5/anarchy_bot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import tgcrypto # type: ignore
     using_tgcrypto = True
 except Exception:
     using_tgcrypto = False
 
 
 app_name = 'anarchy_bot'
-app_version = '23.0.4'
+app_version = '23.0.5'
 c = rich.console.Console()
 c.log(f'imported [deep_sky_blue1]{__file__}')
 app_path = Path(
     __file__
 ).parent.parent.resolve()
 src_path = app_path / app_name
 data_path = app_path / f'{app_name}_data'
```

### Comparing `anarchy_bot-23.0.4/anarchy_bot/inline.py` & `anarchy_bot-23.0.5/anarchy_bot/inline.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/lang.py` & `anarchy_bot-23.0.5/anarchy_bot/lang.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/lists.py` & `anarchy_bot-23.0.5/anarchy_bot/lists.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/main.py` & `anarchy_bot-23.0.5/anarchy_bot/main.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.4/anarchy_bot/msg.py` & `anarchy_bot-23.0.5/anarchy_bot/msg.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,25 @@
         if not log_msg:
             log_msg = error_path
         await msg.reply(
             f'unknown error, please forward this message to @gmankachat\n\nlog: {log_msg}'
         )
 
 
+def is_command(
+    msg_text: str,
+    command: str,
+) -> bool:
+    if msg_text.startswith(command + ''):
+        return True
+    if msg_text.startswith(f'{command}@{config.me.username}'):
+        return True
+    return False
+
+
 async def on_message(
     client: Client,
     msg: Message,
 ) -> None:
     users = {
         '/h': help_msg,
         '/help': help_msg,
@@ -84,27 +95,32 @@
         await chats.remember_chat(
             client,
             msg.chat,
         )
         start = {
             'logs': ask_to_set_logs_chat_msg,
         }
-        for action, func in start.items():
-            if msg.text.endswith(action):
-                await func(client, msg)
+        for action, to_run in start.items():
+            if msg.text.endswith('?startgroup=' + action):
+                await to_run(client, msg)
                 return
-    for excpected_msg, func in users.items():
-        if msg.text.startswith(excpected_msg):
-            c.log(f'got msg {msg.text} from {msg.from_user.id}')
-            return await func(client, msg)
-    for excpected_msg, func in admins.items():
-        if msg.text.startswith(excpected_msg):
+    for excpected_msg, to_run in users.items():
+        if is_command(
+            msg.text,
+            excpected_msg,
+        ):
+            return await to_run(client, msg)
+    for excpected_msg, to_run in admins.items():
+        if is_command(
+            msg.text,
+            excpected_msg,
+        ):
             if await filter_admin(msg):
                 return
-            return await func(client, msg)
+            return await to_run(client, msg)
     if msg.chat.type == pg.enums.ChatType.PRIVATE:
         await msg.reply(
             **get_main_message(msg)
         )
         return
 
 
@@ -112,14 +128,18 @@
     client: Client,
     msg: Message,
 ):
     await msg.reply(
         **get_main_message(msg),
         disable_web_page_preview = True,
     )
+    if msg.from_user.id in config.admins:
+        await msg.reply(
+            t('owner_commands_msg', msg)
+        )
 
 
 async def becomeadmin(
     client: Client,
     msg: Message,
 ):
     splitted = msg.text.split(' ', 1)
@@ -130,14 +150,18 @@
         return
     title = splitted[-1][:16]
     if msg.chat.type != pyrogram.enums.ChatType.SUPERGROUP:
         await msg.reply(
             'wrong chat type, expected supergroup, got ' + str(msg.chat.type).lower()
         )
         return
+    if not msg.from_user:
+        await msg.reply(
+            'you must send message as user, not as channel or chat'
+        )
     text = f'trying to make {mention(msg.from_user)} an admin...'
     responce: Message = await msg.reply(
         text
     )
     while True:
         try:
             await client.promote_chat_member(
```

### Comparing `anarchy_bot-23.0.4/anarchy_bot/lang/en.yml` & `anarchy_bot-23.0.5/anarchy_bot/lang/en.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 help_msg: |
   """
   welcome to @gmanka's anarchy bot
   
   /h | /help - get this command
-  /becomeadmin {title} - makes you an admin with selected title
-
-  admin commands:
-  /setlogs - set this chat as logs chat
+  /ba | /becomeadmin {title} - makes you an admin with selected title
 
   source code - github.com/gmankab/anarchy_bot
   """
+owner_commands_msg: |
+  """
+  bot owner commands:
+
+  /setlogs - set this chat as logs chat
+  """
 admin_panel_button:
   🥔 admin panel
 admin_panel_msg:
   welcome to admin panel
 list_bot_admins_button:
   🥔 admins
 list_bot_users_button:
```

### Comparing `anarchy_bot-23.0.4/pyproject.toml` & `anarchy_bot-23.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [ "gmanka_yml==23.0.*", "pyrogram==2.0.*", "tgcrypto==1.2.*", "uvloop==0.17.*", "rich==13.4.*",]
 name = "anarchy_bot"
-version = "23.0.4"
+version = "23.0.5"
 description = "telegram bot that can add users to minecraft whitelist"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `anarchy_bot-23.0.4/readme.md` & `anarchy_bot-23.0.5/readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 ```bash
 pip install -U anarchy_bot
 ```
 
 ## run
 
 ```bash
-pythom -m anarchy_bot
+python -m anarchy_bot
 ```
 
 ## translate to your language
 
 - fork repo
-- go to [anarchy_bot/lang](https://github.com/gmankab/saltomaru_connect_tg/tree/main/saltomaru_connect_tg/lang)
+- go to [anarchy_bot/lang](https://github.com/gmankab/anarchy_bot/tree/main/anarchy_bot/lang)
 - duplicate `en.yml` file
 - rename it to something like `ru.yml`
 - edit file
 - make pull request
 - bot automatically decects language set in user's telegram client, and will search the dir for file with translation
```

### Comparing `anarchy_bot-23.0.4/PKG-INFO` & `anarchy_bot-23.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anarchy_bot
-Version: 23.0.4
+Version: 23.0.5
 Summary: telegram bot that can add users to minecraft whitelist
 Project-URL: Documentation, https://t.me/gmanka
 Project-URL: Bug Tracker, https://t.me/gmanka
 Project-URL: Homepage, https://t.me/gmanka
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -25,20 +25,20 @@
 ```bash
 pip install -U anarchy_bot
 ```
 
 ## run
 
 ```bash
-pythom -m anarchy_bot
+python -m anarchy_bot
 ```
 
 ## translate to your language
 
 - fork repo
-- go to [anarchy_bot/lang](https://github.com/gmankab/saltomaru_connect_tg/tree/main/saltomaru_connect_tg/lang)
+- go to [anarchy_bot/lang](https://github.com/gmankab/anarchy_bot/tree/main/anarchy_bot/lang)
 - duplicate `en.yml` file
 - rename it to something like `ru.yml`
 - edit file
 - make pull request
 - bot automatically decects language set in user's telegram client, and will search the dir for file with translation
```

