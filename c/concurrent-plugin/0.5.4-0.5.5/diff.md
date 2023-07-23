# Comparing `tmp/concurrent_plugin-0.5.4-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 37554 bytes, number of entries: 19
--rw-rw-r--  2.0 unx        2 b- defN 23-Jun-26 18:26 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    42966 b- defN 23-Jun-26 18:26 concurrent_plugin/concurrent_backend.py
--rw-rw-r--  2.0 unx    16820 b- defN 23-Jun-26 18:26 concurrent_plugin/concurrent_core.py
--rw-rw-r--  2.0 unx    13899 b- defN 23-Jul-07 22:48 concurrent_plugin/concurrent_deployment.py
--rw-rw-r--  2.0 unx    15759 b- defN 23-Jun-26 18:26 concurrent_plugin/login.py
--rw-rw-r--  2.0 unx     3994 b- defN 23-Jun-26 18:26 concurrent_plugin/periodic_run.py
--rw-rw-r--  2.0 unx     2091 b- defN 23-Jun-26 18:26 concurrent_plugin/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/__init__.py
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/infin_download.py
--rw-rw-r--  2.0 unx     1339 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/infin_prefetch.py
--rw-rw-r--  2.0 unx    10783 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/infinfs.py
--rw-rw-r--  2.0 unx     5326 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/infinmount.py
--rw-rw-r--  2.0 unx     1140 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    15974 b- defN 23-Jun-26 18:26 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      205 b- defN 23-Jul-08 05:42 concurrent_plugin-0.5.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-08 05:42 concurrent_plugin-0.5.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx      268 b- defN 23-Jul-08 05:42 concurrent_plugin-0.5.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Jul-08 05:42 concurrent_plugin-0.5.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1750 b- defN 23-Jul-08 05:42 concurrent_plugin-0.5.4.dist-info/RECORD
-19 files, 133416 bytes uncompressed, 34632 bytes compressed:  74.0%
+Zip file size: 37647 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx        2 b- defN 23-Jul-23 17:03 concurrent_plugin/__init__.py
+-rw-rw-r--  2.0 unx    42966 b- defN 23-Jul-23 17:21 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    16820 b- defN 23-Jul-23 17:21 concurrent_plugin/concurrent_core.py
+-rw-rw-r--  2.0 unx    14403 b- defN 23-Jul-23 23:32 concurrent_plugin/concurrent_deployment.py
+-rw-rw-r--  2.0 unx    15759 b- defN 23-Jul-23 17:21 concurrent_plugin/login.py
+-rw-rw-r--  2.0 unx     3994 b- defN 23-Jul-23 17:21 concurrent_plugin/periodic_run.py
+-rw-rw-r--  2.0 unx     2091 b- defN 23-Jul-23 17:21 concurrent_plugin/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-23 17:03 concurrent_plugin/infinfs/__init__.py
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infin_download.py
+-rw-rw-r--  2.0 unx     1339 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infin_prefetch.py
+-rw-rw-r--  2.0 unx    10783 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infinfs.py
+-rw-rw-r--  2.0 unx     5326 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infinmount.py
+-rw-rw-r--  2.0 unx     1140 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/mount_main.py
+-rw-rw-r--  2.0 unx    15974 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      205 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      268 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1750 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/RECORD
+19 files, 133920 bytes uncompressed, 34725 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.5.4.dist-info/METADATA
+Filename: concurrent_plugin-0.5.5.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.5.4.dist-info/WHEEL
+Filename: concurrent_plugin-0.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.5.4.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.5.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.4.dist-info/top_level.txt
+Filename: concurrent_plugin-0.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.4.dist-info/RECORD
+Filename: concurrent_plugin-0.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_deployment.py

```diff
@@ -205,19 +205,23 @@
 
     def explain(self, deployment_name=None, df=None, endpoint=None):
         print(f"PluginConcurrentDeploymentClient.explain: deployment_name={deployment_name}, df={df}, endpoint={endpoint}")
         return "1"
 
     def create_endpoint(self, name, config=None):
         print(f"PluginConcurrentDeploymentClient.create_endpoint: name={name}, config={config}")
+        if not name.startswith('mlflow-deploy-deployment-'):
+            raise RuntimeError(f"Error: incorrect endpont. should be of format mlflow-deploy-deployment-<run-id>")
+        run_id = name[len('mlflow-deploy-deployment-'):]
         if config and config.get("raiseError") == "True":
             raise RuntimeError("Error requested")
         cognito_client_id, _, _, _, region = get_conf()
         token = get_token(cognito_client_id, region, True)
 
+        body = {'name': name}
         headers = {
                 'Content-Type': 'application/x-amz-json-1.1',
                 'Authorization' : 'Bearer ' + token
                 }
         url = get_env_var().rstrip('/') + '/api/2.0/mlflow/parallels/create-endpoint'
         print(f"PluginConcurrentDeploymentClient.create_endpoint: posting {body} to {url}")
         try:
@@ -229,14 +233,17 @@
         except Exception as err:
             _logger.info(f'Other error occurred: {err}')
             raise
         return {"name": f"concurrent-endpoint-{run_id}", "flavor": "transformers"}
 
     def update_endpoint(self, endpoint, config=None):
         print(f"PluginConcurrentDeploymentClient.update_endpoint: endpoint={endpoint}, config={config}")
+        if not endpoint.startswith('mlflow-deploy-deployment-'):
+            raise RuntimeError(f"Error: incorrect endpont. should be of format mlflow-deploy-deployment-<run-id>")
+        run_id = endpoint[len('mlflow-deploy-deployment-'):]
         if config and config.get("raiseError") == "True":
             raise RuntimeError("Error requested")
         cognito_client_id, _, _, _, region = get_conf()
         token = get_token(cognito_client_id, region, True)
 
         body = {'name': endpoint}
         headers = {
```

## Comparing `concurrent_plugin-0.5.4.dist-info/RECORD` & `concurrent_plugin-0.5.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
 concurrent_plugin/concurrent_backend.py,sha256=dASijwn_zQVckPJyqguBhqXyhZnReAUqUWXKKSGrqxo,42966
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
-concurrent_plugin/concurrent_deployment.py,sha256=ACk1G3dGIDakjQNomQ14Ph8eMMM7KlTunjejPLU4Tc8,13899
+concurrent_plugin/concurrent_deployment.py,sha256=57d9oLvzzDs1GWYNEfmfcyCGWEga-WLjW7oHiL4lA-8,14403
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/utils.py,sha256=NpAWse8mKJkP_cyxLuCFizfVe2JjuyWkQWRGbBRjf9w,2091
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
 concurrent_plugin/infinfs/mount_service.py,sha256=G6jpVhFClkiwAoUyp4R35wTrhOzg23MA5-XZkyAWHX0,15974
-concurrent_plugin-0.5.4.dist-info/METADATA,sha256=G5VfqQSumXBE_aKLob2WX2ag1Jw6cV9R7wSbE_LoOV4,205
-concurrent_plugin-0.5.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.5.4.dist-info/entry_points.txt,sha256=OOh9nvgYMGXymz5yNb-XEL0dM2cMrSIhh5HQNOOBFNY,268
-concurrent_plugin-0.5.4.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.5.4.dist-info/RECORD,,
+concurrent_plugin-0.5.5.dist-info/METADATA,sha256=zUnZ5E25g3bp33j6QrMPmH-FM_JFRBu0jNf8XQybHDw,205
+concurrent_plugin-0.5.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.5.5.dist-info/entry_points.txt,sha256=OOh9nvgYMGXymz5yNb-XEL0dM2cMrSIhh5HQNOOBFNY,268
+concurrent_plugin-0.5.5.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.5.5.dist-info/RECORD,,
```

