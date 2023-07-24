# Comparing `tmp/pulumi_opnsense-0.0.66.tar.gz` & `tmp/pulumi_opnsense-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opnsense-0.0.66.tar", last modified: Mon Jul 24 10:54:36 2023, max compression
+gzip compressed data, was "pulumi_opnsense-0.0.67.tar", last modified: Mon Jul 24 11:16:41 2023, max compression
```

## Comparing `pulumi_opnsense-0.0.66.tar` & `pulumi_opnsense-0.0.67.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/host_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 10:54:36.000000 pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:54:36.261136 pulumi_opnsense-0.0.66/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 10:54:35.000000 pulumi_opnsense-0.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:41.072289 pulumi_opnsense-0.0.67/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1192 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)     8367 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/host_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 11:16:40.000000 pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:16:41.076289 pulumi_opnsense-0.0.67/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 11:16:39.000000 pulumi_opnsense-0.0.67/setup.py
```

### Comparing `pulumi_opnsense-0.0.66/PKG-INFO` & `pulumi_opnsense-0.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opnsense
-Version: 0.0.66
+Version: 0.0.67
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.66/README.md` & `pulumi_opnsense-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/__init__.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/_utilities.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/config/vars.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/config/vars.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,7 +32,15 @@
     @property
     def fw_api_secret(self) -> Optional[str]:
         """
         The (entirely uncryptographic) hash function used to encode the "password".
         """
         return __config__.get('fw_api_secret')
 
+    @property
+    def plugin_download_url(self) -> Optional[str]:
+        return __config__.get('pluginDownloadURL')
+
+    @property
+    def version(self) -> Optional[str]:
+        return __config__.get('version')
+
```

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/provider.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  fw_api_address: pulumi.Input[str],
                  fw_api_key: pulumi.Input[str],
-                 fw_api_secret: pulumi.Input[str]):
+                 fw_api_secret: pulumi.Input[str],
+                 plugin_download_url: pulumi.Input[str],
+                 version: pulumi.Input[str]):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
         :param pulumi.Input[str] fw_api_key: The password. It is very secret.
         :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
         pulumi.set(__self__, "fw_api_address", fw_api_address)
         pulumi.set(__self__, "fw_api_key", fw_api_key)
         pulumi.set(__self__, "fw_api_secret", fw_api_secret)
+        pulumi.set(__self__, "plugin_download_url", plugin_download_url)
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def fw_api_address(self) -> pulumi.Input[str]:
         """
         The username. Its important but not secret.
         """
@@ -59,23 +63,43 @@
         """
         return pulumi.get(self, "fw_api_secret")
 
     @fw_api_secret.setter
     def fw_api_secret(self, value: pulumi.Input[str]):
         pulumi.set(self, "fw_api_secret", value)
 
+    @property
+    @pulumi.getter(name="pluginDownloadURL")
+    def plugin_download_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "plugin_download_url")
+
+    @plugin_download_url.setter
+    def plugin_download_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "plugin_download_url", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: pulumi.Input[str]):
+        pulumi.set(self, "version", value)
+
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fw_api_address: Optional[pulumi.Input[str]] = None,
                  fw_api_key: Optional[pulumi.Input[str]] = None,
                  fw_api_secret: Optional[pulumi.Input[str]] = None,
+                 plugin_download_url: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
         :param pulumi.Input[str] fw_api_key: The password. It is very secret.
@@ -103,14 +127,16 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fw_api_address: Optional[pulumi.Input[str]] = None,
                  fw_api_key: Optional[pulumi.Input[str]] = None,
                  fw_api_secret: Optional[pulumi.Input[str]] = None,
+                 plugin_download_url: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -121,14 +147,20 @@
             __props__.__dict__["fw_api_address"] = None if fw_api_address is None else pulumi.Output.secret(fw_api_address)
             if fw_api_key is None and not opts.urn:
                 raise TypeError("Missing required property 'fw_api_key'")
             __props__.__dict__["fw_api_key"] = None if fw_api_key is None else pulumi.Output.secret(fw_api_key)
             if fw_api_secret is None and not opts.urn:
                 raise TypeError("Missing required property 'fw_api_secret'")
             __props__.__dict__["fw_api_secret"] = None if fw_api_secret is None else pulumi.Output.secret(fw_api_secret)
+            if plugin_download_url is None and not opts.urn:
+                raise TypeError("Missing required property 'plugin_download_url'")
+            __props__.__dict__["plugin_download_url"] = plugin_download_url
+            if version is None and not opts.urn:
+                raise TypeError("Missing required property 'version'")
+            __props__.__dict__["version"] = version
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["fw_api_address", "fw_api_key", "fw_api_secret"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'opnsense',
             resource_name,
             __props__,
             opts)
@@ -153,7 +185,17 @@
     @pulumi.getter
     def fw_api_secret(self) -> pulumi.Output[str]:
         """
         The (entirely uncryptographic) hash function used to encode the "password".
         """
         return pulumi.get(self, "fw_api_secret")
 
+    @property
+    @pulumi.getter(name="pluginDownloadURL")
+    def plugin_download_url(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "plugin_download_url")
+
+    @property
+    @pulumi.getter
+    def version(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "version")
+
```

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/host_alias.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/host_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense/unbound/host_override.py` & `pulumi_opnsense-0.0.67/pulumi_opnsense/unbound/host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/PKG-INFO` & `pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.66
+Version: 0.0.67
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.66/pulumi_opnsense.egg-info/SOURCES.txt` & `pulumi_opnsense-0.0.67/pulumi_opnsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.66/setup.py` & `pulumi_opnsense-0.0.67/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.66"
-PLUGIN_VERSION = "0.0.66"
+VERSION = "0.0.67"
+PLUGIN_VERSION = "0.0.67"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

