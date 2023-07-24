# Comparing `tmp/timedctl-5.0.1.tar.gz` & `tmp/timedctl-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.1.tar", max compression
+gzip compressed data, was "timedctl-5.0.2.tar", max compression
```

## Comparing `timedctl-5.0.1.tar` & `timedctl-5.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-23 23:55:15.711716 timedctl-5.0.1/LICENSE
--rw-r--r--   0        0        0      774 2023-07-23 23:55:15.711716 timedctl-5.0.1/README.md
--rw-r--r--   0        0        0      849 2023-07-23 23:55:35.735773 timedctl-5.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 23:55:15.715716 timedctl-5.0.1/timedctl/__init__.py
--rwxr-xr-x   0        0        0    17352 2023-07-23 23:55:15.715716 timedctl-5.0.1/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-24 07:10:31.837005 timedctl-5.0.2/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-24 07:10:31.837005 timedctl-5.0.2/README.md
+-rw-r--r--   0        0        0      849 2023-07-24 07:10:56.961224 timedctl-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 07:10:31.837005 timedctl-5.0.2/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    17405 2023-07-24 07:10:31.837005 timedctl-5.0.2/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.2/PKG-INFO
```

### Comparing `timedctl-5.0.1/LICENSE` & `timedctl-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.1/README.md` & `timedctl-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.1/pyproject.toml` & `timedctl-5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.1"
+version = "5.0.2"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.4.0"
+libtimed = "^0.4.1"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 click-aliases = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `timedctl-5.0.1/timedctl/timedctl.py` & `timedctl-5.0.2/timedctl/timedctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     # format as HH:MM:SS
     return str(total)
 
 
 def select_report(date):
     """FZF prompt to select a report."""
     reports = timed.reports.get(
-        {"date": date}, include="task,task.project,task.project.customer"
+        filters={"date": date}, include="task,task.project,task.project.customer"
     )
     report_view = []
     for report in reports:
         task = report["relationships"]["task"]
         report_view.append(
             [
                 task["attributes"]["name"],
@@ -193,15 +193,15 @@
 
 
 @get.command("reports", aliases=["report", "r"])
 @click.option("--date", default=None)
 def get_reports(date):
     """Get reports."""
     reports = timed.reports.get(
-        {"date": date}, include="task,task.project,task.project.customer"
+        filters={"date": date}, include="task,task.project,task.project.customer"
     )
     table = [["Customer", "Project", "Task", "Comment", "Duration"]]
     for report in reports:
         task_obj = report["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
         project_obj = timed.projects.get(
@@ -230,15 +230,15 @@
 
 
 @get.command("activities", aliases=["a", "ac", "activity"])
 @click.option("--date", default=None)
 def get_activities(date):
     """Get activities."""
     activities = timed.activities.get(
-        {"day": date},
+        filters={"day": date},
         include="task,task.project,task.project.customer",
     )
     table = [["Activity", "Comment", "Start", "End"]]
     for activity_obj in activities:
         task_obj = activity_obj["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
@@ -324,37 +324,37 @@
 def add_report(
     customer, project, task, description, duration, show_archived
 ):  # pylint: disable=R0912
     """Add report(s)."""
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
-    customers = timed.customers.get(cached=True)
+    customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
     projects = timed.projects.get(
-        {"customer": customer["id"]}, filters={"archived": show_archived}, cached=True
+        filters={"customer": customer["id"], "archived": show_archived}, cached=True
     )
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
     tasks = timed.tasks.get(
-        {"project": project["id"]}, filters={"archived": show_archived}, cached=True
+        filters={"project": project["id"], "archived": show_archived}, cached=True
     )
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
@@ -461,27 +461,27 @@
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
     projects = timed.projects.get(
-        {"customer": customer["id"]}, filters={"archived": show_archived}, cached=True
+        filters={"customer": customer["id"], "archived": show_archived}, cached=True
     )
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
     tasks = timed.tasks.get(
-        {"project": project["id"]}, filters={"archived": show_archived}, cached=True
+        filters={"project": project["id"], "archived": show_archived}, cached=True
     )
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
```

### Comparing `timedctl-5.0.1/PKG-INFO` & `timedctl-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.1
+Version: 5.0.2
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
-Requires-Dist: libtimed (>=0.4.0,<0.5.0)
+Requires-Dist: libtimed (>=0.4.1,<0.5.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

