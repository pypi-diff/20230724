# Comparing `tmp/meetnotes_questions-0.1.2-py3-none-any.whl.zip` & `tmp/meetnotes_questions-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4693 bytes, number of entries: 9
+Zip file size: 4714 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       75 b- defN 23-Jul-24 18:38 meetnotes_questions/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jul-24 18:37 meetnotes_questions/__main__.py
--rw-r--r--  2.0 unx     4266 b- defN 23-Jul-24 20:40 meetnotes_questions/meetnotes_questions.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 20:40 meetnotes_questions-0.1.2.dist-info/RECORD
-9 files, 6935 bytes uncompressed, 3229 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx     4301 b- defN 23-Jul-24 20:43 meetnotes_questions/meetnotes_questions.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 20:44 meetnotes_questions-0.1.3.dist-info/RECORD
+9 files, 6970 bytes uncompressed, 3250 bytes compressed:  53.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: meetnotes_questions/__main__.py
 Comment: 
 
 Filename: meetnotes_questions/meetnotes_questions.py
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/LICENSE.txt
+Filename: meetnotes_questions-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/METADATA
+Filename: meetnotes_questions-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/WHEEL
+Filename: meetnotes_questions-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/entry_points.txt
+Filename: meetnotes_questions-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/top_level.txt
+Filename: meetnotes_questions-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.2.dist-info/RECORD
+Filename: meetnotes_questions-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meetnotes_questions/meetnotes_questions.py

```diff
@@ -14,14 +14,16 @@
 from watchdog.observers import Observer
 
 load_dotenv()  # take environment variables from .env.
 
 MODEL = "gpt-3.5-turbo"
 # MODEL = "gpt-4"
 
+MAX_TOKENS = 1000
+
 enc = tiktoken.encoding_for_model(MODEL)
 
 
 # Assume get_question is an asynchronous function that gets the question.
 def get_question(processed_content):
     # Code to get the question goes here...
     response = openai.ChatCompletion.create(
@@ -55,20 +57,20 @@
 def process_file(file_path):
     print(f"File: {file_path}", file=sys.stderr)
     file_content = open(file_path, "rt").read()
     messages = parse_conversation(file_content)
     print("Messages:", messages)
     system_message = {
         "role": "system",
-        "content": 'You are a junior staff member at a company, and trying to learn more about the business and domain. You are transcribing notes between yourself, your colleagues, and clients/prospects. "Me" means messages by me. Propose intelligent questions to ask in the meeting.',
+        "content": 'You are a junior staff member at a company, and trying to learn more about the business and domain. You are transcribing notes between yourself, your colleagues, and clients/prospects. "Me" means messages by me. Propose one or two intelligent question to ask in the meeting.',
     }
     kept_messages = []
     for message in reversed(messages):
         total_text = json.dumps([system_message] + [message] + kept_messages)
-        if len(enc.encode(total_text)) > 4000:
+        if len(enc.encode(total_text)) > MAX_TOKENS:
             break
         kept_messages = [message] + kept_messages
     return [system_message] + kept_messages
 
 
 def process_event(event_type, event):
     print(f"Event type: {event_type}")
```

## Comparing `meetnotes_questions-0.1.2.dist-info/LICENSE.txt` & `meetnotes_questions-0.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `meetnotes_questions-0.1.2.dist-info/RECORD` & `meetnotes_questions-0.1.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 meetnotes_questions/__init__.py,sha256=ozuBNNUzpClNmd99Mrf9nyDde19z_pHY9pN-_20H_Os,75
 meetnotes_questions/__main__.py,sha256=CX1YQrso4UHQcl9jdGvRc7sixnz8LRo0S6ON9sIyIEo,106
-meetnotes_questions/meetnotes_questions.py,sha256=3r-WjKOQrdq8iKNpDymEkIyKJTe_ppdXZOALshfhKoM,4266
-meetnotes_questions-0.1.2.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-meetnotes_questions-0.1.2.dist-info/METADATA,sha256=daVbQcixpfw8ZV5HdHUWEkzPnO5dMPRBYqPjdQ9_f_s,397
-meetnotes_questions-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-meetnotes_questions-0.1.2.dist-info/entry_points.txt,sha256=guo3Be5mJa7c9qf5Lo-POBF0-6yofE3CJUFwGzBSG0A,70
-meetnotes_questions-0.1.2.dist-info/top_level.txt,sha256=23fGx0TLjLVsFol8ZjWXZcgm6UF_KDmQATQUMBbnPj4,20
-meetnotes_questions-0.1.2.dist-info/RECORD,,
+meetnotes_questions/meetnotes_questions.py,sha256=OR38QvHyGLtfnl0KXFIU3B4F3-yLS4MlJCkPXToXJkc,4301
+meetnotes_questions-0.1.3.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+meetnotes_questions-0.1.3.dist-info/METADATA,sha256=5DpNyjOiX_utDcLrD30twHOcQ45HHjbDz6DBISdMElY,397
+meetnotes_questions-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+meetnotes_questions-0.1.3.dist-info/entry_points.txt,sha256=guo3Be5mJa7c9qf5Lo-POBF0-6yofE3CJUFwGzBSG0A,70
+meetnotes_questions-0.1.3.dist-info/top_level.txt,sha256=23fGx0TLjLVsFol8ZjWXZcgm6UF_KDmQATQUMBbnPj4,20
+meetnotes_questions-0.1.3.dist-info/RECORD,,
```

