# Comparing `tmp/certbot-dns-gcore-0.1.7.tar.gz` & `tmp/certbot-dns-gcore-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-gcore-0.1.7.tar", last modified: Tue Aug 23 08:51:40 2022, max compression
+gzip compressed data, was "certbot-dns-gcore-0.1.8.tar", last modified: Mon Jul 24 15:21:22 2023, max compression
```

## Comparing `certbot-dns-gcore-0.1.7.tar` & `certbot-dns-gcore-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 08:51:40.655123 certbot-dns-gcore-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-08-23 08:51:40.655123 certbot-dns-gcore-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5427 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 08:51:40.655123 certbot-dns-gcore-0.1.7/certbot_dns_gcore/
--rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore/api_gcore.py
--rw-r--r--   0 runner    (1001) docker     (121)     8210 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore/dns_gcore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 08:51:40.655123 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-23 08:51:40.000000 certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-23 08:51:40.659123 certbot-dns-gcore-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 08:51:40.655123 certbot-dns-gcore-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-23 08:51:26.000000 certbot-dns-gcore-0.1.7/tests/test_dns_gcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:21:22.349837 certbot-dns-gcore-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-24 15:21:22.349837 certbot-dns-gcore-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:21:22.345837 certbot-dns-gcore-0.1.8/certbot_dns_gcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore/api_gcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore/dns_gcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:21:22.349837 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:21:22.000000 certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 15:21:22.349837 certbot-dns-gcore-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:21:22.349837 certbot-dns-gcore-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-24 15:21:02.000000 certbot-dns-gcore-0.1.8/tests/test_dns_gcore.py
```

### Comparing `certbot-dns-gcore-0.1.7/PKG-INFO` & `certbot-dns-gcore-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-gcore
-Version: 0.1.7
+Version: 0.1.8
 Summary: G-Core DNS Authenticator plugin for Certbot
 Home-page: https://github.com/G-Core/gcore-dns-certbot-plugin
 Author: G-Core Labs
 Author-email: support@gcorelabs.com
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `certbot-dns-gcore-0.1.7/README.md` & `certbot-dns-gcore-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-gcore-0.1.7/certbot_dns_gcore/__init__.py` & `certbot-dns-gcore-0.1.8/certbot_dns_gcore/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gcore-0.1.7/certbot_dns_gcore/api_gcore.py` & `certbot-dns-gcore-0.1.8/certbot_dns_gcore/api_gcore.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     """G-Core DNS API conflict exception."""
 
 
 class GCoreClient:
     """G-Core DNS API client."""
 
     _root_zones = 'v2/zones'
-    _dns_api_url = 'https://api.gcorelabs.com/dns'
-    _auth_url = 'https://api.gcorelabs.com/iam'
+    _dns_api_url = 'https://api.gcore.com/dns'
+    _auth_url = 'https://api.gcore.com/iam'
     _timeout = 10.0
     _error_format = 'Error %s. %s: %r, data: "%r", response: %s'
 
     def __init__(self, token=None, login=None, password=None, api_url=None, dns_api_url=None, auth_url=None):
         self._session = Session()
         if token is not None:
             self._session.headers.update({'Authorization': f'APIKey {token}'})
```

### Comparing `certbot-dns-gcore-0.1.7/certbot_dns_gcore/dns_gcore.py` & `certbot-dns-gcore-0.1.8/certbot_dns_gcore/dns_gcore.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gcore-0.1.7/certbot_dns_gcore.egg-info/PKG-INFO` & `certbot-dns-gcore-0.1.8/certbot_dns_gcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-gcore
-Version: 0.1.7
+Version: 0.1.8
 Summary: G-Core DNS Authenticator plugin for Certbot
 Home-page: https://github.com/G-Core/gcore-dns-certbot-plugin
 Author: G-Core Labs
 Author-email: support@gcorelabs.com
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `certbot-dns-gcore-0.1.7/setup.py` & `certbot-dns-gcore-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gcore-0.1.7/tests/conftest.py` & `certbot-dns-gcore-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gcore-0.1.7/tests/test_dns_gcore.py` & `certbot-dns-gcore-0.1.8/tests/test_dns_gcore.py`

 * *Files identical despite different names*

