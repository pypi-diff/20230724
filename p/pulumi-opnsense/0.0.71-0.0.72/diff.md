# Comparing `tmp/pulumi_opnsense-0.0.71.tar.gz` & `tmp/pulumi_opnsense-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opnsense-0.0.71.tar", last modified: Mon Jul 24 13:17:28 2023, max compression
+gzip compressed data, was "pulumi_opnsense-0.0.72.tar", last modified: Mon Jul 24 13:42:03 2023, max compression
```

## Comparing `pulumi_opnsense-0.0.71.tar` & `pulumi_opnsense-0.0.72.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)     1112 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)     7795 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.464868 pulumi_opnsense-0.0.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:42:03.464868 pulumi_opnsense-0.0.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.460868 pulumi_opnsense-0.0.72/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.464868 pulumi_opnsense-0.0.72/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1112 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)     7795 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.464868 pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/host_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:03.460868 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:42:03.464868 pulumi_opnsense-0.0.72/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 13:42:03.000000 pulumi_opnsense-0.0.72/setup.py
```

### Comparing `pulumi_opnsense-0.0.71/PKG-INFO` & `pulumi_opnsense-0.0.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opnsense
-Version: 0.0.71
+Version: 0.0.72
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.71/README.md` & `pulumi_opnsense-0.0.72/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/__init__.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/_utilities.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/config/vars.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/provider.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_alias.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/host_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_override.py` & `pulumi_opnsense-0.0.72/pulumi_opnsense/unbound/host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/PKG-INFO` & `pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.71
+Version: 0.0.72
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/SOURCES.txt` & `pulumi_opnsense-0.0.72/pulumi_opnsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.71/setup.py` & `pulumi_opnsense-0.0.72/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.71"
-PLUGIN_VERSION = "0.0.71"
+VERSION = "0.0.72"
+PLUGIN_VERSION = "0.0.72"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

