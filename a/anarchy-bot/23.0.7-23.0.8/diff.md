# Comparing `tmp/anarchy_bot-23.0.7.tar.gz` & `tmp/anarchy_bot-23.0.8.tar.gz`

## Comparing `anarchy_bot-23.0.7.tar` & `anarchy_bot-23.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/build.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/changlog.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/pyrightconfig.json
--rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/setup.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/__main__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/cb.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/chats.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/common.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/config.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/inline.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lang.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lists.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/main.py
--rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/msg.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lang/en.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/.gitignore
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/pyproject.toml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/readme.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/build.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/changlog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/pyrightconfig.json
+-rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/setup.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/__main__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/cb.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/chats.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/common.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/inline.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/lang.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/lists.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/main.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/msg.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/anarchy_bot/lang/en.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/.gitignore
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/pyproject.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/readme.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 anarchy_bot-23.0.8/PKG-INFO
```

### Comparing `anarchy_bot-23.0.7/build.py` & `anarchy_bot-23.0.8/build.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/setup.py` & `anarchy_bot-23.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/cb.py` & `anarchy_bot-23.0.8/anarchy_bot/cb.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/chats.py` & `anarchy_bot-23.0.8/anarchy_bot/chats.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/common.py` & `anarchy_bot-23.0.8/anarchy_bot/common.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/config.py` & `anarchy_bot-23.0.8/anarchy_bot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import tgcrypto # type: ignore
     using_tgcrypto = True
 except Exception:
     using_tgcrypto = False
 
 
 app_name = 'anarchy_bot'
-app_version = '23.0.7'
+app_version = '23.0.8'
 c = rich.console.Console()
 c.log(f'imported [deep_sky_blue1]{__file__}')
 app_path = Path(
     __file__
 ).parent.parent.resolve()
 src_path = app_path / app_name
 data_path = app_path / f'{app_name}_data'
```

### Comparing `anarchy_bot-23.0.7/anarchy_bot/inline.py` & `anarchy_bot-23.0.8/anarchy_bot/inline.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/lang.py` & `anarchy_bot-23.0.8/anarchy_bot/lang.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/lists.py` & `anarchy_bot-23.0.8/anarchy_bot/lists.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/main.py` & `anarchy_bot-23.0.8/anarchy_bot/main.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/anarchy_bot/msg.py` & `anarchy_bot-23.0.8/anarchy_bot/msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,17 @@
             msg.text,
             excpected_msg,
         ):
             if await filter_admin(msg):
                 return
             return await to_run(client, msg)
     if msg.chat.type == pg.enums.ChatType.PRIVATE:
-        await msg.reply(
-            **get_main_message(msg)
+        await help_msg(
+            client,
+            msg,
         )
         return
 
 
 async def help_msg(
     client: Client,
     msg: Message,
@@ -140,15 +141,15 @@
             msg,
         ).strip(
             '"""'
         ).strip(
             '"""\n'
         )
         await msg.reply(
-            t(text, msg)
+            text
         )
 
 
 async def becomeadmin(
     client: Client,
     msg: Message,
 ):
```

### Comparing `anarchy_bot-23.0.7/anarchy_bot/lang/en.yml` & `anarchy_bot-23.0.8/anarchy_bot/lang/en.yml`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/pyproject.toml` & `anarchy_bot-23.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [ "gmanka_yml==23.0.*", "pyrogram==2.0.*", "tgcrypto==1.2.*", "uvloop==0.17.*", "rich==13.4.*",]
 name = "anarchy_bot"
-version = "23.0.7"
+version = "23.0.8"
 description = "telegram bot that can add users to minecraft whitelist"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `anarchy_bot-23.0.7/readme.md` & `anarchy_bot-23.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.7/PKG-INFO` & `anarchy_bot-23.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anarchy_bot
-Version: 23.0.7
+Version: 23.0.8
 Summary: telegram bot that can add users to minecraft whitelist
 Project-URL: Documentation, https://t.me/gmanka
 Project-URL: Bug Tracker, https://t.me/gmanka
 Project-URL: Homepage, https://t.me/gmanka
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

