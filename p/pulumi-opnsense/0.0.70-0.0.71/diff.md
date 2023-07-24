# Comparing `tmp/pulumi_opnsense-0.0.70.tar.gz` & `tmp/pulumi_opnsense-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opnsense-0.0.70.tar", last modified: Mon Jul 24 13:07:10 2023, max compression
+gzip compressed data, was "pulumi_opnsense-0.0.71.tar", last modified: Mon Jul 24 13:17:28 2023, max compression
```

## Comparing `pulumi_opnsense-0.0.70.tar` & `pulumi_opnsense-0.0.71.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.914135 pulumi_opnsense-0.0.70/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:07:10.914135 pulumi_opnsense-0.0.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.910135 pulumi_opnsense-0.0.70/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.910135 pulumi_opnsense-0.0.70/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)     1150 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)     7947 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.914135 pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/host_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:10.910135 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:07:10.914135 pulumi_opnsense-0.0.70/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 13:07:10.000000 pulumi_opnsense-0.0.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1112 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)     7795 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 13:17:28.000000 pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:17:28.179329 pulumi_opnsense-0.0.71/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 13:17:27.000000 pulumi_opnsense-0.0.71/setup.py
```

### Comparing `pulumi_opnsense-0.0.70/PKG-INFO` & `pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_opnsense
-Version: 0.0.70
+Name: pulumi-opnsense
+Version: 0.0.71
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.70/README.md` & `pulumi_opnsense-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/__init__.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/_utilities.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/config/vars.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/config/vars.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 __config__ = pulumi.Config('opnsense')
 
 
 class _ExportableConfig(types.ModuleType):
     @property
     def address(self) -> Optional[str]:
         """
-        The username. Its important but not secret.
+        The address of the fw. (without /api)
         """
         return __config__.get('address')
 
     @property
     def key(self) -> Optional[str]:
         """
-        The password. It is very secret.
+        The key to access the api of the fw.
         """
         return __config__.get('key')
 
     @property
     def plugin_download_url(self) -> Optional[str]:
         return __config__.get('pluginDownloadURL')
 
     @property
     def secret(self) -> Optional[str]:
         """
-        The (entirely uncryptographic) hash function used to encode the "password".
+        The secret to access the api of the fw.
         """
         return __config__.get('secret')
 
     @property
     def version(self) -> Optional[str]:
         return __config__.get('version')
```

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/provider.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,41 +17,41 @@
                  address: pulumi.Input[str],
                  key: pulumi.Input[str],
                  plugin_download_url: pulumi.Input[str],
                  secret: pulumi.Input[str],
                  version: pulumi.Input[str]):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] address: The username. Its important but not secret.
-        :param pulumi.Input[str] key: The password. It is very secret.
-        :param pulumi.Input[str] secret: The (entirely uncryptographic) hash function used to encode the "password".
+        :param pulumi.Input[str] address: The address of the fw. (without /api)
+        :param pulumi.Input[str] key: The key to access the api of the fw.
+        :param pulumi.Input[str] secret: The secret to access the api of the fw.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "plugin_download_url", plugin_download_url)
         pulumi.set(__self__, "secret", secret)
         pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Input[str]:
         """
-        The username. Its important but not secret.
+        The address of the fw. (without /api)
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
-        The password. It is very secret.
+        The key to access the api of the fw.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
@@ -64,15 +64,15 @@
     def plugin_download_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "plugin_download_url", value)
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Input[str]:
         """
-        The (entirely uncryptographic) hash function used to encode the "password".
+        The secret to access the api of the fw.
         """
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret", value)
 
@@ -97,17 +97,17 @@
                  secret: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] address: The username. Its important but not secret.
-        :param pulumi.Input[str] key: The password. It is very secret.
-        :param pulumi.Input[str] secret: The (entirely uncryptographic) hash function used to encode the "password".
+        :param pulumi.Input[str] address: The address of the fw. (without /api)
+        :param pulumi.Input[str] key: The key to access the api of the fw.
+        :param pulumi.Input[str] secret: The secret to access the api of the fw.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -165,36 +165,36 @@
             __props__,
             opts)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Output[str]:
         """
-        The username. Its important but not secret.
+        The address of the fw. (without /api)
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
         """
-        The password. It is very secret.
+        The key to access the api of the fw.
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter(name="pluginDownloadURL")
     def plugin_download_url(self) -> pulumi.Output[str]:
         return pulumi.get(self, "plugin_download_url")
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[str]:
         """
-        The (entirely uncryptographic) hash function used to encode the "password".
+        The secret to access the api of the fw.
         """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         return pulumi.get(self, "version")
```

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/host_alias.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense/unbound/host_override.py` & `pulumi_opnsense-0.0.71/pulumi_opnsense/unbound/host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/PKG-INFO` & `pulumi_opnsense-0.0.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-opnsense
-Version: 0.0.70
+Name: pulumi_opnsense
+Version: 0.0.71
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.70/pulumi_opnsense.egg-info/SOURCES.txt` & `pulumi_opnsense-0.0.71/pulumi_opnsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.70/setup.py` & `pulumi_opnsense-0.0.71/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.70"
-PLUGIN_VERSION = "0.0.70"
+VERSION = "0.0.71"
+PLUGIN_VERSION = "0.0.71"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

