# Comparing `tmp/lacuscore-1.6.2.tar.gz` & `tmp/lacuscore-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.6.2.tar", max compression
+gzip compressed data, was "lacuscore-1.6.3.tar", max compression
```

## Comparing `lacuscore-1.6.2.tar` & `lacuscore-1.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.6.2/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.6.2/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.6.2/lacuscore/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-27 10:03:30.510884 lacuscore-1.6.2/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    33491 2023-06-27 10:02:06.046544 lacuscore-1.6.2/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.6.2/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-07-18 08:32:48.882765 lacuscore-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.6.3/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.6.3/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.6.3/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-27 10:03:30.510884 lacuscore-1.6.3/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    33726 2023-07-24 10:22:32.223630 lacuscore-1.6.3/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.6.3/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-07-24 10:23:04.363799 lacuscore-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.6.3/PKG-INFO
```

### Comparing `lacuscore-1.6.2/LICENSE` & `lacuscore-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.2/README.md` & `lacuscore-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.2/lacuscore/lacus_monitoring.py` & `lacuscore-1.6.3/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.2/lacuscore/lacuscore.py` & `lacuscore-1.6.3/lacuscore/lacuscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,40 +502,40 @@
                 result = {'error': f'No valid URL to capture for {uuid} - {to_capture}'}
                 raise CaptureError
 
             splitted_url = urlsplit(url)
             proxy = to_capture.get('proxy')
             if self.tor_proxy:
                 # check if onion or forced
-                if (proxy == 'force_tor'
-                        or (not proxy
+                if (proxy == 'force_tor'  # if the proxy is set to "force_tor", we use the pre-configured tor proxy, regardless the URL.
+                        or (not proxy  # if the TLD is "onion", we use the pre-configured tor proxy
                             and splitted_url.netloc
                             and splitted_url.hostname
                             and splitted_url.hostname.split('.')[-1] == 'onion')):
                     proxy = self.tor_proxy
 
             if self.only_global_lookups and not proxy and splitted_url.scheme not in ['data', 'file']:
                 # not relevant if we also have a proxy, or the thing to capture is a data URI or a file on disk
                 if splitted_url.netloc:
                     if splitted_url.hostname and splitted_url.hostname.split('.')[-1] != 'onion':
                         try:
                             ips_info = socket.getaddrinfo(splitted_url.hostname, None, proto=socket.IPPROTO_TCP)
                         except socket.gaierror:
-                            logger.debug(f'Unable to resolve {splitted_url.hostname}.')
-                            result = {'error': f'Unable to resolve {splitted_url.hostname}.'}
+                            logger.debug(f'Unable to resolve "{splitted_url.hostname}" - Original URL: "{url}".')
+                            result = {'error': f'Unable to resolve "{splitted_url.hostname}" - Original URL: "{url}".'}
                             raise RetryCapture
                         except Exception as e:
-                            result = {'error': f'Issue with hostname resolution ({splitted_url.hostname}): {e}.'}
+                            result = {'error': f'Issue with hostname resolution ({splitted_url.hostname}): {e}. Original URL: "{url}".'}
                             raise CaptureError
                         for info in ips_info:
                             if not ipaddress.ip_address(info[-1][0]).is_global:
                                 result = {'error': f'Capturing ressources on private IPs {info[-1][0]} is disabled.'}
                                 raise CaptureError
                 else:
-                    result = {'error': f'Unable to find hostname or IP in the query: {url}.'}
+                    result = {'error': f'Unable to find hostname or IP in the query: "{url}".'}
                     raise CaptureError
 
             browser_engine: BROWSER = "chromium"
             if to_capture.get('user_agent'):
                 parsed_string = user_agent_parser.ParseUserAgent(to_capture.get('user_agent'))
                 browser_family = parsed_string['family'].lower()
                 if browser_family.startswith('chrom'):
```

### Comparing `lacuscore-1.6.2/pyproject.toml` & `lacuscore-1.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.6.2"
+version = "1.6.3"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -37,17 +37,17 @@
 ua-parser = "^0.18.0"
 redis = {version = "^4.6.0", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.6.0.2"}
+types-redis = {version = "^4.6.0.3"}
 mypy = "^1.4.1"
-types-requests = "^2.31.0.1"
+types-requests = "^2.31.0.2"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
 pytest = "^7.4.0"
 
 [build-system]
```

### Comparing `lacuscore-1.6.2/PKG-INFO` & `lacuscore-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.6.2
+Version: 1.6.3
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

