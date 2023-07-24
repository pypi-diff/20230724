# Comparing `tmp/aio_openapi-3.2.0.tar.gz` & `tmp/aio_openapi-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_openapi-3.2.0.tar", max compression
+gzip compressed data, was "aio_openapi-3.2.1.tar", max compression
```

## Comparing `aio_openapi-3.2.0.tar` & `aio_openapi-3.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1461 2023-04-01 12:22:51.141044 aio_openapi-3.2.0/LICENSE
--rw-r--r--   0        0        0       76 2023-04-01 12:22:51.141044 aio_openapi-3.2.0/openapi/__init__.py
--rw-r--r--   0        0        0     4647 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/cli.py
--rw-r--r--   0        0        0        0 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/__init__.py
--rw-r--r--   0        0        0     6271 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/db.py
--rw-r--r--   0        0        0     2116 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/dump.py
--rw-r--r--   0        0        0      704 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/exc.py
--rw-r--r--   0        0        0    15576 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/fields.py
--rw-r--r--   0        0        0     8736 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/validate.py
--rw-r--r--   0        0        0     3730 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/data/view.py
--rw-r--r--   0        0        0     1204 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/__init__.py
--rw-r--r--   0        0        0      406 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/columns.py
--rw-r--r--   0        0        0     4185 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/commands.py
--rw-r--r--   0        0        0     4549 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/container.py
--rw-r--r--   0        0        0    13697 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/dbmodel.py
--rw-r--r--   0        0        0     2292 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/migrations.py
--rw-r--r--   0        0        0       97 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/openapi/alembic.ini.mako
--rw-r--r--   0        0        0     4124 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/openapi/env.py
--rw-r--r--   0        0        0      948 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/openapi/script.py.mako
--rw-r--r--   0        0        0     9364 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/db/path.py
--rw-r--r--   0        0        0      609 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/exc.py
--rw-r--r--   0        0        0      583 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/json.py
--rw-r--r--   0        0        0     1207 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/logger.py
--rw-r--r--   0        0        0     1518 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/middleware.py
--rw-r--r--   0        0        0      480 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/__init__.py
--rw-r--r--   0        0        0      617 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/create.py
--rw-r--r--   0        0        0     5629 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/cursor.py
--rw-r--r--   0        0        0     3881 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/offset.py
--rw-r--r--   0        0        0     3469 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/pagination.py
--rw-r--r--   0        0        0     1505 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/pagination/search.py
--rw-r--r--   0        0        0        0 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/py.typed
--rw-r--r--   0        0        0     1081 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/rest.py
--rw-r--r--   0        0        0      578 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/sentry.py
--rw-r--r--   0        0        0      293 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/__init__.py
--rw-r--r--   0        0        0      162 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/hdrs.py
--rw-r--r--   0        0        0     1006 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/operation.py
--rw-r--r--   0        0        0     4320 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/path.py
--rw-r--r--   0        0        0     1625 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/redoc.py
--rw-r--r--   0        0        0      633 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/server.py
--rw-r--r--   0        0        0    17113 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/spec.py
--rw-r--r--   0        0        0     2098 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/spec/utils.py
--rw-r--r--   0        0        0     2070 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/testing.py
--rw-r--r--   0        0        0      502 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/types.py
--rw-r--r--   0        0        0      194 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/tz.py
--rw-r--r--   0        0        0     4751 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/utils.py
--rw-r--r--   0        0        0      608 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/__init__.py
--rw-r--r--   0        0        0     3747 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/channel.py
--rw-r--r--   0        0        0     3468 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/channels.py
--rw-r--r--   0        0        0      549 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/errors.py
--rw-r--r--   0        0        0     2623 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/manager.py
--rw-r--r--   0        0        0     4263 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/path.py
--rw-r--r--   0        0        0     3486 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/pubsub.py
--rw-r--r--   0        0        0      737 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/rpc.py
--rw-r--r--   0        0        0      680 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/openapi/ws/utils.py
--rw-r--r--   0        0        0     3142 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1384 2023-04-01 12:22:51.145044 aio_openapi-3.2.0/readme.md
--rw-r--r--   0        0        0     4321 1970-01-01 00:00:00.000000 aio_openapi-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-24 10:23:21.959241 aio_openapi-3.2.1/LICENSE
+-rw-r--r--   0        0        0       76 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/__init__.py
+-rw-r--r--   0        0        0     4647 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/cli.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/__init__.py
+-rw-r--r--   0        0        0     6271 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/db.py
+-rw-r--r--   0        0        0     2116 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/dump.py
+-rw-r--r--   0        0        0      704 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/exc.py
+-rw-r--r--   0        0        0    15576 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/fields.py
+-rw-r--r--   0        0        0     8736 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/validate.py
+-rw-r--r--   0        0        0     3730 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/data/view.py
+-rw-r--r--   0        0        0     1204 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/__init__.py
+-rw-r--r--   0        0        0      406 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/columns.py
+-rw-r--r--   0        0        0     4185 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/commands.py
+-rw-r--r--   0        0        0     4549 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/container.py
+-rw-r--r--   0        0        0    13697 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/dbmodel.py
+-rw-r--r--   0        0        0     2292 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/migrations.py
+-rw-r--r--   0        0        0       97 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/openapi/alembic.ini.mako
+-rw-r--r--   0        0        0     4124 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/openapi/env.py
+-rw-r--r--   0        0        0      948 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/openapi/script.py.mako
+-rw-r--r--   0        0        0     9364 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/db/path.py
+-rw-r--r--   0        0        0      609 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/exc.py
+-rw-r--r--   0        0        0      583 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/json.py
+-rw-r--r--   0        0        0     1207 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/logger.py
+-rw-r--r--   0        0        0     1518 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/middleware.py
+-rw-r--r--   0        0        0      480 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/create.py
+-rw-r--r--   0        0        0     5629 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/cursor.py
+-rw-r--r--   0        0        0     3881 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/offset.py
+-rw-r--r--   0        0        0     3469 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/pagination.py
+-rw-r--r--   0        0        0     1505 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/pagination/search.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/py.typed
+-rw-r--r--   0        0        0     1081 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/rest.py
+-rw-r--r--   0        0        0      578 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/sentry.py
+-rw-r--r--   0        0        0      293 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/__init__.py
+-rw-r--r--   0        0        0      162 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/hdrs.py
+-rw-r--r--   0        0        0     1006 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/operation.py
+-rw-r--r--   0        0        0     4320 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/path.py
+-rw-r--r--   0        0        0     1625 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/redoc.py
+-rw-r--r--   0        0        0      633 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/server.py
+-rw-r--r--   0        0        0    17113 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/spec.py
+-rw-r--r--   0        0        0     2098 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/spec/utils.py
+-rw-r--r--   0        0        0     2070 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/testing.py
+-rw-r--r--   0        0        0      502 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/types.py
+-rw-r--r--   0        0        0      194 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/tz.py
+-rw-r--r--   0        0        0     4751 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/utils.py
+-rw-r--r--   0        0        0      608 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/__init__.py
+-rw-r--r--   0        0        0     3747 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/channel.py
+-rw-r--r--   0        0        0     3468 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/channels.py
+-rw-r--r--   0        0        0      549 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/errors.py
+-rw-r--r--   0        0        0     2623 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/manager.py
+-rw-r--r--   0        0        0     4263 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/path.py
+-rw-r--r--   0        0        0     3486 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/pubsub.py
+-rw-r--r--   0        0        0      737 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/rpc.py
+-rw-r--r--   0        0        0      680 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/openapi/ws/utils.py
+-rw-r--r--   0        0        0     3376 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-07-24 10:23:21.963242 aio_openapi-3.2.1/readme.md
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 aio_openapi-3.2.1/PKG-INFO
```

### Comparing `aio_openapi-3.2.0/LICENSE` & `aio_openapi-3.2.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Quantmind
+Copyright (c) 2023 Quantmind
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `aio_openapi-3.2.0/openapi/cli.py` & `aio_openapi-3.2.1/openapi/cli.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/db.py` & `aio_openapi-3.2.1/openapi/data/db.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/dump.py` & `aio_openapi-3.2.1/openapi/data/dump.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/exc.py` & `aio_openapi-3.2.1/openapi/data/exc.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/fields.py` & `aio_openapi-3.2.1/openapi/data/fields.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/validate.py` & `aio_openapi-3.2.1/openapi/data/validate.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/data/view.py` & `aio_openapi-3.2.1/openapi/data/view.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/__init__.py` & `aio_openapi-3.2.1/openapi/db/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/commands.py` & `aio_openapi-3.2.1/openapi/db/commands.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/container.py` & `aio_openapi-3.2.1/openapi/db/container.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/dbmodel.py` & `aio_openapi-3.2.1/openapi/db/dbmodel.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/migrations.py` & `aio_openapi-3.2.1/openapi/db/migrations.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/openapi/env.py` & `aio_openapi-3.2.1/openapi/db/openapi/env.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/openapi/script.py.mako` & `aio_openapi-3.2.1/openapi/db/openapi/script.py.mako`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/db/path.py` & `aio_openapi-3.2.1/openapi/db/path.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/exc.py` & `aio_openapi-3.2.1/openapi/exc.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/json.py` & `aio_openapi-3.2.1/openapi/json.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/logger.py` & `aio_openapi-3.2.1/openapi/logger.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/middleware.py` & `aio_openapi-3.2.1/openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/pagination/create.py` & `aio_openapi-3.2.1/openapi/pagination/create.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/pagination/cursor.py` & `aio_openapi-3.2.1/openapi/pagination/cursor.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/pagination/offset.py` & `aio_openapi-3.2.1/openapi/pagination/offset.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/pagination/pagination.py` & `aio_openapi-3.2.1/openapi/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/pagination/search.py` & `aio_openapi-3.2.1/openapi/pagination/search.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/rest.py` & `aio_openapi-3.2.1/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/sentry.py` & `aio_openapi-3.2.1/openapi/sentry.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/operation.py` & `aio_openapi-3.2.1/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/path.py` & `aio_openapi-3.2.1/openapi/spec/path.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/redoc.py` & `aio_openapi-3.2.1/openapi/spec/redoc.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/server.py` & `aio_openapi-3.2.1/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/spec.py` & `aio_openapi-3.2.1/openapi/spec/spec.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/spec/utils.py` & `aio_openapi-3.2.1/openapi/spec/utils.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/testing.py` & `aio_openapi-3.2.1/openapi/testing.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/utils.py` & `aio_openapi-3.2.1/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/__init__.py` & `aio_openapi-3.2.1/openapi/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/channel.py` & `aio_openapi-3.2.1/openapi/ws/channel.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/channels.py` & `aio_openapi-3.2.1/openapi/ws/channels.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/errors.py` & `aio_openapi-3.2.1/openapi/ws/errors.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/manager.py` & `aio_openapi-3.2.1/openapi/ws/manager.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/path.py` & `aio_openapi-3.2.1/openapi/ws/path.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/pubsub.py` & `aio_openapi-3.2.1/openapi/ws/pubsub.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/rpc.py` & `aio_openapi-3.2.1/openapi/ws/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/openapi/ws/utils.py` & `aio_openapi-3.2.1/openapi/ws/utils.py`

 * *Files identical despite different names*

### Comparing `aio_openapi-3.2.0/pyproject.toml` & `aio_openapi-3.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-openapi"
-version = "3.2.0"
+version = "3.2.1"
 description = "Minimal OpenAPI asynchronous server application"
 documentation = "https://aio-openapi.readthedocs.io"
 repository = "https://github.com/quantmind/aio-openapi"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 packages = [
@@ -40,65 +40,95 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 aiohttp = "^3.8.0"
 httptools = "^0.5.0"
 simplejson = "^3.17.2"
 SQLAlchemy = { version="^2.0.8", extras=["asyncio"] }
-SQLAlchemy-Utils = "^0.40.0"
+SQLAlchemy-Utils = "^0.41.1"
 psycopg2-binary = "^2.9.2"
 click = "^8.0.3"
 python-dateutil = "^2.8.2"
 PyYAML = "^6.0"
 email-validator = "^1.2.1"
 alembic = "^1.8.1"
-aiodns = {version = "^3.0.0", optional = true}
-PyJWT = {version = "^2.3.0", optional = true}
-colorlog = {version = "^6.6.0", optional = true}
-phonenumbers = {version = "^8.12.37", optional = true}
-Sphinx = {version = "^6.1.3", optional = true}
-sphinx-copybutton = {version = "^0.5.0", optional = true}
-sphinx-autodoc-typehints = {version = "^1.12.0", optional = true}
-aiohttp-theme = {version = "^0.1.6", optional = true}
-recommonmark = {version = "^0.7.1", optional = true}
 "backports.zoneinfo" = { version = "^0.2.1", python="<3.9" }
-asyncpg = "^0.27.0"
+asyncpg = "^0.28.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-flake8 = "^6.0.0"
 pytest = "^7.1.1"
-flake8-blind-except = "^0.2.0"
-flake8-builtins = "^2.0.0"
-flake8-commas = "^2.1.0"
-codecov = "^2.1.12"
-coverage = "^6.1.2"
-coveralls = "^3.3.1"
 mypy = "^1.1.1"
-sqlalchemy-stubs = "^0.4"
 sentry-sdk = "^1.4.3"
 python-dotenv = "^1.0.0"
 openapi-spec-validator = "^0.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.6.1"
 isort = "^5.10.1"
 types-simplejson = "^3.17.5"
 types-python-dateutil = "^2.8.11"
 factory-boy = "^3.2.1"
 pytest-asyncio = "^0.21.0"
+types-pyyaml = "^6.0.12"
+ruff = "^0.0.280"
+
+[tool.poetry.group.extras]
+optional = true
+
+[tool.poetry.group.extras.dependencies]
+aiodns = {version = "^3.0.0"}
+PyJWT = {version = "^2.3.0"}
+colorlog = {version = "^6.6.0"}
+phonenumbers = {version = "^8.12.37"}
+
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = {version = "^6.1.3"}
+sphinx-copybutton = {version = "^0.5.0"}
+sphinx-autodoc-typehints = {version = "^1.12.0"}
+aiohttp-theme = {version = "^0.1.6"}
+recommonmark = {version = "^0.7.1"}
+
 
 [tool.poetry.extras]
 dev = ["aiodns", "PyJWT", "colorlog", "phonenumbers"]
 docs = [
     "Sphinx",
     "recommonmark",
     "aiohttp-theme",
     "sphinx-copybutton",
     "sphinx-autodoc-typehints",
 ]
 
-[tool.poetry.group.dev.dependencies]
-types-pyyaml = "^6.0.12"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+testpaths = [
+    "tests"
+]
+
+[tool.isort]
+profile = "black"
+
+[tool.ruff]
+select = ["E", "F"]
+line-length = 88
+
+[tool.mypy]
+# strict = true
+disallow_untyped_calls = true
+disallow_untyped_defs = true
+warn_no_return = true
+
+[[tool.mypy.overrides]]
+module = "tests.*"
+disallow_untyped_defs = false
+
+[[tool.mypy.overrides]]
+module = "openapi.db.openapi.*"
+ignore_errors = true
```

### Comparing `aio_openapi-3.2.0/readme.md` & `aio_openapi-3.2.1/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # aio-openapi
 
 [![PyPI version](https://badge.fury.io/py/aio-openapi.svg)](https://badge.fury.io/py/aio-openapi)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-openapi.svg)](https://pypi.org/project/aio-openapi)
 [![Build](https://github.com/quantmind/aio-openapi/workflows/build/badge.svg)](https://github.com/quantmind/aio-openapi/actions?query=workflow%3Abuild)
-[![Coverage Status](https://coveralls.io/repos/github/quantmind/aio-openapi/badge.svg?branch=master)](https://coveralls.io/github/quantmind/aio-openapi?branch=master)
+[![codecov](https://codecov.io/github/quantmind/aio-openapi/branch/main/graph/badge.svg?token=XV2GD946QI)](https://codecov.io/github/quantmind/aio-openapi)
 [![Documentation Status](https://readthedocs.org/projects/aio-openapi/badge/?version=latest)](https://aio-openapi.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://img.shields.io/pypi/dd/aio-openapi.svg)](https://pypi.org/project/aio-openapi/)
 
 Asynchronous web middleware for [aiohttp][] and serving Rest APIs with [OpenAPI][] v 3
 specification and with optional [PostgreSql][] database bindings.
 
 See the [tutorial](https://aio-openapi.readthedocs.io/en/latest/tutorial.html) for a quick introduction.
```

