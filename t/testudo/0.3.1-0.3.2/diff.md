# Comparing `tmp/testudo-0.3.1.tar.gz` & `tmp/testudo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testudo-0.3.1.tar", last modified: Mon Jun  5 00:06:11 2023, max compression
+gzip compressed data, was "testudo-0.3.2.tar", last modified: Mon Jul 24 01:12:06 2023, max compression
```

## Comparing `testudo-0.3.1.tar` & `testudo-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34500 2023-03-01 02:56:07.690971 testudo-0.3.1/LICENSE
--rw-r--r--   0        0        0     2370 2023-03-01 02:56:07.690971 testudo-0.3.1/README.md
--rw-r--r--   0        0        0     1542 2023-06-05 00:03:26.345861 testudo-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-04 23:58:01.870951 testudo-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2929 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/integration/test_reporter.py
--rw-r--r--   0        0        0     1589 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/integration/test_runner.py
--rw-r--r--   0        0        0        0 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0       35 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/resources/basic_config.yaml
--rw-r--r--   0        0        0     1118 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_cli.py
--rw-r--r--   0        0        0      788 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_config.py
--rw-r--r--   0        0        0     4569 2023-06-04 23:58:01.870951 testudo-0.3.1/tests/unit/test_reporter.py
--rw-r--r--   0        0        0     2550 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_runner.py
--rw-r--r--   0        0        0     3288 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_task_manager.py
--rw-r--r--   0        0        0      256 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/utils.py
--rw-r--r--   0        0        0        0 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/__init__.py
--rw-r--r--   0        0        0     1762 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/cli.py
--rw-r--r--   0        0        0      995 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/config.py
--rw-r--r--   0        0        0      246 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/log.py
--rw-r--r--   0        0        0     3837 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/reporter.py
--rw-r--r--   0        0        0     3857 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/runner.py
--rw-r--r--   0        0        0     5134 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/task_manager.py
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 testudo-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-06-13 00:54:25.977209 testudo-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2370 2023-06-13 00:54:25.977209 testudo-0.3.2/README.md
+-rw-r--r--   0        0        0     1542 2023-07-24 01:08:22.874645 testudo-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/integration/test_reporter.py
+-rw-r--r--   0        0        0     1589 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/integration/test_runner.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/resources/basic_config.yaml
+-rw-r--r--   0        0        0     1118 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      788 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/test_config.py
+-rw-r--r--   0        0        0     4569 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/test_reporter.py
+-rw-r--r--   0        0        0     2550 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/test_runner.py
+-rw-r--r--   0        0        0     3288 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/test_task_manager.py
+-rw-r--r--   0        0        0      256 2023-06-13 00:54:25.977209 testudo-0.3.2/tests/unit/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/__init__.py
+-rw-r--r--   0        0        0     1674 2023-07-24 01:07:57.849577 testudo-0.3.2/testudo/cli.py
+-rw-r--r--   0        0        0      995 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/config.py
+-rw-r--r--   0        0        0      246 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/log.py
+-rw-r--r--   0        0        0     3837 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/reporter.py
+-rw-r--r--   0        0        0     3857 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/runner.py
+-rw-r--r--   0        0        0     5134 2023-06-13 00:54:25.977209 testudo-0.3.2/testudo/task_manager.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 testudo-0.3.2/PKG-INFO
```

### Comparing `testudo-0.3.1/LICENSE` & `testudo-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/README.md` & `testudo-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/pyproject.toml` & `testudo-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testudo"
-version = "0.3.1"
+version = "0.3.2"
 description = "A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory."
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "click<9.0.0,>=8.0.3",
     "legion-utils<1.0.0,>=0.3.2",
```

### Comparing `testudo-0.3.1/tests/integration/test_reporter.py` & `testudo-0.3.2/tests/integration/test_reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/integration/test_runner.py` & `testudo-0.3.2/tests/integration/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/unit/test_cli.py` & `testudo-0.3.2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/unit/test_config.py` & `testudo-0.3.2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/unit/test_reporter.py` & `testudo-0.3.2/tests/unit/test_reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/unit/test_runner.py` & `testudo-0.3.2/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/tests/unit/test_task_manager.py` & `testudo-0.3.2/tests/unit/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/testudo/cli.py` & `testudo-0.3.2/testudo/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from signal import signal, SIGINT
 from threading import Event
 from typing import Optional
 from logging import DEBUG, INFO
 
 import click
 from yaml import safe_load
-from logzero import loglevel as set_loglevel
 
 from testudo.config import TaskConfig
 from testudo.log import log
 from testudo.runner import run_with_reporter
 
 DEFAULT_CONFIG = Path.cwd() / 'config.yaml'
 
@@ -25,15 +24,14 @@
               type=click.Path(file_okay=True, dir_okay=False,
                               writable=True, readable=True,
                               resolve_path=True, allow_dash=False),
               help="Path to the database file")
 @click.option('--debug', is_flag=True, help='Set logging level to DEBUG')
 def main(config_file: Optional[str], database_file: str, debug: bool) -> None:
     """A script for printing hello world based on some configured values"""
-    set_loglevel(DEBUG if debug else INFO)
     halt_flag = Event()
 
     def handle_sigint(_, __):
         log.info("SIGINT Received, sending shutdown signal...")
         halt_flag.set()
 
     log.debug('Configuring SIGINT handler...')
```

### Comparing `testudo-0.3.1/testudo/config.py` & `testudo-0.3.2/testudo/config.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/testudo/reporter.py` & `testudo-0.3.2/testudo/reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/testudo/runner.py` & `testudo-0.3.2/testudo/runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/testudo/task_manager.py` & `testudo-0.3.2/testudo/task_manager.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.1/PKG-INFO` & `testudo-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testudo
-Version: 0.3.1
+Version: 0.3.2
 Summary: A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory.
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Testudo
```

