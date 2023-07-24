# Comparing `tmp/meetnotes_questions-0.1.8-py3-none-any.whl.zip` & `tmp/meetnotes_questions-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5043 bytes, number of entries: 9
+Zip file size: 5056 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       75 b- defN 23-Jul-24 18:38 meetnotes_questions/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jul-24 18:37 meetnotes_questions/__main__.py
--rw-r--r--  2.0 unx     5335 b- defN 23-Jul-24 21:34 meetnotes_questions/meetnotes_questions.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 21:35 meetnotes_questions-0.1.8.dist-info/RECORD
-9 files, 8004 bytes uncompressed, 3579 bytes compressed:  55.3%
+-rw-r--r--  2.0 unx     5351 b- defN 23-Jul-24 21:37 meetnotes_questions/meetnotes_questions.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 21:37 meetnotes_questions-0.1.9.dist-info/RECORD
+9 files, 8020 bytes uncompressed, 3592 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: meetnotes_questions/__main__.py
 Comment: 
 
 Filename: meetnotes_questions/meetnotes_questions.py
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/LICENSE.txt
+Filename: meetnotes_questions-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/METADATA
+Filename: meetnotes_questions-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/WHEEL
+Filename: meetnotes_questions-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/entry_points.txt
+Filename: meetnotes_questions-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/top_level.txt
+Filename: meetnotes_questions-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.8.dist-info/RECORD
+Filename: meetnotes_questions-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meetnotes_questions/meetnotes_questions.py

```diff
@@ -39,25 +39,27 @@
 
     def on_modified(self, event):
         if self._check_file(event.src_path):
             print("File modified event triggered.")
             self.queue.put(("modified", event))
             print("File modified event processed.")
 
+    """
     def on_created(self, event):
         if self._check_file(event.src_path):
             print("File created event triggered.")
             self.queue.put(("created", event))
             print("File created event processed.")
 
     def on_deleted(self, event):
         if self._check_file(event.src_path):
             print("File deleted event triggered.")
             self.queue.put(("deleted", event))
             print("File deleted event processed.")
+    """
 
     def _check_file(self, file_path):
         filename = os.path.basename(file_path)
         return fnmatch.fnmatch(filename, "2023*.txt")
 
 
 def process_file(file_path):
```

## Comparing `meetnotes_questions-0.1.8.dist-info/LICENSE.txt` & `meetnotes_questions-0.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

