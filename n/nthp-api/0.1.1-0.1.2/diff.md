# Comparing `tmp/nthp_api-0.1.1.tar.gz` & `tmp/nthp_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nthp_api-0.1.1.tar", max compression
+gzip compressed data, was "nthp_api-0.1.2.tar", max compression
```

## Comparing `nthp_api-0.1.1.tar` & `nthp_api-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-22 23:25:03.364745 nthp_api-0.1.1/nthp_api/cli/__init__.py
--rw-r--r--   0        0        0      386 2023-07-22 23:19:37.865743 nthp_api-0.1.1/nthp_api/cli/logs.py
--rw-r--r--   0        0        0        0 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/assets.py
--rw-r--r--   0        0        0      523 2023-07-22 23:19:29.737534 nthp_api-0.1.1/nthp_api/nthp_build/config.py
--rw-r--r--   0        0        0     1103 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/content.py
--rw-r--r--   0        0        0     3996 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/database.py
--rw-r--r--   0        0        0     1427 2023-07-22 23:27:42.751459 nthp_api-0.1.1/nthp_api/nthp_build/documents.py
--rw-r--r--   0        0        0    12110 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/dumper.py
--rw-r--r--   0        0        0      461 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/history.py
--rw-r--r--   0        0        0     7687 2023-07-22 23:11:37.068447 nthp_api-0.1.1/nthp_api/nthp_build/loader.py
--rw-r--r--   0        0        0     4694 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/models.py
--rw-r--r--   0        0        0     1124 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/parallel.py
--rw-r--r--   0        0        0     7912 2023-07-22 21:18:36.830335 nthp_api-0.1.1/nthp_api/nthp_build/people.py
--rw-r--r--   0        0        0     3826 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/playwrights.py
--rw-r--r--   0        0        0     6388 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/roles.py
--rw-r--r--   0        0        0     9700 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/schema.py
--rw-r--r--   0        0        0      416 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/search.py
--rw-r--r--   0        0        0     6446 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/shows.py
--rw-r--r--   0        0        0     1098 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/smugmug.py
--rw-r--r--   0        0        0     9559 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/spec.py
--rw-r--r--   0        0        0     1940 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/trivia.py
--rw-r--r--   0        0        0     2117 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/venues.py
--rw-r--r--   0        0        0     1168 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/nthp_build/years.py
--rw-r--r--   0        0        0      305 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/__init__.py
--rw-r--r--   0        0        0      649 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/album.py
--rw-r--r--   0        0        0     2583 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/client.py
--rw-r--r--   0        0        0      358 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/config.py
--rw-r--r--   0        0        0      661 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/database.py
--rw-r--r--   0        0        0     1134 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/schema.py
--rw-r--r--   0        0        0     2019 2023-07-22 21:18:36.834335 nthp_api-0.1.1/nthp_api/smugmugger/smugmug.py
--rw-r--r--   0        0        0     1887 2023-07-22 23:36:46.538872 nthp_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 nthp_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/cli/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/cli/logs.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/assets.py
+-rw-r--r--   0        0        0      549 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/config.py
+-rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/content.py
+-rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/database.py
+-rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/documents.py
+-rw-r--r--   0        0        0    12110 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/dumper.py
+-rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/history.py
+-rw-r--r--   0        0        0     7687 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/loader.py
+-rw-r--r--   0        0        0     4694 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/models.py
+-rw-r--r--   0        0        0     1124 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/parallel.py
+-rw-r--r--   0        0        0     8105 2023-07-23 23:07:15.093248 nthp_api-0.1.2/nthp_api/nthp_build/people.py
+-rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/playwrights.py
+-rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/roles.py
+-rw-r--r--   0        0        0     9776 2023-07-23 23:04:02.359547 nthp_api-0.1.2/nthp_api/nthp_build/schema.py
+-rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/search.py
+-rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/shows.py
+-rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/smugmug.py
+-rw-r--r--   0        0        0     9610 2023-07-23 23:25:14.890607 nthp_api-0.1.2/nthp_api/nthp_build/spec.py
+-rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/trivia.py
+-rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.2/nthp_api/nthp_build/venues.py
+-rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/nthp_build/years.py
+-rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/album.py
+-rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/client.py
+-rw-r--r--   0        0        0      358 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/config.py
+-rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/database.py
+-rw-r--r--   0        0        0     1134 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/schema.py
+-rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.2/nthp_api/smugmugger/smugmug.py
+-rw-r--r--   0        0        0     1917 2023-07-23 23:26:54.071461 nthp_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 nthp_api-0.1.2/PKG-INFO
```

### Comparing `nthp_api-0.1.1/nthp_api/cli/__init__.py` & `nthp_api-0.1.2/nthp_api/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/assets.py` & `nthp_api-0.1.2/nthp_api/nthp_build/assets.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/config.py` & `nthp_api-0.1.2/nthp_api/nthp_build/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
+from pathlib import Path
 
 from pydantic import BaseSettings
 
 
 class Settings(BaseSettings):
     db_uri: str = "nthp.db"
     branch: str = "master"
-    content_root: str
+    content_root: Path
 
     year_start: int = 1940
     year_end: int = datetime.datetime.now().year
 
     # How many years to wait until guessing someone has left, if it's not been this
     # long we can assume they may still be a student.
     graduation_recency_limit: int = 2
```

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/content.py` & `nthp_api-0.1.2/nthp_api/nthp_build/content.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/database.py` & `nthp_api-0.1.2/nthp_api/nthp_build/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/documents.py` & `nthp_api-0.1.2/nthp_api/nthp_build/documents.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/dumper.py` & `nthp_api-0.1.2/nthp_api/nthp_build/dumper.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/loader.py` & `nthp_api-0.1.2/nthp_api/nthp_build/loader.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/models.py` & `nthp_api-0.1.2/nthp_api/nthp_build/models.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/parallel.py` & `nthp_api-0.1.2/nthp_api/nthp_build/parallel.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/people.py` & `nthp_api-0.1.2/nthp_api/nthp_build/people.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 from collections import defaultdict
 from collections.abc import Iterable
-from typing import Any
 
 import peewee
 from slugify import slugify
 
 from nthp_api.nthp_build import database, models, schema, years
 from nthp_api.nthp_build.config import settings
 
@@ -62,26 +61,30 @@
             ),
         )
         .join(
             database.Show,
             on=(database.PersonRole.target_id == database.Show.id),
             attr="show",
         )
+        .order_by(database.Show.year_id, database.Show.season_sort)
     )
     # Collect all results by show_id
     results_by_show_id: dict[str, list] = defaultdict(list)
-    shows: dict[str, Any] = defaultdict(list)
+    shows: dict[str, database.Show] = {}
     for result in query:
         results_by_show_id[result.target_id].append(result)
         shows[result.target_id] = result.show
 
     return [
         schema.PersonShowRoles(
             show_id=show_id,
             show_title=shows[show_id].title,
+            show_year_id=shows[show_id].year_id,
+            show_year=shows[show_id].year,
+            show_primary_image=shows[show_id].primary_image,
             roles=[
                 schema.PersonShowRoleItem(role=role.role, role_type=role.target_type)
                 for role in roles
             ],
         )
         for show_id, roles in results_by_show_id.items()
     ]
```

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/playwrights.py` & `nthp_api-0.1.2/nthp_api/nthp_build/playwrights.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/roles.py` & `nthp_api-0.1.2/nthp_api/nthp_build/roles.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/schema.py` & `nthp_api-0.1.2/nthp_api/nthp_build/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,17 @@
     role: str | None
     role_type: str
 
 
 class PersonShowRoles(NthpSchema):
     show_id: str
     show_title: str
+    show_year_id: str
+    show_year: int
+    show_primary_image: str | None
     roles: list[PersonShowRoleItem]
 
 
 class PersonCommitteeRole(NthpSchema):
     year_title: str
     year_decade: int
     year_id: str
```

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/shows.py` & `nthp_api-0.1.2/nthp_api/nthp_build/shows.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/smugmug.py` & `nthp_api-0.1.2/nthp_api/nthp_build/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/spec.py` & `nthp_api-0.1.2/nthp_api/nthp_build/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from importlib.metadata import version
 from pathlib import Path
 
 import pydantic.schema
 from pydantic_collections import BaseCollectionModel
 
 from nthp_api.nthp_build import schema
 
@@ -110,15 +111,15 @@
     }
 
 
 SPEC = {
     "openapi": "3.1.0",
     "info": {
         "title": "New Theatre History Project API",
-        "version": "0.0.1",
+        "version": version("nthp_api"),
         "description": "API for serving the content for the New Theatre History "
         "Project. The API is generated from the content repo.",
     },
     "servers": [
         {
             "url": "https://nthp-api.wjdp.uk/v1/{branch}",
             "description": "Production server",
```

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/trivia.py` & `nthp_api-0.1.2/nthp_api/nthp_build/trivia.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/venues.py` & `nthp_api-0.1.2/nthp_api/nthp_build/venues.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/nthp_build/years.py` & `nthp_api-0.1.2/nthp_api/nthp_build/years.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/smugmugger/album.py` & `nthp_api-0.1.2/nthp_api/smugmugger/album.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/smugmugger/client.py` & `nthp_api-0.1.2/nthp_api/smugmugger/client.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/smugmugger/database.py` & `nthp_api-0.1.2/nthp_api/smugmugger/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/smugmugger/schema.py` & `nthp_api-0.1.2/nthp_api/smugmugger/schema.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/nthp_api/smugmugger/smugmug.py` & `nthp_api-0.1.2/nthp_api/smugmugger/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.1/pyproject.toml` & `nthp_api-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nthp_api"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Will Pimblett <will@wjdp.uk>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 nthp = "nthp_api.cli:cli"
 nthp_api = "nthp_api.cli:cli"
@@ -39,14 +39,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 python_version = "3.11"
 files = "nthp_api"
 pretty = true
 ignore_missing_imports = true
+plugins = [ "pydantic.mypy" ]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 
 [tool.ruff]
 select = [
     "E", # pycodestyle errors
```

### Comparing `nthp_api-0.1.1/PKG-INFO` & `nthp_api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nthp-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Will Pimblett
 Author-email: will@wjdp.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

