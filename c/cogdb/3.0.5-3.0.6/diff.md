# Comparing `tmp/cogdb-3.0.5.tar.gz` & `tmp/cogdb-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogdb-3.0.5.tar", last modified: Mon Mar 13 02:18:13 2023, max compression
+gzip compressed data, was "cogdb-3.0.6.tar", last modified: Mon Jul 24 02:52:08 2023, max compression
```

## Comparing `cogdb-3.0.5.tar` & `cogdb-3.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 02:18:13.291639 cogdb-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 02:18:05.000000 cogdb-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-13 02:18:13.291639 cogdb-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-03-13 02:18:05.000000 cogdb-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 02:18:13.287639 cogdb-3.0.5/cog/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-13 02:18:05.000000 cogdb-3.0.5/cog/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 02:18:13.287639 cogdb-3.0.5/cogdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-13 02:18:13.000000 cogdb-3.0.5/cogdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 02:18:13.291639 cogdb-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-13 02:18:05.000000 cogdb-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 02:18:13.291639 cogdb-3.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_db_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-13 02:18:05.000000 cogdb-3.0.5/test/test_torque6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 02:51:58.000000 cogdb-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 02:52:08.153014 cogdb-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-24 02:51:58.000000 cogdb-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.149014 cogdb-3.0.6/cog/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20251 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/cogdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:52:08.153014 cogdb-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 02:51:58.000000 cogdb-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_db_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque6.py
```

### Comparing `cogdb-3.0.5/LICENSE` & `cogdb-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/README.md` & `cogdb-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/cog/cache.py` & `cogdb-3.0.6/cog/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,14 @@
         key = int(key)
         if key in self.cache:
             return self.cache[key]
         else:
             return None
 
     def partial_update_from_zero_index(self, key, partial_value):
-        # print("cache: "+ str(self.cache))
-        # print("parital update: " + str(key) + " -> " + str(partial_value))
         end_pos = len(partial_value)
         if key not in self.cache:
             return
 
         value_byte_array = bytearray(self.cache[key])
         value_byte_array[0: end_pos] = partial_value
         self.cache[key] = bytes(value_byte_array)
```

### Comparing `cogdb-3.0.5/cog/config.py` & `cogdb-3.0.6/cog/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 COG_DEFAULT_NAMESPACE = "default"
 VIEWS = 'views'
 STORE="-store-"
 INDEX="-index-"
 INDEX_BLOCK_LEN = 32
 INDEX_CAPACITY = 100003 # must be a prime number
 STORE_READ_BUFFER_SIZE = 512
+LEVEL_2_CACHE_SIZE = 100000
 
 ''' TORQUE '''
 GRAPH_NODE_SET_TABLE_NAME = 'TOR_NODE_SET'
 GRAPH_EDGE_SET_TABLE_NAME = 'TOR_EDGE_SET'
 EMBEDDING_SET_TABLE_NAME = 'EMBEDDING_SET'
 
 ''' CUSTOM COG DB PATH '''
```

### Comparing `cogdb-3.0.5/cog/core.py` & `cogdb-3.0.6/cog/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os.path
 import sys
 import logging
 # from profilehooks import profile
 from cog.cache import Cache
 import xxhash
 
-
 RECORD_SEP = b'\xFD'
 UNIT_SEP = b'\xAC'
 
 
 class TableMeta:
 
     def __init__(self, name, namespace, db_instance_id, column_mode):
@@ -37,37 +36,43 @@
 
     def __create_store(self, shared_cache):
         return Store(self.table_meta, self.config, self.logger, shared_cache=shared_cache)
 
     def close(self):
         self.indexer.close()
         self.store.close()
-        self.logger.info("closed table: "+self.table_meta.name)
+        self.logger.info("closed table: " + self.table_meta.name)
 
 
 class Record:
-
+    '''
+    Record is the basic unit of storage in cog.
+    value_type: s - string, l - list, u - set
+    '''
     RECORD_LINK_LEN = 16
     RECORD_LINK_NULL = -1
     VALUE_LINK_NULL = -1
 
-    def __init__(self, key, value, tombstone='0', store_position=None, value_type="s",  key_link=-1, value_link=-1):
+    def __init__(self, key, value, tombstone='0', store_position=None, value_type="s", key_link=-1, value_link=-1):
         self.key = key
         self.value = value
         self.tombstone = tombstone
         self.store_position = store_position
         self.key_link = key_link
         self.value_link = value_link
         self.value_type = value_type
 
     def set_store_position(self, pos):
         if type(pos) is not int:
-            raise ValueError("store position must be int but provided : "+str(pos))
+            raise ValueError("store position must be int but provided : " + str(pos))
         self.store_position = pos
 
+    def set_key_link(self, pos):
+        self.key_link = pos
+
     def set_value_link(self, pos):
         self.value_link = pos
 
     def set_value(self, value):
         self.value = value
 
     def is_equal_val(self, other_record):
@@ -79,79 +84,86 @@
     def serialize(self):
         return marshal.dumps((self.key, self.value))
 
     def marshal(self):
         key_link_bytes = str(self.key_link).encode().rjust(Record.RECORD_LINK_LEN)
         serialized = self.serialize()
         m_record = key_link_bytes \
-                + self.tombstone.encode() \
-                + self.value_type.encode() \
-                + str(len(serialized)).encode() \
-                + UNIT_SEP \
-                + serialized
-        if self.value_type == "l":
+                   + self.tombstone.encode() \
+                   + self.value_type.encode() \
+                   + str(len(serialized)).encode() \
+                   + UNIT_SEP \
+                   + serialized
+        if self.value_type == "l" or self.value_type == "u":
             if self.value_link is not None:
                 m_record += str(self.value_link).encode()
         m_record += RECORD_SEP
         return m_record
 
     def is_empty(self):
         return self.key is None and self.value is None
 
     def __str__(self):
-        return "key: {}, value: {}, tombstone: {}, store_position: {}, key_link: {}, value_link: {}, value_type: {}".format(self.key, self.value, self.tombstone, self.store_position, self.key_link, self.value_link, self.value_type)
-
+        return "key: {}, value: {}, tombstone: {}, store_position: {}, key_link: {}, value_link: {}, value_type: {}".format(
+            self.key, self.value, self.tombstone, self.store_position, self.key_link, self.value_link, self.value_type)
 
     @classmethod
     def __read_until(cls, start, sbytes, separtor=UNIT_SEP):
         buff = b''
-        i  = 0 # default
+        i = 0  # default
         for i in range(start, len(sbytes)):
             s_byte = sbytes[i: i + 1]
             if s_byte == separtor:
                 break
             buff += s_byte
         return buff, i
 
     @classmethod
     def unmarshal(cls, store_bytes):
         """reads from bytes and creates object
         """
         base_pos = 0
-        key_link = int(store_bytes[base_pos: base_pos+Record.RECORD_LINK_LEN])
+        key_link = int(store_bytes[base_pos: base_pos + Record.RECORD_LINK_LEN])
         next_base_pos = Record.RECORD_LINK_LEN
         tombstone = store_bytes[next_base_pos:next_base_pos + 1].decode()
         value_type = store_bytes[next_base_pos + 1: next_base_pos + 2].decode()
         value_len, end_pos = cls.__read_until(next_base_pos + 2, store_bytes)
         value_len = int(value_len.decode())
-        value = store_bytes[end_pos+1: end_pos+1 + value_len]
+        value = store_bytes[end_pos + 1: end_pos + 1 + value_len]
         record = marshal.loads(value)
 
         value_link = Record.VALUE_LINK_NULL
-        if value_type == 'l':
-            value_link, end_pos = cls.__read_until(end_pos + value_len + 1,  store_bytes, RECORD_SEP)
+        if value_type == 'l' or value_type == 'u':
+            value_link, end_pos = cls.__read_until(end_pos + value_len + 1, store_bytes, RECORD_SEP)
             value_link = int(value_link.decode())
-        return cls(record[0], record[1], tombstone, store_position=None, value_type=value_type,  key_link=key_link, value_link=value_link)
-
+        return cls(record[0], record[1], tombstone, store_position=None, value_type=value_type, key_link=key_link,
+                   value_link=value_link)
 
     @classmethod
     def __load_value(cls, store_pointer, val_list, store):
         """loads value from the store"""
         while store_pointer != Record.VALUE_LINK_NULL:
             rec = Record.unmarshal(store.read(store_pointer))
-            val_list.append(rec.value)
+            if rec.value_type == 'l':
+                val_list.append(rec.value)
+            else:
+                val_list.add(rec.value)
             store_pointer = rec.value_link
         return val_list
 
     @classmethod
     # @profile
     def load_from_store(cls, position: int, store):
         record = cls.unmarshal(store.read(position))
+        values = None
         if record.value_type == 'l':
             values = cls.__load_value(record.value_link, [record.value], store)
+        elif record.value_type == 'u':
+            values = cls.__load_value(record.value_link, {record.value}, store)
+        if values is not None:
             record.set_value(values)
         return record
 
 
 class Index:
 
     def __init__(self, table_meta, config, logger, index_id=0):
@@ -180,15 +192,14 @@
 
         self.db_mem.seek(0)
         current_block = self.db_mem.read(self.config.INDEX_BLOCK_LEN)
 
     def close(self):
         self.db.close()
 
-
     def get_index_key(self, int_store_position):
         return str(int_store_position).encode().rjust(self.config.INDEX_BLOCK_LEN)
 
     # @profile
     def put(self, key, store_position, store):
         """
         key chain
@@ -201,50 +212,61 @@
         """
         k5 -> k4 -> k3 -> k2 -> k1
         add: k6
         k6 -> k5 -> k4 -> k3 -> k2 -> k1
         add/update: k4
         1. k4 -> k6 -> k5 -> k4 -> k3 -> k2 -> k1
         2. k4 -> k6 -> k5 -> k3 -> k2 -> k1
-        
+
         """
         orig_position, orig_hash = self.get_index(key)
-        data_at_prob_position = self.db_mem[orig_position: orig_position + self.config.INDEX_BLOCK_LEN]
-        self.logger.debug('writing : '+str(key) + ' current data at store position: '+ str(data_at_prob_position))
-        if data_at_prob_position == self.empty_block:
-            # point next link to record null
+        index_value = self.db_mem[orig_position: orig_position + self.config.INDEX_BLOCK_LEN]
+        self.logger.debug('writing : ' + str(key) + ' current data at store position: ' + str(index_value))
+        if index_value == self.empty_block:
+            # First record in the key bucket, point next link to null
             store.update_record_link_inplace(store_position, Record.RECORD_LINK_NULL)
+            key_link = store_position
+            # write the store position to the index
             self.db_mem[orig_position: orig_position + self.config.INDEX_BLOCK_LEN] = self.get_index_key(store_position)
         else:
-            # read existing record and update pointers
-            record = Record.load_from_store(int(data_at_prob_position), store)
-            record.set_store_position(int(data_at_prob_position))
-            if record.key == key:
-                """ update existing record """
-                store.update_record_link_inplace(store_position, int(record.key_link))
+            # there are records in the bucket
+            # read existing record from the store
+            existing_record = Record.load_from_store(int(index_value), store)
+            existing_record.set_store_position(int(index_value))  # this is a bit confusing, should clean up.
+
+            if existing_record.key == key:
+                # the record at the top of the bucket has the same key, update the record in place.
+                # a new entry has been made to the store, update pre and next links.
+                store.update_record_link_inplace(store_position, int(existing_record.key_link))
+                key_link = int(existing_record.key_link)
             else:
-                # set next link to the record at the top of the bucket
-                store.update_record_link_inplace(store_position, record.store_position)
+                # this is hash collision.
+                # the record at the top of the bucket has a different key, add new record to the top of the bucket.
+                # set next link to the record at the top of the bucket, prev is null by default, no need to set.
+                store.update_record_link_inplace(store_position, existing_record.store_position)
+                key_link = existing_record.store_position
+
                 # check if this record exists in the bucket, if yes remove pointer.
                 prev_record = None
-                while record.key_link != Record.RECORD_LINK_NULL:
-                    record = Record.load_from_store(record.key_link, store)
-                    record.set_store_position(record.key_link)
-                    if record.key == key and prev_record is not None:
+                while existing_record.key_link != Record.RECORD_LINK_NULL:
+                    existing_record = Record.load_from_store(existing_record.key_link, store)
+                    existing_record.set_store_position(existing_record.key_link)
+                    if existing_record.key == key and prev_record is not None:
                         """
                         if same key found in bucket, update previous record in chain to point to key_link of this record
                         prev_rec -> current rec.key_link
                         curr_rec will not be linked in the bucket anymore.
                         """
-                        #update in place the key link pointer of pervios record, ! need to add fixed length padding.
-                        store.update_record_link_inplace(prev_record.store_position, record.key_link)
-                    prev_record = record
-
-            self.db_mem[orig_position: orig_position + self.config.INDEX_BLOCK_LEN] = self.get_index_key(store_position)
+                        # update in place the key link pointer of pervios record, ! need to add fixed length padding.
+                        store.update_record_link_inplace(prev_record.store_position, existing_record.key_link)
+                        key_link = existing_record.key_link
+                    prev_record = existing_record
 
+        self.db_mem[orig_position: orig_position + self.config.INDEX_BLOCK_LEN] = self.get_index_key(store_position)
+        return key_link
 
     def get_index(self, key):
         num = cog_hash(key, self.config.INDEX_CAPACITY) % ((sys.maxsize + 1) * 2)
         self.logger.debug("hash for: " + key + " : " + str(num))
         # there may be diff when using mem slice vs write (+1 needed)
         index = (self.config.INDEX_BLOCK_LEN *
                  (max((num % self.config.INDEX_CAPACITY) - 1, 0)))
@@ -266,37 +288,38 @@
         record.set_store_position(data_at_index_position)
         self.logger.debug("read record " + str(record))
 
         if record.key == key:
             return record
         else:
             while record.key_link != Record.RECORD_LINK_NULL:
-                self.logger.debug("record.key_link: "+str(record.key_link))
+                self.logger.debug("record.key_link: " + str(record.key_link))
                 record = Record.load_from_store(record.key_link, store)
                 record.set_store_position(record.key_link)
                 if record.key == key:
                     return record
         return None
 
     '''
         Iterates through record in itr_store.
     '''
-    def scanner(self,store):
+
+    def scanner(self, store):
         scan_cursor = 0
         while True:
             data_at_position = self.db_mem[scan_cursor:scan_cursor + self.config.INDEX_BLOCK_LEN]
-            if len(data_at_position) == 0:#EOF index
+            if len(data_at_position) == 0:  # EOF index
                 self.logger.info("Index EOF reached! Scan terminated.")
                 return
             if data_at_position == self.empty_block:
                 scan_cursor += self.config.INDEX_BLOCK_LEN
                 self.logger.debug("GET: skipping empty block during iteration.")
                 continue
             record = Record.load_from_store(int(data_at_position), store)
-            if record is None:#EOF store
+            if record is None:  # EOF store
                 self.logger.error("Store EOF reached! Iteration terminated.")
                 return
             yield Record(record.key, record.value, record.tombstone)
             scan_cursor += self.config.INDEX_BLOCK_LEN
 
     def delete(self, key, store):
         """
@@ -332,15 +355,14 @@
                     curr_rec will not be linked in the bucket anymore.
                     """
                     # update in place the key link pointer of pervios record, ! need to add fixed length padding.
                     store.update_record_link_inplace(prev_record.store_position, record.key_link)
                 prev_record = record
         return True
 
-
     def flush(self):
         self.db_mem.flush()
 
 
 class Store:
 
     def __init__(self, tablemeta, config, logger, caching_enabled=True, shared_cache=None):
@@ -373,123 +395,123 @@
         if self.caching_enabled:
             self.store_cache.put(store_position, marshalled_record)
         return store_position
 
     def update_record_link_inplace(self, start_pos, int_value):
         """updates record link in store file in place"""
         if type(int_value) is not int:
-            raise ValueError("store position must be int but provided : "+str(start_pos))
+            raise ValueError("store position must be int but provided : " + str(start_pos))
 
         byte_value = str(int_value).encode().rjust(Record.RECORD_LINK_LEN)
         self.logger.debug('update_record_link_inplace: ' + str(byte_value))
         self.store_file.seek(start_pos)
         self.store_file.write(byte_value)
 
         if self.caching_enabled:
             self.store_cache.partial_update_from_zero_index(start_pos, byte_value)
         self.store_file.flush()
 
     # @profile
     def read(self, position):
-        self.logger.debug("store read request at position: "+str(position))
+        self.logger.debug("store read request at position: " + str(position))
         if self.caching_enabled:
             cached_record = self.store_cache.get(position)
             if cached_record is not None:
                 return cached_record
 
         self.store_file.seek(position)
-        record = self.__read_until(RECORD_SEP)
+        record = self.__read_until()
 
         if self.caching_enabled:
             self.store_cache.put(position, record)
 
         return record
 
     # @profile
-    def __read_until(self, separator):
+    def __read_until(self):
         data = None
         while True:
             chunk = self.store_file.read(self.config.STORE_READ_BUFFER_SIZE)
 
             if len(chunk) == 0:
                 return data
                 # raise Exception("EOF store file! Data read error.")
             i = chunk.find(RECORD_SEP)
 
             if i > 0:
-                chunk = chunk[:i+1]
+                chunk = chunk[:i + 1]
                 if data is None:
                     data = chunk
                 else:
                     data += chunk
                 break
 
             if data is None:
                 data = chunk
             else:
                 data += chunk
-        self.logger.debug("store __read_until: "+str(data))
+        self.logger.debug("store __read_until: " + str(data))
         return data
 
 
 class Indexer:
     '''
     Manages indexes. Creates new index when an index is full.
     Searches all indexes for get requests.
     Provides same get/put/del method as single index but over multuple files.
     '''
 
     def __init__(self, tablemeta, config, logger):
         self.tablemeta = tablemeta
         self.config = config
         self.logger = logging.getLogger('indexer')
-        self.index_list = [] #future range index.
+        self.index_list = []  # future range index.
         self.index_id = 0
         self.load_indexes()
-        #if no index currenlty exist, create new live index.
+        # if no index currenlty exist, create new live index.
         if len(self.index_list) == 0:
             self.index_list.append(Index(tablemeta, config, logger, self.index_id))
             self.live_index = self.index_list[self.index_id]
 
     def close(self):
         for idx in self.index_list:
             idx.close()
 
     def load_indexes(self):
         for f in os.listdir(self.config.cog_data_dir(self.tablemeta.namespace)):
             if self.config.INDEX in f:
                 if self.tablemeta.name == self.config.get_table_name(f):
-                    self.logger.info("loading index file: "+f)
+                    self.logger.info("loading index file: " + f)
                     id = self.config.index_id(f)
                     index = Index(self.tablemeta, self.config, self.logger, id)
                     self.index_list.append(index)
-                    #make the latest index the live index.
+                    # make the latest index the live index.
                     if id >= self.index_id:
                         self.index_id = id
                         self.live_index = index
 
     def put(self, key, store_position, store):
-            resp = self.live_index.put(key, store_position, store)
-            self.logger.debug("Key: "+key+" indexed in: "+self.live_index.name)
+        resp = self.live_index.put(key, store_position, store)
+        self.logger.debug("Key: " + key + " indexed in: " + self.live_index.name)
+        return resp
 
     # @profile
     def get(self, key, store):
         idx = self.index_list[0]  # only one index file.
         return idx.get(key, store)
 
     def scanner(self, store):
         for idx in self.index_list:
-            self.logger.debug("SCAN: index: "+idx.name)
+            self.logger.debug("SCAN: index: " + idx.name)
             for r in idx.scanner(store):
                 yield r
 
-
     def delete(self, key, store):
         for idx in self.index_list:
             if idx.delete(key, store):
                 return True
             else:
                 return False
 
 
 def cog_hash(string, index_capacity):
-    return xxhash.xxh32(string, seed=2).intdigest() % index_capacity
+    return xxhash.xxh32(string, seed=2).intdigest() % index_capacity
```

### Comparing `cogdb-3.0.5/cog/database.py` & `cogdb-3.0.6/cog/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 import socket
 import uuid
 from .core import Table
 from . import config
 import xxhash
 import csv
 import shlex
+from collections import OrderedDict
 
 
 # functions
 
 def out_nodes(v):
-    return (v + "__:out:__")
+    return v + "__:out:__"
 
 
 def in_nodes(v):
-    return (v + "__:in:__")
+    return v + "__:in:__"
 
 
 # https://www.w3.org/TR/n-triples/#sec-n-triples-language
 def hash_predicate(predicate):
     return str(xxhash.xxh32(predicate, seed=2).intdigest())
 
 
@@ -45,26 +46,37 @@
 
     if len(tokens) > 3:  # nQuad
         context = tokens[3].strip()
 
     return subject, predicate, object, context
 
 
+class CacheData:
+    def __init__(self, position, value):
+        self.store_position = position
+        self.value = value
+
+    def __str__(self):
+        return f"CacheData(position: {self.store_position}, value: {self.value})"
+
+    __repr__ = __str__
+
 class Cog:
     """
         Read index file, record records stored in 'store' and write out new store file. Update index with position in store.
     """
 
     def __init__(self, shared_cache=None):
         self.logger = logging.getLogger('database')
         self.config = config
         self.logger.info("Cog init.")
         self.namespaces = {}
         self.current_table = None
         self.shared_cache = shared_cache
+        self.cache = OrderedDict()
         '''creates Cog instance files.'''
         if os.path.exists(self.config.cog_instance_sys_file()):
             f = open(self.config.cog_instance_sys_file(), "rb")
             self.m_info = pickle.load(f)
             self.instance_id = self.m_info["m_instance_id"]
             f.close()
         else:
@@ -223,48 +235,65 @@
         new_record = Record(data.key, data.value, value_type='l')
         if record is not None:
             new_record.set_value_link(record.store_position)
         position = self.current_table.store.save(new_record)
         self.current_table.indexer.put(new_record.key, position, self.current_table.store)
 
     def put_set(self, data):
-        '''
-        Creates or appends to a set. If the key does not exist a new list is created, else it adds to the set.
-        :param data:
-        :return:
-        '''
-        assert type(data.key) is str, "Only string type is supported."
-        assert type(data.value) is str, "Only string type is supported."
-        record = self.current_table.indexer.get(data.key, self.current_table.store)
-        # skip insert into store-list if value already present.
-        new_record = Record(data.key, data.value, value_type='l')
-        if record is not None:
-            if data.value not in record.value:  # record value is a linked list.
-                new_record.set_value_link(record.store_position)
-                position = self.current_table.store.save(new_record)
-                self.current_table.indexer.put(new_record.key, position, self.current_table.store)
+        assert isinstance(data.key, str), "Only string type is supported."
+        assert isinstance(data.value, str), "Only string type is supported."
+
+        # use (table name, key) as the cache key
+        cache_key = (self.current_table.table_meta.name, data.key)
+
+        if cache_key in self.cache:
+            record = self.cache[cache_key]
         else:
-            # insert new record
+            record = self.current_table.indexer.get(data.key, self.current_table.store)
+            if len(self.cache) > self.config.LEVEL_2_CACHE_SIZE:
+                self.cache.popitem(last=False)
+
+        new_record = Record(data.key, data.value, value_type='l')
+
+        if record is not None and data.value not in record.value:
+            new_record.set_value_link(record.store_position)
+            position = self.current_table.store.save(new_record)
+            self.current_table.indexer.put(new_record.key, position, self.current_table.store)
+
+            if cache_key in self.cache and data.value not in self.cache[cache_key].value:
+                self.cache[cache_key].value.add(data.value)
+                self.cache[cache_key].store_position = position
+            else:
+                self.cache[cache_key] = CacheData(position, {data.value})
+
+        elif record is None:
             position = self.current_table.store.save(new_record)
             self.current_table.indexer.put(new_record.key, position, self.current_table.store)
+            self.cache[cache_key] = CacheData(position, {data.value})
+        self.cache.move_to_end(cache_key)
 
     def get(self, key):
+        if key in self.cache:
+            return self.cache[key]
         return self.current_table.indexer.get(key, self.current_table.store)
 
     def scanner(self, table=None, scan_filter=None):
         scan_itr = self.current_table.indexer.scanner(self.current_table.store) if not table else table.indexer.scanner(
             table.store)
         for r in scan_itr:
             if scan_filter:
                 yield scan_filter.process(r.key)
             else:
                 yield r
 
     def delete(self, key):
         self.current_table.indexer.delete(key, self.current_table.store)
+        cache_key = (self.current_table.table_meta.name, key)
+        if cache_key in self.cache:
+            del self.cache[cache_key]
 
     def delete_edge(self, vertex1, predicate, vertex2):
         """
         Deletes edge in both directions.
         :param vertex1:
         :param predicate:
         :param vertex2:
```

### Comparing `cogdb-3.0.5/cog/torque.py` & `cogdb-3.0.6/cog/torque.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             self.id = "_:{}{}".format(BlankNode.ID_PREFIX, label)
 
     def __str__(self):
         return self.id
 
     @classmethod
     def is_id(cls, label):
-        # print("--- > is_id", label)
         return label.startswith("_:" + BlankNode.ID_PREFIX)
 
 
 class Graph:
     """
     Creates a graph object.
     """
```

### Comparing `cogdb-3.0.5/cog/view.py` & `cogdb-3.0.6/cog/view.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/cogdb.egg-info/SOURCES.txt` & `cogdb-3.0.6/cogdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_cache.py` & `cogdb-3.0.6/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_core.py` & `cogdb-3.0.6/test/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,43 @@
 
         index.close()
         store.close()
 
         #set original config back
         config.INDEX_CAPACITY = orig_conf
 
+    def test_collision_large(self):
+        orig_conf = config.INDEX_CAPACITY
+        dictConfig(config.logging_config)
+        logger = logging.getLogger()
+
+        table = Table("testdb", "test_table", "test_xcvzdfsadx", config, logger)
+        config.INDEX_CAPACITY = 4
+        print(config.COG_HOME)
+        store = table.store
+        index = table.indexer.index_list[0]
+
+        num_records = 1000  # Increase this as per your requirements
+        expected_data_list = [Record(f"rocket{i}", f"rocket_name_{i}") for i in range(num_records)]
+
+        for rec in expected_data_list:
+            position = store.save(rec)
+            index.put(rec.key, position, store)
+
+        for rec in expected_data_list:
+            returned_data = index.get(rec.key, store)
+            print(f"retrieved data for key {rec.key}: {str(returned_data)}")
+            self.assertTrue(rec.is_equal_val(returned_data))
+
+        index.close()
+        store.close()
+
+        # set original config back
+        config.INDEX_CAPACITY = orig_conf
+
     def test_put_get_list(self):
         dictConfig(config.logging_config)
         logger = logging.getLogger()
 
         fruits = (["apple", "orange", "banana", "pears", "cherry", "mango"])
 
         table = Table("testdb2", "test_table", "test_xcvzdfsadx2", config, logger)
```

### Comparing `cogdb-3.0.5/test/test_db.py` & `cogdb-3.0.6/test/test_db.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_embeddings.py` & `cogdb-3.0.6/test/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_functions.py` & `cogdb-3.0.6/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_index.py` & `cogdb-3.0.6/test/test_index.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_indexer.py` & `cogdb-3.0.6/test/test_indexer.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_lib.py` & `cogdb-3.0.6/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_sim.py` & `cogdb-3.0.6/test/test_sim.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.5/test/test_torque.py` & `cogdb-3.0.6/test/test_torque.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from cog.torque import Graph
 import unittest
 import os
 import shutil
 
 DIR_NAME = "TorqueTest"
 
-#target api set
+
+# target api set
 # in("predicate"), out("predicate"), all, count, tag
 # next release .forEach(function), this can do filter, adding values etc.
 
 # // The working set of this is bob and dani
 # g.V("<charlie>").Out("<follows>").All()
 # // The working set of this is fred, as alice follows bob and bob follows fred.
 # g.V("<alice>").Out("<follows>").Out("<follows>").All()
@@ -18,16 +19,16 @@
 # // Finds all things dani points at on the status linkage.
 # // Result is bob, greg and cool_person
 # g.V("<dani>").Out(["<follows>", "<status>"]).All()
 # // Finds all things dani points at on the status linkage, given from a separate query path.
 # // Result is {"id": "cool_person", "pred": "<status>"}
 # g.V("<dani>").Out(g.V("<status>"), "pred").All()
 
-#https://docs.janusgraph.org/latest/gremlin.html
-#https://tinkerpop.apache.org/gremlin.html
+# https://docs.janusgraph.org/latest/gremlin.html
+# https://tinkerpop.apache.org/gremlin.html
 
 
 def ordered(obj):
     if isinstance(obj, dict):
         return sorted((k, ordered(v)) for k, v in list(obj.items()))
     if isinstance(obj, list):
         return sorted(ordered(x) for x in obj)
@@ -37,25 +38,28 @@
 
 class TorqueTest(unittest.TestCase):
     maxDiff = None
 
     @classmethod
     def setUpClass(cls):
 
-        if not os.path.exists("/tmp/"+DIR_NAME):
+        if os.path.exists("/tmp/" + DIR_NAME):
+            shutil.rmtree("/tmp/" + DIR_NAME)
+
+        if not os.path.exists("/tmp/" + DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
         data_dir = "test/test-data/test.nq"
         # choose appropriate path based on where the test is called from.
         if os.path.exists("test-data/test.nq"):
             data_dir = "test-data/test.nq"
 
         TorqueTest.g = Graph(graph_name="people", cog_home=DIR_NAME)
         TorqueTest.g.load_triples(data_dir, "people")
-        #print TorqueTest.g.v().all()
+        # print TorqueTest.g.v().all()
         print(">>> test setup complete.\n")
 
     def test_torque_1(self):
         self.assertEqual(1, TorqueTest.g.v("<alice>").out().count())
 
     def test_torque_2(self):
         expected = {'result': [{'source': 'cool_person', 'id': 'cool_person'}, {'source': '<fred>', 'id': '<fred>'}]}
@@ -64,35 +68,44 @@
 
     def test_torque_3(self):
         expected = {"result": [{"source": "<fred>", "id": "<greg>", "target": "<greg>"}]}
         actual = TorqueTest.g.v("<bob>").out().tag("source").out().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_4(self):
-        expected = {'result': [{'source': 'cool_person', 'id': '<bob>', 'target': '<bob>'}, {'source': 'cool_person', 'id': '<dani>', 'target': '<dani>'}, {'source': 'cool_person', 'id': '<greg>', 'target': '<greg>'}, {'source': '<fred>', 'id': '<bob>', 'target': '<bob>'}, {'source': '<fred>', 'id': '<emily>', 'target': '<emily>'}]}
+        expected = {'result': [{'source': 'cool_person', 'id': '<bob>', 'target': '<bob>'},
+                               {'source': 'cool_person', 'id': '<dani>', 'target': '<dani>'},
+                               {'source': 'cool_person', 'id': '<greg>', 'target': '<greg>'},
+                               {'source': '<fred>', 'id': '<bob>', 'target': '<bob>'},
+                               {'source': '<fred>', 'id': '<emily>', 'target': '<emily>'}]}
         actual = TorqueTest.g.v("<bob>").out().tag("source").inc().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_5(self):
-        expected = {'result': [{'source': '<greg>', 'id': '<dani>', 'target': '<dani>'}, {'source': '<greg>', 'id': '<fred>', 'target': '<fred>'}]}
+        expected = {'result': [{'source': '<greg>', 'id': '<dani>', 'target': '<dani>'},
+                               {'source': '<greg>', 'id': '<fred>', 'target': '<fred>'}]}
         actual = TorqueTest.g.v("<fred>").out().tag("source").inc().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_6(self):
-        expected = {'result': [{'source': '<greg>', 'id': '<dani>', 'target': '<dani>'}, {'source': '<greg>', 'id': '<fred>', 'target': '<fred>'}]}
+        expected = {'result': [{'source': '<greg>', 'id': '<dani>', 'target': '<dani>'},
+                               {'source': '<greg>', 'id': '<fred>', 'target': '<fred>'}]}
         actual = TorqueTest.g.v("<fred>").out().tag("source").inc().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_7(self):
         expected = {'result': [{'source': '<greg>', 'id': 'cool_person', 'target': 'cool_person'}]}
         actual = TorqueTest.g.v("<fred>").out().tag("source").out().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_8(self):
-        expected = {'result': [{'source': '<greg>', 'id': 'cool_person', 'target': 'cool_person'}, {'source': '<greg>', 'id': '<bob>', 'target': '<bob>'}, {'source': '<greg>', 'id': '<greg>', 'target': '<greg>'}, {'source': '<greg>', 'id': '<greg>', 'target': '<greg>'}]}
+        expected = {'result': [{'source': '<greg>', 'id': 'cool_person', 'target': 'cool_person'},
+                               {'source': '<greg>', 'id': '<bob>', 'target': '<bob>'},
+                               {'source': '<greg>', 'id': '<greg>', 'target': '<greg>'},
+                               {'source': '<greg>', 'id': '<greg>', 'target': '<greg>'}]}
         actual = TorqueTest.g.v("<fred>").out().tag("source").inc().out().tag("target").all()
         self.assertEqual(ordered(expected), ordered(actual))
 
     def test_torque_9(self):
         expected = {'result': [{'source': '<fred>', 'id': '<fred>'}]}
         actual = TorqueTest.g.v("<bob>").out(["<follows>"]).tag("source").all()
         self.assertTrue(ordered(expected) == ordered(actual))
@@ -105,27 +118,29 @@
     # bad predicates, should not break test
     def test_torque_11(self):
         expected = {'result': []}
         actual = TorqueTest.g.v("<bob>").out(["<follows>zzz", "<status>zzz"]).tag("source").all()
         self.assertTrue(ordered(expected) == ordered(actual))
 
     def test_torque_12(self):
-        expected = {'result': [{'id': '<bob>'}, {'id': '<dani>'}, {'id': '<emily>'}, {'id': '"cool_person"'}, {'id': '<greg>'}, {'id': '<fred>'}, {'id': '<alice>'}, {'id': '<charlie>'}]}
-        actual = TorqueTest.g.scan(3,'v')
+        actual = TorqueTest.g.scan(3, 'v')
+        print(actual)
         self.assertTrue(3 == len(actual['result']))
         with self.assertRaises(AssertionError):
-            TorqueTest.g.scan('v',3)
+            TorqueTest.g.scan('v', 3)
 
     def test_torque_13(self):
         expected = {'result': [{'id': '<greg>'}, {'id': '<dani>'}, {'id': '<bob>'}]}
         actual = TorqueTest.g.v().inc(["<status>"]).all()
         self.assertTrue(expected == actual)
 
     def test_torque_14(self):
-        expected = {'result': [{'id': '<fred>'}, {'id': '<dani>'}, {'id': '<charlie>'}, {'id': '<dani>'}, {'id': '<charlie>'}, {'id': '<alice>'}]}
+        expected = {
+            'result': [{'id': '<fred>'}, {'id': '<dani>'}, {'id': '<charlie>'}, {'id': '<dani>'}, {'id': '<charlie>'},
+                       {'id': '<alice>'}]}
         actual = TorqueTest.g.v().inc(["<status>"]).inc("<follows>").all()
         self.assertTrue(expected == actual)
 
     def test_torque_15(self):
         view = TorqueTest.g.v("<bob>").out().tag("from").inc().tag("to").view("bob_view")
         print(view.url)
         self.assertTrue(view.url.endswith("bob_view.html"))
@@ -155,20 +170,21 @@
 
     def test_torque_20(self):
         expected = {'result': [{'id': '<bob>'}, {'id': '<emily>'}]}
         actual = TorqueTest.g.v().has("<follows>", "<fred>").all('e')
         self.assertTrue(expected == actual)
 
     def test_torque_21(self):
-        expected = {'result': [{'id': '<dani>', 'edges': ['<follows>']}, {'id': '<charlie>', 'edges': ['<follows>']}, {'id': '<alice>', 'edges': ['<follows>']}]}
+        expected = {'result': [{'id': '<dani>', 'edges': ['<follows>']}, {'id': '<charlie>', 'edges': ['<follows>']},
+                               {'id': '<alice>', 'edges': ['<follows>']}]}
         actual = TorqueTest.g.v().has("<follows>", "<fred>").inc().all('e')
         self.assertTrue(expected == actual)
 
     @classmethod
     def tearDownClass(cls):
         TorqueTest.g.close()
-        shutil.rmtree("/tmp/"+DIR_NAME)
+        shutil.rmtree("/tmp/" + DIR_NAME)
         print("*** deleted test data.")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cogdb-3.0.5/test/test_torque2.py` & `cogdb-3.0.6/test/test_torque2.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     else:
         return obj
 
 class TorqueTest2(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
+        if os.path.exists("/tmp/"+DIR_NAME):
+            shutil.rmtree("/tmp/"+DIR_NAME)
+
         if not os.path.exists("/tmp/"+DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
     def test_torque_2(self):
         TorqueTest2.g = Graph(graph_name="better_graph", cog_home=DIR_NAME)
         TorqueTest2.g.put("A", "is better than", "B")\
             .put("B", "is better than", "C")\
```

### Comparing `cogdb-3.0.5/test/test_torque3.py` & `cogdb-3.0.6/test/test_torque3.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 DIR_NAME = "TorqueTest3"
 
 
 class TorqueTest3(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
-        if not os.path.exists("/tmp/"+DIR_NAME):
+        if os.path.exists("/tmp/" + DIR_NAME):
+            shutil.rmtree("/tmp/" + DIR_NAME)
+
+        if not os.path.exists("/tmp/" + DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
     def test_torque_load_nq(self):
         nq_file = "test/test-data/100lines.nq"
         if os.path.exists("test-data/100lines.nq"):
             nq_file = "test-data/100lines.nq"
         g = Graph(graph_name="movies3", cog_path_prefix="/tmp/" + DIR_NAME)
```

### Comparing `cogdb-3.0.5/test/test_torque4.py` & `cogdb-3.0.6/test/test_torque4.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 
 class TorqueTest(unittest.TestCase):
     maxDiff = None
 
     @classmethod
     def setUpClass(cls):
 
-        if not os.path.exists("/tmp/"+DIR_NAME):
+        if os.path.exists("/tmp/" + DIR_NAME):
+            shutil.rmtree("/tmp/" + DIR_NAME)
+
+        if not os.path.exists("/tmp/" + DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
         data_dir = "test/test-data/test_func.nq"
         # choose appropriate path based on where the test is called from.
         if os.path.exists("test-data/test_func.nq"):
             data_dir = "test-data/test_func.nq"
```

### Comparing `cogdb-3.0.5/test/test_torque5.py` & `cogdb-3.0.6/test/test_torque5.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 class TorqueTest(unittest.TestCase):
     maxDiff = None
 
     @classmethod
     def setUpClass(cls):
 
-        if not os.path.exists("/tmp/"+DIR_NAME):
+        if os.path.exists("/tmp/" + DIR_NAME):
+            shutil.rmtree("/tmp/" + DIR_NAME)
+
+        if not os.path.exists("/tmp/" + DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
         data_dir = "test/test-data/test-data-sm.json"
         if os.path.exists("test-data/test-data-sm.json"):
             data_dir = "test-data/test-data-sm.json"
 
         TorqueTest.g = Graph(graph_name="people", cog_home=DIR_NAME)
```

### Comparing `cogdb-3.0.5/test/test_torque6.py` & `cogdb-3.0.6/test/test_torque6.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 
 class TorqueTest(unittest.TestCase):
     maxDiff = None
 
     @classmethod
     def setUpClass(cls):
+        if os.path.exists("/tmp/" + DIR_NAME):
+            shutil.rmtree("/tmp/" + DIR_NAME)
+
         if not os.path.exists("/tmp/" + DIR_NAME):
             os.mkdir("/tmp/" + DIR_NAME)
 
     def test_torque_drop_1(self):
         g = Graph(graph_name="test_drop", cog_home=DIR_NAME)
         expected = {'result': [{'id': 'greg'}]}
         g.put("bob", "friends", "greg")
```

