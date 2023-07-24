# Comparing `tmp/pydantic_neo4j-0.3.4.tar.gz` & `tmp/pydantic_neo4j-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.3.4.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.3.5.tar", max compression
```

## Comparing `pydantic_neo4j-0.3.4.tar` & `pydantic_neo4j-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      869 2023-07-18 03:47:13.989691 pydantic_neo4j-0.3.4/pydantic_neo4j/__init__.py
--rw-r--r--   0        0        0     5892 2023-07-24 20:16:00.488940 pydantic_neo4j-0.3.4/pydantic_neo4j/create_operations.py
--rw-r--r--   0        0        0     4872 2023-07-18 00:44:33.557638 pydantic_neo4j-0.3.4/pydantic_neo4j/database_operations.py
--rw-r--r--   0        0        0     3371 2023-07-24 19:45:48.667813 pydantic_neo4j-0.3.4/pydantic_neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10443 2023-07-24 20:17:14.093485 pydantic_neo4j-0.3.4/pydantic_neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-18 02:22:59.959087 pydantic_neo4j-0.3.4/pydantic_neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      601 2023-07-24 20:18:36.977594 pydantic_neo4j-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4039 2023-07-18 03:47:13.985687 pydantic_neo4j-0.3.4/README.md
--rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pydantic_neo4j-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      869 2023-07-18 03:47:13.989691 pydantic_neo4j-0.3.5/pydantic_neo4j/__init__.py
+-rw-r--r--   0        0        0     5892 2023-07-24 20:16:00.488940 pydantic_neo4j-0.3.5/pydantic_neo4j/create_operations.py
+-rw-r--r--   0        0        0     4872 2023-07-18 00:44:33.557638 pydantic_neo4j-0.3.5/pydantic_neo4j/database_operations.py
+-rw-r--r--   0        0        0     3371 2023-07-24 19:45:48.667813 pydantic_neo4j-0.3.5/pydantic_neo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10443 2023-07-24 20:17:14.093485 pydantic_neo4j-0.3.5/pydantic_neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-18 02:22:59.959087 pydantic_neo4j-0.3.5/pydantic_neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      601 2023-07-24 20:50:58.209625 pydantic_neo4j-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4039 2023-07-18 03:47:13.985687 pydantic_neo4j-0.3.5/README.md
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pydantic_neo4j-0.3.5/PKG-INFO
```

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/__init__.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/create_operations.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/database_operations.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/graph_base_models.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/match_operations.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/match_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pydantic_neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.3.5/pydantic_neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/pyproject.toml` & `pydantic_neo4j-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `pydantic_neo4j-0.3.4/README.md` & `pydantic_neo4j-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.4/PKG-INFO` & `pydantic_neo4j-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

