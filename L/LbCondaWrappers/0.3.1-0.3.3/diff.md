# Comparing `tmp/LbCondaWrappers-0.3.1.tar.gz` & `tmp/LbCondaWrappers-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbCondaWrappers-0.3.1.tar", last modified: Mon May  8 19:17:27 2023, max compression
+gzip compressed data, was "public/LbCondaWrappers-0.3.3.tar", last modified: Mon Jul 24 11:38:20 2023, max compression
```

## Comparing `LbCondaWrappers-0.3.1.tar` & `LbCondaWrappers-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1986 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5960 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5097 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2455 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers/
--rw-r--r--   0 root         (0) root         (0)    18415 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5960 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/tests/test_platforms.py
--rw-r--r--   0 root         (0) root         (0)     7105 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/tests/test_running.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers/
+-rw-r--r--   0 root         (0) root         (0)    19286 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/tests/test_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/tests/test_running.py
```

### Comparing `LbCondaWrappers-0.3.1/.gitignore` & `LbCondaWrappers-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.1/.gitlab-ci.yml` & `LbCondaWrappers-0.3.3/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,15 @@
   stage: test
   image: registry.cern.ch/docker.io/library/python:3.9
   rules:
     - when: always
   before_script:
     - pip install pre-commit
   script:
-    - if [ $CI_COMMIT_BRANCH == "master" ] ; then
-    -   pre-commit run --all-files
-    - else
-    -   git fetch origin master
-    -   pre-commit run --from-ref FETCH_HEAD --to-ref HEAD
-    - fi
+    - pre-commit run --all-files
   variables:
     PRE_COMMIT_HOME: ${CI_PROJECT_DIR}/.cache/pre-commit
   cache:
     paths:
       - ${PRE_COMMIT_HOME}
 
 pytest:
```

### Comparing `LbCondaWrappers-0.3.1/.pre-commit-config.yaml` & `LbCondaWrappers-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.1/LICENSE` & `LbCondaWrappers-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.1/PKG-INFO` & `LbCondaWrappers-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.1
+Version: 0.3.3
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.1/README.md` & `LbCondaWrappers-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.1/setup.py` & `LbCondaWrappers-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         "Programming Language :: Python :: 3.9",
     ],
     keywords="LHCb Core task runner",
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.6",
     setup_requires=["setuptools_scm"],
-    install_requires=[],
+    install_requires=["lb_telemetry"],
     extras_require={"testing": ["pytest", "pytest-cov"]},
     package_data={"LbCondaWrappers": package_data},
     entry_points={
         "console_scripts": [
             "lb-conda=LbCondaWrappers:lb_conda",
             "lb-conda-dev=LbCondaWrappers:lb_conda_dev",
         ]
```

### Comparing `LbCondaWrappers-0.3.1/src/LbCondaWrappers/__init__.py` & `LbCondaWrappers-0.3.3/src/LbCondaWrappers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import subprocess
 import sys
 import tempfile
 from collections import defaultdict
 from datetime import datetime
 from os.path import basename, isdir, join, relpath
 
+from lb_telemetry import Logger
+
 
 def compute_conda_subdir():
     if "CONDA_SUBDIR" in os.environ:
         return os.environ["CONDA_SUBDIR"]
     conda_platform = platform.system().lower()
     conda_platform = {"darwin": "osx"}.get(conda_platform, conda_platform)
     conda_arch = platform.machine()
@@ -131,16 +133,17 @@
 
     return envs, display_versions
 
 
 CONDA_ENVIRONMENTS, DISPLAY_VERSIONS = list_environments()
 
 
-def get_env_prefix(env_string):
-    if env_string in CONDA_ENVIRONMENTS:
+def get_env_details(env_string):
+    latest = env_string in CONDA_ENVIRONMENTS
+    if latest:
         env_name = env_string
         env_version = max(CONDA_ENVIRONMENTS[env_string])
     else:
         split_dirpath = env_string.split(os.sep)
         env_name = "/".join(split_dirpath[:-1])
         env_version = split_dirpath[-1]
 
@@ -160,18 +163,33 @@
         env_version = split_dirpath[-1]
         if env_version not in CONDA_ENVIRONMENTS[env_name]:
             sys.stderr.write(
                 "ERROR: No version " + env_version + " found for " + env_name + "\n"
             )
             sys.exit(31)
 
+    return env_name, env_version, latest
+
+
+def get_env_prefix(env_string):
+    env_name, env_version, _ = get_env_details(env_string)
     return CONDA_ENVIRONMENTS[env_name][env_version]
 
 
-def call_in_conda(command, env_prefix, *, with_venv=None, texlive=None, extravars=None):
+def call_in_conda(
+    command,
+    env_prefix,
+    env_name,
+    env_version,
+    latest,
+    *,
+    with_venv=None,
+    texlive=None,
+    extravars=None,
+):
     """Replace the current process with a command in the conda environment
 
     If the command is successfully executed this function will never return.
     """
     env = {k: v for k, v in os.environ.items() if ENV_VAR_WHITELIST.match(k)}
     for var_name, var_value in env.items():
         if re.fullmatch(r"(LANG|LC.*)", var_name) and var_value.lower() == "utf-8":
@@ -227,14 +245,29 @@
         raise NotImplementedError(
             "Unable to launch %s as only bash is supported for now"
             % basename(command[0]),
         )
     else:
         exec_command = " ".join(pipes.quote(x) for x in command)
 
+    telemetry = {
+        "conda-subdir": compute_conda_subdir(),
+        "env_name": env_name,
+        "env_version": env_version,
+        "latest": bool(latest),
+        "with_texlive": bool(texlive),
+    }
+
+    Logger().log_to_monit(
+        "LbConda",
+        telemetry,
+        tags=["latest", "with_texlive"],
+        include_host_info=True,
+    )
+
     logging.debug("Running command %s", exec_command)
     sys.stdout.flush()
     sys.stderr.flush()
     os.execvpe("bash", ["bash", "--norc", "--noprofile", "-c", exec_command], env)
 
 
 def cvmfs_lhcbdev_available(path="/cvmfs/lhcbdev.cern.ch"):
@@ -290,29 +323,32 @@
     args = parser.parse_args()
 
     if not cvmfs_lhcbdev_available():
         sys.stderr.write("ERROR: /cvmfs/lhcbdev.cern.ch unavailable\n")
         sys.exit(1)
 
     if args.command:
+        env_name, env_version, latest = get_env_details(args.command[0])
         env_prefix = get_env_prefix(args.command[0])
         command = args.command[1:] or ["bash"]
     else:
+        env_name = None
+        env_version = None
+        latest = None
         env_prefix = None
         command = None
 
+    texlive = None
     if args.texlive_version:
         texlive = args.texlive_version
     elif args.texlive:
         if list_textlive_versions():
             texlive = max(list_textlive_versions())
         else:
             parser.error("There are no versions of texlive available on this host")
-    else:
-        texlive = None
 
     if args.list or (len(args.command) >= 2 and args.command[1] == "--list"):
         # Handle --list
         if args.command:
             try:
                 print(*sorted(DISPLAY_VERSIONS[args.command[0]]), sep="\n")
                 sys.exit(0)
@@ -340,15 +376,23 @@
     extravars = {}
     for newvar in args.environment_variables or []:
         newvarname, newvarval = newvar.split("=", 1)
         extravars[newvarname] = newvarval
 
     # Try to replace the current process with the desired command
     try:
-        call_in_conda(command, env_prefix, texlive=texlive, extravars=extravars)
+        call_in_conda(
+            command,
+            env_prefix,
+            env_name,
+            env_version,
+            latest,
+            texlive=texlive,
+            extravars=extravars,
+        )
     except Exception as e:
         sys.stderr.write("ERROR: %s\n" % e)
         sys.exit(1)
 
 
 def lb_conda_dev():
     """Invoke a commands in the correct environment"""
```

### Comparing `LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/PKG-INFO` & `LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.1
+Version: 0.3.3
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.1/tests/test_platforms.py` & `LbCondaWrappers-0.3.3/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.1/tests/test_running.py` & `LbCondaWrappers-0.3.3/tests/test_running.py`

 * *Files identical despite different names*

