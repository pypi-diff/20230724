# Comparing `tmp/meetnotes_questions-0.1.6-py3-none-any.whl.zip` & `tmp/meetnotes_questions-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 4971 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       75 b- defN 23-Jul-24 18:38 meetnotes_questions/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jul-24 18:37 meetnotes_questions/__main__.py
--rw-r--r--  2.0 unx     5154 b- defN 23-Jul-24 21:29 meetnotes_questions/meetnotes_questions.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 21:30 meetnotes_questions-0.1.6.dist-info/RECORD
-9 files, 7823 bytes uncompressed, 3507 bytes compressed:  55.2%
+-rw-r--r--  2.0 unx     5153 b- defN 23-Jul-24 21:30 meetnotes_questions/meetnotes_questions.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jul-24 21:31 meetnotes_questions-0.1.7.dist-info/RECORD
+9 files, 7822 bytes uncompressed, 3507 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: meetnotes_questions/__main__.py
 Comment: 
 
 Filename: meetnotes_questions/meetnotes_questions.py
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/LICENSE.txt
+Filename: meetnotes_questions-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/METADATA
+Filename: meetnotes_questions-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/WHEEL
+Filename: meetnotes_questions-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/entry_points.txt
+Filename: meetnotes_questions-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/top_level.txt
+Filename: meetnotes_questions-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: meetnotes_questions-0.1.6.dist-info/RECORD
+Filename: meetnotes_questions-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meetnotes_questions/meetnotes_questions.py

```diff
@@ -152,13 +152,13 @@
     openai.api_key = openai_token
     notes_directory = "~/Downloads/"
     absolute_dir_path = os.path.expanduser(notes_directory)
     assert os.path.isdir(absolute_dir_path), f"Directory not found: {absolute_dir_path}"
     await begin_watching(absolute_dir_path)
 
 
- def main():
+def main():
     asyncio.run(real_main())
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `meetnotes_questions-0.1.6.dist-info/LICENSE.txt` & `meetnotes_questions-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

