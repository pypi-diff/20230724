# Comparing `tmp/podman-4.5.1.tar.gz` & `tmp/podman-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podman-4.5.1.tar", last modified: Wed May 31 15:45:46 2023, max compression
+gzip compressed data, was "podman-4.6.0.tar", last modified: Mon Jul 24 12:53:29 2023, max compression
```

## Comparing `podman-4.5.1.tar` & `podman-4.6.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.201281 podman-4.5.1/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.5.1/LICENSE
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-05-31 15:45:46.201281 podman-4.5.1/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.5.1/README.md
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.194281 podman-4.5.1/podman/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.5.1/podman/__init__.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.197281 podman-4.5.1/podman/api/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/adapter_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/cached_property.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/client.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/http_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3270 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/parse_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9974 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/ssh.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/tar_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109033 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/typing_extensions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5976 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/uds.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8640 2023-04-27 13:32:41.000000 podman-4.5.1/podman/client.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.200281 podman-4.5.1/podman/domain/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3720 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/config.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    18880 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/containers.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    31505 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/containers_create.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5405 2023-02-07 13:10:19.000000 podman-4.5.1/podman/domain/containers_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-02-07 13:10:19.000000 podman-4.5.1/podman/domain/containers_run.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/events.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/images.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/images_build.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14363 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/images_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/ipam.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/manifests.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/networks.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6920 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/networks_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/pods.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5465 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/pods_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/registry_data.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/secrets.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/system.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/volumes.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.200281 podman-4.5.1/podman/errors/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.5.1/podman/errors/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.5.1/podman/errors/exceptions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.5.1/podman/tlsconfig.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-05-31 15:05:01.000000 podman-4.5.1/podman/version.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.195281 podman-4.5.1/podman.egg-info/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-05-31 15:45:45.000000 podman-4.5.1/podman.egg-info/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/SOURCES.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-05-31 15:45:45.000000 podman-4.5.1/podman.egg-info/dependency_links.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       91 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/requires.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/top_level.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      662 2023-04-27 13:32:41.000000 podman-4.5.1/pyproject.toml
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1323 2023-05-31 15:45:46.201281 podman-4.5.1/setup.cfg
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.5.1/setup.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.174663 podman-4.6.0/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.6.0/LICENSE
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-07-24 12:53:29.175663 podman-4.6.0/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.6.0/README.md
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.171663 podman-4.6.0/podman/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.6.0/podman/__init__.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.172663 podman-4.6.0/podman/api/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2023-06-05 14:48:42.000000 podman-4.6.0/podman/api/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.6.0/podman/api/adapter_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.6.0/podman/api/cached_property.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.6.0/podman/api/client.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.6.0/podman/api/http_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3270 2023-06-05 14:48:42.000000 podman-4.6.0/podman/api/parse_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9917 2023-07-03 15:23:31.000000 podman-4.6.0/podman/api/ssh.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.6.0/podman/api/tar_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109033 2023-06-05 14:48:42.000000 podman-4.6.0/podman/api/typing_extensions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5919 2023-07-03 15:23:31.000000 podman-4.6.0/podman/api/uds.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8640 2023-06-05 14:48:42.000000 podman-4.6.0/podman/client.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.174663 podman-4.6.0/podman/domain/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3720 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/config.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    18880 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/containers.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    31505 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/containers_create.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5514 2023-07-03 15:23:31.000000 podman-4.6.0/podman/domain/containers_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/containers_run.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/events.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/images.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/images_build.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14540 2023-07-03 15:23:31.000000 podman-4.6.0/podman/domain/images_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/ipam.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/manifests.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/networks.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6956 2023-07-05 17:06:41.000000 podman-4.6.0/podman/domain/networks_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/pods.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6131 2023-07-03 15:23:31.000000 podman-4.6.0/podman/domain/pods_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/registry_data.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/secrets.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.6.0/podman/domain/system.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-06-05 14:48:42.000000 podman-4.6.0/podman/domain/volumes.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.174663 podman-4.6.0/podman/errors/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.6.0/podman/errors/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.6.0/podman/errors/exceptions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.6.0/podman/tlsconfig.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-07-24 12:04:32.000000 podman-4.6.0/podman/version.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-07-24 12:53:29.171663 podman-4.6.0/podman.egg-info/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-07-24 12:53:28.000000 podman-4.6.0/podman.egg-info/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-07-24 12:53:29.000000 podman-4.6.0/podman.egg-info/SOURCES.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-07-24 12:53:28.000000 podman-4.6.0/podman.egg-info/dependency_links.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       76 2023-07-24 12:53:29.000000 podman-4.6.0/podman.egg-info/requires.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-07-24 12:53:29.000000 podman-4.6.0/podman.egg-info/top_level.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      662 2023-06-05 14:48:42.000000 podman-4.6.0/pyproject.toml
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1304 2023-07-24 12:53:29.175663 podman-4.6.0/setup.cfg
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.6.0/setup.py
```

### Comparing `podman-4.5.1/LICENSE` & `podman-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/PKG-INFO` & `podman-4.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.5.1
+Version: 4.6.0
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
```

### Comparing `podman-4.5.1/README.md` & `podman-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/__init__.py` & `podman-4.6.0/podman/api/__init__.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/adapter_utils.py` & `podman-4.6.0/podman/api/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/client.py` & `podman-4.6.0/podman/api/client.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/http_utils.py` & `podman-4.6.0/podman/api/http_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/parse_utils.py` & `podman-4.6.0/podman/api/parse_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/ssh.py` & `podman-4.6.0/podman/api/ssh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Specialized Transport Adapter for remote Podman access via ssh tunnel.
 
 See Podman go bindings for more details.
 """
 import collections
 import functools
-import http.client
 import logging
 import pathlib
 import random
 import socket
 import subprocess
 import urllib.parse
 from contextlib import suppress
 from typing import Optional, Union
 
 import time
 import xdg.BaseDirectory
 
-try:
-    import urllib3
-except ImportError:
-    from requests.packages import urllib3
+import urllib3
+import urllib3.connection
 
 from requests.adapters import DEFAULT_POOLBLOCK, DEFAULT_RETRIES, HTTPAdapter
 
 from .adapter_utils import _key_normalizer
 
 logger = logging.getLogger("podman.ssh_adapter")
 
@@ -147,15 +144,15 @@
             self._proc.kill()
 
         self.local_sock.unlink()
         self._proc = None
         super().close()
 
 
-class SSHConnection(http.client.HTTPConnection):
+class SSHConnection(urllib3.connection.HTTPConnection):
     """Specialization of HTTPConnection to use a SSH forwarded socket."""
 
     def __init__(
         self,
         host: str,
         port: int,
         timeout: Union[float, urllib3.Timeout, None] = None,
```

### Comparing `podman-4.5.1/podman/api/tar_utils.py` & `podman-4.6.0/podman/api/tar_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/typing_extensions.py` & `podman-4.6.0/podman/api/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/api/uds.py` & `podman-4.6.0/podman/api/uds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Specialized Transport Adapter for UNIX domain sockets."""
 import collections
 import functools
-import http.client
 import logging
 import socket
 from typing import Optional, Union
 from urllib.parse import unquote, urlparse
 
-try:
-    import urllib3
-except ImportError:
-    from requests.packages import urllib3
+import urllib3
+import urllib3.connection
 
 from requests.adapters import DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, DEFAULT_RETRIES, HTTPAdapter
 
 from ..errors import APIError
 
 from .adapter_utils import _key_normalizer
 
@@ -41,15 +38,15 @@
         netloc = unquote(urlparse(self.uds).netloc)
         try:
             super().connect(netloc)
         except Exception as e:
             raise APIError(f"Unable to make connection to UDS '{netloc}'") from e
 
 
-class UDSConnection(http.client.HTTPConnection):
+class UDSConnection(urllib3.connection.HTTPConnection):
     """Specialization of HTTPConnection to use a UNIX domain sockets."""
 
     def __init__(
         self,
         host: str,
         port: int,
         timeout: Union[float, urllib3.Timeout, None] = None,
```

### Comparing `podman-4.5.1/podman/client.py` & `podman-4.6.0/podman/client.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/config.py` & `podman-4.6.0/podman/domain/config.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/containers.py` & `podman-4.6.0/podman/domain/containers.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/containers_create.py` & `podman-4.6.0/podman/domain/containers_create.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/containers_manager.py` & `podman-4.6.0/podman/domain/containers_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,16 +107,20 @@
         """
         params = {"filters": api.prepare_filters(filters)}
         response = self.client.post("/containers/prune", params=params)
         response.raise_for_status()
 
         results = {"ContainersDeleted": [], "SpaceReclaimed": 0}
         for entry in response.json():
-            if entry.get("error") is not None:
-                raise APIError(entry["error"], response=response, explanation=entry["error"])
+            if entry.get("Err") is not None:
+                raise APIError(
+                    entry["Err"],
+                    response=response,
+                    explanation=f"""Failed to prune container '{entry["Id"]}'""",
+                )
 
             results["ContainersDeleted"].append(entry["Id"])
             results["SpaceReclaimed"] += entry["Size"]
         return results
 
     def remove(self, container_id: Union[Container, str], **kwargs):
         """Delete container.
```

### Comparing `podman-4.5.1/podman/domain/containers_run.py` & `podman-4.6.0/podman/domain/containers_run.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/events.py` & `podman-4.6.0/podman/domain/events.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/images.py` & `podman-4.6.0/podman/domain/images.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/images_build.py` & `podman-4.6.0/podman/domain/images_build.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/images_manager.py` & `podman-4.6.0/podman/domain/images_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,25 +369,29 @@
 
                 - is-automated (bool): Image build is automated.
                 - is-official (bool): Image build is owned by product provider.
                 - stars (int): Image has at least this number of stars.
 
             noTrunc (bool): Do not truncate any result string. Default: True.
             limit (int): Maximum number of results.
+            listTags (bool): list the available tags in the repository. Default: False
 
         Raises:
             APIError: when service returns an error
         """
         params = {
             "filters": api.prepare_filters(kwargs.get("filters")),
             "limit": kwargs.get("limit"),
             "noTrunc": True,
             "term": [term],
         }
 
+        if "listTags" in kwargs:
+            params["listTags"] = kwargs.get("listTags")
+
         response = self.client.get("/images/search", params=params)
         response.raise_for_status(not_found=ImageNotFound)
         return response.json()
 
     def scp(
         self,
         source: str,
```

### Comparing `podman-4.5.1/podman/domain/ipam.py` & `podman-4.6.0/podman/domain/ipam.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/manager.py` & `podman-4.6.0/podman/domain/manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/manifests.py` & `podman-4.6.0/podman/domain/manifests.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/networks.py` & `podman-4.6.0/podman/domain/networks.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/networks_manager.py` & `podman-4.6.0/podman/domain/networks_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,16 @@
 
         Args:
             filters: Criteria for selecting volumes to delete. Ignored.
 
         Raises:
             APIError: when service reports error
         """
-        response = self.client.post("/networks/prune", filters=api.prepare_filters(filters))
+        params = {"filters": api.prepare_filters(filters)}
+        response = self.client.post("/networks/prune", params=params)
         response.raise_for_status()
 
         deleted: List[str] = []
         for item in response.json():
             if item["Error"] is not None:
                 raise APIError(
                     item["Error"],
```

### Comparing `podman-4.5.1/podman/domain/pods.py` & `podman-4.6.0/podman/domain/pods.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/pods_manager.py` & `podman-4.6.0/podman/domain/pods_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """PodmanResource manager subclassed for Networks."""
 import json
 import logging
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, Iterator
 
 from podman import api
 from podman.domain.manager import Manager
 from podman.domain.pods import Pod
 from podman.errors import APIError
 
 logger = logging.getLogger("podman.pods")
@@ -99,15 +99,15 @@
 
         deleted: List[str] = []
         for item in response.json():
             if item["Err"] is not None:
                 raise APIError(
                     item["Err"],
                     response=response,
-                    explanation=f"""Failed to prune network '{item["Id"]}'""",
+                    explanation=f"""Failed to prune pod '{item["Id"]}'""",
                 )
             deleted.append(item["Id"])
         return {"PodsDeleted": deleted, "SpaceReclaimed": 0}
 
     def remove(self, pod_id: Union[Pod, str], force: Optional[bool] = None) -> None:
         """Delete pod.
 
@@ -124,28 +124,40 @@
         """
         if isinstance(pod_id, Pod):
             pod_id = pod_id.id
 
         response = self.client.delete(f"/pods/{pod_id}", params={"force": force})
         response.raise_for_status()
 
-    def stats(self, **kwargs) -> Dict[str, Any]:
+    def stats(self, **kwargs) -> Union[List[Dict[str, Any]], Iterator[List[Dict[str, Any]]]]:
         """Resource usage statistics for the containers in pods.
 
         Keyword Args:
             all (bool): Provide statistics for all running pods.
             name (Union[str, List[str]]): Pods to include in report.
+            stream (bool): Stream statistics until cancelled. Default: False.
+            decode (bool): If True, response will be decoded into dict. Default: False.
 
         Raises:
             NotFound: when pod not found
             APIError: when service reports an error
         """
         if "all" in kwargs and "name" in kwargs:
             raise ValueError("Keywords 'all' and 'name' are mutually exclusive.")
 
+        # Keeping the default for stream as False to not break existing users
+        # Should probably be changed in a newer major version to match behavior of container.stats
+        stream = kwargs.get("stream", False)
+        decode = kwargs.get("decode", False)
+
         params = {
             "all": kwargs.get("all"),
             "namesOrIDs": kwargs.get("name"),
+            "stream": stream,
         }
-        response = self.client.get("/pods/stats", params=params)
+        response = self.client.get("/pods/stats", params=params, stream=stream)
         response.raise_for_status()
-        return response.json()
+
+        if stream:
+            return api.stream_helper(response, decode_to_json=decode)
+
+        return json.loads(response.content) if decode else response.content
```

### Comparing `podman-4.5.1/podman/domain/registry_data.py` & `podman-4.6.0/podman/domain/registry_data.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/secrets.py` & `podman-4.6.0/podman/domain/secrets.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/system.py` & `podman-4.6.0/podman/domain/system.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/domain/volumes.py` & `podman-4.6.0/podman/domain/volumes.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/errors/__init__.py` & `podman-4.6.0/podman/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/errors/exceptions.py` & `podman-4.6.0/podman/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman/tlsconfig.py` & `podman-4.6.0/podman/tlsconfig.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/podman.egg-info/PKG-INFO` & `podman-4.6.0/podman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.5.1
+Version: 4.6.0
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
```

### Comparing `podman-4.5.1/podman.egg-info/SOURCES.txt` & `podman-4.6.0/podman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/pyproject.toml` & `podman-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `podman-4.5.1/setup.cfg` & `podman-4.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = podman
-version = 4.5.1
+version = 4.6.0
 author = Brent Baude, Jhon Honce
 author_email = jhonce@redhat.com
 description = Bindings for Podman RESTful API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/containers/podman-py
 license = Apache-2.0
@@ -32,15 +32,15 @@
 include_package_data = True
 python_requires = >=3.6
 test_suite = 
 install_requires = 
 	pyxdg >=0.26
 	requests >=2.24
 	tomli>=1.2.3; python_version<'3.11'
-	urllib3 >= 1.26.5, < 2.0.0
+	urllib3
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 formats = gztar
```

### Comparing `podman-4.5.1/setup.py` & `podman-4.6.0/setup.py`

 * *Files identical despite different names*

