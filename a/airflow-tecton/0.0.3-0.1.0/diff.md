# Comparing `tmp/airflow-tecton-0.0.3.tar.gz` & `tmp/airflow-tecton-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-tecton-0.0.3.tar", last modified: Thu Mar 16 21:13:33 2023, max compression
+gzip compressed data, was "airflow-tecton-0.1.0.tar", last modified: Mon Jul 24 18:11:40 2023, max compression
```

## Comparing `airflow-tecton-0.0.3.tar` & `airflow-tecton-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.946959 airflow-tecton-0.0.3/
--rw-r--r--   0 vitaly     (501) staff       (20)    11343 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/LICENSE
--rw-r--r--   0 vitaly     (501) staff       (20)     7553 2023-03-16 21:13:33.946812 airflow-tecton-0.0.3/PKG-INFO
--rw-r--r--   0 vitaly     (501) staff       (20)     7211 2023-03-16 20:53:09.000000 airflow-tecton-0.0.3/README.md
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.944353 airflow-tecton-0.0.3/airflow_tecton/
--rw-r--r--   0 vitaly     (501) staff       (20)     1310 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/__init__.py
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.945504 airflow-tecton-0.0.3/airflow_tecton/hooks/
--rw-r--r--   0 vitaly     (501) staff       (20)      572 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/hooks/__init__.py
--rw-r--r--   0 vitaly     (501) staff       (20)    10805 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/hooks/tecton_hook.py
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.946128 airflow-tecton-0.0.3/airflow_tecton/operators/
--rw-r--r--   0 vitaly     (501) staff       (20)      572 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/operators/__init__.py
--rw-r--r--   0 vitaly     (501) staff       (20)     6253 2023-03-16 20:53:09.000000 airflow-tecton-0.0.3/airflow_tecton/operators/tecton_job_operator.py
--rw-r--r--   0 vitaly     (501) staff       (20)     4383 2023-03-16 20:53:09.000000 airflow-tecton-0.0.3/airflow_tecton/operators/tecton_trigger_operator.py
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.946601 airflow-tecton-0.0.3/airflow_tecton/sensors/
--rw-r--r--   0 vitaly     (501) staff       (20)      572 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/sensors/__init__.py
--rw-r--r--   0 vitaly     (501) staff       (20)     4542 2023-03-16 18:42:46.000000 airflow-tecton-0.0.3/airflow_tecton/sensors/tecton_sensor.py
-drwxr-xr-x   0 vitaly     (501) staff       (20)        0 2023-03-16 21:13:33.945204 airflow-tecton-0.0.3/airflow_tecton.egg-info/
--rw-r--r--   0 vitaly     (501) staff       (20)     7553 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/PKG-INFO
--rw-r--r--   0 vitaly     (501) staff       (20)      564 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/SOURCES.txt
--rw-r--r--   0 vitaly     (501) staff       (20)        1 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/dependency_links.txt
--rw-r--r--   0 vitaly     (501) staff       (20)       84 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/entry_points.txt
--rw-r--r--   0 vitaly     (501) staff       (20)       29 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/requires.txt
--rw-r--r--   0 vitaly     (501) staff       (20)       15 2023-03-16 21:13:33.000000 airflow-tecton-0.0.3/airflow_tecton.egg-info/top_level.txt
--rw-r--r--   0 vitaly     (501) staff       (20)       38 2023-03-16 21:13:33.947000 airflow-tecton-0.0.3/setup.cfg
--rw-r--r--   0 vitaly     (501) staff       (20)     1516 2023-03-16 21:13:13.000000 airflow-tecton-0.0.3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.708921 airflow-tecton-0.1.0/
+-rw-r--r--   0 alex       (501) staff       (20)    11343 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     7663 2023-07-24 18:11:40.708809 airflow-tecton-0.1.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     7321 2023-07-24 18:11:06.000000 airflow-tecton-0.1.0/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.706615 airflow-tecton-0.1.0/airflow_tecton/
+-rw-r--r--   0 alex       (501) staff       (20)     1310 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.707538 airflow-tecton-0.1.0/airflow_tecton/hooks/
+-rw-r--r--   0 alex       (501) staff       (20)      572 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/hooks/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    12368 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/hooks/tecton_hook.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.708411 airflow-tecton-0.1.0/airflow_tecton/operators/
+-rw-r--r--   0 alex       (501) staff       (20)      572 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2504 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/df_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)     2351 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/job_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)     4336 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/tecton_feature_table_job_operator.py
+-rw-r--r--   0 alex       (501) staff       (20)     4109 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/tecton_feature_table_trigger_operator.py
+-rw-r--r--   0 alex       (501) staff       (20)     5106 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/tecton_job_operator.py
+-rw-r--r--   0 alex       (501) staff       (20)     4383 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/operators/tecton_trigger_operator.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.708658 airflow-tecton-0.1.0/airflow_tecton/sensors/
+-rw-r--r--   0 alex       (501) staff       (20)      572 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/sensors/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4542 2023-07-22 01:57:53.000000 airflow-tecton-0.1.0/airflow_tecton/sensors/tecton_sensor.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:11:40.707319 airflow-tecton-0.1.0/airflow_tecton.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     7663 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      767 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       84 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       56 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       15 2023-07-24 18:11:40.000000 airflow-tecton-0.1.0/airflow_tecton.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-24 18:11:40.708954 airflow-tecton-0.1.0/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1640 2023-07-24 18:11:34.000000 airflow-tecton-0.1.0/setup.py
```

### Comparing `airflow-tecton-0.0.3/LICENSE` & `airflow-tecton-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/PKG-INFO` & `airflow-tecton-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tecton
-Version: 0.0.3
+Version: 0.1.0
 Summary: Provider for using Tecton with Airflow.
 Home-page: http://tecton.ai/
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -29,19 +29,19 @@
 
 Contains an Apache Airflow provider that allows you to author Tecton workflows inside Airflow.
 
 Two basic capabilities are supported:
 1) Submitting materialization jobs
 2) Waiting for Feature View/Feature Service data to materialize.
 
-Note this package is in preview and it will not work with your Tecton installation unless enabled.
-
 ## Changelog
 
-- 0.0.3 Support `allow_overwrite` setting in the operators
+- 0.1.0 Added 2 new operators to support triggering Feature Table ingestion jobs 
+
+- 0.0.3 Added support for `allow_overwrite` setting in the operators
 
 - 0.0.2 Removed type annotations that caused compatibility issues with Airflow versions below 2.4.
 
 - 0.0.1 Initial release
 
 # Installation and Configuration
 
@@ -59,15 +59,15 @@
 
 You can add a new connection by going to `Connections` under the `Admin` tab in the Airflow UI. From there, hit the `+` button and select `Tecton` in the connection type dropdown. From there, you can configure the connection name, Tecton URL, and Tecton API key. Note that the default connection name is `tecton_default`, so we recommend starting with this as a connection name to minimize configuration.
 
 # Usage
 
 ## Configuring a Feature View for manual triggering
 
-A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View.
+A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering only. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View. As of Tecton 0.6, any FeatureView can be manually triggered, but this is recommended mostly for manual usage.
 
 For a `StreamFeatureView`, only batch materialization job scheduling will be impacted by the `batch_trigger` setting. Streaming materialization job scheduling will still be managed by Tecton.
 
 Here’s an example of a `BatchFeatureView` configured for manual triggering.
 
 ```python
 from tecton import batch_feature_view, FilteredSource, Aggregation, BatchTriggerType
@@ -127,26 +127,26 @@
 
 TectonJobOperator(
     task_id="tecton_job",
     workspace="my_workspace",
     feature_view="my_fv",
     online=False,
     offline=True,
-    retries=3
+    retries=3,
 )
 
 
 TectonTriggerOperator(
     task_id="trigger_tecton",
     workspace="my_workspace",
     feature_view="my_fv",
     online=True,
     offline=True,
 )
-```
+``` 
 
 ## Waiting For Materialization
 
 ### [TectonSensor](./airflow_tecton/sensors/tecton_sensor.py)
 
 This enables you to wait for Materialization to complete for both Feature Views and Feature Services. Common uses are for monitoring as well as kicking off a training job after daily materialization completes.
```

### Comparing `airflow-tecton-0.0.3/README.md` & `airflow-tecton-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 Contains an Apache Airflow provider that allows you to author Tecton workflows inside Airflow.
 
 Two basic capabilities are supported:
 1) Submitting materialization jobs
 2) Waiting for Feature View/Feature Service data to materialize.
 
-Note this package is in preview and it will not work with your Tecton installation unless enabled.
-
 ## Changelog
 
-- 0.0.3 Support `allow_overwrite` setting in the operators
+- 0.1.0 Added 2 new operators to support triggering Feature Table ingestion jobs 
+
+- 0.0.3 Added support for `allow_overwrite` setting in the operators
 
 - 0.0.2 Removed type annotations that caused compatibility issues with Airflow versions below 2.4.
 
 - 0.0.1 Initial release
 
 # Installation and Configuration
 
@@ -47,15 +47,15 @@
 
 You can add a new connection by going to `Connections` under the `Admin` tab in the Airflow UI. From there, hit the `+` button and select `Tecton` in the connection type dropdown. From there, you can configure the connection name, Tecton URL, and Tecton API key. Note that the default connection name is `tecton_default`, so we recommend starting with this as a connection name to minimize configuration.
 
 # Usage
 
 ## Configuring a Feature View for manual triggering
 
-A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View.
+A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering only. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View. As of Tecton 0.6, any FeatureView can be manually triggered, but this is recommended mostly for manual usage.
 
 For a `StreamFeatureView`, only batch materialization job scheduling will be impacted by the `batch_trigger` setting. Streaming materialization job scheduling will still be managed by Tecton.
 
 Here’s an example of a `BatchFeatureView` configured for manual triggering.
 
 ```python
 from tecton import batch_feature_view, FilteredSource, Aggregation, BatchTriggerType
@@ -115,26 +115,26 @@
 
 TectonJobOperator(
     task_id="tecton_job",
     workspace="my_workspace",
     feature_view="my_fv",
     online=False,
     offline=True,
-    retries=3
+    retries=3,
 )
 
 
 TectonTriggerOperator(
     task_id="trigger_tecton",
     workspace="my_workspace",
     feature_view="my_fv",
     online=True,
     offline=True,
 )
-```
+``` 
 
 ## Waiting For Materialization
 
 ### [TectonSensor](./airflow_tecton/sensors/tecton_sensor.py)
 
 This enables you to wait for Materialization to complete for both Feature Views and Feature Services. Common uses are for monitoring as well as kicking off a training job after daily materialization completes.
```

### Comparing `airflow-tecton-0.0.3/airflow_tecton/__init__.py` & `airflow-tecton-0.1.0/airflow_tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton/hooks/__init__.py` & `airflow-tecton-0.1.0/airflow_tecton/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton/hooks/tecton_hook.py` & `airflow-tecton-0.1.0/airflow_tecton/hooks/tecton_hook.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 JOBS_API_BASE = "/api/v1/jobs"
 SUBMIT_JOB_METHOD = "submit-materialization-job"
 GET_JOB_METHOD = "get-materialization-job"
 CANCEL_JOB_METHOD = "cancel-materialization-job"
 LIST_JOB_METHOD = "list-materialization-jobs"
 READINESS_METHOD = "get-latest-ready-time"
+INGEST_DATAFRAME = "ingest-dataframe"
+GET_DATAFRAME_INFO = "get-dataframe-info"
 
 
 class TectonHook(BaseHook):
     """
     Interact with Tecton's API. Currently supported are:
         get_materialization_job
         list_materialization_jobs
@@ -141,33 +143,34 @@
         self,
         workspace: str,
         feature_view: str,
         start_time: Union[datetime.datetime, str],
         end_time: Union[datetime.datetime, str],
         online: bool,
         offline: bool,
+        job_type: str ='batch',
     ):
         jobs = [
             x
             for x in self.list_materialization_jobs(
                 workspace=workspace, feature_view=feature_view
             ).get("jobs", [])
         ]
         for job in sorted(
             jobs, reverse=True, key=lambda x: self._parse_time(x["created_at"])
         ):
-            if job["job_type"].lower() != "batch":
-                continue
-            if (
-                job["online"] == online
-                and job["offline"] == offline
-                and job["start_time"] == self._canonicalize_datetime(start_time)
-                and job["end_time"] == self._canonicalize_datetime(end_time)
-            ):
-                return job
+            self.log.info('job = %s' % job)
+            if job_type.lower() == job.get("job_type", "").lower():
+                if (
+                    job["online"] == online
+                    and job["offline"] == offline
+                    and (job["start_time"] == self._canonicalize_datetime(start_time))
+                    and (job["end_time"] == self._canonicalize_datetime(end_time))
+                ):
+                    return job
         return None
 
     def submit_materialization_job(
         self,
         workspace: str,
         feature_view: str,
         start_time: Union[datetime.datetime, str],
@@ -286,14 +289,54 @@
         if offline_key not in result:
             result[offline_key] = None
         elif result[offline_key]:
             result[offline_key] = self._parse_time(result[offline_key])
 
         return result
 
+    def get_dataframe_info(
+        self, feature_view: str, workspace: str
+    ):
+        """
+        Get ingest data frame information
+
+        :param feature_view: feature view name
+        :param workspace:  workspace name
+        :return:
+        """
+        data = {"feature_view": feature_view, "workspace": workspace}
+        return self._make_request(
+            self.get_conn(), f"{JOBS_API_BASE}/{GET_DATAFRAME_INFO}", data, verbose=True
+        )
+
+    def ingest_dataframe(
+        self,
+        feature_view: str,
+        df_path: str,
+        workspace: str,
+        tecton_managed_retries: bool = False,
+    ):
+        """
+        Ingest data frame to FeatureTable from s3 path
+
+        :param feature_view: feature view name
+        :param df_path: s3 path containing pandas dataframe data
+        :param workspace:  workspace name
+        :param tecton_managed_retries: Whether the job should be retried by Tecton automatically.
+               Set to `False` if you want to control and submit retries manually.
+        :return:
+        """
+        data = {"feature_view": feature_view,
+                "df_path": df_path,
+                "workspace": workspace,
+                "use_tecton_managed_retries": tecton_managed_retries}
+        return self._make_request(
+            self.get_conn(), f"{JOBS_API_BASE}/{INGEST_DATAFRAME}", data, verbose=True
+        )
+
     @classmethod
     def create(cls, conn_id: str):
         return cls(conn_id)
 
     @classmethod
     def get_ui_field_behaviour(cls) -> Dict[str, Any]:
         """Returns custom field behaviour"""
```

### Comparing `airflow-tecton-0.0.3/airflow_tecton/operators/__init__.py` & `airflow-tecton-0.1.0/airflow_tecton/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton/operators/tecton_job_operator.py` & `airflow-tecton-0.1.0/airflow_tecton/operators/tecton_job_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 import logging
 import pprint
 import time
-from typing import Any
-from typing import Sequence
-from typing import Union
+from typing import Any, Sequence, Union
 
 from airflow.models import BaseOperator
 
 from airflow_tecton.hooks.tecton_hook import TectonHook
+from airflow_tecton.operators.job_utils import wait_until_completion, kill_job
 
 
 class TectonJobOperator(BaseOperator):
     """
     An Airflow operator that launches a Tecton job, and waits for its completion. If the latest job with the same params
     is running, it will cancel it first. If the latest job with the same params is successful, this will return without
     running a new job.
@@ -69,14 +68,15 @@
         self.end_time = end_time
         self.allow_overwrite = allow_overwrite
         self.conn_id = conn_id
         self.job_id = None
 
     def execute(self, context) -> Any:
         hook = TectonHook.create(self.conn_id)
+
         job = hook.find_materialization_job(
             workspace=self.workspace,
             feature_view=self.feature_view,
             online=self.online,
             offline=self.offline,
             start_time=self.start_time,
             end_time=self.end_time,
@@ -116,41 +116,14 @@
             online=self.online,
             offline=self.offline,
             start_time=self.start_time,
             end_time=self.end_time,
             allow_overwrite=self.allow_overwrite,
             tecton_managed_retries=False,
         )
+
         self.job_id = resp["job"]["id"]
-        job_result = hook.get_materialization_job(
-            self.workspace, self.feature_view, self.job_id
-        )["job"]
-        while job_result["state"].upper().endswith("RUNNING"):
-            if "attempts" in job_result:
-                attempts = job_result["attempts"]
-                latest_attempt = attempts[-1]
-                logging.info(
-                    f"Latest attempt #{len(attempts)} in state {latest_attempt['state']} with URL {latest_attempt['run_url']}"
-                )
-            else:
-                logging.info(f"No attempt launched yet")
-            time.sleep(60)
-            job_result = hook.get_materialization_job(
-                self.workspace, self.feature_view, self.job_id
-            )["job"]
-        if job_result["state"].upper().endswith("SUCCESS"):
-            return
-        else:
-            raise Exception(
-                f"Final job state was {job_result['state']}. Final response:\n {job_result}"
-            )
+
+        wait_until_completion(hook, self.workspace, self.feature_view, self.job_id)
 
     def on_kill(self) -> None:
-        if self.job_id:
-            logging.info(f"Attempting to kill job {self.job_id}")
-            hook = TectonHook.create(self.conn_id)
-            hook.cancel_materialization_job(
-                self.workspace, self.feature_view, self.job_id
-            )
-            logging.info(f"Successfully killed job {self.job_id}")
-        else:
-            logging.debug(f"No job started; none to kill")
+        kill_job(TectonHook.create(self.conn_id), self.workspace, self.feature_view, self.job_id)
```

### Comparing `airflow-tecton-0.0.3/airflow_tecton/operators/tecton_trigger_operator.py` & `airflow-tecton-0.1.0/airflow_tecton/operators/tecton_trigger_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton/sensors/__init__.py` & `airflow-tecton-0.1.0/airflow_tecton/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton/sensors/tecton_sensor.py` & `airflow-tecton-0.1.0/airflow_tecton/sensors/tecton_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-tecton-0.0.3/airflow_tecton.egg-info/PKG-INFO` & `airflow-tecton-0.1.0/airflow_tecton.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tecton
-Version: 0.0.3
+Version: 0.1.0
 Summary: Provider for using Tecton with Airflow.
 Home-page: http://tecton.ai/
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -29,19 +29,19 @@
 
 Contains an Apache Airflow provider that allows you to author Tecton workflows inside Airflow.
 
 Two basic capabilities are supported:
 1) Submitting materialization jobs
 2) Waiting for Feature View/Feature Service data to materialize.
 
-Note this package is in preview and it will not work with your Tecton installation unless enabled.
-
 ## Changelog
 
-- 0.0.3 Support `allow_overwrite` setting in the operators
+- 0.1.0 Added 2 new operators to support triggering Feature Table ingestion jobs 
+
+- 0.0.3 Added support for `allow_overwrite` setting in the operators
 
 - 0.0.2 Removed type annotations that caused compatibility issues with Airflow versions below 2.4.
 
 - 0.0.1 Initial release
 
 # Installation and Configuration
 
@@ -59,15 +59,15 @@
 
 You can add a new connection by going to `Connections` under the `Admin` tab in the Airflow UI. From there, hit the `+` button and select `Tecton` in the connection type dropdown. From there, you can configure the connection name, Tecton URL, and Tecton API key. Note that the default connection name is `tecton_default`, so we recommend starting with this as a connection name to minimize configuration.
 
 # Usage
 
 ## Configuring a Feature View for manual triggering
 
-A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View.
+A `BatchFeatureView` and a `StreamFeatureView` can be configured for manual triggering only. To do so, set `batch_trigger=BatchTriggerType.MANUAL`. When set to manual, Tecton will not automatically create any batch materialization jobs for the Feature View. As of Tecton 0.6, any FeatureView can be manually triggered, but this is recommended mostly for manual usage.
 
 For a `StreamFeatureView`, only batch materialization job scheduling will be impacted by the `batch_trigger` setting. Streaming materialization job scheduling will still be managed by Tecton.
 
 Here’s an example of a `BatchFeatureView` configured for manual triggering.
 
 ```python
 from tecton import batch_feature_view, FilteredSource, Aggregation, BatchTriggerType
@@ -127,26 +127,26 @@
 
 TectonJobOperator(
     task_id="tecton_job",
     workspace="my_workspace",
     feature_view="my_fv",
     online=False,
     offline=True,
-    retries=3
+    retries=3,
 )
 
 
 TectonTriggerOperator(
     task_id="trigger_tecton",
     workspace="my_workspace",
     feature_view="my_fv",
     online=True,
     offline=True,
 )
-```
+``` 
 
 ## Waiting For Materialization
 
 ### [TectonSensor](./airflow_tecton/sensors/tecton_sensor.py)
 
 This enables you to wait for Materialization to complete for both Feature Views and Feature Services. Common uses are for monitoring as well as kicking off a training job after daily materialization completes.
```

### Comparing `airflow-tecton-0.0.3/airflow_tecton.egg-info/SOURCES.txt` & `airflow-tecton-0.1.0/airflow_tecton.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,11 +7,15 @@
 airflow_tecton.egg-info/dependency_links.txt
 airflow_tecton.egg-info/entry_points.txt
 airflow_tecton.egg-info/requires.txt
 airflow_tecton.egg-info/top_level.txt
 airflow_tecton/hooks/__init__.py
 airflow_tecton/hooks/tecton_hook.py
 airflow_tecton/operators/__init__.py
+airflow_tecton/operators/df_utils.py
+airflow_tecton/operators/job_utils.py
+airflow_tecton/operators/tecton_feature_table_job_operator.py
+airflow_tecton/operators/tecton_feature_table_trigger_operator.py
 airflow_tecton/operators/tecton_job_operator.py
 airflow_tecton/operators/tecton_trigger_operator.py
 airflow_tecton/sensors/__init__.py
 airflow_tecton/sensors/tecton_sensor.py
```

### Comparing `airflow-tecton-0.0.3/setup.py` & `airflow-tecton-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-tecton",
-    version="0.0.3",
+    version="0.1.0",
     description="Provider for using Tecton with Airflow.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=airflow_tecton.__init__:get_provider_info"
         ]
@@ -31,15 +31,19 @@
     license="Apache License 2.0",
     packages=[
         "airflow_tecton",
         "airflow_tecton.hooks",
         "airflow_tecton.sensors",
         "airflow_tecton.operators",
     ],
-    install_requires=["apache-airflow>=2.0", "requests"],
+    install_requires=["apache-airflow>=2.0",
+                      "requests",
+                      "pandas",
+                      "pyarrow",
+                      "fastparquet"],
     setup_requires=["setuptools", "wheel"],
     test_require=["requests_mock"],
     url="http://tecton.ai/",
     classifiers=[
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
     ],
```

