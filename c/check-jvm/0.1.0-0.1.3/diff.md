# Comparing `tmp/check_jvm-0.1.0.tar.gz` & `tmp/check_jvm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_jvm-0.1.0.tar", max compression
+gzip compressed data, was "check_jvm-0.1.3.tar", max compression
```

## Comparing `check_jvm-0.1.0.tar` & `check_jvm-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1098 2023-07-24 02:57:15.199928 check_jvm-0.1.0/LICENSE
--rw-r--r--   0        0        0     1220 2023-07-24 18:47:10.806314 check_jvm-0.1.0/README.md
--rw-r--r--   0        0        0     1872 2023-07-24 18:18:18.069290 check_jvm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      259 2023-07-24 03:14:01.063254 check_jvm-0.1.0/src/check_jvm/__init__.py
--rw-r--r--   0        0        0       49 2023-07-24 17:24:17.454058 check_jvm-0.1.0/src/check_jvm/__main__.py
--rw-r--r--   0        0        0     6191 2023-07-24 17:43:39.355959 check_jvm-0.1.0/src/check_jvm/app.py
--rw-r--r--   0        0        0     3479 2023-07-24 10:21:55.008914 check_jvm-0.1.0/src/check_jvm/java_version.py
--rw-r--r--   0        0        0      192 2023-07-24 03:11:59.386980 check_jvm-0.1.0/src/check_jvm/logger.py
--rw-r--r--   0        0        0        0 2023-07-24 03:12:30.381374 check_jvm-0.1.0/src/check_jvm/py.typed
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 check_jvm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-07-24 02:57:15.199928 check_jvm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1220 2023-07-24 18:47:10.806314 check_jvm-0.1.3/README.md
+-rw-r--r--   0        0        0     1872 2023-07-24 19:18:14.828265 check_jvm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-07-24 03:14:01.063254 check_jvm-0.1.3/src/check_jvm/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-24 17:24:17.454058 check_jvm-0.1.3/src/check_jvm/__main__.py
+-rw-r--r--   0        0        0     6258 2023-07-24 19:17:48.495218 check_jvm-0.1.3/src/check_jvm/app.py
+-rw-r--r--   0        0        0     3479 2023-07-24 10:21:55.008914 check_jvm-0.1.3/src/check_jvm/java_version.py
+-rw-r--r--   0        0        0      192 2023-07-24 03:11:59.386980 check_jvm-0.1.3/src/check_jvm/logger.py
+-rw-r--r--   0        0        0        0 2023-07-24 03:12:30.381374 check_jvm-0.1.3/src/check_jvm/py.typed
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 check_jvm-0.1.3/PKG-INFO
```

### Comparing `check_jvm-0.1.0/LICENSE` & `check_jvm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `check_jvm-0.1.0/README.md` & `check_jvm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `check_jvm-0.1.0/pyproject.toml` & `check_jvm-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "check-jvm"
-version = "0.1.0"
+version = "0.1.3"
 description = ""
 authors = ["Dániel Hagyárossy <daniel@hagyarossy.hu>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://"
 # documentation = "https://"
 keywords = ["oracle jvm", "jvm checker"]
```

### Comparing `check_jvm-0.1.0/src/check_jvm/app.py` & `check_jvm-0.1.3/src/check_jvm/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,21 @@
 
 
 log = logging.getLogger(__name__)
 exec_name = "java"
 app = typer.Typer()
 scan_status = None
 
+root_dir = "/"
+
 
 def get_java_files(exec_name: str = "java") -> List[Optional[str]]:
     files = []
     tl_dir = ""
-    for dirpath, _, filenames in os.walk("/"):
+    for dirpath, _, filenames in os.walk(root_dir):
         os_path = dirpath.split(os.sep)
         if tl_dir != f"{os_path[0]}{os.sep}{os_path[1]}":
             tl_dir = f"{os_path[0]}{os.sep}{os_path[1]}"
             log.info(f"Processing '{tl_dir}'")
             if scan_status:
                 scan_status.update(
                     f"Scanning [green]'{tl_dir}'[/] for JAVA files. "
@@ -188,19 +190,21 @@
         bool, typer.Option("--verbose", "-v", help="Verbose output.")
     ] = False,
     debug: Annotated[
         bool, typer.Option("--debug", "-d", help="Enable debug output.")
     ] = False,
 ):
     global exec_name
+    global root_dir
     global stdin
     global stdout
 
     if platform.system() == "Windows":
         exec_name = "java.exe"
+        root_dir = "C:\\"
 
     start = timeit.default_timer()
     print("The start time is :", start)
 
     # https://stackoverflow.com/questions/44780476/windows-cmd-piping-python-3-5-py-file-results-works-but-pyinstaller-exes-leads
     if stdout.isatty():
         stdout = open(stdout.fileno(), "w", encoding="utf-8", closefd=False)
```

### Comparing `check_jvm-0.1.0/src/check_jvm/java_version.py` & `check_jvm-0.1.3/src/check_jvm/java_version.py`

 * *Files identical despite different names*

### Comparing `check_jvm-0.1.0/PKG-INFO` & `check_jvm-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-jvm
-Version: 0.1.0
+Version: 0.1.3
 Summary: 
 License: MIT
 Keywords: oracle jvm,jvm checker
 Author: Dániel Hagyárossy
 Author-email: daniel@hagyarossy.hu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

