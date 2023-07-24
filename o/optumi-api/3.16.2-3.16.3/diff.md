# Comparing `tmp/optumi-api-3.16.2.tar.gz` & `tmp/optumi-api-3.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.16.2.tar", last modified: Sat Jul 15 22:49:31 2023, max compression
+gzip compressed data, was "optumi-api-3.16.3.tar", last modified: Mon Jul 24 13:20:42 2023, max compression
```

## Comparing `optumi-api-3.16.2.tar` & `optumi-api-3.16.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.550059 optumi-api-3.16.2/
--rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-07-15 16:47:20.000000 optumi-api-3.16.2/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-07-15 16:47:20.000000 optumi-api-3.16.2/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-15 22:49:31.550059 optumi-api-3.16.2/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-07-15 16:47:20.000000 optumi-api-3.16.2/README.md
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-07-15 22:49:31.000000 optumi-api-3.16.2/core_version.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.546059 optumi-api-3.16.2/optumi_api/
--rw-rw-r--   0 denis     (1001) denis     (1001)     2839 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3663 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5135 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4044 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Colab.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5371 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Container.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4353 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6589 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Executable.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      976 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/HoldoverTime.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LocalFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2398 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LocalStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1505 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Log.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LoginServer.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     8473 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/Machine.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Machines.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Notebook.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     7280 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/NotebookConfig.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Notifications.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Packages.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1609 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Program.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Provider.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1299 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Providers.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6656 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/Resource.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Script.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Server.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1958 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Summary.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    20567 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Workload.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3110 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Workloads.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    11393 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/api.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/cli.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3806 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.550059 optumi-api-3.16.2/optumi_api.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/entry_points.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       74 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-07-15 22:49:31.550059 optumi-api-3.16.2/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     2644 2023-07-15 16:47:20.000000 optumi-api-3.16.2/setup.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-07-24 13:20:42.815741 optumi-api-3.16.3/
+-rw-rw-r--   0 jj        (1001) jj        (1001)      281 2023-03-28 17:12:40.000000 optumi-api-3.16.3/LICENSE
+-rw-rw-r--   0 jj        (1001) jj        (1001)       58 2023-05-10 18:59:32.000000 optumi-api-3.16.3/MANIFEST.in
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-07-24 13:20:42.815741 optumi-api-3.16.3/PKG-INFO
+-rw-rw-r--   0 jj        (1001) jj        (1001)      422 2023-03-28 17:12:40.000000 optumi-api-3.16.3/README.md
+-rw-rw-r--   0 jj        (1001) jj        (1001)      322 2023-07-24 13:20:42.000000 optumi-api-3.16.3/core_version.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-07-24 13:20:42.811741 optumi-api-3.16.3/optumi_api/
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2839 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/CloudFile.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3663 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5135 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/CloudStorage.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4044 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/Colab.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5578 2023-07-24 11:46:17.000000 optumi-api-3.16.3/optumi_api/Container.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4353 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4179 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6836 2023-07-24 11:46:17.000000 optumi-api-3.16.3/optumi_api/Executable.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      976 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3070 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/LocalFile.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2398 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/LocalStorage.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1505 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/Log.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6281 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/LoginServer.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     8473 2023-07-20 16:50:30.000000 optumi-api-3.16.3/optumi_api/Machine.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1957 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/Machines.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      723 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/Notebook.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     7417 2023-07-24 11:46:17.000000 optumi-api-3.16.3/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2487 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/Notifications.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      819 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/Packages.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1609 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/Program.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5284 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/Provider.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1299 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/Providers.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6927 2023-07-24 13:00:22.000000 optumi-api-3.16.3/optumi_api/Resource.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      696 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/Script.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4168 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/Server.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1958 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/Summary.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)    20567 2023-07-20 16:50:30.000000 optumi-api-3.16.3/optumi_api/Workload.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3110 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/Workloads.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      838 2023-03-28 17:12:40.000000 optumi-api-3.16.3/optumi_api/__init__.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      323 2023-07-21 20:17:24.000000 optumi-api-3.16.3/optumi_api/_version.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)    11393 2023-07-20 16:50:30.000000 optumi-api-3.16.3/optumi_api/api.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1418 2023-05-10 18:59:32.000000 optumi-api-3.16.3/optumi_api/cli.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3806 2023-07-06 16:46:44.000000 optumi-api-3.16.3/optumi_api/utils.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-07-24 13:20:42.815741 optumi-api-3.16.3/optumi_api.egg-info/
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1086 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       47 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jj        (1001) jj        (1001)       74 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       11 2023-07-24 13:20:42.000000 optumi-api-3.16.3/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       38 2023-07-24 13:20:42.815741 optumi-api-3.16.3/setup.cfg
+-rwxrwxr-x   0 jj        (1001) jj        (1001)     2644 2023-07-06 16:46:44.000000 optumi-api-3.16.3/setup.py
```

### Comparing `optumi-api-3.16.2/PKG-INFO` & `optumi-api-3.16.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.16.2
+Version: 3.16.3
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.16.2/optumi_api/CloudFile.py` & `optumi-api-3.16.3/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/CloudFileVersion.py` & `optumi-api-3.16.3/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/CloudStorage.py` & `optumi-api-3.16.3/optumi_api/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Colab.py` & `optumi-api-3.16.3/optumi_api/Colab.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Container.py` & `optumi-api-3.16.3/optumi_api/Container.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,32 +46,34 @@
         self,
         wait: bool = True,
         progress: str = "summary",
         env: Union[EnvironmentVariables, List[EnvironmentVariables]] = [],
         args: List[str] = [],
         resource: Union[Server, Resource] = None,
         notifications: Notifications = None,
+        max_runtime: int = -1
     ):
         """Launch a container given a specific configuration.
 
         Args:
             wait (bool, optional): Whether or not to wait for the workload to finish execution before returning. Defaults to True.
             progress (str, optional): How much progress data to return with the launched workload. Can be one of "silent", "summary", "detail". Defaults to "summary".
             env (EnvironmentVariables or list of EnvironmentVariables, optional): Environment variables to provision before running the container.
             args (list of str, optional): Command-line arguments to provide when running the container.
             resource (Server, Resource, optional): Resource requirements for the server that will be running the container. Defaults to None.
             notifications (Notifications, optional): User notification options when running the container. Defaults to None.
+            max_runtime (int): The maximum runtime of the workload (in minutes). We will automatically terminate the workload if it runs for this long.
 
         Returns:
             Workload: A workload representing the container.
         """
         if progress != None and not progress in Workload.progress:
             raise OptumiException("Unexpected progress '" + progress + "', expected one of " + str(Workload.progress))
 
-        nb_config = create_config(program_type="docker container", env=env, resource=resource, notifications=notifications, registry=self._registry)
+        nb_config = create_config(program_type="docker container", env=env, resource=resource, notifications=notifications, registry=self._registry, max_runtime=max_runtime)
 
         container_name = self._image
 
         setup = json.loads(
             optumi.core.setup_notebook(
                 container_name,
                 self.__utcnow(),
```

### Comparing `optumi-api-3.16.2/optumi_api/ContainerRegistry.py` & `optumi-api-3.16.3/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/EnvironmentVariables.py` & `optumi-api-3.16.3/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Executable.py` & `optumi-api-3.16.3/optumi_api/Executable.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,39 +53,41 @@
         progress: str = "summary",
         packages: Packages = Packages(),
         files: LocalStorage = LocalStorage(),
         env: Union[EnvironmentVariables, List[EnvironmentVariables]] = [],
         resource: Union[Server, Resource] = None,
         notifications: Notifications = None,
         launch_mode: str = "job",
+        max_runtime: int = -1
     ):
         """Launch an executable given a specific configuration.
 
         Args:
             wait (bool, optional): Whether or not to wait for the workload to finish execution before returning. Defaults to True.
             progress (str, optional): How much progress data to return with the launched workload. Can be one of "silent", "summary", "detail". Defaults to 'summary'.
             env (EnvironmentVariables or list of EnvironmentVariables, optional): Environment variables to configure before running the program.
             packages (Packages, optional):  Python packages required for executing the program. Defaults to empty.
             files (LocalStorage, optional): Any input files needed for the program's execution. Defaults to empty.
             resource (Server, Resource, optional): Server or Resource requirements for running the program. Defaults to None (meaning a GPU machine will be used).
             notifications (Notifications, optional): User notification options when running the container. Defaults to None.
             launch_mode (str, optional): The launch mode for running the program. Can be one of "session" or "job". Defaults to "job".
+            max_runtime (int): The maximum runtime of the workload (in minutes). We will automatically terminate the workload if it runs for this long. This only applies to jobs, not session.
 
         Raises:
             OptumiException: Raised if any of the requirements are specified incorrectly.
 
         Returns:
             Workload: A workload representing the program.
         """
 
         if progress != None and not progress in Workload.progress:
             raise OptumiException("Unexpected progress '" + progress + "', expected one of " + str(Workload.progress))
 
         nb_config = create_config(
-            program_type=self._program_type, packages=packages, files=files, env=env, resource=resource, notifications=notifications, launch_mode=launch_mode
+            program_type=self._program_type, packages=packages, files=files, env=env, resource=resource, notifications=notifications, launch_mode=launch_mode, max_runtime=max_runtime
         )
 
         with open(self._path, "r") as f:
             program = f.read()
 
         setup = json.loads(
             optumi.core.setup_notebook(
```

### Comparing `optumi-api-3.16.2/optumi_api/HoldoverTime.py` & `optumi-api-3.16.3/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/LocalFile.py` & `optumi-api-3.16.3/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/LocalStorage.py` & `optumi-api-3.16.3/optumi_api/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Log.py` & `optumi-api-3.16.3/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/LoginServer.py` & `optumi-api-3.16.3/optumi_api/LoginServer.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Machine.py` & `optumi-api-3.16.3/optumi_api/Machine.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Machines.py` & `optumi-api-3.16.3/optumi_api/Machines.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Notebook.py` & `optumi-api-3.16.3/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/NotebookConfig.py` & `optumi-api-3.16.3/optumi_api/NotebookConfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     packages: Packages = Packages(),
     files: LocalStorage = LocalStorage(),
     env: Union[EnvironmentVariables, List[EnvironmentVariables]] = [],
     resource: Resource = None,
     notifications: Notifications = None,
     registry: ContainerRegistry = None,
     launch_mode: str = "job",
+    max_runtime: int = -1,
 ):
     # Start with blank config
     nb_config = {
         "intent": 0.25,
         "compute": {
             "expertise": "component",
             "required": False,
@@ -72,14 +73,15 @@
             "throughput": [-1, -1, -1],
         },
         "upload": {"files": [], "requirements": ""},
         "integrations": [],
         "providers": [],
         "machineAssortment": [],
         "maxRate": -1,
+        "maxRuntime": -1,
         "notifications": {
             "jobStartedSMSEnabled": False,
             "jobCompletedSMSEnabled": False,
             "jobFailedSMSEnabled": False,
             "packageReadySMSEnabled": False,
         },
         "interactive": False,
@@ -188,14 +190,17 @@
         nb_config["memory"]["size"] = [-1, -1, -1] if resource.ram == 0 else [resource.ram * 1024**3, -1, -1]
 
         check_providers(resource.providers)
         nb_config["providers"] = [provider.name for provider in resource.providers]
 
         if resource.max_rate > 0:
             nb_config['maxRate'] = resource.max_rate / 3600 
+        
+    if max_runtime > 0:
+        nb_config['maxRuntime'] = max_runtime * 60
 
     # Plug in requirements
     if notifications != None:
         nb_config["notifications"] = {
             "jobStartedSMSEnabled": notifications.job_started,
             "jobCompletedSMSEnabled": notifications.job_completed,
             "jobFailedSMSEnabled": notifications.job_failed,
```

### Comparing `optumi-api-3.16.2/optumi_api/Notifications.py` & `optumi-api-3.16.3/optumi_api/Notifications.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Packages.py` & `optumi-api-3.16.3/optumi_api/Packages.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Program.py` & `optumi-api-3.16.3/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Provider.py` & `optumi-api-3.16.3/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Providers.py` & `optumi-api-3.16.3/optumi_api/Providers.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Resource.py` & `optumi-api-3.16.3/optumi_api/Resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,34 @@
 
 
 class Resource:
     """A class for creating resource specifications to be used when running scripts, notebooks or containers."""
 
     gpu_required_values = ["required", "optional"]
 
-    def __init__(self, providers: Union[List[str], List[Provider]] = [], gpu: str = "required", num_gpus: int = 0, vram_per_gpu: int = 0, vram_per_system: int = 0, ram: int = 0, num_cpus: int = 0, max_rate: float = -1):
+    def __init__(self, providers: Union[List[str], List[Provider], str, Provider] = [], gpu: str = "required", num_gpus: int = 0, vram_per_gpu: int = 0, vram_per_system: int = 0, ram: int = 0, num_cpus: int = 0, max_rate: float = -1):
         """Constructor for the Resource class.
 
         Args:
             providers (list of str or list of Provider): The providers that can be used. Defaults to [], which means any provider can be used.
             gpu (str): This argument specifies the type of graphics card to use. It can be set to "required" to permit any graphics card, "optional" to permit cpu only machines, or a particular value from the options in gpus(). The default option is "required".
             num_gpus (int): The minimum number of gpu cards. Defaults to 1 if gpu is specified, otherwise 0.
             vram_per_gpu (int): The minimum amount of VRAM in GiB per gpu card. Defaults to 0.
             vram_per_system (int): The minimum amount of VRAM in GiB for the machine. Defaults to 0.
             ram (int): The minimum amount of RAM in GiB for the machine. Defaults to 0.
             num_cpus (int): The minimum number of CPUs (virtual cores) for the machine. Defaults to 0.
             max_rate (float): The maximum rate in $/hr.
         Raises:
             OptumiException: Raised if an unsupported GPU card is specified.
         """
+        
+        # If a user passes in a singleton for provider, put it in a list
+        if not isinstance(providers, list):
+            providers = [providers]
+
         if not type(gpu) is str:
             raise OptumiException("Unexpected GPU type '" + str(gpu) + "', expected one of " + str(Resource.gpu_required_values + Server.gpus()))
         elif not gpu.lower().split('/')[0] in Resource.gpu_required_values + [x.lower() for x in Server.gpus()]:
             gpus = Server.gpus()
             if len(gpus) == 0:
                 if len([p for p in Providers.list() if p.is_activated()]) == 0:
                     raise OptumiException("No activated providers. Contact Optumi for more information.")
@@ -164,8 +169,10 @@
             ret += "vram_per_gpu=" + str(self.vram_per_gpu) + "GiB, "
         if self.vram_per_system > 0:
             ret += "vram_per_system=" + str(self.vram_per_system) + "GiB, "
         if self.ram > 0:
             ret += "ram=" + str(self.ram) + "GiB, "
         if self.num_cpus > 0:
             ret += "num_cpus=" + str(self.num_cpus) + ", "
+        if self.max_rate > 0:
+            ret += "max_rate=$" + str(self.max_rate) + "/hr, "
         return ret[:-2]
```

### Comparing `optumi-api-3.16.2/optumi_api/Script.py` & `optumi-api-3.16.3/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Server.py` & `optumi-api-3.16.3/optumi_api/Server.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Summary.py` & `optumi-api-3.16.3/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Workload.py` & `optumi-api-3.16.3/optumi_api/Workload.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/Workloads.py` & `optumi-api-3.16.3/optumi_api/Workloads.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/__init__.py` & `optumi-api-3.16.3/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/api.py` & `optumi-api-3.16.3/optumi_api/api.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/cli.py` & `optumi-api-3.16.3/optumi_api/cli.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api/utils.py` & `optumi-api-3.16.3/optumi_api/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.16.3/optumi_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.16.2
+Version: 3.16.3
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.16.2/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.16.3/optumi_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.2/setup.py` & `optumi-api-3.16.3/setup.py`

 * *Files identical despite different names*

