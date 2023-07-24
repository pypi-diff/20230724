# Comparing `tmp/secenv-1.2.3.tar.gz` & `tmp/secenv-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secenv-1.2.3.tar", last modified: Mon Jul 10 09:00:23 2023, max compression
+gzip compressed data, was "secenv-1.2.4.tar", last modified: Mon Jul 24 08:44:07 2023, max compression
```

## Comparing `secenv-1.2.3.tar` & `secenv-1.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-10 08:59:43.000000 secenv-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    50212 2023-07-10 09:00:23.015214 secenv-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8953 2023-07-10 08:59:43.000000 secenv-1.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1161 2023-07-10 08:59:44.000000 secenv-1.2.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv/
--rw-rw-rw-   0 root         (0) root         (0)    11962 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3750 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv/contexts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/contexts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/contexts/aws_assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/secenv/stores/
--rw-rw-rw-   0 root         (0) root         (0)     4446 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/aws.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/env.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/pass.py
--rw-rw-rw-   0 root         (0) root         (0)     2701 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/scaleway.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/vault.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv.egg-info/
--rw-r--r--   0 root         (0) root         (0)    50212 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-07-10 09:00:23.000000 secenv-1.2.3/secenv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:00:23.015214 secenv-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-10 08:59:43.000000 secenv-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_config_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_context_output.py
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_fill_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_gen_context.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_list_contexts.py
--rw-rw-rw-   0 root         (0) root         (0)    10980 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.039123 secenv-1.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-24 08:43:31.000000 secenv-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-07-24 08:44:07.039123 secenv-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8953 2023-07-24 08:43:31.000000 secenv-1.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-24 08:43:33.000000 secenv-1.2.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.035123 secenv-1.2.4/secenv/
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.035123 secenv-1.2.4/secenv/contexts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/contexts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/contexts/aws_assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.035123 secenv-1.2.4/secenv/stores/
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/pass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2778 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/scaleway.py
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/stores/vault.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-07-24 08:43:31.000000 secenv-1.2.4/secenv/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.035123 secenv-1.2.4/secenv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 08:44:07.000000 secenv-1.2.4/secenv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 08:44:07.039123 secenv-1.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 08:43:31.000000 secenv-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:44:07.039123 secenv-1.2.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5481 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_config_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_context_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     5710 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_fill_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_gen_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_list_contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)    11240 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-07-24 08:43:31.000000 secenv-1.2.4/tests/test_utils.py
```

### Comparing `secenv-1.2.3/LICENSE` & `secenv-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/PKG-INFO` & `secenv-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.2.3
+Version: 1.2.4
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.2.3/README.md` & `secenv-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/pyproject.toml` & `secenv-1.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "secenv"
-version = "1.2.3"
+version = "1.2.4"
 description = "An utility tool to list, read and fill secrets from multiple stores."
 readme = "README.md"
 authors = [{ name = "Keltio Labs", email = "labs@keltio.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -37,7 +37,10 @@
 Changelog = "https://secenv.keltio.fr/changelog"
 
 [project.scripts]
 secenv = "secenv.__init__:main"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
+
+[tool.black]
+line-length = 120
```

### Comparing `secenv-1.2.3/secenv/__init__.py` & `secenv-1.2.4/secenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,33 +54,23 @@
         argparse.Namespace: A dictionary where the keys are the arguments of the program
             and the keys are the associated values
     """
     parser = argparse.ArgumentParser()
     subparsers_group = parser.add_subparsers()
     subparsers = {}
 
-    subparsers["version"] = subparsers_group.add_parser(
-        "version", help="get secenv version"
-    )
+    subparsers["version"] = subparsers_group.add_parser("version", help="get secenv version")
 
-    subparsers["validate"] = subparsers_group.add_parser(
-        "validate", help="validate secenv config"
-    )
+    subparsers["validate"] = subparsers_group.add_parser("validate", help="validate secenv config")
 
-    subparsers["secrets"] = subparsers_group.add_parser(
-        "secrets", help="fill secrets in the stores"
-    )
+    subparsers["secrets"] = subparsers_group.add_parser("secrets", help="fill secrets in the stores")
 
-    subparsers["contexts"] = subparsers_group.add_parser(
-        "contexts", help="list available contexts"
-    )
+    subparsers["contexts"] = subparsers_group.add_parser("contexts", help="list available contexts")
 
-    subparsers["context"] = subparsers_group.add_parser(
-        "context", help="generate an environment based on a context"
-    )
+    subparsers["context"] = subparsers_group.add_parser("context", help="generate an environment based on a context")
     subparsers["context"].add_argument("context")
     subparsers["context"].add_argument(
         "-o",
         "--output-format",
         choices=context.available_formats,
         default="shell",
         dest="format",
@@ -131,17 +121,15 @@
                 print("Config error: extended store does not exist:", extended)
                 sys.exit(1)
             extended_infos = config["stores"][extended]
             extended_infos.update(infos)
             infos = extended_infos
 
         try:
-            store = importlib.import_module(
-                f".stores.{infos['type']}", package="secenv"
-            )
+            store = importlib.import_module(f".stores.{infos['type']}", package="secenv")
         except ModuleNotFoundError:
             print(f"Config error: no store defined as '{infos['type']}'")
             sys.exit(1)
         stores[name] = store.Store(name, infos)
 
     return stores
 
@@ -257,17 +245,15 @@
         if "type" in obj and "extends" in obj:
             logs.append(f"Store '{name}' contains both 'type' and 'extends' keys")
 
         if "type" not in obj and "extends" not in obj:
             logs.append(f"Store '{name}' contains neither 'type' nor 'extends' keys")
 
         if "extends" in obj and obj["extends"] not in config["stores"]:
-            logs.append(
-                f"Store '{name}' extends an inexistent store '{obj['extends']}'"
-            )
+            logs.append(f"Store '{name}' extends an inexistent store '{obj['extends']}'")
 
     if "secrets" not in config:
         config["secrets"] = []
     for idx, obj in enumerate(config["secrets"]):
         if "store" not in obj:
             logs.append(f"Secret {idx} doesn't contain the 'store' key")
         if "secret" not in obj:
@@ -278,33 +264,25 @@
             logs.append(f"Secret {idx} generation doesn't have a type")
 
     if "contexts" not in config:
         config["contexts"] = {}
     for name, obj in config["contexts"].items():
         for extended in obj.get("extends", []):
             if extended not in config["contexts"]:
-                logs.append(
-                    f"Context '{name}' extends an inexistent context '{extended}'"
-                )
+                logs.append(f"Context '{name}' extends an inexistent context '{extended}'")
 
         for var_name, var_obj in obj.get("vars", {}).items():
             if type(var_obj) is str:
                 continue
             if "store" not in var_obj:
-                logs.append(
-                    f"Secret '{name}/{var_name}' doesn't contain the 'store' key"
-                )
+                logs.append(f"Secret '{name}/{var_name}' doesn't contain the 'store' key")
             if "store" in var_obj and var_obj["store"] not in config["stores"]:
-                logs.append(
-                    f"Secret '{name}/{var_name}' references an inexistent store '{var_obj['store']}'"
-                )
+                logs.append(f"Secret '{name}/{var_name}' references an inexistent store '{var_obj['store']}'")
             if "secret" not in var_obj:
-                logs.append(
-                    f"Secret '{name}/{var_name}' doesn't contain the 'secret' key"
-                )
+                logs.append(f"Secret '{name}/{var_name}' doesn't contain the 'secret' key")
             if "key" in var_obj and type(var_obj["key"]) is not str:
                 logs.append(
                     f"Secret '{name}/{var_name}' defines 'key' with wrong type '{type(var_obj['key'])}' (expects 'str')"
                 )
             if "sensitive" in var_obj and type(var_obj["sensitive"]) is not bool:
                 logs.append(
                     f"Secret '{name}/{var_name}' defines 'sensitive' with wrong type '{type(var_obj['sensitive'])}' (expects 'bool')"
```

### Comparing `secenv-1.2.3/secenv/context.py` & `secenv-1.2.4/secenv/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,15 @@
         return True
 
 
 def gen_vars(vars, stores):
     output = {}
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
-        results = [
-            executor.submit(_handle_var, key, value, stores, output)
-            for key, value in vars.items()
-        ]
+        results = [executor.submit(_handle_var, key, value, stores, output) for key, value in vars.items()]
         for future in concurrent.futures.as_completed(results):
             future.result()
 
     sensitive_output = {}
 
     for key, var_config in vars.items():
         sensitive_output[key] = {
@@ -101,17 +98,15 @@
         if type(v) == str:
             continue
         # and values from stores are computed first
         args = {k2: v2 for k2, v2 in v.items() if k2 != "store" and v2}
         creds[k] = read_secret(stores[v["store"]], args)
 
     try:
-        key_id, secret_key, token = aws_assume_role(
-            creds["key_id"], creds["secret_key"], creds["role"]
-        )
+        key_id, secret_key, token = aws_assume_role(creds["key_id"], creds["secret_key"], creds["role"])
         output["AWS_ACCESS_KEY_ID"] = key_id
         output["AWS_SECRET_ACCESS_KEY"] = secret_key
         output["AWS_SESSION_TOKEN"] = token
     except Exception:
         print(f"AWS error: couldn't assume role '{creds['role']}'")
         sys.exit(1)
```

### Comparing `secenv-1.2.3/secenv/contexts/aws_assume_role.py` & `secenv-1.2.4/secenv/contexts/aws_assume_role.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import boto3
 
 
 def aws_assume_role(access_key_id, secret_access_key, role_arn):
-    session = boto3.Session(
-        aws_access_key_id=access_key_id, aws_secret_access_key=secret_access_key
-    )
+    session = boto3.Session(aws_access_key_id=access_key_id, aws_secret_access_key=secret_access_key)
 
     sts_client = session.client("sts")
-    assumed_role_object = sts_client.assume_role(
-        RoleArn=role_arn, RoleSessionName="AssumeRoleSession1"
-    )
+    assumed_role_object = sts_client.assume_role(RoleArn=role_arn, RoleSessionName="AssumeRoleSession1")
 
     credentials = assumed_role_object["Credentials"]
     access_key_id = credentials["AccessKeyId"]
     secret_access_key = credentials["SecretAccessKey"]
     session_token = credentials["SessionToken"]
 
     return access_key_id, secret_access_key, session_token
```

### Comparing `secenv-1.2.3/secenv/stores/__init__.py` & `secenv-1.2.4/secenv/stores/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,15 @@
     else:
         return secret
 
 
 def fill_secret(store, secret):
     secret_already_exists = False
     try:
-        secret_without_keys_and_type = {
-            k: v for k, v in secret.items() if k not in ["keys", "generate"]
-        }
+        secret_without_keys_and_type = {k: v for k, v in secret.items() if k not in ["keys", "generate"]}
         if store.read_secret(**secret_without_keys_and_type):
             secret_already_exists = True
     except SecretNotFoundError:
         pass
 
     if secret_already_exists and not yes_no(
         f"Secret '{secret['secret']}' already exists in store '{store.name}', overwrite?"
@@ -131,16 +129,15 @@
         """Init the store, check the provided keys, and create possible client"""
         ...
 
     def get_from_config(self, store: str, value: str, infos: dict, default=None) -> str:
         if value not in infos and f"{EnvPrefix}_{store}_{value}" not in os.environ:
             if default is None:
                 raise Exception(
-                    f"Config error: '{value}' is required in store '{store}'"
-                    f" or {EnvPrefix}_{store}_{value} in env"
+                    f"Config error: '{value}' is required in store '{store}'" f" or {EnvPrefix}_{store}_{value} in env"
                 )
             else:
                 return default
         return infos.get(value, os.getenv(f"{EnvPrefix}_{store}_{value}"))
 
     @abstractmethod
     def gen_parser(self, parser: argparse.ArgumentParser) -> None:
```

### Comparing `secenv-1.2.3/secenv/stores/aws.py` & `secenv-1.2.4/secenv/stores/aws.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/secenv/stores/azure.py` & `secenv-1.2.4/secenv/stores/azure.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/secenv/stores/bitwarden.py` & `secenv-1.2.4/secenv/stores/bitwarden.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,12 @@
     @cached
     def read_secret(self, secret) -> str:
         result = subprocess.run(["rbw", "get", secret], capture_output=True)
         if result.returncode != 0:
             stderr = result.stderr.strip().decode("utf-8")
             if "no entry found" in stderr:
                 raise SecretNotFoundError(self.name, secret)
-            raise Exception(
-                f"bitwarden store '{self.name}': rbw error during execution: {stderr}"
-            )
+            raise Exception(f"bitwarden store '{self.name}': rbw error during execution: {stderr}")
         return result.stdout.strip().decode("utf-8")
 
     def fill_secret(self, secret, generate=None):
         raise Exception("Can't write secrets to Bitwarden for now.")
```

### Comparing `secenv-1.2.3/secenv/stores/env.py` & `secenv-1.2.4/secenv/stores/env.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/secenv/stores/gcp.py` & `secenv-1.2.4/secenv/stores/gcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         self.name = name
         self.project_id = super().get_from_config(name, "project_id", infos)
 
         # https://cloud.google.com/docs/authentication/provide-credentials-adc#local-key
         # To use service account keys,
         # the library looks for the `GOOGLE_APPLICATION_CREDENTIALS`
         # environment value.
-        self._creds = super().get_from_config(
-            name, "google_application_credentials", infos, default=""
-        )
+        self._creds = super().get_from_config(name, "google_application_credentials", infos, default="")
 
         self.client = secretmanager.SecretManagerServiceClient()
 
     def gen_parser(self, parser):
         parser.add_argument("secret")
 
     @cached
```

### Comparing `secenv-1.2.3/secenv/stores/pass.py` & `secenv-1.2.4/secenv/stores/pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import passpy
 from . import StoreInterface, cached, ask_secret, SecretNotFoundError, generate_secret
 
 
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
-        directory = super().get_from_config(
-            name, "directory", infos, default="~/.password-store"
-        )
+        directory = super().get_from_config(name, "directory", infos, default="~/.password-store")
         self.store = passpy.Store(store_dir=directory)
 
     def gen_parser(self, parser):
         parser.add_argument("secret")
 
     @cached
     def read_secret(self, secret):
```

### Comparing `secenv-1.2.3/secenv/stores/scaleway.py` & `secenv-1.2.4/secenv/stores/scaleway.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,26 @@
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
         region = super().get_from_config(name, "region", infos)
         self.project_id = super().get_from_config(name, "project_id", infos)
         self.token = super().get_from_config(name, "token", infos)
 
-        self.base_url = (
-            f"https://api.scaleway.com/secret-manager/v1alpha1/regions/{region}"
-        )
+        self.base_url = f"https://api.scaleway.com/secret-manager/v1alpha1/regions/{region}"
 
     def _get(self, url) -> str:
         if not url.startswith("/"):
             url = "/" + url
         ret = requests.get(self.base_url + url, headers={"X-Auth-Token": self.token})
         return ret.text
 
     def _post(self, url, data) -> str:
         if not url.startswith("/"):
             url = "/" + url
-        ret = requests.post(
-            self.base_url + url, headers={"X-Auth-Token": self.token}, json=data
-        )
+        ret = requests.post(self.base_url + url, headers={"X-Auth-Token": self.token}, json=data)
         return ret.text
 
     def _name_to_uid(self, secret):
         ret = json.loads(self._get(f"secrets-by-name/{secret}"))
         if "type" in ret and ret["type"] == "not_found":
             raise SecretNotFoundError(self.name, secret)
         return ret["id"]
@@ -48,32 +44,31 @@
         if "type" in ret and ret["type"] == "not_found":
             raise SecretNotFoundError(self.name, secret)
         return base64.b64decode(ret["data"]).decode()
 
     def filter(self, secret, key):
         return json.loads(secret)[key]
 
-    def fill_secret(self, secret, keys=[], generate=None):
+    def fill_secret(self, secret, keys=[], generate=None, existing=None):
         if keys:
             values = {}
             for key in keys:
                 if generate:
                     values[key] = generate_secret(generate)
                 else:
-                    values[key] = ask_secret(self.name, secret, key)
+                    existing_key = existing[key] if type(existing) is dict and key in existing else None
+                    values[key] = ask_secret(self.name, secret, key, existing_key)
             secret_value = json.dumps(values)
         elif generate:
             secret_value = generate_secret(generate)
         else:
-            secret_value = ask_secret(self.name, secret)
+            secret_value = ask_secret(self.name, secret, existing=existing)
 
         try:
             uid = self._name_to_uid(secret)
         except SecretNotFoundError:
-            ret = self._post(
-                "secrets", {"name": secret, "project_id": self.project_id, "tags": []}
-            )
+            ret = self._post("secrets", {"name": secret, "project_id": self.project_id, "tags": []})
             uid = json.loads(ret)["id"]
 
         url = f"secrets/{uid}/versions"
         data = {"data": base64.b64encode(secret_value.encode()).decode()}
         self._post(url, data)
```

### Comparing `secenv-1.2.3/secenv/stores/vault.py` & `secenv-1.2.4/secenv/stores/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,15 @@
         parser.add_argument("secret")
         parser.add_argument("--key")
         parser.add_argument("--engine")
 
     @cached
     def read_secret(self, secret, engine=""):
         try:
-            read_response = self.client.secrets.kv.read_secret_version(
-                path=secret, mount_point=engine
-            )
+            read_response = self.client.secrets.kv.read_secret_version(path=secret, mount_point=engine)
         except hvac.exceptions.InvalidPath as e:
             if "route entry not found" in str(e.text):
                 raise SecretNotFoundError(self.name, secret)
             raise Exception(f"vault store '{self.name}': error during execution: {e}")
 
         return read_response
 
@@ -41,10 +39,8 @@
                     values[key] = ask_secret(self.name, secret, key)
             secret_value = values
         elif generate:
             secret_value = {secret: generate_secret(generate)}
         else:
             secret_value = {secret: ask_secret(self.name, secret)}
 
-        self.client.secrets.kv.create_or_update_secret(
-            path=secret, mount_point=engine, secret=secret_value
-        )
+        self.client.secrets.kv.create_or_update_secret(path=secret, mount_point=engine, secret=secret_value)
```

### Comparing `secenv-1.2.3/secenv/utils.py` & `secenv-1.2.4/secenv/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     sorted_keys = list(secret_def)
     sorted_keys.sort()
 
     # 2) ignore the 'key' and 'store' parameters as they are not used to retrieve
     # a secret directly
     # > 'store' is used in another way to specify where to retrieve the secret from
     # > 'key' is used to extract data from an already retrieved secret
-    filtered_keys = [
-        secret_def[k] for k in sorted_keys if k not in ["key", "store", "sensitive"]
-    ]
+    filtered_keys = [secret_def[k] for k in sorted_keys if k not in ["key", "store", "sensitive"]]
 
     # 3) generate the final string used as the unique ID
     return "-".join([store] + filtered_keys)
 
 
 def yes_no(ask):
     return input(ask + " [yN] ").lower() in ["y", "yes"]
```

### Comparing `secenv-1.2.3/secenv.egg-info/PKG-INFO` & `secenv-1.2.4/secenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.2.3
+Version: 1.2.4
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.2.3/secenv.egg-info/SOURCES.txt` & `secenv-1.2.4/secenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/tests/test_config_file.py` & `secenv-1.2.4/tests/test_config_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     errors = secenv.validate_config()
     assert errors
     assert "Store 'my_store' extends an inexistent store 'nothing'" in errors
 
 
 @with_tmp_conf
 def test_validate_store_both_type_and_extends(config):
-    config_as_py = {
-        "stores": {"my_store": {"extends": "something", "type": "something"}}
-    }
+    config_as_py = {"stores": {"my_store": {"extends": "something", "type": "something"}}}
     write(config, config_as_py)
 
     errors = secenv.validate_config()
     assert errors
     assert "Store 'my_store' contains both 'type' and 'extends' keys" in errors
 
 
@@ -55,17 +53,15 @@
 
     errors = secenv.validate_config()
     assert errors == []
 
 
 @with_tmp_conf
 def test_validate_store_extends_ok(config):
-    config_as_py = {
-        "stores": {"extending": {"extends": "extended"}, "extended": {"type": "type"}}
-    }
+    config_as_py = {"stores": {"extending": {"extends": "extended"}, "extended": {"type": "type"}}}
     write(config, config_as_py)
 
     errors = secenv.validate_config()
     assert errors == []
 
 
 @with_tmp_conf
@@ -137,17 +133,15 @@
 
     errors = secenv.validate_config()
     assert "Context 'ctx' extends an inexistent context 'inexistent'" in errors
 
 
 @with_tmp_conf
 def test_validate_context_extends_ok(config):
-    config_as_py = {
-        "contexts": {"extended": {}, "extending": {"extends": ["extended"]}}
-    }
+    config_as_py = {"contexts": {"extended": {}, "extending": {"extends": ["extended"]}}}
     write(config, config_as_py)
 
     errors = secenv.validate_config()
     assert errors == []
 
 
 @with_tmp_conf
@@ -162,30 +156,24 @@
 
 @with_tmp_conf
 def test_validate_context_vars_key_wrong_type(config):
     config_as_py = {"contexts": {"ctx": {"vars": {"VAR": {"key": True}}}}}
     write(config, config_as_py)
 
     errors = secenv.validate_config()
-    assert (
-        "Secret 'ctx/VAR' defines 'key' with wrong type '<class 'bool'>' (expects 'str')"
-        in errors
-    )
+    assert "Secret 'ctx/VAR' defines 'key' with wrong type '<class 'bool'>' (expects 'str')" in errors
 
 
 @with_tmp_conf
 def test_validate_context_vars_sensitive_wrong_type(config):
     config_as_py = {"contexts": {"ctx": {"vars": {"VAR": {"sensitive": 42}}}}}
     write(config, config_as_py)
 
     errors = secenv.validate_config()
-    assert (
-        "Secret 'ctx/VAR' defines 'sensitive' with wrong type '<class 'int'>' (expects 'bool')"
-        in errors
-    )
+    assert "Secret 'ctx/VAR' defines 'sensitive' with wrong type '<class 'int'>' (expects 'bool')" in errors
 
 
 @with_tmp_conf
 def test_validate_context_vars_store_not_found(config):
     config_as_py = {"contexts": {"ctx": {"vars": {"VAR": {"store": "inexistent"}}}}}
     write(config, config_as_py)
 
@@ -193,17 +181,13 @@
     assert "Secret 'ctx/VAR' references an inexistent store 'inexistent'" in errors
 
 
 @with_tmp_conf
 def test_validate_context_vars_ok(config):
     config_as_py = {
         "stores": {"my_store": {"type": "ok"}},
-        "contexts": {
-            "ctx": {
-                "vars": {"VAR": {"store": "my_store", "secret": "sec"}, "VAR2": "ok"}
-            }
-        },
+        "contexts": {"ctx": {"vars": {"VAR": {"store": "my_store", "secret": "sec"}, "VAR2": "ok"}}},
     }
     write(config, config_as_py)
 
     errors = secenv.validate_config()
     assert errors == []
```

### Comparing `secenv-1.2.3/tests/test_context_output.py` & `secenv-1.2.4/tests/test_context_output.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/tests/test_fill_secrets.py` & `secenv-1.2.4/tests/test_fill_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,15 @@
     assert secret == "yay!"
 
 
 @with_tmp_conf
 def test_generate_dummy(config):
     config_as_py = {
         "stores": {"local": {"type": "env"}},
-        "secrets": [
-            {"secret": "DUMMY", "store": "local", "generate": {"type": "dummy"}}
-        ],
+        "secrets": [{"secret": "DUMMY", "store": "local", "generate": {"type": "dummy"}}],
     }
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
     secenv.fill_secrets(stores)
     secret = secenv.read_secret(stores["local"], {"secret": "DUMMY"})
@@ -76,17 +74,15 @@
         assert letter in string.printable
 
 
 @with_tmp_conf
 def test_generate_password_no_args(config):
     config_as_py = {
         "stores": {"local": {"type": "env"}},
-        "secrets": [
-            {"secret": "NO_ARGS", "store": "local", "generate": {"type": "password"}}
-        ],
+        "secrets": [{"secret": "NO_ARGS", "store": "local", "generate": {"type": "password"}}],
     }
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
     secenv.fill_secrets(stores)
     secret = secenv.read_secret(stores["local"], {"secret": "NO_ARGS"})
```

### Comparing `secenv-1.2.3/tests/test_gen_context.py` & `secenv-1.2.4/tests/test_gen_context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.3/tests/test_stores.py` & `secenv-1.2.4/tests/test_stores.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,17 +157,15 @@
     secenv.load_config()
     stores = secenv.find_stores()
     with pytest.raises(Exception):
         secenv.read_secret(stores["aws"], {"secret": "AWSSecretNameNotExist"})
 
 
 @with_tmp_conf
-@mock.patch(
-    "subprocess.run", return_value=Object(stdout=b"BitwardenSecretValue", returncode=0)
-)
+@mock.patch("subprocess.run", return_value=Object(stdout=b"BitwardenSecretValue", returncode=0))
 def test_store_bitwarden_secret_exists(config, _):
     config_as_py = {"stores": {"bitwarden": {"type": "bitwarden"}}}
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
     secret = secenv.read_secret(stores["bitwarden"], {"secret": "BitwardenSecretName"})
@@ -179,17 +177,15 @@
 def test_store_bitwarden_secret_not_exists(config, _):
     config_as_py = {"stores": {"bitwarden": {"type": "bitwarden"}}}
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
     with pytest.raises(Exception):
-        secenv.read_secret(
-            stores["bitwarden"], {"secret": "BitwardenSecretNameNotExist"}
-        )
+        secenv.read_secret(stores["bitwarden"], {"secret": "BitwardenSecretNameNotExist"})
 
 
 @with_tmp_conf
 def test_store_env_secret_exists(config):
     config_as_py = {"stores": {"local": {"type": "env"}}}
     write(config, config_as_py)
 
@@ -254,36 +250,42 @@
     secret = secenv.read_secret(stores["gcp"], {"secret": "GCPSecretName"})
     assert secret == "GCPSecretValue"
 
 
 @with_tmp_conf
 @mock.patch(
     "google.cloud.secretmanager.SecretManagerServiceClient",
-    return_value=Object(
-        access_secret_version=lambda _: Object(
-            side_effect=GCPSecretNotFoundError("secret")
-        )
-    ),
+    return_value=Object(access_secret_version=lambda _: Object(side_effect=GCPSecretNotFoundError("secret"))),
 )
 def test_store_gcp_secret_not_exists(config, _):
     config_as_py = {"stores": {"gcp": {"type": "gcp", "project_id": "pnf"}}}
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
     with pytest.raises(Exception):
         secenv.read_secret(stores["gcp"], {"secret": "GCPSecretNameNotFound"})
 
 
+@skip_unimplemented_test
+@with_tmp_conf
+def test_store_gcp_fill_secret(config):
+    ...
+
+
+@skip_unimplemented_test
+@with_tmp_conf
+def test_store_gcp_fill_secret_overwrite(config):
+    ...
+
+
 @with_tmp_conf
 @mock.patch(
     "requests.get",
-    return_value=Object(
-        text=json.dumps({"data": base64.b64encode(b"SWSecretValue").decode(), "id": 1})
-    ),
+    return_value=Object(text=json.dumps({"data": base64.b64encode(b"SWSecretValue").decode(), "id": 1})),
 )
 def test_store_scaleway_secret_exists(config, _):
     config_as_py = {
         "stores": {
             "scaleway": {
                 "type": "scaleway",
                 "region": "r",
@@ -320,20 +322,30 @@
 
     secenv.load_config()
     stores = secenv.find_stores()
     with pytest.raises(Exception):
         secenv.read_secret(stores["scaleway"], {"secret": "SWSecretNameNotFound"})
 
 
+@skip_unimplemented_test
+@with_tmp_conf
+def test_store_scaleway_fill_secret(config):
+    ...
+
+
+@skip_unimplemented_test
+@with_tmp_conf
+def test_store_scaleway_fill_secret_overwrite(config):
+    ...
+
+
 @with_tmp_conf
 @mock.patch(
     "hvac.Client",
-    return_value=Object(
-        secrets=Object(kv=Object(read_secret_version=lambda **_: "VaultSecretValue"))
-    ),
+    return_value=Object(secrets=Object(kv=Object(read_secret_version=lambda **_: "VaultSecretValue"))),
 )
 def test_store_vault_secret_exists(config, _):
     config_as_py = {"stores": {"vault": {"type": "vault", "url": "u", "token": "t"}}}
     write(config, config_as_py)
 
     secenv.load_config()
     stores = secenv.find_stores()
@@ -345,17 +357,15 @@
 @mock.patch(
     "hvac.Client",
     return_value=Object(
         secrets=Object(
             kv=Object(
                 # Python doesn't accept this: `lambda _: raise Exception`
                 # so let's make some really pythonic stuff
-                read_secret_version=lambda **_: (_ for _ in ()).throw(
-                    VaultSecretNotFoundError
-                )
+                read_secret_version=lambda **_: (_ for _ in ()).throw(VaultSecretNotFoundError)
             )
         )
     ),
 )
 def test_store_vault_secret_not_exists(config, _):
     config_as_py = {"stores": {"vault": {"type": "vault", "url": "u", "token": "t"}}}
     write(config, config_as_py)
```

### Comparing `secenv-1.2.3/tests/test_utils.py` & `secenv-1.2.4/tests/test_utils.py`

 * *Files identical despite different names*

