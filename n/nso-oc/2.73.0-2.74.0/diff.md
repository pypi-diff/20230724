# Comparing `tmp/nso-oc-2.73.0.tar.gz` & `tmp/nso-oc-2.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.73.0.tar", last modified: Fri Jul 21 19:21:34 2023, max compression
+gzip compressed data, was "nso-oc-2.74.0.tar", last modified: Mon Jul 24 19:31:20 2023, max compression
```

## Comparing `nso-oc-2.73.0.tar` & `nso-oc-2.74.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-21 19:21:04.000000 nso-oc-2.73.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 19:21:04.000000 nso-oc-2.73.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 19:21:34.484276 nso-oc-2.73.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-21 19:21:04.000000 nso-oc-2.73.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.480276 nso-oc-2.73.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.480276 nso-oc-2.73.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33602 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36876 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-21 19:21:04.000000 nso-oc-2.73.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 19:21:34.484276 nso-oc-2.73.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 19:21:04.000000 nso-oc-2.73.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:31:20.491058 nso-oc-2.74.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-24 19:30:42.000000 nso-oc-2.74.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 19:30:42.000000 nso-oc-2.74.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-24 19:31:20.491058 nso-oc-2.74.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-24 19:30:42.000000 nso-oc-2.74.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:31:20.483058 nso-oc-2.74.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 19:31:20.000000 nso-oc-2.74.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:31:20.487058 nso-oc-2.74.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:31:20.487058 nso-oc-2.74.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33602 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:31:20.491058 nso-oc-2.74.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-24 19:30:42.000000 nso-oc-2.74.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 19:30:42.000000 nso-oc-2.74.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 19:31:20.491058 nso-oc-2.74.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-24 19:30:42.000000 nso-oc-2.74.0/setup.py
```

### Comparing `nso-oc-2.73.0/LICENSE` & `nso-oc-2.74.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/PKG-INFO` & `nso-oc-2.74.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.73.0
+Version: 2.74.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.73.0/README.md` & `nso-oc-2.74.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.74.0/nso_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.73.0
+Version: 2.74.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.73.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.74.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/README.md` & `nso-oc-2.74.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/common.py` & `nso-oc-2.74.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/main.py` & `nso-oc-2.74.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,16 +609,20 @@
         peer_or_neighbor_config["openconfig-network-instance:peer-as"] = neighbor["remote-as"]
         delete_leftover_neighbor_prop("remote-as", index, neighbor_leftover)
     if neighbor.get("description"):
         peer_or_neighbor_config["openconfig-network-instance:description"] = neighbor["description"]
         delete_leftover_neighbor_prop("description", index, neighbor_leftover)
     if neighbor.get("password", {}).get("text"):
         peer_or_neighbor_config["openconfig-network-instance:auth-password"] = neighbor["password"]["text"]
+    if neighbor.get("password", {}).get("enctype") == 7:
+        peer_or_neighbor_config["openconfig-bgp-ext:password-encryption"] = 'ENCRYPTED'
+    elif neighbor.get("password", {}).get("enctype") == 0:
+        peer_or_neighbor_config["openconfig-bgp-ext:password-encryption"] = 'CLEARTEXT'
+    if neighbor.get("password", {}):
         del neighbor_leftover[index]["password"]
-        # delete_leftover_neighbor_prop("password", index, neighbor_leftover)
     if neighbor.get("ao", {}).get("keychain-name"):
         peer_or_neighbor_config["openconfig-bgp-ext:tcpao-keychain"] = neighbor["ao"]["keychain-name"]
         del neighbor_leftover[index]["ao"]
     if is_afi_safi:
         if neighbor.get("local-as", {}).get("as-no"):
             peer_or_neighbor_config["openconfig-network-instance:local-as"] = neighbor["local-as"]["as-no"]
             delete_leftover_neighbor_prop("local-as", index, neighbor_leftover)
```

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_mpls.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_mpls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,16 +676,19 @@
     bgp_before = bgp_before_list[0]
     bgp_leftover = bgp_leftover_list[0]
 
     clean_up_default_neighbors_and_peers(bgp_before, bgp_leftover)
     clean_up_vrf_neighbors_and_peers(bgp_before.get("address-family", {}).get("with-vrf", {}),
                                      bgp_leftover.get("address-family", {}).get("with-vrf", {}).get("ipv4", []))
 
-    if bgp_leftover != None and len(bgp_leftover["bgp"]) == 0:
+    if bgp_leftover != None and bgp_leftover.get("bgp") != None:
         del bgp_leftover["bgp"]
+
+    # if bgp_leftover != None and len(bgp_leftover["bgp"]) == 0:
+    #     del bgp_leftover["bgp"]
     # if bgp_leftover.get("address-family", {}).get("ipv4") != None:
     #     check_delete_protocol_leftovers(bgp_leftover, "ipv4")
     # if bgp_leftover.get("address-family") != None:
     #     check_delete_protocol_leftovers(bgp_leftover, "vpnv4")
     # if bgp_leftover.get("address-family") != None:
     #     pass
```

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.74.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.74.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.74.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.74.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.74.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.74.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.73.0/setup.py` & `nso-oc-2.74.0/setup.py`

 * *Files identical despite different names*

