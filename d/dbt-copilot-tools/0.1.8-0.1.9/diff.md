# Comparing `tmp/dbt_copilot_tools-0.1.8.tar.gz` & `tmp/dbt_copilot_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.8.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.9.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.8.tar` & `dbt_copilot_tools-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0    12476 2023-07-20 14:40:32.289038 dbt_copilot_tools-0.1.8/commands/COMMANDS.md
--rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.8/commands/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.8/commands/__init__.py
--rwxr-xr-x   0        0        0     9834 2023-06-30 15:36:41.153299 dbt_copilot_tools-0.1.8/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0     2563 2023-07-14 15:07:33.244634 dbt_copilot_tools-0.1.8/commands/check_cloudformation.py
--rwxr-xr-x   0        0        0    13567 2023-07-20 11:58:54.500816 dbt_copilot_tools-0.1.8/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     7006 2023-07-20 14:52:58.636758 dbt_copilot_tools-0.1.8/commands/copilot_cli.py
--rw-r--r--   0        0        0      221 2023-07-20 14:52:58.637154 dbt_copilot_tools-0.1.8/commands/default-storage.yml
--rwxr-xr-x   0        0        0    20986 2023-07-14 15:07:33.244923 dbt_copilot_tools-0.1.8/commands/dns_cli.py
--rw-r--r--   0        0        0    10705 2023-07-20 14:52:58.637346 dbt_copilot_tools-0.1.8/commands/schemas/storage-schema.json
--rw-r--r--   0        0        0     4141 2023-07-20 14:52:58.638060 dbt_copilot_tools-0.1.8/commands/storage-plans.yml
--rw-r--r--   0        0        0     1081 2023-07-20 11:58:54.501083 dbt_copilot_tools-0.1.8/commands/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      412 2023-07-20 11:58:54.501306 dbt_copilot_tools-0.1.8/commands/templates/addons/README.md
--rw-r--r--   0        0        0      529 2023-07-20 14:52:58.638828 dbt_copilot_tools-0.1.8/commands/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0     6148 2023-07-20 11:58:54.501686 dbt_copilot_tools-0.1.8/commands/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     8690 2023-07-20 14:52:58.639317 dbt_copilot_tools-0.1.8/commands/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0     4622 2023-07-20 13:18:17.158455 dbt_copilot_tools-0.1.8/commands/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     4062 2023-07-20 11:58:54.502157 dbt_copilot_tools-0.1.8/commands/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     3945 2023-07-20 13:18:17.158705 dbt_copilot_tools-0.1.8/commands/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     1778 2023-07-20 11:58:54.502526 dbt_copilot_tools-0.1.8/commands/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0     1836 2023-07-20 11:58:54.502669 dbt_copilot_tools-0.1.8/commands/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2023-07-20 11:58:54.502781 dbt_copilot_tools-0.1.8/commands/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2023-07-20 11:58:54.502929 dbt_copilot_tools-0.1.8/commands/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      728 2023-07-20 14:52:58.639746 dbt_copilot_tools-0.1.8/commands/templates/env/manifest.yml
--rw-r--r--   0        0        0     2721 2023-07-20 11:58:54.503273 dbt_copilot_tools-0.1.8/commands/templates/instructions.txt
--rw-r--r--   0        0        0      610 2023-07-20 11:58:54.503399 dbt_copilot_tools-0.1.8/commands/templates/storage-instructions.txt
--rw-r--r--   0        0        0     1848 2023-07-20 13:18:17.159484 dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3115 2023-07-20 13:18:17.159767 dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0     5894 2023-07-20 11:58:54.504032 dbt_copilot_tools-0.1.8/commands/utils.py
--rw-r--r--   0        0        0     6007 2023-07-14 15:07:33.245135 dbt_copilot_tools-0.1.8/commands/waf_cli.py
--rwxr-xr-x   0        0        0      970 2023-06-28 12:16:25.470546 dbt_copilot_tools-0.1.8/copilot_helper.py
--rw-r--r--   0        0        0     1102 2023-07-20 14:52:58.640166 dbt_copilot_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0    12476 2023-07-24 08:45:40.845900 dbt_copilot_tools-0.1.9/commands/COMMANDS.md
+-rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.9/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.9/commands/__init__.py
+-rwxr-xr-x   0        0        0     9834 2023-06-30 15:36:41.153299 dbt_copilot_tools-0.1.9/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2772 2023-07-24 17:42:43.787319 dbt_copilot_tools-0.1.9/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13567 2023-07-20 11:58:54.500816 dbt_copilot_tools-0.1.9/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     7231 2023-07-24 17:42:43.787606 dbt_copilot_tools-0.1.9/commands/copilot_cli.py
+-rw-r--r--   0        0        0      221 2023-07-20 14:54:09.361493 dbt_copilot_tools-0.1.9/commands/default-storage.yml
+-rwxr-xr-x   0        0        0    20986 2023-07-14 15:07:33.244923 dbt_copilot_tools-0.1.9/commands/dns_cli.py
+-rw-r--r--   0        0        0    10705 2023-07-20 14:54:09.361653 dbt_copilot_tools-0.1.9/commands/schemas/storage-schema.json
+-rw-r--r--   0        0        0     4141 2023-07-20 14:54:09.361781 dbt_copilot_tools-0.1.9/commands/storage-plans.yml
+-rw-r--r--   0        0        0     1081 2023-07-20 11:58:54.501083 dbt_copilot_tools-0.1.9/commands/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      412 2023-07-20 11:58:54.501306 dbt_copilot_tools-0.1.9/commands/templates/addons/README.md
+-rw-r--r--   0        0        0      529 2023-07-20 15:42:31.049003 dbt_copilot_tools-0.1.9/commands/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0     6148 2023-07-20 11:58:54.501686 dbt_copilot_tools-0.1.9/commands/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     8690 2023-07-20 15:42:31.049484 dbt_copilot_tools-0.1.9/commands/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0     4622 2023-07-20 13:18:17.158455 dbt_copilot_tools-0.1.9/commands/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     4062 2023-07-20 11:58:54.502157 dbt_copilot_tools-0.1.9/commands/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     3945 2023-07-20 13:18:17.158705 dbt_copilot_tools-0.1.9/commands/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     1778 2023-07-20 11:58:54.502526 dbt_copilot_tools-0.1.9/commands/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0     1836 2023-07-20 11:58:54.502669 dbt_copilot_tools-0.1.9/commands/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2023-07-20 11:58:54.502781 dbt_copilot_tools-0.1.9/commands/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2023-07-20 11:58:54.502929 dbt_copilot_tools-0.1.9/commands/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      728 2023-07-20 15:42:31.049801 dbt_copilot_tools-0.1.9/commands/templates/env/manifest.yml
+-rw-r--r--   0        0        0     2721 2023-07-20 11:58:54.503273 dbt_copilot_tools-0.1.9/commands/templates/instructions.txt
+-rw-r--r--   0        0        0      610 2023-07-20 11:58:54.503399 dbt_copilot_tools-0.1.9/commands/templates/storage-instructions.txt
+-rw-r--r--   0        0        0     1848 2023-07-20 13:18:17.159484 dbt_copilot_tools-0.1.9/commands/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3115 2023-07-20 13:18:17.159767 dbt_copilot_tools-0.1.9/commands/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0     5890 2023-07-24 17:42:43.788010 dbt_copilot_tools-0.1.9/commands/utils.py
+-rw-r--r--   0        0        0     6007 2023-07-14 15:07:33.245135 dbt_copilot_tools-0.1.9/commands/waf_cli.py
+-rwxr-xr-x   0        0        0      970 2023-06-28 12:16:25.470546 dbt_copilot_tools-0.1.9/copilot_helper.py
+-rw-r--r--   0        0        0     1102 2023-07-24 17:42:43.788249 dbt_copilot_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.9/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.8/LICENSE` & `dbt_copilot_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/COMMANDS.md` & `dbt_copilot_tools-0.1.9/commands/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/README.md` & `dbt_copilot_tools-0.1.9/commands/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.9/commands/bootstrap_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/check_cloudformation.py` & `dbt_copilot_tools-0.1.9/commands/check_cloudformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,21 @@
     if ctx.invoked_subcommand is None:
         click.secho(f"\n>>> Running all checks", fg="yellow")
         for name, command in ctx.command.commands.items():
             ctx.invoke(command)
 
 
 def get_lint_result(path: str):
-    command = ["cfn-lint", path]
+    command = [
+        "cfn-lint",
+        path,
+        "--ignore-templates",
+        # addons.parameters.yml is not a CloudFormation template file
+        f"{BASE_DIR}/tests/test-application/copilot/**/addons/addons.parameters.yml",
+    ]
 
     click.secho(f"\n>>> Running lint check", fg="yellow")
     click.secho(f"""    {" ".join(command)}\n""", fg="yellow")
 
     return run(command, capture_output=True)
```

### Comparing `dbt_copilot_tools-0.1.8/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.9/commands/codebuild_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.9/commands/copilot_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,19 @@
             "prefix": camel_case(storage_name),
             "storage_type": storage_type,
             **storage_config,
         }
 
         services.append(service)
 
+        if storage_type not in ["s3", "s3-policy"]:
+            contents = templates["env"]["parameters"].render({})
+
+            click.echo(mkfile(output_dir, path / "addons.parameters.yml", contents, overwrite=overwrite))
+
         # s3-policy only applies to individual services
         if storage_type != "s3-policy":
             template = templates["env"][storage_type]
             contents = template.render({"service": service})
 
             click.echo(mkfile(output_dir, path / f"{storage_name}.yml", contents, overwrite=overwrite))
```

### Comparing `dbt_copilot_tools-0.1.8/commands/dns_cli.py` & `dbt_copilot_tools-0.1.9/commands/dns_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/schemas/storage-schema.json` & `dbt_copilot_tools-0.1.9/commands/schemas/storage-schema.json`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/storage-plans.yml` & `dbt_copilot_tools-0.1.9/commands/storage-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/COMMANDS.md.jinja` & `dbt_copilot_tools-0.1.9/commands/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/addons.parameters.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/aurora-postgres.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/opensearch.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/rds-postgres.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/redis-cluster.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/env/s3.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/addons/svc/s3-policy.yml` & `dbt_copilot_tools-0.1.9/commands/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/ci-codebuild-role-policy.json` & `dbt_copilot_tools-0.1.9/commands/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/custom-codebuild-role-policy.json` & `dbt_copilot_tools-0.1.9/commands/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/env/manifest.yml` & `dbt_copilot_tools-0.1.9/commands/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/instructions.txt` & `dbt_copilot_tools-0.1.9/commands/templates/instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/storage-instructions.txt` & `dbt_copilot_tools-0.1.9/commands/templates/storage-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-backend.yml` & `dbt_copilot_tools-0.1.9/commands/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-public.yml` & `dbt_copilot_tools-0.1.9/commands/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/commands/utils.py` & `dbt_copilot_tools-0.1.9/commands/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 def check_aws_conn(aws_profile: str) -> boto3.session.Session:
     # Check that the aws profile exists and is set.
     click.secho("Checking AWS connection...", fg="cyan")
 
     try:
         session = boto3.session.Session(profile_name=aws_profile)
     except botocore.exceptions.ProfileNotFound:
-        click.secho("AWS profile not configured, please ensure they are set.", fg="red")
+        click.secho(f"""AWS profile "{aws_profile}" is not configured.""", fg="red")
         exit()
     except botocore.errorfactory.UnauthorizedException:
         click.secho(
             "The SSO session associated with this profile has expired or is otherwise invalid.  "
             "To refresh this SSO session run aws sso login with the corresponding profile",
             fg="red",
         )
```

### Comparing `dbt_copilot_tools-0.1.8/commands/waf_cli.py` & `dbt_copilot_tools-0.1.9/commands/waf_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/copilot_helper.py` & `dbt_copilot_tools-0.1.9/copilot_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.8/pyproject.toml` & `dbt_copilot_tools-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.8"
+version = "0.1.9"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "commands/README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
```

### Comparing `dbt_copilot_tools-0.1.8/PKG-INFO` & `dbt_copilot_tools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

