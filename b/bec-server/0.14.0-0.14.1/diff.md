# Comparing `tmp/bec-server-0.14.0.tar.gz` & `tmp/bec-server-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.0.tar", last modified: Fri Jul 21 20:43:47 2023, max compression
+gzip compressed data, was "bec-server-0.14.1.tar", last modified: Mon Jul 24 11:48:11 2023, max compression
```

## Comparing `bec-server-0.14.0.tar` & `bec-server-0.14.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.593832 bec-server-0.14.0/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 20:43:47.593832 bec-server-0.14.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.591832 bec-server-0.14.0/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.0/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.0/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.0/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.0/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.592832 bec-server-0.14.0/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 20:43:47.593832 bec-server-0.14.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-07-21 18:30:48.000000 bec-server-0.14.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.118708 bec-server-0.14.1/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 11:48:11.118708 bec-server-0.14.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.117708 bec-server-0.14.1/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:25:17.000000 bec-server-0.14.1/bec_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-23 06:17:58.000000 bec-server-0.14.1/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:25:17.000000 bec-server-0.14.1/bec_server/service_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-23 06:17:58.000000 bec-server-0.14.1/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.118708 bec-server-0.14.1/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 11:48:11.119707 bec-server-0.14.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-24 11:47:29.000000 bec-server-0.14.1/setup.py
```

### Comparing `bec-server-0.14.0/bec_server/launch.py` & `bec-server-0.14.1/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.0/bec_server/service_handler.py` & `bec-server-0.14.1/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.0/bec_server/tmux_launch.py` & `bec-server-0.14.1/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.0/setup.py` & `bec-server-0.14.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,52 +2,65 @@
 import pathlib
 import subprocess
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
+__version__ = "0.14.1"
 
-def get_version():
-    """load the version from the version file"""
-    version_file = os.path.join(current_path, "../semantic_release", "__init__.py")
-    with open(version_file, "r", encoding="utf-8") as file:
-        res = file.readline()
-        version = res.split("=")[1]
-    return version.strip().strip('"')
+
+def run_install(setup_args, bec_deps, editable=False):
+    """
+    Run the setup function with the given arguments. If editable is True, the dependencies are installed in editable mode.
+    """
+    if editable:
+        # check if "[dev]" was requested
+        if "dev" in os.environ.get("EXTRAS_REQUIRE", ""):
+            suffix = "[dev]"
+        else:
+            suffix = ""
+        setup(**setup_args)
+        deps = [f"{current_path}/../{dep[1]}/" for dep in bec_deps]
+        for dep in deps:
+            subprocess.run(f"pip install -e {dep}{suffix}", shell=True, check=True)
+        return
+
+    install_deps = [dep[0] for dep in bec_deps]
+    setup_args["install_requires"].extend(install_deps)
+    print(setup_args)
+    setup(**setup_args)
 
 
 if __name__ == "__main__":
-    setup(
-        entry_points={"console_scripts": ["bec-server = bec_server:main"]},
-        install_requires=["libtmux"],
-        version=get_version(),
-        extras_require={
+    import sys
+
+    bec_deps = [
+        ("bec_lib", "bec_lib"),
+        ("bec_ipython_client", "bec_client"),
+        ("bec_scan_server", "scan_server"),
+        ("bec_scan_bundler", "scan_bundler"),
+        ("bec_file_writer", "file_writer"),
+        ("bec_dap", "data_processing"),
+        ("bec_device_server", "device_server"),
+        ("bec_scihub", "scihub"),
+    ]
+
+    setup_args = {
+        "entry_points": {"console_scripts": ["bec-server = bec_server:main"]},
+        "install_requires": ["libtmux"],
+        "version": __version__,
+        "extras_require": {
             "dev": [
                 "pytest",
                 "pytest-random-order",
                 "pytest-asyncio",
                 "coverage",
                 "black",
                 "pylint",
             ]
         },
-    )
-    bec_deps = [
-        "bec_lib",
-        "bec_client",
-        "scan_server",
-        "scan_bundler",
-        "file_writer",
-        "data_processing",
-        "device_server",
-        "scihub",
-    ]
-    # check if "[dev]" was requested
-    if "dev" in os.environ.get("EXTRAS_REQUIRE", ""):
-        suffix = "[dev]"
-    else:
-        suffix = ""
-
-    deps = [f"{current_path}/../{dep}/" for dep in bec_deps]
-    for dep in deps:
-        subprocess.run(f"pip install -e {dep}{suffix}", shell=True, check=True)
+    }
+
+    editable = bool("-e" in sys.argv)
+    print(f"editable: {editable}")
+    run_install(setup_args, bec_deps, editable=editable)
```

