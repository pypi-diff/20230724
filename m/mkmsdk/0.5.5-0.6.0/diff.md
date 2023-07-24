# Comparing `tmp/mkmsdk-0.5.5.tar.gz` & `tmp/mkmsdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkmsdk-0.5.5.tar", last modified: Mon Aug 23 12:25:20 2021, max compression
+gzip compressed data, was "mkmsdk-0.6.0.tar", last modified: Mon Jul 24 21:35:41 2023, max compression
```

## Comparing `mkmsdk-0.5.5.tar` & `mkmsdk-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alien     (1000) alien     (1000)        0 2021-08-23 12:25:20.076685 mkmsdk-0.5.5/
--rw-r--r--   0 alien     (1000) alien     (1000)     1072 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/LICENSE
--rw-r--r--   0 alien     (1000) alien     (1000)       38 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/MANIFEST.in
--rw-r--r--   0 alien     (1000) alien     (1000)     3895 2021-08-23 12:25:20.076685 mkmsdk-0.5.5/PKG-INFO
--rw-r--r--   0 alien     (1000) alien     (1000)     2877 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/README.rst
-drwxr-xr-x   0 alien     (1000) alien     (1000)        0 2021-08-23 12:25:20.076685 mkmsdk-0.5.5/mkmsdk/
--rw-r--r--   0 alien     (1000) alien     (1000)     1145 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/MKMClient.py
--rw-r--r--   0 alien     (1000) alien     (1000)     1493 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/MKMOAuth1.py
--rw-r--r--   0 alien     (1000) alien     (1000)      153 2021-08-23 12:24:12.000000 mkmsdk-0.5.5/mkmsdk/__init__.py
--rw-r--r--   0 alien     (1000) alien     (1000)     3931 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/api.py
--rw-r--r--   0 alien     (1000) alien     (1000)    25702 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/api_map.py
--rw-r--r--   0 alien     (1000) alien     (1000)     2185 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/exceptions.py
--rw-r--r--   0 alien     (1000) alien     (1000)     1176 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/mkm.py
--rw-r--r--   0 alien     (1000) alien     (1000)     1993 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/resolvers.py
--rw-r--r--   0 alien     (1000) alien     (1000)     1911 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/serializer.py
--rw-r--r--   0 alien     (1000) alien     (1000)      465 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/mkmsdk/utils.py
-drwxr-xr-x   0 alien     (1000) alien     (1000)        0 2021-08-23 12:25:20.076685 mkmsdk-0.5.5/mkmsdk.egg-info/
--rw-r--r--   0 alien     (1000) alien     (1000)     3895 2021-08-23 12:25:19.000000 mkmsdk-0.5.5/mkmsdk.egg-info/PKG-INFO
--rw-r--r--   0 alien     (1000) alien     (1000)      371 2021-08-23 12:25:20.000000 mkmsdk-0.5.5/mkmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 alien     (1000) alien     (1000)        1 2021-08-23 12:25:19.000000 mkmsdk-0.5.5/mkmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 alien     (1000) alien     (1000)       27 2021-08-23 12:25:19.000000 mkmsdk-0.5.5/mkmsdk.egg-info/requires.txt
--rw-r--r--   0 alien     (1000) alien     (1000)        7 2021-08-23 12:25:19.000000 mkmsdk-0.5.5/mkmsdk.egg-info/top_level.txt
--rw-r--r--   0 alien     (1000) alien     (1000)       38 2021-08-23 12:25:20.076685 mkmsdk-0.5.5/setup.cfg
--rw-r--r--   0 alien     (1000) alien     (1000)     2138 2021-08-23 12:14:41.000000 mkmsdk-0.5.5/setup.py
+drwxr-xr-x   0 silvanocerza   (501) staff       (20)        0 2023-07-24 21:35:41.723351 mkmsdk-0.6.0/
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1079 2023-07-24 21:32:13.000000 mkmsdk-0.6.0/LICENSE
+-rw-r--r--   0 silvanocerza   (501) staff       (20)       38 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/MANIFEST.in
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     3838 2023-07-24 21:35:41.723180 mkmsdk-0.6.0/PKG-INFO
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     2840 2023-07-24 21:32:49.000000 mkmsdk-0.6.0/README.md
+drwxr-xr-x   0 silvanocerza   (501) staff       (20)        0 2023-07-24 21:35:41.722201 mkmsdk-0.6.0/mkmsdk/
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1145 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/MKMClient.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1493 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/MKMOAuth1.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)      153 2023-07-24 21:32:57.000000 mkmsdk-0.6.0/mkmsdk/__init__.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     3931 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/api.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)    26324 2023-07-24 20:32:01.000000 mkmsdk-0.6.0/mkmsdk/api_map.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     2185 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/exceptions.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1176 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/mkm.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1993 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/resolvers.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     1911 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/serializer.py
+-rw-r--r--   0 silvanocerza   (501) staff       (20)      465 2023-07-24 19:27:52.000000 mkmsdk-0.6.0/mkmsdk/utils.py
+drwxr-xr-x   0 silvanocerza   (501) staff       (20)        0 2023-07-24 21:35:41.722953 mkmsdk-0.6.0/mkmsdk.egg-info/
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     3838 2023-07-24 21:35:41.000000 mkmsdk-0.6.0/mkmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 silvanocerza   (501) staff       (20)      370 2023-07-24 21:35:41.000000 mkmsdk-0.6.0/mkmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanocerza   (501) staff       (20)        1 2023-07-24 21:35:41.000000 mkmsdk-0.6.0/mkmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanocerza   (501) staff       (20)       27 2023-07-24 21:35:41.000000 mkmsdk-0.6.0/mkmsdk.egg-info/requires.txt
+-rw-r--r--   0 silvanocerza   (501) staff       (20)        7 2023-07-24 21:35:41.000000 mkmsdk-0.6.0/mkmsdk.egg-info/top_level.txt
+-rw-r--r--   0 silvanocerza   (501) staff       (20)       38 2023-07-24 21:35:41.723393 mkmsdk-0.6.0/setup.cfg
+-rw-r--r--   0 silvanocerza   (501) staff       (20)     2131 2023-07-24 21:32:49.000000 mkmsdk-0.6.0/setup.py
```

### Comparing `mkmsdk-0.5.5/LICENSE` & `mkmsdk-0.6.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 The MIT License (MIT)
-Copyright (c) 2015 Evonove
+Copyright (c) 2015 Silvano Cerza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mkmsdk-0.5.5/PKG-INFO` & `mkmsdk-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,118 @@
 Metadata-Version: 2.1
 Name: mkmsdk
-Version: 0.5.5
+Version: 0.6.0
 Summary: MagicKardMarket sdk
-Home-page: https://evonove.it
-Author: Evonove
-Author-email: dev@evonove.it
+Home-page: https://github.com/silvanocerza/mkm-sdk
+Author: Silvano Cerza
 License: MIT
 Keywords: mkm magickardmarket magiccardmarket sdk mtg magic the gathering card market rest tcg trading card game pokemon wow world of warcraft yugioh
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
-Magic Kard Market Python SDK
-============================
+# Magic Kard Market Python SDK
 
-.. image:: https://badge.fury.io/py/mkmsdk.png
-    :target: http://badge.fury.io/py/mkmsdk
+[![image](https://badge.fury.io/py/mkmsdk.png)](http://badge.fury.io/py/mkmsdk)
 
-.. image:: https://readthedocs.org/projects/mkm-sdk/badge/?version=latest
-    :target: http://mkm-sdk.readthedocs.org/en/latest/
+[![image](https://readthedocs.org/projects/mkm-sdk/badge/?version=latest)](http://mkm-sdk.readthedocs.org/en/latest/)
 
-.. image:: https://coveralls.io/repos/evonove/mkm-sdk/badge.svg
-  :target: https://coveralls.io/r/evonove/mkm-sdk
+[![image](https://coveralls.io/repos/evonove/mkm-sdk/badge.svg)](https://coveralls.io/r/evonove/mkm-sdk)
 
-.. image:: https://travis-ci.org/evonove/mkm-sdk.svg
-    :target: https://travis-ci.org/evonove/mkm-sdk
+[![image](https://travis-ci.org/evonove/mkm-sdk.svg)](https://travis-ci.org/evonove/mkm-sdk)
 
-A simple SDK for dedicated and widget apps working with Magic Kard Market.
+A simple SDK for dedicated and widget apps working with Magic Kard
+Market.
 
-Contributing
-============
+# Contributing
 
-Feel free to contribute! Submit `a PR following the guidelines <https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/>`_ and it will be alright.
+Feel free to contribute! Submit [a PR following the
+guidelines](https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/)
+and it will be alright.
 
-Requirements
-============
+# Requirements
 
-* Python 3.4, 3.5, 3.6, 3.7
-* `Requests <http://docs.python-requests.org/>`_
-* `Requests_OAuthlib <https://github.com/requests/requests-oauthlib/>`_
+-   Python 3.8, 3.9, 3.10, 3.11
+-   [Requests](http://docs.python-requests.org/)
+-   [Requests_OAuthlib](https://github.com/requests/requests-oauthlib/)
 
-Setup
-=====
+# Setup
 
-From the command line::
+From the command line:
 
     pip install mkmsdk
 
-For the SDK to work properly you need to create four environment variables holding the tokens necessary to create the
-authorization to make requests. You can find them in your Magic Kard Market account page under the apps section.
+For the SDK to work properly you need to create four environment
+variables holding the tokens necessary to create the authorization to
+make requests. You can find them in your Magic Kard Market account page
+under the apps section.
+
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
 
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+need to be set to empty string if you want to use a widget app.
 
+# Usage
 
-`MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` need to be set to empty string if you want to use a widget app.
-
-Usage
-=====
-
-First thing to do is import the `Mkm` class and the API map::
+First thing to do is import the [Mkm]{.title-ref} class and the API map:
 
     from mkmsdk.mkm import Mkm
     from mkmsdk.api_map import _API_MAP
 
-Instance a new instance of Mkm::
+Instance a new instance of Mkm:
 
     # Using API v1.1
     mkm = Mkm(_API_MAP["1.1"]["api"], _API_MAP["1.1"]["api_root"])
     # Using API v2.0
     mkm = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_root"])
 
-If you want to test on Magic Card Market's sandbox you must use the sandbox root endpoint::
+If you want to test on Magic Card Market\'s sandbox you must use the
+sandbox root endpoint:
 
     mkm_sandbox = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_sandbox_root"])
 
-To make a request::
+To make a request:
 
     response = mkm.account_management.account()
 
     # Formats an endpoint
     response = mkm.market_place.user(user='SampleUser')
 
     # Call endpoint with specified parameters
     response = mkm.account_management.vacation(params={"onVacation": "false"})
 
-
-This will return a `Response <http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/>`_
+This will return a
+[Response](http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/)
 object that contains the response from the server.
 
-Note that only `market_place` requests work when using a widget app.
+Note that only [market_place]{.title-ref} requests work when using a
+widget app.
 
 To get a json you can call response.json().
 
-Tests
-=====
-
-Integration tests will be skipped if the four environment variables are not set.
-
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
-
-Note that some tests will be skipped depending if `MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` are empty strings or not.
+# Tests
 
+Integration tests will be skipped if the four environment variables are
+not set.
 
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
+
+Note that some tests will be skipped depending if
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+are empty strings or not.
```

### Comparing `mkmsdk-0.5.5/README.rst` & `mkmsdk-0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Magic Kard Market Python SDK
-============================
+# Magic Kard Market Python SDK
 
-.. image:: https://badge.fury.io/py/mkmsdk.png
-    :target: http://badge.fury.io/py/mkmsdk
+[![image](https://badge.fury.io/py/mkmsdk.png)](http://badge.fury.io/py/mkmsdk)
 
-.. image:: https://readthedocs.org/projects/mkm-sdk/badge/?version=latest
-    :target: http://mkm-sdk.readthedocs.org/en/latest/
+[![image](https://readthedocs.org/projects/mkm-sdk/badge/?version=latest)](http://mkm-sdk.readthedocs.org/en/latest/)
 
-.. image:: https://coveralls.io/repos/evonove/mkm-sdk/badge.svg
-  :target: https://coveralls.io/r/evonove/mkm-sdk
+[![image](https://coveralls.io/repos/evonove/mkm-sdk/badge.svg)](https://coveralls.io/r/evonove/mkm-sdk)
 
-.. image:: https://travis-ci.org/evonove/mkm-sdk.svg
-    :target: https://travis-ci.org/evonove/mkm-sdk
+[![image](https://travis-ci.org/evonove/mkm-sdk.svg)](https://travis-ci.org/evonove/mkm-sdk)
 
-A simple SDK for dedicated and widget apps working with Magic Kard Market.
+A simple SDK for dedicated and widget apps working with Magic Kard
+Market.
 
-Contributing
-============
+# Contributing
 
-Feel free to contribute! Submit `a PR following the guidelines <https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/>`_ and it will be alright.
+Feel free to contribute! Submit [a PR following the
+guidelines](https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/)
+and it will be alright.
 
-Requirements
-============
+# Requirements
 
-* Python 3.4, 3.5, 3.6, 3.7
-* `Requests <http://docs.python-requests.org/>`_
-* `Requests_OAuthlib <https://github.com/requests/requests-oauthlib/>`_
+-   Python 3.8, 3.9, 3.10, 3.11
+-   [Requests](http://docs.python-requests.org/)
+-   [Requests_OAuthlib](https://github.com/requests/requests-oauthlib/)
 
-Setup
-=====
+# Setup
 
-From the command line::
+From the command line:
 
     pip install mkmsdk
 
-For the SDK to work properly you need to create four environment variables holding the tokens necessary to create the
-authorization to make requests. You can find them in your Magic Kard Market account page under the apps section.
+For the SDK to work properly you need to create four environment
+variables holding the tokens necessary to create the authorization to
+make requests. You can find them in your Magic Kard Market account page
+under the apps section.
+
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
 
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+need to be set to empty string if you want to use a widget app.
 
+# Usage
 
-`MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` need to be set to empty string if you want to use a widget app.
-
-Usage
-=====
-
-First thing to do is import the `Mkm` class and the API map::
+First thing to do is import the [Mkm]{.title-ref} class and the API map:
 
     from mkmsdk.mkm import Mkm
     from mkmsdk.api_map import _API_MAP
 
-Instance a new instance of Mkm::
+Instance a new instance of Mkm:
 
     # Using API v1.1
     mkm = Mkm(_API_MAP["1.1"]["api"], _API_MAP["1.1"]["api_root"])
     # Using API v2.0
     mkm = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_root"])
 
-If you want to test on Magic Card Market's sandbox you must use the sandbox root endpoint::
+If you want to test on Magic Card Market\'s sandbox you must use the
+sandbox root endpoint:
 
     mkm_sandbox = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_sandbox_root"])
 
-To make a request::
+To make a request:
 
     response = mkm.account_management.account()
 
     # Formats an endpoint
     response = mkm.market_place.user(user='SampleUser')
 
     # Call endpoint with specified parameters
     response = mkm.account_management.vacation(params={"onVacation": "false"})
 
-
-This will return a `Response <http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/>`_
+This will return a
+[Response](http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/)
 object that contains the response from the server.
 
-Note that only `market_place` requests work when using a widget app.
+Note that only [market_place]{.title-ref} requests work when using a
+widget app.
 
 To get a json you can call response.json().
 
-Tests
-=====
-
-Integration tests will be skipped if the four environment variables are not set.
+# Tests
 
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
+Integration tests will be skipped if the four environment variables are
+not set.
 
-Note that some tests will be skipped depending if `MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` are empty strings or not.
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
+
+Note that some tests will be skipped depending if
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+are empty strings or not.
```

### Comparing `mkmsdk-0.5.5/mkmsdk/MKMClient.py` & `mkmsdk-0.6.0/mkmsdk/MKMClient.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/MKMOAuth1.py` & `mkmsdk-0.6.0/mkmsdk/MKMOAuth1.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/api.py` & `mkmsdk-0.6.0/mkmsdk/api.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/api_map.py` & `mkmsdk-0.6.0/mkmsdk/api_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,24 @@
                     "description": "Searches users matching the given search string",
                 },
                 "user_articles": {
                     "url": "/users/{user}/articles",
                     "method": "get",
                     "description": "Returns all available articles for the specified user",
                 },
+                "create_export_user_offers": {
+                    "url": "/exports/userOffers/{user}",
+                    "method": "post",
+                    "description": "Request the export of Article entities for available articles from a specific user specified by its ID.",
+                },
+                "get_export_user_offers": {
+                    "url": "/exports/userOffers/{user}",
+                    "method": "get",
+                    "description": "Returns details for a requested export of Article entities for available articles from a specific user specified by its ID.",
+                },
             },
             "order_management": {
                 "get_order": {
                     "url": "/order/{order}",
                     "method": "get",
                     "description": "Returns an order specified by its ID",
                 },
```

### Comparing `mkmsdk-0.5.5/mkmsdk/exceptions.py` & `mkmsdk-0.6.0/mkmsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/mkm.py` & `mkmsdk-0.6.0/mkmsdk/mkm.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/resolvers.py` & `mkmsdk-0.6.0/mkmsdk/resolvers.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk/serializer.py` & `mkmsdk-0.6.0/mkmsdk/serializer.py`

 * *Files identical despite different names*

### Comparing `mkmsdk-0.5.5/mkmsdk.egg-info/PKG-INFO` & `mkmsdk-0.6.0/mkmsdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,118 @@
 Metadata-Version: 2.1
 Name: mkmsdk
-Version: 0.5.5
+Version: 0.6.0
 Summary: MagicKardMarket sdk
-Home-page: https://evonove.it
-Author: Evonove
-Author-email: dev@evonove.it
+Home-page: https://github.com/silvanocerza/mkm-sdk
+Author: Silvano Cerza
 License: MIT
 Keywords: mkm magickardmarket magiccardmarket sdk mtg magic the gathering card market rest tcg trading card game pokemon wow world of warcraft yugioh
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
-Magic Kard Market Python SDK
-============================
+# Magic Kard Market Python SDK
 
-.. image:: https://badge.fury.io/py/mkmsdk.png
-    :target: http://badge.fury.io/py/mkmsdk
+[![image](https://badge.fury.io/py/mkmsdk.png)](http://badge.fury.io/py/mkmsdk)
 
-.. image:: https://readthedocs.org/projects/mkm-sdk/badge/?version=latest
-    :target: http://mkm-sdk.readthedocs.org/en/latest/
+[![image](https://readthedocs.org/projects/mkm-sdk/badge/?version=latest)](http://mkm-sdk.readthedocs.org/en/latest/)
 
-.. image:: https://coveralls.io/repos/evonove/mkm-sdk/badge.svg
-  :target: https://coveralls.io/r/evonove/mkm-sdk
+[![image](https://coveralls.io/repos/evonove/mkm-sdk/badge.svg)](https://coveralls.io/r/evonove/mkm-sdk)
 
-.. image:: https://travis-ci.org/evonove/mkm-sdk.svg
-    :target: https://travis-ci.org/evonove/mkm-sdk
+[![image](https://travis-ci.org/evonove/mkm-sdk.svg)](https://travis-ci.org/evonove/mkm-sdk)
 
-A simple SDK for dedicated and widget apps working with Magic Kard Market.
+A simple SDK for dedicated and widget apps working with Magic Kard
+Market.
 
-Contributing
-============
+# Contributing
 
-Feel free to contribute! Submit `a PR following the guidelines <https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/>`_ and it will be alright.
+Feel free to contribute! Submit [a PR following the
+guidelines](https://mkm-sdk.readthedocs.io/en/latest/contributing.html#pull-request-guidelines/)
+and it will be alright.
 
-Requirements
-============
+# Requirements
 
-* Python 3.4, 3.5, 3.6, 3.7
-* `Requests <http://docs.python-requests.org/>`_
-* `Requests_OAuthlib <https://github.com/requests/requests-oauthlib/>`_
+-   Python 3.8, 3.9, 3.10, 3.11
+-   [Requests](http://docs.python-requests.org/)
+-   [Requests_OAuthlib](https://github.com/requests/requests-oauthlib/)
 
-Setup
-=====
+# Setup
 
-From the command line::
+From the command line:
 
     pip install mkmsdk
 
-For the SDK to work properly you need to create four environment variables holding the tokens necessary to create the
-authorization to make requests. You can find them in your Magic Kard Market account page under the apps section.
+For the SDK to work properly you need to create four environment
+variables holding the tokens necessary to create the authorization to
+make requests. You can find them in your Magic Kard Market account page
+under the apps section.
+
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
 
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+need to be set to empty string if you want to use a widget app.
 
+# Usage
 
-`MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` need to be set to empty string if you want to use a widget app.
-
-Usage
-=====
-
-First thing to do is import the `Mkm` class and the API map::
+First thing to do is import the [Mkm]{.title-ref} class and the API map:
 
     from mkmsdk.mkm import Mkm
     from mkmsdk.api_map import _API_MAP
 
-Instance a new instance of Mkm::
+Instance a new instance of Mkm:
 
     # Using API v1.1
     mkm = Mkm(_API_MAP["1.1"]["api"], _API_MAP["1.1"]["api_root"])
     # Using API v2.0
     mkm = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_root"])
 
-If you want to test on Magic Card Market's sandbox you must use the sandbox root endpoint::
+If you want to test on Magic Card Market\'s sandbox you must use the
+sandbox root endpoint:
 
     mkm_sandbox = Mkm(_API_MAP["2.0"]["api"], _API_MAP["2.0"]["api_sandbox_root"])
 
-To make a request::
+To make a request:
 
     response = mkm.account_management.account()
 
     # Formats an endpoint
     response = mkm.market_place.user(user='SampleUser')
 
     # Call endpoint with specified parameters
     response = mkm.account_management.vacation(params={"onVacation": "false"})
 
-
-This will return a `Response <http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/>`_
+This will return a
+[Response](http://docs.python-requests.org/en/latest/api/?highlight=response#requests.Response/)
 object that contains the response from the server.
 
-Note that only `market_place` requests work when using a widget app.
+Note that only [market_place]{.title-ref} requests work when using a
+widget app.
 
 To get a json you can call response.json().
 
-Tests
-=====
-
-Integration tests will be skipped if the four environment variables are not set.
-
-* ``MKM_APP_TOKEN``
-* ``MKM_APP_SECRET``
-* ``MKM_ACCESS_TOKEN``
-* ``MKM_ACCESS_TOKEN_SECRET``
-
-Note that some tests will be skipped depending if `MKM_ACCESS_TOKEN` and `MKM_ACCESS_TOKEN_SECRET` are empty strings or not.
+# Tests
 
+Integration tests will be skipped if the four environment variables are
+not set.
 
+-   `MKM_APP_TOKEN`
+-   `MKM_APP_SECRET`
+-   `MKM_ACCESS_TOKEN`
+-   `MKM_ACCESS_TOKEN_SECRET`
+
+Note that some tests will be skipped depending if
+[MKM_ACCESS_TOKEN]{.title-ref} and [MKM_ACCESS_TOKEN_SECRET]{.title-ref}
+are empty strings or not.
```

### Comparing `mkmsdk-0.5.5/setup.py` & `mkmsdk-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     init_py = open(os.path.join(package, "__init__.py")).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 
 version = get_version("mkmsdk")
 
 
-LONG_DESCRIPTION = open("README.rst").read()
+LONG_DESCRIPTION = open("README.md").read()
 
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     print("You probably want to also tag the version now:")
     print(" git tag -a %s -m '%s'" % (version, version))
@@ -48,33 +48,32 @@
         "yugioh",
     ]
 )
 
 setup(
     name="mkmsdk",
     version=version,
-    author="Evonove",
-    author_email="dev@evonove.it",
+    author="Silvano Cerza",
     packages=find_packages(exclude=["docs", "tests*"]),
     scripts=[],
-    url="https://evonove.it",
+    url="https://github.com/silvanocerza/mkm-sdk",
     license="MIT",
     description="MagicKardMarket sdk",
     long_description=LONG_DESCRIPTION,
     install_requires=["requests", "requests_oauthlib"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords=keywords,
 )
```

