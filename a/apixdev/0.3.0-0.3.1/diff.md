# Comparing `tmp/apixdev-0.3.0.tar.gz` & `tmp/apixdev-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.3.0.tar", last modified: Mon Jul 24 19:06:13 2023, max compression
+gzip compressed data, was "apixdev-0.3.1.tar", last modified: Mon Jul 24 19:53:44 2023, max compression
```

## Comparing `apixdev-0.3.0.tar` & `apixdev-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.0/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:06:13.543579 apixdev-0.3.0/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.0/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.0/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.0/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1145 2023-07-24 19:04:11.000000 apixdev-0.3.0/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.0/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1478 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5016 2023-07-24 19:01:56.000000 apixdev-0.3.0/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-24 15:45:46.000000 apixdev-0.3.0/apixdev/core/exceptions.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2170 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.0/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/repository.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5092 2023-07-23 16:27:29.000000 apixdev-0.3.0/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2861 2023-07-24 15:49:57.000000 apixdev-0.3.0/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1097 2023-07-24 15:44:34.000000 apixdev-0.3.0/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:06:13.543579 apixdev-0.3.0/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      146 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-24 19:06:13.000000 apixdev-0.3.0/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-24 19:06:13.543579 apixdev-0.3.0/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1596 2023-07-24 19:04:59.000000 apixdev-0.3.0/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.1/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:53:44.609141 apixdev-0.3.1/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.1/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.605141 apixdev-0.3.1/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.1/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.1/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1265 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.1/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1457 2023-07-24 19:09:56.000000 apixdev-0.3.1/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5198 2023-07-24 19:48:50.000000 apixdev-0.3.1/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      908 2023-07-24 19:31:49.000000 apixdev-0.3.1/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2170 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.1/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/repository.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5815 2023-07-24 19:41:43.000000 apixdev-0.3.1/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3036 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1248 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.605141 apixdev-0.3.1/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-24 19:53:44.609141 apixdev-0.3.1/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-24 19:49:56.000000 apixdev-0.3.1/setup.py
```

### Comparing `apixdev-0.3.0/LICENSE` & `apixdev-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/PKG-INFO` & `apixdev-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.0
+Version: 0.3.1
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.0/README.md` & `apixdev-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/cli/config.py` & `apixdev-0.3.1/apixdev/cli/config.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/cli/main.py` & `apixdev-0.3.1/apixdev/cli/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,14 +18,20 @@
     stop,
     update,
     update_modules,
 )
 from apixdev.cli.projects import projects
 from apixdev.core.settings import settings
 
+# try:
+#     settings.check()
+# except ExternalDependenciesMissing as error:
+#     click.echo(error)
+#     sys.exit(1)
+
 if not settings.is_ready:
     click.echo("Please fill configuration to continue :")
     settings.set_config()
 
 
 @click.group()
 def cli():
```

### Comparing `apixdev-0.3.0/apixdev/cli/project.py` & `apixdev-0.3.1/apixdev/cli/project.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/cli/projects.py` & `apixdev-0.3.1/apixdev/cli/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/cli/tools.py` & `apixdev-0.3.1/apixdev/cli/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/common.py` & `apixdev-0.3.1/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/compose.py` & `apixdev-0.3.1/apixdev/core/compose.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,14 @@
     @classmethod
     def from_url(cls, url):
         response = requests.get(url)
         return cls(yaml.safe_load(response.content))
 
     def get_path(self, path):
         res = os.path.join(path, self._name)
-
-        print(res)
-
         return res
 
     def update_dict(self, vals):
         dict_merge(self._content, vals)
 
     def update(self, chain, value):
         keys = chain.split("/")
```

### Comparing `apixdev-0.3.0/apixdev/core/docker.py` & `apixdev-0.3.1/apixdev/core/docker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 import subprocess
 
 from apixdev.core.exceptions import NoContainerFound
 from apixdev.core.settings import vars
 from apixdev.core.tools import convert_stdout_to_json
 
-DOCKER_COMPOSE_RUN_BACKGROUND = "docker-compose up -d"
-DOCKER_COMPOSE_RUN = "docker-compose run --rm --service-ports odoo bash"
-DOCKER_COMPOSE_DOWN = "docker-compose down"
-DOCKER_LOGS = "docker logs -f {}"
-DOCKER_EXEC = "docker exec -it {} {}"
-
-ODOO_MODULES = "odoo -d {} --stop-after-init {} {}"
-ODOO_SHELL = "odoo shell -d {}"
-
 
 class Stack:
     def __init__(self, name, path):
         self.name = name
         self.path = path
         self.service_count = 3
 
     @property
     def is_running(self):
+        """Check if every containers running as excepted."""
         services = self._inspect_services()
 
         if vars.DOCKER_SERVICES_COUNT < len(services):
             return False
 
         states = map(lambda item: item.get("state", False), services)
 
         if not all(map(lambda item: bool(item in ["running"]), states)):
             return False
 
         return True
 
     def run(self, run_on_background=False):
+        """Run docker-compose stack."""
         if run_on_background:
-            cmd = DOCKER_COMPOSE_RUN_BACKGROUND
+            cmd = vars.DOCKER_COMPOSE_RUN_BACKGROUND
         else:
-            cmd = DOCKER_COMPOSE_RUN
+            cmd = vars.DOCKER_COMPOSE_RUN
 
         subprocess.call(cmd.split(" "), cwd=self.path)
 
     def stop(self, clear=False):
-        cmd = DOCKER_COMPOSE_DOWN.split(" ")
+        """Stop docker-compose stack."""
+        cmd = vars.DOCKER_COMPOSE_DOWN.split(" ")
 
         if clear:
             cmd.append("-v")
 
         subprocess.call(cmd, cwd=self.path)
 
     def clear(self):
+        """Stop and clear docker-compose stack."""
         self.stop(True)
 
-    # def ps(self):
-    #     print(self.is_running)
-    #     print(self._get_container_names())
-
     def _convert_container_info(self, vals_list):
         def apply(vals):
             name = vals.get("Name", vals.get("Names", ""))
             return {
                 "name": name,
                 "state": vals.get("State", ""),
             }
@@ -103,71 +94,82 @@
 
         if not container:
             return False
 
         return container[0]
 
     def get_containers(self):
+        """Return containers names"""
         return self._get_container_names()
 
     def get_container(self, service_name):
+        """Return container object"""
         container_name = self._get_container_name(service_name)
         if not container_name:
             raise NoContainerFound(service_name)
         return Container(self, service_name, container_name)
 
     def get_odoo_container(self):
+        """Return Odoo specialized container"""
         container_name = self._get_container_name("odoo")
         if not container_name:
             raise NoContainerFound("odoo")
         return OdooContainer(self, container_name)
 
 
 class Container:
     def __init__(self, stack, service, name):
         self.stack = stack
         self.service = service
         self.name = name
 
     @property
     def path(self):
+        """Path"""
         return self.stack.path
 
     @property
     def is_running(self):
+        """Checks if parent stack is running"""
         return self.stack.is_running
 
     def logs(self):
+        """Show container logs"""
         if not self.is_running:
             return False
 
-        cmd = DOCKER_LOGS.format(self.name).split(" ")
+        cmd = vars.DOCKER_LOGS.format(self.name).split(" ")
         subprocess.call(cmd, cwd=self.path)
 
     def bash(self):
+        """Attach to container bash"""
         if not self.is_running:
             return False
 
-        cmd = DOCKER_EXEC.format(self.name, "bash").split(" ")
+        cmd = vars.DOCKER_EXEC.format(self.name, "bash").split(" ")
         subprocess.call(cmd, cwd=self.path)
 
 
 class OdooContainer(Container):
     def __init__(self, stack, name):
         super().__init__(stack, "odoo", name)
 
     def install_modules(self, database, modules, **kwargs):
+        """Install modules list to Odoo database"""
         if not self.is_running:
             return False
 
         odoo_arg = "-u" if not kwargs.get("install", False) else "-i"
-        odoo_cmd = ODOO_MODULES.format(database, odoo_arg, modules)
-        cmd = DOCKER_EXEC.format(self.name, odoo_cmd).split()
+        odoo_cmd = vars.ODOO_MODULES.format(database, odoo_arg, modules)
+        cmd = vars.DOCKER_EXEC.format(self.name, odoo_cmd).split()
 
         subprocess.call(cmd, cwd=self.path)
 
     def shell(self, database):
+        """Attach to Odoo Shell"""
         if not self.is_running:
             return False
 
-        cmd = DOCKER_EXEC.format(self.name, ODOO_SHELL.format(database)).split(" ")
+        cmd = vars.DOCKER_EXEC.format(
+            self.name, vars.ODOO_SHELL.format(database)
+        ).split(" ")
         subprocess.call(cmd, cwd=self.path)
```

### Comparing `apixdev-0.3.0/apixdev/core/images.py` & `apixdev-0.3.1/apixdev/core/images.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/odoo.py` & `apixdev-0.3.1/apixdev/core/odoo.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/project.py` & `apixdev-0.3.1/apixdev/core/project.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/projects.py` & `apixdev-0.3.1/apixdev/core/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/repository.py` & `apixdev-0.3.1/apixdev/core/repository.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/apixdev/core/settings.py` & `apixdev-0.3.1/apixdev/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 import configparser
 import getpass
 import logging
 import os
+import subprocess
 
 import apixdev.vars as vars
+from apixdev.core.exceptions import ExternalDependenciesMissing
 
-path = os.path.join(vars.HOME_PATH, vars.CONFIG_PATH)
-filename = os.path.join(path, vars.LOGGING_FILE)
+config_dir = os.path.join(vars.HOME_PATH, vars.CONFIG_PATH)
+filename = os.path.join(config_dir, vars.LOGGING_FILE)
 
-if not os.path.isdir(path):
-    os.makedirs(path)
+if not os.path.isdir(config_dir):
+    os.makedirs(config_dir)
 
 logging.basicConfig(filename=filename, level=vars.LOGGING_LEVEL)
 
 _logger = logging.getLogger(__name__)
 
 from apixdev.core.common import SingletonMeta  # noqa: E402
 
 
+def check_system_dependencies(cmd):
+    try:
+        res = subprocess.check_output(cmd.split(" "))
+        res = res.decode("utf8").strip()
+    except FileNotFoundError:
+        return False
+
+    return res
+
+
 class Settings(metaclass=SingletonMeta):
     def __init__(self, path, name="config.ini"):
         self._path = path
         self._name = name
         self._config = None
 
+        self.docker_version = None
+        self.docker_compose_version = None
+
         self._load()
 
+    def check(self, raise_if_not_found=True):
+        for name, cmd in vars.EXTERNAL_DEPENDENCIES.items():
+            res = check_system_dependencies(cmd)
+            if not res and raise_if_not_found:
+                raise ExternalDependenciesMissing(name)
+            _logger.error("Check failed: %s not found.", name)
+
     @property
     def filepath(self):
         return os.path.join(self._path, self._name)
 
     def _load(self):
         self._config = configparser.ConfigParser()
         if not os.path.isdir(self._path):
@@ -176,8 +198,8 @@
         return self.get_var("local.workdir")
 
     @property
     def env_file(self):
         return os.path.join(self._path, ".env")
 
 
-settings = Settings(path)
+settings = Settings(config_dir)
```

### Comparing `apixdev-0.3.0/apixdev/core/tools.py` & `apixdev-0.3.1/apixdev/core/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import json
 import os
+import subprocess
 
 import requirements as req_tool
 from packaging.specifiers import SpecifierSet
 
 
+def check_system_dependencies(cmd):
+    try:
+        res = subprocess.check_output(cmd)
+    except FileNotFoundError:
+        return False
+
+    return res
+
+
 def text_to_list(data):
     res = data.split("\n")
 
     return list(filter(bool, map(str.strip, res)))
 
 
 def deduplicate(items):
```

### Comparing `apixdev-0.3.0/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.1/apixdev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.0
+Version: 0.3.1
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.0/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.1/apixdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.0/setup.py` & `apixdev-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.3.0",
+    version="0.3.1",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
@@ -31,15 +31,14 @@
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
         "click>=8.1.6",
         "OdooRPC>=0.9.0",
         "PyYAML>=6.0.1",
         "requests>=2.28.2",
-        "sh>=2.0.4",
         "requirements-parser>=0.5.0",
         "git-aggregator>=4.0",
         "packaging>=23.1",
         "pandas>=2.0.0",
     ],
     entry_points={
         "console_scripts": [
```

