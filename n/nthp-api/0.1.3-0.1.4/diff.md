# Comparing `tmp/nthp_api-0.1.3.tar.gz` & `tmp/nthp_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nthp_api-0.1.3.tar", max compression
+gzip compressed data, was "nthp_api-0.1.4.tar", max compression
```

## Comparing `nthp_api-0.1.3.tar` & `nthp_api-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/__init__.py
--rw-r--r--   0        0        0     2051 2023-07-23 23:36:08.316226 nthp_api-0.1.3/nthp_api/cli/__init__.py
--rw-r--r--   0        0        0      386 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/cli/logs.py
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/assets.py
--rw-r--r--   0        0        0      549 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/config.py
--rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/content.py
--rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/database.py
--rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/documents.py
--rw-r--r--   0        0        0    12110 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/dumper.py
--rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/history.py
--rw-r--r--   0        0        0     7687 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/loader.py
--rw-r--r--   0        0        0     4694 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/models.py
--rw-r--r--   0        0        0     1124 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/parallel.py
--rw-r--r--   0        0        0     8105 2023-07-23 23:07:15.093248 nthp_api-0.1.3/nthp_api/nthp_build/people.py
--rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/playwrights.py
--rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/roles.py
--rw-r--r--   0        0        0     9776 2023-07-23 23:04:02.359547 nthp_api-0.1.3/nthp_api/nthp_build/schema.py
--rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/search.py
--rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/shows.py
--rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/smugmug.py
--rw-r--r--   0        0        0     9756 2023-07-23 23:32:24.722305 nthp_api-0.1.3/nthp_api/nthp_build/spec.py
--rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/trivia.py
--rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.3/nthp_api/nthp_build/venues.py
--rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/nthp_build/years.py
--rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/__init__.py
--rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/album.py
--rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/client.py
--rw-r--r--   0        0        0      358 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/config.py
--rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/database.py
--rw-r--r--   0        0        0     1134 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/schema.py
--rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.3/nthp_api/smugmugger/smugmug.py
--rw-r--r--   0        0        0     1917 2023-07-23 23:36:28.880360 nthp_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 nthp_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2020 2023-07-23 23:42:23.589970 nthp_api-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-23 23:44:46.802802 nthp_api-0.1.4/nthp_api/cli/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/cli/logs.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/assets.py
+-rw-r--r--   0        0        0      549 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/config.py
+-rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/content.py
+-rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/database.py
+-rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/documents.py
+-rw-r--r--   0        0        0    12110 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/dumper.py
+-rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/history.py
+-rw-r--r--   0        0        0     7687 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/loader.py
+-rw-r--r--   0        0        0     4694 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/models.py
+-rw-r--r--   0        0        0     1124 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/parallel.py
+-rw-r--r--   0        0        0     8105 2023-07-23 23:07:15.093248 nthp_api-0.1.4/nthp_api/nthp_build/people.py
+-rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/playwrights.py
+-rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/roles.py
+-rw-r--r--   0        0        0     9776 2023-07-23 23:04:02.359547 nthp_api-0.1.4/nthp_api/nthp_build/schema.py
+-rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/search.py
+-rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/shows.py
+-rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/smugmug.py
+-rw-r--r--   0        0        0     9756 2023-07-23 23:32:24.722305 nthp_api-0.1.4/nthp_api/nthp_build/spec.py
+-rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/trivia.py
+-rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/venues.py
+-rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/nthp_build/years.py
+-rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/album.py
+-rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/client.py
+-rw-r--r--   0        0        0      358 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/config.py
+-rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/database.py
+-rw-r--r--   0        0        0     1134 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/schema.py
+-rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/smugmug.py
+-rw-r--r--   0        0        0     2138 2023-07-23 23:45:03.190902 nthp_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 nthp_api-0.1.4/PKG-INFO
```

### Comparing `nthp_api-0.1.3/nthp_api/cli/__init__.py` & `nthp_api-0.1.4/nthp_api/cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,22 +64,14 @@
 @cli.command()
 def build(path):
     # Set settings using environment variables as workers and threads will recreate
     # the settings object and not pick up the values if set here.
     environ["DB_URI"] = ":memory:"
     environ["CONTENT_ROOT"] = str(path)
 
-    from nthp_api.nthp_build.config import settings
-
-    # Ensure that the settings are set correctly, if this breaks we've probably imported
-    # settings before setting the env vars.
-    assert (
-        settings.content_root == path
-    ), f"Content root improperly loaded, {settings.content_root} != {path}"
-
     log.info(f"Building from {path} using in-memory database")
 
     import nthp_api.smugmugger.database
     from nthp_api.nthp_build import database, dumper, loader, smugmug
 
     database.init_db(create=True)
     loader.run_loaders()
```

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/assets.py` & `nthp_api-0.1.4/nthp_api/nthp_build/assets.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/config.py` & `nthp_api-0.1.4/nthp_api/nthp_build/config.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/content.py` & `nthp_api-0.1.4/nthp_api/nthp_build/content.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/database.py` & `nthp_api-0.1.4/nthp_api/nthp_build/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/documents.py` & `nthp_api-0.1.4/nthp_api/nthp_build/documents.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/dumper.py` & `nthp_api-0.1.4/nthp_api/nthp_build/dumper.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/loader.py` & `nthp_api-0.1.4/nthp_api/nthp_build/loader.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/models.py` & `nthp_api-0.1.4/nthp_api/nthp_build/models.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/parallel.py` & `nthp_api-0.1.4/nthp_api/nthp_build/parallel.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/people.py` & `nthp_api-0.1.4/nthp_api/nthp_build/people.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/playwrights.py` & `nthp_api-0.1.4/nthp_api/nthp_build/playwrights.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/roles.py` & `nthp_api-0.1.4/nthp_api/nthp_build/roles.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/schema.py` & `nthp_api-0.1.4/nthp_api/nthp_build/schema.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/shows.py` & `nthp_api-0.1.4/nthp_api/nthp_build/shows.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/smugmug.py` & `nthp_api-0.1.4/nthp_api/nthp_build/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/spec.py` & `nthp_api-0.1.4/nthp_api/nthp_build/spec.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/trivia.py` & `nthp_api-0.1.4/nthp_api/nthp_build/trivia.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/venues.py` & `nthp_api-0.1.4/nthp_api/nthp_build/venues.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/nthp_build/years.py` & `nthp_api-0.1.4/nthp_api/nthp_build/years.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/smugmugger/album.py` & `nthp_api-0.1.4/nthp_api/smugmugger/album.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/smugmugger/client.py` & `nthp_api-0.1.4/nthp_api/smugmugger/client.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/smugmugger/database.py` & `nthp_api-0.1.4/nthp_api/smugmugger/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/smugmugger/schema.py` & `nthp_api-0.1.4/nthp_api/smugmugger/schema.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/nthp_api/smugmugger/smugmug.py` & `nthp_api-0.1.4/nthp_api/smugmugger/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.3/pyproject.toml` & `nthp_api-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "nthp_api"
-version = "0.1.3"
-description = ""
+version = "0.1.4"
+description = "This is a CLI tool for building the Nottingham New Theatre's History Project content database."
 authors = ["Will Pimblett <will@wjdp.uk>"]
 license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/newtheatre/nthp-api"
+repository = "https://github.com/newtheatre/nthp-api"
 
 [tool.poetry.scripts]
 nthp = "nthp_api.cli:cli"
 nthp_api = "nthp_api.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

