# Comparing `tmp/lumacli-0.0.3.tar.gz` & `tmp/lumacli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lumacli-0.0.3.tar` & `lumacli-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,29 @@
--rw-r--r--   0        0        0      821 2023-06-28 13:48:32.641571 lumacli-0.0.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3145 2023-06-28 13:48:32.641571 lumacli-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2023-06-28 13:48:32.641571 lumacli-0.0.3/LICENSE
--rw-r--r--   0        0        0     2338 2023-06-28 13:48:32.641571 lumacli-0.0.3/README.md
--rw-r--r--   0        0        0      502 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/__init__.py
--rw-r--r--   0        0        0     2367 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/common.py
--rw-r--r--   0        0        0     6050 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/dbt.py
--rw-r--r--   0        0        0      323 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/luma.py
--rw-r--r--   0        0        0        0 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     8087 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/tests/catalog.json
--rw-r--r--   0        0        0   173474 2023-06-28 13:48:32.641571 lumacli-0.0.3/lumaCLI/tests/manifest.json
--rw-r--r--   0        0        0    10271 2023-06-28 13:48:32.645571 lumacli-0.0.3/lumaCLI/tests/run_results.json
--rw-r--r--   0        0        0     9716 2023-06-28 13:48:32.645571 lumacli-0.0.3/lumaCLI/tests/sources.json
--rw-r--r--   0        0        0      330 2023-06-28 13:48:32.645571 lumacli-0.0.3/lumaCLI/tests/test_common.py
--rw-r--r--   0        0        0      396 2023-06-28 13:48:32.645571 lumacli-0.0.3/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0      150 2023-06-28 13:48:32.645571 lumacli-0.0.3/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0     1057 2023-06-28 13:48:32.645571 lumacli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 lumacli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-24 10:07:59.207682 lumacli-0.0.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     3166 2023-07-24 10:07:59.207682 lumacli-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2023-07-24 10:07:59.207682 lumacli-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3390 2023-07-24 10:07:59.207682 lumacli-0.0.4/README.md
+-rw-r--r--   0        0        0      502 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     6528 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/dbt.py
+-rw-r--r--   0        0        0      483 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/luma.py
+-rw-r--r--   0        0        0     2401 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     3817 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0     8087 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/catalog.json
+-rw-r--r--   0        0        0        0 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/file.txt
+-rw-r--r--   0        0        0      260 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/invalid_json.json
+-rw-r--r--   0        0        0   173474 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/manifest.json
+-rw-r--r--   0        0        0     5109 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
+-rw-r--r--   0        0        0    10271 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/run_results.json
+-rw-r--r--   0        0        0     9716 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/sources.json
+-rw-r--r--   0        0        0       90 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0      691 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_dbt.py
+-rw-r--r--   0        0        0     3981 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_dbt_utils.py
+-rw-r--r--   0        0        0      305 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_postgres.py
+-rw-r--r--   0        0        0     3002 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_postgres_utils.py
+-rw-r--r--   0        0        0      394 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/tests/utils.py
+-rw-r--r--   0        0        0      320 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/dbt_utils.py
+-rw-r--r--   0        0        0     8456 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1371 2023-07-24 10:07:59.211682 lumacli-0.0.4/playground.py
+-rw-r--r--   0        0        0     1065 2023-07-24 10:07:59.211682 lumacli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 lumacli-0.0.4/PKG-INFO
```

### Comparing `lumacli-0.0.3/.github/workflows/publish_to_pypi.yml` & `lumacli-0.0.4/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/.gitignore` & `lumacli-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+lumaCLI/tests/temp/*
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `lumacli-0.0.3/LICENSE` & `lumacli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/lumaCLI/common.py` & `lumacli-0.0.4/lumaCLI/utils/dbt_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 import os
 from pathlib import Path
-from rich import print
 from rich.panel import Panel
+from rich import print
 
 
-def validate_json(json_path: str, endswith: str = ".json") -> bool:
+def validate_json(json_path: Path, endswith: str = ".json") -> bool:
     """
     Validates whether the provided file is a valid JSON file and ends with the specified string.
 
     Args:
         json_path (str): The full path to the file to be validated.
         endswith (str, optional): The string the file should end with. Defaults to ".json".
 
     Returns:
         bool: True if valid, False otherwise.
     """
-    file = Path(json_path)
 
     # Check that file exists
-    if not file.is_file():
-        error_message = f"[red]Error[/red]: [yellow]{file.absolute()}[/yellow] [blue]is not a file[/blue]"
+    if not json_path.is_file():
+        error_message = f"[red]Error[/red]: [yellow]{json_path.absolute()}[/yellow] [blue]is not a file[/blue]"
         print(Panel(error_message))
         return False
 
     # Check that filename ends with the required string
-    if not str(file).endswith(endswith):
-        error_message = f"[red]Error[/red]: [blue]File[/blue] [yellow]{os.path.basename(file.absolute())}[/yellow] [blue]does not have the required structure, it should end with [/blue][yellow]'{endswith}'[/yellow]"
+    if not str(json_path).endswith(endswith):
+        error_message = f"[red]Error[/red]: [blue]File[/blue] [yellow]{os.path.basename(json_path.absolute())}[/yellow] [blue]does not have the required structure, it should end with [/blue][yellow]'{endswith}'[/yellow]"
         print(Panel(error_message))
         return False
 
     return True
 
 
 def json_to_dict(json_path):
@@ -53,28 +52,20 @@
     Prints the HTTP response.
 
     Args:
         response (Response): The HTTP response to be printed.
     """
     if not response.ok:
         try:
-            print(
-                Panel(
-                    f"[red]An HTTP error occurred, response status code[/red]: {response.status_code} {json.loads(response.text)['detail']}"
-                )
-            )
+            error_message = f"[red]An HTTP error occurred, response status code[/red]: {response.status_code} {response.json()['detail']}"
         except:
-            print(
-                Panel(
-                    f"[red]An HTTP error occurred, response status code[/red]: {response.status_code} {response.text}"
-                )
-            )
+            error_message = f"[red]An HTTP error occurred, response status code[/red]: {response.status_code} {response.text}"
+        print(Panel(error_message))
     else:
-        print(
-            Panel(
-                "[green]The dbt ingestion to luma was successful!\nItems ingested:[/green]"
-            )
+        success_message = (
+            "[green]The dbt ingestion to luma was successful!\nItems ingested:[/green]"
         )
+        print(Panel(success_message))
         try:
             print(response.json())
         except:
-            print("Error at printing items ingested")
+            print(Panel("[red]Error at printing items ingested[/red]"))
```

### Comparing `lumacli-0.0.3/lumaCLI/dbt.py` & `lumacli-0.0.4/lumaCLI/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 import os
 from pathlib import Path
 import requests
 import typer
 from rich import print
 from rich.panel import Panel
-from lumaCLI.common import (
+from lumaCLI.utils import (
     validate_json,
     json_to_dict,
     print_response,
 )
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
+
+
+def get_current_working_directory(metadata_dir, ctx: typer.Context) -> Path:
+    if ctx.resilient_parsing:
+        return
+    if metadata_dir is not None:
+        return metadata_dir
+    cwd = Path(os.getcwd())
+    print(
+        Panel(
+            f"[yellow]'metadata_dir' not specified, using current working directory {cwd}[/yellow]"
+        )
+    )
+    return cwd
 
 
 @app.command()
 def ingest(
-    metadata_dir: str = typer.Argument(
+    metadata_dir: Path = typer.Argument(
         None,
         help="Path to the directory with dbt metadata files. If not provided, current working directory will be used.",
+        callback=get_current_working_directory,
+        exists=True,
+        dir_okay=True,
+        resolve_path=True,
     ),
     endpoint: str = typer.Option(
         ...,
         "--endpoint",
         "-e",
+        envvar="LUMA_DBT_INGEST_ENDPOINT",
         help="URL of the ingestion endpoint.",
     ),
 ):
     """
     Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
 
     Args:
         metadata_dir (str, optional): Directory path containing all the metadata files. Defaults to current working directory if not provided.
         endpoint (str): The endpoint URL for ingestion.
 
     Returns:
         response: The HTTP response obtained from the endpoint.
     """
-    if metadata_dir is None:
-        metadata_dir = os.getcwd()
-        print(
-            Panel(
-                f"[yellow]'metadata_dir' not specified, using current working directory {metadata_dir}[/yellow]"
-            )
-        )
+
     # Define JSON paths
-    manifest_json_path = os.path.join(metadata_dir, "manifest.json")
-    catalog_json_path = os.path.join(metadata_dir, "catalog.json")
-    sources_json_path = os.path.join(metadata_dir, "sources.json")
-    run_results_json_path = os.path.join(metadata_dir, "run_results.json")
+
+    manifest_json_path = metadata_dir / "manifest.json"
+    catalog_json_path = metadata_dir / "catalog.json"
+    sources_json_path = metadata_dir / "sources.json"
+    run_results_json_path = metadata_dir / "run_results.json"
 
     # Validate each JSON file
     is_manifest_json_valid = validate_json(
         json_path=manifest_json_path, endswith="manifest.json"
     )
     is_catalog_json_valid = validate_json(
         json_path=catalog_json_path, endswith="catalog.json"
@@ -107,22 +121,27 @@
 
     print_response(response)
     return response
 
 
 @app.command()
 def send_test_results(
-    metadata_dir: str = typer.Argument(
+    metadata_dir: Path = typer.Argument(
         None,
         help="Path to the directory with the run_results.json file. If not provided, current working directory will be used.",
+        callback=get_current_working_directory,
+        exists=True,
+        dir_okay=True,
+        resolve_path=True,
     ),
     endpoint: str = typer.Option(
         ...,
         "--endpoint",
         "-e",
+        envvar="LUMA_DBT_SEND-TEST-RESULTS_ENDPOINT",
         help="URL of the ingestion endpoint.",
     ),
 ):
     """
     Sends the run_results.json file located in the specified directory to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
 
     Args:
```

### Comparing `lumacli-0.0.3/lumaCLI/tests/catalog.json` & `lumacli-0.0.4/lumaCLI/tests/metadata_dir/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/lumaCLI/tests/manifest.json` & `lumacli-0.0.4/lumaCLI/tests/metadata_dir/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/lumaCLI/tests/run_results.json` & `lumacli-0.0.4/lumaCLI/tests/metadata_dir/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/lumaCLI/tests/sources.json` & `lumacli-0.0.4/lumaCLI/tests/metadata_dir/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.3/pyproject.toml` & `lumacli-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "lumaCLI"
 description = "A CLI tool for managing the data catalog platform."
 readme = "README.md"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name="Facundo Goiriz", email="fgoiriz@dyvenia.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["cli", "dbt", "luma", "data", "catalog"]
 requires-python = ">=3.10, <4"
 dependencies = [
     "typer[all]~=0.9.0",
+    "psycopg2-binary~=2.9",
     "requests~=2.28.2",
-    "rich~=13.3.5",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1,<8.0",
     "pytest-cov>=3.0,<4",
     "coverage>=6.4,<7",
```

