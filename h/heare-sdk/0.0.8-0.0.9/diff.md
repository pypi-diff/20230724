# Comparing `tmp/heare-sdk-0.0.8.tar.gz` & `tmp/heare-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heare-sdk-0.0.8.tar", last modified: Sun May 15 04:48:30 2022, max compression
+gzip compressed data, was "heare-sdk-0.0.9.tar", last modified: Sun May 15 06:17:22 2022, max compression
```

## Comparing `heare-sdk-0.0.8.tar` & `heare-sdk-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.901660 heare-sdk-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.901660 heare-sdk-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/.github/workflows/publish-to-test-pypy.yml
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.901660 heare-sdk-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.901660 heare-sdk-0.0.8/src/heare/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.901660 heare-sdk-0.0.8/src/heare/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/src/heare/client/events/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/client/events/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/client/events/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/src/heare/logging/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/src/heare/skills/
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/skills/container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/src/heare/skills/intent/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/skills/intent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-05-15 04:48:17.000000 heare-sdk-0.0.8/src/heare/skills/intent/adapt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 04:48:30.905660 heare-sdk-0.0.8/src/heare_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-15 04:48:30.000000 heare-sdk-0.0.8/src/heare_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-05-15 04:48:30.000000 heare-sdk-0.0.8/src/heare_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-15 04:48:30.000000 heare-sdk-0.0.8/src/heare_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-15 04:48:30.000000 heare-sdk-0.0.8/src/heare_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-15 04:48:30.000000 heare-sdk-0.0.8/src/heare_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/.github/workflows/publish-to-test-pypy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.222722 heare-sdk-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.222722 heare-sdk-0.0.9/src/heare/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare/client/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare/client/events/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/client/events/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/client/events/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare/skills/
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/skills/container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare/skills/intent/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/skills/intent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-05-15 06:17:10.000000 heare-sdk-0.0.9/src/heare/skills/intent/adapt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 06:17:22.226722 heare-sdk-0.0.9/src/heare_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-15 06:17:22.000000 heare-sdk-0.0.9/src/heare_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-05-15 06:17:22.000000 heare-sdk-0.0.9/src/heare_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-15 06:17:22.000000 heare-sdk-0.0.9/src/heare_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-15 06:17:22.000000 heare-sdk-0.0.9/src/heare_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-15 06:17:22.000000 heare-sdk-0.0.9/src/heare_sdk.egg-info/top_level.txt
```

### Comparing `heare-sdk-0.0.8/.github/workflows/publish-to-test-pypy.yml` & `heare-sdk-0.0.9/.github/workflows/publish-to-test-pypy.yml`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/LICENSE` & `heare-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/PKG-INFO` & `heare-sdk-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heare-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Software Development Kit for Heare.io applications.
 Home-page: https://github.com/heare-io/heare-sdk
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/heare-io/heare-sdk/issues
 Platform: UNKNOWN
```

### Comparing `heare-sdk-0.0.8/setup.cfg` & `heare-sdk-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/client/events/message.py` & `heare-sdk-0.0.9/src/heare/client/events/message.py`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/client/events/ws.py` & `heare-sdk-0.0.9/src/heare/client/events/ws.py`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/logging/__init__.py` & `heare-sdk-0.0.9/src/heare/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/skills/__init__.py` & `heare-sdk-0.0.9/src/heare/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/skills/container.py` & `heare-sdk-0.0.9/src/heare/skills/container.py`

 * *Files identical despite different names*

### Comparing `heare-sdk-0.0.8/src/heare/skills/intent/adapt.py` & `heare-sdk-0.0.9/src/heare/skills/intent/adapt.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def on_register_entity(self, register_entity_event: Message):
         payload = register_entity_event.data
         self.engine.register_entity(
             entity_type=payload['entity_type'],
             entity_value=payload['entity_value']
         )
 
-        for alias in payload.get('entity_values', []):
+        for alias in payload.get('entity_aliases', []):
             self.engine.register_entity(
                 entity_type=payload['entity_type'],
                 entity_value=alias,
                 alias_of=payload['entity_value']
             )
 
     def on_register_regex(self, register_regex_event: Message):
```

### Comparing `heare-sdk-0.0.8/src/heare_sdk.egg-info/PKG-INFO` & `heare-sdk-0.0.9/src/heare_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heare-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Software Development Kit for Heare.io applications.
 Home-page: https://github.com/heare-io/heare-sdk
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/heare-io/heare-sdk/issues
 Platform: UNKNOWN
```

### Comparing `heare-sdk-0.0.8/src/heare_sdk.egg-info/SOURCES.txt` & `heare-sdk-0.0.9/src/heare_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

