# Comparing `tmp/utilspkg-0.3.2.tar.gz` & `tmp/utilspkg-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilspkg-0.3.2.tar", last modified: Sun Jul  9 23:44:50 2023, max compression
+gzip compressed data, was "utilspkg-0.3.3.tar", last modified: Mon Jul 24 15:49:43 2023, max compression
```

## Comparing `utilspkg-0.3.2.tar` & `utilspkg-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.839333 utilspkg-0.3.2/
--rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-09 23:44:50.839228 utilspkg-0.3.2/PKG-INFO
--rw-r--r--   0 croft      (501) staff       (20)       86 2023-06-26 21:37:37.000000 utilspkg-0.3.2/pyproject.toml
--rw-r--r--   0 croft      (501) staff       (20)       38 2023-07-09 23:44:50.839372 utilspkg-0.3.2/setup.cfg
--rw-r--r--   0 croft      (501) staff       (20)      422 2023-07-02 14:31:40.000000 utilspkg-0.3.2/setup.py
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.838618 utilspkg-0.3.2/utilspkg/
--rw-r--r--   0 croft      (501) staff       (20)     1053 2023-06-26 19:52:42.000000 utilspkg-0.3.2/utilspkg/__init__.py
--rw-r--r--   0 croft      (501) staff       (20)     3460 2023-06-26 19:52:59.000000 utilspkg-0.3.2/utilspkg/utils_db.py
--rw-r--r--   0 croft      (501) staff       (20)     2206 2023-06-26 19:53:12.000000 utilspkg-0.3.2/utilspkg/utils_email.py
--rw-r--r--   0 croft      (501) staff       (20)     3375 2023-06-26 19:53:16.000000 utilspkg-0.3.2/utilspkg/utils_gpt.py
--rw-r--r--   0 croft      (501) staff       (20)     1661 2023-07-02 00:32:38.000000 utilspkg-0.3.2/utilspkg/utils_init.py
--rw-r--r--   0 croft      (501) staff       (20)      764 2023-06-26 01:09:40.000000 utilspkg-0.3.2/utilspkg/utils_misc.py
--rw-r--r--   0 croft      (501) staff       (20)     6775 2023-07-02 00:46:04.000000 utilspkg-0.3.2/utilspkg/utils_slack.py
--rw-r--r--   0 croft      (501) staff       (20)     3353 2023-06-26 01:09:40.000000 utilspkg-0.3.2/utilspkg/utils_time.py
--rw-r--r--   0 croft      (501) staff       (20)     2947 2023-07-09 23:40:36.000000 utilspkg-0.3.2/utilspkg/utils_times.py
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.839051 utilspkg-0.3.2/utilspkg.egg-info/
--rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/PKG-INFO
--rw-r--r--   0 croft      (501) staff       (20)      356 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/SOURCES.txt
--rw-r--r--   0 croft      (501) staff       (20)        1 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/dependency_links.txt
--rw-r--r--   0 croft      (501) staff       (20)        9 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/top_level.txt
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-24 15:49:43.000853 utilspkg-0.3.3/
+-rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-24 15:49:43.000748 utilspkg-0.3.3/PKG-INFO
+-rw-r--r--   0 croft      (501) staff       (20)       86 2023-06-26 21:37:37.000000 utilspkg-0.3.3/pyproject.toml
+-rw-r--r--   0 croft      (501) staff       (20)       38 2023-07-24 15:49:43.000892 utilspkg-0.3.3/setup.cfg
+-rw-r--r--   0 croft      (501) staff       (20)      422 2023-07-24 15:49:39.000000 utilspkg-0.3.3/setup.py
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-24 15:49:43.000171 utilspkg-0.3.3/utilspkg/
+-rw-r--r--   0 croft      (501) staff       (20)     1053 2023-06-26 19:52:42.000000 utilspkg-0.3.3/utilspkg/__init__.py
+-rw-r--r--   0 croft      (501) staff       (20)     3460 2023-06-26 19:52:59.000000 utilspkg-0.3.3/utilspkg/utils_db.py
+-rw-r--r--   0 croft      (501) staff       (20)     2206 2023-06-26 19:53:12.000000 utilspkg-0.3.3/utilspkg/utils_email.py
+-rw-r--r--   0 croft      (501) staff       (20)     3375 2023-06-26 19:53:16.000000 utilspkg-0.3.3/utilspkg/utils_gpt.py
+-rw-r--r--   0 croft      (501) staff       (20)     1661 2023-07-02 00:32:38.000000 utilspkg-0.3.3/utilspkg/utils_init.py
+-rw-r--r--   0 croft      (501) staff       (20)      764 2023-06-26 01:09:40.000000 utilspkg-0.3.3/utilspkg/utils_misc.py
+-rw-r--r--   0 croft      (501) staff       (20)     7150 2023-07-23 23:56:30.000000 utilspkg-0.3.3/utilspkg/utils_slack.py
+-rw-r--r--   0 croft      (501) staff       (20)     3353 2023-06-26 01:09:40.000000 utilspkg-0.3.3/utilspkg/utils_time.py
+-rw-r--r--   0 croft      (501) staff       (20)     2947 2023-07-09 23:40:36.000000 utilspkg-0.3.3/utilspkg/utils_times.py
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-24 15:49:43.000599 utilspkg-0.3.3/utilspkg.egg-info/
+-rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-24 15:49:42.000000 utilspkg-0.3.3/utilspkg.egg-info/PKG-INFO
+-rw-r--r--   0 croft      (501) staff       (20)      356 2023-07-24 15:49:42.000000 utilspkg-0.3.3/utilspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 croft      (501) staff       (20)        1 2023-07-24 15:49:42.000000 utilspkg-0.3.3/utilspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 croft      (501) staff       (20)        9 2023-07-24 15:49:42.000000 utilspkg-0.3.3/utilspkg.egg-info/top_level.txt
```

### Comparing `utilspkg-0.3.2/utilspkg/__init__.py` & `utilspkg-0.3.3/utilspkg/__init__.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_db.py` & `utilspkg-0.3.3/utilspkg/utils_db.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_email.py` & `utilspkg-0.3.3/utilspkg/utils_email.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_gpt.py` & `utilspkg-0.3.3/utilspkg/utils_gpt.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_init.py` & `utilspkg-0.3.3/utilspkg/utils_init.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_misc.py` & `utilspkg-0.3.3/utilspkg/utils_misc.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_slack.py` & `utilspkg-0.3.3/utilspkg/utils_slack.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,31 @@
 
         channel_or_slack_id = channel_or_slack_id if not testing_flag else self.testing_dm_or_channel
 
         if channel_or_slack_id.startswith("U"):  # check if it's a user ID
             dm = self.slack_client.conversations_open(users=channel_or_slack_id)
             channel_or_slack_id = dm['channel']['id']
 
-        response = self.slack_client.chat_postMessage(
-            channel=channel_or_slack_id,
-            text=message,
-            thread_ts=thread_ts,  # ok if None
-            unfurl_links=False,
-            unfurl_media=False)
-        
+        # empty dictionary
+        response = {}
+
+        #handle corner case of message being empty
+        if not message:
+            logger.error(f"Message is empty")
+            response['ok'] = False
+            response['error'] = "ERROR: Tried to send empty message on Slack via slackutils"
+        else:
+            #proceeding as normal
+            response = self.slack_client.chat_postMessage(
+                channel=channel_or_slack_id,
+                text=message,
+                thread_ts=thread_ts,  # ok if None
+                unfurl_links=False,
+                unfurl_media=False)
+            
         return response
 
     def get_list_of_channels(self, bool_public_channels=True, bool_private_channels=True, exclude_archived=True):
         '''https://api.slack.com/methods/conversations.list
             Returns the conversations_list() result of 'all channels
             The object can then be iterated over (for channel in all_channels). Some properties:
             channel_id = channel["id"]
```

### Comparing `utilspkg-0.3.2/utilspkg/utils_time.py` & `utilspkg-0.3.3/utilspkg/utils_time.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.2/utilspkg/utils_times.py` & `utilspkg-0.3.3/utilspkg/utils_times.py`

 * *Files identical despite different names*

