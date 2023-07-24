# Comparing `tmp/apimatic-core-interfaces-0.1.3.tar.gz` & `tmp/apimatic-core-interfaces-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-core-interfaces-0.1.3.tar", last modified: Tue Apr  4 08:47:27 2023, max compression
+gzip compressed data, was "apimatic-core-interfaces-0.1.4.tar", last modified: Mon Jul 24 06:43:23 2023, max compression
```

## Comparing `apimatic-core-interfaces-0.1.3.tar` & `apimatic-core-interfaces-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.695248 apimatic-core-interfaces-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/client/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/factories/response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/types/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/types/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/types/http_method_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:27.691248 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-04 08:47:27.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-04 08:47:27.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:47:27.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 08:47:27.000000 apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:47:27.695248 apimatic-core-interfaces-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-04 08:47:10.000000 apimatic-core-interfaces-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/http_method_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/union_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/setup.py
```

### Comparing `apimatic-core-interfaces-0.1.3/LICENSE` & `apimatic-core-interfaces-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.3/PKG-INFO` & `apimatic-core-interfaces-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core-interfaces
-Version: 0.1.3
+Version: 0.1.4
 Summary: An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter and APIMatic SDKs.
 Home-page: https://github.com/apimatic/core-interfaces-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,19 +22,20 @@
 ## Installation 
 Simply run the command below in your SDK as the apimatic-core-interfaces will be added as a dependency in the SDK.
 ```python
 pip install apimatic-core-interfaces
 ```
 
 ## Interfaces
-| Name                                                                       | Description                                                                              |
-|--------------------------------------------------------------------------- |------------------------------------------------------------------------------------------|
-| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)             | To save both Request and Response after the completion of response                         |
-| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py)| To convert the client-adapter response into a custom HTTP response                       |
-| [`Authentication`](apimatic_core_interfaces/types/authentication.py)       | To setup methods for the validation and application of the required authentication scheme|
+| Name                                                                        | Description                                                                               |
+|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
+| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
+| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
+| [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
+| [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
 
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
```

### Comparing `apimatic-core-interfaces-0.1.3/README.md` & `apimatic-core-interfaces-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 ## Installation 
 Simply run the command below in your SDK as the apimatic-core-interfaces will be added as a dependency in the SDK.
 ```python
 pip install apimatic-core-interfaces
 ```
 
 ## Interfaces
-| Name                                                                       | Description                                                                              |
-|--------------------------------------------------------------------------- |------------------------------------------------------------------------------------------|
-| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)             | To save both Request and Response after the completion of response                         |
-| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py)| To convert the client-adapter response into a custom HTTP response                       |
-| [`Authentication`](apimatic_core_interfaces/types/authentication.py)       | To setup methods for the validation and application of the required authentication scheme|
+| Name                                                                        | Description                                                                               |
+|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
+| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
+| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
+| [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
+| [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
 
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
```

### Comparing `apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/client/http_client.py` & `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/http_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.3/apimatic_core_interfaces/types/http_method_enum.py` & `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/PKG-INFO` & `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core-interfaces
-Version: 0.1.3
+Version: 0.1.4
 Summary: An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter and APIMatic SDKs.
 Home-page: https://github.com/apimatic/core-interfaces-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,19 +22,20 @@
 ## Installation 
 Simply run the command below in your SDK as the apimatic-core-interfaces will be added as a dependency in the SDK.
 ```python
 pip install apimatic-core-interfaces
 ```
 
 ## Interfaces
-| Name                                                                       | Description                                                                              |
-|--------------------------------------------------------------------------- |------------------------------------------------------------------------------------------|
-| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)             | To save both Request and Response after the completion of response                         |
-| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py)| To convert the client-adapter response into a custom HTTP response                       |
-| [`Authentication`](apimatic_core_interfaces/types/authentication.py)       | To setup methods for the validation and application of the required authentication scheme|
+| Name                                                                        | Description                                                                               |
+|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
+| [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
+| [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
+| [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
+| [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
 
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
```

### Comparing `apimatic-core-interfaces-0.1.3/apimatic_core_interfaces.egg-info/SOURCES.txt` & `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 apimatic_core_interfaces.egg-info/top_level.txt
 apimatic_core_interfaces/client/__init__.py
 apimatic_core_interfaces/client/http_client.py
 apimatic_core_interfaces/factories/__init__.py
 apimatic_core_interfaces/factories/response_factory.py
 apimatic_core_interfaces/types/__init__.py
 apimatic_core_interfaces/types/authentication.py
-apimatic_core_interfaces/types/http_method_enum.py
+apimatic_core_interfaces/types/http_method_enum.py
+apimatic_core_interfaces/types/union_type.py
```

### Comparing `apimatic-core-interfaces-0.1.3/setup.py` & `apimatic-core-interfaces-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-core-interfaces',
-    version='0.1.3',
+    version='0.1.4',
     description='An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter '
                 'and APIMatic SDKs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
```

