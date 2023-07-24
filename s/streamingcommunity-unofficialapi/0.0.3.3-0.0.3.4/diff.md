# Comparing `tmp/streamingcommunity_unofficialapi-0.0.3.3.tar.gz` & `tmp/streamingcommunity-unofficialapi-0.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcommunity_unofficialapi-0.0.3.3.tar", last modified: Mon Jul 24 13:14:58 2023, max compression
+gzip compressed data, was "streamingcommunity-unofficialapi-0.0.3.4.tar", last modified: Mon Jul 24 15:30:06 2023, max compression
```

## Comparing `streamingcommunity_unofficialapi-0.0.3.3.tar` & `streamingcommunity-unofficialapi-0.0.3.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/src/scuapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:30:06.377390 streamingcommunity-unofficialapi-0.0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 15:29:53.000000 streamingcommunity-unofficialapi-0.0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-24 15:30:06.377390 streamingcommunity-unofficialapi-0.0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-24 15:29:53.000000 streamingcommunity-unofficialapi-0.0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:30:06.377390 streamingcommunity-unofficialapi-0.0.3.4/scuapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 15:29:53.000000 streamingcommunity-unofficialapi-0.0.3.4/scuapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-24 15:29:53.000000 streamingcommunity-unofficialapi-0.0.3.4/scuapi/scuapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:30:06.377390 streamingcommunity-unofficialapi-0.0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 15:29:53.000000 streamingcommunity-unofficialapi-0.0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:30:06.377390 streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-24 15:30:06.000000 streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 15:30:06.000000 streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:30:06.000000 streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 15:30:06.000000 streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/top_level.txt
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/LICENSE` & `streamingcommunity-unofficialapi-0.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/PKG-INFO` & `streamingcommunity-unofficialapi-0.0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
-Name: streamingcommunity_unofficialapi
-Version: 0.0.3.3
+Name: streamingcommunity-unofficialapi
+Version: 0.0.3.4
 Summary: A simple unofficial api for the italian StreamingCommunity website.
 Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
 Author: Beqir Stafa
-Author-email: beqirstafa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
@@ -39,27 +38,27 @@
 ```
 
 
 ## Utilizzo
 
 Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 
 ```
 
 ### Ricerca
 Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.search('John Wick')
 
 ```
 
 La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
 
 #### Esempio:
@@ -123,17 +122,17 @@
 ```
 
 ### Info Film/Serie
 
 Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
 ```
 
 La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
 
 #### Esempio:
 ```
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/README.md` & `streamingcommunity-unofficialapi-0.0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 ```
 
 
 ## Utilizzo
 
 Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 
 ```
 
 ### Ricerca
 Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.search('John Wick')
 
 ```
 
 La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
 
 #### Esempio:
@@ -107,17 +107,17 @@
 ```
 
 ### Info Film/Serie
 
 Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
 ```
 
 La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
 
 #### Esempio:
 ```
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/setup.py` & `streamingcommunity-unofficialapi-0.0.3.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from setuptools import setup, find_packages
+import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setup(
-    name="streamingcommunity_unofficialapi",
+setuptools.setup(
+    name="streamingcommunity-unofficialapi",
+    version="0.0.3.4",
     author="Beqir Stafa",
-    author_email="beqirstafa@gmail.com",
-    license='MIT',
+    description="A simple unofficial api for the italian StreamingCommunity website.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blu-Tiger/streamingcommunity-unofficialapi",
-    description="A simple unofficial api for the italian StreamingCommunity website.",
-    version="0.0.3.3",
-    packages=find_packages(),
-    install_requires=[
-        "setuptools>=61.0",
-    ],
+    packages=setuptools.find_packages(),
+    install_requires=[],
+	license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Topic :: Utilities",
+		"Topic :: Utilities",
     ],
     python_requires='>= 3.10',
 )
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/src/scuapi.py` & `streamingcommunity-unofficialapi-0.0.3.4/scuapi/scuapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import base64
 import json
 import re
 
 
 #streamingcommunity bet
 
-class SCAPI:
+class API:
     def __init__(self, DOMAIN, userAgent="Mozilla/5.0 (Windows NT 11.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"):
         self.userAgent = userAgent
         self.DOMAIN = DOMAIN
         self.URL = 'https://' + self.DOMAIN
 
     def search(self, query):
         headers = {'user-agent': self.userAgent}
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/PKG-INFO` & `streamingcommunity-unofficialapi-0.0.3.4/streamingcommunity_unofficialapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: streamingcommunity-unofficialapi
-Version: 0.0.3.3
+Version: 0.0.3.4
 Summary: A simple unofficial api for the italian StreamingCommunity website.
 Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
 Author: Beqir Stafa
-Author-email: beqirstafa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
@@ -39,27 +38,27 @@
 ```
 
 
 ## Utilizzo
 
 Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 
 ```
 
 ### Ricerca
 Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.search('John Wick')
 
 ```
 
 La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
 
 #### Esempio:
@@ -123,17 +122,17 @@
 ```
 
 ### Info Film/Serie
 
 Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
 
 ```
-from scuapi import SCAPI
+from scuapi import API
 
-sc = SCAPI('StreamingCommunity.esempio')
+sc = API('StreamingCommunity.esempio')
 sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
 ```
 
 La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
 
 #### Esempio:
 ```
```

