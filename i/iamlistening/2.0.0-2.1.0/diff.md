# Comparing `tmp/iamlistening-2.0.0.tar.gz` & `tmp/iamlistening-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-2.0.0.tar", max compression
+gzip compressed data, was "iamlistening-2.1.0.tar", max compression
```

## Comparing `iamlistening-2.0.0.tar` & `iamlistening-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-23 19:35:03.439154 iamlistening-2.0.0/LICENSE
--rw-r--r--   0        0        0     2910 2023-07-23 19:35:03.439154 iamlistening-2.0.0/README.md
--rw-r--r--   0        0        0      122 2023-07-23 19:35:07.095184 iamlistening-2.0.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/config.py
--rw-r--r--   0        0        0     2669 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4734 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0      540 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/platform/discord.py
--rw-r--r--   0        0        0     1239 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/platform/matrix.py
--rw-r--r--   0        0        0      402 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/platform/rocket_chat.py
--rw-r--r--   0        0        0      591 2023-07-23 19:35:03.439154 iamlistening-2.0.0/iamlistening/platform/telegram.py
--rw-r--r--   0        0        0     3146 2023-07-23 19:35:07.087184 iamlistening-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 iamlistening-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 10:18:49.213510 iamlistening-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2910 2023-07-24 10:18:49.213510 iamlistening-2.1.0/README.md
+-rw-r--r--   0        0        0      122 2023-07-24 10:18:51.057615 iamlistening-2.1.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/config.py
+-rw-r--r--   0        0        0     2669 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4780 2023-07-24 10:18:49.213510 iamlistening-2.1.0/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/discord.py
+-rw-r--r--   0        0        0     1239 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/matrix.py
+-rw-r--r--   0        0        0      402 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/rocket_chat.py
+-rw-r--r--   0        0        0      591 2023-07-24 10:18:49.217510 iamlistening-2.1.0/iamlistening/platform/telegram.py
+-rw-r--r--   0        0        0     3164 2023-07-24 10:18:51.045614 iamlistening-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 iamlistening-2.1.0/PKG-INFO
```

### Comparing `iamlistening-2.0.0/LICENSE` & `iamlistening-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/README.md` & `iamlistening-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/iamlistening/config.py` & `iamlistening-2.1.0/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/iamlistening/default_settings.toml` & `iamlistening-2.1.0/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/iamlistening/main.py` & `iamlistening-2.1.0/iamlistening/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
  IAmListening Main
 """
 
 import asyncio
-import logging
 import threading
 
 import discord
 import simplematrixbotlib as botlib
+
+# import logging
+from loguru import logger
 from telethon import TelegramClient, events
 
 from iamlistening import __version__
 
 from .config import settings
 
 # from .platform.discord import start_discord
 # from .platform import discord, matrix, rocket_chat, telegram
 
 
 class Listener:
     """ 👂 Listener class """
 
     def __init__(self):
-        self.logger = logging.getLogger("Listener")
+        self.logger = logger
+        # logging.getLogger("Listener")
         self.latest_message = None
         self.loop = asyncio.get_event_loop()
         self.lock = threading.Lock()
         self.stopped = False
 
     async def get_info_listener(self):
         return (f"ℹ️ IAmListening v{__version__}\n")
```

### Comparing `iamlistening-2.0.0/iamlistening/platform/discord.py` & `iamlistening-2.1.0/iamlistening/platform/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/iamlistening/platform/matrix.py` & `iamlistening-2.1.0/iamlistening/platform/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/iamlistening/platform/telegram.py` & `iamlistening-2.1.0/iamlistening/platform/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-2.0.0/pyproject.toml` & `iamlistening-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "2.0.0"
+version = "2.1.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
@@ -23,14 +23,15 @@
 "Changelog" =  "https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/iamlistening/discussions"
 "Issues" =  "https://github.com/mraniki/iamlistening/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
+loguru = "^0.7.0"
 telethon= "^1.28.5"
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
 rocketchat-API= "^1.30.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `iamlistening-2.0.0/PKG-INFO` & `iamlistening-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 2.0.0
+Version: 2.1.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: py-cord (>=2.4.1,<3.0.0)
 Requires-Dist: rocketchat-API (>=1.30.0,<2.0.0)
 Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0)
 Requires-Dist: telethon (>=1.28.5,<2.0.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 2.0.0 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 2.1.0 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-Dist:
-rocketchat-API (>=1.30.0,<2.0.0) Requires-Dist: simplematrixbotlib
-(>=2.9.0,<3.0.0) Requires-Dist: telethon (>=1.28.5,<2.0.0) Project-URL:
-Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
-Project-URL: Issues, https://github.com/mraniki/iamlistening/issues Project-
-URL: Support, https://github.com/mraniki/iamlistening/discussions Description-
-Content-Type: text/markdown
+(>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord
+(>=2.4.1,<3.0.0) Requires-Dist: rocketchat-API (>=1.30.0,<2.0.0) Requires-Dist:
+simplematrixbotlib (>=2.9.0,<3.0.0) Requires-Dist: telethon (>=1.28.5,<2.0.0)
+Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/
+CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/iamlistening/
+issues Project-URL: Support, https://github.com/mraniki/iamlistening/
+discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [Docker_Pulls]
 [https://img.shields.io/badge/tips-000000?style=for-the-             [Logo]
 badge&logo=buymeacoffee&logoColor=white] [https://
```

