# Comparing `tmp/pulumi-opnsense-v0.0.55.tar.gz` & `tmp/pulumi-opnsense-v0.0.56.tar.gz`

## Comparing `pulumi-opnsense-v0.0.55.tar` & `pulumi-opnsense-v0.0.56.tar`

### file list

```diff
@@ -1,49 +1,60 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 11:46:11.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     1877 2023-07-21 11:46:11.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-21 11:46:11.000000 ./bin/dist/pulumi_opnsense-0.0.55.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 11:46:10.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     1875 2023-07-21 11:46:10.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:10.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:10.000000 ./pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:10.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:10.000000 ./pulumi_opnsense/pulumi-plugin.json
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:44.000000 ./bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:43.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:19:43.000000 ./bin/README.md
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-24 08:19:43.000000 ./bin/setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/_utilities.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/__init__.pyi
+-rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:43.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:43.000000 ./bin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-24 08:19:44.000000 ./bin/dist/pulumi_opnsense-0.0.56.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-24 08:19:41.000000 ./README.md
+-rw-------   0 runner    (1001) docker     (123)     2007 2023-07-24 08:19:40.000000 ./setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-24 08:19:40.000000 ./pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     6631 2023-07-24 08:19:40.000000 ./pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-24 08:19:40.000000 ./pulumi_opnsense/_utilities.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      576 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/__init__.pyi
+-rw-------   0 runner    (1001) docker     (123)      978 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-24 08:19:40.000000 ./pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-24 08:19:40.000000 ./pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-24 08:19:40.000000 ./pulumi_opnsense/pulumi-plugin.json
```

### ./bin/pulumi_opnsense.egg-info/PKG-INFO

```diff
@@ -1,10 +1,12 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.55
+Version: 0.0.56
+License: Apache-2.0
+Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
 
 This repository is a boilerplate showing how to create a native Pulumi provider.
```

### ./bin/pulumi_opnsense.egg-info/SOURCES.txt

```diff
@@ -7,10 +7,12 @@
 pulumi_opnsense/py.typed
 pulumi_opnsense.egg-info/PKG-INFO
 pulumi_opnsense.egg-info/SOURCES.txt
 pulumi_opnsense.egg-info/dependency_links.txt
 pulumi_opnsense.egg-info/not-zip-safe
 pulumi_opnsense.egg-info/requires.txt
 pulumi_opnsense.egg-info/top_level.txt
+pulumi_opnsense/config/__init__.py
+pulumi_opnsense/config/vars.py
 pulumi_opnsense/unbound/__init__.py
 pulumi_opnsense/unbound/host_alias.py
 pulumi_opnsense/unbound/host_override.py
```

### ./bin/build/lib/pulumi_opnsense/unbound/host_override.py

```diff
@@ -14,29 +14,32 @@
 @pulumi.input_type
 class HostOverrideArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  domain: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  hostname: pulumi.Input[str],
-                 mx: pulumi.Input[str],
-                 mx_prio: pulumi.Input[int],
                  rr: pulumi.Input[str],
-                 server: pulumi.Input[str]):
+                 mx: Optional[pulumi.Input[str]] = None,
+                 mx_prio: Optional[pulumi.Input[int]] = None,
+                 server: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a HostOverride resource.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "hostname", hostname)
-        pulumi.set(__self__, "mx", mx)
-        pulumi.set(__self__, "mx_prio", mx_prio)
         pulumi.set(__self__, "rr", rr)
-        pulumi.set(__self__, "server", server)
+        if mx is not None:
+            pulumi.set(__self__, "mx", mx)
+        if mx_prio is not None:
+            pulumi.set(__self__, "mx_prio", mx_prio)
+        if server is not None:
+            pulumi.set(__self__, "server", server)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         return pulumi.get(self, "description")
 
     @description.setter
@@ -68,46 +71,46 @@
 
     @hostname.setter
     def hostname(self, value: pulumi.Input[str]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Input[str]:
+    def rr(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "rr")
+
+    @rr.setter
+    def rr(self, value: pulumi.Input[str]):
+        pulumi.set(self, "rr", value)
+
+    @property
+    @pulumi.getter
+    def mx(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "mx")
 
     @mx.setter
-    def mx(self, value: pulumi.Input[str]):
+    def mx(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mx", value)
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Input[int]:
+    def mx_prio(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "mx_prio")
 
     @mx_prio.setter
-    def mx_prio(self, value: pulumi.Input[int]):
+    def mx_prio(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "mx_prio", value)
 
     @property
     @pulumi.getter
-    def rr(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "rr")
-
-    @rr.setter
-    def rr(self, value: pulumi.Input[str]):
-        pulumi.set(self, "rr", value)
-
-    @property
-    @pulumi.getter
-    def server(self) -> pulumi.Input[str]:
+    def server(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "server")
 
     @server.setter
-    def server(self, value: pulumi.Input[str]):
+    def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
 
 class HostOverride(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -174,25 +177,19 @@
             __props__.__dict__["domain"] = domain
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
             if hostname is None and not opts.urn:
                 raise TypeError("Missing required property 'hostname'")
             __props__.__dict__["hostname"] = hostname
-            if mx is None and not opts.urn:
-                raise TypeError("Missing required property 'mx'")
             __props__.__dict__["mx"] = mx
-            if mx_prio is None and not opts.urn:
-                raise TypeError("Missing required property 'mx_prio'")
             __props__.__dict__["mx_prio"] = mx_prio
             if rr is None and not opts.urn:
                 raise TypeError("Missing required property 'rr'")
             __props__.__dict__["rr"] = rr
-            if server is None and not opts.urn:
-                raise TypeError("Missing required property 'server'")
             __props__.__dict__["server"] = server
             __props__.__dict__["result"] = None
         super(HostOverride, __self__).__init__(
             'opnsense:unbound:HostOverride',
             resource_name,
             __props__,
             opts)
@@ -242,30 +239,30 @@
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Output[str]:
+    def mx(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "mx")
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Output[int]:
+    def mx_prio(self) -> pulumi.Output[Optional[int]]:
         return pulumi.get(self, "mx_prio")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def rr(self) -> pulumi.Output[str]:
         return pulumi.get(self, "rr")
 
     @property
     @pulumi.getter
-    def server(self) -> pulumi.Output[str]:
+    def server(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "server")
```

### ./bin/build/lib/pulumi_opnsense/provider.py

```diff
@@ -9,37 +9,87 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
-    def __init__(__self__):
+    def __init__(__self__, *,
+                 fw_api_address: pulumi.Input[str],
+                 fw_api_key: pulumi.Input[str],
+                 fw_api_secret: pulumi.Input[str]):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
-        pass
+        pulumi.set(__self__, "fw_api_address", fw_api_address)
+        pulumi.set(__self__, "fw_api_key", fw_api_key)
+        pulumi.set(__self__, "fw_api_secret", fw_api_secret)
+
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Input[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @fw_api_address.setter
+    def fw_api_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_address", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Input[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @fw_api_key.setter
+    def fw_api_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_key", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Input[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
+    @fw_api_secret.setter
+    def fw_api_secret(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_secret", value)
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ProviderArgs] = None,
+                 args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -50,22 +100,60 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            if fw_api_address is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_address'")
+            __props__.__dict__["fw_api_address"] = None if fw_api_address is None else pulumi.Output.secret(fw_api_address)
+            if fw_api_key is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_key'")
+            __props__.__dict__["fw_api_key"] = None if fw_api_key is None else pulumi.Output.secret(fw_api_key)
+            if fw_api_secret is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_secret'")
+            __props__.__dict__["fw_api_secret"] = None if fw_api_secret is None else pulumi.Output.secret(fw_api_secret)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["fw_api_address", "fw_api_key", "fw_api_secret"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'opnsense',
             resource_name,
             __props__,
             opts)
 
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Output[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Output[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Output[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
```

### ./bin/build/lib/pulumi_opnsense/__init__.py

```diff
@@ -5,17 +5,20 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
+    import pulumi_opnsense.config as __config
+    config = __config
     import pulumi_opnsense.unbound as __unbound
     unbound = __unbound
 else:
+    config = _utilities.lazy_import('pulumi_opnsense.config')
     unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
```

### ./bin/setup.py

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.55"
-PLUGIN_VERSION = "0.0.55"
+VERSION = "0.0.56"
+PLUGIN_VERSION = "0.0.56"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
@@ -41,14 +41,18 @@
       python_requires='>=3.7',
       version=VERSION,
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
+      project_urls={
+          'Repository': 'https://github.com/oss4u/pulumi-opnsense-native'
+      },
+      license='Apache-2.0',
       packages=find_packages(),
       package_data={
           'pulumi_opnsense': [
               'py.typed',
               'pulumi-plugin.json',
           ]
       },
```

### ./bin/pulumi_opnsense/unbound/host_override.py

```diff
@@ -14,29 +14,32 @@
 @pulumi.input_type
 class HostOverrideArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  domain: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  hostname: pulumi.Input[str],
-                 mx: pulumi.Input[str],
-                 mx_prio: pulumi.Input[int],
                  rr: pulumi.Input[str],
-                 server: pulumi.Input[str]):
+                 mx: Optional[pulumi.Input[str]] = None,
+                 mx_prio: Optional[pulumi.Input[int]] = None,
+                 server: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a HostOverride resource.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "hostname", hostname)
-        pulumi.set(__self__, "mx", mx)
-        pulumi.set(__self__, "mx_prio", mx_prio)
         pulumi.set(__self__, "rr", rr)
-        pulumi.set(__self__, "server", server)
+        if mx is not None:
+            pulumi.set(__self__, "mx", mx)
+        if mx_prio is not None:
+            pulumi.set(__self__, "mx_prio", mx_prio)
+        if server is not None:
+            pulumi.set(__self__, "server", server)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         return pulumi.get(self, "description")
 
     @description.setter
@@ -68,46 +71,46 @@
 
     @hostname.setter
     def hostname(self, value: pulumi.Input[str]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Input[str]:
+    def rr(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "rr")
+
+    @rr.setter
+    def rr(self, value: pulumi.Input[str]):
+        pulumi.set(self, "rr", value)
+
+    @property
+    @pulumi.getter
+    def mx(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "mx")
 
     @mx.setter
-    def mx(self, value: pulumi.Input[str]):
+    def mx(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mx", value)
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Input[int]:
+    def mx_prio(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "mx_prio")
 
     @mx_prio.setter
-    def mx_prio(self, value: pulumi.Input[int]):
+    def mx_prio(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "mx_prio", value)
 
     @property
     @pulumi.getter
-    def rr(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "rr")
-
-    @rr.setter
-    def rr(self, value: pulumi.Input[str]):
-        pulumi.set(self, "rr", value)
-
-    @property
-    @pulumi.getter
-    def server(self) -> pulumi.Input[str]:
+    def server(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "server")
 
     @server.setter
-    def server(self, value: pulumi.Input[str]):
+    def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
 
 class HostOverride(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -174,25 +177,19 @@
             __props__.__dict__["domain"] = domain
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
             if hostname is None and not opts.urn:
                 raise TypeError("Missing required property 'hostname'")
             __props__.__dict__["hostname"] = hostname
-            if mx is None and not opts.urn:
-                raise TypeError("Missing required property 'mx'")
             __props__.__dict__["mx"] = mx
-            if mx_prio is None and not opts.urn:
-                raise TypeError("Missing required property 'mx_prio'")
             __props__.__dict__["mx_prio"] = mx_prio
             if rr is None and not opts.urn:
                 raise TypeError("Missing required property 'rr'")
             __props__.__dict__["rr"] = rr
-            if server is None and not opts.urn:
-                raise TypeError("Missing required property 'server'")
             __props__.__dict__["server"] = server
             __props__.__dict__["result"] = None
         super(HostOverride, __self__).__init__(
             'opnsense:unbound:HostOverride',
             resource_name,
             __props__,
             opts)
@@ -242,30 +239,30 @@
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Output[str]:
+    def mx(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "mx")
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Output[int]:
+    def mx_prio(self) -> pulumi.Output[Optional[int]]:
         return pulumi.get(self, "mx_prio")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def rr(self) -> pulumi.Output[str]:
         return pulumi.get(self, "rr")
 
     @property
     @pulumi.getter
-    def server(self) -> pulumi.Output[str]:
+    def server(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "server")
```

### ./bin/pulumi_opnsense/provider.py

```diff
@@ -9,37 +9,87 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
-    def __init__(__self__):
+    def __init__(__self__, *,
+                 fw_api_address: pulumi.Input[str],
+                 fw_api_key: pulumi.Input[str],
+                 fw_api_secret: pulumi.Input[str]):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
-        pass
+        pulumi.set(__self__, "fw_api_address", fw_api_address)
+        pulumi.set(__self__, "fw_api_key", fw_api_key)
+        pulumi.set(__self__, "fw_api_secret", fw_api_secret)
+
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Input[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @fw_api_address.setter
+    def fw_api_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_address", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Input[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @fw_api_key.setter
+    def fw_api_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_key", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Input[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
+    @fw_api_secret.setter
+    def fw_api_secret(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_secret", value)
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ProviderArgs] = None,
+                 args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -50,22 +100,60 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            if fw_api_address is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_address'")
+            __props__.__dict__["fw_api_address"] = None if fw_api_address is None else pulumi.Output.secret(fw_api_address)
+            if fw_api_key is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_key'")
+            __props__.__dict__["fw_api_key"] = None if fw_api_key is None else pulumi.Output.secret(fw_api_key)
+            if fw_api_secret is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_secret'")
+            __props__.__dict__["fw_api_secret"] = None if fw_api_secret is None else pulumi.Output.secret(fw_api_secret)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["fw_api_address", "fw_api_key", "fw_api_secret"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'opnsense',
             resource_name,
             __props__,
             opts)
 
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Output[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Output[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Output[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
```

### ./bin/pulumi_opnsense/__init__.py

```diff
@@ -5,17 +5,20 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
+    import pulumi_opnsense.config as __config
+    config = __config
     import pulumi_opnsense.unbound as __unbound
     unbound = __unbound
 else:
+    config = _utilities.lazy_import('pulumi_opnsense.config')
     unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
```

### ./setup.py

```diff
@@ -41,14 +41,18 @@
       python_requires='>=3.7',
       version=VERSION,
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
+      project_urls={
+          'Repository': 'https://github.com/oss4u/pulumi-opnsense-native'
+      },
+      license='Apache-2.0',
       packages=find_packages(),
       package_data={
           'pulumi_opnsense': [
               'py.typed',
               'pulumi-plugin.json',
           ]
       },
```

### ./pulumi_opnsense/unbound/host_override.py

```diff
@@ -14,29 +14,32 @@
 @pulumi.input_type
 class HostOverrideArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  domain: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  hostname: pulumi.Input[str],
-                 mx: pulumi.Input[str],
-                 mx_prio: pulumi.Input[int],
                  rr: pulumi.Input[str],
-                 server: pulumi.Input[str]):
+                 mx: Optional[pulumi.Input[str]] = None,
+                 mx_prio: Optional[pulumi.Input[int]] = None,
+                 server: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a HostOverride resource.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "hostname", hostname)
-        pulumi.set(__self__, "mx", mx)
-        pulumi.set(__self__, "mx_prio", mx_prio)
         pulumi.set(__self__, "rr", rr)
-        pulumi.set(__self__, "server", server)
+        if mx is not None:
+            pulumi.set(__self__, "mx", mx)
+        if mx_prio is not None:
+            pulumi.set(__self__, "mx_prio", mx_prio)
+        if server is not None:
+            pulumi.set(__self__, "server", server)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         return pulumi.get(self, "description")
 
     @description.setter
@@ -68,46 +71,46 @@
 
     @hostname.setter
     def hostname(self, value: pulumi.Input[str]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Input[str]:
+    def rr(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "rr")
+
+    @rr.setter
+    def rr(self, value: pulumi.Input[str]):
+        pulumi.set(self, "rr", value)
+
+    @property
+    @pulumi.getter
+    def mx(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "mx")
 
     @mx.setter
-    def mx(self, value: pulumi.Input[str]):
+    def mx(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mx", value)
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Input[int]:
+    def mx_prio(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "mx_prio")
 
     @mx_prio.setter
-    def mx_prio(self, value: pulumi.Input[int]):
+    def mx_prio(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "mx_prio", value)
 
     @property
     @pulumi.getter
-    def rr(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "rr")
-
-    @rr.setter
-    def rr(self, value: pulumi.Input[str]):
-        pulumi.set(self, "rr", value)
-
-    @property
-    @pulumi.getter
-    def server(self) -> pulumi.Input[str]:
+    def server(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "server")
 
     @server.setter
-    def server(self, value: pulumi.Input[str]):
+    def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
 
 class HostOverride(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -174,25 +177,19 @@
             __props__.__dict__["domain"] = domain
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
             if hostname is None and not opts.urn:
                 raise TypeError("Missing required property 'hostname'")
             __props__.__dict__["hostname"] = hostname
-            if mx is None and not opts.urn:
-                raise TypeError("Missing required property 'mx'")
             __props__.__dict__["mx"] = mx
-            if mx_prio is None and not opts.urn:
-                raise TypeError("Missing required property 'mx_prio'")
             __props__.__dict__["mx_prio"] = mx_prio
             if rr is None and not opts.urn:
                 raise TypeError("Missing required property 'rr'")
             __props__.__dict__["rr"] = rr
-            if server is None and not opts.urn:
-                raise TypeError("Missing required property 'server'")
             __props__.__dict__["server"] = server
             __props__.__dict__["result"] = None
         super(HostOverride, __self__).__init__(
             'opnsense:unbound:HostOverride',
             resource_name,
             __props__,
             opts)
@@ -242,30 +239,30 @@
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
-    def mx(self) -> pulumi.Output[str]:
+    def mx(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "mx")
 
     @property
     @pulumi.getter
-    def mx_prio(self) -> pulumi.Output[int]:
+    def mx_prio(self) -> pulumi.Output[Optional[int]]:
         return pulumi.get(self, "mx_prio")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def rr(self) -> pulumi.Output[str]:
         return pulumi.get(self, "rr")
 
     @property
     @pulumi.getter
-    def server(self) -> pulumi.Output[str]:
+    def server(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "server")
```

### ./pulumi_opnsense/provider.py

```diff
@@ -9,37 +9,87 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
-    def __init__(__self__):
+    def __init__(__self__, *,
+                 fw_api_address: pulumi.Input[str],
+                 fw_api_key: pulumi.Input[str],
+                 fw_api_secret: pulumi.Input[str]):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
-        pass
+        pulumi.set(__self__, "fw_api_address", fw_api_address)
+        pulumi.set(__self__, "fw_api_key", fw_api_key)
+        pulumi.set(__self__, "fw_api_secret", fw_api_secret)
+
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Input[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @fw_api_address.setter
+    def fw_api_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_address", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Input[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @fw_api_key.setter
+    def fw_api_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_key", value)
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Input[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
+    @fw_api_secret.setter
+    def fw_api_secret(self, value: pulumi.Input[str]):
+        pulumi.set(self, "fw_api_secret", value)
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] fw_api_address: The username. Its important but not secret.
+        :param pulumi.Input[str] fw_api_key: The password. It is very secret.
+        :param pulumi.Input[str] fw_api_secret: The (entirely uncryptographic) hash function used to encode the "password".
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ProviderArgs] = None,
+                 args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a Opnsense resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -50,22 +100,60 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 fw_api_address: Optional[pulumi.Input[str]] = None,
+                 fw_api_key: Optional[pulumi.Input[str]] = None,
+                 fw_api_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            if fw_api_address is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_address'")
+            __props__.__dict__["fw_api_address"] = None if fw_api_address is None else pulumi.Output.secret(fw_api_address)
+            if fw_api_key is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_key'")
+            __props__.__dict__["fw_api_key"] = None if fw_api_key is None else pulumi.Output.secret(fw_api_key)
+            if fw_api_secret is None and not opts.urn:
+                raise TypeError("Missing required property 'fw_api_secret'")
+            __props__.__dict__["fw_api_secret"] = None if fw_api_secret is None else pulumi.Output.secret(fw_api_secret)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["fw_api_address", "fw_api_key", "fw_api_secret"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'opnsense',
             resource_name,
             __props__,
             opts)
 
+    @property
+    @pulumi.getter
+    def fw_api_address(self) -> pulumi.Output[str]:
+        """
+        The username. Its important but not secret.
+        """
+        return pulumi.get(self, "fw_api_address")
+
+    @property
+    @pulumi.getter
+    def fw_api_key(self) -> pulumi.Output[str]:
+        """
+        The password. It is very secret.
+        """
+        return pulumi.get(self, "fw_api_key")
+
+    @property
+    @pulumi.getter
+    def fw_api_secret(self) -> pulumi.Output[str]:
+        """
+        The (entirely uncryptographic) hash function used to encode the "password".
+        """
+        return pulumi.get(self, "fw_api_secret")
+
```

### ./pulumi_opnsense/__init__.py

```diff
@@ -5,17 +5,20 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
+    import pulumi_opnsense.config as __config
+    config = __config
     import pulumi_opnsense.unbound as __unbound
     unbound = __unbound
 else:
+    config = _utilities.lazy_import('pulumi_opnsense.config')
     unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
```

