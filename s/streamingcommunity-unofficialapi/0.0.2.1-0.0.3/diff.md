# Comparing `tmp/streamingcommunity_unofficialapi-0.0.2.1.tar.gz` & `tmp/streamingcommunity-unofficialapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "streamingcommunity-unofficialapi-0.0.3.tar", last modified: Mon Jul 24 12:14:35 2023, max compression
```

## Comparing `streamingcommunity_unofficialapi-0.0.2.1.tar` & `streamingcommunity-unofficialapi-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/SCuapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/README.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:14:35.797045 streamingcommunity-unofficialapi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 12:14:21.000000 streamingcommunity-unofficialapi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-24 12:14:35.797045 streamingcommunity-unofficialapi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-24 12:14:21.000000 streamingcommunity-unofficialapi-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 12:14:21.000000 streamingcommunity-unofficialapi-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:14:35.797045 streamingcommunity-unofficialapi-0.0.3/sc_uapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:14:35.797045 streamingcommunity-unofficialapi-0.0.3/sc_uapi/streamingcommunity_unofficialapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-24 12:14:35.000000 streamingcommunity-unofficialapi-0.0.3/sc_uapi/streamingcommunity_unofficialapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 12:14:35.000000 streamingcommunity-unofficialapi-0.0.3/sc_uapi/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:14:35.000000 streamingcommunity-unofficialapi-0.0.3/sc_uapi/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:14:35.000000 streamingcommunity-unofficialapi-0.0.3/sc_uapi/streamingcommunity_unofficialapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:14:35.797045 streamingcommunity-unofficialapi-0.0.3/setup.cfg
```

### Comparing `streamingcommunity_unofficialapi-0.0.2.1/README.md` & `streamingcommunity-unofficialapi-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,196 +1,203 @@
-A simple unofficial api for the italian StreamingCommunity website.
-
-
-
-# StreamingCommunity-API
-
-## Installazione
-
-Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
-
-È Possibile installarare la libreria tramite pip:
-
-
-```
-pip install streamingcommunity-unofficialapi
-```
-
-
-## Utilizzo
-
-Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-
-```
-
-### Ricerca
-Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
-
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-sc.search('John Wick')
-
-```
-
-La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
-
-#### Esempio:
-```
-{
-    "John Wick": {
-        "id": 6,
-        "slug": "john-wick",
-        "name": "John Wick",
-        "type": "movie",
-        "score": "8.1",
-        "sub_ita": 0,
-        "last_air_date": "2014-10-22",
-        "seasons_count": 0,
-        "images": [
-            {
-                "imageable_id": 6,
-                "imageable_type": "title",
-                "filename": "f7887fba-d2d3-4252-b2e9-45129e1ecfd9.webp",
-                "type": "poster",
-                "original_url_field": None,
-            },
-            {
-                "imageable_id": 6,
-                "imageable_type": "title",
-                "filename": "3ca16987-4229-4369-ba0b-670e0ec2b4df.webp",
-                "type": "background",
-                "original_url_field": None,
-            }
-        ],
-        "url": "https://StreamingCommunity.esempio/titles/6-john-wick",
-    },
-    "John Wick 4": {
-        "id": 6203,
-        "slug": "john-wick-4",
-        "name": "John Wick 4",
-        "type": "movie",
-        "score": "8.6",
-        "sub_ita": 0,
-        "last_air_date": "2023-03-22",
-        "seasons_count": 0,
-        "images": [
-            {
-                "imageable_id": 6203,
-                "imageable_type": "title",
-                "filename": "8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
-                "type": "cover_mobile",
-                "original_url_field": None,
-            },
-            {
-                "imageable_id": 6203,
-                "imageable_type": "title",
-                "filename": "64934c02-794f-4307-a860-758eed06b717.webp",
-                "type": "logo",
-                "original_url_field": None,
-            }
-        ],
-        "url": "https://StreamingCommunity.esempio/titles/6203-john-wick-4",
-    },
-}
-```
-
-### Info Film/Serie
-
-Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
-
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
-```
-
-La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
-
-#### Esempio:
-```
-{
-    "name": "John Wick 4",
-    "url": "https://StreamingCommunity.esempio/watch/6203",
-    "scws_id": 157670,
-    "type": "Movie",
-    "posterUrl": "https://cdn.StreamingCommunity.esempio/images/8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
-    "year": 2023,
-    "plot": "John Wick trova una via per sconfiggere la Gran Tavola. Ma prima di guadagnare la libertà, Wick deve affrontare un nuovo nemico che ha potenti alleanze in tutto il mondo e ha mezzi tali da tramutare vecchi amici in nuovi nemici.",
-    "tmdb_id": 603692,
-    "imdb_id": "tt10366206",
-    "netflix_id": None,
-    "prime_id": None,
-    "disney_id": None,
-    "release_date": "2023-03-22",
-    "sub_ita": False,
-    "rating": 8600,
-    "tags": ["Crime", "Azione", "Thriller"],
-    "duration": 169,
-    "trailerUrl": "https://www.youtube.com/watch?v=049RtZzgAtA",
-    "recommendations": [
-        {
-            "id": 5077,
-            "slug": "luomo-ombra",
-            "name": "L'uomo ombra",
-            "type": "movie",
-            "score": "6.0",
-            "sub_ita": 0,
-            "last_air_date": "1994-07-01",
-            "seasons_count": 0,
-            "images": [
-                {
-                    "imageable_id": 5077,
-                    "imageable_type": "title",
-                    "filename": "125664cb-82c6-403b-a262-916080307f77.webp",
-                    "type": "poster",
-                    "original_url_field": None,
-                },
-                {
-                    "imageable_id": 5077,
-                    "imageable_type": "title",
-                    "filename": "1666007b-f7df-4308-910b-4e4ae414f35a.webp",
-                    "type": "background",
-                    "original_url_field": None,
-                }
-            ],
-        },
-        {
-            "id": 1636,
-            "slug": "il-padrino",
-            "name": "Il padrino",
-            "type": "movie",
-            "score": "9.2",
-            "sub_ita": 0,
-            "last_air_date": "1972-03-14",
-            "seasons_count": 0,
-            "images": [
-                {
-                    "imageable_id": 1636,
-                    "imageable_type": "title",
-                    "filename": "37beda03-f1c5-4958-9456-b696b9d8918f.webp",
-                    "type": "cover",
-                    "original_url_field": None,
-                },
-                {
-                    "imageable_id": 1636,
-                    "imageable_type": "title",
-                    "filename": "d6bf67db-6644-4381-a3a1-7d5a75b393c6.webp",
-                    "type": "cover_mobile",
-                    "original_url_field": None,
-                }
-            ],
-        }
-    ],
-}
-
-```
-
-### Download link
-
+A simple unofficial api for the italian StreamingCommunity website.
+
+
+![PyPI](https://img.shields.io/pypi/v/streamingcommunity-unofficialapi)
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/Blu-Tiger/streamingcommunity-unofficialapi)
+
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+
+
+# StreamingCommunity-API
+
+## Installazione
+
+Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
+
+È Possibile installarare la libreria tramite pip:
+
+
+```
+pip install streamingcommunity-unofficialapi
+```
+
+
+## Utilizzo
+
+Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
+```
+from SCuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+
+```
+
+### Ricerca
+Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
+
+```
+from SCuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+sc.search('John Wick')
+
+```
+
+La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
+
+#### Esempio:
+```
+{
+    "John Wick": {
+        "id": 6,
+        "slug": "john-wick",
+        "name": "John Wick",
+        "type": "movie",
+        "score": "8.1",
+        "sub_ita": 0,
+        "last_air_date": "2014-10-22",
+        "seasons_count": 0,
+        "images": [
+            {
+                "imageable_id": 6,
+                "imageable_type": "title",
+                "filename": "f7887fba-d2d3-4252-b2e9-45129e1ecfd9.webp",
+                "type": "poster",
+                "original_url_field": None,
+            },
+            {
+                "imageable_id": 6,
+                "imageable_type": "title",
+                "filename": "3ca16987-4229-4369-ba0b-670e0ec2b4df.webp",
+                "type": "background",
+                "original_url_field": None,
+            }
+        ],
+        "url": "https://StreamingCommunity.esempio/titles/6-john-wick",
+    },
+    "John Wick 4": {
+        "id": 6203,
+        "slug": "john-wick-4",
+        "name": "John Wick 4",
+        "type": "movie",
+        "score": "8.6",
+        "sub_ita": 0,
+        "last_air_date": "2023-03-22",
+        "seasons_count": 0,
+        "images": [
+            {
+                "imageable_id": 6203,
+                "imageable_type": "title",
+                "filename": "8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
+                "type": "cover_mobile",
+                "original_url_field": None,
+            },
+            {
+                "imageable_id": 6203,
+                "imageable_type": "title",
+                "filename": "64934c02-794f-4307-a860-758eed06b717.webp",
+                "type": "logo",
+                "original_url_field": None,
+            }
+        ],
+        "url": "https://StreamingCommunity.esempio/titles/6203-john-wick-4",
+    },
+}
+```
+
+### Info Film/Serie
+
+Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
+
+```
+from SCuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
+```
+
+La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
+
+#### Esempio:
+```
+{
+    "name": "John Wick 4",
+    "url": "https://StreamingCommunity.esempio/watch/6203",
+    "scws_id": 157670,
+    "type": "Movie",
+    "posterUrl": "https://cdn.StreamingCommunity.esempio/images/8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
+    "year": 2023,
+    "plot": "John Wick trova una via per sconfiggere la Gran Tavola. Ma prima di guadagnare la libertà, Wick deve affrontare un nuovo nemico che ha potenti alleanze in tutto il mondo e ha mezzi tali da tramutare vecchi amici in nuovi nemici.",
+    "tmdb_id": 603692,
+    "imdb_id": "tt10366206",
+    "netflix_id": None,
+    "prime_id": None,
+    "disney_id": None,
+    "release_date": "2023-03-22",
+    "sub_ita": False,
+    "rating": 8600,
+    "tags": ["Crime", "Azione", "Thriller"],
+    "duration": 169,
+    "trailerUrl": "https://www.youtube.com/watch?v=049RtZzgAtA",
+    "recommendations": [
+        {
+            "id": 5077,
+            "slug": "luomo-ombra",
+            "name": "L'uomo ombra",
+            "type": "movie",
+            "score": "6.0",
+            "sub_ita": 0,
+            "last_air_date": "1994-07-01",
+            "seasons_count": 0,
+            "images": [
+                {
+                    "imageable_id": 5077,
+                    "imageable_type": "title",
+                    "filename": "125664cb-82c6-403b-a262-916080307f77.webp",
+                    "type": "poster",
+                    "original_url_field": None,
+                },
+                {
+                    "imageable_id": 5077,
+                    "imageable_type": "title",
+                    "filename": "1666007b-f7df-4308-910b-4e4ae414f35a.webp",
+                    "type": "background",
+                    "original_url_field": None,
+                }
+            ],
+        },
+        {
+            "id": 1636,
+            "slug": "il-padrino",
+            "name": "Il padrino",
+            "type": "movie",
+            "score": "9.2",
+            "sub_ita": 0,
+            "last_air_date": "1972-03-14",
+            "seasons_count": 0,
+            "images": [
+                {
+                    "imageable_id": 1636,
+                    "imageable_type": "title",
+                    "filename": "37beda03-f1c5-4958-9456-b696b9d8918f.webp",
+                    "type": "cover",
+                    "original_url_field": None,
+                },
+                {
+                    "imageable_id": 1636,
+                    "imageable_type": "title",
+                    "filename": "d6bf67db-6644-4381-a3a1-7d5a75b393c6.webp",
+                    "type": "cover_mobile",
+                    "original_url_field": None,
+                }
+            ],
+        }
+    ],
+}
+
+```
+
+### Download link
+
 In progresso.
```

### Comparing `streamingcommunity_unofficialapi-0.0.2.1/PKG-INFO` & `streamingcommunity-unofficialapi-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: streamingcommunity-unofficialapi
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: A simple unofficial api for the italian StreamingCommunity website
 Author-email: Beqir Stafa <beqirstafa@gmail.com>
-License-File: LICENSE
+Project-URL: Homepage, https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 A simple unofficial api for the italian StreamingCommunity website.
 
 
+![PyPI](https://img.shields.io/pypi/v/streamingcommunity-unofficialapi)
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/Blu-Tiger/streamingcommunity-unofficialapi)
+
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+
 
 # StreamingCommunity-API
 
 ## Installazione
 
 Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
 
@@ -201,8 +209,8 @@
     ],
 }
 
 ```
 
 ### Download link
 
-In progresso.
+In progresso.
```

