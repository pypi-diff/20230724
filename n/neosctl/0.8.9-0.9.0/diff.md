# Comparing `tmp/neosctl-0.8.9.tar.gz` & `tmp/neosctl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.9.tar", max compression
+gzip compressed data, was "neosctl-0.9.0.tar", max compression
```

## Comparing `neosctl-0.8.9.tar` & `neosctl-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-07-06 12:44:12.933411 neosctl-0.8.9/README.md
--rw-r--r--   0        0        0       22 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3564 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     5684 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3243 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      122 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     7848 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12904 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-07-06 12:44:12.935411 neosctl-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     2962 2023-07-24 12:05:12.994174 neosctl-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/constant.py
+-rw-r--r--   0        0        0     4654 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/profile.py
+-rw-r--r--   0        0        0     2668 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-07-24 12:05:12.995174 neosctl-0.9.0/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3490 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0    14484 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0     1283 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      184 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     7848 2023-07-24 12:05:12.996174 neosctl-0.9.0/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    14103 2023-07-24 12:05:12.997174 neosctl-0.9.0/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-07-24 12:05:12.997174 neosctl-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 neosctl-0.9.0/PKG-INFO
```

### Comparing `neosctl-0.8.9/README.md` & `neosctl-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.9
+# Core CLI v0.9.0
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
@@ -108,14 +108,25 @@
 ```bash
 $ neosctl product get my-data-product
 ...
 $ export NEOSCTL_PRODUCT=my-data-product
 $ neosctl product get
 ```
 
+## Generate docs
+
+To generate docs in a markdown format, run the following command.
+The output DOCS.md file could be used to update the NEOS documentation site
+([docs.neosmesh.com](https://docs.neosmesh.com)).
+
+```bash
+pip install typer-cli
+typer neosctl.cli utils docs --name neosctl --output DOCS.md
+```
+
 ## Releases
 
 Release management is handled using `bump2version`. The below commands will tag
 a new release. This will also update the helm chart version, this should not be
 manually changed.
 
 ```bash
```

### Comparing `neosctl-0.8.9/neosctl/auth.py` & `neosctl-0.9.0/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/cli.py` & `neosctl-0.9.0/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/profile.py` & `neosctl-0.9.0/neosctl/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     *,
     hostname: typing.Optional[str] = typer.Option(None, "--host", "-h", callback=util.sanitize),
     gateway_api_url: typing.Optional[str] = typer.Option(None, "--gateway-api-url", "-g", callback=util.sanitize),
     registry_api_url: typing.Optional[str] = typer.Option(None, "--registry-api-url", "-r", callback=util.sanitize),
     iam_api_url: typing.Optional[str] = typer.Option(None, "--iam-api-url", "-i", callback=util.sanitize),
     storage_api_url: typing.Optional[str] = typer.Option(None, "--storage-api-url", "-s", callback=util.sanitize),
     username: typing.Optional[str] = typer.Option(None, "--username", "-u", callback=util.sanitize),
+    account: typing.Optional[str] = typer.Option("root", "--account", "-a", callback=util.sanitize),
     ignore_tls: bool = typer.Option(
         False,
         "--ignore-tls",
         help="Ignore TLS errors (useful in local/development environments",
     ),
     non_interactive: bool = typer.Option(
         False,
@@ -97,14 +98,15 @@
             "Username",
             **kwargs,
         )
         username = username_input
 
     profile = schema.Profile(  # nosec: B106
         user=username,
+        account=account,
         access_token="",
         refresh_token="",
         ignore_tls=ignore_tls,
         **urls,
     )
 
     upsert_config(ctx, profile)
```

### Comparing `neosctl-0.8.9/neosctl/schema.py` & `neosctl-0.9.0/neosctl/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,37 +17,46 @@
     registry_api_url: str = ""
     iam_api_url: str = ""
     storage_api_url: str = ""
     user: str = ""
     access_token: str = ""
     refresh_token: str = ""
     ignore_tls: bool = False
+    account: str = ""
 
 
 class Profile(OptionalProfile):
     gateway_api_url: str
     registry_api_url: str
     iam_api_url: str
     storage_api_url: str
     user: str
     access_token: str
     refresh_token: str
     ignore_tls: bool
+    account: str = "root"  # backwards compat default
 
 
 @dataclasses.dataclass
 class Common:
     gateway_api_url: str
     registry_api_url: str
     iam_api_url: str
     storage_api_url: str
     profile_name: str
     config: configparser.ConfigParser
     profile: Optional[Union[Profile, OptionalProfile]]
 
+    def get_account(self) -> str:
+        """Return system account."""
+        if self.profile:
+            return self.profile.account
+
+        return "root"
+
     def get_gateway_api_url(self) -> str:
         """Return gateway api url.
 
         If a user profile is provided and defines a gateway url, return that,
         otherwise or fall back to cli defined default.
         """
         if self.profile and self.profile.gateway_api_url:
```

### Comparing `neosctl-0.8.9/neosctl/services/gateway/__init__.py` & `neosctl-0.9.0/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/data_product.py` & `neosctl-0.9.0/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/data_source.py` & `neosctl-0.9.0/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/data_system.py` & `neosctl-0.9.0/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/data_unit.py` & `neosctl-0.9.0/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/entity.py` & `neosctl-0.9.0/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/link.py` & `neosctl-0.9.0/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/output.py` & `neosctl-0.9.0/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/schema.py` & `neosctl-0.9.0/neosctl/services/gateway/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,31 +34,25 @@
 
 
 class JournalEntry(BaseModel):
     note: str
 
 
 class FieldMetadata(BaseModel):
-    field: str
-    tag: Optional[str]
+    tags: Optional[List[str]]
     description: Optional[str]
 
 
-class FieldMetadataWithTag(BaseModel):
-    field: str
-    tag: str
-
-
 class UpdateEntityMetadataRequest(BaseModel):
-    fields: List[FieldMetadata]
+    fields: Dict[str, FieldMetadata]
     tags: List[str]
 
 
 class DeleteEntityMetadataRequest(BaseModel):
-    fields: List[FieldMetadataWithTag]
+    fields: Dict[str, FieldMetadata]
     tags: List[str]
 
 
 class FieldDataType(pydantic.BaseModel):
     meta: Dict[str, str]
     column_type: str
```

### Comparing `neosctl-0.8.9/neosctl/services/gateway/secret.py` & `neosctl-0.9.0/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/spark.py` & `neosctl-0.9.0/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/gateway/tag.py` & `neosctl-0.9.0/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/services/registry/registry.py` & `neosctl-0.9.0/neosctl/services/registry/registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import httpx
 import typer
 
 from neosctl import util
-from neosctl.services.registry.schema import RegisterCore, RemoveCore
+from neosctl.services.registry.schema import MigrateCore, RegisterCore, RemoveCore
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _core_url(registry_api_url: str) -> str:
     return "{}/core".format(registry_api_url.rstrip("/"))
@@ -38,14 +38,42 @@
 
     rc = RegisterCore(name=name)
 
     r = _request(ctx, rc)
     process_response(r)
 
 
+@app.command(name="migrate-core")
+def migrate_core(
+    ctx: typer.Context,
+    urn: str = typer.Option(..., help="Core urn", callback=util.sanitize),
+    account: str = typer.Option(..., help="Account name", callback=util.sanitize),
+) -> None:
+    """Migrate a core out of root account.
+
+    Migrate a core from `root` into an actual account.
+    """
+
+    @util.ensure_login
+    def _request(ctx: typer.Context, mc: MigrateCore) -> httpx.Response:
+        return util.post(
+            ctx,
+            f"{_core_url(ctx.obj.get_registry_api_url())}/migrate",
+            json=mc.dict(),
+        )
+
+    mc = MigrateCore(
+        urn=urn,
+        account=account,
+    )
+
+    r = _request(ctx, mc)
+    process_response(r)
+
+
 @app.command(name="list-cores")
 def list_cores(
     ctx: typer.Context,
     search: str = typer.Option(None, help="Search core name(s)", callback=util.sanitize),
 ) -> None:
     """List existing registered cores."""
```

### Comparing `neosctl-0.8.9/neosctl/services/storage/storage.py` & `neosctl-0.9.0/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.9/neosctl/util.py` & `neosctl-0.9.0/neosctl/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,26 +108,26 @@
     )
 
 
 def _auth_url(iam_api_url: str) -> str:
     return "{}".format(iam_api_url.rstrip("/"))
 
 
-def check_refresh_token_exists(ctx: click.Context) -> bool:
+def check_refresh_token_exists(ctx: typer.Context) -> bool:
     """Check if refresh token exists."""
     if not ctx.obj.profile.refresh_token:  # nosec: B105
         raise exit_with_output(
             msg=f"You need to login. Run neosctl -p {ctx.obj.profile_name} auth login",
             exit_code=1,
         )
 
     return True
 
 
-def _refresh_token(ctx: click.Context) -> httpx.Response:
+def _refresh_token(ctx: typer.Context) -> httpx.Response:
     check_profile_exists(ctx)
     check_refresh_token_exists(ctx)
 
     r = post(
         ctx,
         f"{_auth_url(ctx.obj.get_iam_api_url())}/refresh",
         json={"refresh_token": ctx.obj.profile.refresh_token},
@@ -149,15 +149,15 @@
 
     On request failure check if the response is a 401, and attempt to refresh the access_token.
     Retry the request with refreshed token, on subsequent failure, return.
     """
 
     def check_access_token(*args: P.args, **kwargs: P.kwargs) -> httpx.Response:
         ctx = args[0]
-        if not isinstance(ctx, click.Context):
+        if not isinstance(ctx, (typer.Context, click.Context)):
             # Developer reminder
             msg = "First argument should be click.Context instance"
             raise TypeError(msg)
 
         r = method(*args, **kwargs)
 
         check_profile_exists(ctx)
@@ -178,15 +178,15 @@
 
         return r
 
     return check_access_token
 
 
 def update_profile(
-    ctx: click.Context,
+    ctx: typer.Context,
     auth: schema.Auth = schema.Auth(),
 ) -> schema.Profile:
     """Update user profile."""
     return schema.Profile(
         gateway_api_url=ctx.obj.gateway_api_url,
         registry_api_url=ctx.obj.registry_api_url,
         iam_api_url=ctx.obj.iam_api_url,
@@ -224,48 +224,48 @@
                     profile_name,
                 ),
                 exit_code=1,
             )
     return None
 
 
-def bearer(ctx: click.Context) -> typing.Optional[typing.Dict]:
+def bearer(ctx: typer.Context) -> typing.Optional[typing.Dict]:
     """Generate bearer authorization header."""
     if not (ctx.obj.profile and ctx.obj.profile.access_token):  # nosec: B105
         return None
 
     return {"Authorization": f"Bearer {ctx.obj.profile.access_token}"}
 
 
-def check_profile_exists(ctx: click.Context) -> bool:
+def check_profile_exists(ctx: typer.Context) -> bool:
     """Check if a profile exists in neosctl configuration or exit."""
     if not ctx.obj.profile:
         raise exit_with_output(
             msg=f"Profile not found! Run neosctl -p {ctx.obj.profile_name} profile init",
             exit_code=1,
         )
 
     return True
 
 
 def upsert_config(
-    ctx: click.Context,
+    ctx: typer.Context,
     profile: schema.Profile,
 ) -> configparser.ConfigParser:
     """Update neosctl configuration profile in place."""
     ctx.obj.config[ctx.obj.profile_name] = profile.dict()
 
     with constant.PROFILE_FILEPATH.open("w") as profile_file:
         ctx.obj.config.write(profile_file)
 
     return ctx.obj.config
 
 
 def remove_config(
-    ctx: click.Context,
+    ctx: typer.Context,
 ) -> configparser.ConfigParser:
     """Remove a profile from neosctl configuration."""
     if not ctx.obj.config.remove_section(ctx.obj.profile_name):
         raise exit_with_output(
             msg=f"Can not remove {ctx.obj.profile_name} profile, profile not found.",
             exit_code=1,
         )
@@ -305,121 +305,147 @@
 T = typing.TypeVar("T", bound=pydantic.BaseModel)
 
 
 def load_object(t: typing.Type[T], filepath: str, file_description: str) -> T:
     """Trying to read and parse JSON file into the given data type."""
     fp = get_file_location(filepath)
     obj = load_json_file(fp, file_description)
-    return t(**obj)
+    if not isinstance(obj, dict):
+        raise exit_with_output(
+            msg=f"Require a json file containing an object, `{type(obj)}` provided.",
+            exit_code=1,
+        )
+    try:
+        return t(**obj)
+    except pydantic.error_wrappers.ValidationError as e:
+        raise exit_with_output(
+            msg=str(e),
+            exit_code=1,
+        ) from e
 
 
-def _request(ctx: click.Context, method: str, url: str, **kwargs: ...) -> httpx.Response:
+def _request(ctx: typer.Context, method: str, url: str, **kwargs: ...) -> httpx.Response:
     headers = bearer(ctx) or {}
-    headers_ = kwargs.pop("headers", {})
+
+    headers_ = kwargs.pop("headers", None) or {}
     headers.update(headers_)
-    return httpx.request(method=method, url=url, headers=headers, verify=not ctx.obj.profile.ignore_tls, **kwargs)
+
+    headers_, params_ = extract_account(ctx, account=kwargs.pop("account", None))
+    headers.update(headers_)
+
+    params = kwargs.pop("params", None) or {}
+    params.update(params_ or {})
+
+    return httpx.request(
+        method=method,
+        url=url,
+        headers=headers,
+        params=params,
+        verify=not ctx.obj.profile.ignore_tls,
+        **kwargs,
+    )
 
 
-def _request_and_process(ctx: click.Context, method: str, url: str, **kwargs: ...) -> None:
+def _request_and_process(ctx: typer.Context, method: str, url: str, **kwargs: ...) -> None:
     @ensure_login
-    def internal_request(context: click.Context) -> httpx.Response:
+    def internal_request(context: typer.Context) -> httpx.Response:
         return _request(context, method, url, **kwargs)
 
     response = internal_request(ctx)
     process_response(response)
 
 
-def get_and_process(ctx: click.Context, url: str, **kwargs: ...) -> None:
+def get_and_process(ctx: typer.Context, url: str, **kwargs: ...) -> None:
     """Execute and process GET request."""
     _request_and_process(ctx, "GET", url, **kwargs)
 
 
-def post_and_process(ctx: click.Context, url: str, **kwargs: ...) -> None:
+def post_and_process(ctx: typer.Context, url: str, **kwargs: ...) -> None:
     """Execute and process POST request."""
     _request_and_process(ctx, "POST", url, **kwargs)
 
 
-def put_and_process(ctx: click.Context, url: str, **kwargs: ...) -> None:
+def put_and_process(ctx: typer.Context, url: str, **kwargs: ...) -> None:
     """Execute and process PUT request."""
     _request_and_process(ctx, "PUT", url, **kwargs)
 
 
-def delete_and_process(ctx: click.Context, url: str, **kwargs: ...) -> None:
+def delete_and_process(ctx: typer.Context, url: str, **kwargs: ...) -> None:
     """Execute and process DELETE request."""
     _request_and_process(ctx, "DELETE", url, **kwargs)
 
 
-def patch_and_process(ctx: click.Context, url: str, **kwargs: ...) -> None:
+def patch_and_process(ctx: typer.Context, url: str, **kwargs: ...) -> None:
     """Execute and process PATCH request."""
     _request_and_process(ctx, "PATCH", url, **kwargs)
 
 
-def get(ctx: click.Context, url: str, **kwargs: ...) -> httpx.Response:
+def get(ctx: typer.Context, url: str, **kwargs: ...) -> httpx.Response:
     """Execute a GET request."""
     return _request(ctx, "GET", url, **kwargs)
 
 
-def post(ctx: click.Context, url: str, **kwargs: ...) -> httpx.Response:
+def post(ctx: typer.Context, url: str, **kwargs: ...) -> httpx.Response:
     """Execute a POST request."""
     return _request(ctx, "POST", url, **kwargs)
 
 
-def put(ctx: click.Context, url: str, **kwargs: ...) -> httpx.Response:
+def put(ctx: typer.Context, url: str, **kwargs: ...) -> httpx.Response:
     """Execute a PUT request."""
     return _request(ctx, "PUT", url, **kwargs)
 
 
-def delete(ctx: click.Context, url: str, **kwargs: ...) -> httpx.Response:
+def delete(ctx: typer.Context, url: str, **kwargs: ...) -> httpx.Response:
     """Execute a DELETE request."""
     return _request(ctx, "DELETE", url, **kwargs)
 
 
 def sanitize(
-    ctx: click.Context,  # noqa: ARG001
+    ctx: typer.Context,  # noqa: ARG001
     param: click.Parameter,  # noqa: ARG001
     value: typing.Optional[str],
 ) -> typing.Optional[str]:
     """Parameter's sanitize callback."""
     if value and isinstance(value, str):
         return value.rstrip("\r\n")
 
     return value
 
 
 def validate_string_not_empty(
-    ctx: click.Context,
+    ctx: typer.Context,
     param: click.Parameter,
     value: str,
 ) -> str:
     """String validation callback."""
     value = value.strip()
 
     if not value:
         message = "Value must be a non-empty string."
         raise typer.BadParameter(message, ctx=ctx, param=param)
 
     return value
 
 
 def validate_strings_are_not_empty(
-    ctx: click.Context,
+    ctx: typer.Context,
     param: click.Parameter,
     values: typing.List[str],
 ) -> typing.List[str]:
     """List of strings validation callback."""
     return [validate_string_not_empty(ctx, param, value) for value in values]
 
 
 def validate_regex(
     pattern: str,
-) -> typing.Callable[[click.Context, click.Parameter, str], str]:
+) -> typing.Callable[[typer.Context, click.Parameter, str], str]:
     """Regex validation callback."""
 
     def factory(
-        ctx: click.Context,
+        ctx: typer.Context,
         param: click.Parameter,
         value: str,
     ) -> str:
         value = value.strip()
 
         if not re.match(pattern, value):
             message = f"Value does not satisfy the rule {pattern}"
@@ -432,7 +458,25 @@
 
 def user_profile_callback(
     ctx: typer.Context,
 ) -> None:
     """Inject required user_profile into context."""
     user_profile = get_user_profile(ctx.obj.config, ctx.obj.profile_name)
     ctx.obj.profile = user_profile
+
+
+def extract_account(
+    ctx: typer.Context,
+    account: typing.Optional[str] = None,
+) -> typing.Tuple[dict, typing.Optional[dict]]:
+    """Set up account header and params."""
+    profile_account = ctx.obj.get_account()
+    if profile_account != "root" and account is not None:
+        raise exit_with_output(
+            msg="Only root account admins can impersonate other accounts.",
+            exit_code=1,
+        )
+
+    headers = {"X-Account": profile_account}
+    params = {"account": account} if account else None
+
+    return headers, params
```

### Comparing `neosctl-0.8.9/pyproject.toml` & `neosctl-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.9"
+version = "0.9.0"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.9/PKG-INFO` & `neosctl-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.9
+Version: 0.9.0
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.9
+# Core CLI v0.9.0
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
@@ -131,14 +131,25 @@
 ```bash
 $ neosctl product get my-data-product
 ...
 $ export NEOSCTL_PRODUCT=my-data-product
 $ neosctl product get
 ```
 
+## Generate docs
+
+To generate docs in a markdown format, run the following command.
+The output DOCS.md file could be used to update the NEOS documentation site
+([docs.neosmesh.com](https://docs.neosmesh.com)).
+
+```bash
+pip install typer-cli
+typer neosctl.cli utils docs --name neosctl --output DOCS.md
+```
+
 ## Releases
 
 Release management is handled using `bump2version`. The below commands will tag
 a new release. This will also update the helm chart version, this should not be
 manually changed.
 
 ```bash
```

