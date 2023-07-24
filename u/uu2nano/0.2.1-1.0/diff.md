# Comparing `tmp/uu2nano-0.2.1-py3-none-any.whl.zip` & `tmp/uu2nano-1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2674 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1067 b- defN 23-Jul-23 16:33 uu2nano.py
--rw-r--r--  2.0 unx     2084 b- defN 23-Jul-23 16:34 uu2nano-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 16:34 uu2nano-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 16:34 uu2nano-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      364 b- defN 23-Jul-23 16:34 uu2nano-0.2.1.dist-info/RECORD
-5 files, 3615 bytes uncompressed, 1996 bytes compressed:  44.8%
+Zip file size: 2670 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jul-24 12:09 uu2nano.py
+-rw-r--r--  2.0 unx     2091 b- defN 23-Jul-24 12:10 uu2nano-1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 12:10 uu2nano-1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-24 12:10 uu2nano-1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      356 b- defN 23-Jul-24 12:10 uu2nano-1.0.dist-info/RECORD
+5 files, 3586 bytes uncompressed, 2008 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: uu2nano.py
 Comment: 
 
-Filename: uu2nano-0.2.1.dist-info/METADATA
+Filename: uu2nano-1.0.dist-info/METADATA
 Comment: 
 
-Filename: uu2nano-0.2.1.dist-info/WHEEL
+Filename: uu2nano-1.0.dist-info/WHEEL
 Comment: 
 
-Filename: uu2nano-0.2.1.dist-info/top_level.txt
+Filename: uu2nano-1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: uu2nano-0.2.1.dist-info/RECORD
+Filename: uu2nano-1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uu2nano.py

```diff
@@ -1,40 +1,40 @@
 import uuid
 
 
-__version__ = '0.2.1'
+__version__ = '1.0'
 
 
 def _make_alpharev(alphabet):
     alpharev = bytearray(max(c for c in alphabet) + 1)
     for i, c in enumerate(alphabet):
         alpharev[c] = i
     return bytes(alpharev)
 
 
-alphabet = b'_-0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
-alpharev = _make_alpharev(alphabet)
-_low_mask = 2 ** 62 - 1
-_const_bits = 0b10 << 62
+ALPHABET = b'_-0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
+ALPHAREV = _make_alpharev(ALPHABET)
+_LOW_MASK = 2 ** 62 - 1
+_CONST_BITS = 0b10 << 62
 
 
-def uuid_to_nanoid(uu: uuid.UUID, *, alphabet=alphabet) -> str:
+def uuid_to_nanoid(uu: uuid.UUID, *, alphabet=ALPHABET) -> str:
     uu = uu.int
-    assert uu >> 62 & 0b11 == 2, "Wrong mark bits. Use fix_uuid() for true random input"
-    uu = (uu >> 64 << 62) | (uu & _low_mask)
+    assert uu >> 62 & 0b11 == 2, "Not RFC 4122 compliant UUID"
+    uu = (uu >> 64 << 62) | (uu & _LOW_MASK)
     b = bytearray(21)
     for i in range(21):
         b[20 - i] = alphabet[uu >> (6 * i) & 0b111111]
     return b.decode()
 
 
-def nanoid_to_uuid(nano: str, *, alpharev=alpharev) -> uuid.UUID:
+def nanoid_to_uuid(nano: str, *, alpharev=ALPHAREV) -> uuid.UUID:
     uu = 0
     for c in nano.encode():
         uu = (uu << 6) | alpharev[c]
-    uu = (uu >> 62 << 64) | (uu & _low_mask) | _const_bits
+    uu = (uu >> 62 << 64) | (uu & _LOW_MASK) | _CONST_BITS
     return uuid.UUID(int=uu)
 
 
 def fix_uuid(uu: uuid.UUID) -> uuid.UUID:
-    uu = uu.int & ~(0b11 << 62) | _const_bits
+    uu = uu.int & ~(0b11 << 62) | _CONST_BITS
     return uuid.UUID(int=uu)
```

## Comparing `uu2nano-0.2.1.dist-info/METADATA` & `uu2nano-1.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uu2nano
-Version: 0.2.1
+Version: 1.0
 Summary: Conversion tool from UUID to nanoid and vice versa
 Author-email: Aleksandr Karpinskii <homm86@gmail.com>
 Project-URL: Repository, https://github.com/homm/uu2nano
 Keywords: uuid,nanoid
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -43,15 +43,15 @@
 from uu2nano import fix_uuid, nanoid_to_uuid, uuid_to_nanoid
 
 uu = uuid.uuid4()
 nano = uuid_to_nanoid(uu)
 assert uu == nanoid_to_uuid(nano)
 ```
 
-If you receive UUIDs from an untrusted place, there is a chance that eventually
+If you receive not compliant UUIDs from third parties, there is a chance that eventually
 two reserved fixed bits could be wrong. In this case `uuid_to_nanoid` will fail:
 
 ```python
 
 @app.post
 def find_book(uu: uuid.UUID):
     nano = uuid_to_nanoid(uu)
```

