# Comparing `tmp/dotstat_io-0.1.3.tar.gz` & `tmp/dotstat_io-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstat_io-0.1.3.tar", max compression
+gzip compressed data, was "dotstat_io-0.1.4.tar", max compression
```

## Comparing `dotstat_io-0.1.3.tar` & `dotstat_io-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.3/dotstat_io/__init__.py
--rw-r--r--   0        0        0    10527 2023-06-21 07:52:47.915175 dotstat_io-0.1.3/dotstat_io/authentication.py
--rw-r--r--   0        0        0    10098 2023-06-27 13:03:05.856024 dotstat_io-0.1.3/dotstat_io/download_upload.py
--rw-r--r--   0        0        0      610 2023-06-27 13:10:52.656847 dotstat_io-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5862 2023-06-22 09:57:29.580014 dotstat_io-0.1.3/README.md
--rw-r--r--   0        0        0     6411 1970-01-01 00:00:00.000000 dotstat_io-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.4/dotstat_io/__init__.py
+-rw-r--r--   0        0        0    10527 2023-06-21 07:52:47.915175 dotstat_io-0.1.4/dotstat_io/authentication.py
+-rw-r--r--   0        0        0    10097 2023-07-24 07:51:33.397995 dotstat_io-0.1.4/dotstat_io/download_upload.py
+-rw-r--r--   0        0        0      610 2023-07-24 08:00:18.259100 dotstat_io-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5856 2023-07-19 12:28:12.511143 dotstat_io-0.1.4/README.md
+-rw-r--r--   0        0        0     6405 1970-01-01 00:00:00.000000 dotstat_io-0.1.4/PKG-INFO
```

### Comparing `dotstat_io-0.1.3/dotstat_io/authentication.py` & `dotstat_io-0.1.4/dotstat_io/authentication.py`

 * *Files identical despite different names*

### Comparing `dotstat_io-0.1.3/dotstat_io/download_upload.py` & `dotstat_io-0.1.4/dotstat_io/download_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                 'id': requestId
             }
 
             transfer_url = transfer_url.replace("import", "status")
             transfer_url = transfer_url.replace("sdmxFile", "request")
 
             response = requests.post(
-                transfer_url, verify=False, headers=headers, data=payload)
+                transfer_url, verify=True, headers=headers, data=payload)
 
         except Exception as err:
             Returned_Message = self.__ERROR  + str(err)
         else:
             if response.status_code != 200:
                 Returned_Message = self.__ERROR  + 'Error code: ' + \
                     str(response.status_code) + ' Reason: ' + str(response.reason)
```

### Comparing `dotstat_io-0.1.3/pyproject.toml` & `dotstat_io-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dotstat_io"
-version = "0.1.3"
+version = "0.1.4"
 description = "Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it"
 license = "MIT"
 authors = ["Gyorgy Gyomai <gyorgy.gyomai@oecd.org>", "Abdel Aliaoui <abdel.aliaoui@oecd.org>"]
 readme = "README.md"
 packages = [{include = "dotstat_io"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dotstat_io-0.1.3/README.md` & `dotstat_io-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         scopes=scopes,
         authority_url=authority_url,
         redirect_port=redirect_port) as Interactive_obj:
     token = Interactive_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `scopes:` Scopes requested to access a protected API (a resource defined by sdmx_resource_id)
 * `authority_url:` URL that identifies a token authority
 * `redirect_port:` The port of the address to return to upon receiving a response from the authority
 
 #### 2. To initialise the module for non-interactive use using a secret: 
 ```python
@@ -33,30 +33,30 @@
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         scopes=scopes,
         authority_url=authority_url,
         client_secret=client_secret) as Nointeractive_with_secret_obj:
     token = Nointeractive_with_secret_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `scopes:` Scopes requested to access a protected API (a resource defined by sdmx_resource_id)
 * `authority_url:` URL that identifies a token authority
 * `client_secret:` The application secret that you created during app registration in ADFS
 
 #### 3. To initialise the module for non-interactive use using windows client authentication:
 ```python
 from dotstat_io.authentication import AdfsAuthentication
 with AdfsAuthentication.nointeractive_with_adfs(
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         token_url=token_url) as Nointeractive_with_adfs_obj:
     token = Nointeractive_with_adfs_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `token_url:` URL of the authentication service
 
 #### 4. To get a token after initialisation of "AdfsAuthentication" object as shown above: 
 ```python
 token = [Authentication Object Name].get_token()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dotstat_io-0.1.3/PKG-INFO` & `dotstat_io-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstat-io
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it
 License: MIT
 Author: Gyorgy Gyomai
 Author-email: gyorgy.gyomai@oecd.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         scopes=scopes,
         authority_url=authority_url,
         redirect_port=redirect_port) as Interactive_obj:
     token = Interactive_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `scopes:` Scopes requested to access a protected API (a resource defined by sdmx_resource_id)
 * `authority_url:` URL that identifies a token authority
 * `redirect_port:` The port of the address to return to upon receiving a response from the authority
 
 #### 2. To initialise the module for non-interactive use using a secret: 
 ```python
@@ -51,30 +51,30 @@
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         scopes=scopes,
         authority_url=authority_url,
         client_secret=client_secret) as Nointeractive_with_secret_obj:
     token = Nointeractive_with_secret_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `scopes:` Scopes requested to access a protected API (a resource defined by sdmx_resource_id)
 * `authority_url:` URL that identifies a token authority
 * `client_secret:` The application secret that you created during app registration in ADFS
 
 #### 3. To initialise the module for non-interactive use using windows client authentication:
 ```python
 from dotstat_io.authentication import AdfsAuthentication
 with AdfsAuthentication.nointeractive_with_adfs(
         client_id=client_id,
         sdmx_resource_id=sdmx_resource_id,
         token_url=token_url) as Nointeractive_with_adfs_obj:
     token = Nointeractive_with_adfs_obj.get_token()
 ```
-* `client_id:` The Application (client) ID that the ADFS assigned to your app
+* `client_id:` The Application (client) ID that the ADFS assigned to your app
 * `sdmx_resource_id:` The ID of the application to be accessed such as .Stat Suite PP
 * `token_url:` URL of the authentication service
 
 #### 4. To get a token after initialisation of "AdfsAuthentication" object as shown above: 
 ```python
 token = [Authentication Object Name].get_token()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

