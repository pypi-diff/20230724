# Comparing `tmp/pulumi-opnsense-v0.0.57.tar.gz` & `tmp/pulumi_opnsense-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, was "pulumi_opnsense-0.0.64.tar", last modified: Mon Jul 24 09:41:34 2023, max compression
```

## Comparing `pulumi-opnsense-v0.0.57.tar` & `pulumi_opnsense-0.0.64.tar`

### file list

```diff
@@ -1,60 +1,25 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/unbound/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/config/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:32:50.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 08:32:50.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/_utilities.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/__init__.pyi
--rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-24 08:32:51.000000 ./bin/dist/pulumi_opnsense-0.0.57.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:32:49.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     2007 2023-07-24 08:32:49.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:49.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:49.000000 ./pulumi_opnsense/_utilities.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/__init__.pyi
--rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:49.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:49.000000 ./pulumi_opnsense/pulumi-plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/host_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:41:34.979644 pulumi_opnsense-0.0.64/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 09:41:34.000000 pulumi_opnsense-0.0.64/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `./bin/pulumi_opnsense.egg-info/PKG-INFO` & `pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.57
+Version: 0.0.64
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `./bin/pulumi_opnsense.egg-info/SOURCES.txt` & `pulumi_opnsense-0.0.64/pulumi_opnsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/unbound/host_alias.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/host_alias.py`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/unbound/host_override.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/unbound/host_override.py`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/provider.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/provider.py`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/_utilities.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/_utilities.py`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/config/vars.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/config/vars.py`

 * *Files identical despite different names*

### Comparing `./bin/build/lib/pulumi_opnsense/__init__.py` & `pulumi_opnsense-0.0.64/pulumi_opnsense/__init__.py`

 * *Files identical despite different names*

### Comparing `./bin/README.md` & `pulumi_opnsense-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `./bin/setup.py` & `pulumi_opnsense-0.0.64/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.57"
-PLUGIN_VERSION = "0.0.57"
+VERSION = "0.0.64"
+PLUGIN_VERSION = "0.0.64"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

### Comparing `./README.md` & `pulumi_opnsense-0.0.64/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: pulumi_opnsense
+Version: 0.0.64
+License: Apache-2.0
+Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Pulumi Native Provider Boilerplate
 
 This repository is a boilerplate showing how to create a native Pulumi provider.
 
 ## Authoring a Pulumi Native Provider
 
 This boilerplate creates a working Pulumi-owned provider named `opnsense`.
```

