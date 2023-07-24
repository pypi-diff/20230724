# Comparing `tmp/promptquality-0.2.2.tar.gz` & `tmp/promptquality-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.2.2.tar", max compression
+gzip compressed data, was "promptquality-0.2.3.tar", max compression
```

## Comparing `promptquality-0.2.2.tar` & `promptquality-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10946 2023-07-21 21:05:56.084023 promptquality-0.2.2/LICENSE
--rw-r--r--   0        0        0      157 2023-07-21 21:05:56.084023 promptquality-0.2.2/README.md
--rw-r--r--   0        0        0     1543 2023-07-21 21:05:56.088023 promptquality-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      398 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/__init__.py
--rw-r--r--   0        0        0      353 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/config.py
--rw-r--r--   0        0        0       80 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/integrations.py
--rw-r--r--   0        0        0      172 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/job.py
--rw-r--r--   0        0        0      618 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/routes.py
--rw-r--r--   0        0        0      150 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/run.py
--rw-r--r--   0        0        0     1840 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/get_metrics.py
--rw-r--r--   0        0        0     4588 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/helpers.py
--rw-r--r--   0        0        0      543 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/integrations.py
--rw-r--r--   0        0        0     1060 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/job_progress.py
--rw-r--r--   0        0        0      466 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/login.py
--rw-r--r--   0        0        0     1603 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/run.py
--rw-r--r--   0        0        0     1019 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/set_config.py
--rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/__init__.py
--rw-r--r--   0        0        0     7781 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/config.py
--rw-r--r--   0        0        0     3619 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/run.py
--rw-r--r--   0        0        0      474 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/settings.py
--rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/__init__.py
--rw-r--r--   0        0        0     4460 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/api_client.py
--rw-r--r--   0        0        0      838 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/config.py
--rw-r--r--   0        0        0       60 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/logger.py
--rw-r--r--   0        0        0    24261 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/name.py
--rw-r--r--   0        0        0     1625 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/request.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-07-24 19:45:14.732241 promptquality-0.2.3/LICENSE
+-rw-r--r--   0        0        0      157 2023-07-24 19:45:14.732241 promptquality-0.2.3/README.md
+-rw-r--r--   0        0        0     1543 2023-07-24 19:45:14.732241 promptquality-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      398 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0       80 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/integrations.py
+-rw-r--r--   0        0        0      172 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/job.py
+-rw-r--r--   0        0        0      651 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      150 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0     1840 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0     5276 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/helpers.py
+-rw-r--r--   0        0        0      543 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/integrations.py
+-rw-r--r--   0        0        0     1060 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      466 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/login.py
+-rw-r--r--   0        0        0     1910 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/run.py
+-rw-r--r--   0        0        0     1019 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/set_config.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7781 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/config.py
+-rw-r--r--   0        0        0     3619 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/run.py
+-rw-r--r--   0        0        0      632 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/settings.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     4576 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0      838 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/config.py
+-rw-r--r--   0        0        0       60 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24559 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.3/PKG-INFO
```

### Comparing `promptquality-0.2.2/LICENSE` & `promptquality-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/pyproject.toml` & `promptquality-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptquality"
-version = "0.2.2"
+version = "0.2.3"
 description = "🦸 Supercharge your prompts with Galileo's Prompt Inspector!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 requests = "^2.31.0"
```

### Comparing `promptquality-0.2.2/src/promptquality/constants/routes.py` & `promptquality-0.2.3/src/promptquality/constants/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # into strings. https://github.com/python/mypy/issues/15269
 Routes = SimpleNamespace(
     healthcheck="healthcheck",
     login="login",
     get_token="get-token",
     current_user="current_user",
     projects="projects",
+    all_projects="projects/all",
     templates="projects/{project_id}/templates",
     dataset="projects/{project_id}/upload_prompt_dataset",
     runs="projects/{project_id}/runs",
     jobs="jobs",
     metrics="projects/{project_id}/runs/{run_id}/metrics",
     integrations="integrations/{integration_name}",
 )
```

### Comparing `promptquality-0.2.2/src/promptquality/get_metrics.py` & `promptquality-0.2.3/src/promptquality/get_metrics.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/helpers.py` & `promptquality-0.2.3/src/promptquality/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional
+from typing import Dict, List, Optional
 
 from pydantic import UUID4
 
 from promptquality.set_config import set_config
 from promptquality.types.config import Config
 from promptquality.types.run import (
     CreateJobRequest,
@@ -20,46 +20,63 @@
 )
 from promptquality.types.settings import Settings
 from promptquality.utils.logger import logger
 
 
 def create_project(
     project_name: Optional[str] = None, config: Optional[Config] = None
-) -> UUID4:
+) -> CreateProjectResponse:
     config = config or set_config()
     project_request = CreateProjectRequest(name=project_name)
-    logger.debug(f"Creating project {project_request.name}...")
-    response_dict = config.api_client.create_project(project_request)
-    project_response = CreateProjectResponse.model_validate(response_dict)
+    existing_projects: Dict[str, CreateProjectResponse] = {
+        proj.name: proj for proj in get_all_projects(config)
+    }
+    if project_request.name in existing_projects:
+        logger.info(f"Project {project_request.name} already exists, using it.")
+        project_response = existing_projects[project_request.name]
+    else:
+        logger.debug(f"Creating project {project_request.name}...")
+        response_dict = config.api_client.create_project(project_request)
+        project_response = CreateProjectResponse.model_validate(response_dict)
+        logger.debug(
+            f"Created project with name {project_response.name}, ID "
+            f"{project_response.id}."
+        )
     config.merge_project(project_response)
-    logger.debug(
-        f"Created project with name {project_response.name}, ID {project_response.id}."
-    )
-    return project_response.id
+    return project_response
+
+
+def get_all_projects(config: Optional[Config] = None) -> List[CreateProjectResponse]:
+    config = config or set_config()
+    logger.debug("Getting all projects...")
+    return [
+        CreateProjectResponse.model_validate(proj)
+        for proj in config.api_client.get_projects()
+    ]
 
 
 def create_template(
     template: str,
     project_id: UUID4,
     template_name: Optional[str] = None,
     config: Optional[Config] = None,
-) -> UUID4:
+) -> CreateTemplateResponse:
     config = config or set_config()
     template_request = CreateTemplateRequest(
         template=template, project_id=project_id, name=template_name
     )
     logger.debug(f"Creating template {template_request.name}...")
     response_dict = config.api_client.create_template(template_request)
     template_response = CreateTemplateResponse.model_validate(response_dict)
     config.merge_template(template_response)
     logger.debug(
         f"Created template with name {template_response.name}, ID "
         f"{template_response.id}."
     )
-    return template_response.selected_version_id
+    return template_response
 
 
 def upload_dataset(
     dataset: Path,
     project_id: UUID4,
     template_version_id: UUID4,
     config: Optional[Config] = None,
```

### Comparing `promptquality-0.2.2/src/promptquality/integrations.py` & `promptquality-0.2.3/src/promptquality/integrations.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/job_progress.py` & `promptquality-0.2.3/src/promptquality/job_progress.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/run.py` & `promptquality-0.2.3/src/promptquality/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,56 +9,61 @@
     create_template,
     upload_dataset,
 )
 from promptquality.job_progress import job_progress
 from promptquality.set_config import set_config
 from promptquality.types.run import PromptMetrics
 from promptquality.types.settings import Settings
+from promptquality.utils.name import ts_run_name
 
 
 def run(
     template: str,
     dataset: Path,
     project_name: Optional[str] = None,
     run_name: Optional[str] = None,
     template_name: Optional[str] = None,
     settings: Optional[Settings] = None,
     wait: bool = True,
 ) -> Optional[PromptMetrics]:
     config = set_config()
     # Create project.
-    project_id = create_project(project_name, config)
+    project = create_project(project_name, config)
     # Create template.
-    template_version_id = create_template(
+    template_response = create_template(
         template,
-        project_id,
-        template_name,
-        config,
+        project.id,
+        # Use project name as template name if not provided.
+        template_name=template_name or project.name,
+        config=config,
     )
     # Upload dataset.
     dataset_id = upload_dataset(
         dataset,
-        project_id,
-        template_version_id,
+        project.id,
+        template_response.selected_version_id,
         config,
     )
     # Run prompt.
     run_id = create_run(
-        project_id,
-        run_name,
-        config,
+        project.id,
+        run_name=run_name
+        or ts_run_name(
+            template_response.name, template_response.selected_version.version
+        ),
+        config=config,
     )
     job_id = create_job(
-        project_id,
+        project.id,
         run_id,
         dataset_id,
-        template_version_id,
+        template_response.selected_version_id,
         settings,
         config,
     )
     if wait:
         job_progress(job_id, config)
     print(f"🔭 View your prompt run on the Galileo console at: {config.run_url}")
     metrics = get_metrics(
-        project_id=project_id, run_id=run_id, job_id=job_id, config=config
+        project_id=project.id, run_id=run_id, job_id=job_id, config=config
     )
     return metrics
```

### Comparing `promptquality-0.2.2/src/promptquality/set_config.py` & `promptquality-0.2.3/src/promptquality/set_config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/types/config.py` & `promptquality-0.2.3/src/promptquality/types/config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/types/run.py` & `promptquality-0.2.3/src/promptquality/types/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/utils/api_client.py` & `promptquality-0.2.3/src/promptquality/utils/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,17 @@
             headers=headers,
             timeout=timeout,
         )
 
     def get_current_user(self) -> Dict[str, str]:
         return self._make_request(get, endpoint=Routes.current_user)
 
+    def get_projects(self) -> Dict[str, str]:
+        return self._make_request(get, endpoint=Routes.all_projects)
+
     def create_project(self, project_request: CreateProjectRequest) -> Dict[str, str]:
         return self._make_request(
             post,
             endpoint=Routes.projects,
             body=project_request.model_dump(),
         )
```

### Comparing `promptquality-0.2.2/src/promptquality/utils/config.py` & `promptquality-0.2.3/src/promptquality/utils/config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/src/promptquality/utils/name.py` & `promptquality-0.2.3/src/promptquality/utils/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from random import choice
 from re import findall
 from typing import Optional
 
 BAD_CHARS_REGEX = r"[^\w -]+"
 
 
@@ -1600,7 +1601,15 @@
 
     return name
 
 
 def random_name() -> str:
     sub_names = [choice(ADJECTIVES), choice(COLORS), choice(ANIMALS)]
     return "_".join(sub_names).lower()
+
+
+def ts_run_name(prompt_template_name: str, prompt_template_version: int) -> str:
+    "Jul_19_3_07_12_demo_template_v4"
+    ts = datetime.now()
+    ts_string = ts.strftime("%b_%d_%H_%M_%S")
+
+    return f"{ts_string}_{prompt_template_name}_v{prompt_template_version}"
```

### Comparing `promptquality-0.2.2/src/promptquality/utils/request.py` & `promptquality-0.2.3/src/promptquality/utils/request.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.2/PKG-INFO` & `promptquality-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptquality
-Version: 0.2.2
+Version: 0.2.3
 Summary: 🦸 Supercharge your prompts with Galileo's Prompt Inspector!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

