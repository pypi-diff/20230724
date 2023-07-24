# Comparing `tmp/yente-3.5.0.tar.gz` & `tmp/yente-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.5.0.tar", last modified: Tue Jul  4 08:39:49 2023, max compression
+gzip compressed data, was "yente-3.6.0.tar", last modified: Mon Jul 24 07:45:56 2023, max compression
```

## Comparing `yente-3.5.0.tar` & `yente-3.6.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 08:38:02.000000 yente-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 08:38:02.000000 yente-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-04 08:39:49.863565 yente-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-04 08:38:02.000000 yente-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:39:49.863565 yente-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-04 08:38:02.000000 yente-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-04 08:38:02.000000 yente-3.5.0/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-04 08:38:02.000000 yente-3.5.0/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-04 08:38:02.000000 yente-3.5.0/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 08:38:02.000000 yente-3.5.0/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-04 08:38:02.000000 yente-3.5.0/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 08:38:02.000000 yente-3.5.0/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 08:38:02.000000 yente-3.5.0/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-04 08:38:02.000000 yente-3.5.0/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 08:38:02.000000 yente-3.5.0/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:38:17.000000 yente-3.5.0/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 07:44:08.000000 yente-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 07:44:08.000000 yente-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-24 07:45:56.321580 yente-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 07:44:08.000000 yente-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:45:56.321580 yente-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-24 07:44:08.000000 yente-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-24 07:44:08.000000 yente-3.6.0/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-24 07:44:08.000000 yente-3.6.0/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-24 07:44:08.000000 yente-3.6.0/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 07:44:08.000000 yente-3.6.0/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-24 07:44:08.000000 yente-3.6.0/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 07:44:08.000000 yente-3.6.0/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 07:44:08.000000 yente-3.6.0/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-24 07:44:08.000000 yente-3.6.0/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-24 07:44:08.000000 yente-3.6.0/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:44:23.000000 yente-3.6.0/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/top_level.txt
```

### Comparing `yente-3.5.0/LICENSE` & `yente-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/PKG-INFO` & `yente-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.5.0
+Version: 3.6.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.5.0/README.md` & `yente-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/setup.py` & `yente-3.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.5.0",
+    version="3.6.0",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
-        "followthemoney==3.4.3",
-        "nomenklatura==3.1.0",
+        "followthemoney==3.5.1",
+        "nomenklatura==3.3.4",
         "asyncstdlib==3.10.8",
         "aiocron==1.8",
         "aiocsv==1.2.4",
         "aiofiles==23.1.0",
-        "types-aiofiles==23.1.0.4",
-        "aiohttp[speedups]==3.8.4",
-        "elasticsearch[async]==8.8.0",
-        "fastapi==0.99.1",
-        "uvicorn[standard]==0.22.0",
+        "types-aiofiles>=23.1.0.4,<23.2",
+        "aiohttp[speedups]==3.8.5",
+        "elasticsearch[async]==8.8.2",
+        "fastapi==0.100.0",
+        "uvicorn[standard]==0.23.1",
         "python-multipart==0.0.6",
         "email-validator==2.0.0.post2",
         "structlog==23.1.0",
         "pyicu==2.11",
         "jellyfish==1.0.0",
-        "orjson==3.9.1",
+        "orjson==3.9.2",
         "text-unidecode==1.3",
-        "click==8.0.4",
+        "click==8.1.6",
         "normality==2.4.0",
         "languagecodes==1.1.1",
-        "countrynames==1.15.0",
+        "countrynames==1.15.1",
         "fingerprints==1.1.0",
-        "pantomime==0.6.0",
+        "pantomime==0.6.1",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
             "wheel>=0.29.0",
             "twine",
```

### Comparing `yente-3.5.0/yente/app.py` & `yente-3.6.0/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/cli.py` & `yente-3.6.0/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/data/__init__.py` & `yente-3.6.0/yente/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 async def get_catalog() -> Catalog:
     async with lock:
         if Catalog.instance is None:
             Catalog.instance = await Catalog.load()
     return Catalog.instance
 
 
-async def refresh_catalog() -> None:
+async def _PREV_refresh_catalog() -> None:
     # HACK: PyYAML is so slow that it sometimes hangs the workers, so
     # spawning a thread is unblocking.
 
     async def update_in_thread() -> None:
         log.info("Refreshing manifest/catalog...", catalog=Catalog.instance)
         try:
             Catalog.instance = await Catalog.load()
@@ -29,7 +29,15 @@
 
     thread = threading.Thread(
         target=asyncio.run,
         args=(update_in_thread(),),
         daemon=True,
     )
     thread.start()
+
+
+async def refresh_catalog() -> None:
+    log.info("Refreshing manifest/catalog...", catalog=Catalog.instance)
+    try:
+        Catalog.instance = await Catalog.load()
+    except (Exception, KeyboardInterrupt) as exc:
+        log.exception("Metadata fetch error: %s" % exc)
```

### Comparing `yente-3.5.0/yente/data/common.py` & `yente-3.6.0/yente/data/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,146 +6,124 @@
 from yente import settings
 from yente.data.entity import Entity
 
 EntityProperties = Dict[str, List[Union[str, "EntityResponse"]]]
 
 
 class ErrorResponse(BaseModel):
-    detail: str = Field(..., example="Detailed error message")
+    detail: str = Field(..., examples=["Detailed error message"])
 
 
 class EntityResponse(BaseModel):
-    id: str = Field(..., example="NK-A7z....")
-    caption: str = Field(..., example="John Doe")
-    schema_: str = Field(..., example="LegalEntity", alias="schema")
-    properties: EntityProperties = Field(..., example={"name": ["John Doe"]})
-    datasets: List[str] = Field([], example=["us_ofac_sdn"])
-    referents: List[str] = Field([], example=["ofac-1234"])
+    id: str = Field(..., examples=["NK-A7z...."])
+    caption: str = Field(..., examples=["John Doe"])
+    schema_: str = Field(..., examples=["LegalEntity"], alias="schema")
+    properties: EntityProperties = Field(..., examples=[{"name": ["John Doe"]}])
+    datasets: List[str] = Field([], examples=[["us_ofac_sdn"]])
+    referents: List[str] = Field([], examples=[["ofac-1234"]])
     target: bool = Field(False)
-    first_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
-    last_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
-    last_change: Optional[datetime] = Field(..., example=datetime.utcnow())
+    first_seen: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
+    last_seen: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
+    last_change: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
 
     @classmethod
     def from_entity(cls, entity: Entity) -> "EntityResponse":
-        return cls.construct(
-            id=entity.id,
-            caption=entity._caption,
-            schema=entity.schema.name,
-            properties=dict(entity.properties),
-            datasets=list(entity.datasets),
-            referents=list(entity.referents),
-            target=entity.target,
-            first_seen=entity.first_seen,
-            last_seen=entity.last_seen,
-            last_change=entity.last_change,
-        )
+        return cls.model_validate(entity.to_dict())
 
 
-EntityResponse.update_forward_refs()
+EntityResponse.model_rebuild()
 
 
 class ScoredEntityResponse(EntityResponse):
     score: float = 0.99
     features: Dict[str, float]
     match: bool = False
 
     @classmethod
     def from_entity_result(
         cls, entity: Entity, result: MatchingResult, threshold: float
     ) -> "ScoredEntityResponse":
-        return cls.construct(
-            id=entity.id,
-            caption=entity._caption,
-            schema=entity.schema.name,
-            properties=entity.properties,
-            datasets=list(entity.datasets),
-            referents=list(entity.referents),
-            target=entity.target,
-            first_seen=entity.first_seen,
-            last_seen=entity.last_seen,
-            last_change=entity.last_change,
-            score=result["score"],
-            match=result["score"] >= threshold,
-            features=result["features"],
-        )
+        data = entity.to_dict()
+        data.update(result)
+        data["match"] = result["score"] >= threshold
+        return cls.model_validate(data)
 
 
 class StatusResponse(BaseModel):
     status: str = "ok"
 
 
 class SearchFacetItem(BaseModel):
-    name: str = Field(..., example="ru")
-    label: str = Field(..., example="Russia")
-    count: int = Field(1, example=42)
+    name: str = Field(..., examples=["ru"])
+    label: str = Field(..., examples=["Russia"])
+    count: int = Field(1, examples=[42])
 
 
 class SearchFacet(BaseModel):
-    label: str = Field(..., example="Countries")
+    label: str = Field(..., examples=["Countries"])
     values: List[SearchFacetItem]
 
 
 class TotalSpec(BaseModel):
-    value: int = Field(..., example=42)
-    relation: str = Field("eq", example="eq")
+    value: int = Field(..., examples=[42])
+    relation: str = Field("eq", examples=["eq"])
 
 
 class ResultsResponse(BaseModel):
-    limit: int = Field(..., example=20)
-    offset: int = Field(0, example=0)
+    limit: int = Field(..., examples=[20])
+    offset: int = Field(0, examples=[0])
     total: TotalSpec
 
 
 class SearchResponse(ResultsResponse):
     results: List[EntityResponse]
     facets: Dict[str, SearchFacet]
 
 
 class EntityExample(BaseModel):
-    id: Optional[str] = Field(None, example="my-entity-id")
-    schema_: str = Field(..., example=settings.BASE_SCHEMA, alias="schema")
+    id: Optional[str] = Field(None, examples=["my-entity-id"])
+    schema_: str = Field(..., examples=[settings.BASE_SCHEMA], alias="schema")
     properties: Dict[str, Union[str, List[str]]] = Field(
-        ..., example={"name": ["John Doe"]}
+        ..., examples=[{"name": ["John Doe"]}]
     )
 
 
 class EntityMatchQuery(BaseModel):
     queries: Dict[str, EntityExample]
 
 
 class EntityMatches(BaseModel):
-    status: int = Field(200, example=200)
+    status: int = Field(200, examples=[200])
     results: List[ScoredEntityResponse]
     total: TotalSpec
     query: EntityExample
 
 
 class EntityMatchResponse(BaseModel):
     responses: Dict[str, EntityMatches]
     matcher: FeatureDocs
-    limit: int = Field(..., example=5)
+    limit: int = Field(..., examples=[5])
 
 
 class DatasetModel(BaseModel):
     name: str
     title: str
-    summary: Optional[str]
-    url: Optional[str]
+    summary: Optional[str] = None
+    url: Optional[str] = None
     load: bool
-    entities_url: Optional[str]
+    entities_url: Optional[str] = None
     version: str
     children: List[str]
 
 
 class DataCatalogModel(BaseModel):
     datasets: List[DatasetModel]
 
 
 class Algorithm(BaseModel):
     name: str
-    description: Optional[str]
+    description: Optional[str] = None
     features: FeatureDocs
 
 
 class AlgorithmResponse(BaseModel):
     algorithms: List[Algorithm]
```

### Comparing `yente-3.5.0/yente/data/dataset.py` & `yente-3.6.0/yente/data/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class Dataset(NKDataset):
     def __init__(self, catalog: DataCatalog["Dataset"], data: Dict[str, Any]):
         name = data["name"]
         norm_name = slugify(name, sep="_")
         if name != norm_name:
             raise ValueError("Invalid dataset name %r (try: %r)" % (name, norm_name))
         super().__init__(catalog, data)
+        self._children.update(data.get("scopes", []))
 
         if self.version is None:
             ts = data.get("last_export", BOOT_TIME)
             self.version = iso_to_version(ts) or "static"
 
         self.load = as_bool(data.get("load"), True)
         self.entities_url = self._get_entities_url(data)
@@ -51,8 +52,10 @@
         return None
 
     def to_dict(self) -> Dict[str, Any]:
         data = super().to_dict()
         data["load"] = self.load
         data["entities_url"] = self.entities_url
         data["namespace"] = self.ns is not None
+        if "children" not in data:
+            data["children"] = [c.name for c in self.children]
         return data
```

### Comparing `yente-3.5.0/yente/data/entity.py` & `yente-3.6.0/yente/data/entity.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/data/freebase.py` & `yente-3.6.0/yente/data/freebase.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 from followthemoney.property import Property
 
 from yente import settings
 from yente.data.common import ScoredEntityResponse
 
 
 class FreebaseType(BaseModel):
-    id: str = Field(..., example="Person")
-    name: str = Field(..., example="People")
-    description: Optional[str] = Field(None, example="...")
+    id: str = Field(..., examples=["Person"])
+    name: str = Field(..., examples=["People"])
+    description: Optional[str] = None
 
     @classmethod
     def from_schema(cls, schema: Schema) -> "FreebaseType":
         desc = schema.description or schema.label
         return cls(id=schema.name, name=schema.plural, description=desc)
 
 
 class FreebaseProperty(BaseModel):
-    id: str = Field(..., example="birthDate")
-    name: str = Field(..., example="Date of birth")
-    description: Optional[str] = Field(None, example="...")
+    id: str = Field(..., examples=["birthDate"])
+    name: str = Field(..., examples=["Date of birth"])
+    description: Optional[str] = None
 
     @classmethod
     def from_prop(cls, prop: Property) -> "FreebaseProperty":
         return cls(id=prop.qname, name=prop.label, description=prop.description)
 
 
 class FreebaseEntity(BaseModel):
-    id: str = Field(..., example="NK-A7z....")
-    name: str = Field(..., example="John Doe")
-    description: Optional[str] = Field(None, example="...")
+    id: str = Field(..., examples=["NK-A7z...."])
+    name: str = Field(..., examples=["John Doe"])
+    description: Optional[str] = None
     type: List[FreebaseType]
 
     @classmethod
     def from_proxy(cls, proxy: EntityProxy) -> "FreebaseEntity":
         type_ = [FreebaseType.from_schema(proxy.schema)]
         return FreebaseEntity(
             id=proxy.id,
             name=proxy.caption,
             type=type_,
             description=proxy.schema.label,
         )
 
 
 class FreebaseScoredEntity(FreebaseEntity):
-    score: Optional[float] = Field(..., example=0.99)
-    match: Optional[bool] = Field(..., example=False)
+    score: Optional[float] = Field(..., examples=[0.99])
+    match: Optional[bool] = Field(..., examples=[False])
 
     @classmethod
     def from_scored(cls, data: ScoredEntityResponse) -> "FreebaseScoredEntity":
         schema = model.get(data.schema_)
         if schema is None:
             raise RuntimeError("Missing schema: %s" % data.schema_)
         return cls(
@@ -85,19 +85,19 @@
 
 
 class FreebasePropertySuggestResponse(FreebaseSuggestResponse):
     result: List[FreebaseProperty]
 
 
 class FreebaseManifestView(BaseModel):
-    url: str
+    url: AnyHttpUrl
 
 
 class FreebaseManifestPreview(BaseModel):
-    url: str
+    url: AnyHttpUrl
     width: int
     height: int
 
 
 class FreebaseManifestSuggestType(BaseModel):
     service_url: AnyHttpUrl
     service_path: str
@@ -106,16 +106,16 @@
 class FreebaseManifestSuggest(BaseModel):
     entity: FreebaseManifestSuggestType
     type: FreebaseManifestSuggestType
     property: FreebaseManifestSuggestType
 
 
 class FreebaseManifest(BaseModel):
-    versions: List[str] = Field(..., example=["0.2"])
-    name: str = Field(..., example=settings.TITLE)
+    versions: List[str] = Field(..., examples=[["0.2"]])
+    name: str = Field(..., examples=[settings.TITLE])
     identifierSpace: AnyHttpUrl
     schemaSpace: AnyHttpUrl
     view: FreebaseManifestView
     preview: FreebaseManifestPreview
     suggest: FreebaseManifestSuggest
     defaultTypes: List[FreebaseType]
```

### Comparing `yente-3.5.0/yente/data/loader.py` & `yente-3.6.0/yente/data/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,39 @@
 
 BUFFER = 10 * 1024 * 1024
 
 log = get_logger(__name__)
 
 
 async def load_yaml_url(url: str) -> Any:
+    if url.lower().endswith(".json"):
+        return await load_json_url(url)
     url_ = resolve_url_type(url)
     if isinstance(url_, Path):
         async with aiofiles.open(url_, "r") as fh:
             data = await fh.read()
     else:
         async with http_session() as client:
             async with client.get(url) as resp:
                 data = await resp.text()
     return yaml.safe_load(data)
 
 
+async def load_json_url(url: str) -> Any:
+    url_ = resolve_url_type(url)
+    if isinstance(url_, Path):
+        async with aiofiles.open(url_, "rb") as fh:
+            data = await fh.read()
+    else:
+        async with http_session() as client:
+            async with client.get(url) as resp:
+                data = await resp.read()
+    return orjson.loads(data)
+
+
 async def fetch_url_to_path(url: str, path: Path) -> None:
     async with http_session() as client:
         async with client.get(url) as resp:
             resp.raise_for_status()
             async with aiofiles.open(path, "wb") as outfh:
                 async for chunk in resp.content.iter_chunked(BUFFER):
                     await outfh.write(chunk)
```

### Comparing `yente-3.5.0/yente/data/manifest.py` & `yente-3.6.0/yente/data/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
         if self.scope is not None:
             self.scopes.append(self.scope)
 
         for ds in data["datasets"]:
             if self.scope is not None:
                 ds["load"] = ds["name"] in self.scopes
             if self.namespace is not None:
-                ds["namesapce"] = self.namespace
+                ds["namespace"] = self.namespace
             if self.resource_name is not None:
                 ds["resource_name"] = self.resource_name
             if self.resource_type is not None:
                 ds["resource_type"] = self.resource_type
             manifest.datasets.append(ds)
 
 
 class Manifest(BaseModel):
     catalogs: List[CatalogManifest] = []
     datasets: List[Dict[str, Any]] = []
 
     @classmethod
     async def load(cls) -> "Manifest":
         data = await load_yaml_url(settings.MANIFEST)
-        manifest = cls.parse_obj(data)
+        manifest = cls.model_validate(data)
         for catalog in manifest.catalogs:
             await catalog.fetch(manifest)
         # TODO: load remote metadata from a `metadata_url` on each dataset?
         return manifest
 
 
 class Catalog(DataCatalog[Dataset]):
```

### Comparing `yente-3.5.0/yente/data/util.py` & `yente-3.6.0/yente/data/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,19 @@
     raise RuntimeError("Cannot open resource: %s" % url)
 
 
 @asynccontextmanager
 async def http_session() -> AsyncGenerator[ClientSession, None]:
     timeout = ClientTimeout(
         total=84600,
-        connect=None,
+        connect=30,
         sock_connect=None,
         sock_read=None,
     )
     connector = TCPConnector(limit=10)
     async with ClientSession(
-        timeout=timeout, trust_env=True, connector=connector
+        timeout=timeout,
+        trust_env=True,
+        connector=connector,
+        read_bufsize=10 * 1024 * 1024,
     ) as client:
         yield client
```

### Comparing `yente-3.5.0/yente/logs.py` & `yente-3.6.0/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/resources/favicon.ico` & `yente-3.6.0/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/routers/admin.py` & `yente-3.6.0/yente/routers/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,24 +85,25 @@
 async def catalog() -> DataCatalogModel:
     """Return the service manifest, which includes a list of all indexed datasets.
 
     The manifest is the configuration file of the yente service. It specifies what
     data sources are included, and how often they should be loaded.
     """
     catalog = await get_catalog()
-    return DataCatalogModel.parse_obj(catalog.to_dict())
+    return DataCatalogModel.model_validate(catalog.to_dict())
 
 
 @router.get(
     "/algorithms",
     tags=["System information"],
     response_model=AlgorithmResponse,
 )
 async def algorithms() -> AlgorithmResponse:
-    """Return a list of the supported matching/scoring algorithms used by the matching endpoing.
+    """Return a list of the supported matching/scoring algorithms used by the matching
+    endpoint.
 
     See also the [scoring documentation](https://www.opensanctions.org/docs/api/scoring/)."""
     algorithms: List[Algorithm] = []
     for algo in ALGORITHMS:
         desc = Algorithm(
             name=algo.NAME,
             description=collapse_spaces(algo.__doc__),
```

### Comparing `yente-3.5.0/yente/routers/match.py` & `yente-3.6.0/yente/routers/match.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,24 @@
         settings.SCORE_CUTOFF,
         title="Lower bound of score for results to be returned at all",
     ),
     algorithm: str = Query(
         settings.DEFAULT_ALGORITHM,
         title=f"Scoring algorithm to use, options: {ALGO_LIST}",
     ),
+    fuzzy: bool = Query(
+        settings.MATCH_FUZZY,
+        title="Use slow matching for candidate generation, does not affect scores",
+    ),
 ) -> EntityMatchResponse:
     """Match entities based on a complex set of criteria, like name, date of birth
     and nationality of a person. This works by submitting a batch of entities, each
     formatted like those returned by the API.
 
-    Tutorial: [Using the matching API to do KYC-style checks](https://www.opensanctions.org/docs/api/matching/).
+    Tutorial: [Using the matching API](https://www.opensanctions.org/docs/api/matching/).
 
     For example, the following would be valid query examples:
 
     ```json
     "queries": {
         "entity1": {
             "schema": "Person",
@@ -120,15 +124,15 @@
     queries = []
     entities = []
     responses: Dict[str, EntityMatches] = {}
 
     for name, example in match.queries.items():
         try:
             entity = Entity.from_example(example)
-            query = entity_query(ds, entity)
+            query = entity_query(ds, entity, fuzzy=fuzzy)
         except Exception as exc:
             log.info("Cannot parse example entity: %s" % str(exc))
             raise HTTPException(
                 status_code=400,
                 detail=f"Cannot parse example entity: {exc}",
             )
         queries.append(search_entities(query, limit=limit * 10))
@@ -154,15 +158,15 @@
             schema=entity.schema.name,
             results=total.value,
         )
         responses[name] = EntityMatches(
             status=200,
             results=scored,
             total=total,
-            query=EntityExample.parse_obj(entity.to_dict()),
+            query=EntityExample.model_validate(entity.to_dict()),
         )
     response.headers["x-batch-size"] = str(len(responses))
     return EntityMatchResponse(
         responses=responses,
         matcher=algorithm_type.explain(),
         limit=limit,
     )
```

### Comparing `yente-3.5.0/yente/routers/reconcile.py` & `yente-3.6.0/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/routers/search.py` & `yente-3.6.0/yente/routers/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 async def search(
     response: Response,
     q: str = Query("", title="Query text"),
     dataset: str = PATH_DATASET,
     schema: str = Query(
         settings.BASE_SCHEMA, title="Types of entities that can match the search"
     ),
+    exclude_schema: List[str] = Query(
+        [], title="Remove the given types of entities from results"
+    ),
     countries: List[str] = Query([], title="Filter by country codes"),
     topics: List[str] = Query(
         [], title="Filter by entity topics (e.g. sanction, role.pep)"
     ),
     datasets: List[str] = Query([], title="Filter by data sources"),
     limit: int = Query(10, title="Number of results to return", le=settings.MAX_PAGE),
     offset: int = Query(
@@ -53,31 +56,39 @@
     fuzzy: bool = Query(False, title="Allow fuzzy query syntax"),
     simple: bool = Query(False, title="Use simple syntax for user-facing query boxes"),
 ) -> SearchResponse:
     """Search endpoint for matching entities based on a simple piece of text, e.g.
     a name. This can be used to implement a simple, user-facing search. For proper
     entity matching, the multi-property matching API should be used instead.
 
-    Search queries can use the [ElasticSearch Query string syntax](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-query-string-query.html#query-string-syntax)
-    to perform field-specific searches, wildcard and fuzzy searches.
+    Search queries can include field-specific fitlers, wildcards and fuzzy searches.
+    See also: [search API documentation](https://www.opensanctions.org/docs/api/search/).
     """
     limit, offset = limit_window(limit, offset, 10)
     ds = await get_dataset(dataset)
     catalog = await get_catalog()
     schema_obj = model.get(schema)
     if schema_obj is None:
         raise HTTPException(400, detail="Invalid schema")
     filters: FilterDict = {
         "countries": countries,
         "topics": topics,
         "datasets": datasets,
     }
     if target is not None:
         filters["target"] = target
-    query = text_query(ds, schema_obj, q, filters=filters, fuzzy=fuzzy, simple=simple)
+    query = text_query(
+        ds,
+        schema_obj,
+        q,
+        filters=filters,
+        fuzzy=fuzzy,
+        simple=simple,
+        exclude_schema=exclude_schema,
+    )
     aggregations = facet_aggregations([f for f in filters.keys()])
     resp = await search_entities(
         query,
         limit=limit,
         offset=offset,
         aggregations=aggregations,
         sort=parse_sorts(sort),
@@ -111,18 +122,20 @@
         307: {"description": "The entity was merged into another ID"},
         404: {"model": ErrorResponse, "description": "Entity not found"},
         500: {"model": ErrorResponse, "description": "Server error"},
     },
 )
 async def fetch_entity(
     response: Response,
-    entity_id: str = Path(description="ID of the entity to retrieve", example="Q7747"),
+    entity_id: str = Path(
+        description="ID of the entity to retrieve", examples=["Q7747"]
+    ),
     nested: bool = Query(
         True,
-        title="Include adjacent entities (e.g. addresses, family, subsidiaries) in response",
+        title="Include adjacent entities (e.g. addresses, family) in response",
     ),
 ) -> Union[RedirectResponse, EntityResponse]:
     """Retrieve a single entity by its ID. The entity will be returned in
     full, with data from all datasets and with nested entities (adjacent
     passport, sanction and associated entities) included. If the entity ID
     has been merged into a different canonical entity, an HTTP redirect will
     be triggered.
```

### Comparing `yente-3.5.0/yente/routers/util.py` & `yente-3.6.0/yente/routers/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from yente.data.dataset import Dataset
 from yente.data import get_catalog
 
 
 PATH_DATASET = Path(
     description="Data source or collection name to be queries",
-    example="default",
+    examples=["default"],
 )
 QUERY_PREFIX = Query("", min_length=1, description="Search prefix")
 
 
 async def get_dataset(name: str) -> Dataset:
     catalog = await get_catalog()
     dataset = catalog.get(name)
```

### Comparing `yente-3.5.0/yente/scoring.py` & `yente-3.6.0/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/search/base.py` & `yente-3.6.0/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/search/indexer.py` & `yente-3.6.0/yente/search/indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import threading
 from normality import WS
 from typing import Any, AsyncGenerator, Dict, List
 from elasticsearch import AsyncElasticsearch
 from elasticsearch.helpers import async_bulk, BulkIndexError
 from elasticsearch.exceptions import BadRequestError
 from followthemoney import model
+from followthemoney.exc import FollowTheMoneyException
 from followthemoney.types.date import DateType
 from followthemoney.types.name import NameType
 from nomenklatura.util import fingerprint_name
 
 from yente import settings
 from yente.logs import get_logger
 from yente.data.entity import Entity
@@ -33,51 +34,54 @@
     datasets = set(dataset.dataset_names)
     idx = 0
     async for data in load_json_lines(dataset.entities_url, index):
         if idx % 1000 == 0 and idx > 0:
             log.info("Index: %d entities..." % idx, index=index)
         idx += 1
 
-        entity = Entity.from_dict(model, data)
-        entity.datasets = entity.datasets.intersection(datasets)
-        if not len(entity.datasets):
-            entity.datasets.add(dataset.name)
-        if dataset.ns is not None:
-            entity = dataset.ns.apply(entity)
-
-        texts = entity.pop("indexText")
-        doc = entity.to_full_dict(matchable=True)
-        doc["text"] = texts
-        names = doc.pop(NameType.group, [])
-        expanded_names = set(names)
-        name_parts = set()
-        for name in names:
-            fp = fingerprint_name(name)
-            if fp is not None:
-                expanded_names.add(fp)
-                name_parts.update(fp.split(WS))
-        doc[NAMES_FIELD] = list(expanded_names)
-        doc[NAME_PART_FIELD] = list(name_parts)
-        doc[SOUNDEX_FIELD] = soundex_names(names)
-        doc[DateType.group] = expand_dates(doc.pop(DateType.group, []))
-        entity_id = doc.pop("id")
-        yield {"_index": index, "_id": entity_id, "_source": doc}
+        try:
+            entity = Entity.from_dict(model, data)
+            entity.datasets = entity.datasets.intersection(datasets)
+            if not len(entity.datasets):
+                entity.datasets.add(dataset.name)
+            if dataset.ns is not None:
+                entity = dataset.ns.apply(entity)
+
+            texts = entity.pop("indexText")
+            doc = entity.to_full_dict(matchable=True)
+            doc["text"] = texts
+            names = doc.pop(NameType.group, [])
+            expanded_names = set(names)
+            name_parts = set()
+            for name in names:
+                fp = fingerprint_name(name)
+                if fp is not None:
+                    expanded_names.add(fp)
+                    name_parts.update(fp.split(WS))
+            doc[NAMES_FIELD] = list(expanded_names)
+            doc[NAME_PART_FIELD] = list(name_parts)
+            doc[SOUNDEX_FIELD] = soundex_names(names)
+            doc[DateType.group] = expand_dates(doc.pop(DateType.group, []))
+            entity_id = doc.pop("id")
+            yield {"_index": index, "_id": entity_id, "_source": doc}
+        except FollowTheMoneyException as exc:
+            log.warning("Invalid entity: %s" % exc, data=data)
 
 
 async def index_entities_rate_limit(
     es: AsyncElasticsearch, dataset: Dataset, force: bool
 ) -> bool:
     async with index_semaphore:
         return await index_entities(es, dataset, force=force)
 
 
 async def index_entities(es: AsyncElasticsearch, dataset: Dataset, force: bool) -> bool:
     """Index entities in a particular dataset, with versioning of the index."""
     if not dataset.load:
-        log.debug("Dataset is not loadable", dataset=dataset.name)
+        log.debug("Dataset is going to be loaded", dataset=dataset.name)
         return False
     if dataset.entities_url is None:
         log.warning("Cannot identify resource with FtM entities", dataset=dataset.name)
         return False
 
     # Versioning defaults to the software version instead of a data update date:
     version = f"{settings.INDEX_VERSION}{dataset.version}"
@@ -117,18 +121,22 @@
         BulkIndexError,
         KeyboardInterrupt,
         OSError,
         Exception,
         asyncio.TimeoutError,
         asyncio.CancelledError,
     ) as exc:
+        errors = None
+        if hasattr(exc, "errors"):
+            errors = exc.errors
         log.exception(
             "Indexing error: %r" % exc,
             dataset=dataset.name,
             index=next_index,
+            errors=errors,
             entities_url=dataset.entities_url,
         )
         await es.indices.delete(index=next_index)
         return False
 
     await es.indices.refresh(index=next_index)
     res = await es.indices.put_alias(index=next_index, name=settings.ENTITY_INDEX)
```

### Comparing `yente-3.5.0/yente/search/mapping.py` & `yente-3.6.0/yente/search/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from followthemoney.types.common import PropertyType
 from followthemoney.types.name import NameType
 
 from yente import settings
 
 MappingProperty = Dict[str, Union[List[str], str]]
 
-DATE_FORMAT = "yyyy-MM-dd'T'HH||yyyy-MM-dd'T'HH:mm||yyyy-MM-dd'T'HH:mm:ss||yyyy-MM-dd||yyyy-MM||yyyy||strict_date_optional_time"
+DATE_FORMAT = "yyyy-MM-dd'T'HH||yyyy-MM-dd'T'HH:mm||yyyy-MM-dd'T'HH:mm:ss||yyyy-MM-dd||yyyy-MM||yyyy||strict_date_optional_time"  # noqa
 TEXT_TYPES = (registry.name, registry.address)
 INDEX_SETTINGS = {
     "analysis": {
         "normalizer": {
             "osa-normalizer": {
                 "type": "custom",
                 "filter": ["lowercase", "asciifolding"],
```

### Comparing `yente-3.5.0/yente/search/nested.py` & `yente-3.6.0/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente/search/queries.py` & `yente-3.6.0/yente/search/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from followthemoney.proxy import EntityProxy
 from followthemoney.types import registry
 from nomenklatura.util import name_words
 
 from yente.logs import get_logger
 from yente.data.dataset import Dataset
 from yente.data.util import pick_names, soundex_names
-from yente.search.mapping import TEXT_TYPES, NAMES_FIELD, SOUNDEX_FIELD, NAME_PART_FIELD
+from yente.search.mapping import NAMES_FIELD, SOUNDEX_FIELD, NAME_PART_FIELD
 
 log = get_logger(__name__)
 FilterDict = Dict[str, Union[bool, str, List[str]]]
 Clause = Dict[str, Any]
 
 
 def filter_query(
     shoulds: List[Clause],
     dataset: Optional[Dataset] = None,
     schema: Optional[Schema] = None,
     filters: FilterDict = {},
+    exclude_schema: List[str] = [],
 ) -> Clause:
     filterqs: List[Clause] = []
     if dataset is not None:
         filterqs.append({"terms": {"datasets": dataset.dataset_names}})
     if schema is not None:
         schemata = schema.matchable_schemata
         schemata.add(schema)
@@ -33,61 +34,74 @@
     for field, values in filters.items():
         if isinstance(values, (bool, str)):
             filterqs.append({"term": {field: {"value": values}}})
             continue
         values = [v for v in values if len(v)]
         if len(values):
             filterqs.append({"terms": {field: values}})
-    return {"bool": {"filter": filterqs, "should": shoulds, "minimum_should_match": 1}}
+    must_not: List[Clause] = []
+    for schema_name in exclude_schema:
+        must_not.append({"term": {"schema": schema_name}})
+    return {
+        "bool": {
+            "filter": filterqs,
+            "must_not": must_not,
+            "should": shoulds,
+            "minimum_should_match": 1,
+        }
+    }
 
 
-def names_query(entity: EntityProxy) -> List[Clause]:
+def names_query(entity: EntityProxy, fuzzy: bool = True) -> List[Clause]:
     names = entity.get_type_values(registry.name, matchable=True)
     shoulds = []
     for name in pick_names(names, limit=5):
         match = {
             NAMES_FIELD: {
                 "query": name,
-                "fuzziness": "AUTO",
                 "minimum_should_match": "70%",
+                "fuzziness": 0,
                 "boost": 3.0,
             }
         }
+        if fuzzy:
+            match[NAMES_FIELD]["fuzziness"] = "AUTO"
         shoulds.append({"match": match})
     for token in name_words(names):
         shoulds.append({"term": {NAME_PART_FIELD: {"value": token}}})
     for phoneme in soundex_names(names):
         shoulds.append({"term": {SOUNDEX_FIELD: {"value": phoneme}}})
     return shoulds
 
 
-def entity_query(dataset: Dataset, entity: EntityProxy) -> Clause:
+def entity_query(dataset: Dataset, entity: EntityProxy, fuzzy: bool = True) -> Clause:
     shoulds: List[Clause] = []
     for prop, value in entity.itervalues():
         if prop.type == registry.name or not prop.matchable:
             continue
-        if prop.type in TEXT_TYPES:
-            query = {"match": {prop.type.group: {"query": value}}}
+        if prop.type == registry.address:
+            query = {"match": {prop.type.group: value}}
             shoulds.append(query)
         elif prop.type.group is not None:
             shoulds.append({"term": {prop.type.group: value}})
-        else:
-            shoulds.append({"match_phrase": {"text": value}})
+        elif fuzzy:
+            shoulds.append({"match": {"text": value}})
 
-    shoulds.extend(names_query(entity))
+    shoulds.extend(names_query(entity, fuzzy=fuzzy))
     return filter_query(shoulds, dataset=dataset, schema=entity.schema)
 
 
 def text_query(
     dataset: Dataset,
     schema: Schema,
     query: str,
     filters: FilterDict = {},
     fuzzy: bool = False,
     simple: bool = False,
+    exclude_schema: List[str] = [],
 ) -> Clause:
     if not len(query.strip()):
         should: Clause = {"match_all": {}}
     elif simple:
         should = {
             "simple_query_string": {
                 "query": query,
@@ -105,15 +119,21 @@
                 "default_operator": "AND",
                 "fuzziness": "AUTO" if fuzzy else 0,
                 "analyzer": "osa-analyzer",
                 "lenient": True,
             }
         }
         # log.info("Query", should=should)
-    return filter_query([should], dataset=dataset, schema=schema, filters=filters)
+    return filter_query(
+        [should],
+        dataset=dataset,
+        schema=schema,
+        filters=filters,
+        exclude_schema=exclude_schema,
+    )
 
 
 def prefix_query(
     dataset: Dataset,
     prefix: str,
 ) -> Clause:
     if not len(prefix.strip()):
```

### Comparing `yente-3.5.0/yente/search/search.py` & `yente-3.6.0/yente/search/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Generator, Set, Union
+from typing import Generator, Set
 from typing import Any, Dict, List, Optional
 from elasticsearch import TransportError, ApiError
 from elasticsearch.exceptions import NotFoundError
 from elastic_transport import ObjectApiResponse
 from fastapi import HTTPException
 from followthemoney import model
 from followthemoney.schema import Schema
@@ -50,24 +50,32 @@
     facets: Dict[str, SearchFacet] = {}
     aggs: Dict[str, Dict[str, Any]] = response.get("aggregations", {})
     for field, agg in aggs.items():
         facet = SearchFacet(label=field, values=[])
         buckets: List[Dict[str, Any]] = agg.get("buckets", [])
         for bucket in buckets:
             key: Optional[str] = bucket.get("key")
+            if key is not None:
+                key = str(key)
             count: Optional[int] = bucket.get("doc_count")
             if key is None or count is None:
                 continue
             value = SearchFacetItem(name=key, label=key, count=count)
             if field == "datasets":
                 facet.label = "Data sources"
                 value.label = key
                 ds = catalog.get(key)
                 if ds is not None:
                     value.label = ds.title or key
+            if field == "schema":
+                facet.label = "Entity types"
+                value.label = key
+                schema_obj = model.get(key)
+                if schema_obj is not None:
+                    value.label = schema_obj.plural
             if field in registry.groups:
                 type_ = registry.groups[field]
                 facet.label = type_.plural
                 value.label = type_.caption(key) or value.label
             facet.values.append(value)
         facets[field] = facet
     return facets
```

### Comparing `yente-3.5.0/yente/settings.py` & `yente-3.6.0/yente/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.5.0"
+VERSION = "3.6.0"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
@@ -109,14 +109,15 @@
 }
 MAX_PAGE = 500
 MAX_BATCH = int(env_str("YENTE_MAX_BATCH") or "100")
 MAX_RESULTS = 9999
 MAX_OFFSET = MAX_RESULTS - MAX_PAGE
 MAX_MATCHES = 10
 MATCH_PAGE = int(env_str("YENTE_MATCH_PAGE") or "5")
+MATCH_FUZZY = as_bool(env_str("YENTE_MATCH_FUZZY") or "true")
 QUERY_CONCURRENCY = int(env_str("YENTE_QUERY_CONCURRENCY") or "10")
 INDEX_CONCURRENCY = int(env_str("YENTE_INDEX_CONCURRENCY") or "5")
 
 SCORE_THRESHOLD = 0.70
 SCORE_CUTOFF = 0.10
 
 # ElasticSearch settings:
@@ -124,14 +125,14 @@
 ES_USERNAME = env_str("YENTE_ELASTICSEARCH_USERNAME")
 ES_PASSWORD = env_str("YENTE_ELASTICSEARCH_PASSWORD")
 ES_CLOUD_ID = env_str("YENTE_ELASTICSEARCH_CLOUD_ID")
 ES_SNIFF = as_bool(env_str("YENTE_ELASTICSEARCH_SNIFF") or "false")
 ES_INDEX = env_str("YENTE_ELASTICSEARCH_INDEX", "yente")
 ES_SHARDS = int(env_str("YENTE_ELASTICSEARCH_SHARDS") or "1")
 ENTITY_INDEX = f"{ES_INDEX}-entities"
-INDEX_VERSION = "004"
+INDEX_VERSION = env_str("YENTE_INDEX_VERSION", "005")
 
 LOG_JSON = as_bool(env_str("YENTE_LOG_JSON", "false"))
 LOG_LEVEL = logging.DEBUG if DEBUG else logging.INFO
 
 # Used to pad out first_seen, last_seen on static collections
 RUN_TIME = datetime.utcnow().isoformat()[:19]
```

### Comparing `yente-3.5.0/yente/util.py` & `yente-3.6.0/yente/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any, Optional, Tuple, cast
+from typing import Any, Optional, Tuple
 from pydantic import AnyHttpUrl
-from pydantic.tools import parse_obj_as
+from pydantic.type_adapter import TypeAdapter
 
 from yente import settings
 
 
 class EntityRedirect(Exception):
     def __init__(self, canonical_id: str) -> None:
         self.canonical_id = canonical_id
 
 
 def typed_url(url: Any) -> AnyHttpUrl:
-    return cast(AnyHttpUrl, parse_obj_as(AnyHttpUrl, url))
+    return TypeAdapter(AnyHttpUrl).validate_python(url)
 
 
 def match_prefix(prefix: str, *labels: Optional[str]) -> bool:
     prefix = prefix.lower().strip()
     if not len(prefix):
         return False
     for label in labels:
```

### Comparing `yente-3.5.0/yente.egg-info/PKG-INFO` & `yente-3.6.0/yente.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.5.0
+Version: 3.6.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.5.0/yente.egg-info/SOURCES.txt` & `yente-3.6.0/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.5.0/yente.egg-info/requires.txt` & `yente-3.6.0/yente.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-followthemoney==3.4.3
-nomenklatura==3.1.0
+followthemoney==3.5.1
+nomenklatura==3.3.4
 asyncstdlib==3.10.8
 aiocron==1.8
 aiocsv==1.2.4
 aiofiles==23.1.0
-types-aiofiles==23.1.0.4
-aiohttp[speedups]==3.8.4
-elasticsearch[async]==8.8.0
-fastapi==0.99.1
-uvicorn[standard]==0.22.0
+types-aiofiles<23.2,>=23.1.0.4
+aiohttp[speedups]==3.8.5
+elasticsearch[async]==8.8.2
+fastapi==0.100.0
+uvicorn[standard]==0.23.1
 python-multipart==0.0.6
 email-validator==2.0.0.post2
 structlog==23.1.0
 pyicu==2.11
 jellyfish==1.0.0
-orjson==3.9.1
+orjson==3.9.2
 text-unidecode==1.3
-click==8.0.4
+click==8.1.6
 normality==2.4.0
 languagecodes==1.1.1
-countrynames==1.15.0
+countrynames==1.15.1
 fingerprints==1.1.0
-pantomime==0.6.0
+pantomime==0.6.1
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
 twine
 mypy
```

