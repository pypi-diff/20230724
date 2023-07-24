# Comparing `tmp/pulumi-opnsense-v0.0.56.tar.gz` & `tmp/pulumi-opnsense-v0.0.57.tar.gz`

## Comparing `pulumi-opnsense-v0.0.56.tar` & `pulumi-opnsense-v0.0.57.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:44.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:19:43.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 08:19:43.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/_utilities.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/__init__.pyi
--rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-24 08:19:44.000000 ./bin/dist/pulumi_opnsense-0.0.56.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:19:41.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     2007 2023-07-24 08:19:40.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:40.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:40.000000 ./pulumi_opnsense/_utilities.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/__init__.pyi
--rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:40.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:40.000000 ./pulumi_opnsense/pulumi-plugin.json
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:32:51.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/unbound/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/build/lib/pulumi_opnsense/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:50.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:32:50.000000 ./bin/README.md
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 08:32:50.000000 ./bin/setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/_utilities.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/__init__.pyi
+-rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:50.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:51.000000 ./bin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-24 08:32:51.000000 ./bin/dist/pulumi_opnsense-0.0.57.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:32:49.000000 ./README.md
+-rw-------   0 runner    (1001) docker     (123)     2007 2023-07-24 08:32:49.000000 ./setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:32:49.000000 ./pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:32:49.000000 ./pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:32:49.000000 ./pulumi_opnsense/_utilities.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/__init__.pyi
+-rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:32:49.000000 ./pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:32:49.000000 ./pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:32:49.000000 ./pulumi_opnsense/pulumi-plugin.json
```

### ./bin/pulumi_opnsense.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.56
+Version: 0.0.57
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### ./bin/setup.py

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.56"
-PLUGIN_VERSION = "0.0.56"
+VERSION = "0.0.57"
+PLUGIN_VERSION = "0.0.57"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

