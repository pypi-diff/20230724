# Comparing `tmp/bec-server-0.14.3.tar.gz` & `tmp/bec-server-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.3.tar", last modified: Mon Jul 24 12:06:02 2023, max compression
+gzip compressed data, was "bec-server-0.14.4.tar", last modified: Mon Jul 24 15:02:34 2023, max compression
```

## Comparing `bec-server-0.14.3.tar` & `bec-server-0.14.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.952386 bec-server-0.14.3/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 12:06:02.952386 bec-server-0.14.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.951386 bec-server-0.14.3/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.3/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.3/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.3/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.3/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.952386 bec-server-0.14.3/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 12:06:02.953385 bec-server-0.14.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-24 12:05:30.000000 bec-server-0.14.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.881447 bec-server-0.14.4/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 15:02:34.882447 bec-server-0.14.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.880447 bec-server-0.14.4/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.4/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.4/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.4/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.4/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.881447 bec-server-0.14.4/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 15:02:34.882447 bec-server-0.14.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-24 15:02:01.000000 bec-server-0.14.4/setup.py
```

### Comparing `bec-server-0.14.3/bec_server/launch.py` & `bec-server-0.14.4/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.3/bec_server/service_handler.py` & `bec-server-0.14.4/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.3/bec_server/tmux_launch.py` & `bec-server-0.14.4/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.3/setup.py` & `bec-server-0.14.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 import pathlib
 import subprocess
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "0.14.3"
+__version__ = "0.14.4"
 
 
-def run_install(setup_args, bec_deps, editable=False):
+def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
-    Run the setup function with the given arguments. If editable is True, the dependencies are installed in editable mode.
+    Run the setup function with the given arguments.
+
+    Args:
+        setup_args (dict): Arguments for the setup function.
+        bec_deps (list): List of tuples with the dependencies of the BEC server.
+        editable (bool, optional): If True, the dependencies are installed in editable mode. Defaults to False.
     """
     if editable:
         # check if "[dev]" was requested
         if "dev" in os.environ.get("EXTRAS_REQUIRE", ""):
             suffix = "[dev]"
         else:
             suffix = ""
@@ -28,16 +33,14 @@
     install_deps = [dep[0] for dep in bec_deps]
     setup_args["install_requires"].extend(install_deps)
     print(setup_args)
     setup(**setup_args)
 
 
 if __name__ == "__main__":
-    import sys
-
     bec_deps = [
         ("bec_lib", "bec_lib"),
         ("bec_ipython_client", "bec_client"),
         ("bec_scan_server", "scan_server"),
         ("bec_scan_bundler", "scan_bundler"),
         ("bec_file_writer", "file_writer"),
         ("bec_dap", "data_processing"),
@@ -57,10 +60,9 @@
                 "coverage",
                 "black",
                 "pylint",
             ]
         },
     }
 
-    editable = bool("-e" in sys.argv)
-    print(f"editable: {editable}")
+    editable = os.path.dirname(os.path.abspath(__file__)).split("/")[-1] == "bec_server"
     run_install(setup_args, bec_deps, editable=editable)
```

