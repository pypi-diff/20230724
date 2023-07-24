# Comparing `tmp/Wavelink-2.6.0.tar.gz` & `tmp/wavelink-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.6.0.tar", last modified: Wed Jul 12 04:05:29 2023, max compression
+gzip compressed data, was "wavelink-2.6.1.tar", last modified: Mon Jul 24 19:51:24 2023, max compression
```

## Comparing `Wavelink-2.6.0.tar` & `wavelink-2.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.692616 Wavelink-2.6.0/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.6.0/LICENSE
--rw-rw-rw-   0        0        0     5812 2023-07-12 04:05:29.692616 Wavelink-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5011 2023-06-23 14:10:49.000000 Wavelink-2.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.676058 Wavelink-2.6.0/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5812 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-07-12 04:05:10.000000 Wavelink-2.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 04:05:29.693117 Wavelink-2.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.686597 Wavelink-2.6.0/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-07-12 04:05:10.000000 Wavelink-2.6.0/wavelink/__init__.py
--rw-rw-rw-   0        0        0      992 2023-06-24 08:28:29.000000 Wavelink-2.6.0/wavelink/__main__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/backoff.py
--rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.6.0/wavelink/enums.py
--rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.6.0/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.667128 Wavelink-2.6.0/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.688102 Wavelink-2.6.0/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    16863 2023-07-12 03:52:50.000000 Wavelink-2.6.0/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0     5115 2023-06-27 13:30:40.000000 Wavelink-2.6.0/wavelink/ext/spotify/utils.py
--rw-rw-rw-   0        0        0    20509 2023-06-21 14:04:01.000000 Wavelink-2.6.0/wavelink/filters.py
--rw-rw-rw-   0        0        0    19314 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.6.0/wavelink/payloads.py
--rw-rw-rw-   0        0        0    30563 2023-06-29 12:10:11.000000 Wavelink-2.6.0/wavelink/player.py
--rw-rw-rw-   0        0        0    20409 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/queue.py
--rw-rw-rw-   0        0        0    11769 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.691615 Wavelink-2.6.0/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/track.py
--rw-rw-rw-   0        0        0    11011 2023-07-12 04:02:26.000000 Wavelink-2.6.0/wavelink/websocket.py
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.465679 wavelink-2.6.1/
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     1088 2023-07-24 18:01:33.000000 wavelink-2.6.1/LICENSE
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     5645 2023-07-24 19:51:24.465679 wavelink-2.6.1/PKG-INFO
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     4864 2023-07-24 18:01:33.000000 wavelink-2.6.1/README.rst
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      974 2023-07-24 19:50:50.000000 wavelink-2.6.1/pyproject.toml
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)       47 2023-07-24 18:01:33.000000 wavelink-2.6.1/requirements.txt
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)       38 2023-07-24 19:51:24.465679 wavelink-2.6.1/setup.cfg
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.461679 wavelink-2.6.1/wavelink/
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     1458 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/__init__.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      950 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/__main__.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     2630 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/backoff.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     3536 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/enums.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     2935 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/exceptions.py
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.449678 wavelink-2.6.1/wavelink/ext/
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.465679 wavelink-2.6.1/wavelink/ext/spotify/
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    16352 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/ext/spotify/__init__.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     4944 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/ext/spotify/utils.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    19878 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/filters.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    18740 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/node.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     3366 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/payloads.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    29860 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/player.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    19722 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/queue.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    11378 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/tracks.py
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.465679 wavelink-2.6.1/wavelink/types/
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      825 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/types/events.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      602 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/types/request.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      408 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/types/state.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      325 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/types/track.py
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)    10730 2023-07-24 18:01:33.000000 wavelink-2.6.1/wavelink/websocket.py
+drwxrwxr-x   0 chillymosh  (1000) chillymosh  (1008)        0 2023-07-24 19:51:24.465679 wavelink-2.6.1/wavelink.egg-info/
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)     5645 2023-07-24 19:51:24.000000 wavelink-2.6.1/wavelink.egg-info/PKG-INFO
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)      610 2023-07-24 19:51:24.000000 wavelink-2.6.1/wavelink.egg-info/SOURCES.txt
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)        1 2023-07-24 19:51:24.000000 wavelink-2.6.1/wavelink.egg-info/dependency_links.txt
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)       48 2023-07-24 19:51:24.000000 wavelink-2.6.1/wavelink.egg-info/requires.txt
+-rw-rw-r--   0 chillymosh  (1000) chillymosh  (1008)        9 2023-07-24 19:51:24.000000 wavelink-2.6.1/wavelink.egg-info/top_level.txt
```

### Comparing `Wavelink-2.6.0/LICENSE` & `wavelink-2.6.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019-Current PythonistaGuild, EvieePy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2019-Current PythonistaGuild, EvieePy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `Wavelink-2.6.0/PKG-INFO` & `wavelink-2.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: Wavelink
-Version: 2.6.0
-Summary: A robust and powerful Lavalink wrapper for discord.py
-Author-email: EvieePy <evieepy@gmail.com>
-Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
-
-
-.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
-    :target: https://www.python.org
-
-
-.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
-    :target: LICENSE
-
-
-.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
-   :target: https://discord.gg/RAKc3HF
-
-
-.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
-    :target: https://pypi.org/project/Wavelink
-    :alt: PyPI - Downloads
-
-
-.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
-    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
-    :alt: Maintenance
-
-
-
-Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
-Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-
-
-**Features:**
-
-- Fully Asynchronous
-- Auto-Play and Looping (With the inbuilt Queue system)
-- Spotify Support
-- Node Balancing and Fail-over
-- Supports Lavalink 3.7+
-
-
-Documentation
----------------------------
-`Official Documentation <https://wavelink.dev/>`_
-
-Support
----------------------------
-For support using WaveLink, please join the official `support server
-<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
-
-.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
-    :target: https://discord.gg/RAKc3HF
-
-
-Installation
----------------------------
-The following commands are currently the valid ways of installing WaveLink.
-
-**WaveLink 2 requires Python 3.10+**
-
-**Windows**
-
-.. code:: sh
-
-    py -3.10 -m pip install -U Wavelink
-
-**Linux**
-
-.. code:: sh
-
-    python3.10 -m pip install -U Wavelink
-
-Getting Started
-----------------------------
-
-**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
-
-.. code:: py
-
-    import discord
-    import wavelink
-    from discord.ext import commands
-
-
-    class Bot(commands.Bot):
-
-        def __init__(self) -> None:
-            intents = discord.Intents.default()
-            intents.message_content = True
-
-            super().__init__(intents=intents, command_prefix='?')
-
-        async def on_ready(self) -> None:
-            print(f'Logged in {self.user} | {self.user.id}')
-
-        async def setup_hook(self) -> None:
-            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-            # and pass it to NodePool.connect with the client/bot.
-            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-            await wavelink.NodePool.connect(client=self, nodes=[node])
-
-
-    bot = Bot()
-
-
-    @bot.command()
-    async def play(ctx: commands.Context, *, search: str) -> None:
-        """Simple play command."""
-
-        if not ctx.voice_client:
-            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
-        else:
-            vc: wavelink.Player = ctx.voice_client
-
-        tracks = await wavelink.YouTubeTrack.search(search)
-        if not tracks:
-            await ctx.send(f'No tracks found with query: `{search}`')
-            return
-
-        track = tracks[0]
-        await vc.play(track)
-
-
-    @bot.command()
-    async def disconnect(ctx: commands.Context) -> None:
-        """Simple disconnect command.
-
-        This command assumes there is a currently connected Player.
-        """
-        vc: wavelink.Player = ctx.voice_client
-        await vc.disconnect()
-
-
-Lavalink Installation
----------------------
-
-Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
-
-- Create a folder for storing Lavalink.jar and related files/folders.
-- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
-- Change your password in the ``application.yml`` and store it in a config for your bot.
-- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
-- Save and exit.
-- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
-- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
-- Run: ``java -jar Lavalink.jar``
-
-If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
+Metadata-Version: 2.1
+Name: wavelink
+Version: 2.6.1
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
+Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
+
+
+.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
+    :target: https://www.python.org
+
+
+.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
+    :target: LICENSE
+
+
+.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
+   :target: https://discord.gg/RAKc3HF
+
+
+.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
+    :target: https://pypi.org/project/Wavelink
+    :alt: PyPI - Downloads
+
+
+.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
+    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
+    :alt: Maintenance
+
+
+
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
+Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
+
+
+**Features:**
+
+- Fully Asynchronous
+- Auto-Play and Looping (With the inbuilt Queue system)
+- Spotify Support
+- Node Balancing and Fail-over
+- Supports Lavalink 3.7+
+
+
+Documentation
+---------------------------
+`Official Documentation <https://wavelink.dev/>`_
+
+Support
+---------------------------
+For support using WaveLink, please join the official `support server
+<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
+
+.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
+    :target: https://discord.gg/RAKc3HF
+
+
+Installation
+---------------------------
+The following commands are currently the valid ways of installing WaveLink.
+
+**WaveLink 2 requires Python 3.10+**
+
+**Windows**
+
+.. code:: sh
+
+    py -3.10 -m pip install -U Wavelink
+
+**Linux**
+
+.. code:: sh
+
+    python3.10 -m pip install -U Wavelink
+
+Getting Started
+----------------------------
+
+**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
+
+.. code:: py
+
+    import discord
+    import wavelink
+    from discord.ext import commands
+
+
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
+
+
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
+        await vc.play(track)
+
+
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
+        """Simple disconnect command.
+
+        This command assumes there is a currently connected Player.
+        """
+        vc: wavelink.Player = ctx.voice_client
+        await vc.disconnect()
+
+
+Lavalink Installation
+---------------------
+
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
+
+- Create a folder for storing Lavalink.jar and related files/folders.
+- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
+- Change your password in the ``application.yml`` and store it in a config for your bot.
+- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
+- Save and exit.
+- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
+- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
+- Run: ``java -jar Lavalink.jar``
+
+If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.6.0/README.rst` & `wavelink-2.6.1/README.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
-
-
-.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
-    :target: https://www.python.org
-
-
-.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
-    :target: LICENSE
-
-
-.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
-   :target: https://discord.gg/RAKc3HF
-
-
-.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
-    :target: https://pypi.org/project/Wavelink
-    :alt: PyPI - Downloads
-
-
-.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
-    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
-    :alt: Maintenance
-
-
-
-Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
-Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-
-
-**Features:**
-
-- Fully Asynchronous
-- Auto-Play and Looping (With the inbuilt Queue system)
-- Spotify Support
-- Node Balancing and Fail-over
-- Supports Lavalink 3.7+
-
-
-Documentation
----------------------------
-`Official Documentation <https://wavelink.dev/>`_
-
-Support
----------------------------
-For support using WaveLink, please join the official `support server
-<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
-
-.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
-    :target: https://discord.gg/RAKc3HF
-
-
-Installation
----------------------------
-The following commands are currently the valid ways of installing WaveLink.
-
-**WaveLink 2 requires Python 3.10+**
-
-**Windows**
-
-.. code:: sh
-
-    py -3.10 -m pip install -U Wavelink
-
-**Linux**
-
-.. code:: sh
-
-    python3.10 -m pip install -U Wavelink
-
-Getting Started
-----------------------------
-
-**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
-
-.. code:: py
-
-    import discord
-    import wavelink
-    from discord.ext import commands
-
-
-    class Bot(commands.Bot):
-
-        def __init__(self) -> None:
-            intents = discord.Intents.default()
-            intents.message_content = True
-
-            super().__init__(intents=intents, command_prefix='?')
-
-        async def on_ready(self) -> None:
-            print(f'Logged in {self.user} | {self.user.id}')
-
-        async def setup_hook(self) -> None:
-            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-            # and pass it to NodePool.connect with the client/bot.
-            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-            await wavelink.NodePool.connect(client=self, nodes=[node])
-
-
-    bot = Bot()
-
-
-    @bot.command()
-    async def play(ctx: commands.Context, *, search: str) -> None:
-        """Simple play command."""
-
-        if not ctx.voice_client:
-            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
-        else:
-            vc: wavelink.Player = ctx.voice_client
-
-        tracks = await wavelink.YouTubeTrack.search(search)
-        if not tracks:
-            await ctx.send(f'No tracks found with query: `{search}`')
-            return
-
-        track = tracks[0]
-        await vc.play(track)
-
-
-    @bot.command()
-    async def disconnect(ctx: commands.Context) -> None:
-        """Simple disconnect command.
-
-        This command assumes there is a currently connected Player.
-        """
-        vc: wavelink.Player = ctx.voice_client
-        await vc.disconnect()
-
-
-Lavalink Installation
----------------------
-
-Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
-
-- Create a folder for storing Lavalink.jar and related files/folders.
-- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
-- Change your password in the ``application.yml`` and store it in a config for your bot.
-- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
-- Save and exit.
-- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
-- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
-- Run: ``java -jar Lavalink.jar``
-
-If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
+.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
+
+
+.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
+    :target: https://www.python.org
+
+
+.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
+    :target: LICENSE
+
+
+.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
+   :target: https://discord.gg/RAKc3HF
+
+
+.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
+    :target: https://pypi.org/project/Wavelink
+    :alt: PyPI - Downloads
+
+
+.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
+    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
+    :alt: Maintenance
+
+
+
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
+Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
+
+
+**Features:**
+
+- Fully Asynchronous
+- Auto-Play and Looping (With the inbuilt Queue system)
+- Spotify Support
+- Node Balancing and Fail-over
+- Supports Lavalink 3.7+
+
+
+Documentation
+---------------------------
+`Official Documentation <https://wavelink.dev/>`_
+
+Support
+---------------------------
+For support using WaveLink, please join the official `support server
+<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
+
+.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
+    :target: https://discord.gg/RAKc3HF
+
+
+Installation
+---------------------------
+The following commands are currently the valid ways of installing WaveLink.
+
+**WaveLink 2 requires Python 3.10+**
+
+**Windows**
+
+.. code:: sh
+
+    py -3.10 -m pip install -U Wavelink
+
+**Linux**
+
+.. code:: sh
+
+    python3.10 -m pip install -U Wavelink
+
+Getting Started
+----------------------------
+
+**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
+
+.. code:: py
+
+    import discord
+    import wavelink
+    from discord.ext import commands
+
+
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
+
+
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
+        await vc.play(track)
+
+
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
+        """Simple disconnect command.
+
+        This command assumes there is a currently connected Player.
+        """
+        vc: wavelink.Player = ctx.voice_client
+        await vc.disconnect()
+
+
+Lavalink Installation
+---------------------
+
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
+
+- Create a folder for storing Lavalink.jar and related files/folders.
+- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
+- Change your password in the ``application.yml`` and store it in a config for your bot.
+- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
+- Save and exit.
+- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
+- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
+- Run: ``java -jar Lavalink.jar``
+
+If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.6.0/Wavelink.egg-info/PKG-INFO` & `wavelink-2.6.1/wavelink.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: Wavelink
-Version: 2.6.0
-Summary: A robust and powerful Lavalink wrapper for discord.py
-Author-email: EvieePy <evieepy@gmail.com>
-Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
-
-
-.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
-    :target: https://www.python.org
-
-
-.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
-    :target: LICENSE
-
-
-.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
-   :target: https://discord.gg/RAKc3HF
-
-
-.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
-    :target: https://pypi.org/project/Wavelink
-    :alt: PyPI - Downloads
-
-
-.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
-    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
-    :alt: Maintenance
-
-
-
-Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
-Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-
-
-**Features:**
-
-- Fully Asynchronous
-- Auto-Play and Looping (With the inbuilt Queue system)
-- Spotify Support
-- Node Balancing and Fail-over
-- Supports Lavalink 3.7+
-
-
-Documentation
----------------------------
-`Official Documentation <https://wavelink.dev/>`_
-
-Support
----------------------------
-For support using WaveLink, please join the official `support server
-<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
-
-.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
-    :target: https://discord.gg/RAKc3HF
-
-
-Installation
----------------------------
-The following commands are currently the valid ways of installing WaveLink.
-
-**WaveLink 2 requires Python 3.10+**
-
-**Windows**
-
-.. code:: sh
-
-    py -3.10 -m pip install -U Wavelink
-
-**Linux**
-
-.. code:: sh
-
-    python3.10 -m pip install -U Wavelink
-
-Getting Started
-----------------------------
-
-**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
-
-.. code:: py
-
-    import discord
-    import wavelink
-    from discord.ext import commands
-
-
-    class Bot(commands.Bot):
-
-        def __init__(self) -> None:
-            intents = discord.Intents.default()
-            intents.message_content = True
-
-            super().__init__(intents=intents, command_prefix='?')
-
-        async def on_ready(self) -> None:
-            print(f'Logged in {self.user} | {self.user.id}')
-
-        async def setup_hook(self) -> None:
-            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-            # and pass it to NodePool.connect with the client/bot.
-            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-            await wavelink.NodePool.connect(client=self, nodes=[node])
-
-
-    bot = Bot()
-
-
-    @bot.command()
-    async def play(ctx: commands.Context, *, search: str) -> None:
-        """Simple play command."""
-
-        if not ctx.voice_client:
-            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
-        else:
-            vc: wavelink.Player = ctx.voice_client
-
-        tracks = await wavelink.YouTubeTrack.search(search)
-        if not tracks:
-            await ctx.send(f'No tracks found with query: `{search}`')
-            return
-
-        track = tracks[0]
-        await vc.play(track)
-
-
-    @bot.command()
-    async def disconnect(ctx: commands.Context) -> None:
-        """Simple disconnect command.
-
-        This command assumes there is a currently connected Player.
-        """
-        vc: wavelink.Player = ctx.voice_client
-        await vc.disconnect()
-
-
-Lavalink Installation
----------------------
-
-Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
-
-- Create a folder for storing Lavalink.jar and related files/folders.
-- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
-- Change your password in the ``application.yml`` and store it in a config for your bot.
-- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
-- Save and exit.
-- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
-- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
-- Run: ``java -jar Lavalink.jar``
-
-If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
+Metadata-Version: 2.1
+Name: wavelink
+Version: 2.6.1
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
+Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
+
+
+.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
+    :target: https://www.python.org
+
+
+.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
+    :target: LICENSE
+
+
+.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
+   :target: https://discord.gg/RAKc3HF
+
+
+.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
+    :target: https://pypi.org/project/Wavelink
+    :alt: PyPI - Downloads
+
+
+.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
+    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
+    :alt: Maintenance
+
+
+
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
+Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
+
+
+**Features:**
+
+- Fully Asynchronous
+- Auto-Play and Looping (With the inbuilt Queue system)
+- Spotify Support
+- Node Balancing and Fail-over
+- Supports Lavalink 3.7+
+
+
+Documentation
+---------------------------
+`Official Documentation <https://wavelink.dev/>`_
+
+Support
+---------------------------
+For support using WaveLink, please join the official `support server
+<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
+
+.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
+    :target: https://discord.gg/RAKc3HF
+
+
+Installation
+---------------------------
+The following commands are currently the valid ways of installing WaveLink.
+
+**WaveLink 2 requires Python 3.10+**
+
+**Windows**
+
+.. code:: sh
+
+    py -3.10 -m pip install -U Wavelink
+
+**Linux**
+
+.. code:: sh
+
+    python3.10 -m pip install -U Wavelink
+
+Getting Started
+----------------------------
+
+**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
+
+.. code:: py
+
+    import discord
+    import wavelink
+    from discord.ext import commands
+
+
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
+
+
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
+        await vc.play(track)
+
+
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
+        """Simple disconnect command.
+
+        This command assumes there is a currently connected Player.
+        """
+        vc: wavelink.Player = ctx.voice_client
+        await vc.disconnect()
+
+
+Lavalink Installation
+---------------------
+
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
+
+- Create a folder for storing Lavalink.jar and related files/folders.
+- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
+- Change your password in the ``application.yml`` and store it in a config for your bot.
+- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
+- Save and exit.
+- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
+- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
+- Run: ``java -jar Lavalink.jar``
+
+If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.6.0/Wavelink.egg-info/SOURCES.txt` & `wavelink-2.6.1/wavelink.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
-Wavelink.egg-info/PKG-INFO
-Wavelink.egg-info/SOURCES.txt
-Wavelink.egg-info/dependency_links.txt
-Wavelink.egg-info/requires.txt
-Wavelink.egg-info/top_level.txt
 wavelink/__init__.py
 wavelink/__main__.py
 wavelink/backoff.py
 wavelink/enums.py
 wavelink/exceptions.py
 wavelink/filters.py
 wavelink/node.py
 wavelink/payloads.py
 wavelink/player.py
 wavelink/queue.py
 wavelink/tracks.py
 wavelink/websocket.py
+wavelink.egg-info/PKG-INFO
+wavelink.egg-info/SOURCES.txt
+wavelink.egg-info/dependency_links.txt
+wavelink.egg-info/requires.txt
+wavelink.egg-info/top_level.txt
 wavelink/ext/spotify/__init__.py
 wavelink/ext/spotify/utils.py
 wavelink/types/events.py
 wavelink/types/request.py
 wavelink/types/state.py
 wavelink/types/track.py
```

### Comparing `Wavelink-2.6.0/wavelink/__init__.py` & `wavelink-2.6.1/wavelink/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-__title__ = "WaveLink"
-__author__ = "PythonistaGuild, EvieePy"
-__license__ = "MIT"
-__copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.6.0"
-
-from .enums import *
-from .exceptions import *
-from .node import *
-from .payloads import *
-from .player import Player as Player
-from .tracks import *
-from .queue import *
-from .filters import *
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+__title__ = "WaveLink"
+__author__ = "PythonistaGuild, EvieePy"
+__license__ = "MIT"
+__copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
+__version__ = "2.6.1"
+
+from .enums import *
+from .exceptions import *
+from .node import *
+from .payloads import *
+from .player import Player as Player
+from .tracks import *
+from .queue import *
+from .filters import *
```

### Comparing `Wavelink-2.6.0/wavelink/__main__.py` & `wavelink-2.6.1/wavelink/__main__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import argparse
-import platform
-import subprocess
-import sys
-
-import aiohttp
-import discord
-
-import wavelink
-
-
-parser = argparse.ArgumentParser(prog='wavelink')
-parser.add_argument('--version', action='store_true', help='Get version and debug information for wavelink.')
-
-
-args = parser.parse_args()
-
-
-def get_debug_info() -> None:
-    python_info = '\n'.join(sys.version.split('\n'))
-    java_version = subprocess.check_output(['java', '-version'], stderr=subprocess.STDOUT)
-    java_version = f'\n{" " * 8}- '.join(v for v in java_version.decode().split('\r\n') if v)
-
-    info: str = f"""
-    Python:
-        - {python_info}
-    System:
-        - {platform.platform()}
-    Java:
-        - {java_version or "Version Not Found"}
-    Libraries:
-        - wavelink   : v{wavelink.__version__}
-        - discord.py : v{discord.__version__}
-        - aiohttp    : v{aiohttp.__version__}
-    """
-
-    print(info)
-
-
-if args.version:
-    get_debug_info()
-
+import argparse
+import platform
+import subprocess
+import sys
+
+import aiohttp
+import discord
+
+import wavelink
+
+
+parser = argparse.ArgumentParser(prog='wavelink')
+parser.add_argument('--version', action='store_true', help='Get version and debug information for wavelink.')
+
+
+args = parser.parse_args()
+
+
+def get_debug_info() -> None:
+    python_info = '\n'.join(sys.version.split('\n'))
+    java_version = subprocess.check_output(['java', '-version'], stderr=subprocess.STDOUT)
+    java_version = f'\n{" " * 8}- '.join(v for v in java_version.decode().split('\r\n') if v)
+
+    info: str = f"""
+    Python:
+        - {python_info}
+    System:
+        - {platform.platform()}
+    Java:
+        - {java_version or "Version Not Found"}
+    Libraries:
+        - wavelink   : v{wavelink.__version__}
+        - discord.py : v{discord.__version__}
+        - aiohttp    : v{aiohttp.__version__}
+    """
+
+    print(info)
+
+
+if args.version:
+    get_debug_info()
+
```

### Comparing `Wavelink-2.6.0/wavelink/backoff.py` & `wavelink-2.6.1/wavelink/backoff.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-"""
-The MIT License (MIT)
-Copyright (c) 2021-Present PythonistaGuild, EvieePy, Rapptz
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-from __future__ import annotations
-
-import random
-from collections.abc import Callable
-
-
-class Backoff:
-    """An implementation of an Exponential Backoff.
-    Parameters
-    ----------
-    base: int
-        The base time to multiply exponentially. Defaults to 1.
-    maximum_time: float
-        The maximum wait time. Defaults to 30.0
-    maximum_tries: Optional[int]
-        The amount of times to backoff before resetting. Defaults to 5. If set to None, backoff will run indefinitely.
-    """
-
-    def __init__(self, *, base: int = 1, maximum_time: float = 30.0, maximum_tries: int | None = 5) -> None:
-        self._base: int = base
-        self._maximum_time: float = maximum_time
-        self._maximum_tries: int | None = maximum_tries
-        self._retries: int = 1
-
-        rand = random.Random()
-        rand.seed()
-
-        self._rand: Callable[[float, float], float] = rand.uniform
-
-        self._last_wait: float = 0
-
-    def calculate(self) -> float:
-        exponent = min((self._retries ** 2), self._maximum_time)
-        wait = self._rand(0, (self._base * 2) * exponent)
-
-        if wait <= self._last_wait:
-            wait = self._last_wait * 2
-
-        self._last_wait = wait
-
-        if wait > self._maximum_time:
-            wait = self._maximum_time
-            self._retries = 0
-            self._last_wait = 0
-
-        if self._maximum_tries and self._retries >= self._maximum_tries:
-            self._retries = 0
-            self._last_wait = 0
-
-        self._retries += 1
-
-        return wait
+"""
+The MIT License (MIT)
+Copyright (c) 2021-Present PythonistaGuild, EvieePy, Rapptz
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+import random
+from collections.abc import Callable
+
+
+class Backoff:
+    """An implementation of an Exponential Backoff.
+    Parameters
+    ----------
+    base: int
+        The base time to multiply exponentially. Defaults to 1.
+    maximum_time: float
+        The maximum wait time. Defaults to 30.0
+    maximum_tries: Optional[int]
+        The amount of times to backoff before resetting. Defaults to 5. If set to None, backoff will run indefinitely.
+    """
+
+    def __init__(self, *, base: int = 1, maximum_time: float = 30.0, maximum_tries: int | None = 5) -> None:
+        self._base: int = base
+        self._maximum_time: float = maximum_time
+        self._maximum_tries: int | None = maximum_tries
+        self._retries: int = 1
+
+        rand = random.Random()
+        rand.seed()
+
+        self._rand: Callable[[float, float], float] = rand.uniform
+
+        self._last_wait: float = 0
+
+    def calculate(self) -> float:
+        exponent = min((self._retries ** 2), self._maximum_time)
+        wait = self._rand(0, (self._base * 2) * exponent)
+
+        if wait <= self._last_wait:
+            wait = self._last_wait * 2
+
+        self._last_wait = wait
+
+        if wait > self._maximum_time:
+            wait = self._maximum_time
+            self._retries = 0
+            self._last_wait = 0
+
+        if self._maximum_tries and self._retries >= self._maximum_tries:
+            self._retries = 0
+            self._last_wait = 0
+
+        self._retries += 1
+
+        return wait
```

### Comparing `Wavelink-2.6.0/wavelink/enums.py` & `wavelink-2.6.1/wavelink/enums.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from discord.enums import Enum
-
-__all__ = ('NodeStatus', 'TrackSource', 'LoadType', 'TrackEventType', 'DiscordVoiceCloseType')
-
-
-class NodeStatus(Enum):
-    """Enum representing the current status of a Node.
-
-    Attributes
-    ----------
-    DISCONNECTED
-        0
-    CONNECTING
-        1
-    CONNECTED
-        2
-    """
-
-    DISCONNECTED = 0
-    CONNECTING = 1
-    CONNECTED = 2
-
-
-class TrackSource(Enum):
-    """Enum representing the Track Source Type.
-
-    Attributes
-    ----------
-    YouTube
-        0
-    YouTubeMusic
-        1
-    SoundCloud
-        2
-    Local
-        3
-    Unknown
-        4
-    """
-
-    YouTube = 0
-    YouTubeMusic = 1
-    SoundCloud = 2
-    Local = 3
-    Unknown = 4
-
-
-class LoadType(Enum):
-    """Enum representing the Tracks Load Type.
-
-    Attributes
-    ----------
-    track_loaded
-        "TRACK_LOADED"
-    playlist_loaded
-        "PLAYLIST_LOADED"
-    search_result
-        "SEARCH_RESULT"
-    no_matches
-        "NO_MATCHES"
-    load_failed
-        "LOAD_FAILED"
-    """
-    track_loaded = "TRACK_LOADED"
-    playlist_loaded = "PLAYLIST_LOADED"
-    search_result = "SEARCH_RESULT"
-    no_matches = "NO_MATCHES"
-    load_failed = "LOAD_FAILED"
-
-
-class TrackEventType(Enum):
-    """Enum representing the TrackEvent types.
-
-    Attributes
-    ----------
-    START
-        "TrackStartEvent"
-    END
-        "TrackEndEvent"
-    """
-
-    START = 'TrackStartEvent'
-    END = 'TrackEndEvent'
-
-
-class DiscordVoiceCloseType(Enum):
-    """Enum representing the various Discord Voice Websocket Close Codes.
-
-    Attributes
-    ----------
-    CLOSE_NORMAL
-        1000
-    UNKNOWN_OPCODE
-        4001
-    FAILED_DECODE_PAYLOAD
-        4002
-    NOT_AUTHENTICATED
-        4003
-    AUTHENTICATION_FAILED
-        4004
-    ALREADY_AUTHENTICATED
-        4005
-    SESSION_INVALID
-        4006
-    SESSION_TIMEOUT
-        4009
-    SERVER_NOT_FOUND
-        4011
-    UNKNOWN_PROTOCOL
-        4012
-    DISCONNECTED
-        4014
-    VOICE_SERVER_CRASHED
-        4015
-    UNKNOWN_ENCRYPTION_MODE
-        4016
-    """
-    CLOSE_NORMAL = 1000  # Not Discord but standard websocket
-    UNKNOWN_OPCODE = 4001
-    FAILED_DECODE_PAYLOAD = 4002
-    NOT_AUTHENTICATED = 4003
-    AUTHENTICATION_FAILED = 4004
-    ALREADY_AUTHENTICATED = 4005
-    SESSION_INVALID = 4006
-    SESSION_TIMEOUT = 4009
-    SERVER_NOT_FOUND = 4011
-    UNKNOWN_PROTOCOL = 4012
-    DISCONNECTED = 4014
-    VOICE_SERVER_CRASHED = 4015
-    UNKNOWN_ENCRYPTION_MODE = 4016
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from discord.enums import Enum
+
+__all__ = ('NodeStatus', 'TrackSource', 'LoadType', 'TrackEventType', 'DiscordVoiceCloseType')
+
+
+class NodeStatus(Enum):
+    """Enum representing the current status of a Node.
+
+    Attributes
+    ----------
+    DISCONNECTED
+        0
+    CONNECTING
+        1
+    CONNECTED
+        2
+    """
+
+    DISCONNECTED = 0
+    CONNECTING = 1
+    CONNECTED = 2
+
+
+class TrackSource(Enum):
+    """Enum representing the Track Source Type.
+
+    Attributes
+    ----------
+    YouTube
+        0
+    YouTubeMusic
+        1
+    SoundCloud
+        2
+    Local
+        3
+    Unknown
+        4
+    """
+
+    YouTube = 0
+    YouTubeMusic = 1
+    SoundCloud = 2
+    Local = 3
+    Unknown = 4
+
+
+class LoadType(Enum):
+    """Enum representing the Tracks Load Type.
+
+    Attributes
+    ----------
+    track_loaded
+        "TRACK_LOADED"
+    playlist_loaded
+        "PLAYLIST_LOADED"
+    search_result
+        "SEARCH_RESULT"
+    no_matches
+        "NO_MATCHES"
+    load_failed
+        "LOAD_FAILED"
+    """
+    track_loaded = "TRACK_LOADED"
+    playlist_loaded = "PLAYLIST_LOADED"
+    search_result = "SEARCH_RESULT"
+    no_matches = "NO_MATCHES"
+    load_failed = "LOAD_FAILED"
+
+
+class TrackEventType(Enum):
+    """Enum representing the TrackEvent types.
+
+    Attributes
+    ----------
+    START
+        "TrackStartEvent"
+    END
+        "TrackEndEvent"
+    """
+
+    START = 'TrackStartEvent'
+    END = 'TrackEndEvent'
+
+
+class DiscordVoiceCloseType(Enum):
+    """Enum representing the various Discord Voice Websocket Close Codes.
+
+    Attributes
+    ----------
+    CLOSE_NORMAL
+        1000
+    UNKNOWN_OPCODE
+        4001
+    FAILED_DECODE_PAYLOAD
+        4002
+    NOT_AUTHENTICATED
+        4003
+    AUTHENTICATION_FAILED
+        4004
+    ALREADY_AUTHENTICATED
+        4005
+    SESSION_INVALID
+        4006
+    SESSION_TIMEOUT
+        4009
+    SERVER_NOT_FOUND
+        4011
+    UNKNOWN_PROTOCOL
+        4012
+    DISCONNECTED
+        4014
+    VOICE_SERVER_CRASHED
+        4015
+    UNKNOWN_ENCRYPTION_MODE
+        4016
+    """
+    CLOSE_NORMAL = 1000  # Not Discord but standard websocket
+    UNKNOWN_OPCODE = 4001
+    FAILED_DECODE_PAYLOAD = 4002
+    NOT_AUTHENTICATED = 4003
+    AUTHENTICATION_FAILED = 4004
+    ALREADY_AUTHENTICATED = 4005
+    SESSION_INVALID = 4006
+    SESSION_TIMEOUT = 4009
+    SERVER_NOT_FOUND = 4011
+    UNKNOWN_PROTOCOL = 4012
+    DISCONNECTED = 4014
+    VOICE_SERVER_CRASHED = 4015
+    UNKNOWN_ENCRYPTION_MODE = 4016
```

### Comparing `Wavelink-2.6.0/wavelink/exceptions.py` & `wavelink-2.6.1/wavelink/exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-from typing import Any
-
-__all__ = (
-    'WavelinkException',
-    'AuthorizationFailed',
-    'InvalidNode',
-    'InvalidLavalinkVersion',
-    'InvalidLavalinkResponse',
-    'NoTracksError',
-    'QueueEmpty',
-    'InvalidChannelStateError',
-    'InvalidChannelPermissions',
-)
-
-
-class WavelinkException(Exception):
-    """Base wavelink exception."""
-
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        super().__init__(*args)
-
-
-class AuthorizationFailed(WavelinkException):
-    """Exception raised when password authorization failed for this Lavalink node."""
-    pass
-
-
-class InvalidNode(WavelinkException):
-    pass
-
-
-class InvalidLavalinkVersion(WavelinkException):
-    """Exception raised when you try to use wavelink 2 with a Lavalink version under 3.7."""
-    pass
-
-
-class InvalidLavalinkResponse(WavelinkException):
-    """Exception raised when wavelink receives an invalid response from Lavalink.
-
-    Attributes
-    ----------
-    status: int | None
-        The status code. Could be None.
-    """
-
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        super().__init__(*args)
-        self.status: int | None = kwargs.get('status')
-
-
-class NoTracksError(WavelinkException):
-    """Exception raised when no tracks could be found."""
-    pass
-
-
-class QueueEmpty(WavelinkException):
-    """Exception raised when you try to retrieve from an empty queue."""
-    pass
-
-
-class InvalidChannelStateError(WavelinkException):
-    """Base exception raised when an error occurs trying to connect to a :class:`discord.VoiceChannel`."""
-
-
-class InvalidChannelPermissions(InvalidChannelStateError):
-    """Exception raised when the client does not have correct permissions to join the channel.
-
-    Could also be raised when there are too many users already in a user limited channel.
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+from typing import Any
+
+__all__ = (
+    'WavelinkException',
+    'AuthorizationFailed',
+    'InvalidNode',
+    'InvalidLavalinkVersion',
+    'InvalidLavalinkResponse',
+    'NoTracksError',
+    'QueueEmpty',
+    'InvalidChannelStateError',
+    'InvalidChannelPermissions',
+)
+
+
+class WavelinkException(Exception):
+    """Base wavelink exception."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args)
+
+
+class AuthorizationFailed(WavelinkException):
+    """Exception raised when password authorization failed for this Lavalink node."""
+    pass
+
+
+class InvalidNode(WavelinkException):
+    pass
+
+
+class InvalidLavalinkVersion(WavelinkException):
+    """Exception raised when you try to use wavelink 2 with a Lavalink version under 3.7."""
+    pass
+
+
+class InvalidLavalinkResponse(WavelinkException):
+    """Exception raised when wavelink receives an invalid response from Lavalink.
+
+    Attributes
+    ----------
+    status: int | None
+        The status code. Could be None.
+    """
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args)
+        self.status: int | None = kwargs.get('status')
+
+
+class NoTracksError(WavelinkException):
+    """Exception raised when no tracks could be found."""
+    pass
+
+
+class QueueEmpty(WavelinkException):
+    """Exception raised when you try to retrieve from an empty queue."""
+    pass
+
+
+class InvalidChannelStateError(WavelinkException):
+    """Base exception raised when an error occurs trying to connect to a :class:`discord.VoiceChannel`."""
+
+
+class InvalidChannelPermissions(InvalidChannelStateError):
+    """Exception raised when the client does not have correct permissions to join the channel.
+
+    Could also be raised when there are too many users already in a user limited channel.
     """
```

### Comparing `Wavelink-2.6.0/wavelink/ext/spotify/__init__.py` & `wavelink-2.6.1/wavelink/ext/spotify/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,511 +1,511 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import asyncio
-import base64
-import logging
-import time
-from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
-
-import aiohttp
-from discord.ext import commands
-
-import wavelink
-from wavelink import Node, NodePool
-
-from .utils import *
-
-
-if TYPE_CHECKING:
-    from wavelink import Player, Playable
-
-
-__all__ = (
-    'SpotifySearchType',
-    'SpotifyClient',
-    'SpotifyTrack',
-    'SpotifyRequestError',
-    'decode_url',
-    'SpotifyDecodePayload'
-)
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-ST = TypeVar("ST", bound="Playable")
-
-
-class SpotifyAsyncIterator:
-
-    def __init__(self, *, query: str, limit: int, type: SpotifySearchType, node: Node):
-        self._query = query
-        self._limit = limit
-        self._type = type
-        self._node = node
-
-        self._first = True
-        self._count = 0
-        self._queue = asyncio.Queue()
-
-    def __aiter__(self):
-        return self
-
-    async def fill_queue(self):
-        tracks = await self._node._spotify._search(query=self._query, iterator=True, type=self._type)
-
-        for track in tracks:
-            await self._queue.put(track)
-
-    async def __anext__(self):
-        if self._first:
-            await self.fill_queue()
-            self._first = False
-
-        if self._limit is not None and self._count == self._limit:
-            raise StopAsyncIteration
-
-        try:
-            track = self._queue.get_nowait()
-        except asyncio.QueueEmpty as e:
-            raise StopAsyncIteration from e
-
-        if track is None:
-            return await self.__anext__()
-
-        track = SpotifyTrack(track)
-
-        self._count += 1
-        return track
-
-
-class SpotifyRequestError(Exception):
-    """Base error for Spotify requests.
-
-    Attributes
-    ----------
-    status: int
-        The status code returned from the request.
-    reason: Optional[str]
-        The reason the request failed. Could be None.
-    """
-
-    def __init__(self, status: int, reason: Optional[str] = None):
-        self.status = status
-        self.reason = reason
-
-
-class SpotifyTrack:
-    """A track retrieved via Spotify.
-
-
-    .. container:: operations
-
-        .. describe:: str(track)
-
-            Returns a string representing this SpotifyTrack's name and artists.
-
-        .. describe:: repr(track)
-
-            Returns an official string representation of this SpotifyTrack.
-
-        .. describe:: track == other_track
-
-            Check whether a track is equal to another. Tracks are equal if they both have the same Spotify ID.
-
-
-    Attributes
-    ----------
-    raw: dict[str, Any]
-        The raw payload from Spotify for this track.
-    album: str
-        The album name this track belongs to.
-    images: list[str]
-        A list of URLs to images associated with this track.
-    artists: list[str]
-        A list of artists for this track.
-    genres: list[str]
-        A list of genres associated with this tracks artist.
-    name: str
-        The track name.
-    title: str
-        An alias to name.
-    uri: str
-        The URI for this spotify track.
-    id: str
-        The spotify ID for this track.
-    isrc: str | None
-        The International Standard Recording Code associated with this track.
-    length: int
-        The track length in milliseconds.
-    duration: int
-        Alias to length.
-    explicit: bool
-        Whether this track is explicit or not.
-    """
-
-    __slots__ = (
-        'raw',
-        'album',
-        'images',
-        'artists',
-        'name',
-        'title',
-        'uri',
-        'id',
-        'length',
-        'duration',
-        'explicit',
-        'isrc',
-        '__dict__'
-    )
-
-    def __init__(self, data: dict[str, Any]) -> None:
-        self.raw: dict[str, Any] = data
-
-        album = data['album']
-        self.album: str = album['name']
-        self.images: list[str] = [i['url'] for i in album['images']]
-
-        artists = data['artists']
-        self.artists: list[str] = [a['name'] for a in artists]
-        # self.genres: list[str] = [a['genres'] for a in artists]
-
-        self.name: str = data['name']
-        self.title: str = self.name
-        self.uri: str = data['uri']
-        self.id: str = data['id']
-        self.length: int = data['duration_ms']
-        self.duration: int = self.length
-        self.isrc: str | None = data.get("external_ids", {}).get('irsc')
-        self.explicit: bool = data.get('explicit', False) in {"true", True}
-
-    def __str__(self) -> str:
-        return f'{self.name} - {self.artists[0]}'
-
-    def __repr__(self) -> str:
-        return f'SpotifyTrack(id={self.id}, isrc={self.isrc}, name={self.name}, duration={self.duration})'
-
-    def __eq__(self, other) -> bool:
-        if isinstance(other, SpotifyTrack):
-            return self.id == other.id
-        raise NotImplemented
-
-    @classmethod
-    async def search(
-            cls,
-            query: str,
-            *,
-            node: Node | None = None,
-    ) -> list['SpotifyTrack']:
-        """|coro|
-
-        Search for tracks with the given query.
-
-        Parameters
-        ----------
-        query: str
-            The Spotify URL to query for.
-        node: Optional[:class:`wavelink.Node`]
-            An optional Node to use to make the search with.
-
-        Returns
-        -------
-        List[:class:`SpotifyTrack`]
-
-        Examples
-        --------
-        Searching for a singular tack to play...
-
-        .. code:: python3
-
-            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
-            if not tracks:
-                # No tracks found, do something?
-                return
-
-            track: spotify.SpotifyTrack = tracks[0]
-
-
-        Searching for all tracks in an album...
-
-        .. code:: python3
-
-            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
-            if not tracks:
-                # No tracks found, do something?
-                return
-
-
-        .. versionchanged:: 2.6.0
-
-            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
-            if the ``type`` returned by :func:`decode_url` is unusable, this method will return an empty :class:`list`
-        """
-        if node is None:
-            node: Node = NodePool.get_connected_node()
-
-        decoded: SpotifyDecodePayload = decode_url(query)
-
-        if not decoded or decoded.type is SpotifySearchType.unusable:
-            logger.debug(f'Spotify search handled an unusable search type for query: "{query}".')
-            return []
-
-        return await node._spotify._search(query=query, type=decoded.type)
-
-    @classmethod
-    def iterator(cls,
-                 *,
-                 query: str,
-                 limit: int | None = None,
-                 node: Node | None = None,
-                 ):
-        """An async iterator version of search.
-
-        This can be useful when searching for large playlists or albums with Spotify.
-
-        Parameters
-        ----------
-        query: str
-            The Spotify URL to search for. Must be of type Playlist or Album.
-        limit: Optional[int]
-            Limit the amount of tracks returned.
-        node: Optional[:class:`wavelink.Node`]
-            An optional node to use when querying for tracks. Defaults to the best available.
-
-        Examples
-        --------
-
-        .. code:: python3
-
-                async for track in spotify.SpotifyTrack.iterator(query=...):
-                    ...
-
-
-        .. versionchanged:: 2.6.0
-
-            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
-            if the ``type`` returned by :func:`decode_url` is not either ``album`` or ``playlist`` this method will
-            raise a :exc:`TypeError`.
-        """
-        decoded: SpotifyDecodePayload = decode_url(query)
-
-        if not decoded or decoded.type is not SpotifySearchType.album and decoded.type is not SpotifySearchType.playlist:
-            raise TypeError('Spotify iterator query must be either a valid Spotify album or playlist URL.')
-
-        if node is None:
-            node = NodePool.get_connected_node()
-
-        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=decoded.type)
-
-    @classmethod
-    async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
-        """Converter which searches for and returns the first track.
-
-        Used as a type hint in a
-        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
-        """
-        results = await cls.search(argument)
-
-        if not results:
-            raise commands.BadArgument(f"Could not find any songs matching query: {argument}")
-
-        return results[0]
-
-    async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
-        """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
-
-        .. warning::
-
-            Usually you would not call this directly. Instead you would set :attr:`wavelink.Player.autoplay` to true,
-            and allow the player to fulfill this request automatically.
-
-
-        Parameters
-        ----------
-        player: :class:`wavelink.player.Player`
-            If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
-        cls
-            The class to convert this Spotify Track to.
-        """
-
-        if not self.isrc:
-            tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
-        else:
-            tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-            if not tracks:
-                tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
-
-        if not player.autoplay or not populate:
-            return tracks[0]
-
-        node: Node = player.current_node
-        sc: SpotifyClient | None = node._spotify
-
-        if not sc:
-            raise RuntimeError(f"There is no spotify client associated with <{node:!r}>")
-
-        if sc.is_token_expired():
-            await sc._get_bearer_token()
-
-        if len(player._track_seeds) == 5:
-            player._track_seeds.pop(0)
-
-        player._track_seeds.append(self.id)
-
-        url: str = RECURL.format(tracks=','.join(player._track_seeds))
-        async with node._session.get(url=url, headers=sc.bearer_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-
-        recos = [SpotifyTrack(t) for t in data['tracks']]
-        for reco in recos:
-            if reco in player.auto_queue or reco in player.auto_queue.history:
-                continue
-
-            await player.auto_queue.put_wait(reco)
-
-        return tracks[0]
-
-
-class SpotifyClient:
-    """Spotify client passed to :class:`wavelink.Node` for searching via Spotify.
-
-    Parameters
-    ----------
-    client_id: str
-        Your spotify application client ID.
-    client_secret: str
-        Your spotify application secret.
-    """
-
-    def __init__(self, *, client_id: str, client_secret: str):
-        self._client_id = client_id
-        self._client_secret = client_secret
-
-        self.session = aiohttp.ClientSession()
-
-        self._bearer_token: str | None = None
-        self._expiry: int = 0
-
-    @property
-    def grant_headers(self) -> dict:
-        authbytes = f'{self._client_id}:{self._client_secret}'.encode()
-        return {'Authorization': f'Basic {base64.b64encode(authbytes).decode()}',
-                'Content-Type': 'application/x-www-form-urlencoded'}
-
-    @property
-    def bearer_headers(self) -> dict:
-        return {'Authorization': f'Bearer {self._bearer_token}'}
-
-    async def _get_bearer_token(self) -> None:
-        async with self.session.post(GRANTURL, headers=self.grant_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-            self._bearer_token = data['access_token']
-            self._expiry = time.time() + (int(data['expires_in']) - 10)
-
-    def is_token_expired(self) -> bool:
-        return time.time() >= self._expiry
-
-    async def _search(self,
-                      query: str,
-                      type: SpotifySearchType = SpotifySearchType.track,
-                      iterator: bool = False,
-                      ) -> list[SpotifyTrack]:
-
-        if self.is_token_expired():
-            await self._get_bearer_token()
-
-        regex_result = URLREGEX.match(query)
-
-        url = (
-            BASEURL.format(
-                entity=regex_result['type'], identifier=regex_result['id']
-            )
-            if regex_result
-            else BASEURL.format(entity=type.name, identifier=query)
-        )
-
-        async with self.session.get(url, headers=self.bearer_headers) as resp:
-            if resp.status == 400:
-                return []
-
-            elif resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-
-        if data['type'] == 'track':
-            return [SpotifyTrack(data)]
-
-        elif data['type'] == 'album':
-            album_data: dict[str, Any] = {
-                                        'album_type': data['album_type'],
-                                        'artists': data['artists'],
-                                        'available_markets': data['available_markets'],
-                                        'external_urls': data['external_urls'],
-                                        'href': data['href'],
-                                        'id': data['id'],
-                                        'images': data['images'],
-                                        'name': data['name'],
-                                        'release_date': data['release_date'],
-                                        'release_date_precision': data['release_date_precision'],
-                                        'total_tracks': data['total_tracks'],
-                                        'type': data['type'],
-                                        'uri': data['uri'],
-                                        }
-            tracks = []
-            for track in data['tracks']['items']:
-                track['album'] = album_data
-                if iterator:
-                    tracks.append(track)
-                else:
-                    tracks.append(SpotifyTrack(track))
-
-            return tracks
-
-        elif data['type'] == 'playlist':
-            if not iterator:
-                return [SpotifyTrack(t['track']) for t in data['tracks']['items']]
-            if not data['tracks']['next']:
-                return [t['track'] for t in data['tracks']['items']]
-
-            url = data['tracks']['next']
-
-            items = [t['track'] for t in data['tracks']['items']]
-            while True:
-                async with self.session.get(url, headers=self.bearer_headers) as resp:
-                    data = await resp.json()
-
-                    items.extend([t['track'] for t in data['items']])
-                    if not data['next']:
-                        return items
-
-                    url = data['next']
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import asyncio
+import base64
+import logging
+import time
+from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
+
+import aiohttp
+from discord.ext import commands
+
+import wavelink
+from wavelink import Node, NodePool
+
+from .utils import *
+
+
+if TYPE_CHECKING:
+    from wavelink import Player, Playable
+
+
+__all__ = (
+    'SpotifySearchType',
+    'SpotifyClient',
+    'SpotifyTrack',
+    'SpotifyRequestError',
+    'decode_url',
+    'SpotifyDecodePayload'
+)
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+ST = TypeVar("ST", bound="Playable")
+
+
+class SpotifyAsyncIterator:
+
+    def __init__(self, *, query: str, limit: int, type: SpotifySearchType, node: Node):
+        self._query = query
+        self._limit = limit
+        self._type = type
+        self._node = node
+
+        self._first = True
+        self._count = 0
+        self._queue = asyncio.Queue()
+
+    def __aiter__(self):
+        return self
+
+    async def fill_queue(self):
+        tracks = await self._node._spotify._search(query=self._query, iterator=True, type=self._type)
+
+        for track in tracks:
+            await self._queue.put(track)
+
+    async def __anext__(self):
+        if self._first:
+            await self.fill_queue()
+            self._first = False
+
+        if self._limit is not None and self._count == self._limit:
+            raise StopAsyncIteration
+
+        try:
+            track = self._queue.get_nowait()
+        except asyncio.QueueEmpty as e:
+            raise StopAsyncIteration from e
+
+        if track is None:
+            return await self.__anext__()
+
+        track = SpotifyTrack(track)
+
+        self._count += 1
+        return track
+
+
+class SpotifyRequestError(Exception):
+    """Base error for Spotify requests.
+
+    Attributes
+    ----------
+    status: int
+        The status code returned from the request.
+    reason: Optional[str]
+        The reason the request failed. Could be None.
+    """
+
+    def __init__(self, status: int, reason: Optional[str] = None):
+        self.status = status
+        self.reason = reason
+
+
+class SpotifyTrack:
+    """A track retrieved via Spotify.
+
+
+    .. container:: operations
+
+        .. describe:: str(track)
+
+            Returns a string representing this SpotifyTrack's name and artists.
+
+        .. describe:: repr(track)
+
+            Returns an official string representation of this SpotifyTrack.
+
+        .. describe:: track == other_track
+
+            Check whether a track is equal to another. Tracks are equal if they both have the same Spotify ID.
+
+
+    Attributes
+    ----------
+    raw: dict[str, Any]
+        The raw payload from Spotify for this track.
+    album: str
+        The album name this track belongs to.
+    images: list[str]
+        A list of URLs to images associated with this track.
+    artists: list[str]
+        A list of artists for this track.
+    genres: list[str]
+        A list of genres associated with this tracks artist.
+    name: str
+        The track name.
+    title: str
+        An alias to name.
+    uri: str
+        The URI for this spotify track.
+    id: str
+        The spotify ID for this track.
+    isrc: str | None
+        The International Standard Recording Code associated with this track.
+    length: int
+        The track length in milliseconds.
+    duration: int
+        Alias to length.
+    explicit: bool
+        Whether this track is explicit or not.
+    """
+
+    __slots__ = (
+        'raw',
+        'album',
+        'images',
+        'artists',
+        'name',
+        'title',
+        'uri',
+        'id',
+        'length',
+        'duration',
+        'explicit',
+        'isrc',
+        '__dict__'
+    )
+
+    def __init__(self, data: dict[str, Any]) -> None:
+        self.raw: dict[str, Any] = data
+
+        album = data['album']
+        self.album: str = album['name']
+        self.images: list[str] = [i['url'] for i in album['images']]
+
+        artists = data['artists']
+        self.artists: list[str] = [a['name'] for a in artists]
+        # self.genres: list[str] = [a['genres'] for a in artists]
+
+        self.name: str = data['name']
+        self.title: str = self.name
+        self.uri: str = data['uri']
+        self.id: str = data['id']
+        self.length: int = data['duration_ms']
+        self.duration: int = self.length
+        self.isrc: str | None = data.get("external_ids", {}).get('irsc')
+        self.explicit: bool = data.get('explicit', False) in {"true", True}
+
+    def __str__(self) -> str:
+        return f'{self.name} - {self.artists[0]}'
+
+    def __repr__(self) -> str:
+        return f'SpotifyTrack(id={self.id}, isrc={self.isrc}, name={self.name}, duration={self.duration})'
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, SpotifyTrack):
+            return self.id == other.id
+        raise NotImplemented
+
+    @classmethod
+    async def search(
+            cls,
+            query: str,
+            *,
+            node: Node | None = None,
+    ) -> list['SpotifyTrack']:
+        """|coro|
+
+        Search for tracks with the given query.
+
+        Parameters
+        ----------
+        query: str
+            The Spotify URL to query for.
+        node: Optional[:class:`wavelink.Node`]
+            An optional Node to use to make the search with.
+
+        Returns
+        -------
+        List[:class:`SpotifyTrack`]
+
+        Examples
+        --------
+        Searching for a singular tack to play...
+
+        .. code:: python3
+
+            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+            if not tracks:
+                # No tracks found, do something?
+                return
+
+            track: spotify.SpotifyTrack = tracks[0]
+
+
+        Searching for all tracks in an album...
+
+        .. code:: python3
+
+            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+            if not tracks:
+                # No tracks found, do something?
+                return
+
+
+        .. versionchanged:: 2.6.0
+
+            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
+            if the ``type`` returned by :func:`decode_url` is unusable, this method will return an empty :class:`list`
+        """
+        if node is None:
+            node: Node = NodePool.get_connected_node()
+
+        decoded: SpotifyDecodePayload = decode_url(query)
+
+        if not decoded or decoded.type is SpotifySearchType.unusable:
+            logger.debug(f'Spotify search handled an unusable search type for query: "{query}".')
+            return []
+
+        return await node._spotify._search(query=query, type=decoded.type)
+
+    @classmethod
+    def iterator(cls,
+                 *,
+                 query: str,
+                 limit: int | None = None,
+                 node: Node | None = None,
+                 ):
+        """An async iterator version of search.
+
+        This can be useful when searching for large playlists or albums with Spotify.
+
+        Parameters
+        ----------
+        query: str
+            The Spotify URL to search for. Must be of type Playlist or Album.
+        limit: Optional[int]
+            Limit the amount of tracks returned.
+        node: Optional[:class:`wavelink.Node`]
+            An optional node to use when querying for tracks. Defaults to the best available.
+
+        Examples
+        --------
+
+        .. code:: python3
+
+                async for track in spotify.SpotifyTrack.iterator(query=...):
+                    ...
+
+
+        .. versionchanged:: 2.6.0
+
+            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
+            if the ``type`` returned by :func:`decode_url` is not either ``album`` or ``playlist`` this method will
+            raise a :exc:`TypeError`.
+        """
+        decoded: SpotifyDecodePayload = decode_url(query)
+
+        if not decoded or decoded.type is not SpotifySearchType.album and decoded.type is not SpotifySearchType.playlist:
+            raise TypeError('Spotify iterator query must be either a valid Spotify album or playlist URL.')
+
+        if node is None:
+            node = NodePool.get_connected_node()
+
+        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=decoded.type)
+
+    @classmethod
+    async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
+        """Converter which searches for and returns the first track.
+
+        Used as a type hint in a
+        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
+        """
+        results = await cls.search(argument)
+
+        if not results:
+            raise commands.BadArgument(f"Could not find any songs matching query: {argument}")
+
+        return results[0]
+
+    async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
+        """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
+
+        .. warning::
+
+            Usually you would not call this directly. Instead you would set :attr:`wavelink.Player.autoplay` to true,
+            and allow the player to fulfill this request automatically.
+
+
+        Parameters
+        ----------
+        player: :class:`wavelink.player.Player`
+            If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
+        cls
+            The class to convert this Spotify Track to.
+        """
+
+        if not self.isrc:
+            tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
+        else:
+            tracks: list[cls] = await cls.search(f'"{self.isrc}"')
+            if not tracks:
+                tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
+
+        if not player.autoplay or not populate:
+            return tracks[0]
+
+        node: Node = player.current_node
+        sc: SpotifyClient | None = node._spotify
+
+        if not sc:
+            raise RuntimeError(f"There is no spotify client associated with <{node:!r}>")
+
+        if sc.is_token_expired():
+            await sc._get_bearer_token()
+
+        if len(player._track_seeds) == 5:
+            player._track_seeds.pop(0)
+
+        player._track_seeds.append(self.id)
+
+        url: str = RECURL.format(tracks=','.join(player._track_seeds))
+        async with node._session.get(url=url, headers=sc.bearer_headers) as resp:
+            if resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+
+        recos = [SpotifyTrack(t) for t in data['tracks']]
+        for reco in recos:
+            if reco in player.auto_queue or reco in player.auto_queue.history:
+                continue
+
+            await player.auto_queue.put_wait(reco)
+
+        return tracks[0]
+
+
+class SpotifyClient:
+    """Spotify client passed to :class:`wavelink.Node` for searching via Spotify.
+
+    Parameters
+    ----------
+    client_id: str
+        Your spotify application client ID.
+    client_secret: str
+        Your spotify application secret.
+    """
+
+    def __init__(self, *, client_id: str, client_secret: str):
+        self._client_id = client_id
+        self._client_secret = client_secret
+
+        self.session = aiohttp.ClientSession()
+
+        self._bearer_token: str | None = None
+        self._expiry: int = 0
+
+    @property
+    def grant_headers(self) -> dict:
+        authbytes = f'{self._client_id}:{self._client_secret}'.encode()
+        return {'Authorization': f'Basic {base64.b64encode(authbytes).decode()}',
+                'Content-Type': 'application/x-www-form-urlencoded'}
+
+    @property
+    def bearer_headers(self) -> dict:
+        return {'Authorization': f'Bearer {self._bearer_token}'}
+
+    async def _get_bearer_token(self) -> None:
+        async with self.session.post(GRANTURL, headers=self.grant_headers) as resp:
+            if resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+            self._bearer_token = data['access_token']
+            self._expiry = time.time() + (int(data['expires_in']) - 10)
+
+    def is_token_expired(self) -> bool:
+        return time.time() >= self._expiry
+
+    async def _search(self,
+                      query: str,
+                      type: SpotifySearchType = SpotifySearchType.track,
+                      iterator: bool = False,
+                      ) -> list[SpotifyTrack]:
+
+        if self.is_token_expired():
+            await self._get_bearer_token()
+
+        regex_result = URLREGEX.match(query)
+
+        url = (
+            BASEURL.format(
+                entity=regex_result['type'], identifier=regex_result['id']
+            )
+            if regex_result
+            else BASEURL.format(entity=type.name, identifier=query)
+        )
+
+        async with self.session.get(url, headers=self.bearer_headers) as resp:
+            if resp.status == 400:
+                return []
+
+            elif resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+
+        if data['type'] == 'track':
+            return [SpotifyTrack(data)]
+
+        elif data['type'] == 'album':
+            album_data: dict[str, Any] = {
+                                        'album_type': data['album_type'],
+                                        'artists': data['artists'],
+                                        'available_markets': data['available_markets'],
+                                        'external_urls': data['external_urls'],
+                                        'href': data['href'],
+                                        'id': data['id'],
+                                        'images': data['images'],
+                                        'name': data['name'],
+                                        'release_date': data['release_date'],
+                                        'release_date_precision': data['release_date_precision'],
+                                        'total_tracks': data['total_tracks'],
+                                        'type': data['type'],
+                                        'uri': data['uri'],
+                                        }
+            tracks = []
+            for track in data['tracks']['items']:
+                track['album'] = album_data
+                if iterator:
+                    tracks.append(track)
+                else:
+                    tracks.append(SpotifyTrack(track))
+
+            return tracks
+
+        elif data['type'] == 'playlist':
+            if not iterator:
+                return [SpotifyTrack(t['track']) for t in data['tracks']['items']]
+            if not data['tracks']['next']:
+                return [t['track'] for t in data['tracks']['items']]
+
+            url = data['tracks']['next']
+
+            items = [t['track'] for t in data['tracks']['items']]
+            while True:
+                async with self.session.get(url, headers=self.bearer_headers) as resp:
+                    data = await resp.json()
+
+                    items.extend([t['track'] for t in data['items']])
+                    if not data['next']:
+                        return items
+
+                    url = data['next']
```

### Comparing `Wavelink-2.6.0/wavelink/node.py` & `wavelink-2.6.1/wavelink/node.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,574 +1,574 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import logging
-import random
-import re
-import string
-from typing import TYPE_CHECKING, Any, TypeVar
-
-import aiohttp
-import discord
-from discord.enums import try_enum
-from discord.utils import MISSING, classproperty
-import urllib.parse
-
-from . import __version__
-from .enums import LoadType, NodeStatus
-from .exceptions import *
-from .websocket import Websocket
-
-if TYPE_CHECKING:
-    from .player import Player
-    from .tracks import *
-    from .types.request import Request
-    from .ext import spotify as spotify_
-
-    PlayableT = TypeVar('PlayableT', bound=Playable)
-    
-
-__all__ = ('Node', 'NodePool')
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-# noinspection PyShadowingBuiltins
-class Node:
-    """The base Wavelink Node.
-
-    The Node is responsible for keeping the Websocket alive, tracking the state of Players
-    and fetching/decoding Tracks and Playlists.
-
-    .. note::
-
-        The Node class should only be created once per Lavalink connection.
-        To retrieve a Node use the appropriate :class:`NodePool` methods instead.
-
-    .. warning::
-
-        The Node will not be connected until passed to :meth:`NodePool.connect`.
-
-
-    .. container:: operations
-
-        .. describe:: repr(node)
-
-            Returns an official string representation of this Node.
-
-
-    Parameters
-    ----------
-    id: Optional[str]
-        The unique identifier for this Node. If not passed, one will be generated randomly.
-    uri: str
-        The uri to connect to your Lavalink server. E.g ``http://localhost:2333``.
-    password: str
-        The password used to connect to your Lavalink server.
-    secure: Optional[bool]
-        Whether the connection should use https/wss.
-    use_http: Optional[bool]
-        Whether to use http:// over ws:// when connecting to the Lavalink websocket. Defaults to False.
-    session: Optional[aiohttp.ClientSession]
-        The session to use for this Node. If no session is passed a default will be used.
-    heartbeat: float
-        The time in seconds to send a heartbeat ack. Defaults to 15.0.
-    retries: Optional[int]
-        The amount of times this Node will try to reconnect after a disconnect.
-        If not set the Node will try unlimited times.
-
-    Attributes
-    ----------
-    heartbeat: float
-        The time in seconds to send a heartbeat ack. Defaults to 15.0.
-    client: :class:`discord.Client`
-        The discord client used to connect this Node. Could be None if this Node has not been connected.
-    """
-
-    def __init__(
-            self,
-            *,
-            id: str | None = None,
-            uri: str,
-            password: str,
-            secure: bool = False,
-            use_http: bool = False,
-            session: aiohttp.ClientSession = MISSING,
-            heartbeat: float = 15.0,
-            retries: int | None = None,
-    ) -> None:
-        if id is None:
-            id = ''.join(random.sample(string.ascii_letters + string.digits, 12))
-
-        self._id: str = id
-        self._uri: str = uri
-        self._secure: bool = secure
-        self._use_http: bool = use_http
-        host: str = re.sub(r'(?:http|ws)s?://', '', self._uri)
-        self._host: str = f'{"https://" if secure else "http://"}{host}'
-        self._password: str = password
-
-        self._session: aiohttp.ClientSession = session
-        self.heartbeat: float = heartbeat
-        self._retries: int | None = retries
-
-        self.client: discord.Client | None = None
-        self._websocket: Websocket = MISSING
-        self._session_id: str | None = None
-
-        self._players: dict[int, Player] = {}
-        self._invalidated: dict[int, Player] = {}
-
-        self._status: NodeStatus = NodeStatus.DISCONNECTED
-        self._major_version: int | None = None
-
-        self._spotify: spotify_.SpotifyClient | None = None
-
-    def __repr__(self) -> str:
-        return f'Node(id="{self._id}", uri="{self.uri}", status={self.status})'
-
-    def __eq__(self, other: object) -> bool:
-        return self.id == other.id if isinstance(other, Node) else NotImplemented
-
-    @property
-    def id(self) -> str:
-        """The Nodes unique identifier."""
-        return self._id
-
-    @property
-    def uri(self) -> str:
-        """The URI used to connect this Node to Lavalink."""
-        return self._host
-
-    @property
-    def password(self) -> str:
-        """The password used to connect this Node to Lavalink."""
-        return self._password
-
-    @property
-    def players(self) -> dict[int, Player]:
-        """A mapping of Guild ID to Player."""
-        return self._players
-
-    @property
-    def status(self) -> NodeStatus:
-        """The connection status of this Node.
-
-        DISCONNECTED
-        CONNECTING
-        CONNECTED
-        """
-        return self._status
-
-    def get_player(self, guild_id: int, /) -> Player | None:
-        """Return the :class:`player.Player` associated with the provided guild ID.
-
-        If no :class:`player.Player` is found, returns None.
-
-        Parameters
-        ----------
-        guild_id: int
-            The Guild ID to return a Player for.
-
-        Returns
-        -------
-        Optional[:class:`player.Player`]
-        """
-        return self._players.get(guild_id, None)
-
-    async def _connect(self, client: discord.Client) -> None:
-        if client.user is None:
-            raise RuntimeError('')
-
-        if not self._session:
-            self._session = aiohttp.ClientSession(headers={'Authorization': self._password})
-
-        self.client = client
-
-        self._websocket = Websocket(node=self)
-
-        await self._websocket.connect()
-
-        async with self._session.get(f'{self._host}/version') as resp:
-            version: str = await resp.text()
-
-            if version.endswith('-SNAPSHOT'):
-                self._major_version = 3
-                return
-
-            try:
-                version_tuple = tuple(int(v) for v in version.split('.'))
-            except ValueError:
-                logging.warning(f'Lavalink "{version}" is unknown and may not be compatible with: '
-                                f'Wavelink "{__version__}". Wavelink is assuming the Lavalink version.')
-
-                self._major_version = 3
-                return
-
-            if version_tuple[0] < 3:
-                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with Lavalink "{version}".')
-
-            if version_tuple[0] == 3 and version_tuple[1] < 7:
-                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with '
-                                             f'Lavalink versions under "3.7".')
-
-            self._major_version = version_tuple[0]
-            logger.info(f'Lavalink version "{version}" connected for Node: {self.id}')
-
-    async def _send(self,
-                    *,
-                    method: str,
-                    path: str,
-                    guild_id: int | str | None = None,
-                    query: str | None = None,
-                    data: Request | None = None,
-                    ) -> dict[str, Any] | None:
-
-        uri: str = f'{self._host}/' \
-                   f'v{self._major_version}/' \
-                   f'{path}' \
-                   f'{f"/{guild_id}" if guild_id else ""}' \
-                   f'{f"?{query}" if query else ""}'
-
-        logger.debug(f'Node {self} is sending payload to [{method}] "{uri}" with payload: {data}')
-
-        async with self._session.request(method=method, url=uri, json=data or {}) as resp:
-            rdata: dict[str | int, Any] | None = None
-
-            if resp.content_type == 'application/json':
-                rdata = await resp.json()
-
-            logger.debug(f'Node {self} received payload from Lavalink after sending to "{uri}" with response: '
-                         f'<status={resp.status}, data={rdata}>')
-
-            if resp.status >= 300:
-                raise InvalidLavalinkResponse(f'An error occurred when attempting to reach: "{uri}".',
-                                              status=resp.status)
-
-            if resp.status == 204:
-                return
-
-            return rdata
-
-    async def get_tracks(self, cls: type[PlayableT], query: str) -> list[PlayableT]:
-        """|coro|
-
-        Search for and retrieve Tracks based on the query and cls provided.
-
-        .. note::
-
-            If the query is not a Local search or direct URL, you will need to provide a search prefix.
-            E.g. ``ytsearch:`` for a YouTube search.
-
-        Parameters
-        ----------
-        cls: type[PlayableT]
-            The type of Playable tracks that should be returned.
-        query: str
-            The query to search for and return tracks.
-
-        Returns
-        -------
-        list[PlayableT]
-            A list of found tracks converted to the provided cls.
-        """
-        logger.debug(f'Node {self} is requesting tracks with query "{query}".')
-
-        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
-        load_type = try_enum(LoadType, data.get("loadType"))
-
-        if load_type is LoadType.load_failed:
-            # TODO - Proper Exception...
-
-            raise ValueError('Track Failed to load.')
-
-        if load_type is LoadType.no_matches:
-            return []
-
-        if load_type is LoadType.track_loaded:
-            track_data = data["tracks"][0]
-            return [cls(track_data)]
-
-        if load_type is not LoadType.search_result:
-            # TODO - Proper Exception...
-
-            raise ValueError('Track Failed to load.')
-
-        return [cls(track_data) for track_data in data["tracks"]]
-
-    async def get_playlist(self, cls: Playlist, query: str):
-        """|coro|
-
-        Search for and return a :class:`tracks.Playlist` given an identifier.
-
-        Parameters
-        ----------
-        cls: Type[:class:`tracks.Playlist`]
-            The type of which playlist should be returned, this must subclass :class:`tracks.Playlist`.
-        query: str
-            The playlist's identifier. This may be a YouTube playlist URL for example.
-
-        Returns
-        -------
-        Optional[:class:`tracks.Playlist`]:
-            The related wavelink track object or ``None`` if none was found.
-
-        Raises
-        ------
-        ValueError
-            Loading the playlist failed.
-        WavelinkException
-            An unspecified error occurred when loading the playlist.
-        """
-        logger.debug(f'Node {self} is requesting a playlist with query "{query}".')
-
-        encoded_query = urllib.parse.quote(query)
-        data = await self._send(method='GET', path='loadtracks', query=f'identifier={encoded_query}')
-
-        load_type = try_enum(LoadType, data.get("loadType"))
-
-        if load_type is LoadType.load_failed:
-            # TODO Proper exception...
-            raise ValueError('Tracks failed to Load.')
-
-        if load_type is LoadType.no_matches:
-            return None
-
-        if load_type is not LoadType.playlist_loaded:
-            raise WavelinkException("Track failed to load.")
-
-        return cls(data)
-
-    async def build_track(self, *, cls: type[PlayableT], encoded: str) -> PlayableT:
-        """|coro|
-
-        Build a track from the provided encoded string with the given Track class.
-
-        Parameters
-        ----------
-        cls: type[PlayableT]
-            The type of Playable track that should be returned.
-        encoded: str
-            The Tracks unique encoded string.
-        """
-        encoded_query = urllib.parse.quote(encoded)
-        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
-
-        logger.debug(f'Node {self} built encoded track with encoding "{encoded}". Response data: {data}')
-        return cls(data=data)
-
-
-# noinspection PyShadowingBuiltins
-class NodePool:
-    """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
-
-    Attributes
-    ----------
-    nodes: dict[str, :class:`Node`]
-        A mapping of :class:`Node` identifier to :class:`Node`.
-
-
-    .. warning::
-
-        This class should never be initialised. All methods are class methods.
-    """
-
-    __nodes: dict[str, Node] = {}
-
-    @classmethod
-    async def connect(
-            cls,
-            *,
-            client: discord.Client,
-            nodes: list[Node],
-            spotify: spotify_.SpotifyClient | None = None
-    ) -> dict[str, Node]:
-        """|coro|
-
-        Connect a list of Nodes.
-
-        Parameters
-        ----------
-        client: :class:`discord.Client`
-            The discord Client or Bot used to connect the Nodes.
-        nodes: list[:class:`Node`]
-            A list of Nodes to connect.
-        spotify: Optional[:class:`ext.spotify.SpotifyClient`]
-            The spotify Client to use when searching for Spotify Tracks.
-
-        Returns
-        -------
-        dict[str, :class:`Node`]
-            A mapping of :class:`Node` identifier to :class:`Node`.
-        """
-        if client.user is None:
-            raise RuntimeError('')
-
-        for node in nodes:
-
-            if spotify:
-                node._spotify = spotify
-
-            if node.id in cls.__nodes:
-                logger.error(f'A Node with the ID "{node.id}" already exists on the NodePool. Disregarding.')
-                continue
-
-            try:
-                await node._connect(client)
-            except AuthorizationFailed:
-                logger.error(f'The Node <{node!r}> failed to authenticate properly. '
-                             f'Please check your password and try again.')
-            else:
-                cls.__nodes[node.id] = node
-
-        return cls.nodes
-
-    @classproperty
-    def nodes(cls) -> dict[str, Node]:
-        """A mapping of :class:`Node` identifier to :class:`Node`."""
-        return cls.__nodes
-
-    @classmethod
-    def get_node(cls, id: str | None = None) -> Node:
-        """Retrieve a :class:`Node` with the given ID or best, if no ID was passed.
-
-        Parameters
-        ----------
-        id: Optional[str]
-            The unique identifier of the :class:`Node` to retrieve. If not passed the best :class:`Node`
-            will be fetched.
-
-        Returns
-        -------
-        :class:`Node`
-
-        Raises
-        ------
-        InvalidNode
-            The given id does nto resolve to a :class:`Node` or no :class:`Node` has been connected.
-        """
-        if id:
-            if id not in cls.__nodes:
-                raise InvalidNode(f'A Node with ID "{id}" does not exist on the Wavelink NodePool.')
-
-            return cls.__nodes[id]
-
-        if not cls.__nodes:
-            raise InvalidNode('No Node currently exists on the Wavelink NodePool.')
-
-        nodes = cls.__nodes.values()
-        return sorted(nodes, key=lambda n: len(n.players))[0]
-
-    @classmethod
-    def get_connected_node(cls) -> Node:
-        """Get the best available connected :class:`Node`.
-
-        Returns
-        -------
-        :class:`Node`
-            The best available connected Node.
-
-        Raises
-        ------
-        InvalidNode
-            No Nodes are currently in the connected state.
-        """
-
-        nodes: list[Node] = [n for n in cls.__nodes.values() if n.status is NodeStatus.CONNECTED]
-        if not nodes:
-            raise InvalidNode('There are no Nodes on the Wavelink NodePool that are currently in the connected state.')
-
-        return sorted(nodes, key=lambda n: len(n.players))[0]
-
-    @classmethod
-    async def get_tracks(cls_,  # type: ignore
-                         query: str,
-                         /,
-                         *,
-                         cls: type[PlayableT],
-                         node: Node | None = None
-                         ) -> list[PlayableT]:
-        """|coro|
-
-        Helper method to retrieve tracks from the NodePool without fetching a :class:`Node`.
-
-        Parameters
-        ----------
-        query: str
-            The query to search for and return tracks.
-        cls: type[PlayableT]
-            The type of Playable tracks that should be returned.
-        node: Optional[:class:`Node`]
-            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
-            Defaults to None.
-
-        Returns
-        -------
-        list[PlayableT]
-            A list of found tracks converted to the provided cls.
-        """
-        if not node:
-            node = cls_.get_connected_node()
-
-        return await node.get_tracks(cls=cls, query=query)
-
-    @classmethod
-    async def get_playlist(cls_,  # type: ignore
-                           query: str,
-                           /,
-                           *,
-                           cls: Playlist,
-                           node: Node | None = None
-                           ) -> Playlist:
-        """|coro|
-
-        Helper method to retrieve a playlist from the NodePool without fetching a :class:`Node`.
-
-
-        .. warning::
-
-            The only playlists currently supported are :class:`tracks.YouTubePlaylist` and
-            :class:`tracks.YouTubePlaylist`.
-
-
-        Parameters
-        ----------
-        query: str
-            The query to search for and return a playlist.
-        cls: type[PlayableT]
-            The type of Playlist that should be returned.
-        node: Optional[:class:`Node`]
-            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
-            Defaults to None.
-
-        Returns
-        -------
-        Playlist
-            A Playlist with its tracks.
-        """
-        if not node:
-            node = cls_.get_connected_node()
-
-        return await node.get_playlist(cls=cls, query=query)
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import logging
+import random
+import re
+import string
+from typing import TYPE_CHECKING, Any, TypeVar
+
+import aiohttp
+import discord
+from discord.enums import try_enum
+from discord.utils import MISSING, classproperty
+import urllib.parse
+
+from . import __version__
+from .enums import LoadType, NodeStatus
+from .exceptions import *
+from .websocket import Websocket
+
+if TYPE_CHECKING:
+    from .player import Player
+    from .tracks import *
+    from .types.request import Request
+    from .ext import spotify as spotify_
+
+    PlayableT = TypeVar('PlayableT', bound=Playable)
+    
+
+__all__ = ('Node', 'NodePool')
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+# noinspection PyShadowingBuiltins
+class Node:
+    """The base Wavelink Node.
+
+    The Node is responsible for keeping the Websocket alive, tracking the state of Players
+    and fetching/decoding Tracks and Playlists.
+
+    .. note::
+
+        The Node class should only be created once per Lavalink connection.
+        To retrieve a Node use the appropriate :class:`NodePool` methods instead.
+
+    .. warning::
+
+        The Node will not be connected until passed to :meth:`NodePool.connect`.
+
+
+    .. container:: operations
+
+        .. describe:: repr(node)
+
+            Returns an official string representation of this Node.
+
+
+    Parameters
+    ----------
+    id: Optional[str]
+        The unique identifier for this Node. If not passed, one will be generated randomly.
+    uri: str
+        The uri to connect to your Lavalink server. E.g ``http://localhost:2333``.
+    password: str
+        The password used to connect to your Lavalink server.
+    secure: Optional[bool]
+        Whether the connection should use https/wss.
+    use_http: Optional[bool]
+        Whether to use http:// over ws:// when connecting to the Lavalink websocket. Defaults to False.
+    session: Optional[aiohttp.ClientSession]
+        The session to use for this Node. If no session is passed a default will be used.
+    heartbeat: float
+        The time in seconds to send a heartbeat ack. Defaults to 15.0.
+    retries: Optional[int]
+        The amount of times this Node will try to reconnect after a disconnect.
+        If not set the Node will try unlimited times.
+
+    Attributes
+    ----------
+    heartbeat: float
+        The time in seconds to send a heartbeat ack. Defaults to 15.0.
+    client: :class:`discord.Client`
+        The discord client used to connect this Node. Could be None if this Node has not been connected.
+    """
+
+    def __init__(
+            self,
+            *,
+            id: str | None = None,
+            uri: str,
+            password: str,
+            secure: bool = False,
+            use_http: bool = False,
+            session: aiohttp.ClientSession = MISSING,
+            heartbeat: float = 15.0,
+            retries: int | None = None,
+    ) -> None:
+        if id is None:
+            id = ''.join(random.sample(string.ascii_letters + string.digits, 12))
+
+        self._id: str = id
+        self._uri: str = uri
+        self._secure: bool = secure
+        self._use_http: bool = use_http
+        host: str = re.sub(r'(?:http|ws)s?://', '', self._uri)
+        self._host: str = f'{"https://" if secure else "http://"}{host}'
+        self._password: str = password
+
+        self._session: aiohttp.ClientSession = session
+        self.heartbeat: float = heartbeat
+        self._retries: int | None = retries
+
+        self.client: discord.Client | None = None
+        self._websocket: Websocket = MISSING
+        self._session_id: str | None = None
+
+        self._players: dict[int, Player] = {}
+        self._invalidated: dict[int, Player] = {}
+
+        self._status: NodeStatus = NodeStatus.DISCONNECTED
+        self._major_version: int | None = None
+
+        self._spotify: spotify_.SpotifyClient | None = None
+
+    def __repr__(self) -> str:
+        return f'Node(id="{self._id}", uri="{self.uri}", status={self.status})'
+
+    def __eq__(self, other: object) -> bool:
+        return self.id == other.id if isinstance(other, Node) else NotImplemented
+
+    @property
+    def id(self) -> str:
+        """The Nodes unique identifier."""
+        return self._id
+
+    @property
+    def uri(self) -> str:
+        """The URI used to connect this Node to Lavalink."""
+        return self._host
+
+    @property
+    def password(self) -> str:
+        """The password used to connect this Node to Lavalink."""
+        return self._password
+
+    @property
+    def players(self) -> dict[int, Player]:
+        """A mapping of Guild ID to Player."""
+        return self._players
+
+    @property
+    def status(self) -> NodeStatus:
+        """The connection status of this Node.
+
+        DISCONNECTED
+        CONNECTING
+        CONNECTED
+        """
+        return self._status
+
+    def get_player(self, guild_id: int, /) -> Player | None:
+        """Return the :class:`player.Player` associated with the provided guild ID.
+
+        If no :class:`player.Player` is found, returns None.
+
+        Parameters
+        ----------
+        guild_id: int
+            The Guild ID to return a Player for.
+
+        Returns
+        -------
+        Optional[:class:`player.Player`]
+        """
+        return self._players.get(guild_id, None)
+
+    async def _connect(self, client: discord.Client) -> None:
+        if client.user is None:
+            raise RuntimeError('')
+
+        if not self._session:
+            self._session = aiohttp.ClientSession(headers={'Authorization': self._password})
+
+        self.client = client
+
+        self._websocket = Websocket(node=self)
+
+        await self._websocket.connect()
+
+        async with self._session.get(f'{self._host}/version') as resp:
+            version: str = await resp.text()
+
+            if version.endswith('-SNAPSHOT'):
+                self._major_version = 3
+                return
+
+            try:
+                version_tuple = tuple(int(v) for v in version.split('.'))
+            except ValueError:
+                logging.warning(f'Lavalink "{version}" is unknown and may not be compatible with: '
+                                f'Wavelink "{__version__}". Wavelink is assuming the Lavalink version.')
+
+                self._major_version = 3
+                return
+
+            if version_tuple[0] < 3:
+                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with Lavalink "{version}".')
+
+            if version_tuple[0] == 3 and version_tuple[1] < 7:
+                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with '
+                                             f'Lavalink versions under "3.7".')
+
+            self._major_version = version_tuple[0]
+            logger.info(f'Lavalink version "{version}" connected for Node: {self.id}')
+
+    async def _send(self,
+                    *,
+                    method: str,
+                    path: str,
+                    guild_id: int | str | None = None,
+                    query: str | None = None,
+                    data: Request | None = None,
+                    ) -> dict[str, Any] | None:
+
+        uri: str = f'{self._host}/' \
+                   f'v{self._major_version}/' \
+                   f'{path}' \
+                   f'{f"/{guild_id}" if guild_id else ""}' \
+                   f'{f"?{query}" if query else ""}'
+
+        logger.debug(f'Node {self} is sending payload to [{method}] "{uri}" with payload: {data}')
+
+        async with self._session.request(method=method, url=uri, json=data or {}) as resp:
+            rdata: dict[str | int, Any] | None = None
+
+            if resp.content_type == 'application/json':
+                rdata = await resp.json()
+
+            logger.debug(f'Node {self} received payload from Lavalink after sending to "{uri}" with response: '
+                         f'<status={resp.status}, data={rdata}>')
+
+            if resp.status >= 300:
+                raise InvalidLavalinkResponse(f'An error occurred when attempting to reach: "{uri}".',
+                                              status=resp.status)
+
+            if resp.status == 204:
+                return
+
+            return rdata
+
+    async def get_tracks(self, cls: type[PlayableT], query: str) -> list[PlayableT]:
+        """|coro|
+
+        Search for and retrieve Tracks based on the query and cls provided.
+
+        .. note::
+
+            If the query is not a Local search or direct URL, you will need to provide a search prefix.
+            E.g. ``ytsearch:`` for a YouTube search.
+
+        Parameters
+        ----------
+        cls: type[PlayableT]
+            The type of Playable tracks that should be returned.
+        query: str
+            The query to search for and return tracks.
+
+        Returns
+        -------
+        list[PlayableT]
+            A list of found tracks converted to the provided cls.
+        """
+        logger.debug(f'Node {self} is requesting tracks with query "{query}".')
+
+        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
+        load_type = try_enum(LoadType, data.get("loadType"))
+
+        if load_type is LoadType.load_failed:
+            # TODO - Proper Exception...
+
+            raise ValueError('Track Failed to load.')
+
+        if load_type is LoadType.no_matches:
+            return []
+
+        if load_type is LoadType.track_loaded:
+            track_data = data["tracks"][0]
+            return [cls(track_data)]
+
+        if load_type is not LoadType.search_result:
+            # TODO - Proper Exception...
+
+            raise ValueError('Track Failed to load.')
+
+        return [cls(track_data) for track_data in data["tracks"]]
+
+    async def get_playlist(self, cls: Playlist, query: str):
+        """|coro|
+
+        Search for and return a :class:`tracks.Playlist` given an identifier.
+
+        Parameters
+        ----------
+        cls: Type[:class:`tracks.Playlist`]
+            The type of which playlist should be returned, this must subclass :class:`tracks.Playlist`.
+        query: str
+            The playlist's identifier. This may be a YouTube playlist URL for example.
+
+        Returns
+        -------
+        Optional[:class:`tracks.Playlist`]:
+            The related wavelink track object or ``None`` if none was found.
+
+        Raises
+        ------
+        ValueError
+            Loading the playlist failed.
+        WavelinkException
+            An unspecified error occurred when loading the playlist.
+        """
+        logger.debug(f'Node {self} is requesting a playlist with query "{query}".')
+
+        encoded_query = urllib.parse.quote(query)
+        data = await self._send(method='GET', path='loadtracks', query=f'identifier={encoded_query}')
+
+        load_type = try_enum(LoadType, data.get("loadType"))
+
+        if load_type is LoadType.load_failed:
+            # TODO Proper exception...
+            raise ValueError('Tracks failed to Load.')
+
+        if load_type is LoadType.no_matches:
+            return None
+
+        if load_type is not LoadType.playlist_loaded:
+            raise WavelinkException("Track failed to load.")
+
+        return cls(data)
+
+    async def build_track(self, *, cls: type[PlayableT], encoded: str) -> PlayableT:
+        """|coro|
+
+        Build a track from the provided encoded string with the given Track class.
+
+        Parameters
+        ----------
+        cls: type[PlayableT]
+            The type of Playable track that should be returned.
+        encoded: str
+            The Tracks unique encoded string.
+        """
+        encoded_query = urllib.parse.quote(encoded)
+        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
+
+        logger.debug(f'Node {self} built encoded track with encoding "{encoded}". Response data: {data}')
+        return cls(data=data)
+
+
+# noinspection PyShadowingBuiltins
+class NodePool:
+    """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
+
+    Attributes
+    ----------
+    nodes: dict[str, :class:`Node`]
+        A mapping of :class:`Node` identifier to :class:`Node`.
+
+
+    .. warning::
+
+        This class should never be initialised. All methods are class methods.
+    """
+
+    __nodes: dict[str, Node] = {}
+
+    @classmethod
+    async def connect(
+            cls,
+            *,
+            client: discord.Client,
+            nodes: list[Node],
+            spotify: spotify_.SpotifyClient | None = None
+    ) -> dict[str, Node]:
+        """|coro|
+
+        Connect a list of Nodes.
+
+        Parameters
+        ----------
+        client: :class:`discord.Client`
+            The discord Client or Bot used to connect the Nodes.
+        nodes: list[:class:`Node`]
+            A list of Nodes to connect.
+        spotify: Optional[:class:`ext.spotify.SpotifyClient`]
+            The spotify Client to use when searching for Spotify Tracks.
+
+        Returns
+        -------
+        dict[str, :class:`Node`]
+            A mapping of :class:`Node` identifier to :class:`Node`.
+        """
+        if client.user is None:
+            raise RuntimeError('')
+
+        for node in nodes:
+
+            if spotify:
+                node._spotify = spotify
+
+            if node.id in cls.__nodes:
+                logger.error(f'A Node with the ID "{node.id}" already exists on the NodePool. Disregarding.')
+                continue
+
+            try:
+                await node._connect(client)
+            except AuthorizationFailed:
+                logger.error(f'The Node <{node!r}> failed to authenticate properly. '
+                             f'Please check your password and try again.')
+            else:
+                cls.__nodes[node.id] = node
+
+        return cls.nodes
+
+    @classproperty
+    def nodes(cls) -> dict[str, Node]:
+        """A mapping of :class:`Node` identifier to :class:`Node`."""
+        return cls.__nodes
+
+    @classmethod
+    def get_node(cls, id: str | None = None) -> Node:
+        """Retrieve a :class:`Node` with the given ID or best, if no ID was passed.
+
+        Parameters
+        ----------
+        id: Optional[str]
+            The unique identifier of the :class:`Node` to retrieve. If not passed the best :class:`Node`
+            will be fetched.
+
+        Returns
+        -------
+        :class:`Node`
+
+        Raises
+        ------
+        InvalidNode
+            The given id does nto resolve to a :class:`Node` or no :class:`Node` has been connected.
+        """
+        if id:
+            if id not in cls.__nodes:
+                raise InvalidNode(f'A Node with ID "{id}" does not exist on the Wavelink NodePool.')
+
+            return cls.__nodes[id]
+
+        if not cls.__nodes:
+            raise InvalidNode('No Node currently exists on the Wavelink NodePool.')
+
+        nodes = cls.__nodes.values()
+        return sorted(nodes, key=lambda n: len(n.players))[0]
+
+    @classmethod
+    def get_connected_node(cls) -> Node:
+        """Get the best available connected :class:`Node`.
+
+        Returns
+        -------
+        :class:`Node`
+            The best available connected Node.
+
+        Raises
+        ------
+        InvalidNode
+            No Nodes are currently in the connected state.
+        """
+
+        nodes: list[Node] = [n for n in cls.__nodes.values() if n.status is NodeStatus.CONNECTED]
+        if not nodes:
+            raise InvalidNode('There are no Nodes on the Wavelink NodePool that are currently in the connected state.')
+
+        return sorted(nodes, key=lambda n: len(n.players))[0]
+
+    @classmethod
+    async def get_tracks(cls_,  # type: ignore
+                         query: str,
+                         /,
+                         *,
+                         cls: type[PlayableT],
+                         node: Node | None = None
+                         ) -> list[PlayableT]:
+        """|coro|
+
+        Helper method to retrieve tracks from the NodePool without fetching a :class:`Node`.
+
+        Parameters
+        ----------
+        query: str
+            The query to search for and return tracks.
+        cls: type[PlayableT]
+            The type of Playable tracks that should be returned.
+        node: Optional[:class:`Node`]
+            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
+            Defaults to None.
+
+        Returns
+        -------
+        list[PlayableT]
+            A list of found tracks converted to the provided cls.
+        """
+        if not node:
+            node = cls_.get_connected_node()
+
+        return await node.get_tracks(cls=cls, query=query)
+
+    @classmethod
+    async def get_playlist(cls_,  # type: ignore
+                           query: str,
+                           /,
+                           *,
+                           cls: Playlist,
+                           node: Node | None = None
+                           ) -> Playlist:
+        """|coro|
+
+        Helper method to retrieve a playlist from the NodePool without fetching a :class:`Node`.
+
+
+        .. warning::
+
+            The only playlists currently supported are :class:`tracks.YouTubePlaylist` and
+            :class:`tracks.YouTubePlaylist`.
+
+
+        Parameters
+        ----------
+        query: str
+            The query to search for and return a playlist.
+        cls: type[PlayableT]
+            The type of Playlist that should be returned.
+        node: Optional[:class:`Node`]
+            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
+            Defaults to None.
+
+        Returns
+        -------
+        Playlist
+            A Playlist with its tracks.
+        """
+        if not node:
+            node = cls_.get_connected_node()
+
+        return await node.get_playlist(cls=cls, query=query)
```

### Comparing `Wavelink-2.6.0/wavelink/payloads.py` & `wavelink-2.6.1/wavelink/payloads.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Any
-
-from discord.enums import try_enum
-
-from .enums import TrackEventType, DiscordVoiceCloseType
-
-if TYPE_CHECKING:
-    from .player import Player
-    from .tracks import Playable
-    from .types.events import EventOp
-
-__all__ = ('TrackEventPayload', 'WebsocketClosedPayload')
-
-
-class TrackEventPayload:
-    """The Wavelink Track Event Payload.
-
-    .. warning::
-
-        This class should not be created manually, instead you will receive it from the
-        various wavelink track events.
-
-    Attributes
-    ----------
-    event: :class:`TrackEventType`
-        An enum of the type of event.
-    track: :class:`Playable`
-        The track associated with this event.
-    original: Optional[:class:`Playable`]
-        The original requested track before conversion. Could be None.
-    player: :class:`player.Player`
-        The player associated with this event.
-    reason: Optional[str]
-        The reason this event was fired.
-    """
-
-    def __init__(self, *, data: EventOp, track: Playable, original: Playable | None, player: Player) -> None:
-        self.event: TrackEventType = try_enum(TrackEventType, data['type'])
-        self.track: Playable = track
-        self.original: Playable | None = original
-        self.player: Player = player
-
-        self.reason: str = data.get('reason')
-
-
-class WebsocketClosedPayload:
-    """The Wavelink WebsocketClosed Event Payload.
-
-    .. warning::
-
-        This class should not be created manually, instead you will receive it from the
-        wavelink `on_wavelink_websocket_closed` event.
-
-    Attributes
-    ----------
-    code: :class:`DiscordVoiceCloseType`
-        An Enum representing the close code from Discord.
-    reason: Optional[str]
-        The reason the Websocket was closed.
-    by_discord: bool
-        Whether the websocket was closed by Discord.
-    player: :class:`player.Player`
-        The player associated with this event.
-    """
-
-    def __init__(self, *, data: dict[str, Any], player: Player) -> None:
-        self.code: DiscordVoiceCloseType = try_enum(DiscordVoiceCloseType, data['code'])
-        self.reason: str = data.get('reason')
-        self.by_discord: bool = data.get('byRemote')
-        self.player: Player = player
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
+
+from discord.enums import try_enum
+
+from .enums import TrackEventType, DiscordVoiceCloseType
+
+if TYPE_CHECKING:
+    from .player import Player
+    from .tracks import Playable
+    from .types.events import EventOp
+
+__all__ = ('TrackEventPayload', 'WebsocketClosedPayload')
+
+
+class TrackEventPayload:
+    """The Wavelink Track Event Payload.
+
+    .. warning::
+
+        This class should not be created manually, instead you will receive it from the
+        various wavelink track events.
+
+    Attributes
+    ----------
+    event: :class:`TrackEventType`
+        An enum of the type of event.
+    track: :class:`Playable`
+        The track associated with this event.
+    original: Optional[:class:`Playable`]
+        The original requested track before conversion. Could be None.
+    player: :class:`player.Player`
+        The player associated with this event.
+    reason: Optional[str]
+        The reason this event was fired.
+    """
+
+    def __init__(self, *, data: EventOp, track: Playable, original: Playable | None, player: Player) -> None:
+        self.event: TrackEventType = try_enum(TrackEventType, data['type'])
+        self.track: Playable = track
+        self.original: Playable | None = original
+        self.player: Player = player
+
+        self.reason: str = data.get('reason')
+
+
+class WebsocketClosedPayload:
+    """The Wavelink WebsocketClosed Event Payload.
+
+    .. warning::
+
+        This class should not be created manually, instead you will receive it from the
+        wavelink `on_wavelink_websocket_closed` event.
+
+    Attributes
+    ----------
+    code: :class:`DiscordVoiceCloseType`
+        An Enum representing the close code from Discord.
+    reason: Optional[str]
+        The reason the Websocket was closed.
+    by_discord: bool
+        Whether the websocket was closed by Discord.
+    player: :class:`player.Player`
+        The player associated with this event.
+    """
+
+    def __init__(self, *, data: dict[str, Any], player: Player) -> None:
+        self.code: DiscordVoiceCloseType = try_enum(DiscordVoiceCloseType, data['code'])
+        self.reason: str = data.get('reason')
+        self.by_discord: bool = data.get('byRemote')
+        self.player: Player = player
```

### Comparing `Wavelink-2.6.0/wavelink/player.py` & `wavelink-2.6.1/wavelink/player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,825 +1,828 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import datetime
-import logging
-from typing import TYPE_CHECKING, Any, Union
-
-import discord
-from discord.utils import MISSING
-
-from .enums import *
-from .exceptions import *
-from .ext import spotify
-from .filters import Filter
-from .node import Node, NodePool
-from .payloads import TrackEventPayload
-from .queue import Queue
-from .tracks import *
-
-
-if TYPE_CHECKING:
-    from discord.types.voice import GuildVoiceState, VoiceServerUpdate
-    from typing_extensions import Self
-
-    from .types.events import PlayerState, PlayerUpdateOp
-    from .types.request import EncodedTrackRequest, Request
-    from .types.state import DiscordVoiceState
-
-__all__ = ("Player",)
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-VoiceChannel = Union[
-    discord.VoiceChannel, discord.StageChannel
-]  # todo: VocalGuildChannel?
-
-
-class Player(discord.VoiceProtocol):
-    """Wavelink Player class.
-
-    This class is used as a :class:`~discord.VoiceProtocol` and inherits all its members.
-
-    You must pass this class to :meth:`discord.VoiceChannel.connect` with ``cls=...``. This ensures the player is
-    set up correctly and put into the discord.py voice client cache.
-
-    You **can** make an instance of this class *before* passing it to
-    :meth:`discord.VoiceChannel.connect` with ``cls=...``, but you **must** still pass it.
-
-    Once you have connected this class you do not need to store it anywhere as it will be stored on the
-    :class:`~wavelink.Node` and in the discord.py voice client cache. Meaning you can access this player where you
-    have access to a :class:`~wavelink.NodePool`, the specific :class:`~wavelink.Node` or a :class:`~discord.Guild`
-    including in :class:`~discord.ext.commands.Context` and :class:`~discord.Interaction`.
-
-    Examples
-    --------
-
-    .. code:: python3
-
-        # Connect the player...
-        player: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
-
-        # Retrieve the player later...
-        player: wavelink.Player = ctx.guild.voice_client
-
-
-    .. note::
-
-        The Player class comes with an in-built queue. See :class:`queue.Queue` for more information on how this queue
-        works.
-
-    Parameters
-    ----------
-    nodes: Optional[list[:class:`node.Node`]]
-        An optional list of :class:`node.Node` to use with this Player. If no Nodes are provided
-        the best connected Node will be used.
-    swap_node_on_disconnect: bool
-        If a list of :class:`node.Node` is provided the Player will swap Nodes on Node disconnect.
-        Defaults to True.
-
-    Attributes
-    ----------
-    client: :class:`discord.Client`
-        The discord Client or Bot associated with this Player.
-    channel: :class:`discord.VoiceChannel`
-        The channel this player is currently connected to.
-    nodes: list[:class:`node.Node`]
-        The list of Nodes this player is currently using.
-    current_node: :class:`node.Node`
-        The Node this player is currently using.
-    queue: :class:`queue.Queue`
-        The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
-        Meaning any songs in this queue will be played before auto_queue songs.
-    auto_queue: :class:`queue.Queue`
-        The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
-        When a song is retrieved from this queue in the AutoPlay event,
-        it is added to the main :attr:`wavelink.Queue.history` queue.
-    """
-
-    def __call__(self, client: discord.Client, channel: VoiceChannel) -> Self:
-        self.client = client
-        self.channel = channel
-
-        return self
-
-    def __init__(
-        self,
-        client: discord.Client = MISSING,
-        channel: VoiceChannel = MISSING,
-        *,
-        nodes: list[Node] | None = None,
-        swap_node_on_disconnect: bool = True
-    ) -> None:
-        self.client: discord.Client = client
-        self.channel: VoiceChannel | None = channel
-
-        self.nodes: list[Node]
-        self.current_node: Node
-
-        if swap_node_on_disconnect and not nodes:
-            nodes = list(NodePool.nodes.values())
-            self.nodes = sorted(nodes, key=lambda n: len(n.players))
-            self.current_node = self.nodes[0]
-        elif nodes:
-            nodes = sorted(nodes, key=lambda n: len(n.players))
-            self.current_node = nodes[0]
-            self.nodes = nodes
-        else:
-            self.current_node = NodePool.get_connected_node()
-            self.nodes = [self.current_node]
-
-        if not self.client:
-            if self.current_node.client is None:
-                raise RuntimeError('')
-            self.client = self.current_node.client
-
-        self._guild: discord.Guild | None = None
-        self._voice_state: DiscordVoiceState = {}
-        self._player_state: dict[str, Any] = {}
-
-        self.swap_on_disconnect: bool = swap_node_on_disconnect
-
-        self.last_update: datetime.datetime | None = None
-        self.last_position: int = 0
-
-        self._ping: int = 0
-
-        self.queue: Queue = Queue()
-        self._current: Playable | None = None
-        self._original: Playable | None = None
-
-        self._volume: int = 50
-        self._paused: bool = False
-
-        self._track_seeds: list[str] = []
-        self._autoplay: bool = False
-        self.auto_queue: Queue = Queue()
-        self._auto_threshold: int = 100
-        self._filter: Filter | None = None
-
-        self._destroyed: bool = False
-
-    async def _auto_play_event(self, payload: TrackEventPayload) -> None:
-        logger.debug(f'Player {self.guild.id} entered autoplay event.')
-
-        if not self.autoplay:
-            logger.debug(f'Player {self.guild.id} autoplay is set to False. Exiting autoplay event.')
-            return
-
-        if payload.reason == 'REPLACED':
-            logger.debug(f'Player {self.guild.id} autoplay reason is REPLACED. Exiting autoplay event.')
-            return
-
-        if self.queue.loop:
-            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True.')
-
-            try:
-                track = self.queue.get()
-            except QueueEmpty:
-                logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True '
-                             f'but no track was available. Exiting autoplay event.')
-                return
-
-            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True. Looping track "{track}"')
-            await self.play(track)
-            return
-
-        if self.queue:
-            track = self.queue.get()
-
-            populate = len(self.auto_queue) < self._auto_threshold
-            await self.play(track, populate=populate)
-
-            logger.debug(f'Player {self.guild.id} autoplay found track in default queue, populate={populate}.')
-            return
-
-        if self.queue.loop_all:
-            await self.play(self.queue.get())
-            return
-
-        if not self.auto_queue:
-            logger.debug(f'Player {self.guild.id} has no auto queue. Exiting autoplay event.')
-            return
-
-        await self.queue.put_wait(await self.auto_queue.get_wait())
-        populate = self.auto_queue.is_empty
-
-        track = await self.queue.get_wait()
-        await self.play(track, populate=populate)
-
-        logger.debug(f'Player {self.guild.id} playing track "{track}" from autoplay with populate={populate}.')
-
-    @property
-    def autoplay(self) -> bool:
-        """Returns a ``bool`` indicating whether the :class:`~Player` is in AutoPlay mode or not.
-
-        This property can be set to ``True`` or ``False``.
-
-        When ``autoplay`` is ``True``, the player will automatically handle fetching and playing the next track from
-        the queue. It also searches tracks in the ``auto_queue``, a special queue populated with recommended tracks,
-        from the Spotify API or YouTube Recommendations.
-
-
-        .. note::
-
-            You can still use the :func:`~wavelink.on_wavelink_track_end` event when ``autoplay`` is ``True``,
-            but it is recommended to **not** do any queue logic or invoking play from this event.
-
-            Most users are able to use ``autoplay`` and :func:`~wavelink.on_wavelink_track_start` together to handle
-            their logic. E.g. sending a message when a track starts playing.
-
-
-        .. note::
-
-            The ``auto_queue`` will be populated when you play a :class:`~wavelink.ext.spotify.SpotifyTrack` or
-            :class:`~wavelink.YouTubeTrack`, and have initially set ``populate`` to ``True`` in
-            :meth:`~wavelink.Player.play`. See :meth:`~wavelink.Player.play` for more info.
-
-
-        .. versionadded:: 2.0
-
-
-        .. versionchanged:: 2.6.0
-
-            The autoplay event now populates the ``auto_queue`` when playing :class:`~wavelink.YouTubeTrack` **or**
-            :class:`~wavelink.ext.spotify.SpotifyTrack`.
-        """
-        return self._autoplay
-
-    @autoplay.setter
-    def autoplay(self, value: bool) -> None:
-        """Set AutoPlay to True or False."""
-        self._autoplay = value
-
-    def is_connected(self) -> bool:
-        """Whether the player is connected to a voice channel."""
-        return self.channel is not None and self.channel is not MISSING
-
-    def is_playing(self) -> bool:
-        """Whether the Player is currently playing a track."""
-        return self.current is not None
-
-    def is_paused(self) -> bool:
-        """Whether the Player is currently paused."""
-        return self._paused
-
-    @property
-    def volume(self) -> int:
-        """The current volume of the Player."""
-        return self._volume
-
-    @property
-    def guild(self) -> discord.Guild | None:
-        """The discord Guild associated with the Player."""
-        return self._guild
-
-    @property
-    def position(self) -> float:
-        """The position of the currently playing track in milliseconds."""
-
-        if not self.is_playing():
-            return 0
-
-        if self.is_paused():
-            return min(self.last_position, self.current.duration)  # type: ignore
-
-        delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
-        position = self.last_position + delta
-
-        return min(position, self.current.duration)
-
-    @property
-    def ping(self) -> int:
-        """The ping to the discord endpoint in milliseconds.
-
-        .. versionadded:: 2.0
-        """
-        return self._ping
-
-    @property
-    def current(self) -> Playable | None:
-        """The currently playing Track if there is one.
-
-        Could be ``None`` if no Track is playing.
-        """
-        return self._current
-
-    @property
-    def filter(self) -> dict[str, Any]:
-        """The currently applied filter."""
-        return self._filter._payload
-
-    async def _update_event(self, data: PlayerUpdateOp | None) -> None:
-        assert self._guild is not None
-
-        if data is None: 
-            if self.swap_on_disconnect:
-
-                if len(self.nodes) < 2:
-                    return
-
-                new: Node = [n for n in self.nodes if n != self.current_node and n.status is NodeStatus.CONNECTED][0]
-                del self.current_node._players[self._guild.id]
-
-                if not new:
-                    return
-
-                self.current_node: Node = new
-                new._players[self._guild.id] = self
-
-                await self._dispatch_voice_update()
-                await self._swap_state()
-            return
-
-        data.pop('op')  # type: ignore
-        self._player_state.update(**data)
-
-        state: PlayerState = data['state']
-        self.last_update = datetime.datetime.fromtimestamp(state.get("time", 0) / 1000, datetime.timezone.utc)
-        self.last_position = state.get('position', 0)
-
-        self._ping = state['ping']
-
-    async def on_voice_server_update(self, data: VoiceServerUpdate) -> None:
-        """|coro|
-
-        An abstract method that is called when initially connecting to voice. This corresponds to VOICE_SERVER_UPDATE.
-
-        .. warning::
-
-            Do not override this method.
-        """
-        self._voice_state['token'] = data['token']
-        self._voice_state['endpoint'] = data['endpoint']
-
-        await self._dispatch_voice_update()
-
-    async def on_voice_state_update(self, data: GuildVoiceState) -> None:
-        """|coro|
-
-        An abstract method that is called when the client’s voice state has changed.
-        This corresponds to VOICE_STATE_UPDATE.
-
-        .. warning::
-
-            Do not override this method.
-        """
-        assert self._guild is not None
-
-        channel_id = data["channel_id"]
-
-        if not channel_id:
-            await self._destroy()
-            return
-
-        self._voice_state['session_id'] = data['session_id']
-        self.channel = self.client.get_channel(int(channel_id))  # type: ignore
-
-        if not self._guild:
-            self._guild = self.channel.guild  # type: ignore
-            assert self._guild is not None
-            self.current_node._players[self._guild.id] = self
-
-    async def _dispatch_voice_update(self, data: DiscordVoiceState | None = None) -> None:
-        assert self._guild is not None
-
-        data = data or self._voice_state
-
-        try:
-            session_id: str = data['session_id']
-            token: str = data['token']
-            endpoint: str = data['endpoint']
-        except KeyError:
-            return
-
-        voice: Request = {'voice': {'sessionId': session_id, 'token': token, 'endpoint': endpoint}}
-        self._player_state.update(**voice)
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=voice)
-
-        logger.debug(f'Player {self.guild.id} is dispatching VOICE_UPDATE: {resp}')
-
-    def _connection_check(self, channel: VoiceChannel) -> None:
-        if channel.permissions_for(channel.guild.me).administrator:
-            return
-
-        if not channel.permissions_for(channel.guild.me).connect:
-            logger.debug(f'Player tried connecting to channel "{channel.id}", but does not have correct permissions.')
-
-            raise InvalidChannelPermissions('You do not have connect permissions to join this channel.')
-
-        limit: int = channel.user_limit
-        total: int = len(channel.members)
-
-        if limit == 0:
-            pass
-
-        elif total >= limit:
-            msg: str = f'There are currently too many users in this channel. <{total}/{limit}>'
-            logger.debug(f'Player tried connecting to channel "{channel.id}", but the it is full. <{total}/{limit}>')
-
-            raise InvalidChannelPermissions(msg)
-
-    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
-        if self.channel is None:
-            self._invalidate(before_connect=True)
-
-            msg: str = 'Please use the method "discord.VoiceChannel.connect" and pass this player to cls='
-            logger.debug(f'Player tried connecting without a channel. {msg}')
-
-            raise InvalidChannelStateError(msg)
-
-        if not self._guild:
-            self._guild = self.channel.guild
-            self.current_node._players[self._guild.id] = self
-
-        try:
-            self._connection_check(self.channel)
-        except InvalidChannelPermissions as e:
-            self._invalidate(before_connect=True)
-            raise e
-
-        await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
-        logger.info(f'Player {self.guild.id} connected to channel: {self.channel}')
-
-    async def move_to(self, channel: discord.VoiceChannel) -> None:
-        """|coro|
-
-        Moves the player to a different voice channel.
-
-        Parameters
-        -----------
-        channel: :class:`discord.VoiceChannel`
-            The channel to move to. Must be a voice channel.
-        """
-        self._connection_check(channel)
-
-        await self.guild.change_voice_state(channel=channel)
-        logger.info(f'Player {self.guild.id} moved to channel: {channel}')
-
-    async def play(self,
-                   track: Playable | spotify.SpotifyTrack,
-                   replace: bool = True,
-                   start: int | None = None,
-                   end: int | None = None,
-                   volume: int | None = None,
-                   *,
-                   populate: bool = False
-                   ) -> Playable:
-        """|coro|
-
-        Play a WaveLink Track.
-
-        Parameters
-        ----------
-        track: :class:`tracks.Playable`
-            The :class:`tracks.Playable` or :class:`~wavelink.ext.spotify.SpotifyTrack` track to start playing.
-        replace: bool
-            Whether this track should replace the current track. Defaults to ``True``.
-        start: Optional[int]
-            The position to start the track at in milliseconds.
-            Defaults to ``None`` which will start the track at the beginning.
-        end: Optional[int]
-            The position to end the track at in milliseconds.
-            Defaults to ``None`` which means it will play until the end.
-        volume: Optional[int]
-            Sets the volume of the player. Must be between ``0`` and ``1000``.
-            Defaults to ``None`` which will not change the volume.
-        populate: bool
-            Whether to populate the AutoPlay queue. Defaults to ``False``.
-
-            .. versionadded:: 2.0
-
-        Returns
-        -------
-        :class:`~tracks.Playable`
-            The track that is now playing.
-
-
-        .. note::
-
-            If you pass a :class:`~wavelink.YouTubeTrack` **or** :class:`~wavelink.ext.spotify.SpotifyTrack` and set
-            ``populate=True``, **while** :attr:`~wavelink.Player.autoplay` is set to ``True``, this method will populate
-            the ``auto_queue`` with recommended songs. When the ``auto_queue`` is low on tracks this method will
-            automatically populate the ``auto_queue`` with more tracks, and continue this cycle until either the
-            player has been disconnected or :attr:`~wavelink.Player.autoplay` is set to ``False``.
-
-
-        Example
-        -------
-
-        .. code:: python3
-
-            tracks: list[wavelink.YouTubeTrack] = await wavelink.YouTubeTrack.search(...)
-            if not tracks:
-                # Do something as no tracks were found...
-                return
-
-            await player.queue.put_wait(tracks[0])
-
-            if not player.is_playing():
-                await player.play(player.queue.get(), populate=True)
-
-
-        .. versionchanged:: 2.6.0
-
-            This method now accepts :class:`~wavelink.YouTubeTrack` or :class:`~wavelink.ext.spotify.SpotifyTrack`
-            when populating the ``auto_queue``.
-        """
-        assert self._guild is not None
-
-        if isinstance(track, YouTubeTrack) and self.autoplay and populate:
-            query: str = f'https://www.youtube.com/watch?v={track.identifier}&list=RD{track.identifier}'
-
-            recos: YouTubePlaylist = await self.current_node.get_playlist(query=query, cls=YouTubePlaylist)
-            recos: list[YouTubeTrack] = getattr(recos, 'tracks', [])
-
-            queues = set(self.queue) | set(self.auto_queue) | set(self.auto_queue.history) | {track}
-
-            for track_ in recos:
-                if track_ in queues:
-                    continue
-
-                await self.auto_queue.put_wait(track_)
-
-            self.auto_queue.shuffle()
-
-        elif isinstance(track, spotify.SpotifyTrack):
-            original = track
-            track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
-
-            if populate:
-                self.auto_queue.shuffle()
-
-            for attr, value in original.__dict__.items():
-                if hasattr(track, attr):
-                    logger.warning(f'Player {self.guild.id} was unable to set attribute "{attr}" '
-                                   f'when converting a SpotifyTrack as it conflicts with the new track type.')
-                    continue
-
-                setattr(track, attr, value)
-
-        data = {
-            'encodedTrack': track.encoded,
-            'position': start or 0,
-            'volume': volume or self._volume
-        }
-
-        if end:
-            data['endTime'] = end
-
-        self._current = track
-        self._original = track
-
-        try:
-
-            resp: dict[str, Any] = await self.current_node._send(
-                method='PATCH',
-                path=f'sessions/{self.current_node._session_id}/players',
-                guild_id=self._guild.id,
-                data=data,
-                query=f'noReplace={not replace}'
-            )
-
-        except InvalidLavalinkResponse as e:
-            self._current = None
-            self._original = None
-            logger.debug(f'Player {self._guild.id} attempted to load track: {track}, but failed: {e}')
-            raise e
-
-        self._player_state['track'] = resp['track']['encoded']
-
-        if not (self.queue.loop and self.queue._loaded):
-            self.queue.history.put(track)
-
-        self.queue._loaded = track
-
-        logger.debug(f'Player {self._guild.id} loaded and started playing track: {track}.')
-        return track
-
-    async def set_volume(self, value: int) -> None:
-        """|coro|
-
-        Set the Player volume.
-
-        Parameters
-        ----------
-        value: int
-            A volume value between 0 and 1000.
-        """
-        assert self._guild is not None
-
-        self._volume = max(min(value, 1000), 0)
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'volume': self._volume})
-
-        logger.debug(f'Player {self.guild.id} volume was set to {self._volume}.')
-
-    async def seek(self, position: int) -> None:
-        """|coro|
-
-        Seek to the provided position, in milliseconds.
-
-        Parameters
-        ----------
-        position: int
-            The position to seek to in milliseconds.
-        """
-        if not self._current:
-            return
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'position': position})
-
-        logger.debug(f'Player {self.guild.id} seeked current track to position {position}.')
-
-    async def pause(self) -> None:
-        """|coro|
-
-        Pauses the Player.
-        """
-        assert self._guild is not None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'paused': True})
-
-        self._paused = True
-        logger.debug(f'Player {self.guild.id} was paused.')
-
-    async def resume(self) -> None:
-        """|coro|
-
-        Resumes the Player.
-        """
-        assert self._guild is not None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'paused': False})
-
-        self._paused = False
-        logger.debug(f'Player {self.guild.id} was resumed.')
-
-    async def stop(self, *, force: bool = True) -> None:
-        """|coro|
-
-        Stops the currently playing Track.
-
-        Parameters
-        ----------
-        force: Optional[bool]
-            Whether to stop the currently playing track and proceed to the next regardless if :attr:`~Queue.loop`
-            is ``True``. Defaults to ``True``.
-
-
-        .. versionchanged:: 2.6
-
-            Added the ``force`` keyword argument.
-        """
-        assert self._guild is not None
-
-        if force:
-            self.queue._loaded = None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'encodedTrack': None})
-
-        self._player_state['track'] = None
-        logger.debug(f'Player {self.guild.id} was stopped.')
-
-    async def set_filter(
-        self,
-        _filter: Filter,
-        /, *,
-        seek: bool = False
-    ) -> None:
-        """|coro|
-
-        Set the player's filter.
-
-        Parameters
-        ----------
-        filter: :class:`wavelink.Filter`
-            The filter to apply to the player.
-        seek: bool
-            Whether to seek the player to its current position
-            which will apply the filter immediately. Defaults to ``False``.
-        """
-
-        assert self._guild is not None
-
-        self._filter = _filter
-        data: Request = {"filters": _filter._payload}
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=data)        
-
-        if self.is_playing() and seek:
-            await self.seek(int(self.position))
-
-        logger.debug(f'Player {self.guild.id} set filter to: {_filter}')
-
-    def _invalidate(self, *, silence: bool = False, before_connect: bool = False) -> None:
-        self.current_node._players.pop(self._guild.id, None)
-
-        if not before_connect:
-            self.current_node._invalidated[self._guild.id] = self
-
-        try:
-            self.cleanup()
-        except AttributeError:
-            pass
-        except Exception as e:
-            logger.debug(f'Failed to cleanup player, most likely due to never having been connected: {e}')
-
-        self._voice_state = {}
-        self._player_state = {}
-        self.channel = None
-
-        if not silence:
-            logger.debug(f'Player {self._guild.id} was invalidated.')
-
-    async def _destroy(self, *, guild_id: int | None = None) -> None:
-        if self._destroyed:
-            return
-
-        self._invalidate(silence=True)
-
-        guild_id = guild_id or self._guild.id
-
-        await self.current_node._send(method='DELETE',
-                                      path=f'sessions/{self.current_node._session_id}/players',
-                                      guild_id=guild_id)
-
-        self._destroyed = True
-        self.current_node._invalidated.pop(guild_id, None)
-        logger.debug(f'Player {guild_id} was destroyed.')
-
-    async def disconnect(self, **kwargs) -> None:
-        """|coro|
-
-        Disconnect the Player from voice and cleanup the Player state.
-
-        .. versionchanged:: 2.5
-
-            The discord.py Voice Client cache and Player are invalidated as soon as this is called.
-        """
-        self._invalidate()
-        await self.guild.change_voice_state(channel=None)
-
-        logger.debug(f'Player {self._guild.id} was disconnected.')
-
-    async def _swap_state(self) -> None:
-        assert self._guild is not None
-
-        try:
-            self._player_state['track']
-        except KeyError:
-            return
-
-        data: EncodedTrackRequest = {'encodedTrack': self._player_state['track'], 'position': self.position}
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=data)
-
-        logger.debug(f'Player {self.guild.id} is swapping State: {resp}')
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import datetime
+import logging
+from typing import TYPE_CHECKING, Any, Union
+
+import discord
+from discord.utils import MISSING
+
+from .enums import *
+from .exceptions import *
+from .ext import spotify
+from .filters import Filter
+from .node import Node, NodePool
+from .payloads import TrackEventPayload
+from .queue import Queue
+from .tracks import *
+
+
+if TYPE_CHECKING:
+    from discord.types.voice import GuildVoiceState, VoiceServerUpdate
+    from typing_extensions import Self
+
+    from .types.events import PlayerState, PlayerUpdateOp
+    from .types.request import EncodedTrackRequest, Request
+    from .types.state import DiscordVoiceState
+
+__all__ = ("Player",)
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+VoiceChannel = Union[
+    discord.VoiceChannel, discord.StageChannel
+]  # todo: VocalGuildChannel?
+
+
+class Player(discord.VoiceProtocol):
+    """Wavelink Player class.
+
+    This class is used as a :class:`~discord.VoiceProtocol` and inherits all its members.
+
+    You must pass this class to :meth:`discord.VoiceChannel.connect` with ``cls=...``. This ensures the player is
+    set up correctly and put into the discord.py voice client cache.
+
+    You **can** make an instance of this class *before* passing it to
+    :meth:`discord.VoiceChannel.connect` with ``cls=...``, but you **must** still pass it.
+
+    Once you have connected this class you do not need to store it anywhere as it will be stored on the
+    :class:`~wavelink.Node` and in the discord.py voice client cache. Meaning you can access this player where you
+    have access to a :class:`~wavelink.NodePool`, the specific :class:`~wavelink.Node` or a :class:`~discord.Guild`
+    including in :class:`~discord.ext.commands.Context` and :class:`~discord.Interaction`.
+
+    Examples
+    --------
+
+    .. code:: python3
+
+        # Connect the player...
+        player: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+
+        # Retrieve the player later...
+        player: wavelink.Player = ctx.guild.voice_client
+
+
+    .. note::
+
+        The Player class comes with an in-built queue. See :class:`queue.Queue` for more information on how this queue
+        works.
+
+    Parameters
+    ----------
+    nodes: Optional[list[:class:`node.Node`]]
+        An optional list of :class:`node.Node` to use with this Player. If no Nodes are provided
+        the best connected Node will be used.
+    swap_node_on_disconnect: bool
+        If a list of :class:`node.Node` is provided the Player will swap Nodes on Node disconnect.
+        Defaults to True.
+
+    Attributes
+    ----------
+    client: :class:`discord.Client`
+        The discord Client or Bot associated with this Player.
+    channel: :class:`discord.VoiceChannel`
+        The channel this player is currently connected to.
+    nodes: list[:class:`node.Node`]
+        The list of Nodes this player is currently using.
+    current_node: :class:`node.Node`
+        The Node this player is currently using.
+    queue: :class:`queue.Queue`
+        The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
+        Meaning any songs in this queue will be played before auto_queue songs.
+    auto_queue: :class:`queue.Queue`
+        The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
+        When a song is retrieved from this queue in the AutoPlay event,
+        it is added to the main :attr:`wavelink.Queue.history` queue.
+    """
+
+    def __call__(self, client: discord.Client, channel: VoiceChannel) -> Self:
+        self.client = client
+        self.channel = channel
+
+        return self
+
+    def __init__(
+        self,
+        client: discord.Client = MISSING,
+        channel: VoiceChannel = MISSING,
+        *,
+        nodes: list[Node] | None = None,
+        swap_node_on_disconnect: bool = True
+    ) -> None:
+        self.client: discord.Client = client
+        self.channel: VoiceChannel | None = channel
+
+        self.nodes: list[Node]
+        self.current_node: Node
+
+        if swap_node_on_disconnect and not nodes:
+            nodes = list(NodePool.nodes.values())
+            self.nodes = sorted(nodes, key=lambda n: len(n.players))
+            self.current_node = self.nodes[0]
+        elif nodes:
+            nodes = sorted(nodes, key=lambda n: len(n.players))
+            self.current_node = nodes[0]
+            self.nodes = nodes
+        else:
+            self.current_node = NodePool.get_connected_node()
+            self.nodes = [self.current_node]
+
+        if not self.client:
+            if self.current_node.client is None:
+                raise RuntimeError('')
+            self.client = self.current_node.client
+
+        self._guild: discord.Guild | None = None
+        self._voice_state: DiscordVoiceState = {}
+        self._player_state: dict[str, Any] = {}
+
+        self.swap_on_disconnect: bool = swap_node_on_disconnect
+
+        self.last_update: datetime.datetime | None = None
+        self.last_position: int = 0
+
+        self._ping: int = 0
+
+        self.queue: Queue = Queue()
+        self._current: Playable | None = None
+        self._original: Playable | None = None
+
+        self._volume: int = 50
+        self._paused: bool = False
+
+        self._track_seeds: list[str] = []
+        self._autoplay: bool = False
+        self.auto_queue: Queue = Queue()
+        self._auto_threshold: int = 100
+        self._filter: Filter | None = None
+
+        self._destroyed: bool = False
+
+    async def _auto_play_event(self, payload: TrackEventPayload) -> None:
+        logger.debug(f'Player {self.guild.id} entered autoplay event.')
+
+        if not self.autoplay:
+            logger.debug(f'Player {self.guild.id} autoplay is set to False. Exiting autoplay event.')
+            return
+
+        if payload.reason == 'REPLACED':
+            logger.debug(f'Player {self.guild.id} autoplay reason is REPLACED. Exiting autoplay event.')
+            return
+
+        if self.queue.loop:
+            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True.')
+
+            try:
+                track = self.queue.get()
+            except QueueEmpty:
+                logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True '
+                             f'but no track was available. Exiting autoplay event.')
+                return
+
+            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True. Looping track "{track}"')
+            await self.play(track)
+            return
+
+        if self.queue:
+            track = self.queue.get()
+
+            populate = len(self.auto_queue) < self._auto_threshold
+            await self.play(track, populate=populate)
+
+            logger.debug(f'Player {self.guild.id} autoplay found track in default queue, populate={populate}.')
+            return
+
+        if self.queue.loop_all:
+            await self.play(self.queue.get())
+            return
+
+        if not self.auto_queue:
+            logger.debug(f'Player {self.guild.id} has no auto queue. Exiting autoplay event.')
+            return
+
+        await self.queue.put_wait(await self.auto_queue.get_wait())
+        populate = self.auto_queue.is_empty
+
+        track = await self.queue.get_wait()
+        await self.play(track, populate=populate)
+
+        logger.debug(f'Player {self.guild.id} playing track "{track}" from autoplay with populate={populate}.')
+
+    @property
+    def autoplay(self) -> bool:
+        """Returns a ``bool`` indicating whether the :class:`~Player` is in AutoPlay mode or not.
+
+        This property can be set to ``True`` or ``False``.
+
+        When ``autoplay`` is ``True``, the player will automatically handle fetching and playing the next track from
+        the queue. It also searches tracks in the ``auto_queue``, a special queue populated with recommended tracks,
+        from the Spotify API or YouTube Recommendations.
+
+
+        .. note::
+
+            You can still use the :func:`~wavelink.on_wavelink_track_end` event when ``autoplay`` is ``True``,
+            but it is recommended to **not** do any queue logic or invoking play from this event.
+
+            Most users are able to use ``autoplay`` and :func:`~wavelink.on_wavelink_track_start` together to handle
+            their logic. E.g. sending a message when a track starts playing.
+
+
+        .. note::
+
+            The ``auto_queue`` will be populated when you play a :class:`~wavelink.ext.spotify.SpotifyTrack` or
+            :class:`~wavelink.YouTubeTrack`, and have initially set ``populate`` to ``True`` in
+            :meth:`~wavelink.Player.play`. See :meth:`~wavelink.Player.play` for more info.
+
+
+        .. versionadded:: 2.0
+
+
+        .. versionchanged:: 2.6.0
+
+            The autoplay event now populates the ``auto_queue`` when playing :class:`~wavelink.YouTubeTrack` **or**
+            :class:`~wavelink.ext.spotify.SpotifyTrack`.
+        """
+        return self._autoplay
+
+    @autoplay.setter
+    def autoplay(self, value: bool) -> None:
+        """Set AutoPlay to True or False."""
+        self._autoplay = value
+
+    def is_connected(self) -> bool:
+        """Whether the player is connected to a voice channel."""
+        return self.channel is not None and self.channel is not MISSING
+
+    def is_playing(self) -> bool:
+        """Whether the Player is currently playing a track."""
+        return self.current is not None and not self._paused
+
+    def is_paused(self) -> bool:
+        """Whether the Player is currently paused."""
+        return self._paused
+
+    @property
+    def volume(self) -> int:
+        """The current volume of the Player."""
+        return self._volume
+
+    @property
+    def guild(self) -> discord.Guild | None:
+        """The discord Guild associated with the Player."""
+        return self._guild
+
+    @property
+    def position(self) -> float:
+        """The position of the currently playing track in milliseconds."""
+
+        if not self.is_playing():
+            return 0
+
+        if self.is_paused():
+            return min(self.last_position, self.current.duration)  # type: ignore
+
+        delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
+        position = self.last_position + delta
+
+        return min(position, self.current.duration)
+
+    @property
+    def ping(self) -> int:
+        """The ping to the discord endpoint in milliseconds.
+
+        .. versionadded:: 2.0
+        """
+        return self._ping
+
+    @property
+    def current(self) -> Playable | None:
+        """The currently playing Track if there is one.
+
+        Could be ``None`` if no Track is playing.
+        """
+        return self._current
+
+    @property
+    def filter(self) -> dict[str, Any]:
+        """The currently applied filter."""
+        return self._filter._payload
+
+    async def _update_event(self, data: PlayerUpdateOp | None) -> None:
+        assert self._guild is not None
+
+        if data is None: 
+            if self.swap_on_disconnect:
+
+                if len(self.nodes) < 2:
+                    return
+
+                new: Node = [n for n in self.nodes if n != self.current_node and n.status is NodeStatus.CONNECTED][0]
+                del self.current_node._players[self._guild.id]
+
+                if not new:
+                    return
+
+                self.current_node: Node = new
+                new._players[self._guild.id] = self
+
+                await self._dispatch_voice_update()
+                await self._swap_state()
+            return
+
+        data.pop('op')  # type: ignore
+        self._player_state.update(**data)
+
+        state: PlayerState = data['state']
+        self.last_update = datetime.datetime.fromtimestamp(state.get("time", 0) / 1000, datetime.timezone.utc)
+        self.last_position = state.get('position', 0)
+
+        self._ping = state['ping']
+
+    async def on_voice_server_update(self, data: VoiceServerUpdate) -> None:
+        """|coro|
+
+        An abstract method that is called when initially connecting to voice. This corresponds to VOICE_SERVER_UPDATE.
+
+        .. warning::
+
+            Do not override this method.
+        """
+        self._voice_state['token'] = data['token']
+        self._voice_state['endpoint'] = data['endpoint']
+
+        await self._dispatch_voice_update()
+
+    async def on_voice_state_update(self, data: GuildVoiceState) -> None:
+        """|coro|
+
+        An abstract method that is called when the client’s voice state has changed.
+        This corresponds to VOICE_STATE_UPDATE.
+
+        .. warning::
+
+            Do not override this method.
+        """
+        assert self._guild is not None
+
+        channel_id = data["channel_id"]
+
+        if not channel_id:
+            await self._destroy()
+            return
+
+        self._voice_state['session_id'] = data['session_id']
+        self.channel = self.client.get_channel(int(channel_id))  # type: ignore
+
+        if not self._guild:
+            self._guild = self.channel.guild  # type: ignore
+            assert self._guild is not None
+            self.current_node._players[self._guild.id] = self
+
+    async def _dispatch_voice_update(self, data: DiscordVoiceState | None = None) -> None:
+        assert self._guild is not None
+
+        data = data or self._voice_state
+
+        try:
+            session_id: str = data['session_id']
+            token: str = data['token']
+            endpoint: str = data['endpoint']
+        except KeyError:
+            return
+
+        voice: Request = {'voice': {'sessionId': session_id, 'token': token, 'endpoint': endpoint}}
+        self._player_state.update(**voice)
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=voice)
+
+        logger.debug(f'Player {self.guild.id} is dispatching VOICE_UPDATE: {resp}')
+
+    def _connection_check(self, channel: VoiceChannel) -> None:
+        if channel.permissions_for(channel.guild.me).administrator:
+            return
+
+        if not channel.permissions_for(channel.guild.me).connect:
+            logger.debug(f'Player tried connecting to channel "{channel.id}", but does not have correct permissions.')
+
+            raise InvalidChannelPermissions('You do not have connect permissions to join this channel.')
+
+        limit: int = channel.user_limit
+        total: int = len(channel.members)
+
+        if limit == 0:
+            pass
+
+        elif total >= limit:
+            msg: str = f'There are currently too many users in this channel. <{total}/{limit}>'
+            logger.debug(f'Player tried connecting to channel "{channel.id}", but the it is full. <{total}/{limit}>')
+
+            raise InvalidChannelPermissions(msg)
+
+    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
+        if self.channel is None:
+            self._invalidate(before_connect=True)
+
+            msg: str = 'Please use the method "discord.VoiceChannel.connect" and pass this player to cls='
+            logger.debug(f'Player tried connecting without a channel. {msg}')
+
+            raise InvalidChannelStateError(msg)
+
+        if not self._guild:
+            self._guild = self.channel.guild
+            self.current_node._players[self._guild.id] = self
+
+        try:
+            self._connection_check(self.channel)
+        except InvalidChannelPermissions as e:
+            self._invalidate(before_connect=True)
+            raise e
+
+        await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
+        logger.info(f'Player {self.guild.id} connected to channel: {self.channel}')
+
+    async def move_to(self, channel: discord.VoiceChannel) -> None:
+        """|coro|
+
+        Moves the player to a different voice channel.
+
+        Parameters
+        -----------
+        channel: :class:`discord.VoiceChannel`
+            The channel to move to. Must be a voice channel.
+        """
+        self._connection_check(channel)
+
+        await self.guild.change_voice_state(channel=channel)
+        logger.info(f'Player {self.guild.id} moved to channel: {channel}')
+
+    async def play(self,
+                   track: Playable | spotify.SpotifyTrack,
+                   replace: bool = True,
+                   start: int | None = None,
+                   end: int | None = None,
+                   volume: int | None = None,
+                   *,
+                   populate: bool = False
+                   ) -> Playable:
+        """|coro|
+
+        Play a WaveLink Track.
+
+        Parameters
+        ----------
+        track: :class:`tracks.Playable`
+            The :class:`tracks.Playable` or :class:`~wavelink.ext.spotify.SpotifyTrack` track to start playing.
+        replace: bool
+            Whether this track should replace the current track. Defaults to ``True``.
+        start: Optional[int]
+            The position to start the track at in milliseconds.
+            Defaults to ``None`` which will start the track at the beginning.
+        end: Optional[int]
+            The position to end the track at in milliseconds.
+            Defaults to ``None`` which means it will play until the end.
+        volume: Optional[int]
+            Sets the volume of the player. Must be between ``0`` and ``1000``.
+            Defaults to ``None`` which will not change the volume.
+        populate: bool
+            Whether to populate the AutoPlay queue. Defaults to ``False``.
+
+            .. versionadded:: 2.0
+
+        Returns
+        -------
+        :class:`~tracks.Playable`
+            The track that is now playing.
+
+
+        .. note::
+
+            If you pass a :class:`~wavelink.YouTubeTrack` **or** :class:`~wavelink.ext.spotify.SpotifyTrack` and set
+            ``populate=True``, **while** :attr:`~wavelink.Player.autoplay` is set to ``True``, this method will populate
+            the ``auto_queue`` with recommended songs. When the ``auto_queue`` is low on tracks this method will
+            automatically populate the ``auto_queue`` with more tracks, and continue this cycle until either the
+            player has been disconnected or :attr:`~wavelink.Player.autoplay` is set to ``False``.
+
+
+        Example
+        -------
+
+        .. code:: python3
+
+            tracks: list[wavelink.YouTubeTrack] = await wavelink.YouTubeTrack.search(...)
+            if not tracks:
+                # Do something as no tracks were found...
+                return
+
+            await player.queue.put_wait(tracks[0])
+
+            if not player.is_playing():
+                await player.play(player.queue.get(), populate=True)
+
+
+        .. versionchanged:: 2.6.0
+
+            This method now accepts :class:`~wavelink.YouTubeTrack` or :class:`~wavelink.ext.spotify.SpotifyTrack`
+            when populating the ``auto_queue``.
+        """
+        assert self._guild is not None
+
+        if isinstance(track, YouTubeTrack) and self.autoplay and populate:
+            query: str = f'https://www.youtube.com/watch?v={track.identifier}&list=RD{track.identifier}'
+
+            try:
+                recos: YouTubePlaylist = await self.current_node.get_playlist(query=query, cls=YouTubePlaylist)
+                recos: list[YouTubeTrack] = getattr(recos, 'tracks', [])
+
+                queues = set(self.queue) | set(self.auto_queue) | set(self.auto_queue.history) | {track}
+
+                for track_ in recos:
+                    if track_ in queues:
+                        continue
+
+                    await self.auto_queue.put_wait(track_)
+
+                self.auto_queue.shuffle()
+            except ValueError:
+                pass
+
+        elif isinstance(track, spotify.SpotifyTrack):
+            original = track
+            track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
+
+            if populate:
+                self.auto_queue.shuffle()
+
+            for attr, value in original.__dict__.items():
+                if hasattr(track, attr):
+                    logger.warning(f'Player {self.guild.id} was unable to set attribute "{attr}" '
+                                   f'when converting a SpotifyTrack as it conflicts with the new track type.')
+                    continue
+
+                setattr(track, attr, value)
+
+        data = {
+            'encodedTrack': track.encoded,
+            'position': start or 0,
+            'volume': volume or self._volume
+        }
+
+        if end:
+            data['endTime'] = end
+
+        self._current = track
+        self._original = track
+
+        try:
+
+            resp: dict[str, Any] = await self.current_node._send(
+                method='PATCH',
+                path=f'sessions/{self.current_node._session_id}/players',
+                guild_id=self._guild.id,
+                data=data,
+                query=f'noReplace={not replace}'
+            )
+
+        except InvalidLavalinkResponse as e:
+            self._current = None
+            self._original = None
+            logger.debug(f'Player {self._guild.id} attempted to load track: {track}, but failed: {e}')
+            raise e
+
+        self._player_state['track'] = resp['track']['encoded']
+
+        if not (self.queue.loop and self.queue._loaded):
+            self.queue.history.put(track)
+
+        self.queue._loaded = track
+
+        logger.debug(f'Player {self._guild.id} loaded and started playing track: {track}.')
+        return track
+
+    async def set_volume(self, value: int) -> None:
+        """|coro|
+
+        Set the Player volume.
+
+        Parameters
+        ----------
+        value: int
+            A volume value between 0 and 1000.
+        """
+        assert self._guild is not None
+
+        self._volume = max(min(value, 1000), 0)
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'volume': self._volume})
+
+        logger.debug(f'Player {self.guild.id} volume was set to {self._volume}.')
+
+    async def seek(self, position: int) -> None:
+        """|coro|
+
+        Seek to the provided position, in milliseconds.
+
+        Parameters
+        ----------
+        position: int
+            The position to seek to in milliseconds.
+        """
+        if not self._current:
+            return
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'position': position})
+
+        logger.debug(f'Player {self.guild.id} seeked current track to position {position}.')
+
+    async def pause(self) -> None:
+        """|coro|
+
+        Pauses the Player.
+        """
+        assert self._guild is not None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'paused': True})
+
+        self._paused = True
+        logger.debug(f'Player {self.guild.id} was paused.')
+
+    async def resume(self) -> None:
+        """|coro|
+
+        Resumes the Player.
+        """
+        assert self._guild is not None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'paused': False})
+
+        self._paused = False
+        logger.debug(f'Player {self.guild.id} was resumed.')
+
+    async def stop(self, *, force: bool = True) -> None:
+        """|coro|
+
+        Stops the currently playing Track.
+
+        Parameters
+        ----------
+        force: Optional[bool]
+            Whether to stop the currently playing track and proceed to the next regardless if :attr:`~Queue.loop`
+            is ``True``. Defaults to ``True``.
+
+
+        .. versionchanged:: 2.6
+
+            Added the ``force`` keyword argument.
+        """
+        assert self._guild is not None
+
+        if force:
+            self.queue._loaded = None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'encodedTrack': None})
+
+        self._player_state['track'] = None
+        logger.debug(f'Player {self.guild.id} was stopped.')
+
+    async def set_filter(
+        self,
+        _filter: Filter,
+        /, *,
+        seek: bool = False
+    ) -> None:
+        """|coro|
+
+        Set the player's filter.
+
+        Parameters
+        ----------
+        filter: :class:`wavelink.Filter`
+            The filter to apply to the player.
+        seek: bool
+            Whether to seek the player to its current position
+            which will apply the filter immediately. Defaults to ``False``.
+        """
+
+        assert self._guild is not None
+
+        self._filter = _filter
+        data: Request = {"filters": _filter._payload}
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=data)        
+
+        if self.is_playing() and seek:
+            await self.seek(int(self.position))
+
+        logger.debug(f'Player {self.guild.id} set filter to: {_filter}')
+
+    def _invalidate(self, *, silence: bool = False, before_connect: bool = False) -> None:
+        self.current_node._players.pop(self._guild.id, None)
+
+        if not before_connect:
+            self.current_node._invalidated[self._guild.id] = self
+
+        try:
+            self.cleanup()
+        except AttributeError:
+            pass
+        except Exception as e:
+            logger.debug(f'Failed to cleanup player, most likely due to never having been connected: {e}')
+
+        self._voice_state = {}
+        self._player_state = {}
+        self.channel = None
+
+        if not silence:
+            logger.debug(f'Player {self._guild.id} was invalidated.')
+
+    async def _destroy(self, *, guild_id: int | None = None) -> None:
+        if self._destroyed:
+            return
+
+        self._invalidate(silence=True)
+
+        guild_id = guild_id or self._guild.id
+
+        await self.current_node._send(method='DELETE',
+                                      path=f'sessions/{self.current_node._session_id}/players',
+                                      guild_id=guild_id)
+
+        self._destroyed = True
+        self.current_node._invalidated.pop(guild_id, None)
+        logger.debug(f'Player {guild_id} was destroyed.')
+
+    async def disconnect(self, **kwargs) -> None:
+        """|coro|
+
+        Disconnect the Player from voice and cleanup the Player state.
+
+        .. versionchanged:: 2.5
+
+            The discord.py Voice Client cache and Player are invalidated as soon as this is called.
+        """
+        self._invalidate()
+        await self.guild.change_voice_state(channel=None)
+
+        logger.debug(f'Player {self._guild.id} was disconnected.')
+
+    async def _swap_state(self) -> None:
+        assert self._guild is not None
+
+        try:
+            self._player_state['track']
+        except KeyError:
+            return
+
+        data: EncodedTrackRequest = {'encodedTrack': self._player_state['track'], 'position': self.position}
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=data)
+
+        logger.debug(f'Player {self.guild.id} is swapping State: {resp}')
```

### Comparing `Wavelink-2.6.0/wavelink/tracks.py` & `wavelink-2.6.1/wavelink/tracks.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,391 +1,391 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import abc
-from typing import TYPE_CHECKING, ClassVar, Literal, overload, Optional, Any
-
-import aiohttp
-import yarl
-from discord.ext import commands
-
-from .enums import TrackSource
-from .exceptions import NoTracksError
-from .node import Node, NodePool
-
-if TYPE_CHECKING:
-    from typing_extensions import Self
-
-    from .types.track import Track as TrackPayload
-
-__all__ = (
-    'Playable',
-    'Playlist',
-    'YouTubeTrack',
-    'GenericTrack',
-    'YouTubeMusicTrack',
-    'SoundCloudTrack',
-    'YouTubePlaylist',
-    'SoundCloudPlaylist'
-)
-
-
-_source_mapping: dict[str, TrackSource] = {
-    'youtube': TrackSource.YouTube
-}
-
-
-class Playlist(metaclass=abc.ABCMeta):
-    """An ABC that defines the basic structure of a lavalink playlist resource.
-
-    Attributes
-    ----------
-    data: Dict[str, Any]
-        The raw data supplied by Lavalink.
-    """
-
-    def __init__(self, data: dict[str, Any]):
-        self.data: dict[str, Any] = data
-
-
-class Playable(metaclass=abc.ABCMeta):
-    """Base ABC Track used in all the Wavelink Track types.
-
-
-    .. container:: operations
-
-        .. describe:: str(track)
-
-            Returns a string representing the tracks name.
-
-        .. describe:: repr(track)
-
-            Returns an official string representation of this track.
-
-        .. describe:: track == other_track
-
-            Check whether a track is equal to another. A track is equal when they have the same Base64 Encoding.
-
-
-    Attributes
-    ----------
-    data: dict[str, Any]
-        The raw data received via Lavalink.
-    encoded: str
-        The encoded Track string.
-    is_seekable: bool
-        Whether the Track is seekable.
-    is_stream: bool
-        Whether the Track is a stream.
-    length: int
-        The length of the track in milliseconds.
-    duration: int
-        An alias for length.
-    position: int
-        The position the track will start in milliseconds. Defaults to 0.
-    title: str
-        The Track title.
-    source: :class:`wavelink.TrackSource`
-        The source this Track was fetched from.
-    uri: Optional[str]
-        The URI of this track. Could be None.
-    author: Optional[str]
-        The author of this track. Could be None.
-    identifier: Optional[str]
-        The Youtube/YoutubeMusic identifier for this track. Could be None.
-    """
-
-    PREFIX: ClassVar[str] = ''
-    
-    def __init__(self, data: TrackPayload) -> None:
-        self.data: TrackPayload = data
-        self.encoded: str = data['encoded']
-
-        info = data['info']
-        self.is_seekable: bool = info.get('isSeekable', False)
-        self.is_stream: bool = info.get('isStream', False)
-        self.length: int = info.get('length', 0)
-        self.duration: int = self.length
-        self.position: int = info.get('position', 0)
-
-        self.title: str = info.get('title', 'Unknown Title')
-
-        source: str | None = info.get('sourceName')
-        self.source: TrackSource = _source_mapping.get(source, TrackSource.Unknown)
-
-        self.uri: str | None = info.get('uri')
-        self.author: str | None = info.get('author')
-        self.identifier: str | None = info.get('identifier')
-
-    def __hash__(self) -> int:
-        return hash(self.encoded)
-
-    def __str__(self) -> str:
-        return self.title
-
-    def __repr__(self) -> str:
-        return f'Playable: source={self.source}, title={self.title}'
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, Playable):
-            return self.encoded == other.encoded
-        return NotImplemented
-    
-    @overload
-    @classmethod
-    async def search(cls,
-                     query: str,
-                     /,
-                     *,
-                     node: Node | None = ...
-                     ) -> list[Self]:
-        ...
-
-    @overload
-    @classmethod
-    async def search(cls,
-                     query: str,
-                     /,
-                     *,
-                     node: Node | None = ...
-                     ) -> YouTubePlaylist:
-        ...
-
-    @overload
-    @classmethod
-    async def search(cls,
-                     query: str,
-                     /,
-                     *,
-                     node: Node | None = ...
-                     ) -> SoundCloudPlaylist:
-        ...
-
-    @classmethod
-    async def search(cls,
-                     query: str,
-                     /,
-                     *,
-                     node: Node | None = None
-                     ) -> list[Self]:
-        """Search and retrieve tracks for the given query.
-
-        Parameters
-        ----------
-        query: str
-            The query to search for.
-        node: Optional[:class:`wavelink.Node`]
-            The node to use when searching for tracks. If no :class:`wavelink.Node` is passed,
-            one will be fetched via the :class:`wavelink.NodePool`.
-        """
-
-        check = yarl.URL(query)
-
-        if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
-                cls.PREFIX == 'ytpl:':
-
-            playlist = await NodePool.get_playlist(query, cls=YouTubePlaylist, node=node)
-            return playlist
-        elif str(check.host) == 'soundcloud.com' or str(check.host) == 'www.soundcloud.com' and 'sets' in check.parts:
-
-            playlist = await NodePool.get_playlist(query, cls=SoundCloudPlaylist, node=node)
-            return playlist
-        elif check.host:
-            tracks = await NodePool.get_tracks(query, cls=cls, node=node)
-        else:
-            tracks = await NodePool.get_tracks(f'{cls.PREFIX}{query}', cls=cls, node=node)
-
-        return tracks
-
-    @classmethod
-    async def convert(cls, ctx: commands.Context, argument: str) -> Self:
-        """Converter which searches for and returns the first track.
-
-        Used as a type hint in a
-        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
-        """
-        results = await cls.search(argument)
-
-        if not results:
-            raise commands.BadArgument("Could not find any songs matching that query.")
-
-        if issubclass(cls, YouTubePlaylist):
-            return results  # type: ignore
-
-        return results[0]
-
-
-class GenericTrack(Playable):
-    """Generic Wavelink Track.
-
-    Use this track for searching for Local songs or direct URLs.
-    """
-    ...
-
-
-class YouTubeTrack(Playable):
-
-    PREFIX: str = 'ytsearch:'
-
-    def __init__(self, data: TrackPayload) -> None:
-        super().__init__(data)
-
-        self._thumb: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
-
-    @property
-    def thumbnail(self) -> str:
-        """The URL to the thumbnail of this video.
-
-        .. note::
-
-            Due to YouTube limitations this may not always return a valid thumbnail.
-            Use :meth:`.fetch_thumbnail` to fallback.
-
-        Returns
-        -------
-        str
-            The URL to the video thumbnail.
-        """
-        return self._thumb
-
-    thumb = thumbnail
-
-    async def fetch_thumbnail(self, *, node: Node | None = None) -> str:
-        """Fetch the max resolution thumbnail with a fallback if it does not exist.
-
-        This sets and overrides the default ``thumbnail`` and ``thumb`` properties.
-
-        .. note::
-
-            This method uses an API request to fetch the thumbnail.
-
-        Returns
-        -------
-        str
-            The URL to the video thumbnail.
-        """
-        if not node:
-            node = NodePool.get_node()
-
-        session: aiohttp.ClientSession = node._session
-        url: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
-
-        async with session.get(url=url) as resp:
-            if resp.status == 404:
-                url = f'https://img.youtube.com/vi/{self.identifier}/hqdefault.jpg'
-
-        self._thumb = url
-        return url
-
-
-class YouTubeMusicTrack(YouTubeTrack):
-    """A track created using a search to YouTube Music."""
-
-    PREFIX: str = "ytmsearch:"
-
-
-class SoundCloudTrack(Playable):
-    """A track created using a search to SoundCloud."""
-
-    PREFIX: str = "scsearch:"
-
-
-class YouTubePlaylist(Playable, Playlist):
-    """Represents a Lavalink YouTube playlist object.
-
-
-    .. container:: operations
-
-        .. describe:: str(playlist)
-
-            Returns a string representing the playlists name.
-
-
-    Attributes
-    ----------
-    name: str
-        The name of the playlist.
-    tracks: :class:`YouTubeTrack`
-        The list of :class:`YouTubeTrack` in the playlist.
-    selected_track: Optional[int]
-        The selected video in the playlist. This could be ``None``.
-    """
-
-    PREFIX: str = "ytpl:"
-
-    def __init__(self, data: dict):
-        self.tracks: list[YouTubeTrack] = []
-        self.name: str = data["playlistInfo"]["name"]
-
-        self.selected_track: Optional[int] = data["playlistInfo"].get("selectedTrack")
-        if self.selected_track is not None:
-            self.selected_track = int(self.selected_track)
-
-        for track_data in data["tracks"]:
-            track = YouTubeTrack(track_data)
-            self.tracks.append(track)
-
-        self.source = TrackSource.YouTube
-
-    def __str__(self) -> str:
-        return self.name
-
-
-class SoundCloudPlaylist(Playable, Playlist):
-    """Represents a Lavalink SoundCloud playlist object.
-
-
-    .. container:: operations
-
-        .. describe:: str(playlist)
-
-            Returns a string representing the playlists name.
-
-
-    Attributes
-    ----------
-    name: str
-        The name of the playlist.
-    tracks: :class:`SoundCloudTrack`
-        The list of :class:`SoundCloudTrack` in the playlist.
-    selected_track: Optional[int]
-        The selected video in the playlist. This could be ``None``.
-    """
-
-    def __init__(self, data: dict):
-        self.tracks: list[SoundCloudTrack] = []
-        self.name: str = data["playlistInfo"]["name"]
-
-        self.selected_track: Optional[int] = data["playlistInfo"].get("selectedTrack")
-        if self.selected_track is not None:
-            self.selected_track = int(self.selected_track)
-
-        for track_data in data["tracks"]:
-            track = SoundCloudTrack(track_data)
-            self.tracks.append(track)
-
-        self.source = TrackSource.SoundCloud
-
-    def __str__(self) -> str:
-        return self.name
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import abc
+from typing import TYPE_CHECKING, ClassVar, Literal, overload, Optional, Any
+
+import aiohttp
+import yarl
+from discord.ext import commands
+
+from .enums import TrackSource
+from .exceptions import NoTracksError
+from .node import Node, NodePool
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    from .types.track import Track as TrackPayload
+
+__all__ = (
+    'Playable',
+    'Playlist',
+    'YouTubeTrack',
+    'GenericTrack',
+    'YouTubeMusicTrack',
+    'SoundCloudTrack',
+    'YouTubePlaylist',
+    'SoundCloudPlaylist'
+)
+
+
+_source_mapping: dict[str, TrackSource] = {
+    'youtube': TrackSource.YouTube
+}
+
+
+class Playlist(metaclass=abc.ABCMeta):
+    """An ABC that defines the basic structure of a lavalink playlist resource.
+
+    Attributes
+    ----------
+    data: Dict[str, Any]
+        The raw data supplied by Lavalink.
+    """
+
+    def __init__(self, data: dict[str, Any]):
+        self.data: dict[str, Any] = data
+
+
+class Playable(metaclass=abc.ABCMeta):
+    """Base ABC Track used in all the Wavelink Track types.
+
+
+    .. container:: operations
+
+        .. describe:: str(track)
+
+            Returns a string representing the tracks name.
+
+        .. describe:: repr(track)
+
+            Returns an official string representation of this track.
+
+        .. describe:: track == other_track
+
+            Check whether a track is equal to another. A track is equal when they have the same Base64 Encoding.
+
+
+    Attributes
+    ----------
+    data: dict[str, Any]
+        The raw data received via Lavalink.
+    encoded: str
+        The encoded Track string.
+    is_seekable: bool
+        Whether the Track is seekable.
+    is_stream: bool
+        Whether the Track is a stream.
+    length: int
+        The length of the track in milliseconds.
+    duration: int
+        An alias for length.
+    position: int
+        The position the track will start in milliseconds. Defaults to 0.
+    title: str
+        The Track title.
+    source: :class:`wavelink.TrackSource`
+        The source this Track was fetched from.
+    uri: Optional[str]
+        The URI of this track. Could be None.
+    author: Optional[str]
+        The author of this track. Could be None.
+    identifier: Optional[str]
+        The Youtube/YoutubeMusic identifier for this track. Could be None.
+    """
+
+    PREFIX: ClassVar[str] = ''
+    
+    def __init__(self, data: TrackPayload) -> None:
+        self.data: TrackPayload = data
+        self.encoded: str = data['encoded']
+
+        info = data['info']
+        self.is_seekable: bool = info.get('isSeekable', False)
+        self.is_stream: bool = info.get('isStream', False)
+        self.length: int = info.get('length', 0)
+        self.duration: int = self.length
+        self.position: int = info.get('position', 0)
+
+        self.title: str = info.get('title', 'Unknown Title')
+
+        source: str | None = info.get('sourceName')
+        self.source: TrackSource = _source_mapping.get(source, TrackSource.Unknown)
+
+        self.uri: str | None = info.get('uri')
+        self.author: str | None = info.get('author')
+        self.identifier: str | None = info.get('identifier')
+
+    def __hash__(self) -> int:
+        return hash(self.encoded)
+
+    def __str__(self) -> str:
+        return self.title
+
+    def __repr__(self) -> str:
+        return f'Playable: source={self.source}, title={self.title}'
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, Playable):
+            return self.encoded == other.encoded
+        return NotImplemented
+    
+    @overload
+    @classmethod
+    async def search(cls,
+                     query: str,
+                     /,
+                     *,
+                     node: Node | None = ...
+                     ) -> list[Self]:
+        ...
+
+    @overload
+    @classmethod
+    async def search(cls,
+                     query: str,
+                     /,
+                     *,
+                     node: Node | None = ...
+                     ) -> YouTubePlaylist:
+        ...
+
+    @overload
+    @classmethod
+    async def search(cls,
+                     query: str,
+                     /,
+                     *,
+                     node: Node | None = ...
+                     ) -> SoundCloudPlaylist:
+        ...
+
+    @classmethod
+    async def search(cls,
+                     query: str,
+                     /,
+                     *,
+                     node: Node | None = None
+                     ) -> list[Self]:
+        """Search and retrieve tracks for the given query.
+
+        Parameters
+        ----------
+        query: str
+            The query to search for.
+        node: Optional[:class:`wavelink.Node`]
+            The node to use when searching for tracks. If no :class:`wavelink.Node` is passed,
+            one will be fetched via the :class:`wavelink.NodePool`.
+        """
+
+        check = yarl.URL(query)
+
+        if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
+                cls.PREFIX == 'ytpl:':
+
+            playlist = await NodePool.get_playlist(query, cls=YouTubePlaylist, node=node)
+            return playlist
+        elif str(check.host) == 'soundcloud.com' or str(check.host) == 'www.soundcloud.com' and 'sets' in check.parts:
+
+            playlist = await NodePool.get_playlist(query, cls=SoundCloudPlaylist, node=node)
+            return playlist
+        elif check.host:
+            tracks = await NodePool.get_tracks(query, cls=cls, node=node)
+        else:
+            tracks = await NodePool.get_tracks(f'{cls.PREFIX}{query}', cls=cls, node=node)
+
+        return tracks
+
+    @classmethod
+    async def convert(cls, ctx: commands.Context, argument: str) -> Self:
+        """Converter which searches for and returns the first track.
+
+        Used as a type hint in a
+        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
+        """
+        results = await cls.search(argument)
+
+        if not results:
+            raise commands.BadArgument("Could not find any songs matching that query.")
+
+        if issubclass(cls, YouTubePlaylist):
+            return results  # type: ignore
+
+        return results[0]
+
+
+class GenericTrack(Playable):
+    """Generic Wavelink Track.
+
+    Use this track for searching for Local songs or direct URLs.
+    """
+    ...
+
+
+class YouTubeTrack(Playable):
+
+    PREFIX: str = 'ytsearch:'
+
+    def __init__(self, data: TrackPayload) -> None:
+        super().__init__(data)
+
+        self._thumb: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
+
+    @property
+    def thumbnail(self) -> str:
+        """The URL to the thumbnail of this video.
+
+        .. note::
+
+            Due to YouTube limitations this may not always return a valid thumbnail.
+            Use :meth:`.fetch_thumbnail` to fallback.
+
+        Returns
+        -------
+        str
+            The URL to the video thumbnail.
+        """
+        return self._thumb
+
+    thumb = thumbnail
+
+    async def fetch_thumbnail(self, *, node: Node | None = None) -> str:
+        """Fetch the max resolution thumbnail with a fallback if it does not exist.
+
+        This sets and overrides the default ``thumbnail`` and ``thumb`` properties.
+
+        .. note::
+
+            This method uses an API request to fetch the thumbnail.
+
+        Returns
+        -------
+        str
+            The URL to the video thumbnail.
+        """
+        if not node:
+            node = NodePool.get_node()
+
+        session: aiohttp.ClientSession = node._session
+        url: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
+
+        async with session.get(url=url) as resp:
+            if resp.status == 404:
+                url = f'https://img.youtube.com/vi/{self.identifier}/hqdefault.jpg'
+
+        self._thumb = url
+        return url
+
+
+class YouTubeMusicTrack(YouTubeTrack):
+    """A track created using a search to YouTube Music."""
+
+    PREFIX: str = "ytmsearch:"
+
+
+class SoundCloudTrack(Playable):
+    """A track created using a search to SoundCloud."""
+
+    PREFIX: str = "scsearch:"
+
+
+class YouTubePlaylist(Playable, Playlist):
+    """Represents a Lavalink YouTube playlist object.
+
+
+    .. container:: operations
+
+        .. describe:: str(playlist)
+
+            Returns a string representing the playlists name.
+
+
+    Attributes
+    ----------
+    name: str
+        The name of the playlist.
+    tracks: :class:`YouTubeTrack`
+        The list of :class:`YouTubeTrack` in the playlist.
+    selected_track: Optional[int]
+        The selected video in the playlist. This could be ``None``.
+    """
+
+    PREFIX: str = "ytpl:"
+
+    def __init__(self, data: dict):
+        self.tracks: list[YouTubeTrack] = []
+        self.name: str = data["playlistInfo"]["name"]
+
+        self.selected_track: Optional[int] = data["playlistInfo"].get("selectedTrack")
+        if self.selected_track is not None:
+            self.selected_track = int(self.selected_track)
+
+        for track_data in data["tracks"]:
+            track = YouTubeTrack(track_data)
+            self.tracks.append(track)
+
+        self.source = TrackSource.YouTube
+
+    def __str__(self) -> str:
+        return self.name
+
+
+class SoundCloudPlaylist(Playable, Playlist):
+    """Represents a Lavalink SoundCloud playlist object.
+
+
+    .. container:: operations
+
+        .. describe:: str(playlist)
+
+            Returns a string representing the playlists name.
+
+
+    Attributes
+    ----------
+    name: str
+        The name of the playlist.
+    tracks: :class:`SoundCloudTrack`
+        The list of :class:`SoundCloudTrack` in the playlist.
+    selected_track: Optional[int]
+        The selected video in the playlist. This could be ``None``.
+    """
+
+    def __init__(self, data: dict):
+        self.tracks: list[SoundCloudTrack] = []
+        self.name: str = data["playlistInfo"]["name"]
+
+        self.selected_track: Optional[int] = data["playlistInfo"].get("selectedTrack")
+        if self.selected_track is not None:
+            self.selected_track = int(self.selected_track)
+
+        for track_data in data["tracks"]:
+            track = SoundCloudTrack(track_data)
+            self.tracks.append(track)
+
+        self.source = TrackSource.SoundCloud
+
+    def __str__(self) -> str:
+        return self.name
```

### Comparing `Wavelink-2.6.0/wavelink/types/request.py` & `wavelink-2.6.1/wavelink/types/request.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, TypedDict
-
-from .state import VoiceState
-
-if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
-
-
-class Filters(TypedDict):
-    ...
-
-
-class _BaseRequest(TypedDict, total=False):
-    voice: VoiceState
-    position: int
-    endTime: int
-    volume: int
-    paused: bool
-    filters: Filters
-    voice: VoiceState
-
-
-class EncodedTrackRequest(_BaseRequest):
-    encodedTrack: str | None
-
-
-class IdentifierRequest(_BaseRequest):
-    identifier: str
-
-
-Request: TypeAlias = '_BaseRequest | EncodedTrackRequest | IdentifierRequest'
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, TypedDict
+
+from .state import VoiceState
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
+
+class Filters(TypedDict):
+    ...
+
+
+class _BaseRequest(TypedDict, total=False):
+    voice: VoiceState
+    position: int
+    endTime: int
+    volume: int
+    paused: bool
+    filters: Filters
+    voice: VoiceState
+
+
+class EncodedTrackRequest(_BaseRequest):
+    encodedTrack: str | None
+
+
+class IdentifierRequest(_BaseRequest):
+    identifier: str
+
+
+Request: TypeAlias = '_BaseRequest | EncodedTrackRequest | IdentifierRequest'
```

### Comparing `Wavelink-2.6.0/wavelink/websocket.py` & `wavelink-2.6.1/wavelink/websocket.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import asyncio
-import logging
-from typing import TYPE_CHECKING, Any, Optional
-
-import aiohttp
-
-import wavelink
-
-from . import __version__
-from .backoff import Backoff
-from .enums import NodeStatus, TrackEventType
-from .exceptions import *
-from .payloads import TrackEventPayload, WebsocketClosedPayload
-
-if TYPE_CHECKING:
-    from .node import Node
-    from .player import Player
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-class Websocket:
-
-    __slots__ = (
-        'node',
-        'socket',
-        'retries',
-        'retry',
-        '_original_attempts',
-        'backoff',
-        '_listener_task',
-        '_reconnect_task'
-    )
-
-    def __init__(self, *, node: Node) -> None:
-        self.node: Node = node
-        self.socket: aiohttp.ClientWebSocketResponse | None = None
-
-        self.retries: int | None = node._retries
-        self.retry: float = 1
-        self._original_attempts: int | None = node._retries
-
-        self.backoff: Backoff = Backoff()
-
-        self._listener_task: asyncio.Task | None = None
-        self._reconnect_task: asyncio.Task | None = None
-
-    @property
-    def headers(self) -> dict[str, str]:
-        assert self.node.client is not None
-        assert self.node.client.user is not None
-
-        return {
-            'Authorization': self.node.password,
-            'User-Id': str(self.node.client.user.id),
-            'Client-Name': f'Wavelink/{__version__}'
-        }
-
-    def is_connected(self) -> bool:
-        return self.socket is not None and not self.socket.closed
-
-    async def connect(self) -> None:
-        if self.node.status is NodeStatus.CONNECTED:
-            logger.error(f'Node {self.node} websocket tried connecting in an already connected state. '
-                         f'Disregarding.')
-            return
-
-        self.node._status = NodeStatus.CONNECTING
-
-        if self._listener_task:
-            try:
-                self._listener_task.cancel()
-            except Exception as e:
-                logger.debug(f'Node {self.node} encountered an error while cancelling the websocket listener: {e}. '
-                             f'This is likely not an issue and will not affect connection.')
-
-        uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
-
-        if self.node._use_http:
-            uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
-        else:
-            uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
-
-        heartbeat: float = self.node.heartbeat
-
-        try:
-            self.socket = await self.node._session.ws_connect(url=uri, heartbeat=heartbeat, headers=self.headers)
-        except Exception as e:
-            if isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 401:
-                raise AuthorizationFailed from e
-            else:
-                logger.error(f'An error occurred connecting to node: "{self.node}". {e}')
-
-        if self.is_connected():
-            self.retries = self._original_attempts
-            self._reconnect_task = None
-            # TODO - Configure Resuming...
-        else:
-            await self._reconnect()
-            return
-
-        self._listener_task = asyncio.create_task(self._listen())
-
-    async def _reconnect(self) -> None:
-        self.node._status = NodeStatus.CONNECTING
-        self.retry = self.backoff.calculate()
-
-        if self.retries == 0:
-            logger.error(f'Node {self.node} websocket was unable to connect, '
-                         f'and has exhausted the reconnection attempt limit. '
-                         'Please check your Lavalink Node is started and your connection details are correct.')
-
-            await self.cleanup()
-            return
-
-        retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
-        logger.error(f'Node {self.node} websocket was unable to connect, retrying connection in: '
-                     f'"{self.retry}" seconds. {retries}')
-
-        if self.retries:
-            self.retries -= 1
-
-        await asyncio.sleep(self.retry)
-        await self.connect()
-
-    async def _listen(self) -> None:
-        while True:
-            message = await self.socket.receive()
-
-            if message.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
-
-                for player in self.node.players.copy().values():
-                    await player._update_event(data=None)
-
-                self._reconnect_task = asyncio.create_task(self._reconnect())
-                return
-
-            if message.data == 1011:
-                logger.error(f'Node {self.node} websocket encountered an internal error which can not be resolved. '
-                             'Make sure your Lavalink sever is up to date, and try restarting.')
-
-                await self.cleanup()
-                return
-
-            if message.data is None:
-                logger.info(f'Node {self.node} websocket received a message from Lavalink with empty data. '
-                            f'Disregarding.')
-                continue
-
-            data = message.json()
-            logger.debug(f'Node {self.node} websocket received a message from Lavalink: {data}')
-
-            op = data.get('op', None)
-            if not op:
-                logger.info(f'Node {self.node} websocket payload "op" from Lavalink was None. Disregarding.')
-                continue
-
-            if op == 'ready':
-                self.node._status = NodeStatus.CONNECTED
-                self.node._session_id = data['sessionId']
-
-                self.dispatch('node_ready', self.node)
-
-            elif op == 'stats':
-                payload = ...
-                logger.debug(f'Node {self.node} websocket received a Stats Update payload: {data}')
-                self.dispatch('stats_update', data)
-
-            elif op == 'event':
-                logger.debug(f'Node {self.node} websocket received an event payload: {data}')
-                player = self.get_player(data)
-
-                if data['type'] == 'WebSocketClosedEvent':
-                    player = player or self.node._invalidated.get(int(data['guildId']), None)
-
-                    if not player:
-                        logger.debug(f'Node {self.node} received a WebsocketClosedEvent in an "unknown" state. '
-                                     f'Disregarding.')
-                        continue
-
-                    if self.node._invalidated.get(player.guild.id):
-                        await player._destroy()
-
-                    logger.debug(f'Node {self.node} websocket acknowledged "WebsocketClosedEvent": '
-                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>. '
-                                 f'Cleanup on player {player.guild.id} has been completed.')
-
-                    payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
-
-                    self.dispatch('websocket_closed', payload)
-                    continue
-
-                if player is None:
-                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
-                                 f'Disregarding.')
-                    continue
-
-                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
-                payload: TrackEventPayload = TrackEventPayload(
-                    data=data,
-                    track=track,
-                    player=player,
-                    original=player._original
-                )
-
-                if payload.event is TrackEventType.END and payload.reason != 'REPLACED':
-                    player._current = None
-
-                self.dispatch('track_event', payload)
-
-                if payload.event is TrackEventType.END:
-                    self.dispatch('track_end', payload)
-                    asyncio.create_task(player._auto_play_event(payload))
-
-                elif payload.event is TrackEventType.START:
-                    self.dispatch('track_start', payload)
-
-            elif op == 'playerUpdate':
-                player = self.get_player(data)
-                if player is None:
-                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
-                                 f'Disregarding.')
-                    continue
-
-                await player._update_event(data)
-                self.dispatch("player_update", data)
-                logger.debug(f'Node {self.node} websocket received Player Update payload: {data}')
-
-            else:
-                logger.warning(f'Received unknown payload from Lavalink: <{data}>. '
-                               f'If this continues consider making a ticket on the Wavelink GitHub. '
-                               f'https://github.com/PythonistaGuild/Wavelink')
-
-    def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
-        return self.node.players.get(int(payload['guildId']), None)
-
-    def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
-        self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
-        logger.debug(f'Node {self.node} is dispatching an event: "on_wavelink_{event}".')
-
-    # noinspection PyBroadException
-    async def cleanup(self) -> None:
-        try:
-            await self.socket.close()
-        except AttributeError:
-            pass
-
-        try:
-            self._listener_task.cancel()
-        except Exception:
-            pass
-
-        self.node._status = NodeStatus.DISCONNECTED
-
-        logger.debug(f'Successfully cleaned up websocket for node: {self.node}')
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import asyncio
+import logging
+from typing import TYPE_CHECKING, Any, Optional
+
+import aiohttp
+
+import wavelink
+
+from . import __version__
+from .backoff import Backoff
+from .enums import NodeStatus, TrackEventType
+from .exceptions import *
+from .payloads import TrackEventPayload, WebsocketClosedPayload
+
+if TYPE_CHECKING:
+    from .node import Node
+    from .player import Player
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+class Websocket:
+
+    __slots__ = (
+        'node',
+        'socket',
+        'retries',
+        'retry',
+        '_original_attempts',
+        'backoff',
+        '_listener_task',
+        '_reconnect_task'
+    )
+
+    def __init__(self, *, node: Node) -> None:
+        self.node: Node = node
+        self.socket: aiohttp.ClientWebSocketResponse | None = None
+
+        self.retries: int | None = node._retries
+        self.retry: float = 1
+        self._original_attempts: int | None = node._retries
+
+        self.backoff: Backoff = Backoff()
+
+        self._listener_task: asyncio.Task | None = None
+        self._reconnect_task: asyncio.Task | None = None
+
+    @property
+    def headers(self) -> dict[str, str]:
+        assert self.node.client is not None
+        assert self.node.client.user is not None
+
+        return {
+            'Authorization': self.node.password,
+            'User-Id': str(self.node.client.user.id),
+            'Client-Name': f'Wavelink/{__version__}'
+        }
+
+    def is_connected(self) -> bool:
+        return self.socket is not None and not self.socket.closed
+
+    async def connect(self) -> None:
+        if self.node.status is NodeStatus.CONNECTED:
+            logger.error(f'Node {self.node} websocket tried connecting in an already connected state. '
+                         f'Disregarding.')
+            return
+
+        self.node._status = NodeStatus.CONNECTING
+
+        if self._listener_task:
+            try:
+                self._listener_task.cancel()
+            except Exception as e:
+                logger.debug(f'Node {self.node} encountered an error while cancelling the websocket listener: {e}. '
+                             f'This is likely not an issue and will not affect connection.')
+
+        uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
+
+        if self.node._use_http:
+            uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
+        else:
+            uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
+
+        heartbeat: float = self.node.heartbeat
+
+        try:
+            self.socket = await self.node._session.ws_connect(url=uri, heartbeat=heartbeat, headers=self.headers)
+        except Exception as e:
+            if isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 401:
+                raise AuthorizationFailed from e
+            else:
+                logger.error(f'An error occurred connecting to node: "{self.node}". {e}')
+
+        if self.is_connected():
+            self.retries = self._original_attempts
+            self._reconnect_task = None
+            # TODO - Configure Resuming...
+        else:
+            await self._reconnect()
+            return
+
+        self._listener_task = asyncio.create_task(self._listen())
+
+    async def _reconnect(self) -> None:
+        self.node._status = NodeStatus.CONNECTING
+        self.retry = self.backoff.calculate()
+
+        if self.retries == 0:
+            logger.error(f'Node {self.node} websocket was unable to connect, '
+                         f'and has exhausted the reconnection attempt limit. '
+                         'Please check your Lavalink Node is started and your connection details are correct.')
+
+            await self.cleanup()
+            return
+
+        retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
+        logger.error(f'Node {self.node} websocket was unable to connect, retrying connection in: '
+                     f'"{self.retry}" seconds. {retries}')
+
+        if self.retries:
+            self.retries -= 1
+
+        await asyncio.sleep(self.retry)
+        await self.connect()
+
+    async def _listen(self) -> None:
+        while True:
+            message = await self.socket.receive()
+
+            if message.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
+
+                for player in self.node.players.copy().values():
+                    await player._update_event(data=None)
+
+                self._reconnect_task = asyncio.create_task(self._reconnect())
+                return
+
+            if message.data == 1011:
+                logger.error(f'Node {self.node} websocket encountered an internal error which can not be resolved. '
+                             'Make sure your Lavalink sever is up to date, and try restarting.')
+
+                await self.cleanup()
+                return
+
+            if message.data is None:
+                logger.info(f'Node {self.node} websocket received a message from Lavalink with empty data. '
+                            f'Disregarding.')
+                continue
+
+            data = message.json()
+            logger.debug(f'Node {self.node} websocket received a message from Lavalink: {data}')
+
+            op = data.get('op', None)
+            if not op:
+                logger.info(f'Node {self.node} websocket payload "op" from Lavalink was None. Disregarding.')
+                continue
+
+            if op == 'ready':
+                self.node._status = NodeStatus.CONNECTED
+                self.node._session_id = data['sessionId']
+
+                self.dispatch('node_ready', self.node)
+
+            elif op == 'stats':
+                payload = ...
+                logger.debug(f'Node {self.node} websocket received a Stats Update payload: {data}')
+                self.dispatch('stats_update', data)
+
+            elif op == 'event':
+                logger.debug(f'Node {self.node} websocket received an event payload: {data}')
+                player = self.get_player(data)
+
+                if data['type'] == 'WebSocketClosedEvent':
+                    player = player or self.node._invalidated.get(int(data['guildId']), None)
+
+                    if not player:
+                        logger.debug(f'Node {self.node} received a WebsocketClosedEvent in an "unknown" state. '
+                                     f'Disregarding.')
+                        continue
+
+                    if self.node._invalidated.get(player.guild.id):
+                        await player._destroy()
+
+                    logger.debug(f'Node {self.node} websocket acknowledged "WebsocketClosedEvent": '
+                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>. '
+                                 f'Cleanup on player {player.guild.id} has been completed.')
+
+                    payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
+
+                    self.dispatch('websocket_closed', payload)
+                    continue
+
+                if player is None:
+                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
+                                 f'Disregarding.')
+                    continue
+
+                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
+                payload: TrackEventPayload = TrackEventPayload(
+                    data=data,
+                    track=track,
+                    player=player,
+                    original=player._original
+                )
+
+                if payload.event is TrackEventType.END and payload.reason != 'REPLACED':
+                    player._current = None
+
+                self.dispatch('track_event', payload)
+
+                if payload.event is TrackEventType.END:
+                    self.dispatch('track_end', payload)
+                    asyncio.create_task(player._auto_play_event(payload))
+
+                elif payload.event is TrackEventType.START:
+                    self.dispatch('track_start', payload)
+
+            elif op == 'playerUpdate':
+                player = self.get_player(data)
+                if player is None:
+                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
+                                 f'Disregarding.')
+                    continue
+
+                await player._update_event(data)
+                self.dispatch("player_update", data)
+                logger.debug(f'Node {self.node} websocket received Player Update payload: {data}')
+
+            else:
+                logger.warning(f'Received unknown payload from Lavalink: <{data}>. '
+                               f'If this continues consider making a ticket on the Wavelink GitHub. '
+                               f'https://github.com/PythonistaGuild/Wavelink')
+
+    def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
+        return self.node.players.get(int(payload['guildId']), None)
+
+    def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
+        self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
+        logger.debug(f'Node {self.node} is dispatching an event: "on_wavelink_{event}".')
+
+    # noinspection PyBroadException
+    async def cleanup(self) -> None:
+        try:
+            await self.socket.close()
+        except AttributeError:
+            pass
+
+        try:
+            self._listener_task.cancel()
+        except Exception:
+            pass
+
+        self.node._status = NodeStatus.DISCONNECTED
+
+        logger.debug(f'Successfully cleaned up websocket for node: {self.node}')
```

