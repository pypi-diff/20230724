# Comparing `tmp/pisync-0.0.5.tar.gz` & `tmp/pisync-0.0.6.tar.gz`

## Comparing `pisync-0.0.5.tar` & `pisync-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pisync-0.0.5/Makefile
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pisync-0.0.5/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pisync-0.0.5/examples/run_backups.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/__about__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/config/__init__.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/config/base_config.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/config/local_config.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/config/remote_config.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pisync-0.0.5/src/pisync/util/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pisync-0.0.5/tests/test_backup.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pisync-0.0.5/tests/test_local_config.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pisync-0.0.5/tests/test_remote_config.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pisync-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.5/LICENSE
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pisync-0.0.5/README.md
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 pisync-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 pisync-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pisync-0.0.6/Makefile
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pisync-0.0.6/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pisync-0.0.6/examples/run_backups.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/__about__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/config/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/config/base_config.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/config/local_config.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/config/remote_config.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pisync-0.0.6/src/pisync/util/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pisync-0.0.6/tests/test_backup.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pisync-0.0.6/tests/test_local_config.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pisync-0.0.6/tests/test_remote_config.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pisync-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pisync-0.0.6/README.md
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 pisync-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 pisync-0.0.6/PKG-INFO
```

### Comparing `pisync-0.0.5/Makefile` & `pisync-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/.github/workflows/main.yaml` & `pisync-0.0.6/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/examples/run_backups.py` & `pisync-0.0.6/examples/run_backups.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/src/pisync/config/base_config.py` & `pisync-0.0.6/src/pisync/config/base_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/src/pisync/config/local_config.py` & `pisync-0.0.6/src/pisync/config/local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/src/pisync/config/remote_config.py` & `pisync-0.0.6/src/pisync/config/remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/src/pisync/util/__init__.py` & `pisync-0.0.6/src/pisync/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/tests/conftest.py` & `pisync-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/tests/test_backup.py` & `pisync-0.0.6/tests/test_backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/tests/test_local_config.py` & `pisync-0.0.6/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/tests/test_remote_config.py` & `pisync-0.0.6/tests/test_remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/LICENSE` & `pisync-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/README.md` & `pisync-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     log_file="/tmp/backup-logs/backups.log" # local machine
 )
 
 backup(local_docs)
 backup(remote_docs)
 ```
 
-Also see [an example config](example config) for how I backup my home server
+Also see [an example config][example config] for how I backup my home server
 both locally and to an offsite [raspberry pi][pi].
 
 # Notes
 
 ## Safety
 
 - Creating a `LocalConfig` or `RemoteConfig` object will fail if `source_dir`
```

### Comparing `pisync-0.0.5/pyproject.toml` & `pisync-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.5/PKG-INFO` & `pisync-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisync
-Version: 0.0.5
+Version: 0.0.6
 Summary: Minimal incremental backup script using rsync 
 Project-URL: Documentation, https://github.com/erietz/pisync#readme
 Project-URL: Issues, https://github.com/erietz/pisync/issues
 Project-URL: Source, https://github.com/erietz/pisync
 Author-email: erietz <ewrietz@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -57,15 +57,15 @@
     log_file="/tmp/backup-logs/backups.log" # local machine
 )
 
 backup(local_docs)
 backup(remote_docs)
 ```
 
-Also see [an example config](example config) for how I backup my home server
+Also see [an example config][example config] for how I backup my home server
 both locally and to an offsite [raspberry pi][pi].
 
 # Notes
 
 ## Safety
 
 - Creating a `LocalConfig` or `RemoteConfig` object will fail if `source_dir`
```

