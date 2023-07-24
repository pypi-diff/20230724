# Comparing `tmp/pgvector-0.1.8-py2.py3-none-any.whl.zip` & `tmp/pgvector-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7559 bytes, number of entries: 11
+Zip file size: 7669 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      272 b- defN 21-Jun-23 06:42 pgvector/asyncpg/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 23-May-13 19:32 pgvector/django/__init__.py
+-rw-r--r--  2.0 unx     2624 b- defN 23-Jul-23 16:11 pgvector/django/__init__.py
 -rw-r--r--  2.0 unx     1743 b- defN 23-May-10 04:14 pgvector/psycopg/__init__.py
 -rw-r--r--  2.0 unx      881 b- defN 21-Jun-13 19:29 pgvector/psycopg2/__init__.py
 -rw-r--r--  2.0 unx     1033 b- defN 22-May-23 01:12 pgvector/sqlalchemy/__init__.py
 -rw-r--r--  2.0 unx     1305 b- defN 21-Jun-23 02:28 pgvector/utils/__init__.py
--rw-r--r--  2.0 unx     1083 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6462 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/RECORD
-11 files, 16236 bytes uncompressed, 6027 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     1083 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6666 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/RECORD
+11 files, 16630 bytes uncompressed, 6137 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pgvector/sqlalchemy/__init__.py
 Comment: 
 
 Filename: pgvector/utils/__init__.py
 Comment: 
 
-Filename: pgvector-0.1.8.dist-info/LICENSE.txt
+Filename: pgvector-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pgvector-0.1.8.dist-info/METADATA
+Filename: pgvector-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pgvector-0.1.8.dist-info/WHEEL
+Filename: pgvector-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pgvector-0.1.8.dist-info/top_level.txt
+Filename: pgvector-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pgvector-0.1.8.dist-info/RECORD
+Filename: pgvector-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pgvector/django/__init__.py

```diff
@@ -38,14 +38,20 @@
 
     def get_prep_value(self, value):
         return to_db(value)
 
     def value_to_string(self, obj):
         return self.get_prep_value(self.value_from_object(obj))
 
+    def validate(self, value, model_instance):
+        super().validate(value.tolist(), model_instance)
+
+    def run_validators(self, value):
+        super().run_validators(value.tolist())
+
 
 class IvfflatIndex(PostgresIndex):
     suffix = 'ivfflat'
 
     def __init__(self, *expressions, lists=None, **kwargs):
         self.lists = lists
         super().__init__(*expressions, **kwargs)
```

## Comparing `pgvector-0.1.8.dist-info/LICENSE.txt` & `pgvector-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pgvector-0.1.8.dist-info/METADATA` & `pgvector-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pgvector
-Version: 0.1.8
+Version: 0.2.0
 Summary: pgvector support for Python
 Home-page: https://github.com/pgvector/pgvector-python
 Author: Andrew Kane
 Author-email: andrew@ankane.org
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 
 # pgvector-python
 
 [pgvector](https://github.com/pgvector/pgvector) support for Python
@@ -36,14 +36,15 @@
 - [Psycopg 2](#psycopg-2)
 - [asyncpg](#asyncpg)
 
 Or check out some examples:
 
 - [Embeddings](examples/openai_embeddings.py) with OpenAI
 - [Sentence embeddings](examples/sentence_embeddings.py) with SentenceTransformers
+- [Hybrid search](examples/hybrid_search.py) with SentenceTransformers
 - [Image search](examples/pytorch_image_search.py) with PyTorch
 - [Implicit feedback recommendations](examples/implicit_recs.py) with Implicit
 - [Explicit feedback recommendations](examples/surprise_recs.py) with Surprise
 - [Recommendations](examples/lightfm_recs.py) with LightFM
 
 ## Django
 
@@ -256,14 +257,23 @@
 
 ```python
 from pgvector.asyncpg import register_vector
 
 await register_vector(conn)
 ```
 
+or your pool
+
+```python
+async def init(conn):
+    await register_vector(conn)
+
+pool = await asyncpg.create_pool(..., init=init)
+```
+
 Insert a vector
 
 ```python
 embedding = np.array([1, 2, 3])
 await conn.execute('INSERT INTO item (embedding) VALUES ($1)', embedding)
 ```
```

## Comparing `pgvector-0.1.8.dist-info/RECORD` & `pgvector-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pgvector/asyncpg/__init__.py,sha256=VffBZUNIwvinQdh0lIYoSWgSQq57nFkpj9VhPjp11QQ,272
-pgvector/django/__init__.py,sha256=8OX-LD3QpZD4a7a4vKVNSRXw9mbQlhHDTHQFhPpDe1M,2434
+pgvector/django/__init__.py,sha256=Gm_rZr0WVv6HfZUzar9QndJqElKhQjzGycffRrRWvlo,2624
 pgvector/psycopg/__init__.py,sha256=BjyTM_VGtl3RB-Fh4gPBppr8LutuH7hR3l0C7MJYMyw,1743
 pgvector/psycopg2/__init__.py,sha256=w_uHyKJzHMI79IyKYwFv6CK_k1RI1X6sWiML55Wo4b4,881
 pgvector/sqlalchemy/__init__.py,sha256=LUEkR6UIxW_o6fmjRKQmasMm6ZkyylnkW7VDMWyi-EI,1033
 pgvector/utils/__init__.py,sha256=udvrI2Gl5cjO-eXYkb5opTDUFs0indJIPQJ9qgpH-j4,1305
-pgvector-0.1.8.dist-info/LICENSE.txt,sha256=3Nr5vwERQHKYiiQHzy_AO2HurO6I3TonpJlYOmwbmcI,1083
-pgvector-0.1.8.dist-info/METADATA,sha256=CWy0YjvD3twmA6Kp90wY8Nykvf9bjf7cWQE948E3jbs,6462
-pgvector-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pgvector-0.1.8.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
-pgvector-0.1.8.dist-info/RECORD,,
+pgvector-0.2.0.dist-info/LICENSE.txt,sha256=3Nr5vwERQHKYiiQHzy_AO2HurO6I3TonpJlYOmwbmcI,1083
+pgvector-0.2.0.dist-info/METADATA,sha256=HGNl3-iv2BPJkqniB0tQCY2V9H0-7uDSZ9oMhFruiNQ,6666
+pgvector-0.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pgvector-0.2.0.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
+pgvector-0.2.0.dist-info/RECORD,,
```

