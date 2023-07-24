# Comparing `tmp/wiki_as_base-0.5.8.tar.gz` & `tmp/wiki_as_base-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiki_as_base-0.5.8.tar", last modified: Fri Jul  7 22:21:44 2023, max compression
+gzip compressed data, was "wiki_as_base-0.5.9.tar", last modified: Mon Jul 24 17:55:24 2023, max compression
```

## Comparing `wiki_as_base-0.5.8.tar` & `wiki_as_base-0.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/LICENSE
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10704 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10099 2023-07-07 22:20:12.000000 wiki_as_base-0.5.8/README.md
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/pyproject.toml
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      872 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/setup.cfg
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/wiki_as_base/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      158 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/src/wiki_as_base/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     6367 2023-07-05 07:29:06.000000 wiki_as_base-0.5.8/src/wiki_as_base/cli.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1583 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/src/wiki_as_base/constants.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    15993 2023-07-07 06:01:14.000000 wiki_as_base-0.5.8/src/wiki_as_base/parser.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    53110 2023-07-07 06:39:57.000000 wiki_as_base-0.5.8/src/wiki_as_base/wiki_as_base.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10704 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      531 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/SOURCES.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/dependency_links.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       76 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/entry_points.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       39 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/requires.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       13 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/top_level.txt
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/tests/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      774 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_internals.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1258 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_tables.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3394 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_wikitext.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_wikitext_with_network.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/LICENSE
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    11522 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10917 2023-07-24 17:53:55.000000 wiki_as_base-0.5.9/README.md
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/pyproject.toml
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      872 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/setup.cfg
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/src/
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/src/wiki_as_base/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      158 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/src/wiki_as_base/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     8784 2023-07-10 21:40:03.000000 wiki_as_base-0.5.9/src/wiki_as_base/cli.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1615 2023-07-10 20:20:17.000000 wiki_as_base-0.5.9/src/wiki_as_base/constants.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    16348 2023-07-10 20:14:21.000000 wiki_as_base-0.5.9/src/wiki_as_base/parser.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    52880 2023-07-24 17:54:05.000000 wiki_as_base-0.5.9/src/wiki_as_base/wiki_as_base.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    11522 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      531 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       76 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/entry_points.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       39 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/requires.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       13 2023-07-24 17:55:24.000000 wiki_as_base-0.5.9/src/wiki_as_base.egg-info/top_level.txt
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-24 17:55:24.394626 wiki_as_base-0.5.9/tests/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      774 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/tests/test_internals.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1258 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/tests/test_tables.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3394 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/tests/test_wikitext.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.9/tests/test_wikitext_with_network.py
```

### Comparing `wiki_as_base-0.5.8/LICENSE` & `wiki_as_base-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.8/PKG-INFO` & `wiki_as_base-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiki_as_base
-Version: 0.5.8
+Version: 0.5.9
 Summary: Use MediaWiki Wiki page content as read-only database
 Home-page: https://github.com/fititnt/wiki_as_base-py
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/wiki_as_base-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -46,27 +46,38 @@
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
 ## Alternative:
-# pip install wiki_as_base==0.5.8
+# pip install wiki_as_base==0.5.9
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
 export WIKI_NS='osmwiki'
-export WTXT_PAGE_LIMIT='50'
+export CACHE_TTL='82800'  # 82800 seconds = 23 hours
+```
+
+**Suggested**. Customize user agent. [Follows the logic of MediaWiki user agent](https://meta.wikimedia.org/wiki/User-Agent_policy). Without `WIKI_AS_BASE_BOT_CONTACT` customization, for recursive and pagination requests already not cached locally will far slower, with a delay 10 seconds. This default may increase in future releases. Does not affect direct requests (likely ones with less than 50 pages).
+
+<!-- export WIKI_AS_BASE_BOTNAME='wiki_as_base-cli-bot/0.5.9' -->
+
+```bash
+export WIKI_AS_BASE_BOT_CONTACT='https://github.com/fititnt/wiki_as_base-py; generic@example.org'
 ```
 
 <!--
+# To increase de delay over the 1
+
+export WIKI_AS_BASE_BOT_CUSTOM_DELAY='60'
 export WIKI_INFOBOXES='ValueDescription\nKeyDescription'
 export WIKI_DATA_LANGS='yaml\nturtle'
 -->
 
 ## Command line Usage
 
 ### Quickstart
@@ -194,15 +205,20 @@
 
 ## Filter Templates
 wiki_as_base --titles 'User:EmericusPetro/sandbox/Wiki-as-base' | jq '.data[] | select(.["@type"] == "wtxt:Template")'
 ```
 
 ### Save JSON-LD extracted as files
 
-> TODO: explain the implemented feature
+Use `--output-zip-file` parameter. One example:
+
+```bash
+wiki_as_base --input-autodetect 'Category:References' --output-zip-file ~/Downloads/Category:References.zip
+
+```
 
 ## Library usage
 
 <!--
 - See [src/wiki_as_base/cli.py](src/wiki_as_base/cli.py)
 - See [tests/](tests/)
 -->
@@ -211,15 +227,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.8
+wiki_as_base==0.5.9
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.8/README.md` & `wiki_as_base-0.5.9/src/wiki_as_base.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiki-as-base
+Version: 0.5.9
+Summary: Use MediaWiki Wiki page content as read-only database
+Home-page: https://github.com/fititnt/wiki_as_base-py
+Author: Emerson Rocha
+Author-email: rocha@ieee.org
+Project-URL: Bug Tracker, https://github.com/fititnt/wiki_as_base-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Operating System :: OS Independent
+Classifier: Typing :: Typed
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # wiki_as_base-py
 [MVP] Use MediaWiki Wiki page content as read-only database. Python library implementation. See https://github.com/fititnt/openstreetmap-serverless-functions/tree/main/function/wiki-as-base
 
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%2Fwiki_as_base--py-lightgrey?logo=github&style=social[fititnt/wiki_as_base-py] "GitHub")](https://github.com/fititnt/wiki_as_base-py)
 [![Pypi: wiki_as_base](https://img.shields.io/badge/python%20pypi-wiki_as_base-brightgreen[Python] 
  "Pypi: wiki_as_base")](https://pypi.org/project/wiki_as_base)
 
@@ -29,27 +46,38 @@
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
 ## Alternative:
-# pip install wiki_as_base==0.5.8
+# pip install wiki_as_base==0.5.9
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
 export WIKI_NS='osmwiki'
-export WTXT_PAGE_LIMIT='50'
+export CACHE_TTL='82800'  # 82800 seconds = 23 hours
+```
+
+**Suggested**. Customize user agent. [Follows the logic of MediaWiki user agent](https://meta.wikimedia.org/wiki/User-Agent_policy). Without `WIKI_AS_BASE_BOT_CONTACT` customization, for recursive and pagination requests already not cached locally will far slower, with a delay 10 seconds. This default may increase in future releases. Does not affect direct requests (likely ones with less than 50 pages).
+
+<!-- export WIKI_AS_BASE_BOTNAME='wiki_as_base-cli-bot/0.5.9' -->
+
+```bash
+export WIKI_AS_BASE_BOT_CONTACT='https://github.com/fititnt/wiki_as_base-py; generic@example.org'
 ```
 
 <!--
+# To increase de delay over the 1
+
+export WIKI_AS_BASE_BOT_CUSTOM_DELAY='60'
 export WIKI_INFOBOXES='ValueDescription\nKeyDescription'
 export WIKI_DATA_LANGS='yaml\nturtle'
 -->
 
 ## Command line Usage
 
 ### Quickstart
@@ -177,15 +205,20 @@
 
 ## Filter Templates
 wiki_as_base --titles 'User:EmericusPetro/sandbox/Wiki-as-base' | jq '.data[] | select(.["@type"] == "wtxt:Template")'
 ```
 
 ### Save JSON-LD extracted as files
 
-> TODO: explain the implemented feature
+Use `--output-zip-file` parameter. One example:
+
+```bash
+wiki_as_base --input-autodetect 'Category:References' --output-zip-file ~/Downloads/Category:References.zip
+
+```
 
 ## Library usage
 
 <!--
 - See [src/wiki_as_base/cli.py](src/wiki_as_base/cli.py)
 - See [tests/](tests/)
 -->
@@ -194,15 +227,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.8
+wiki_as_base==0.5.9
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.8/setup.cfg` & `wiki_as_base-0.5.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wiki_as_base
-version = 0.5.8
+version = 0.5.9
 author = Emerson Rocha
 author_email = rocha@ieee.org
 description = Use MediaWiki Wiki page content as read-only database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fititnt/wiki_as_base-py
 project_urls =
```

### Comparing `wiki_as_base-0.5.8/src/wiki_as_base/constants.py` & `wiki_as_base-0.5.9/src/wiki_as_base/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 # TODO make this configurable per wiki
 _default_templates = {
     # https://wiki.openstreetmap.org/wiki/Template:Description
     "Description": "",
     "Feature": "",
     "KeyDescription": "",
+    "KeyDescriptionStrict": "",
     "ValueDescription": "",
     "KeyPrefixDescription": "",
     # https://wiki.openstreetmap.org/wiki/Template:RelationDescription
     "RelationDescription": "",
     # https://wiki.openstreetmap.org/wiki/Template:ElementUsage
     "ElementUsage": "",
 }
```

### Comparing `wiki_as_base-0.5.8/src/wiki_as_base/parser.py` & `wiki_as_base-0.5.9/src/wiki_as_base/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,26 @@
 import re
 import wikitextparser as wtp
 
 from .constants import WIKI_DATA_LANGS, WIKI_TEMPLATES, _default_langs
 
 
 @dataclass
+class WikibaseContext:
+    wikibasejson: str
+    pageid: int
+    title: str
+    user: str
+    timestamp: str
+    title_norm: str = field(init=False)
+
+    def __post_init__(self):
+        self.title_norm = self.title.replace(" ", "_")
+
+@dataclass
 class WikipageContext:
     wikitext: str
     pageid: int
     title: str
     user: str
     timestamp: str
     title_norm: str = field(init=False)
@@ -180,14 +192,19 @@
 def parse_all(
     pagectx: WikipageContext,
     sitectx: WikisiteContext,
     itemfilter: WikitextOutputFilter = None,
 ) -> list:
     page_data = []
 
+    # print(WikipageContext)
+    # print(WikipageContext.__dict__)
+
+    # raise ValueError(WikipageContext)
+
     if not itemfilter or itemfilter.allowed_type("wtxt:TextCorpus"):
         tcorpus = wtxt_text_corpus(pagectx.wikitext)
         if tcorpus:
             page_data.append(
                 {
                     # "@type": "wiki/outline",
                     # "@type": "wtxt:DataCollectionOutline",
```

### Comparing `wiki_as_base-0.5.8/src/wiki_as_base/wiki_as_base.py` & `wiki_as_base-0.5.9/src/wiki_as_base/wiki_as_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # from ctypes import Union
 import datetime
 import io
 import json
 import os
 import re
 import sys
+import time
 
 # import sys
 # from typing import Any, List, Union
 from typing import List
 import zipfile
 import requests
 import requests_cache
@@ -48,17 +49,32 @@
     # parse_sections,
     # parse_tables,
     wtxt_text_corpus,
 )
 
 from .constants import WIKI_DATA_LANGS
 
-_REFVER = "0.5.8"
+_REFVER = "0.5.9"
 
-USER_AGENT = os.getenv("USER_AGENT", "wiki-as-base/" + _REFVER)
+
+WIKI_AS_BASE_BOTNAME = os.getenv(
+    "WIKI_AS_BASE_BOTNAME", "wiki_as_base-cli-bot/" + _REFVER
+)
+_WIKI_AS_BASE_BOT_CONTACT_DEFAULT = (
+    "https://github.com/fititnt/wiki_as_base-py; generic@example.org"
+)
+WIKI_AS_BASE_BOT_CONTACT = os.getenv(
+    "WIKI_AS_BASE_BOT_CONTACT", _WIKI_AS_BASE_BOT_CONTACT_DEFAULT
+)
+WIKI_AS_BASE_LIB = f"wiki_as_base/{_REFVER}"
+
+_USER_AGENT_MERGED = (
+    f"{WIKI_AS_BASE_BOTNAME} ({WIKI_AS_BASE_BOT_CONTACT}) {WIKI_AS_BASE_LIB}"
+)
+USER_AGENT = os.getenv("USER_AGENT", _USER_AGENT_MERGED)
 WIKI_API = os.getenv("WIKI_API", "https://wiki.openstreetmap.org/w/api.php")
 
 # Consider using prefix like https://dumps.wikimedia.org/backup-index.html
 WIKI_NS = os.getenv("WIKI_NS", "osmwiki")
 WIKI_BASE = os.getenv("WIKI_BASE", lambda x: WIKI_API.replace("/w/api.php", "/wiki/"))
 
 # @TODO document better this part
@@ -66,14 +82,23 @@
 WTXT_PAGE_OFFSET = int(os.getenv("WTXT_PAGE_OFFSET", "0"))
 
 CACHE_DRIVER = os.getenv("CACHE_DRIVER", "sqlite")
 
 # CACHE_TTL = int(os.getenv("CACHE_TTL", "3600"))  # 1 hour
 CACHE_TTL = int(os.getenv("CACHE_TTL", "82800"))  # 23 hours
 
+DELAY_GENERIC_CONTACT = int(os.getenv("DELAY_GENERIC_CONTACT", "10"))  # 10 seconds
+# DELAY_NONGENERIC_CONTACT = int(
+#     os.getenv("DELAY_GENERIC_CONTACT", "0")
+# )  # 0 seconds (0 seconds + server delay for pagination)
+DELAY_NONGENERIC_CONTACT = 1  # 1 second
+WIKI_AS_BASE_BOT_CUSTOM_DELAY = int(
+    os.getenv("WIKI_AS_BASE_BOT_CUSTOM_DELAY", DELAY_NONGENERIC_CONTACT)
+)
+
 # @see https://requests-cache.readthedocs.io/en/stable/
 requests_cache.install_cache(
     "wikiasbase",
     # /tmp OpenFaaS allow /tmp be writtable even in read-only mode
     # However, is not granted that changes will persist or shared
     db_path="/tmp/wikiasbase_cache.sqlite",
     backend=CACHE_DRIVER,
@@ -90,14 +115,17 @@
     "https://wtxt.etica.ai/context.jsonld"
 )
 _JSONSCHEMA = (
     # "https://raw.githubusercontent.com/fititnt/wiki_as_base-py/main/schema.json"
     "https://wtxt.etica.ai/schema.json"
 )
 
+# @TODO maybe also implement Wikibase fetch?
+
+# https://wiki.openstreetmap.org/wiki/Special:ApiSandbox#action=wbgetentities&format=json&ids=Q12345
 
 # raise ValueError(WIKI_DATA_LANGS)
 # CACHE_DRIVER = os.getenv("CACHE_DRIVER", "sqlite")
 # CACHE_TTL = os.getenv("CACHE_TTL", "3600")  # 1 hour
 
 # # @see https://requests-cache.readthedocs.io/en/stable/
 # requests_cache.install_cache(
@@ -118,14 +146,29 @@
 # REG = re.compile('<syntaxhighlight lang=\"([a-z0-9]{2,20})\">(.*?)</syntaxhighlight>', flags='gmus')
 # REG_SH_GENERIC = re.compile(
 #     '<syntaxhighlight lang="(?P<lang>[a-z0-9]{2,20})">(?P<data>.*?)</syntaxhighlight>',
 #     flags=re.M | re.S | re.U,
 # )
 
 
+def delay_consecutive_request():
+    """delay_consecutive_request compute delay for implicit requests
+
+    Returns:
+        int: delay in seconds
+    """
+    # Identified users or not, we allow higher defined delays than the default 10s
+    if WIKI_AS_BASE_BOT_CUSTOM_DELAY > DELAY_NONGENERIC_CONTACT:
+        return WIKI_AS_BASE_BOT_CUSTOM_DELAY
+
+    if WIKI_AS_BASE_BOT_CONTACT == _WIKI_AS_BASE_BOT_CONTACT_DEFAULT:
+        return DELAY_GENERIC_CONTACT
+    return DELAY_NONGENERIC_CONTACT
+
+
 def wiki_as_base_all(
     wikitext: str,
     template_keys: List[str] = None,
     syntaxhighlight_langs: List[str] = None,
     meta: dict = None,
     _next_release: bool = False,
 ) -> dict:
@@ -594,25 +637,39 @@
                     zip_file.writestr(file_name, file_data)
 
             zip_buffer.seek(0)
             return zip_buffer.getvalue()
             # return str(zip_buffer.getvalue())
 
 
+def wikitext_item_as_file(jsonld_object: dict) -> str:
+    if not jsonld_object or not isinstance(jsonld_object, dict):
+        raise SyntaxError("wikitext_item_as_file invalid type")
+
+    if "wtxt:literalData" in jsonld_object:
+        return jsonld_object["wtxt:literalData"]
+    else:
+        # TODO improve this part
+        return json.dumps(jsonld_object, ensure_ascii=False, indent=2)
+
+
 class WikitextAsData:
     """Main class to deal with conversion from Wikitext to linked data"""
 
     wikitext: str
     api_response: dict
     errors: list
     is_fetch_required: bool
     _wikiapi_meta: dict
     _req_params: dict
     _req_params_rest: dict
+    _req_params_wb: dict
+    _req_params_wb_rest: dict
     _reloaded: bool
+    _mode: str = "wikitext"  # wikitext, wikibase
     # _filters: dict
     _filters: WikitextOutputFilter = None
 
     # # The individual resources to add on the JSON-LD data field
     _resources: list
 
     def __init__(self, api_params: dict = None, filters: dict = None) -> None:
@@ -642,14 +699,34 @@
             "titles": None,
             "pageids": None,
             "revids": None,
             "format": "json",
             "formatversion": "2",
         }
 
+        default_params_wb = {
+            "action": "wbgetentities",
+            # "prop": "revisions",
+            # "prop": "revisions|categories|templates",
+            "prop": "info|sitelinks|aliases|labels|descriptions|claims|datatype|sitelinks/urls",
+            # nfo%7Csitelinks%7Caliases%7Clabels%7Cdescriptions%7Cclaims%7Cdatatype%7Csitelinks%2Furls
+            # "rvprop": "content",
+            # "rvprop": "content|timestamp|user",
+            # "rvprop": "content|timestamp|user|langlinks",
+            # "rvslots": "main",
+            # "rvlimit": 1,
+            # "titles": title,
+            # "titles": None,
+            # "pageids": None,
+            # "revids": None,
+            "ids": None,
+            "format": "json",
+            "formatversion": "2",
+        }
+
         # @TODO maybe remove this part later
         ## prop=pageprops, prop=wbentityusage (example from Key:maxspeed)
         # "pageprops": {
         #     "displaytitle": "Key:maxspeed",
         #     "wikibase_item": "Q414"
         # },
         # "wbentityusage": {
@@ -678,21 +755,26 @@
 
         self._req_params = default_params
         self._req_params_rest = {
             "titles": None,
             "pageids": None,
             "revids": None,
         }
+        self._req_params_wb = default_params_wb
+        self._req_params_wb_rest = {"ids": None}
 
         # @TODO deal better with reset of the class to avoid reuse
         self.wikitext = None
         self.api_response = None
         self.errors = []
         self.is_fetch_required = None
         self.is_fetch_incomplete = None
+        self.is_verbose = False
+        self._last_fetch_from_cache = None
+        self._last_fetch_expired = None
         self._wikiapi_meta = None
         self._reloaded = None
         self._resources = []
 
     def _add_resource(self, resource: dict):
         self._resources.append(resource)
 
@@ -722,14 +804,17 @@
 
         res = None
 
         try:
             headers = {"User-Agent": USER_AGENT}
             req = requests.get(WIKI_API, headers=headers, params=self._req_params)
             res = req.json()
+            # https://requests-cache.readthedocs.io/en/stable/user_guide/expiration.html
+            self._last_fetch_from_cache = req.from_cache
+            self._last_fetch_expired = req.is_expired
         except Exception as err:
             # sys.stderr.write(f"{err}\n")
             self.errors.append(f"_request_api get {err}")
             # print(err)
             pass
 
         if res:
@@ -776,144 +861,72 @@
                 timestamp=page["revisions"][0]["timestamp"],
             )
             self._resources.extend(parse_all(wpage, wsite, self._filters))
             continue
 
         return True
 
-        for page in self.api_response["query"]["pages"]:
-            _pageid = page["pageid"]
-            _title = page["title"]
-            _title_norm = _title.replace(" ", "_")
-
-            # @TODO fix me, only <NS:pagetitle> is wrong; some pages are in
-            #       subfolders
-
-            # We only get the first revision
-            _user = page["revisions"][0]["user"]
-            _timestamp = page["revisions"][0]["timestamp"]
-            _wikitext = page["revisions"][0]["slots"]["main"]["content"]
-
-            # outline
-            tcorpus = wtxt_text_corpus(_wikitext)
-            if tcorpus:
-                self._resources.append(
-                    {
-                        # "@type": "wiki/outline",
-                        # "@type": "wtxt:DataCollectionOutline",
-                        "@type": "wtxt:TextCorpus",
-                        "@id": f"{WIKI_NS}:{_title_norm}#__textcorpus",
-                        "wtxt:inWikipage": f"{WIKI_NS}:{_title_norm}",
-                        # @TODO remove prefix outline/ from here
-                        #       and implement on zip output only
-                        "wtxt:suggestedFilename": f"corpora/{WIKI_NS}:{_title_norm}.txt",
-                        "wtxt:uniqueFilename": f"corpora/{WIKI_NS}_pageid{_pageid}.txt",
-                        "wtxt:timestamp": _timestamp,
-                        "wtxt:user": _user,
-                        # 'data_raw': outline,
-                        # data_raw_key: outline,
-                        "wtxt:literalData": tcorpus,
-                    }
-                )
-
-            # wth = WikitextHeading(_wikitext)
-            # outline = wth.get_outline()
-            # if outline:
-            #     self._resources.append(
-            #         {
-            #             # "@type": "wiki/outline",
-            #             # "@type": "wtxt:DataCollectionOutline",
-            #             "@type": "wtxt:PageOutline",
-            #             "@id": f"{WIKI_NS}:{_title_norm}#__outline",
-            #             "wtxt:inWikipage": f"{WIKI_NS}:{_title_norm}",
-            #             # @TODO remove prefix outline/ from here
-            #             #       and implement on zip output only
-            #             "wtxt:suggestedFilename": f"outline/{WIKI_NS}:{_title_norm}.html",
-            #             "wtxt:uniqueFilename": f"outline/{WIKI_NS}_pageid{_pageid}.html",
-            #             "wtxt:timestamp": _timestamp,
-            #             "wtxt:user": _user,
-            #             # 'data_raw': outline,
-            #             # data_raw_key: outline,
-            #             "wtxt:literalData": outline,
-            #         }
-            #     )
-
-            # Infoboxes
-            if template_keys is not None and len(template_keys) > 0:
-                for item in template_keys:
-                    result = wiki_as_base_from_infobox(_wikitext, item)
-                    if result:
-                        self._resources.append(result)
-
-            # preformated blocks
-            if syntaxhighlight_langs is not None and len(syntaxhighlight_langs) > 0:
-                index_syntax = 0
-                for item in syntaxhighlight_langs:
-                    results = wiki_as_base_from_syntaxhighlight(_wikitext, item)
-                    # results = wiki_as_base_from_syntaxhighlight(wikitext)
-                    index_syntax += 1
-                    if results:
-                        for result in results:
-                            if not result:
-                                continue
-                            fileextension = result[1]
-                            if result[2]:
-                                # @TODO make this smarter
-                                self._resources.append(
-                                    {
-                                        "@type": "wtxt:PreformattedCode",
-                                        "wtxt:syntaxLang": result[1],
-                                        "wtxt:suggestedFilename": result[2],
-                                        "wtxt:uniqueFilename": f"{WIKI_NS}_pageid{_pageid}_item{index_syntax}.{fileextension}",
-                                        "wtxt:inWikipage": f"{WIKI_NS}:{_title_norm}",
-                                        "wtxt:literalData": result[0],
-                                    }
-                                )
-                            else:
-                                self._resources.append(
-                                    {
-                                        "@type": "wtxt:PreformattedCode",
-                                        "wtxt:syntaxLang": result[1],
-                                        "wtxt:uniqueFilename": f"{WIKI_NS}_pageid{_pageid}_item{index_syntax}.{fileextension}",
-                                        "wtxt:inWikipage": f"{WIKI_NS}:{_title_norm}",
-                                        "wtxt:literalData": result[0],
-                                    }
-                                )
-
-            wmt = WikitextTable(_wikitext)
-            tables = wmt.get_tables()
-            if tables and len(tables) > 0:
-                index = 1
-                for table in tables:
-                    table_data = [table["header"]] + table["data"]
-
-                    _tbl = {
-                        "@type": "wtxt:Table",
-                        # "@id": f"t{index}",
-                        "@id": f"{WIKI_NS}_pageid{_pageid}_table{index}",
-                        # "wtxt:uniqueFilename": f"{WIKI_NS}_pageid{_pageid}_table{index}.csv",
-                        "wtxt:inWikipage": f"{WIKI_NS}:{_title_norm}",
-                        "wtxt:tableData": table_data,
-                        "_is_complete": table["_is_complete"],
-                        "_errors": table["_errors"]
-                        # "_type": "wtxt:Table",
-                    }
-                    # table["@type"] = "wtxt:Table"
-                    # table["@id"] = f"t{index}"
-                    # _tbl.update(table)
-                    self._resources.append(_tbl)
-                    index += 1
-
     def get(self, key: str, strict: bool = True):
         if key in self.__dict__:
             return self.__dict__[key]
 
         if strict:
             raise ValueError(f"WikitextAsData key [{key}]?")
 
+    # def get_singlefile(self, filename_hint: str) -> Tuple(str, list, list):
+    def get_singlefile(self, filename_hint: str) -> Tuple:
+        file_mached = False
+        list_fileids = []
+        list_named = []
+        # list_namesuggested = []
+        list_ambiguous = set()
+
+        if not self._reloaded:
+            self.prepare()
+
+        if self.is_success():
+            for item in self._resources:
+                if "wtxt:uniqueFilename" in item:
+                    list_fileids.append(item["wtxt:uniqueFilename"])
+
+                    if item["wtxt:uniqueFilename"] == filename_hint:
+                        file_mached = item
+                        break
+
+                if "wtxt:suggestedFilename" in item:
+                    if item["wtxt:suggestedFilename"] in list_named:
+                        list_ambiguous.add(item["wtxt:suggestedFilename"])
+                    else:
+                        list_named.append(item["wtxt:suggestedFilename"])
+                # print(item)
+            # pass
+            if not file_mached:
+                _suggested_mached = None
+
+                # @TODO: do a fuzzy match if don't find an near exact.
+                # @TODO: mimic user giving as name the #Title_Hash of a title and get files inside
+                for potential in list_named:
+                    if filename_hint == potential:
+                        _suggested_mached = potential
+                        break
+
+                for item in self._resources:
+                    if (
+                        "wtxt:suggestedFilename" in item
+                        and _suggested_mached == item["wtxt:suggestedFilename"]
+                    ):
+                        file_mached = item
+                        break
+
+        if file_mached:
+            file_mached = wikitext_item_as_file(file_mached)
+
+        # self.is_verbose = filename_hint
+        return file_mached, list_fileids, list_named, list(list_ambiguous)
+
     def is_success(self) -> bool:
         """is_success is remote fetch okay?
 
         Returns:
             bool: True if okay
         """
         return not self.errors or len(self.errors) == 0
@@ -1041,15 +1054,23 @@
 
             elif self._req_params_rest["titles"] is not None:
                 self.set_titles(self._req_params_rest["titles"])
             else:
                 raise NotImplemented
 
             # Move this to somewhere else
-            print("loop...", file=sys.stderr)
+            if self.is_verbose:
+                print(
+                    f"loop... Cached: [{self._last_fetch_from_cache}] Expired: [{self._last_fetch_expired}] delay if not cached [{delay_consecutive_request()}]",
+                    file=sys.stderr,
+                )
+
+            if not self._last_fetch_from_cache:
+                time.sleep(delay_consecutive_request())
+
             return self.prepare()
 
         self._reloaded = True
 
         return self
 
     # def set_filters(self, filters: dict):
@@ -1152,14 +1173,27 @@
         self.is_fetch_required = True
         self.is_fetch_incomplete = bool(self._req_params_rest["titles"])
         del self._req_params["pageids"]
         del self._req_params["revids"]
 
         return self
 
+    def set_verbose(self, is_verbose: bool = True):
+        self.is_verbose = is_verbose
+        return self
+
+    def set_wikibaseids(self, wikibaseids: str):
+        self._mode = "wikibase"
+
+        self._req_params_wb["ids"], self._req_params_rest["ids"] = self._pagination(
+            wikibaseids
+        )
+
+        return self
+
     def set_wikitext(self, wikitext: str):
         """set_wikitext set Wikitext directly instead of make API request
 
         Potential use: for piped in content
 
         Args:
             wikitext (str): the Wikitext
@@ -1167,14 +1201,17 @@
         self.wikitext = wikitext
 
         # If user define wikitext directly, we assume no remote call is need
         self.is_fetch_required = False
         return self
 
 
+# class WikibaseInternalJSONAsData(WikitextAsData):
+#     pass
+
 # class Wikipage:
 #     pass
 
 
 class WikitextGenericPart(ABC):
     """WikitextGenericPart abstract class for parts of a page"""
```

### Comparing `wiki_as_base-0.5.8/src/wiki_as_base.egg-info/PKG-INFO` & `wiki_as_base-0.5.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiki-as-base
-Version: 0.5.8
-Summary: Use MediaWiki Wiki page content as read-only database
-Home-page: https://github.com/fititnt/wiki_as_base-py
-Author: Emerson Rocha
-Author-email: rocha@ieee.org
-Project-URL: Bug Tracker, https://github.com/fititnt/wiki_as_base-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Operating System :: OS Independent
-Classifier: Typing :: Typed
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # wiki_as_base-py
 [MVP] Use MediaWiki Wiki page content as read-only database. Python library implementation. See https://github.com/fititnt/openstreetmap-serverless-functions/tree/main/function/wiki-as-base
 
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%2Fwiki_as_base--py-lightgrey?logo=github&style=social[fititnt/wiki_as_base-py] "GitHub")](https://github.com/fititnt/wiki_as_base-py)
 [![Pypi: wiki_as_base](https://img.shields.io/badge/python%20pypi-wiki_as_base-brightgreen[Python] 
  "Pypi: wiki_as_base")](https://pypi.org/project/wiki_as_base)
 
@@ -46,27 +29,38 @@
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
 ## Alternative:
-# pip install wiki_as_base==0.5.8
+# pip install wiki_as_base==0.5.9
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
 export WIKI_NS='osmwiki'
-export WTXT_PAGE_LIMIT='50'
+export CACHE_TTL='82800'  # 82800 seconds = 23 hours
+```
+
+**Suggested**. Customize user agent. [Follows the logic of MediaWiki user agent](https://meta.wikimedia.org/wiki/User-Agent_policy). Without `WIKI_AS_BASE_BOT_CONTACT` customization, for recursive and pagination requests already not cached locally will far slower, with a delay 10 seconds. This default may increase in future releases. Does not affect direct requests (likely ones with less than 50 pages).
+
+<!-- export WIKI_AS_BASE_BOTNAME='wiki_as_base-cli-bot/0.5.9' -->
+
+```bash
+export WIKI_AS_BASE_BOT_CONTACT='https://github.com/fititnt/wiki_as_base-py; generic@example.org'
 ```
 
 <!--
+# To increase de delay over the 1
+
+export WIKI_AS_BASE_BOT_CUSTOM_DELAY='60'
 export WIKI_INFOBOXES='ValueDescription\nKeyDescription'
 export WIKI_DATA_LANGS='yaml\nturtle'
 -->
 
 ## Command line Usage
 
 ### Quickstart
@@ -194,15 +188,20 @@
 
 ## Filter Templates
 wiki_as_base --titles 'User:EmericusPetro/sandbox/Wiki-as-base' | jq '.data[] | select(.["@type"] == "wtxt:Template")'
 ```
 
 ### Save JSON-LD extracted as files
 
-> TODO: explain the implemented feature
+Use `--output-zip-file` parameter. One example:
+
+```bash
+wiki_as_base --input-autodetect 'Category:References' --output-zip-file ~/Downloads/Category:References.zip
+
+```
 
 ## Library usage
 
 <!--
 - See [src/wiki_as_base/cli.py](src/wiki_as_base/cli.py)
 - See [tests/](tests/)
 -->
@@ -211,15 +210,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.8
+wiki_as_base==0.5.9
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.8/src/wiki_as_base.egg-info/SOURCES.txt` & `wiki_as_base-0.5.9/src/wiki_as_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.8/tests/test_internals.py` & `wiki_as_base-0.5.9/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.8/tests/test_tables.py` & `wiki_as_base-0.5.9/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.8/tests/test_wikitext.py` & `wiki_as_base-0.5.9/tests/test_wikitext.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.8/tests/test_wikitext_with_network.py` & `wiki_as_base-0.5.9/tests/test_wikitext_with_network.py`

 * *Files identical despite different names*

