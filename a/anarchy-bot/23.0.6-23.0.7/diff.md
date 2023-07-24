# Comparing `tmp/anarchy_bot-23.0.6.tar.gz` & `tmp/anarchy_bot-23.0.7.tar.gz`

## Comparing `anarchy_bot-23.0.6.tar` & `anarchy_bot-23.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/build.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/changlog.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/pyrightconfig.json
--rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/setup.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/__main__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/cb.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/chats.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/common.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/config.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/inline.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/lang.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/lists.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/main.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/msg.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/anarchy_bot/lang/en.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/.gitignore
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/pyproject.toml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/readme.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 anarchy_bot-23.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/build.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/changlog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/pyrightconfig.json
+-rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/setup.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/__main__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/cb.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/chats.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/common.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/inline.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lang.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lists.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/main.py
+-rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/msg.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/anarchy_bot/lang/en.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/.gitignore
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/pyproject.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/readme.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 anarchy_bot-23.0.7/PKG-INFO
```

### Comparing `anarchy_bot-23.0.6/build.py` & `anarchy_bot-23.0.7/build.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/setup.py` & `anarchy_bot-23.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/cb.py` & `anarchy_bot-23.0.7/anarchy_bot/cb.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/chats.py` & `anarchy_bot-23.0.7/anarchy_bot/chats.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/common.py` & `anarchy_bot-23.0.7/anarchy_bot/common.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/config.py` & `anarchy_bot-23.0.7/anarchy_bot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import tgcrypto # type: ignore
     using_tgcrypto = True
 except Exception:
     using_tgcrypto = False
 
 
 app_name = 'anarchy_bot'
-app_version = '23.0.6'
+app_version = '23.0.7'
 c = rich.console.Console()
 c.log(f'imported [deep_sky_blue1]{__file__}')
 app_path = Path(
     __file__
 ).parent.parent.resolve()
 src_path = app_path / app_name
 data_path = app_path / f'{app_name}_data'
```

### Comparing `anarchy_bot-23.0.6/anarchy_bot/inline.py` & `anarchy_bot-23.0.7/anarchy_bot/inline.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/lang.py` & `anarchy_bot-23.0.7/anarchy_bot/lang.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/lists.py` & `anarchy_bot-23.0.7/anarchy_bot/lists.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/main.py` & `anarchy_bot-23.0.7/anarchy_bot/main.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/anarchy_bot/msg.py` & `anarchy_bot-23.0.7/anarchy_bot/msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         )
 
 
 def is_command(
     msg_text: str,
     command: str,
 ) -> bool:
+    if msg_text == command:
+        return True
     if msg_text.startswith(command + ' '):
         return True
     if msg_text.startswith(f'{command}@{config.me.username}'):
         return True
     return False
```

### Comparing `anarchy_bot-23.0.6/anarchy_bot/lang/en.yml` & `anarchy_bot-23.0.7/anarchy_bot/lang/en.yml`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/pyproject.toml` & `anarchy_bot-23.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [ "gmanka_yml==23.0.*", "pyrogram==2.0.*", "tgcrypto==1.2.*", "uvloop==0.17.*", "rich==13.4.*",]
 name = "anarchy_bot"
-version = "23.0.6"
+version = "23.0.7"
 description = "telegram bot that can add users to minecraft whitelist"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `anarchy_bot-23.0.6/readme.md` & `anarchy_bot-23.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.6/PKG-INFO` & `anarchy_bot-23.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anarchy_bot
-Version: 23.0.6
+Version: 23.0.7
 Summary: telegram bot that can add users to minecraft whitelist
 Project-URL: Documentation, https://t.me/gmanka
 Project-URL: Bug Tracker, https://t.me/gmanka
 Project-URL: Homepage, https://t.me/gmanka
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

