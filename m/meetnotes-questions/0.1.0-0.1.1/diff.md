# Comparing `tmp/meetnotes_questions-0.1.0-py3-none-any.whl.zip` & `tmp/meetnotes_questions-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4673 bytes, number of entries: 9
+Zip file size: 4689 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       75 b- defN 23-Jul-24 18:38 meetnotes_questions/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jul-24 18:37 meetnotes_questions/__main__.py
--rw-r--r--  2.0 unx     4227 b- defN 23-Jul-24 20:15 meetnotes_questions/meetnotes_questions.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 20:22 meetnotes_questions-0.1.0.dist-info/RECORD
-9 files, 6897 bytes uncompressed, 3209 bytes compressed:  53.5%
+-rw-r--r--  2.0 unx     4266 b- defN 23-Jul-24 20:38 meetnotes_questions/meetnotes_questions.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 20:38 meetnotes_questions-0.1.1.dist-info/RECORD
+9 files, 6935 bytes uncompressed, 3225 bytes compressed:  53.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: meetnotes_questions/__main__.py
 Comment: 
 
 Filename: meetnotes_questions/meetnotes_questions.py
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/LICENSE.txt
+Filename: meetnotes_questions-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/METADATA
+Filename: meetnotes_questions-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/WHEEL
+Filename: meetnotes_questions-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/entry_points.txt
+Filename: meetnotes_questions-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/top_level.txt
+Filename: meetnotes_questions-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.0.dist-info/RECORD
+Filename: meetnotes_questions-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meetnotes_questions/meetnotes_questions.py

```diff
@@ -11,22 +11,25 @@
 import tiktoken
 from dotenv import load_dotenv
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
 load_dotenv()  # take environment variables from .env.
 
-enc = tiktoken.get_encoding("cl100k_base")
+MODEL = "gpt-3.5-turbo"
+# MODEL = "gpt-4"
+
+enc = tiktoken.get_encoding_model(MODEL)
 
 
 # Assume get_question is an asynchronous function that gets the question.
 def get_question(processed_content):
     # Code to get the question goes here...
     response = openai.ChatCompletion.create(
-        model="gpt-4",
+        model=MODEL,
         messages=processed_content,
     )
     return response.choices[0].message["content"]
 
 
 class FileWatcher(FileSystemEventHandler):
     def __init__(self, event_queue):
```

## Comparing `meetnotes_questions-0.1.0.dist-info/LICENSE.txt` & `meetnotes_questions-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

