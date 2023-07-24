# Comparing `tmp/ossapi-3.3.1.tar.gz` & `tmp/ossapi-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.3.1.tar", last modified: Mon Jul 17 20:08:19 2023, max compression
+gzip compressed data, was "ossapi-3.3.2.tar", last modified: Mon Jul 24 19:08:53 2023, max compression
```

## Comparing `ossapi-3.3.1.tar` & `ossapi-3.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.276321 ossapi-3.3.1/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.3.1/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-17 20:08:19.276072 ossapi-3.3.1/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9958 2023-07-16 05:35:26.000000 ossapi-3.3.1/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.273502 ossapi-3.3.1/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3990 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.3.1/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    17243 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-07-17 19:16:28.000000 ossapi-3.3.1/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36593 2023-07-17 20:07:54.000000 ossapi-3.3.1/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-06-05 19:43:51.000000 ossapi-3.3.1/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    88249 2023-07-17 20:02:29.000000 ossapi-3.3.1/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    92896 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.3.1/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     9237 2023-07-17 20:04:46.000000 ossapi-3.3.1/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.274384 ossapi-3.3.1/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-07-17 20:08:08.000000 ossapi-3.3.1/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-07-17 20:08:19.276367 ossapi-3.3.1/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.275709 ossapi-3.3.1/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.3.1/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.3.1/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)    11001 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-24 19:08:53.004306 ossapi-3.3.2/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.3.2/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-24 19:08:53.003941 ossapi-3.3.2/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9958 2023-07-16 05:35:26.000000 ossapi-3.3.2/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-24 19:08:53.000972 ossapi-3.3.2/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3990 2023-07-16 04:59:00.000000 ossapi-3.3.2/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.3.2/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    17263 2023-07-24 19:07:42.000000 ossapi-3.3.2/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-07-17 19:16:28.000000 ossapi-3.3.2/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36666 2023-07-18 02:40:09.000000 ossapi-3.3.2/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-06-05 19:43:51.000000 ossapi-3.3.2/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    88249 2023-07-17 20:02:29.000000 ossapi-3.3.2/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    92896 2023-07-16 04:59:00.000000 ossapi-3.3.2/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.3.2/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     9237 2023-07-17 20:04:46.000000 ossapi-3.3.2/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-24 19:08:53.002028 ossapi-3.3.2/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-24 19:08:52.000000 ossapi-3.3.2/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-07-24 19:08:52.000000 ossapi-3.3.2/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-07-24 19:08:52.000000 ossapi-3.3.2/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-07-24 19:08:52.000000 ossapi-3.3.2/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-07-24 19:08:52.000000 ossapi-3.3.2/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-07-24 19:08:27.000000 ossapi-3.3.2/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-07-24 19:08:53.004370 ossapi-3.3.2/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-24 19:08:53.003646 ossapi-3.3.2/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.3.2/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.3.2/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11001 2023-07-16 04:59:00.000000 ossapi-3.3.2/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.3.2/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.3.2/tests/test_v1.py
```

### Comparing `ossapi-3.3.1/LICENSE` & `ossapi-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/PKG-INFO` & `ossapi-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.3.1
+Version: 3.3.2
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.3.1/README.md` & `ossapi-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/__init__.py` & `ossapi-3.3.2/ossapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/encoder.py` & `ossapi-3.3.2/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/enums.py` & `ossapi-3.3.2/ossapi/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 class UserBeatmapType(EnumModel):
     FAVOURITE = "favourite"
     GRAVEYARD = "graveyard"
     LOVED = "loved"
     MOST_PLAYED = "most_played"
     RANKED = "ranked"
     PENDING = "pending"
+    GUEST = "guest"
 
 class BeatmapDiscussionPostSort(EnumModel):
     NEW = "id_desc"
     OLD = "id_asc"
 
 class BeatmapsetStatus(EnumModel):
     ALL = "all"
```

### Comparing `ossapi-3.3.1/ossapi/mod.py` & `ossapi-3.3.2/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/models.py` & `ossapi-3.3.2/ossapi/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,17 @@
     user_achievements: Optional[List[UserAchievement]]
     user_preferences: Optional[UserProfileCustomization]
 
 
     def expand(self) -> User:
         return self._fk_user(self.id)
 
+    def refresh(self) -> User:
+        return self._fk_user(self.id)
+
 class User(UserCompact):
     comments_count: int
     cover_url: str
     discord: Optional[str]
     has_supported: bool
     interests: Optional[str]
     join_date: Datetime
@@ -1132,15 +1135,15 @@
     # deprecated, replaced by global_rank and country_rank
     rank: Optional[Any]
     ranked_score: int
     replays_watched_by_others: int
     total_hits: int
     total_score: int
     user: Optional[UserCompact]
-    variants: Optional[List[StatisticsVariant]]
+    variants: Optional[List[StatisticsVariant]] #!
 
 class UserStatisticsRulesets(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserStatisti
     # csRulesetsTransformer.php
     osu: Optional[UserStatistics]
     taiko: Optional[UserStatistics]
```

### Comparing `ossapi-3.3.1/ossapi/ossapi.py` & `ossapi-3.3.2/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/ossapiv2.py` & `ossapi-3.3.2/ossapi/ossapiv2.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/ossapiv2_async.py` & `ossapi-3.3.2/ossapi/ossapiv2_async.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/replay.py` & `ossapi-3.3.2/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi/utils.py` & `ossapi-3.3.2/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/ossapi.egg-info/PKG-INFO` & `ossapi-3.3.2/ossapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.3.1
+Version: 3.3.2
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.3.1/pyproject.toml` & `ossapi-3.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.3.1"
+version = "3.3.2"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.3.1/tests/__init__.py` & `ossapi-3.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/tests/test_cursor.py` & `ossapi-3.3.2/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/tests/test_endpoints.py` & `ossapi-3.3.2/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/tests/test_models.py` & `ossapi-3.3.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.1/tests/test_v1.py` & `ossapi-3.3.2/tests/test_v1.py`

 * *Files identical despite different names*

