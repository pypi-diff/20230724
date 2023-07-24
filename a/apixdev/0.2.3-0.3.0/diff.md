# Comparing `tmp/apixdev-0.2.3.tar.gz` & `tmp/apixdev-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.2.3.tar", last modified: Sun Jul 23 19:29:17 2023, max compression
+gzip compressed data, was "apixdev-0.3.0.tar", last modified: Mon Jul 24 19:06:13 2023, max compression
```

## Comparing `apixdev-0.2.3.tar` & `apixdev-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-23 19:29:17.061757 apixdev-0.2.3/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.2.3/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-23 19:29:17.061757 apixdev-0.2.3/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.2.3/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-23 19:29:17.057757 apixdev-0.2.3/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-23 19:29:17.057757 apixdev-0.2.3/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.2.3/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.2.3/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      569 2023-07-23 16:32:30.000000 apixdev-0.2.3/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2984 2023-07-23 19:06:10.000000 apixdev-0.2.3/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-23 19:29:17.061757 apixdev-0.2.3/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1478 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3351 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2170 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4399 2023-07-23 19:06:10.000000 apixdev-0.2.3/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/repository.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5092 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2492 2023-07-23 16:27:29.000000 apixdev-0.2.3/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2206 2023-07-23 19:27:37.000000 apixdev-0.2.3/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-23 19:29:17.057757 apixdev-0.2.3/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      668 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      146 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-23 19:29:17.000000 apixdev-0.2.3/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-23 19:29:17.061757 apixdev-0.2.3/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1596 2023-07-23 19:28:47.000000 apixdev-0.2.3/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.0/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:06:13.543579 apixdev-0.3.0/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.0/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.0/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.0/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1145 2023-07-24 19:04:11.000000 apixdev-0.3.0/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.0/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1478 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5016 2023-07-24 19:01:56.000000 apixdev-0.3.0/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-24 15:45:46.000000 apixdev-0.3.0/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2170 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.0/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/repository.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5092 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2861 2023-07-24 15:49:57.000000 apixdev-0.3.0/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1097 2023-07-24 15:44:34.000000 apixdev-0.3.0/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      146 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-24 19:06:13.543579 apixdev-0.3.0/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1596 2023-07-24 19:04:59.000000 apixdev-0.3.0/setup.py
```

### Comparing `apixdev-0.2.3/LICENSE` & `apixdev-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/PKG-INFO` & `apixdev-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.2.3
+Version: 0.3.0
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.2.3/README.md` & `apixdev-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/cli/config.py` & `apixdev-0.3.0/apixdev/cli/config.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/cli/projects.py` & `apixdev-0.3.0/apixdev/cli/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/cli/tools.py` & `apixdev-0.3.0/apixdev/cli/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/common.py` & `apixdev-0.3.0/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/compose.py` & `apixdev-0.3.0/apixdev/core/compose.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/images.py` & `apixdev-0.3.0/apixdev/core/images.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/odoo.py` & `apixdev-0.3.0/apixdev/core/odoo.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/project.py` & `apixdev-0.3.0/apixdev/core/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,121 @@
+import logging
 import os
 import subprocess
 from shutil import rmtree
 
 import requests
 from requests.exceptions import HTTPError
 
 from apixdev.core.compose import Compose
-from apixdev.core.settings import Settings
+from apixdev.core.docker import Stack
+from apixdev.core.exceptions import DownloadError
+from apixdev.core.settings import settings, vars
 from apixdev.core.tools import (
     filter_requirements,
     get_requirements_from_path,
     list_to_text,
     text_to_list,
 )
 
-settings = Settings()
+_logger = logging.getLogger(__name__)
 
 
 class Project:
     def __init__(self, name, path=None):
         self.root_path = settings.workdir
         self.path = path or os.path.join(self.root_path, name)
         self.name = name
+        self.uuid = None
 
         os.makedirs(self.path, exist_ok=True)
 
     def __repr__(self) -> str:
         return f"Project({self.name})"
 
     def __str__(self) -> str:
         return self.name
 
     @classmethod
     def from_path(cls, path):
+        """Load project from path"""
         name = os.path.basename(path)
         instance = cls(name, path)
 
         return instance
 
     @property
     def compose_file(self):
+        """Complete filepath to docker-compose.yaml"""
         return os.path.join(self.path, "docker-compose.yaml")
 
     @property
     def repositories_file(self):
+        """Complete filepath to repositories.yaml"""
         return os.path.join(self.path, "repositories.yaml")
 
     @property
     def manifest_file(self):
+        """Complete filepath to manifest.yaml"""
         return os.path.join(self.path, "manifest.yaml")
 
     @property
     def env_file(self):
+        """Complete filepath to .env file"""
         return os.path.join(self.path, ".env")
 
     @property
     def repositories_path(self):
+        """Complete path to repositories"""
         return os.path.join(self.path, "repositories")
 
     @property
     def is_ready(self):
+        """A project is considered ready if all 3 manifests are present"""
         files = [
             self.compose_file,
             self.repositories_file,
             self.manifest_file,
         ]
         return bool(all(map(os.path.exists, files)))
 
     def download(self, filename, url, force=False):
         filepath = os.path.join(self.path, filename)
         headers = {
             "X-Api-Token": settings.get_var("apix.token"),
         }
 
         if force and os.path.exists(filepath):
-            print("remove %s" % filepath)
+            _logger.info("Remove %s file", filepath)
             os.remove(filepath)
 
         try:
-            response = requests.get(url, headers=headers, allow_redirects=False)
+            response = requests.get(
+                url,
+                headers=headers,
+                allow_redirects=False,
+                timeout=vars.DEFAULT_TIMEOUT,
+            )
             response.raise_for_status()
         except HTTPError as error:
             code = error.response.status_code
-            raise Exception(
-                f"Error while trying to download {filename} from {url} (HTTP {code})."
-            )
+            raise DownloadError(filename, url, code) from error
 
         with open(filepath, "wb") as file:
             file.write(response.content)
 
         return True
 
     def pull_repositories(self):
+        """Recursively pull code repositories"""
         if not self.repositories_file:
             return False
 
         env_file = self.env_file if os.path.exists(self.env_file) else settings.env_file
 
-        # gitaggregate(f"-c {self.repositories_file}", _cwd=self.path)
-        # gitaggregate(
-        #     [
-        #         "-c",
-        #         "repositories.yaml",
-        #         "--expand-env",
-        #         "--env-file",
-        #         settings.env_file,
-        #     ],
-        #     _cwd=self.path,
-        #     _in=sys.stdin,
-        #     _out=sys.stdout,
-        # )
-
         args = [
             "gitaggregate",
             "-c",
             "repositories.yaml",
             "--expand-env",
             "--env-file",
             env_file,
@@ -134,25 +135,26 @@
         compose.update("services/odoo/environment/CUSTOM_REQUIREMENTS", text)
         compose.save(self.compose_file)
 
     def load_manifest(self):
         manifest = Compose.from_path(self.manifest_file)
         self.uuid = manifest.extract("uuid")
 
-        print(self.uuid)
-
         keys = [
             (self.compose_file, "docker_compose_url"),
             (self.repositories_file, "repositories_url"),
         ]
 
         for filename, key in keys:
             url = manifest.extract(key)
             self.download(filename, url, True)
 
+    def get_stack(self):
+        return Stack(self.name, self.path)
+
     # def __del__(self):
     #     rmtree(self.path, ignore_errors=True)
     #     self.root_path = None
     #     self.path = None
     #     self.name = None
 
     def delete(self):
```

### Comparing `apixdev-0.2.3/apixdev/core/projects.py` & `apixdev-0.3.0/apixdev/core/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/repository.py` & `apixdev-0.3.0/apixdev/core/repository.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/settings.py` & `apixdev-0.3.0/apixdev/core/settings.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.2.3/apixdev/core/tools.py` & `apixdev-0.3.0/apixdev/core/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,7 +89,21 @@
 def bytes_to_json(data):
     res = data.rstrip().decode("utf8").replace("'", '"').replace("\n", ",")
     res = "[" + res + "]"
     res = res.replace(",]", "]")
     json_data = json.loads(res)
 
     return json_data
+
+
+def convert_stdout_to_json(content):
+    try:
+        data = json.loads(content)
+    except json.decoder.JSONDecodeError:
+        content = content.decode("utf8")
+        content = content.strip().rstrip().lstrip()
+        content = f"[{content}]"
+        content = content.replace("}", "},").replace("},]", "}]")
+
+        data = json.loads(content)
+
+    return data
```

### Comparing `apixdev-0.2.3/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.0/apixdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.2.3
+Version: 0.3.0
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.2.3/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.0/apixdev.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 apixdev/cli/project.py
 apixdev/cli/projects.py
 apixdev/cli/tools.py
 apixdev/core/__init__.py
 apixdev/core/common.py
 apixdev/core/compose.py
 apixdev/core/docker.py
+apixdev/core/exceptions.py
 apixdev/core/images.py
 apixdev/core/odoo.py
 apixdev/core/project.py
 apixdev/core/projects.py
 apixdev/core/repository.py
 apixdev/core/settings.py
 apixdev/core/tools.py
```

### Comparing `apixdev-0.2.3/setup.py` & `apixdev-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.2.3",
+    version="0.3.0",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
```

