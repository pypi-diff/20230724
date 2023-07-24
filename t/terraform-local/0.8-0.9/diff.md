# Comparing `tmp/terraform-local-0.8.tar.gz` & `tmp/terraform-local-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-local-0.8.tar", last modified: Thu Apr 27 08:56:37 2023, max compression
+gzip compressed data, was "terraform-local-0.9.tar", last modified: Wed Jun 21 18:14:58 2023, max compression
```

## Comparing `terraform-local-0.8.tar` & `terraform-local-0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.656624 terraform-local-0.8/
--rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-15 00:02:30.000000 terraform-local-0.8/LICENSE
--rw-r--r--   0 whummer    (501) staff       (20)     3056 2023-04-27 08:56:37.656686 terraform-local-0.8/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     2340 2023-04-27 08:56:05.000000 terraform-local-0.8/README.md
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.655051 terraform-local-0.8/bin/
--rwxr-xr-x   0 whummer    (501) staff       (20)     7328 2023-04-27 08:56:05.000000 terraform-local-0.8/bin/tflocal
--rwxr-xr-x   0 whummer    (501) staff       (20)       37 2022-06-15 00:02:30.000000 terraform-local-0.8/bin/tflocal.bat
--rw-r--r--   0 whummer    (501) staff       (20)      884 2023-04-27 08:56:37.657021 terraform-local-0.8/setup.cfg
--rwxr-xr-x   0 whummer    (501) staff       (20)       61 2022-06-15 00:02:31.000000 terraform-local-0.8/setup.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.655975 terraform-local-0.8/terraform_local.egg-info/
--rw-r--r--   0 whummer    (501) staff       (20)     3056 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)      352 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2022-08-23 10:49:00.000000 terraform-local-0.8/terraform_local.egg-info/not-zip-safe
--rw-r--r--   0 whummer    (501) staff       (20)       63 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/requires.txt
--rw-r--r--   0 whummer    (501) staff       (20)        6 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/top_level.txt
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.656400 terraform-local-0.8/tests/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2022-08-27 23:32:12.000000 terraform-local-0.8/tests/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)      228 2022-08-27 23:01:35.000000 terraform-local-0.8/tests/conftest.py
--rw-r--r--   0 whummer    (501) staff       (20)     2850 2023-03-28 11:59:17.000000 terraform-local-0.8/tests/test_apply.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-21 18:14:58.091856 terraform-local-0.9/
+-rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-15 00:02:30.000000 terraform-local-0.9/LICENSE
+-rw-r--r--   0 whummer    (501) staff       (20)     3116 2023-06-21 18:14:58.091915 terraform-local-0.9/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     2400 2023-06-21 18:14:41.000000 terraform-local-0.9/README.md
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-21 18:14:58.090775 terraform-local-0.9/bin/
+-rwxr-xr-x   0 whummer    (501) staff       (20)     7357 2023-06-21 18:14:41.000000 terraform-local-0.9/bin/tflocal
+-rwxr-xr-x   0 whummer    (501) staff       (20)       37 2022-06-15 00:02:30.000000 terraform-local-0.9/bin/tflocal.bat
+-rw-r--r--   0 whummer    (501) staff       (20)      884 2023-06-21 18:14:58.092213 terraform-local-0.9/setup.cfg
+-rwxr-xr-x   0 whummer    (501) staff       (20)       61 2022-06-15 00:02:31.000000 terraform-local-0.9/setup.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-21 18:14:58.091421 terraform-local-0.9/terraform_local.egg-info/
+-rw-r--r--   0 whummer    (501) staff       (20)     3116 2023-06-21 18:14:58.000000 terraform-local-0.9/terraform_local.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)      352 2023-06-21 18:14:58.000000 terraform-local-0.9/terraform_local.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2023-06-21 18:14:58.000000 terraform-local-0.9/terraform_local.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2022-08-23 10:49:00.000000 terraform-local-0.9/terraform_local.egg-info/not-zip-safe
+-rw-r--r--   0 whummer    (501) staff       (20)       63 2023-06-21 18:14:58.000000 terraform-local-0.9/terraform_local.egg-info/requires.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        6 2023-06-21 18:14:58.000000 terraform-local-0.9/terraform_local.egg-info/top_level.txt
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-21 18:14:58.091754 terraform-local-0.9/tests/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2022-08-27 23:32:12.000000 terraform-local-0.9/tests/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)      228 2022-08-27 23:01:35.000000 terraform-local-0.9/tests/conftest.py
+-rw-r--r--   0 whummer    (501) staff       (20)     2850 2023-03-28 11:59:17.000000 terraform-local-0.9/tests/test_apply.py
```

### Comparing `terraform-local-0.8/LICENSE` & `terraform-local-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-local-0.8/PKG-INFO` & `terraform-local-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-local
-Version: 0.8
+Version: 0.9
 Summary: Thin wrapper script to run Terraform against LocalStack
 Home-page: https://github.com/localstack/terraform-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.9: Fix unsupported provider override for emrserverless
 * v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
```

### Comparing `terraform-local-0.8/README.md` & `terraform-local-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.9: Fix unsupported provider override for emrserverless
 * v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
```

### Comparing `terraform-local-0.8/bin/tflocal` & `terraform-local-0.9/bin/tflocal`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     provider_aliases = provider_aliases or []
 
     # maps services to be replaced with alternative names
     service_replaces = {
         "apigatewaymanagementapi": "",
         "ce": "costexplorer",
         "edge": "",
+        "emrserverless": "",
         "iotdata": "",
         "iotjobsdata": "",
         "logs": "cloudwatchlogs",
         "timestream": ""
     }
     # service names to be excluded (not yet available in TF)
     service_excludes = ["meteringmarketplace"]
```

### Comparing `terraform-local-0.8/setup.cfg` & `terraform-local-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = terraform-local
-version = 0.8
+version = 0.9
 url = https://github.com/localstack/terraform-local
 author = LocalStack Team
 author_email = info@localstack.cloud
 description = Thin wrapper script to run Terraform against LocalStack
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
```

### Comparing `terraform-local-0.8/terraform_local.egg-info/PKG-INFO` & `terraform-local-0.9/terraform_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-local
-Version: 0.8
+Version: 0.9
 Summary: Thin wrapper script to run Terraform against LocalStack
 Home-page: https://github.com/localstack/terraform-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.9: Fix unsupported provider override for emrserverless
 * v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
```

### Comparing `terraform-local-0.8/tests/test_apply.py` & `terraform-local-0.9/tests/test_apply.py`

 * *Files identical despite different names*

