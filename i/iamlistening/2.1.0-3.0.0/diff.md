# Comparing `tmp/iamlistening-2.1.0.tar.gz` & `tmp/iamlistening-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-2.1.0.tar", max compression
+gzip compressed data, was "iamlistening-3.0.0.tar", max compression
```

## Comparing `iamlistening-2.1.0.tar` & `iamlistening-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-24 10:18:49.213510 iamlistening-2.1.0/LICENSE
--rw-r--r--   0        0        0     2910 2023-07-24 10:18:49.213510 iamlistening-2.1.0/README.md
--rw-r--r--   0        0        0      122 2023-07-24 10:18:51.057615 iamlistening-2.1.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/config.py
--rw-r--r--   0        0        0     2669 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4780 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0      540 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/discord.py
--rw-r--r--   0        0        0     1239 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/matrix.py
--rw-r--r--   0        0        0      402 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/rocket_chat.py
--rw-r--r--   0        0        0      591 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/telegram.py
--rw-r--r--   0        0        0     3164 2023-07-24 10:18:51.045614 iamlistening-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 iamlistening-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 20:08:59.461929 iamlistening-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2746 2023-07-24 20:08:59.461929 iamlistening-3.0.0/README.md
+-rw-r--r--   0        0        0      122 2023-07-24 20:09:01.661970 iamlistening-3.0.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/config.py
+-rw-r--r--   0        0        0     2722 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1660 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0      761 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/platform/discord.py
+-rw-r--r--   0        0        0     1489 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/platform/matrix.py
+-rw-r--r--   0        0        0      609 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/platform/rocket_chat.py
+-rw-r--r--   0        0        0      808 2023-07-24 20:08:59.461929 iamlistening-3.0.0/iamlistening/platform/telegram.py
+-rw-r--r--   0        0        0     3188 2023-07-24 20:09:01.653970 iamlistening-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 iamlistening-3.0.0/PKG-INFO
```

### Comparing `iamlistening-2.1.0/LICENSE` & `iamlistening-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-2.1.0/README.md` & `iamlistening-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,17 @@
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
       from iamlistening import Listener
-        listener = Listener()
-        task = asyncio.create_task(listener.run_forever())
-        while True:
-          msg = await listener.get_latest_message()
+      listener = Listener()
+      await listener.start()
+      while True:
+          msg = await listener.handler.get_latest_message()
           if msg:
-            print(f"Frasier👂: {msg}"
-        await task
+            logger.info(f"Frasier👂: {msg}")
+
 </code>
 </pre>
 
-<h5>Example</h5>
-
-https://github.com/mraniki/iamlistening/blob/dcc5dad8887300e34d66d1e36635479ad3b54685/examples/example.py#L1
```

#### html2text {}

```diff
@@ -21,17 +21,14 @@
 [https://codebeat.co/badges/4085334e-4590-41f6-a70c-
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
       from iamlistening import Listener
-        listener = Listener()
-        task = asyncio.create_task(listener.run_forever())
-        while True:
-          msg = await listener.get_latest_message()
+      listener = Listener()
+      await listener.start()
+      while True:
+          msg = await listener.handler.get_latest_message()
           if msg:
-            print(f"Frasierð: {msg}"
-        await task
-** Example **
-https://github.com/mraniki/iamlistening/blob/
-dcc5dad8887300e34d66d1e36635479ad3b54685/examples/example.py#L1
+            logger.info(f"Frasierð: {msg}")
+
```

### Comparing `iamlistening-2.1.0/iamlistening/config.py` & `iamlistening-3.0.0/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-2.1.0/iamlistening/default_settings.toml` & `iamlistening-3.0.0/iamlistening/default_settings.toml`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 [testingmatrix]
 VALUE = "On Testing Matrix"
 iamlistening_enabled = true
 bot_token = "1234556"
 bot_channel_id = "1234556"
 telethon_api_id = ""
 telethon_api_hash = ""
-matrix_hostname = "123456789"
+matrix_hostname = "https://matrix.org"
 matrix_user = "123456789"
 matrix_pass = "123456789"
 rocket_chat_server = ""
 rocket_chat_user_id = ""
 rocket_chat_auth_token = ""
 
 [testingrocketchat]
@@ -112,10 +112,10 @@
 bot_token = "1234556"
 bot_channel_id = "1234556"
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
 matrix_user = ""
 matrix_pass = ""
-rocket_chat_server = ""
-rocket_chat_user_id = ""
-rocket_chat_auth_token = ""
+rocket_chat_server = "https://demo.rocket.chat"
+rocket_chat_user_id = "1234567890"
+rocket_chat_auth_token = "1234567890"
```

### Comparing `iamlistening-2.1.0/iamlistening/platform/discord.py` & `iamlistening-3.0.0/iamlistening/platform/discord.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """
 Discord  🟣
 """
-# import discord
+import asyncio
 
-# from iamlistening.config import settings
+import discord
+from loguru import logger
 
+from iamlistening.config import settings
+from iamlistening.main import ChatManager
 
-# async def start_discord(listener):
-#     """Start the Discord handler."""
 
-#     intents = discord.Intents.default()
-#     intents.message_content = True
-#     bot = discord.Bot(intents=intents)
+class DiscordHandler(ChatManager):
 
-#     @bot.event
-#     async def on_ready():
-#         await listener.post_init()
+    def __init__(self):
+        super().__init__()
 
-#     @bot.event
-#     async def on_message(message: discord.Message):
-#         await listener.handle_message(message.content)
+    async def start(self):
+        """Start the Discord handler."""
+        logger.debug("Discord setup")
+        intents = discord.Intents.default()
+        intents.message_content = True
+        bot = discord.Bot(intents=intents)
 
-#         await bot.start(settings.bot_token)
+        @bot.event
+        async def on_ready():
+            logger.info("listener is online")
+
+        @bot.event
+        async def on_message(message: discord.Message):
+            await self.handle_message(message.content)
+    
+        await bot.start(settings.bot_token)
```

### Comparing `iamlistening-2.1.0/iamlistening/platform/matrix.py` & `iamlistening-3.0.0/iamlistening/platform/matrix.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-# """
-# Matrix ⚫ 
-# """
-# import simplematrixbotlib as botlib
-
-# from iamlistening.config import settings
-
-
-# async def start_matrix(listener):
-#     """Start the Matrix handler."""
-
-#     config = botlib.Config()
-#     config.emoji_verify = True
-#     config.ignore_unverified_devices = True
-#     config.store_path = './config/matrix/'
-#     creds = botlib.Creds(
-#                 settings.matrix_hostname,
-#                 settings.matrix_user,
-#                 settings.matrix_pass
-#                 )
-#     bot = botlib.Bot(creds, config)
-
-#     @bot.listener.on_startup
-#     async def room_joined(room):
-#         await listener.post_init()
-
-#     @bot.listener.on_message_event
-#     async def on_matrix_message(room, message):
-#         await listener.handle_message(message.body)
-#     await bot.api.login()
-#     bot.api.async_client.callbacks = botlib.Callbacks(
-#         bot.api.async_client, bot
-#         )
-#     await bot.api.async_client.callbacks.setup_callbacks()
-#     for action in bot.listener._startup_registry:
-#         for room_id in bot.api.async_client.rooms:
-#             await action(room_id)
-#     await bot.api.async_client.sync_forever(
-#         timeout=3000,
-#         full_state=True
-#         )
+"""
+Matrix ⚫ 
+"""
+import asyncio
+
+import simplematrixbotlib as botlib
+from loguru import logger
+
+from iamlistening.config import settings
+from iamlistening.main import ChatManager
+
+
+class MatrixHandler(ChatManager):
+
+    def __init__(self):
+        super().__init__()
+
+    async def start(self):
+        """Start the Matrix handler."""
+        logger.debug("Matrix setup")
+        config = botlib.Config()
+        config.emoji_verify = True
+        config.ignore_unverified_devices = True
+        config.store_path = './config/matrix/'
+        creds = botlib.Creds(
+                    settings.matrix_hostname,
+                    settings.matrix_user,
+                    settings.matrix_pass
+                    )
+        bot = botlib.Bot(creds, config)
+ 
+        @bot.listener.on_startup
+        async def room_joined(room):
+            logger.info("listener is online")
+
+        @bot.listener.on_message_event
+        async def on_matrix_message(room, message):
+            await self.handle_message(message.body)
+        await bot.api.login()
+        bot.api.async_client.callbacks = botlib.Callbacks(
+            bot.api.async_client, bot
+            )
+        await bot.api.async_client.callbacks.setup_callbacks()
+        for action in bot.listener._startup_registry:
+            for room_id in bot.api.async_client.rooms:
+                await action(room_id)
+        await bot.api.async_client.sync_forever(
+            timeout=3000,
+            full_state=True
+            )
```

### Comparing `iamlistening-2.1.0/pyproject.toml` & `iamlistening-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "2.1.0"
+version = "3.0.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
@@ -59,15 +59,15 @@
 ]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
-
+pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=6,<8"
 sphinx_bootstrap_theme = "^0.8.1"
```

### Comparing `iamlistening-2.1.0/PKG-INFO` & `iamlistening-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 2.1.0
+Version: 3.0.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,21 +51,18 @@
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
       from iamlistening import Listener
-        listener = Listener()
-        task = asyncio.create_task(listener.run_forever())
-        while True:
-          msg = await listener.get_latest_message()
+      listener = Listener()
+      await listener.start()
+      while True:
+          msg = await listener.handler.get_latest_message()
           if msg:
-            print(f"Frasier👂: {msg}"
-        await task
+            logger.info(f"Frasier👂: {msg}")
+
 </code>
 </pre>
 
-<h5>Example</h5>
-
-https://github.com/mraniki/iamlistening/blob/dcc5dad8887300e34d66d1e36635479ad3b54685/examples/example.py#L1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 2.1.0 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.0.0 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord
@@ -35,17 +35,14 @@
 [https://codebeat.co/badges/4085334e-4590-41f6-a70c-
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
       from iamlistening import Listener
-        listener = Listener()
-        task = asyncio.create_task(listener.run_forever())
-        while True:
-          msg = await listener.get_latest_message()
+      listener = Listener()
+      await listener.start()
+      while True:
+          msg = await listener.handler.get_latest_message()
           if msg:
-            print(f"Frasierð: {msg}"
-        await task
-** Example **
-https://github.com/mraniki/iamlistening/blob/
-dcc5dad8887300e34d66d1e36635479ad3b54685/examples/example.py#L1
+            logger.info(f"Frasierð: {msg}")
+
```

