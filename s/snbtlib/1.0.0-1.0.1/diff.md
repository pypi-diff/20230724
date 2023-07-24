# Comparing `tmp/snbtlib-1.0.0.tar.gz` & `tmp/snbtlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snbtlib-1.0.0.tar", last modified: Fri Jun  2 05:48:00 2023, max compression
+gzip compressed data, was "snbtlib-1.0.1.tar", last modified: Mon Jul 24 06:44:37 2023, max compression
```

## Comparing `snbtlib-1.0.0.tar` & `snbtlib-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.443722 snbtlib-1.0.0/
--rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      716 2023-06-02 05:48:00.443722 snbtlib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 05:48:00.443722 snbtlib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-05-24 01:43:44.000000 snbtlib-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.439722 snbtlib-1.0.0/snbtlib/
--rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-1.0.0/snbtlib/__init__.py
--rw-rw-rw-   0        0        0     7009 2023-06-02 05:46:10.000000 snbtlib-1.0.0/snbtlib/formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.442721 snbtlib-1.0.0/snbtlib.egg-info/
--rw-rw-rw-   0        0        0      716 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.442721 snbtlib-1.0.0/test/
--rw-rw-rw-   0        0        0      224 2023-05-24 02:31:49.000000 snbtlib-1.0.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:37.164564 snbtlib-1.0.1/
+-rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      814 2023-07-24 06:44:37.164564 snbtlib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-06-02 05:53:43.000000 snbtlib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:44:37.165565 snbtlib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-07-24 06:44:35.000000 snbtlib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:37.161520 snbtlib-1.0.1/snbtlib/
+-rw-rw-rw-   0        0        0      302 2023-07-24 06:44:00.000000 snbtlib-1.0.1/snbtlib/__init__.py
+-rw-rw-rw-   0        0        0     7600 2023-07-24 06:44:07.000000 snbtlib-1.0.1/snbtlib/formatter.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:37.163574 snbtlib-1.0.1/snbtlib.egg-info/
+-rw-rw-rw-   0        0        0      814 2023-07-24 06:44:37.000000 snbtlib-1.0.1/snbtlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-07-24 06:44:37.000000 snbtlib-1.0.1/snbtlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:44:37.000000 snbtlib-1.0.1/snbtlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 06:44:37.000000 snbtlib-1.0.1/snbtlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:37.164564 snbtlib-1.0.1/test/
+-rw-rw-rw-   0        0        0      224 2023-05-24 02:31:49.000000 snbtlib-1.0.1/test/test.py
```

### Comparing `snbtlib-1.0.0/LICENSE` & `snbtlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snbtlib-1.0.0/PKG-INFO` & `snbtlib-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
@@ -24,10 +24,10 @@
 import snbtlib
 from pathlib import Path
 
 # Reading Text to JSON
 json = snbtlib.loads(Path('quest.snbt').read_text(encoding='utf-8'))
 
 # Dumping JSON to Text
-text = snbtlib.dumps(json)
+text = snbtlib.dumps(json, compact=False)  # When compact is True, the output will be compatible with Version 1.12 and below
 Path('quest.snbt').write_text(text, encoding='utf-8')
 ```
```

### Comparing `snbtlib-1.0.0/setup.py` & `snbtlib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='snbtlib',
-    version='1.0.0',
+    version='1.0.1',
     keywords='minecraft',
     description='a formatter for snbt from minecraft',
     long_description=long_description,
     license='MIT License',
     url='',
     author='Tryanks',
     author_email='tryanks@outlook.com',
```

### Comparing `snbtlib-1.0.0/snbtlib/formatter.py` & `snbtlib-1.0.1/snbtlib/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,18 @@
     def next(self):
         if self.index >= len(self.TokenList):
             return False
         token = self.TokenList[self.index]
         self.index += 1
         return token
 
+    def last(self):
+        self.index -= 1
+        return self.TokenList[self.index - 1]
+
 
 def loads(file, format=False):
     snbt_token = snbt_to_token_list(file)
     snbt_dict = None
     iterator = TokenIterator(snbt_token)
     while i := iterator.next():
         if i.type == Token.BEGIN_DICT:
@@ -132,14 +136,19 @@
         if value.startswith('$number$'):
             text += value[8:] + '\n'
         else:
             text += f'"{value}"\n'
     elif type(value) == bool:
         text += 'true' if value else 'false'
         text += '\n'
+    elif type(value) == bytes:
+        text += "[B;\n"
+        for i in value:
+            text += '\t' * (indent + 1) + str(int.from_bytes(i, 'big')) + 'b\n'
+        text += '\t' * indent + ']\n'
     return text
 
 
 def dict_iterator(token):
     tdict = {}
     key = ''
     while i := token.next():
@@ -159,14 +168,24 @@
         if i.type == Token.STRING_IN_QUOTE:
             key = f'"{key}"'
     return tdict
 
 
 def list_iterator(token):
     tlist = []
+    if token.next() == "B;":
+        tlist = b''
+        while i := token.next():
+            if i.type == Token.END_LIST:
+                break
+            value = i.value[:-1]
+            tlist += int(value).to_bytes(1, 'big')
+        return tlist
+    else:
+        token.last()
     while i := token.next():
         if i.type == Token.BEGIN_DICT:
             tlist.append(dict_iterator(token))
         elif i.type == Token.BEGIN_LIST:
             tlist.append(list_iterator(token))
         elif i.type in (Token.BOOL, Token.STRING, Token.NUMBER, Token.INTEGER, Token.STRING_IN_QUOTE):
             tlist.append(i.value)
@@ -207,15 +226,15 @@
     return token_list
 
 
 def NumberBuilder(r):
     s = StringIO()
     s.write(r.get_point())
     while i := r.next():
-        if i in '},\n:' or i.isspace():
+        if i in '}],\n:' or i.isspace():
             r.last()
             break
         s.write(i)
     return '$number$' + s.getvalue()
 
 
 def StringBuilder(r):
@@ -245,8 +264,8 @@
     if not text:
         return ''
     else:
         lines = text.splitlines()
         for i in range(len(lines)-1):
             if lines[i][-1] not in '[{' and lines[i+1].strip()[0] not in ']}':
                 lines[i] += ','
-        return '\n'.join(lines)
+        return '\n'.join(lines)
```

### Comparing `snbtlib-1.0.0/snbtlib.egg-info/PKG-INFO` & `snbtlib-1.0.1/snbtlib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
@@ -24,10 +24,10 @@
 import snbtlib
 from pathlib import Path
 
 # Reading Text to JSON
 json = snbtlib.loads(Path('quest.snbt').read_text(encoding='utf-8'))
 
 # Dumping JSON to Text
-text = snbtlib.dumps(json)
+text = snbtlib.dumps(json, compact=False)  # When compact is True, the output will be compatible with Version 1.12 and below
 Path('quest.snbt').write_text(text, encoding='utf-8')
 ```
```

