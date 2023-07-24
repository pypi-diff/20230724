# Comparing `tmp/pyconfita-1.0.8.tar.gz` & `tmp/pyconfita-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconfita-1.0.8.tar", last modified: Tue Oct 25 21:42:42 2022, max compression
+gzip compressed data, was "pyconfita-1.0.9.tar", last modified: Tue Oct 25 22:15:53 2022, max compression
```

## Comparing `pyconfita-1.0.8.tar` & `pyconfita-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.214518 pyconfita-1.0.8/
--rw-r--r--   0 marc       (501) staff       (20)      870 2022-10-25 21:39:56.000000 pyconfita-1.0.8/CHANGELOG.md
--rw-r--r--   0 marc       (501) staff       (20)     1069 2022-10-13 17:53:42.000000 pyconfita-1.0.8/LICENSE
--rw-r--r--   0 marc       (501) staff       (20)       21 2022-10-21 11:01:43.000000 pyconfita-1.0.8/MANIFEST.in
--rw-r--r--   0 marc       (501) staff       (20)     3819 2022-10-25 21:42:42.214102 pyconfita-1.0.8/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)     3470 2022-10-24 08:23:29.000000 pyconfita-1.0.8/README.md
--rw-r--r--   0 marc       (501) staff       (20)       38 2022-10-25 21:42:42.214687 pyconfita-1.0.8/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)     1076 2022-10-25 21:33:31.000000 pyconfita-1.0.8/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.198486 pyconfita-1.0.8/src/
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.204643 pyconfita-1.0.8/src/pyconfita/
--rw-r--r--   0 marc       (501) staff       (20)      388 2022-10-24 08:23:29.000000 pyconfita-1.0.8/src/pyconfita/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.207997 pyconfita-1.0.8/src/pyconfita/backend/
--rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     1776 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/backend.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.209092 pyconfita-1.0.8/src/pyconfita/backend/dict/
--rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/dict/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)      494 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/dict/dict.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.210694 pyconfita-1.0.8/src/pyconfita/backend/environment/
--rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/environment/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)      407 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/environment/environment.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.212159 pyconfita-1.0.8/src/pyconfita/backend/file/
--rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/file/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)      969 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/file/file.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.213131 pyconfita-1.0.8/src/pyconfita/backend/vault/
--rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.8/src/pyconfita/backend/vault/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     9193 2022-10-25 21:36:47.000000 pyconfita-1.0.8/src/pyconfita/backend/vault/vault.py
--rw-r--r--   0 marc       (501) staff       (20)      389 2022-10-24 08:23:29.000000 pyconfita-1.0.8/src/pyconfita/logging_interface.py
--rw-r--r--   0 marc       (501) staff       (20)     2536 2022-10-24 08:23:29.000000 pyconfita-1.0.8/src/pyconfita/pyconfita.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 21:42:42.207246 pyconfita-1.0.8/src/pyconfita.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)     3819 2022-10-25 21:42:42.000000 pyconfita-1.0.8/src/pyconfita.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      710 2022-10-25 21:42:42.000000 pyconfita-1.0.8/src/pyconfita.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2022-10-25 21:42:42.000000 pyconfita-1.0.8/src/pyconfita.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       37 2022-10-25 21:42:42.000000 pyconfita-1.0.8/src/pyconfita.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)       10 2022-10-25 21:42:42.000000 pyconfita-1.0.8/src/pyconfita.egg-info/top_level.txt
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.657634 pyconfita-1.0.9/
+-rw-r--r--   0 marc       (501) staff       (20)      897 2022-10-25 22:14:17.000000 pyconfita-1.0.9/CHANGELOG.md
+-rw-r--r--   0 marc       (501) staff       (20)     1069 2022-10-13 17:53:42.000000 pyconfita-1.0.9/LICENSE
+-rw-r--r--   0 marc       (501) staff       (20)       21 2022-10-21 11:01:43.000000 pyconfita-1.0.9/MANIFEST.in
+-rw-r--r--   0 marc       (501) staff       (20)     3819 2022-10-25 22:15:53.657170 pyconfita-1.0.9/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)     3470 2022-10-24 08:23:29.000000 pyconfita-1.0.9/README.md
+-rw-r--r--   0 marc       (501) staff       (20)       38 2022-10-25 22:15:53.657782 pyconfita-1.0.9/setup.cfg
+-rw-r--r--   0 marc       (501) staff       (20)     1076 2022-10-25 21:33:31.000000 pyconfita-1.0.9/setup.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.633784 pyconfita-1.0.9/src/
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.640769 pyconfita-1.0.9/src/pyconfita/
+-rw-r--r--   0 marc       (501) staff       (20)      388 2022-10-24 08:23:29.000000 pyconfita-1.0.9/src/pyconfita/__init__.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.646388 pyconfita-1.0.9/src/pyconfita/backend/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     1776 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/backend.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.648731 pyconfita-1.0.9/src/pyconfita/backend/dict/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/dict/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)      494 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/dict/dict.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.652772 pyconfita-1.0.9/src/pyconfita/backend/environment/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/environment/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)      407 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/environment/environment.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.654263 pyconfita-1.0.9/src/pyconfita/backend/file/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/file/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)      969 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/file/file.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.655777 pyconfita-1.0.9/src/pyconfita/backend/vault/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2022-10-21 11:01:43.000000 pyconfita-1.0.9/src/pyconfita/backend/vault/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)    10233 2022-10-25 22:15:42.000000 pyconfita-1.0.9/src/pyconfita/backend/vault/vault.py
+-rw-r--r--   0 marc       (501) staff       (20)      389 2022-10-24 08:23:29.000000 pyconfita-1.0.9/src/pyconfita/logging_interface.py
+-rw-r--r--   0 marc       (501) staff       (20)     2536 2022-10-24 08:23:29.000000 pyconfita-1.0.9/src/pyconfita/pyconfita.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2022-10-25 22:15:53.644498 pyconfita-1.0.9/src/pyconfita.egg-info/
+-rw-r--r--   0 marc       (501) staff       (20)     3819 2022-10-25 22:15:53.000000 pyconfita-1.0.9/src/pyconfita.egg-info/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      710 2022-10-25 22:15:53.000000 pyconfita-1.0.9/src/pyconfita.egg-info/SOURCES.txt
+-rw-r--r--   0 marc       (501) staff       (20)        1 2022-10-25 22:15:53.000000 pyconfita-1.0.9/src/pyconfita.egg-info/dependency_links.txt
+-rw-r--r--   0 marc       (501) staff       (20)       37 2022-10-25 22:15:53.000000 pyconfita-1.0.9/src/pyconfita.egg-info/requires.txt
+-rw-r--r--   0 marc       (501) staff       (20)       10 2022-10-25 22:15:53.000000 pyconfita-1.0.9/src/pyconfita.egg-info/top_level.txt
```

### Comparing `pyconfita-1.0.8/CHANGELOG.md` & `pyconfita-1.0.9/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.0.9 (2022-10-25)
+
+- 
+
 ## 1.0.8 (2022-10-25)
 
 - Updated requirements to replace `cachetools` by `cacheout` 
 
 ## 1.0.7 (2022-10-24)
 
 - Updated requirement cachetools<5.0.0
```

### Comparing `pyconfita-1.0.8/LICENSE` & `pyconfita-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/PKG-INFO` & `pyconfita-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconfita
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyConfita: Confita-like library for Python
 Home-page: https://github.com/m-letourneur/pyconfita.git
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyconfita-1.0.8/README.md` & `pyconfita-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/setup.py` & `pyconfita-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/src/pyconfita/backend/backend.py` & `pyconfita-1.0.9/src/pyconfita/backend/backend.py`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/src/pyconfita/backend/file/file.py` & `pyconfita-1.0.9/src/pyconfita/backend/file/file.py`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/src/pyconfita/backend/vault/vault.py` & `pyconfita-1.0.9/src/pyconfita/backend/vault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,14 +253,20 @@
         Cache key-value store (loaded from path) if caching is enabled.
         """
         if self.cache is not None:
             for k, v in kv_store.items():
                 cache_key = KeyRef(path=path, key=k).get_cache_key()
                 try:
                     self.cache.set(cache_key, v)
+                    self.logger.log(
+                        **{
+                            "level": "debug",
+                            "message": {"message": f"[Vault] Set key {k} in cache"},
+                        }
+                    )
                 except Exception as e:
                     self.logger.log(
                         **{
                             "level": "error",
                             "message": {
                                 "message": f"[Vault] Failed to cache value"
                                 f" for cache key={cache_key}"
@@ -282,17 +288,40 @@
         :return:
         """
         _value = None
 
         _path = kwargs.get("path", self.default_key_path)
         k_ref = KeyRef(path=_path, key=key)
         if self.cache:  # Cache enabled
+            self.logger.log(
+                **{
+                    "level": "debug",
+                    "message": {
+                        "message": f"[Vault][cache enabled] try to get key"
+                        f" {key} from cache"
+                    },
+                }
+            )
             _value = self.cache.get(
                 k_ref.get_cache_key(), default=KEY_NOT_FOUND_IN_CACHE
             )
             if _value == KEY_NOT_FOUND_IN_CACHE:
+                self.logger.log(
+                    **{
+                        "level": "debug",
+                        "message": {"message": f"[Vault] key {key} not found in cache"},
+                    }
+                )
                 kv_store = self._get_kv_store_when_ready(path=k_ref.path)
                 self._cache_kv_store(path=k_ref.path, kv_store=kv_store)
-                _value = kv_store.get(k_ref.key, None)
+                _value = self.cache.get(k_ref.key, default=None)
         else:
+            self.logger.log(
+                **{
+                    "level": "debug",
+                    "message": {
+                        "message": f"[Vault][cache disabled] call _get_key_when_ready"
+                    },
+                }
+            )
             _value = self._get_key_when_ready(k_ref)
         return _value
```

### Comparing `pyconfita-1.0.8/src/pyconfita/pyconfita.py` & `pyconfita-1.0.9/src/pyconfita/pyconfita.py`

 * *Files identical despite different names*

### Comparing `pyconfita-1.0.8/src/pyconfita.egg-info/PKG-INFO` & `pyconfita-1.0.9/src/pyconfita.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconfita
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyConfita: Confita-like library for Python
 Home-page: https://github.com/m-letourneur/pyconfita.git
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyconfita-1.0.8/src/pyconfita.egg-info/SOURCES.txt` & `pyconfita-1.0.9/src/pyconfita.egg-info/SOURCES.txt`

 * *Files identical despite different names*

