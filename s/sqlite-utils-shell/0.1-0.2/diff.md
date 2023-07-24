# Comparing `tmp/sqlite-utils-shell-0.1.tar.gz` & `tmp/sqlite-utils-shell-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-utils-shell-0.1.tar", last modified: Mon Jul 24 03:48:19 2023, max compression
+gzip compressed data, was "sqlite-utils-shell-0.2.tar", last modified: Mon Jul 24 14:44:47 2023, max compression
```

## Comparing `sqlite-utils-shell-0.1.tar` & `sqlite-utils-shell-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:48:19.245335 sqlite-utils-shell-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 03:48:03.000000 sqlite-utils-shell-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-24 03:48:19.245335 sqlite-utils-shell-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-24 03:48:03.000000 sqlite-utils-shell-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 03:48:03.000000 sqlite-utils-shell-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:48:19.245335 sqlite-utils-shell-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:48:19.245335 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:48:19.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-24 03:48:03.000000 sqlite-utils-shell-0.1/sqlite_utils_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:48:19.245335 sqlite-utils-shell-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-24 03:48:03.000000 sqlite-utils-shell-0.1/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:44:47.830537 sqlite-utils-shell-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 14:44:27.000000 sqlite-utils-shell-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-24 14:44:47.830537 sqlite-utils-shell-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-24 14:44:27.000000 sqlite-utils-shell-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 14:44:27.000000 sqlite-utils-shell-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:44:47.830537 sqlite-utils-shell-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:44:47.830537 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 14:44:47.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-24 14:44:27.000000 sqlite-utils-shell-0.2/sqlite_utils_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:44:47.830537 sqlite-utils-shell-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 14:44:27.000000 sqlite-utils-shell-0.2/tests/test_shell.py
```

### Comparing `sqlite-utils-shell-0.1/LICENSE` & `sqlite-utils-shell-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-utils-shell-0.1/PKG-INFO` & `sqlite-utils-shell-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-shell
-Version: 0.1
+Version: 0.2
 Summary: An interactive shell for sqlite-utils
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/sqlite-utils-shell
 Project-URL: Changelog, https://github.com/simonw/sqlite-utils-shell/releases
 Project-URL: Issues, https://github.com/simonw/sqlite-utils-shell/issues
 Project-URL: CI, https://github.com/simonw/sqlite-utils-shell/actions
```

### Comparing `sqlite-utils-shell-0.1/README.md` & `sqlite-utils-shell-0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlite-utils-shell-0.1/pyproject.toml` & `sqlite-utils-shell-0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlite-utils-shell"
-version = "0.1"
+version = "0.2"
 description = "An interactive shell for sqlite-utils"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `sqlite-utils-shell-0.1/sqlite_utils_shell.egg-info/PKG-INFO` & `sqlite-utils-shell-0.2/sqlite_utils_shell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-shell
-Version: 0.1
+Version: 0.2
 Summary: An interactive shell for sqlite-utils
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/sqlite-utils-shell
 Project-URL: Changelog, https://github.com/simonw/sqlite-utils-shell/releases
 Project-URL: Issues, https://github.com/simonw/sqlite-utils-shell/issues
 Project-URL: CI, https://github.com/simonw/sqlite-utils-shell/actions
```

### Comparing `sqlite-utils-shell-0.1/sqlite_utils_shell.py` & `sqlite-utils-shell-0.2/sqlite_utils_shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,75 +36,88 @@
     readline.parse_and_bind("tab: complete")
 readline.set_completer(completer)
 
 
 @sqlite_utils.hookimpl
 def register_commands(cli):
     @cli.command()
-    @click.argument("path", type=click.Path(dir_okay=False, readable=True), required=False)
+    @click.argument(
+        "path", type=click.Path(dir_okay=False, readable=True), required=False
+    )
     def shell(path):
         "Start an interactive SQL shell for this database"
-        run_sql_shell(path)
+        run_sql_shell(path, input, print)
 
 
-def run_sql_shell(path):
+def run_sql_shell(path, input_, print_):
     if path:
         db = sqlite_utils.Database(path)
-        print("Attached to {}".format(path))
+        print_("Attached to {}".format(path))
     else:
         db = sqlite_utils.Database(memory=True)
-        print("In-memory database, content will be lost on exit")
+        print_("In-memory database, content will be lost on exit")
 
-    print("Type 'exit' to exit.")
+    print_("Type 'exit' to exit.")
 
     statement = ""
 
     prompt = "sqlite-utils> "
 
+    def is_valid_query(sql):
+        try:
+            db.execute("explain " + sql)
+        except sqlite3.OperationalError:
+            return False
+        return True
+
     while True:
-        line = input(prompt)
+        line = input_(prompt)
         if line:
             readline.add_history(line)
 
         prompt = "         ...> "
 
         if line.lower() in ("exit", "quit"):
             break
 
         statement += "\n" + line
 
-        if sqlite3.complete_statement(statement):
+        if sqlite3.complete_statement(statement) or (
+            not statement.strip().endswith(";") and is_valid_query(statement + ";")
+        ):
             try:
                 statement = statement.strip()
                 cursor = db.execute(statement)
                 if cursor.description is None:
                     # It was create table / insert / update
                     rowcount = cursor.rowcount
                     if rowcount != -1:
-                        print(
+                        print_(
                             "{} row{} affected".format(
                                 rowcount, "s" if rowcount != 1 else ""
                             )
                         )
+                    else:
+                        print_("Done")
                 else:
                     headers = [row[0] for row in cursor.description]
 
                     # Only show first MAX_ROWS_TO_RETURN
                     first_rows = list(cursor.fetchmany(MAX_ROWS_TO_RETURN + 1))
                     has_more = len(first_rows) == MAX_ROWS_TO_RETURN + 1
-                    print(
+                    print_(
                         tabulate.tabulate(
                             first_rows[:MAX_ROWS_TO_RETURN], headers=headers
                         )
                     )
                     if has_more:
-                        print("[ results were truncated ]")
+                        print_("[ results were truncated ]")
 
             except sqlite3.Error as e:
-                print("An error occurred:", e)
+                print_("An error occurred:", e)
 
             finally:
                 prompt = "sqlite-utils> "
 
             statement = ""
 
     db.conn.close()
```

