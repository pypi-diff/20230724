# Comparing `tmp/mongodriver-1.2.1.tar.gz` & `tmp/mongodriver-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.1.tar", last modified: Thu Jul 20 15:40:50 2023, max compression
+gzip compressed data, was "mongodriver-1.2.2.tar", last modified: Mon Jul 24 15:55:22 2023, max compression
```

## Comparing `mongodriver-1.2.1.tar` & `mongodriver-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.175050 mongodriver-1.2.1/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.1/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-20 15:40:50.175156 mongodriver-1.2.1/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.1/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.1/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-07-20 15:40:50.175441 mongodriver-1.2.1/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      891 2023-07-20 14:49:45.000000 mongodriver-1.2.1/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.172850 mongodriver-1.2.1/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.174056 mongodriver-1.2.1/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.1/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     7887 2023-07-20 15:20:58.000000 mongodriver-1.2.1/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.174916 mongodriver-1.2.1/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      304 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.548739 mongodriver-1.2.2/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.2/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-24 15:55:22.548868 mongodriver-1.2.2/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.2/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.2/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-07-24 15:55:22.549247 mongodriver-1.2.2/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      891 2023-07-24 15:54:30.000000 mongodriver-1.2.2/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.545881 mongodriver-1.2.2/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.547497 mongodriver-1.2.2/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.2/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     7943 2023-07-24 15:51:04.000000 mongodriver-1.2.2/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.548562 mongodriver-1.2.2/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      304 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.1/LICENSE` & `mongodriver-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.1/PKG-INFO` & `mongodriver-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.1
+Version: 1.2.2
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongodriver-1.2.1/README.md` & `mongodriver-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.1/setup.py` & `mongodriver-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.2.1',
+    version='1.2.2',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
     packages=find_packages('src'),
     url='https://github.com/jakestrouse00/mongodriver',
     package_dir={'': 'src'},
     keywords='mongodb',
```

### Comparing `mongodriver-1.2.1/src/mongodriver/mongodriver.py` & `mongodriver-1.2.2/src/mongodriver/mongodriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,36 +111,44 @@
 
     def create(self, data: dict) -> Document:
         """CREATE A DOCUMENT FROM A DICT AND RETURN THE Document OBJECT"""
         document = self.client.insert_one(data)
         python_document = Document(document.inserted_id, data, self.client)
         return python_document
 
-    def update(self, data: dict | Document, new_values: dict, sort: dict = None) -> Document:
+    def update(
+        self, data: dict | Document, new_values: dict, sort: dict = None
+    ) -> Document:
         if "_id" in new_values.keys():
             new_values.pop("_id")
         if isinstance(data, Document):
             if sort is not None:
                 sort = sort.items()
-            self.client.find_one_and_update(filter={"_id": ObjectId(data._id)}, update={"$set" :new_values}, sort=sort, return_document=True)
+            self.client.find_one_and_update(
+                filter={"_id": ObjectId(data._id)},
+                update={"$set": new_values},
+                sort=sort,
+                return_document=True,
+            )
             for _, (key, value) in enumerate(new_values.items()):
-                class_value = Variable(
-                    data._id, key, value, self.client, data
-                )
+                class_value = Variable(data._id, key, value, self.client, data)
 
                 data.variables[key] = new_values[key]
                 # setattr(self, variable, class_value)
                 data.__dict__[key] = class_value
             return data
         else:
-            document = self.client.find_one_and_update(filter=data, update={"$set": update},
-                                                       sort=sort.items(), return_document=True)
+            document = self.client.find_one_and_update(
+                filter=data,
+                update={"$set": update},
+                sort=sort.items(),
+                return_document=True,
+            )
             return Document(document.inserted_id, data, self.client)
 
-
     def remove(self, data: dict | Document):
         if isinstance(data, Document):
             self.client.find_one_and_delete({"_id": ObjectId(data._id)})
         else:
             if "_id" in data.keys() and not isinstance(data["_id"], ObjectId):
                 data["_id"] = ObjectId(data["_id"])
             self.client.find_one_and_delete(data)
@@ -152,42 +160,41 @@
         for document in documents:
             doc_id = document["_id"]
             document.pop("_id")
             python_document = Document(str(doc_id), document, self.client)
             loaded_documents.append(python_document)
         return loaded_documents
 
-    def find(self, search_terms: dict) -> List[Document] | None:
+    def find(self, search_terms: dict) -> List[Document]:
         """FIND A DOCUMENT AND RETURN IT AS A Document CLASS"""
-        if "_id" in search_terms.keys() and not isinstance(search_terms["_id"], ObjectId):
+        if "_id" in search_terms.keys() and not isinstance(
+            search_terms["_id"], ObjectId
+        ):
             search_terms["_id"] = ObjectId(search_terms["_id"])
         processed_documents = []
         documents = self.client.find(search_terms)
-        if len(documents) == 0:
-            return None
         for document in documents:
             doc_id = str(document["_id"])
             python_document = Document(doc_id, document, self.client)
             processed_documents.append(python_document)
         return processed_documents
 
     def find_one(self, search_terms: dict) -> Document | None:
-        if "_id" in search_terms.keys() and not isinstance(search_terms["_id"], ObjectId):
+        if "_id" in search_terms.keys() and not isinstance(
+            search_terms["_id"], ObjectId
+        ):
             search_terms["_id"] = ObjectId(search_terms["_id"])
         document = self.client.find_one(search_terms)
         if document is None:
             return None
         doc_id = str(document["_id"])
         python_document = Document(doc_id, document, self.client)
         return python_document
 
 
-
-
-
 class ObjectPacker:
     # packing and unpacking objects is simple and technically this implementation may not be needed.
     # But I thought it was a nice touch just in case :)
 
     @staticmethod
     def pack(input_dict: dict, packed_name: str = "PackedObject"):
         """PACK A DICT INTO A PYTHON CLASS"""
```

### Comparing `mongodriver-1.2.1/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.2.2/src/mongodriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.1
+Version: 1.2.2
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

