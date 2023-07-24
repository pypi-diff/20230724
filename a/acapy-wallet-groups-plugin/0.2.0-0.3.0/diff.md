# Comparing `tmp/acapy_wallet_groups_plugin-0.2.0.tar.gz` & `tmp/acapy_wallet_groups_plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapy_wallet_groups_plugin-0.2.0.tar", max compression
+gzip compressed data, was "acapy_wallet_groups_plugin-0.3.0.tar", max compression
```

## Comparing `acapy_wallet_groups_plugin-0.2.0.tar` & `acapy_wallet_groups_plugin-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11334 2023-07-20 07:07:27.221675 acapy_wallet_groups_plugin-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1241 2023-07-20 07:07:27.221675 acapy_wallet_groups_plugin-0.2.0/acapy_wallet_groups_plugin/__init__.py
--rw-r--r--   0        0        0    10001 2023-07-20 07:07:27.221675 acapy_wallet_groups_plugin-0.2.0/acapy_wallet_groups_plugin/routes.py
--rw-r--r--   0        0        0      622 2023-07-20 07:07:27.225675 acapy_wallet_groups_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-24 10:14:18.403536 acapy_wallet_groups_plugin-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1241 2023-07-24 10:14:18.403536 acapy_wallet_groups_plugin-0.3.0/acapy_wallet_groups_plugin/__init__.py
+-rw-r--r--   0        0        0    10001 2023-07-24 10:14:18.403536 acapy_wallet_groups_plugin-0.3.0/acapy_wallet_groups_plugin/routes.py
+-rw-r--r--   0        0        0      622 2023-07-24 10:14:18.407536 acapy_wallet_groups_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.3.0/PKG-INFO
```

### Comparing `acapy_wallet_groups_plugin-0.2.0/LICENSE.md` & `acapy_wallet_groups_plugin-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.2.0/acapy_wallet_groups_plugin/__init__.py` & `acapy_wallet_groups_plugin-0.3.0/acapy_wallet_groups_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.2.0/acapy_wallet_groups_plugin/routes.py` & `acapy_wallet_groups_plugin-0.3.0/acapy_wallet_groups_plugin/routes.py`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.2.0/pyproject.toml` & `acapy_wallet_groups_plugin-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "acapy_wallet_groups_plugin"
-version = "0.2.0"
+version = "0.3.0"
 description = "Agent plugin to add a group id to a wallet"
 authors = ["Berend Sliedrecht <berend@animo.id>"]
 packages = [{ include = "acapy_wallet_groups_plugin" }]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<3.10.0"
-aries-cloudagent = { extras = ["indy"], version = "0.8.1" }
+aries-cloudagent = { extras = ["indy"], version = "0.8.2" }
 aiohttp = "^3.8.4"
 marshmallow = "^3.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
```

