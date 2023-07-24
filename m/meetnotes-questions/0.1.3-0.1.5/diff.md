# Comparing `tmp/meetnotes_questions-0.1.3-py3-none-any.whl.zip` & `tmp/meetnotes_questions-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4714 bytes, number of entries: 9
+Zip file size: 4968 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       75 b- defN 23-Jul-24 18:38 meetnotes_questions/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jul-24 18:37 meetnotes_questions/__main__.py
--rw-r--r--  2.0 unx     4301 b- defN 23-Jul-24 20:43 meetnotes_questions/meetnotes_questions.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/RECORD
-9 files, 6970 bytes uncompressed, 3250 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx     5156 b- defN 23-Jul-24 21:27 meetnotes_questions/meetnotes_questions.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 21:27 meetnotes_questions-0.1.5.dist-info/RECORD
+9 files, 7825 bytes uncompressed, 3504 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: meetnotes_questions/__main__.py
 Comment: 
 
 Filename: meetnotes_questions/meetnotes_questions.py
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/LICENSE.txt
+Filename: meetnotes_questions-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/METADATA
+Filename: meetnotes_questions-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/WHEEL
+Filename: meetnotes_questions-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/entry_points.txt
+Filename: meetnotes_questions-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/top_level.txt
+Filename: meetnotes_questions-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.3.dist-info/RECORD
+Filename: meetnotes_questions-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meetnotes_questions/meetnotes_questions.py

```diff
@@ -1,15 +1,14 @@
 import asyncio
-import hashlib
+import fnmatch
 import json
 import os
 import queue
+import re
 import sys
-import threading
-import time
 
 import openai
 import tiktoken
 from dotenv import load_dotenv
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
@@ -35,37 +34,44 @@
 
 class FileWatcher(FileSystemEventHandler):
     def __init__(self, event_queue):
         super().__init__()
         self.queue = event_queue
 
     def on_modified(self, event):
-        print("File modified event triggered.")
-        self.queue.put(("modified", event))
-        print("File modified event processed.")
+        if self._check_file(event.src_path):
+            print("File modified event triggered.")
+            self.queue.put(("modified", event))
+            print("File modified event processed.")
 
     def on_created(self, event):
-        print("File created event triggered.")
-        self.queue.put(("created", event))
-        print("File created event processed.")
+        if self._check_file(event.src_path):
+            print("File created event triggered.")
+            self.queue.put(("created", event))
+            print("File created event processed.")
 
     def on_deleted(self, event):
-        print("File deleted event triggered.")
-        self.queue.put(("deleted", event))
-        print("File deleted event processed.")
+        if self._check_file(event.src_path):
+            print("File deleted event triggered.")
+            self.queue.put(("deleted", event))
+            print("File deleted event processed.")
+
+    def _check_file(self, file_path):
+        filename = os.path.basename(file_path)
+        return fnmatch.fnmatch(filename, "2023*.txt")
 
 
 def process_file(file_path):
     print(f"File: {file_path}", file=sys.stderr)
-    file_content = open(file_path, "rt").read()
+    file_content = open(file_path, "r", encoding="utf-8-sig").read()
     messages = parse_conversation(file_content)
     print("Messages:", messages)
     system_message = {
         "role": "system",
-        "content": 'You are a junior staff member at a company, and trying to learn more about the business and domain. You are transcribing notes between yourself, your colleagues, and clients/prospects. "Me" means messages by me. Propose one or two intelligent question to ask in the meeting.',
+        "content": "You are a junior staff member at a company, and trying to learn more about the business and domain. You are transcribing notes between yourself, your colleagues, and clients/prospects as bullet points. Propose one or two intelligent question to ask in the meeting.",
     }
     kept_messages = []
     for message in reversed(messages):
         total_text = json.dumps([system_message] + [message] + kept_messages)
         if len(enc.encode(total_text)) > MAX_TOKENS:
             break
         kept_messages = [message] + kept_messages
@@ -99,14 +105,15 @@
         event_type, event = event_queue.get()
         print("Got event: ", event_type, event)
         process_event(event_type, event)
         event_queue.task_done()
     observer.join()
 
 
+"""
 def parse_conversation(text):
     segments = text.split("[")[1:]  # Exclude the first split as it will be empty
     conversation = []
     for segment in segments:
         speaker, paragraphs = segment.split("]: ", 1)
         if len(speaker) > 24:
             continue  # Skip the speaker names that are longer than 24 characters
@@ -114,25 +121,44 @@
         conversation.append(
             {
                 "role": "user",
                 "content": f"{speaker}: {' '.join(paragraphs.splitlines())}",
             }
         )
     return conversation
+"""
+
+
+def parse_conversation(text):
+    messages = re.split("\n\s*\*", text)
+    messages = [message.strip() for message in messages if message.strip()]
+
+    conversation = [{"role": "user", "content": message} for message in messages]
+
+    print(conversation)
+
+    return conversation
+
+
+# text = "* New meeting with TestCompany\n   * They are not yet a customer (*note that they want to become a customer)\n* They are in construction.\nThey are are Test Company.\n* They want lightning data."
+
+
+# def main():
+#    parse_conversation(text)
 
 
 async def real_main():
     openai_token = os.environ.get("OPENAI_TOKEN")
     assert openai_token, "OPENAI_TOKEN not found in the environment variables."
     openai.api_key = openai_token
-    notes_directory = "~/notes"
+    notes_directory = "~/Downloads/"
     absolute_dir_path = os.path.expanduser(notes_directory)
     assert os.path.isdir(absolute_dir_path), f"Directory not found: {absolute_dir_path}"
     await begin_watching(absolute_dir_path)
 
 
-def main():
-    asyncio.run(real_main())
+# def main():
+#    asyncio.run(real_main())
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `meetnotes_questions-0.1.3.dist-info/LICENSE.txt` & `meetnotes_questions-0.1.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `meetnotes_questions-0.1.3.dist-info/RECORD` & `meetnotes_questions-0.1.5.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 meetnotes_questions/__init__.py,sha256=ozuBNNUzpClNmd99Mrf9nyDde19z_pHY9pN-_20H_Os,75
 meetnotes_questions/__main__.py,sha256=CX1YQrso4UHQcl9jdGvRc7sixnz8LRo0S6ON9sIyIEo,106
-meetnotes_questions/meetnotes_questions.py,sha256=OR38QvHyGLtfnl0KXFIU3B4F3-yLS4MlJCkPXToXJkc,4301
-meetnotes_questions-0.1.3.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-meetnotes_questions-0.1.3.dist-info/METADATA,sha256=5DpNyjOiX_utDcLrD30twHOcQ45HHjbDz6DBISdMElY,397
-meetnotes_questions-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-meetnotes_questions-0.1.3.dist-info/entry_points.txt,sha256=guo3Be5mJa7c9qf5Lo-POBF0-6yofE3CJUFwGzBSG0A,70
-meetnotes_questions-0.1.3.dist-info/top_level.txt,sha256=23fGx0TLjLVsFol8ZjWXZcgm6UF_KDmQATQUMBbnPj4,20
-meetnotes_questions-0.1.3.dist-info/RECORD,,
+meetnotes_questions/meetnotes_questions.py,sha256=xGWAiCuuDcFibBKtCZInFWk96_9Gy185f4ZpRIJRdD8,5156
+meetnotes_questions-0.1.5.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+meetnotes_questions-0.1.5.dist-info/METADATA,sha256=VMEkmCyPNHLDE9U1NOLB14I2CDO0u0cGk85kZW7jJlg,397
+meetnotes_questions-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+meetnotes_questions-0.1.5.dist-info/entry_points.txt,sha256=guo3Be5mJa7c9qf5Lo-POBF0-6yofE3CJUFwGzBSG0A,70
+meetnotes_questions-0.1.5.dist-info/top_level.txt,sha256=23fGx0TLjLVsFol8ZjWXZcgm6UF_KDmQATQUMBbnPj4,20
+meetnotes_questions-0.1.5.dist-info/RECORD,,
```

