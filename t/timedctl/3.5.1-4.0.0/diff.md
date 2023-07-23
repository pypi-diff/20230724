# Comparing `tmp/timedctl-3.5.1.tar.gz` & `tmp/timedctl-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-3.5.1.tar", max compression
+gzip compressed data, was "timedctl-4.0.0.tar", max compression
```

## Comparing `timedctl-3.5.1.tar` & `timedctl-4.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-21 11:07:39.703091 timedctl-3.5.1/LICENSE
--rw-r--r--   0        0        0      810 2023-07-21 11:07:39.703091 timedctl-3.5.1/README.md
--rw-r--r--   0        0        0      849 2023-07-21 11:07:40.495108 timedctl-3.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/__init__.py
--rw-r--r--   0        0        0    36864 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/http_cache.sqlite
--rwxr-xr-x   0        0        0    16931 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/timedctl.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-23 22:54:56.023008 timedctl-4.0.0/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-23 22:54:56.023008 timedctl-4.0.0/README.md
+-rw-r--r--   0        0        0      850 2023-07-23 22:55:16.002652 timedctl-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 22:54:56.023008 timedctl-4.0.0/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    17352 2023-07-23 22:54:56.023008 timedctl-4.0.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-4.0.0/PKG-INFO
```

### Comparing `timedctl-3.5.1/LICENSE` & `timedctl-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-3.5.1/README.md` & `timedctl-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-3.5.1/pyproject.toml` & `timedctl-4.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "3.5.1"
+version = "v4.0.0"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.3.0"
+libtimed = "^0.4.0"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 click-aliases = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `timedctl-3.5.1/timedctl/timedctl.py` & `timedctl-4.0.0/timedctl/timedctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,20 +200,21 @@
         {"date": date}, include="task,task.project,task.project.customer"
     )
     table = [["Customer", "Project", "Task", "Comment", "Duration"]]
     for report in reports:
         task_obj = report["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
-        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"], cached=True)
+        project_obj = timed.projects.get(
+            id=task_obj["relationships"]["project"]["id"], cached=True
+        )
         project = project_obj["attributes"]["name"]
 
         customer_obj = timed.customers.get(
-            id=project_obj["relationships"]["customer"]["data"]["id"],
-            cached=True
+            id=project_obj["relationships"]["customer"]["data"]["id"], cached=True
         )
         customer = customer_obj["attributes"]["name"]
 
         table.append(
             [
                 customer,
                 project,
@@ -237,20 +238,21 @@
         include="task,task.project,task.project.customer",
     )
     table = [["Activity", "Comment", "Start", "End"]]
     for activity_obj in activities:
         task_obj = activity_obj["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
-        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"], cached=True)
+        project_obj = timed.projects.get(
+            id=task_obj["relationships"]["project"]["id"], cached=True
+        )
         project = project_obj["attributes"]["name"]
 
         customer_obj = timed.customers.get(
-            id=project_obj["relationships"]["customer"]["data"]["id"],
-            cached=True
+            id=project_obj["relationships"]["customer"]["data"]["id"], cached=True
         )
         customer = customer_obj["attributes"]["name"]
 
         table.append(
             [
                 f"{customer} > {project} > {task}",
                 activity_obj["attributes"]["comment"],
@@ -314,39 +316,46 @@
 
 @add.command("report", aliases=["r"])
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 @click.option("--description", default=None)
 @click.option("--duration", default=None)
-def add_report(customer, project, task, description, duration):  # pylint: disable=R0912
+@click.option("--show-archived", default=False, is_flag=True)
+def add_report(
+    customer, project, task, description, duration, show_archived
+):  # pylint: disable=R0912
     """Add report(s)."""
-    customers = timed.customers.get(cached=True)
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
+    customers = timed.customers.get(cached=True)
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
-    projects = timed.projects.get({"customer": customer["id"]}, cached=True)
+    projects = timed.projects.get(
+        {"customer": customer["id"]}, filters={"archived": show_archived}, cached=True
+    )
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
-    tasks = timed.tasks.get({"project": project["id"]}, cached=True)
+    tasks = timed.tasks.get(
+        {"project": project["id"]}, filters={"archived": show_archived}, cached=True
+    )
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
     else:
@@ -436,39 +445,44 @@
 
 
 @activity.command(aliases=["add", "a"])
 @click.argument("comment")
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
-def start(comment, customer, project, task):
+@click.option("--show-archived", default=False, is_flag=True)
+def start(comment, customer, project, task, show_archived):
     """Start recording activity."""
-    customers = timed.customers.get(cached=True)
+    customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
-    projects = timed.projects.get({"customer": customer["id"]}, cached=True)
+    projects = timed.projects.get(
+        {"customer": customer["id"]}, filters={"archived": show_archived}, cached=True
+    )
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
-    tasks = timed.tasks.get({"project": project["id"]}, cached=True)
+    tasks = timed.tasks.get(
+        {"project": project["id"]}, filters={"archived": show_archived}, cached=True
+    )
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
     else:
```

### Comparing `timedctl-3.5.1/PKG-INFO` & `timedctl-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 3.5.1
+Version: 4.0.0
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
-Requires-Dist: libtimed (>=0.3.0,<0.4.0)
+Requires-Dist: libtimed (>=0.4.0,<0.5.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

