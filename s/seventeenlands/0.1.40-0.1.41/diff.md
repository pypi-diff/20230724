# Comparing `tmp/seventeenlands-0.1.40.tar.gz` & `tmp/seventeenlands-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventeenlands-0.1.40.tar", last modified: Mon Jul 10 22:10:12 2023, max compression
+gzip compressed data, was "seventeenlands-0.1.41.tar", last modified: Mon Jul 24 01:18:26 2023, max compression
```

## Comparing `seventeenlands-0.1.40.tar` & `seventeenlands-0.1.41.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/
--rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      585 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/README.md
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      839 2023-07-10 22:10:05.000000 seventeenlands-0.1.40/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/seventeenlands/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/seventeenlands/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     4461 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/api_client.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1040 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/logging_utils.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    55087 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/mtga_follower.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2301 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/retry_utils.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/seventeenlands.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      406 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       70 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       15 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-24 01:18:26.263238 seventeenlands-0.1.41/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2023-05-24 15:00:01.000000 seventeenlands-0.1.41/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-24 01:18:26.263238 seventeenlands-0.1.41/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      585 2023-05-24 15:00:01.000000 seventeenlands-0.1.41/README.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-07-24 01:18:26.263238 seventeenlands-0.1.41/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      839 2023-07-24 01:18:14.000000 seventeenlands-0.1.41/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-24 01:18:26.263238 seventeenlands-0.1.41/seventeenlands/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-24 15:00:01.000000 seventeenlands-0.1.41/seventeenlands/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4461 2023-07-24 01:17:24.000000 seventeenlands-0.1.41/seventeenlands/api_client.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1040 2023-07-24 01:17:24.000000 seventeenlands-0.1.41/seventeenlands/logging_utils.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    55814 2023-07-24 01:17:24.000000 seventeenlands-0.1.41/seventeenlands/mtga_follower.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2301 2023-07-24 01:17:24.000000 seventeenlands-0.1.41/seventeenlands/retry_utils.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-24 01:18:26.263238 seventeenlands-0.1.41/seventeenlands.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      406 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       70 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       15 2023-07-24 01:18:26.000000 seventeenlands-0.1.41/seventeenlands.egg-info/top_level.txt
```

### Comparing `seventeenlands-0.1.40/LICENSE` & `seventeenlands-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.40/PKG-INFO` & `seventeenlands-0.1.41/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.40
+Version: 0.1.41
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seventeenlands-0.1.40/README.md` & `seventeenlands-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.40/setup.py` & `seventeenlands-0.1.41/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seventeenlands",
-    version="0.1.40",
+    version="0.1.41",
     author="Robert Conroy",
     author_email="seventeenlands@gmail.com",
     description="Utility to upload MTG Arena data to 17Lands.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rconroy293/mtga-log-client",
     packages=setuptools.find_packages(),
```

### Comparing `seventeenlands-0.1.40/seventeenlands/api_client.py` & `seventeenlands-0.1.41/seventeenlands/api_client.py`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.40/seventeenlands/logging_utils.py` & `seventeenlands-0.1.41/seventeenlands/logging_utils.py`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.40/seventeenlands/mtga_follower.py` & `seventeenlands-0.1.41/seventeenlands/mtga_follower.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import dateutil.parser
 
 import seventeenlands.api_client
 import seventeenlands.logging_utils
 
 logger = seventeenlands.logging_utils.get_logger('17Lands')
 
-CLIENT_VERSION = '0.1.40.p'
+CLIENT_VERSION = '0.1.41.p'
 
 UPDATE_CHECK_INTERVAL = datetime.timedelta(hours=1)
 UPDATE_PROMPT_FREQUENCY = 24
 
 TOKEN_ENTRY_TITLE = 'MTGA Log Client Token'
 TOKEN_ENTRY_MESSAGE = 'Please enter your client token from 17lands.com/account: '
 TOKEN_MISSING_TITLE = 'Error: Client Token Needed'
@@ -244,14 +244,15 @@
         self.user_screen_name = None
         self.screen_names = defaultdict(lambda: '')
         self.game_history_events = []
         self.pending_game_submission = {}
         self.pending_game_result = {}
         self.pending_match_result = {}
 
+        self.last_blob = ''
         self.current_debug_blob = ''
         self.recent_lines = []
 
         self.__clear_match_data()
 
     def _add_base_api_data(self, blob):
         return {
@@ -272,26 +273,23 @@
         :param follow:   Whether or not to continue looking for updates to the file after parsing
                          all the initial lines.
         """
         while True:
             self._reinitialize()
             last_read_time = time.time()
             last_file_size = 0
-            last_line = ''
             try:
                 with open(filename, errors='replace') as f:
                     while True:
                         line = f.readline()
                         file_size = pathlib.Path(filename).stat().st_size
                         if line:
-                            if line != last_line:
-                                self.__append_line(line)
+                            self.__append_line(line)
                             last_read_time = time.time()
                             last_file_size = file_size
-                            last_line = line
                         else:
                             self.__handle_complete_log_entry()
                             last_modified_time = os.stat(filename).st_mtime
                             if file_size < last_file_size:
                                 logger.info(f'Starting from beginning of file as file is smaller than before (previous = {last_file_size}; current = {file_size})')
                                 break
                             elif last_modified_time > last_read_time + FILE_UPDATED_FORCE_REFRESH_SECONDS:
@@ -371,22 +369,27 @@
             return
         if self.cur_log_time is None:
             self.buffer = []
             return
 
         full_log = ''.join(self.buffer)
         self.current_debug_blob = full_log
-        try:
-            self.__handle_blob(full_log)
-        except Exception as e:
-            self._log_error(
-                message=f'Error {e} while processing {full_log}',
-                error=e,
-                stacktrace=traceback.format_exc(),
-            )
+        if full_log != self.last_blob:
+            try:
+                self.__handle_blob(full_log)
+            except Exception as e:
+                self._log_error(
+                    message=f'Error {e} while processing {full_log}',
+                    error=e,
+                    stacktrace=traceback.format_exc(),
+                )
+
+            self.last_blob = full_log
+        else:
+            logger.info(f'Skipping repeated complete log entry: {full_log}')
 
         self.buffer = []
         # self.cur_log_time = None
 
     def __maybe_get_utc_timestamp(self, blob):
         timestamp = None
         if 'timestamp' in blob:
@@ -586,14 +589,17 @@
             self._add_to_game_history(message_blob, timestamp)
         elif message_blob['type'] == 'GREMessageType_UIMessage' and 'onChat' in message_blob['uiMessage']:
             self._add_to_game_history(message_blob, timestamp)
 
         if message_blob['type'] == 'GREMessageType_ConnectResp':
             self.__handle_gre_connect_response(message_blob)
 
+        elif message_blob['type'] == 'GREMessageType_EdictalMessage':
+            self.__handle_gre_edictal_message(message_blob, timestamp)
+
         elif message_blob['type'] == 'GREMessageType_GameStateMessage':
             try:
                 system_seat_ids = message_blob.get('systemSeatIds', [])
                 if len(system_seat_ids) > 0:
                     self.seat_id = system_seat_ids[0]
 
                 game_state_message = message_blob.get('gameStateMessage', {})
@@ -709,14 +715,27 @@
         except Exception as e:
             self._log_error(
                 message=f'Error {e} parsing GRE to client UI messages from {payload}',
                 error=e,
                 stacktrace=traceback.format_exc(),
             )
 
+    def __handle_gre_edictal_message(self, payload, timestamp):
+        try:
+            edictMessage = payload.get('edictalMessage', {}).get('edictMessage', {})
+            return self.__handle_client_to_gre_message(edictMessage, timestamp=timestamp)
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing edictal message from {payload}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+
     def __handle_log_business_game_end(self, payload):
         try:
             if self.starting_team_id is None:
                 self.starting_team_id = payload.get('StartingTeamId')
 
             if self.__enqueue_game_data():
                 self.pending_game_result = {
```

### Comparing `seventeenlands-0.1.40/seventeenlands/retry_utils.py` & `seventeenlands-0.1.41/seventeenlands/retry_utils.py`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.40/seventeenlands.egg-info/PKG-INFO` & `seventeenlands-0.1.41/seventeenlands.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.40
+Version: 0.1.41
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

