# Comparing `tmp/garden_ai-0.5.3.tar.gz` & `tmp/garden_ai-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.5.3.tar", max compression
+gzip compressed data, was "garden_ai-0.5.4.tar", max compression
```

## Comparing `garden_ai-0.5.3.tar` & `garden_ai-0.5.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-07-14 16:00:50.387446 garden_ai-0.5.3/LICENSE
--rw-r--r--   0        0        0      797 2023-07-14 16:00:50.387446 garden_ai-0.5.3/README.md
--rw-r--r--   0        0        0      418 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/__main__.py
--rw-r--r--   0        0        0     4454 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/_model.py
--rw-r--r--   0        0        0      180 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/console.py
--rw-r--r--   0        0        0    11506 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/main.py
--rw-r--r--   0        0        0     3895 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/model.py
--rw-r--r--   0        0        0    11770 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0     4002 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/backend_client.py
--rw-r--r--   0        0        0    18710 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/client.py
--rw-r--r--   0        0        0      440 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/constants.py
--rw-r--r--   0        0        0     9394 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/datacite.py
--rw-r--r--   0        0        0    14824 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2802 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1603 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      798 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7553 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/local_data.py
--rw-r--r--   0        0        0     8176 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/mlmodel.py
--rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/model_file_transfer/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/model_file_transfer/upload.py
--rw-r--r--   0        0        0    19626 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10745 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/steps.py
--rw-r--r--   0        0        0     2019 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     5258 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0     1018 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0     8533 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2903 2023-07-14 16:01:03.123311 garden_ai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 garden_ai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-24 14:46:38.901248 garden_ai-0.5.4/LICENSE
+-rw-r--r--   0        0        0      797 2023-07-24 14:46:38.901248 garden_ai-0.5.4/README.md
+-rw-r--r--   0        0        0      418 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/__main__.py
+-rw-r--r--   0        0        0     4454 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/_model.py
+-rw-r--r--   0        0        0      180 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/main.py
+-rw-r--r--   0        0        0     5227 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/model.py
+-rw-r--r--   0        0        0    16109 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     4002 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    27068 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/client.py
+-rw-r--r--   0        0        0      440 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/datacite.py
+-rw-r--r--   0        0        0     1068 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/garden_file_adapter.py
+-rw-r--r--   0        0        0    14824 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0      798 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/local_data.py
+-rw-r--r--   0        0        0    10014 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    21228 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10745 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     5797 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0      627 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0     8533 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2903 2023-07-24 14:46:52.973315 garden_ai-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 garden_ai-0.5.4/PKG-INFO
```

### Comparing `garden_ai-0.5.3/LICENSE` & `garden_ai-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/README.md` & `garden_ai-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/_model.py` & `garden_ai-0.5.4/garden_ai/_model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/app/console.py` & `garden_ai-0.5.4/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/app/garden.py` & `garden_ai-0.5.4/garden_ai/app/garden.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/app/main.py` & `garden_ai-0.5.4/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/app/model.py` & `garden_ai-0.5.4/garden_ai/app/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from pathlib import Path
-from typing import Optional, List
+from typing import List
 
 from garden_ai import local_data
 from garden_ai.client import GardenClient
 from garden_ai.mlmodel import (
     DatasetConnection,
     LocalModel,
     ModelFlavor,
+    ModelNotFoundException,
 )
+
 from garden_ai.app.console import console, get_local_model_rich_table
 
 import typer
 import rich
+from rich.prompt import Prompt
 import logging
 
 model_app = typer.Typer(name="model", no_args_is_help=True)
 
 logger = logging.getLogger()
 
 
@@ -46,60 +49,98 @@
     flavor: str = typer.Argument(
         "sklearn",
         help=(
             "What ML library did you make the model with? "
             "Currently we support the following flavors 'sklearn', 'tensorflow', and 'pytorch'."
         ),
     ),
-    dataset_url: Optional[str] = typer.Option(
-        None,
-        "--dataset-url",
-        help=(
-            "If you trained this model on a Foundry dataset, include a link to the dataset with this option"
-        ),
-    ),
-    dataset_doi: Optional[str] = typer.Option(
-        None,
-        "--dataset-doi",
-        help=(
-            "If you trained this model on a Foundry dataset, include the doi of the dataset"
-        ),
-    ),
 ):
     """Register a model in Garden. Outputs a full model identifier that you can reference in a Pipeline."""
     if flavor not in [f.value for f in ModelFlavor]:
         raise typer.BadParameter(
             f"Sorry, we only support 'sklearn', 'tensorflow', and 'pytorch'. The {flavor} flavor is not yet supported."
         )
 
-    only_one_dataset_option_provided = (dataset_url and not dataset_doi) or (
-        dataset_doi and not dataset_url
-    )
-    if only_one_dataset_option_provided:
-        raise typer.BadParameter(
-            "If you are linking a Foundry dataset, please include both --dataset-url and --dataset-doi"
-        )
-
     client = GardenClient()
     local_model = LocalModel(
         local_path=str(model_path),
         model_name=name,
         flavor=flavor,
         user_email=client.get_email(),
     )
-    if dataset_doi and dataset_url:
-        dataset_metadata = DatasetConnection(doi=dataset_doi, url=dataset_url)
-        local_model.connections.append(dataset_metadata)
 
     registered_model = client.register_model(local_model)
     rich.print(
         f"Successfully uploaded your model! The full name to include in your pipeline is '{registered_model.full_name}'"
     )
 
 
+@model_app.command(no_args_is_help=True)
+def add_dataset(
+    model_name: str = typer.Option(
+        ...,
+        "-m",
+        "--model",
+        help="The name of the model you would like to link your dataset to",
+        rich_help_panel="Required",
+    ),
+    title: str = typer.Option(
+        ...,
+        "-t",
+        "--title",
+        prompt="Please enter a short and descriptive title of your dataset",
+        rich_help_panel="Required",
+    ),
+    url: str = typer.Option(
+        ...,
+        "-u",
+        "--url",
+        prompt="If you trained this model on a dataset, include a link to the dataset. e.g., Kaggle, Foundry, Zenodo...",
+        rich_help_panel="Required",
+    ),
+    doi: str = typer.Option(
+        None,
+        "-d",
+        "--doi",
+        help="If dataset has a doi it can be referenced by, include the doi.",
+        rich_help_panel="Recommended",
+    ),
+    data_type: str = typer.Option(
+        None,
+        "-da",
+        "--datatype",
+        help="Please enter the file type of data in this dataset. e.g.: .csv,.json,.hdf5,...",
+        rich_help_panel="Recommended",
+    ),
+):
+    model = local_data.get_local_model_by_name(model_name)
+    if not model:
+        raise ModelNotFoundException("This model cannot be found.")
+    if not doi:
+        doi = Prompt.ask("Add the doi of the dataset? (leave blank to skip)")
+    if not data_type:
+        data_type = Prompt.ask("Add the filetype of the dataset (leave blank to skip)")
+    only_one_dataset_option_provided = (url and not doi) or (doi and not url)
+    if only_one_dataset_option_provided:
+        logger.warning(
+            "If you are linking a Foundry dataset, please include both --url and --doi"
+        )
+    if not url and not doi and not data_type:
+        raise typer.BadParameter(
+            "The parameters of your dataset are empty. Please input more information"
+            "about the dataset you would like to link with your model."
+        )
+    local_dataset = DatasetConnection(
+        title=title, doi=doi, data_type=data_type, url=url
+    )
+    model.dataset = local_dataset
+    local_data.put_local_model(model)
+    rich.print(f"Successfully added dataset to model {model_name}")
+
+
 @model_app.command(no_args_is_help=False)
 def list():
     """Lists all local models."""
 
     resource_table_cols = ["full_name", "model_name", "flavor"]
     table_name = "Local Models"
```

### Comparing `garden_ai-0.5.3/garden_ai/backend_client.py` & `garden_ai-0.5.4/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/client.py` & `garden_ai-0.5.4/garden_ai/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,45 +6,50 @@
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import UUID
 
 import typer
 from globus_compute_sdk import Client
 from globus_compute_sdk.serialize.concretes import DillCode
+from globus_compute_sdk.sdk.login_manager.tokenstore import get_token_storage_adapter
+from garden_ai.garden_file_adapter import GardenFileAdapter
 from globus_sdk import (
     AuthAPIError,
     AuthClient,
     ClientCredentialsAuthorizer,
     ConfidentialAppAuthClient,
     GroupsClient,
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
 )
-from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
+from globus_sdk.scopes import ScopeBuilder
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
 from rich import print
 from rich.prompt import Prompt
 
 from garden_ai import GardenConstants, local_data
 from garden_ai.backend_client import BackendClient
 from garden_ai.gardens import Garden
 from garden_ai.globus_compute.containers import build_container
-from garden_ai.globus_compute.login_manager import ComputeLoginManager
 from garden_ai.globus_compute.remote_functions import register_pipeline
 from garden_ai.globus_search import garden_search
 from garden_ai.local_data import GardenNotFoundException, PipelineNotFoundException
 from garden_ai.mlmodel import (
     LocalModel,
     ModelMetadata,
+    DatasetConnection,
+    ModelNotFoundException,
+    Model,
     clear_mlflow_staging_directory,
     stage_model_for_upload,
 )
 from garden_ai.model_file_transfer.upload import upload_mlmodel_to_s3
-from garden_ai.pipelines import Pipeline, RegisteredPipeline
+from garden_ai.pipelines import Pipeline, RegisteredPipeline, Paper, Repository
+from garden_ai.steps import step
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
 
@@ -81,17 +86,22 @@
     def __init__(
         self,
         auth_client: Union[AuthClient, ConfidentialAppAuthClient] = None,
         search_client: SearchClient = None,
     ):
         key_store_path = Path(GardenConstants.GARDEN_DIR)
         key_store_path.mkdir(exist_ok=True)
-        self.auth_key_store = SimpleJSONFileAdapter(
+        self.garden_key_store = SimpleJSONFileAdapter(
             os.path.join(key_store_path, "tokens.json")
         )
+        self.compute_key_store = get_token_storage_adapter()
+        self.auth_key_store = GardenFileAdapter(
+            self.garden_key_store, self.compute_key_store
+        )
+
         self.client_id = os.environ.get(
             "GARDEN_CLIENT_ID", "cf9f8938-fb72-439c-a70b-85addf1b8539"
         )
 
         # If auth_client is type AuthClient or None, do an
         # Authorization Code Grant and make RefreshTokenAuthorizers.
         # If auth_client is type ConfidentialAppAuthClient, do a
@@ -149,22 +159,15 @@
         self.backend_client = BackendClient(self.garden_authorizer)
 
     def _get_garden_access_token(self):
         self.garden_authorizer.ensure_valid_token()
         return self.garden_authorizer.access_token
 
     def _make_compute_client(self):
-        scope_to_authorizer = {
-            AuthScopes.openid: self.openid_authorizer,
-            SearchScopes.all: self.search_authorizer,
-            Client.FUNCX_SCOPE: self.compute_authorizer,
-        }
-        compute_login_manager = ComputeLoginManager(scope_to_authorizer)
         return Client(
-            login_manager=compute_login_manager,
             do_version_check=False,
             code_serialization_strategy=DillCode(),
         )
 
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
@@ -311,14 +314,53 @@
                 logger.error("Original exception: " + str(e))
                 # We can still proceed, there is just some cruft in the user's home directory.
                 pass
         registered_model = ModelMetadata(**local_model.dict())
         local_data.put_local_model(registered_model)
         return registered_model
 
+    def add_dataset(self, model_name: str, title: str, url: str, **kwargs) -> None:
+        """Adds a ``DatasetConnection`` to ``ModelMetadata`` corresponding to the given full model name.
+
+        Parameters
+        ----------
+        model_name : str
+            The previously registered model's full model name. Raises an
+            exception if not found.
+
+        title : str
+            An official name or title for the dataset.
+
+        url: str
+            The url to access this dataset.
+
+        **kwargs :
+            Metadata for the new DatasetConnection object. Keyword arguments matching
+            required or recommended fields will be (where necessary) coerced to the appropriate type.
+            May include: Optional[str] doi, Optional[str] data_type.
+
+        Raises
+        ------
+        ModelNotFoundException
+            Raised when no known model exists with the given identifier.
+        """
+        model = local_data.get_local_model_by_name(model_name)
+        data = dict(kwargs)
+        if not model:
+            raise ModelNotFoundException("This model could not be found")
+        if model_name:
+            data["model_name"] = model_name
+        if title:
+            data["title"] = title
+        if url:
+            data["url"] = url
+        dataset = DatasetConnection(**data)
+        model.dataset = dataset
+        local_data.put_local_model(model)
+
     def _mint_draft_doi(self, test: bool = True) -> str:
         """Register a new draft doi with DataCite via Garden backend.
 
         Expects environment variable GARDEN_ENDPOINT to be set (not including `/doi`).
 
         Parameters
         ----------
@@ -358,14 +400,192 @@
         func_uuid = register_pipeline(self.compute_client, pipeline, container_uuid)
         pipeline.func_uuid = UUID(func_uuid)
         self._update_datacite(pipeline)
         registered = RegisteredPipeline.from_pipeline(pipeline)
         local_data.put_local_pipeline(registered)
         return func_uuid
 
+    def add_paper(self, title: str, doi: str, **kwargs) -> None:
+        """Adds a ``Paper`` to a ``RegisteredPipeline`` corresponding to the given doi.
+
+        Parameters
+        ----------
+        doi : str
+            The previously registered pipeline's DOI. Raises an
+            exception if not found.
+
+        title : str
+            An official name or title for the paper.
+
+        **kwargs :
+            Metadata for the new Paper object. Keyword arguments matching
+            required or recommended fields will be (where necessary) coerced to the appropriate type.
+            May include: List[str] authors and Optional[str] citation.
+
+        Raises
+        ------
+        PipelineNotFoundException
+            Raised when no known pipeline exists with the given identifier.
+        """
+        pipeline = local_data.get_local_pipeline_by_doi(doi)
+        if not pipeline:
+            raise PipelineNotFoundException(
+                f"Could not find any pipelines with DOI {doi}."
+            )
+        data = dict(kwargs)
+        if title:
+            data["title"] = title
+        paper = Paper(**data)
+        pipeline.papers.append(paper)
+        local_data.put_local_pipeline(pipeline)
+
+    def add_repository(self, doi: str, url: str, repo_name: str, **kwargs) -> None:
+        """Adds a ``Repository`` to a ``RegisteredPipeline`` corresponding to the given doi.
+
+        Parameters
+        ----------
+        doi : str
+            The previously registered pipeline's DOI. Raises an
+            exception if not found.
+
+        title : str
+            An official name or title for the repository.
+
+        url: str
+            The url to access this repository.
+
+        **kwargs :
+            Metadata for the new Repository object. Keyword arguments matching
+            required or recommended fields will be (where necessary) coerced to the appropriate type.
+            May include: List[str] contributors.
+
+        Raises
+        ------
+        PipelineNotFoundException
+            Raised when no known pipeline exists with the given identifier.
+        """
+        data = dict(kwargs)
+        print(data)
+        if doi:
+            data["doi"] = doi
+        if url:
+            data["url"] = url
+        if repo_name:
+            data["repo_name"] = repo_name
+        pipeline = local_data.get_local_pipeline_by_doi(doi)
+        if not pipeline:
+            raise PipelineNotFoundException(
+                f"Could not find any pipelines with DOI {doi}."
+            )
+
+        repository = Repository(**data)
+        pipeline.repositories.append(repository)
+        local_data.put_local_pipeline(pipeline)
+
+    def add_simple_model_to_garden(
+        self,
+        local_model: LocalModel,
+        garden_doi: str,
+        *,
+        input_type: type,
+        output_type: type,
+        title: str = None,
+        description: str = None,
+        **kwargs,
+    ) -> str:
+        """Take a `LocalModel` object and automatically perform all the necessary steps,
+        using the additional provided information, to publish the model such that it is prepared to be run remotely.
+
+        Parameters
+        ----------
+        local_model : LocalModel
+            The model for which remote executiotability is desired. The object's necessary fields are documented at
+            `~mlmodel.LocalModel` and its parent `~mlmodel.ModelMetadata`.
+
+        garden_doi : str
+            The DOI of a previously published Garden that the model will be added to in order to facilitate findability
+            and remote execution.
+
+        input_type : type
+            The type that describes the expected input to your model.
+
+        output_type : type
+            The type that describes the expected output of your model.
+
+        title : str
+            Title that describes the pipeline that is implicitly generated. If no title is provided, one will be generated.
+
+        description : str
+            Description of the pipeline that is implicitly generated. If no description is provided, one will be generated.
+
+        **kwargs :
+            Metadata for the new Pipeline object that runs the model. Keyword arguments matching
+            required or recommended fields will be (where necessary) coerced to the
+            appropriate type and validated per the documentation found at `~pipelines.Pipeline`.
+            NOTE: Some fields are necessary for proper publication. e.g. `pip_dependecies` if your model needs them.
+
+        Returns
+        -------
+        The DOI of your auto-generated pipeline. Use this DOI to access your pipeline at a later date.
+
+        Examples
+        --------
+        client = GardenClient()
+        local_model = LocalModel(
+            model_name="dendrite_segmentation",
+            flavor="tensorflow",
+            local_path="model.h5",
+            user_email=client.get_email()
+        )
+        my_pipeline = client.add_simple_model_to_garden(local_model, "10.1234/doi-here",
+                                                        input_type=np.ndarray,
+                                                        output_type=np.ndarray,
+                                                        authors=["Monty Python", "Guido van Rossum"],
+                                                        pip_dependencies=["tensorflow"],
+                                                        tags=["materials science", "computer vision"]
+        )
+        """
+        registered_model = self.register_model(local_model)
+
+        # we ignore these type errors, because we want the step to be typed correctly but mypy does not acknowledge that it would be
+        @step
+        def run_inference(
+            input_arg: input_type, model=Model(registered_model.full_name)  # type: ignore
+        ) -> output_type:  # type: ignore
+            return model.predict(input_arg)
+
+        pipeline = self.create_pipeline(
+            title=title or f"Inference on model: {local_model.model_name}",
+            short_name=local_model.model_name,
+            steps=(run_inference,),
+            description=description
+            or "Auto-generated pipeline that executes a single step which runs an inference.",
+            **kwargs,
+        )
+        container_uuid = self.build_container(pipeline)
+        self.register_pipeline(pipeline, container_uuid)
+
+        garden = self.get_published_garden(garden_doi)
+
+        # add pipeline to garden
+        if pipeline not in garden.pipelines:
+            garden.pipeline_ids += [pipeline.doi]
+
+        self.publish_garden_metadata(garden)
+        # bandaid in the event the index is written more than once simultaneously
+        # note: still not perfect, communication is key
+        if (
+            pipeline.doi
+            not in (remote := self.get_published_garden(garden.doi)).pipeline_ids
+        ):
+            remote.pipeline_ids += [pipeline.doi]
+            self.publish_garden_metadata(remote)
+
+        return pipeline.doi
+
     def get_registered_pipeline(self, doi: str) -> RegisteredPipeline:
         """Return a callable ``RegisteredPipeline`` corresponding to the given doi.
 
         Parameters
         ----------
         doi : str
             The previously registered pipeline's DOI. Raises an
```

### Comparing `garden_ai-0.5.3/garden_ai/datacite.py` & `garden_ai-0.5.4/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/gardens.py` & `garden_ai-0.5.4/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/globus_compute/containers.py` & `garden_ai-0.5.4/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.5.4/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/globus_search/garden_search.py` & `garden_ai-0.5.4/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/local_data.py` & `garden_ai-0.5.4/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/mlmodel.py` & `garden_ai-0.5.4/garden_ai/mlmodel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 import os
 import pathlib
 import pickle
 import shutil
 from enum import Enum
-from typing import List
+from typing import Optional
+import functools
 
 import mlflow  # type: ignore
 from pydantic import BaseModel, Field, validator
 
 from garden_ai import GardenConstants
 from garden_ai._model import _Model
 
+
 MODEL_STAGING_DIR = pathlib.Path(GardenConstants.GARDEN_DIR) / "mlflow"
 MODEL_STAGING_DIR.mkdir(parents=True, exist_ok=True)
 
 
 class ModelUploadException(Exception):
     """Exception raised when an attempt to upload a model to ML Flow fails"""
 
     pass
 
 
+class ModelNotFoundException(Exception):
+    """Exception raised when an attempt to access a model that does not exist"""
+
+    pass
+
+
 class PipelineLoadScaffoldedException(Exception):
     """Exception raised when a user attempts to load model with the name SCAFFOLDED_MODEL_NAME"""
 
     pass
 
 
 class ModelFlavor(Enum):
     SKLEARN = "sklearn"
     PYTORCH = "pytorch"
     TENSORFLOW = "tensorflow"
 
 
 class DatasetConnection(BaseModel):
     """
-    A first step towards the Accelerate Connection Schema
+    The ``DataSetConnection`` class represents all the metadata we want to \
+    publically expose about the datasets that can be utilized with this model.
+
+    Attributes:
+        title (str):
+            A short and descriptive name of the dataset.
+        doi (str):
+            A digital identifier to the dataset.
+        url (str):
+            Location where the dataset can be accessed. If using foundry \
+            dataset, both url and doi must be provided.
+        data_type (str):
+            Optional, the type of file of dataset.
+
     """
 
-    type: str = "dataset"
-    relationship: str = "origin"
-    doi: str = Field(...)
-    repository: str = "Foundry"
+    title: str = Field(...)
+    doi: Optional[str] = Field(None)
     url: str = Field(...)
+    data_type: Optional[str] = Field(None)
 
 
 class ModelMetadata(BaseModel):
     """
     The ``ModelMetadata`` class represents all the metadata we want to \
     publicly expose about an ML model that has been registered with Garden.
 
     Attributes:
         model_name (str): A short and descriptive name of the model
         flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
-        connections (List[DatasetConnection]):
-            A list of dataset records that the model was trained on.
+        dataset (DatasetConnection):
+            A dataset record that the model was trained on.
         user_email (str): The email address of the user uploading the model.
         full_name (str): The user_email and model_name together like "foo@example.edu/my_model"
         mlflow_name (str): The user_email and model_name together like "foo@example.edu-my_model"
 
     """
 
     model_name: str = Field(...)
     user_email: str = Field(...)
     flavor: str = Field(...)
-    connections: List[DatasetConnection] = Field(default_factory=list)
+    dataset: Optional[DatasetConnection] = Field(None)
     full_name: str = ""
     mlflow_name: str = ""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # The / separator is canonical because it is nice for S3
         # and conveys that your email is a namespace.
@@ -180,15 +200,29 @@
         item_path = os.path.join(path, item)
         if os.path.isfile(item_path):
             os.remove(item_path)
         elif os.path.isdir(item_path):
             shutil.rmtree(item_path)
 
 
+def trackcalls(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        wrapper.has_been_called = True
+        return func(*args, **kwargs)
+
+    wrapper.has_been_called = False
+    return wrapper
+
+
+@trackcalls
 def Model(full_model_name: str) -> _Model:
+    from garden_ai.utils.filesystem import PipelineLoadException
+    from .local_data import get_local_model_by_name
+
     """Load a registered model from Garden-AI's (MLflow) tracking server.
 
     Tip:
         This is meant to be used as a "default argument" in a `@step`-decorated \
         function. This allows the step to collect model-specific dependencies, \
         including any user-specified dependencies when the model was registered.
 
@@ -213,14 +247,29 @@
         The object returned by this function waits as long as possible - i.e. \
         until the model actually needs to make a prediction - to actually \
         download and deserialize the registered model. This is done so that \
         ``Model('me@uni.edu-myModel/2)`` in a step (like above) an argument \
         default is lighter-weight when the function itself is serialized for \
         remote execution of a pipeline.
     """
+    if not full_model_name:
+        raise PipelineLoadException(
+            "The parameters of Model() are empty. Please enter your registered model name in your pipeline.py"
+        )
+    if not get_local_model_by_name(full_model_name):
+        raise ModelNotFoundException(f"No model with {full_model_name} exists.")
+    if full_model_name == GardenConstants.SCAFFOLDED_MODEL_NAME:
+        error_message = (
+            "Failed to load model. It looks like you are using the placeholder model name from a scaffolded pipeline. "
+            f"Please replace {GardenConstants.SCAFFOLDED_MODEL_NAME} in your pipeline.py"
+            " with the name of a registered Garden model."
+            "\nFor more information on how to use Garden, please read our docs: "
+            "https://garden-ai.readthedocs.io/en/latest/"
+        )
+        raise PipelineLoadScaffoldedException(error_message)
     try:
         from __main__ import _Model
     except ImportError:
         # re-import only seems necessary for pytest
         from garden_ai._model import _Model  # type: ignore
         from garden_ai.utils._meta import redef_in_main
```

### Comparing `garden_ai-0.5.3/garden_ai/model_file_transfer/upload.py` & `garden_ai-0.5.4/garden_ai/model_file_transfer/upload.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/pipelines.py` & `garden_ai-0.5.4/garden_ai/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,59 @@
     read_conda_deps,
     safe_compose,
 )
 
 logger = logging.getLogger()
 
 
+class Repository(BaseModel):
+    """
+    The `Repository` class represents all the metadata we want to \
+    publically expose about the repositories used to build the pipeline.
+
+    Attributes:
+        repo_name (str):
+            A title that the repository can be referenced by.
+        url (str):
+            A link where this repository can be publically viewed.
+        contributors List[str]:
+            Acknowledge contributors to the development of \
+            this repository.
+
+    """
+
+    repo_name: str = Field(...)
+    url: str = Field(...)
+    contributors: List[str] = Field(default_factory=list)
+
+
+class Paper(BaseModel):
+    """
+    The `Paper` class represents all the metadata we want to \
+    publically expose about the papers used to build the pipeline.
+
+    Attributes:
+        title (str):
+            The official title that the paper can be referenced by.
+        authors List[str]:
+            The main researchers involved in producing the paper. Personal name \
+            format should be: "Family, Given". Order is preserved. (at least one required)
+        doi (str):
+            The digital object identifier of the paper. (Optional)
+        citation (str):
+            Description of how the paper may be cited officially. (Optional)
+
+    """
+
+    title: str = Field(...)
+    authors: List[str] = Field(default_factory=list)
+    doi: Optional[str] = Field(None)
+    citation: Optional[str] = Field(None)
+
+
 @dataclass(config=DataclassConfig)
 class Pipeline:
     """The `Pipeline` class represents a sequence of simpler `steps` composed \
     together to perform a more complex task, typically running inference with a \
     pretrained AI/ML Model.
 
     See also: [RegisteredPipeline][garden_ai.pipelines.RegisteredPipeline]
@@ -365,14 +410,16 @@
         tags:
         python_version:
         doi:
         func_uuid:
         pip_dependencies:
         conda_dependencies:
         model_full_names:
+        repositories:
+        papers:
     """
 
     doi: str = Field(...)
     func_uuid: Optional[UUID] = Field(...)
     title: str = Field(...)
     short_name: str = Field(...)
     authors: List[str] = Field(...)
@@ -384,14 +431,16 @@
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     python_version: Optional[str] = Field(None)
     pip_dependencies: List[str] = Field(default_factory=list)
     conda_dependencies: List[str] = Field(default_factory=list)
     _env_vars: Dict[str, str] = PrivateAttr(default_factory=dict)
     model_full_names: List[str] = Field(default_factory=list)
+    repositories: List[Repository] = Field(default_factory=list)
+    papers: List[Paper] = Field(default_factory=list)
 
     def __call__(
         self,
         *args: Any,
         endpoint: Union[UUID, str] = None,
         **kwargs: Any,
     ) -> Any:
```

### Comparing `garden_ai-0.5.3/garden_ai/steps.py` & `garden_ai-0.5.4/garden_ai/steps.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/templates/pipeline` & `garden_ai-0.5.4/garden_ai/templates/pipeline`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/garden_ai/utils/_meta.py` & `garden_ai-0.5.4/garden_ai/utils/_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import inspect
 import linecache
 import textwrap
+import logging
+
+logger = logging.getLogger()
 
 
 def redef_in_main(obj):
     """Helper: redefine an object in __main__, e.g. garden_ai._Model -> __main__._Model.
 
     This has the effect of coaxing dill into serializing both the definition and
     the instance of an object together (in the case of a class), so it can be
@@ -100,23 +103,24 @@
             return getlines(filename, module_globals)
 
     linecache.getlines = monkey_patch
 
     try:
         exec(source, globals, locals)
         # you can now use inspect.getsource() on the result of exec() here
-
     finally:
         linecache.getlines = getlines
 
 
 def _load_pipeline_from_python_file(python_file):
     import __main__
 
     from garden_ai import Pipeline
+    from garden_ai.utils.filesystem import PipelineLoadException
+    from garden_ai.mlmodel import Model
 
     with open(python_file, "r") as file:
         pipeline_code = file.read()
 
     # dynamically create a class that we're using exclusively for the sake of a
     # simpler namespace than a ModuleType object.
     #
@@ -131,19 +135,26 @@
     code_str = f"""
 class _USER_PIPELINE_MODULE:
 {textwrap.indent(pipeline_code, '    ')}
 """
 
     # run the user's code as `__main__._USER_PIPELINE_MODULE` namespace
     local_namespace: dict = {}
+
     exec_getsource(code_str, __main__.__dict__, local_namespace)
-    cls = local_namespace["_USER_PIPELINE_MODULE"]
 
+    cls = local_namespace["_USER_PIPELINE_MODULE"]
     # Now, one of those class attributes is going to be a Pipeline instance
     for name, value in vars(cls).items():
         if isinstance(value, Pipeline):
-            # use whatever identifier the user assigned the pipeline to in their code
+            if not Model.has_been_called:
+                logger.warning(
+                    f"No model exists in file. If this pipeline includes a model, please input the model in {python_file} "
+                    "with the name of a registered Garden model."
+                    "\nFor more information on how to use Garden, please read our docs: "
+                    "https://garden-ai.readthedocs.io/en/latest/"
+                )
             value.short_name = value.short_name or name
             return value
-    raise ValueError(
-        f"Did not find top-level pipeline object defined in {python_file}."
+    raise PipelineLoadException(
+        "Pipeline couldn't be loaded from the user's module. Could not find pipeline object in file."
     )
```

### Comparing `garden_ai-0.5.3/garden_ai/utils/misc.py` & `garden_ai-0.5.4/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.3/pyproject.toml` & `garden_ai-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.5.3" # placeholder
+version = "0.5.4" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
```

### Comparing `garden_ai-0.5.3/PKG-INFO` & `garden_ai-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.5.3
+Version: 0.5.4
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
```

