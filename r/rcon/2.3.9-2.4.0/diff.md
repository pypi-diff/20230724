# Comparing `tmp/rcon-2.3.9.tar.gz` & `tmp/rcon-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcon-2.3.9.tar", last modified: Fri Jan 13 23:01:27 2023, max compression
+gzip compressed data, was "rcon-2.4.0.tar", last modified: Mon Jul 24 16:26:02 2023, max compression
```

## Comparing `rcon-2.3.9.tar` & `rcon-2.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.605425 rcon-2.3.9/
--rw-r--r--   0 rne       (1000) rne       (1000)     1806 2022-02-16 22:26:45.000000 rcon-2.3.9/.gitignore
--rw-r--r--   0 rne       (1000) rne       (1000)       35 2021-08-19 17:31:33.000000 rcon-2.3.9/.readthedocs.yml
--rw-r--r--   0 rne       (1000) rne       (1000)      720 2021-08-19 17:31:33.000000 rcon-2.3.9/Jenkinsfile
--rw-r--r--   0 rne       (1000) rne       (1000)    35147 2021-08-19 17:31:33.000000 rcon-2.3.9/LICENSE.txt
--rw-r--r--   0 rne       (1000) rne       (1000)      443 2022-02-16 22:26:45.000000 rcon-2.3.9/Makefile
--rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-01-13 23:01:27.605425 rcon-2.3.9/PKG-INFO
--rw-r--r--   0 rne       (1000) rne       (1000)     2293 2022-08-21 15:01:03.000000 rcon-2.3.9/README.md
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.595425 rcon-2.3.9/docs/
--rw-r--r--   0 rne       (1000) rne       (1000)      638 2021-08-19 17:31:33.000000 rcon-2.3.9/docs/Makefile
--rw-r--r--   0 rne       (1000) rne       (1000)      804 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/make.bat
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.598758 rcon-2.3.9/docs/source/
--rw-r--r--   0 rne       (1000) rne       (1000)      193 2021-08-19 17:31:33.000000 rcon-2.3.9/docs/source/bugs.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      950 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/conf.py
--rw-r--r--   0 rne       (1000) rne       (1000)      457 2021-08-19 17:31:33.000000 rcon-2.3.9/docs/source/index.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      321 2021-08-19 17:31:33.000000 rcon-2.3.9/docs/source/installation.rst
--rw-r--r--   0 rne       (1000) rne       (1000)    35493 2021-08-19 17:31:33.000000 rcon-2.3.9/docs/source/license.rst
--rw-r--r--   0 rne       (1000) rne       (1000)       49 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/modules.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      480 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/rcon.battleye.rst
--rw-r--r--   0 rne       (1000) rne       (1000)     1386 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/rcon.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      619 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/rcon.source.rst
--rw-r--r--   0 rne       (1000) rne       (1000)     2764 2022-11-18 21:28:04.000000 rcon-2.3.9/docs/source/usage.rst
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.602091 rcon-2.3.9/rcon/
--rw-r--r--   0 rne       (1000) rne       (1000)      986 2022-08-21 11:21:50.000000 rcon-2.3.9/rcon/__init__.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.602091 rcon-2.3.9/rcon/battleye/
--rw-r--r--   0 rne       (1000) rne       (1000)      163 2022-11-18 21:28:04.000000 rcon-2.3.9/rcon/battleye/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2230 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/battleye/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     4455 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/battleye/proto.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1884 2022-11-18 21:28:04.000000 rcon-2.3.9/rcon/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2892 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/config.py
--rw-r--r--   0 rne       (1000) rne       (1000)     3447 2023-01-13 22:58:22.000000 rcon-2.3.9/rcon/console.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1264 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/errorhandler.py
--rw-r--r--   0 rne       (1000) rne       (1000)      588 2022-08-21 11:17:49.000000 rcon-2.3.9/rcon/exceptions.py
--rw-r--r--   0 rne       (1000) rne       (1000)     7254 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/gui.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1933 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/rconclt.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1905 2023-01-13 22:59:15.000000 rcon-2.3.9/rcon/rconshell.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1242 2022-08-14 21:07:43.000000 rcon-2.3.9/rcon/readline.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.605425 rcon-2.3.9/rcon/source/
--rw-r--r--   0 rne       (1000) rne       (1000)      144 2022-02-16 22:26:45.000000 rcon-2.3.9/rcon/source/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2097 2022-08-21 14:51:30.000000 rcon-2.3.9/rcon/source/async_rcon.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2389 2022-08-21 14:00:07.000000 rcon-2.3.9/rcon/source/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     6162 2022-08-21 14:59:53.000000 rcon-2.3.9/rcon/source/proto.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.602091 rcon-2.3.9/rcon.egg-info/
--rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/PKG-INFO
--rw-r--r--   0 rne       (1000) rne       (1000)      962 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/SOURCES.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        1 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/dependency_links.txt
--rw-r--r--   0 rne       (1000) rne       (1000)      102 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/entry_points.txt
--rw-r--r--   0 rne       (1000) rne       (1000)       23 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/requires.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        5 2023-01-13 23:01:27.000000 rcon-2.3.9/rcon.egg-info/top_level.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        0 2021-08-19 17:31:33.000000 rcon-2.3.9/requirements.txt
--rw-r--r--   0 rne       (1000) rne       (1000)       38 2023-01-13 23:01:27.608758 rcon-2.3.9/setup.cfg
--rwxr-xr-x   0 rne       (1000) rne       (1000)      846 2022-02-22 02:28:31.000000 rcon-2.3.9/setup.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-01-13 23:01:27.605425 rcon-2.3.9/tests/
--rw-r--r--   0 rne       (1000) rne       (1000)       18 2022-02-16 22:26:45.000000 rcon-2.3.9/tests/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)      500 2022-02-16 22:26:45.000000 rcon-2.3.9/tests/test_battleye_proto.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1789 2022-02-16 22:26:45.000000 rcon-2.3.9/tests/test_config.py
--rw-r--r--   0 rne       (1000) rne       (1000)     5638 2022-02-16 22:26:45.000000 rcon-2.3.9/tests/test_source_proto.py
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.555612 rcon-2.4.0/
+-rw-r--r--   0 rne       (1000) rne       (1000)     1806 2022-02-17 09:30:26.000000 rcon-2.4.0/.gitignore
+-rw-r--r--   0 rne       (1000) rne       (1000)       35 2020-12-22 14:06:00.000000 rcon-2.4.0/.readthedocs.yml
+-rw-r--r--   0 rne       (1000) rne       (1000)      720 2021-01-11 21:30:07.000000 rcon-2.4.0/Jenkinsfile
+-rw-r--r--   0 rne       (1000) rne       (1000)    35147 2018-08-10 22:34:58.000000 rcon-2.4.0/LICENSE.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)      443 2022-02-17 09:30:26.000000 rcon-2.4.0/Makefile
+-rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-07-24 16:26:02.555612 rcon-2.4.0/PKG-INFO
+-rw-r--r--   0 rne       (1000) rne       (1000)     2293 2022-08-25 20:42:40.000000 rcon-2.4.0/README.md
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.548945 rcon-2.4.0/docs/
+-rw-r--r--   0 rne       (1000) rne       (1000)      638 2020-12-04 16:56:37.000000 rcon-2.4.0/docs/Makefile
+-rw-r--r--   0 rne       (1000) rne       (1000)      804 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/make.bat
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/docs/source/
+-rw-r--r--   0 rne       (1000) rne       (1000)      193 2020-12-19 22:39:46.000000 rcon-2.4.0/docs/source/bugs.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)      950 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/conf.py
+-rw-r--r--   0 rne       (1000) rne       (1000)      457 2020-12-19 22:36:25.000000 rcon-2.4.0/docs/source/index.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)      321 2020-12-19 22:27:44.000000 rcon-2.4.0/docs/source/installation.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)    35493 2020-12-04 16:56:37.000000 rcon-2.4.0/docs/source/license.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)       49 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/modules.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)      480 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.battleye.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)     1386 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)      619 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.source.rst
+-rw-r--r--   0 rne       (1000) rne       (1000)     2764 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/usage.rst
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/
+-rw-r--r--   0 rne       (1000) rne       (1000)      986 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/__init__.py
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/battleye/
+-rw-r--r--   0 rne       (1000) rne       (1000)      163 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/battleye/__init__.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     3022 2023-07-24 16:18:40.000000 rcon-2.4.0/rcon/battleye/client.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     4821 2023-07-24 12:26:16.000000 rcon-2.4.0/rcon/battleye/proto.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1884 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/client.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     2892 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/config.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     3447 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/console.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1264 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/errorhandler.py
+-rw-r--r--   0 rne       (1000) rne       (1000)      588 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/exceptions.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     7243 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/gui.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1933 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/rconclt.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1905 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/rconshell.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1254 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/readline.py
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/source/
+-rw-r--r--   0 rne       (1000) rne       (1000)      144 2022-02-17 09:30:26.000000 rcon-2.4.0/rcon/source/__init__.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     2097 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/async_rcon.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     2389 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/client.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     6162 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/proto.py
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon.egg-info/
+-rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/PKG-INFO
+-rw-r--r--   0 rne       (1000) rne       (1000)      962 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/SOURCES.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)        1 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/dependency_links.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)      102 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/entry_points.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)       23 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/requires.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)        5 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/top_level.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)        0 2021-01-07 21:40:17.000000 rcon-2.4.0/requirements.txt
+-rw-r--r--   0 rne       (1000) rne       (1000)       38 2023-07-24 16:26:02.555612 rcon-2.4.0/setup.cfg
+-rwxr-xr-x   0 rne       (1000) rne       (1000)      846 2022-08-25 20:42:40.000000 rcon-2.4.0/setup.py
+drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.555612 rcon-2.4.0/tests/
+-rw-r--r--   0 rne       (1000) rne       (1000)       18 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/__init__.py
+-rw-r--r--   0 rne       (1000) rne       (1000)      500 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_battleye_proto.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     1789 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_config.py
+-rw-r--r--   0 rne       (1000) rne       (1000)     5638 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_source_proto.py
```

### Comparing `rcon-2.3.9/.gitignore` & `rcon-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/Jenkinsfile` & `rcon-2.4.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/LICENSE.txt` & `rcon-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/PKG-INFO` & `rcon-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcon
-Version: 2.3.9
+Version: 2.4.0
 Summary: An RCON client library.
 Home-page: https://github.com/conqp/rcon
 Author: Richard Neumann
 Author-email: mail@richard-neumann.de
 License: GPLv3
 Keywords: python rcon client
 Requires-Python: >=3.10
```

### Comparing `rcon-2.3.9/README.md` & `rcon-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/Makefile` & `rcon-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/make.bat` & `rcon-2.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/source/conf.py` & `rcon-2.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/source/license.rst` & `rcon-2.4.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/source/rcon.rst` & `rcon-2.4.0/docs/source/rcon.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/source/rcon.source.rst` & `rcon-2.4.0/docs/source/rcon.source.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/docs/source/usage.rst` & `rcon-2.4.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/__init__.py` & `rcon-2.4.0/rcon/__init__.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/battleye/client.py` & `rcon-2.4.0/rcon/battleye/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """BattlEye RCon client."""
 
+from collections import defaultdict
 from logging import getLogger
 from socket import SOCK_DGRAM
 from typing import Callable
 
 from rcon.battleye.proto import RESPONSE_TYPES
 from rcon.battleye.proto import CommandRequest
 from rcon.battleye.proto import Header
 from rcon.battleye.proto import LoginRequest
 from rcon.battleye.proto import Request
 from rcon.battleye.proto import Response
 from rcon.battleye.proto import ServerMessage
+from rcon.battleye.proto import ServerMessageAck
 from rcon.client import BaseClient
 from rcon.exceptions import WrongPassword
 
 
 __all__ = ['Client']
 
 
@@ -27,48 +29,72 @@
     getLogger('Server message').info(server_message.message)
 
 
 class Client(BaseClient, socket_type=SOCK_DGRAM):
     """BattlEye RCon client."""
 
     def __init__(
-            self, *args,
+            self,
+            *args,
+            max_length: int = 4096,
             message_handler: MessageHandler = log_message,
             **kwargs
     ):
         super().__init__(*args, **kwargs)
-        self._handle_server_message = message_handler
+        self.max_length = max_length
+        self.message_handler = message_handler
 
-    def _receive(self, max_length: int) -> Response:
+    def handle_server_message(self, message: ServerMessage):
+        """Handle the respective server message."""
+        with self._socket.makefile('wb') as file:
+            file.write(bytes(ServerMessageAck(message.seq)))
+
+        self.message_handler(message)
+
+    def receive(self) -> Response:
         """Receive a packet."""
         return RESPONSE_TYPES[
             (header := Header.from_bytes(
-                (data := self._socket.recv(max_length))[:8]
+                (data := self._socket.recv(self.max_length))[:8]
             )).type
         ].from_bytes(header, data[8:])
 
-    def receive(self, max_length: int = 4096) -> Response:
-        """Receive a message."""
-        while isinstance(response := self._receive(max_length), ServerMessage):
-            self._handle_server_message(response)
-
-        return response
-
-    def communicate(self, request: Request) -> Response:
+    def communicate(self, request: Request) -> Response | str:
         """Send a request and receive a response."""
-        with self._socket.makefile('wb') as file:
-            file.write(bytes(request))
+        acknowledged = defaultdict(set)
+        messages = []
 
-        return self.receive()
+        while True:
+            with self._socket.makefile('wb') as file:
+                file.write(bytes(request))
+
+            response = self.receive()
+
+            try:
+                seq = response.seq
+            except AttributeError:
+                return response
+
+            if seq in acknowledged[msg_type := type(response)]:
+                break
+            else:
+                acknowledged[msg_type].add(seq)
+
+            if isinstance(response, ServerMessage):
+                self.handle_server_message(response)
+            else:
+                messages.append(response)
+
+        return ''.join(
+            msg.message for msg in sorted(messages, key=lambda msg: msg.seq)
+        )
 
     def login(self, passwd: str) -> bool:
         """Log-in the user."""
         if not self.communicate(LoginRequest(passwd)).success:
             raise WrongPassword()
 
         return True
 
     def run(self, command: str, *args: str) -> str:
         """Execute a command and return the text message."""
-        return self.communicate(
-            CommandRequest.from_command(command, *args)
-        ).message
+        return self.communicate(CommandRequest.from_command(command, *args))
```

### Comparing `rcon-2.3.9/rcon/battleye/proto.py` & `rcon-2.4.0/rcon/battleye/proto.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     'RESPONSE_TYPES',
     'Header',
     'LoginRequest',
     'LoginResponse',
     'CommandRequest',
     'CommandResponse',
     'ServerMessage',
+    'ServerMessageAck',
     'Request',
     'Response'
 ]
 
 
 PREFIX = 'BE'
 INFIX = 0xff
@@ -168,15 +169,29 @@
 
     @property
     def message(self) -> str:
         """Return the text message."""
         return self.payload.decode('ascii')
 
 
-Request = LoginRequest | CommandRequest
+class ServerMessageAck(NamedTuple):
+    """An acknowledgement of a message from the server."""
+
+    seq: int
+
+    def __bytes__(self):
+        return (0x02).to_bytes(1, 'little') + self.payload
+
+    @property
+    def payload(self) -> bytes:
+        """Return the payload."""
+        return self.seq.to_bytes(1, 'little')
+
+
+Request = LoginRequest | CommandRequest | ServerMessageAck
 Response = LoginResponse | CommandResponse | ServerMessage
 
 RESPONSE_TYPES = {
     0x00: LoginResponse,
     0x01: CommandResponse,
     0x02: ServerMessage
 }
```

### Comparing `rcon-2.3.9/rcon/client.py` & `rcon-2.4.0/rcon/client.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/config.py` & `rcon-2.4.0/rcon/config.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/console.py` & `rcon-2.4.0/rcon/console.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/errorhandler.py` & `rcon-2.4.0/rcon/errorhandler.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/exceptions.py` & `rcon-2.4.0/rcon/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/gui.py` & `rcon-2.4.0/rcon/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     host: str
     port: int
     passwd: str
     command: Iterable[str]
 
 
-class GUI(Gtk.Window):  # pylint: disable=R0902
+class GUI(Gtk.Window):
     """A GTK based GUI for RCON."""
 
     def __init__(self, args: Namespace):
         """Initialize the GUI."""
         super().__init__(title='RCON GUI')
         self.args = args
 
@@ -110,17 +110,19 @@
         """Return the client class."""
         return battleye.Client if self.args.battleye else source.Client
 
     @property
     def result_text(self) -> str:
         """Return the result text."""
         if (buf := self.result.get_buffer()) is not None:
-            start = buf.get_iter_at_line(0)
-            end = buf.get_iter_at_line(buf.get_line_count())
-            return buf.get_text(start, end, True)
+            return buf.get_text(
+                buf.get_iter_at_line(0),
+                buf.get_iter_at_line(buf.get_line_count()),
+                True
+            )
 
         return ''
 
     @result_text.setter
     def result_text(self, text: str):
         """Set the result text."""
         if (buf := self.result.get_buffer()) is not None:
```

### Comparing `rcon-2.3.9/rcon/rconclt.py` & `rcon-2.4.0/rcon/rconclt.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/rconshell.py` & `rcon-2.4.0/rcon/rconshell.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/readline.py` & `rcon-2.4.0/rcon/readline.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,42 +8,41 @@
 except ModuleNotFoundError:
     read_history_file = write_history_file = lambda _: None
 
 
 __all__ = ['CommandHistory']
 
 
-HIST_FILE = Path.home().joinpath('.rconshell_history')
+HIST_FILE = Path.home() / '.rconshell_history'
 
 
 class CommandHistory:
     """Context manager for the command line history."""
 
-    __slots__ = ('logger',)
-
-    def __init__(self, logger: Logger):
+    def __init__(self, logger: Logger, file: Path = HIST_FILE):
         """Set the logger to use."""
         self.logger = logger
+        self.file = file
 
     def __enter__(self):
         """Load the history file."""
         try:
-            read_history_file(HIST_FILE)
+            read_history_file(self.file)
         except FileNotFoundError:
             self.logger.warning(
-                'Could not find history file: %s', HIST_FILE
+                'Could not find history file: %s', self.file
             )
         except PermissionError:
             self.logger.error(
-                'Insufficient permissions to read: %s', HIST_FILE
+                'Insufficient permissions to read: %s', self.file
             )
 
         return self
 
     def __exit__(self, *_):
         """Write to the history file."""
         try:
-            write_history_file(HIST_FILE)
+            write_history_file(self.file)
         except PermissionError:
             self.logger.error(
-                'Insufficient permissions to write: %s', HIST_FILE
+                'Insufficient permissions to write: %s', self.file
             )
```

### Comparing `rcon-2.3.9/rcon/source/async_rcon.py` & `rcon-2.4.0/rcon/source/async_rcon.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/source/client.py` & `rcon-2.4.0/rcon/source/client.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon/source/proto.py` & `rcon-2.4.0/rcon/source/proto.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/rcon.egg-info/PKG-INFO` & `rcon-2.4.0/rcon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcon
-Version: 2.3.9
+Version: 2.4.0
 Summary: An RCON client library.
 Home-page: https://github.com/conqp/rcon
 Author: Richard Neumann
 Author-email: mail@richard-neumann.de
 License: GPLv3
 Keywords: python rcon client
 Requires-Python: >=3.10
```

### Comparing `rcon-2.3.9/rcon.egg-info/SOURCES.txt` & `rcon-2.4.0/rcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/setup.py` & `rcon-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/tests/test_config.py` & `rcon-2.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rcon-2.3.9/tests/test_source_proto.py` & `rcon-2.4.0/tests/test_source_proto.py`

 * *Files identical despite different names*

