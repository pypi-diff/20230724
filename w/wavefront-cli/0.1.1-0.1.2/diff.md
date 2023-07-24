# Comparing `tmp/wavefront-cli-0.1.1.tar.gz` & `tmp/wavefront-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavefront-cli-0.1.1.tar", last modified: Mon Jul  3 09:58:40 2023, max compression
+gzip compressed data, was "wavefront-cli-0.1.2.tar", last modified: Mon Jul 24 15:36:05 2023, max compression
```

## Comparing `wavefront-cli-0.1.1.tar` & `wavefront-cli-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.487782 wavefront-cli-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.487782 wavefront-cli-0.1.1/wavefront_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.487782 wavefront-cli-0.1.1/wavefront_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/commands/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/wavefront_cli/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/integrations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/integrations/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/integrations/statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/integrations/wavefront.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/wavefront_cli/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 09:58:13.000000 wavefront-cli-0.1.1/wavefront_cli/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:58:40.491782 wavefront-cli-0.1.1/wavefront_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-03 09:58:40.000000 wavefront-cli-0.1.1/wavefront_cli.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 15:36:05.797507 wavefront-cli-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.789507 wavefront-cli-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.789507 wavefront-cli-0.1.2/wavefront_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/wavefront_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/commands/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/wavefront_cli/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/integrations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/integrations/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/integrations/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/integrations/wavefront.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/wavefront_cli/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-24 15:35:30.000000 wavefront-cli-0.1.2/wavefront_cli/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:05.793507 wavefront-cli-0.1.2/wavefront_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 15:36:05.000000 wavefront-cli-0.1.2/wavefront_cli.egg-info/SOURCES.txt
```

### Comparing `wavefront-cli-0.1.1/LICENSE` & `wavefront-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/PKG-INFO` & `wavefront-cli-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavefront-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: VMware Aria Operations for Applications CLI Utility.
 Home-page: https://github.com/wavefrontHQ/wavefront-cli
 Author: VMware Aria Operations for Applications Team
 Author-email: chitimba@wavefront.com
 License: APACHE-V2
 Keywords: apps,cli,lib,observability,ops,wavefront
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wavefront-cli-0.1.1/setup.py` & `wavefront-cli-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         errno = subprocess.call(['py.test', '--cov=wave',
                                  '--cov-report=term-missing'])
         raise SystemExit(errno)
 
 
 setuptools.setup(
     name='wavefront-cli',
-    version='0.1.1',
+    version='0.1.2',
     description='VMware Aria Operations for Applications CLI Utility.',
     long_description=long_description,
     url='https://github.com/wavefrontHQ/wavefront-cli',
     author='VMware Aria Operations for Applications Team',
     author_email='chitimba@wavefront.com',
     license='APACHE-V2',
     classifiers=[
```

### Comparing `wavefront-cli-0.1.1/tests/test_cli.py` & `wavefront-cli-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/cli.py` & `wavefront-cli-0.1.2/wavefront_cli/cli.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/commands/install.py` & `wavefront-cli-0.1.2/wavefront_cli/commands/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                                   " [default: no]: \n").lower()
                 aws = bool(aws_input.lower() in ("y", "yes"))
 
         if proxy:
             if not wavefront_url:
                 wavefront_url = input("Please enter the url to your Wavefront"
                                       " instance (default = "
-                                      "https://try.wavefront.com): \n")\
+                                      "https://try.wavefront.com): \n") \
                                 or "https://try.wavefront.com"
 
             auth_type = False
             if csp_org_id and csp_app_id and csp_app_secret:
                 auth_type = True
             elif csp_api_token:
                 auth_type = True
@@ -142,14 +142,30 @@
                 print("Error: Invalid combination of parameters.")
                 sys.exit(1)
 
             # Install Proxy
             if not lib.proxy.install_proxy(proxy_next):
                 sys.exit(1)
 
+            if csp_org_id and csp_app_id and csp_app_secret:
+                lib.configure_csp_oauth_options()
+                lib.comment_auth_methods(csp_api_token=True,
+                                         csp_oauth_app=False,
+                                         wavefront_api_token=True)
+            elif csp_api_token:
+                lib.configure_csp_api_token_options()
+                lib.comment_auth_methods(csp_api_token=False,
+                                         csp_oauth_app=True,
+                                         wavefront_api_token=True)
+            elif wavefront_api_token:
+                lib.configure_wavefront_api_token_options()
+                lib.comment_auth_methods(csp_api_token=True,
+                                         csp_oauth_app=True,
+                                         wavefront_api_token=False)
+
             # Configure Proxy
             if not lib.proxy.configure_proxy(wavefront_url,
                                              wavefront_api_token,
                                              csp_api_token,
                                              csp_app_id,
                                              csp_app_secret,
                                              csp_org_id):
@@ -159,15 +175,15 @@
             # required agent options
             if not proxy_address:
                 proxy_address = input("Please enter the address to your"
                                       " Wavefront proxy (default = "
                                       "localhost): \n") or "localhost"
             if not proxy_port:
                 proxy_port = input("Please enter the port of your"
-                                   " Wavefront proxy (default = 2878): \n")\
+                                   " Wavefront proxy (default = 2878): \n") \
                              or "2878"
 
             # Install the Wf integration first (Telegraf won't start
             # if an output plugin is not already created
             # Configure Wavefront Integration
             wf_opts = {}
             wf_opts["proxy_address"] = proxy_address
```

### Comparing `wavefront-cli-0.1.1/wavefront_cli/commands/integration.py` & `wavefront-cli-0.1.2/wavefront_cli/commands/integration.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/integrations/base.py` & `wavefront-cli-0.1.2/wavefront_cli/integrations/base.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/integrations/example.py` & `wavefront-cli-0.1.2/wavefront_cli/integrations/example.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/integrations/statsd.py` & `wavefront-cli-0.1.2/wavefront_cli/integrations/statsd.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/integrations/wavefront.py` & `wavefront-cli-0.1.2/wavefront_cli/integrations/wavefront.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/agent.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/agent.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/api.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/api.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/auth.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/auth.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/aws.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/aws.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/message.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/message.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/system.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/system.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli/lib/util.py` & `wavefront-cli-0.1.2/wavefront_cli/lib/util.py`

 * *Files identical despite different names*

### Comparing `wavefront-cli-0.1.1/wavefront_cli.egg-info/SOURCES.txt` & `wavefront-cli-0.1.2/wavefront_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

