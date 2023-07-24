# Comparing `tmp/pisync-0.0.3.tar.gz` & `tmp/pisync-0.0.4.tar.gz`

## Comparing `pisync-0.0.3.tar` & `pisync-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,20 @@
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pisync-0.0.3/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pisync-0.0.3/dev-requirements.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pisync-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pisync-0.0.3/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pisync-0.0.3/examples/run_backups.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/__init__.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/backup.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/util.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/base_config.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/local_config.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/remote_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_backup.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_local_config.py
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_remote_config.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pisync-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.3/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pisync-0.0.3/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pisync-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 pisync-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pisync-0.0.4/Makefile
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pisync-0.0.4/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pisync-0.0.4/examples/run_backups.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/__about__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/config/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/config/base_config.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/config/local_config.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/config/remote_config.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pisync-0.0.4/src/pisync/util/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pisync-0.0.4/tests/test_backup.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pisync-0.0.4/tests/test_local_config.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pisync-0.0.4/tests/test_remote_config.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pisync-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pisync-0.0.4/README.md
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 pisync-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pisync-0.0.4/PKG-INFO
```

### Comparing `pisync-0.0.3/.github/workflows/main.yaml` & `pisync-0.0.4/.github/workflows/main.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,49 @@
-# This workflow will install Python dependencies, run tests and lint with a
-# variety of Python versions For more information see:
-# https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
-
 name: Python package
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
-
   lint:
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v3
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8
-    - name: Lint with flake8
+        pip install hatch
+    - name: Lint
       run: |
-        # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics --per-file-ignores="__init__.py:F401"
-        # The GitHub editor is 127 chars wide
-        flake8 . --count --max-complexity=10 --max-line-length=127 --statistics --per-file-ignores="__init__.py:F401"
-
+        hatch run lint:all
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
-
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Allow password-less ssh into localhost for tests
       run: |
         ssh-keygen -t ed25519 -f ~/.ssh/id_ed25519 -N ''
         cat > ~/.ssh/config <<EOF
           HOST *
             StrictHostKeyChecking no
         EOF
         chmod og-rw ~
-        ls -al ~/.ssh
         cat ~/.ssh/id_ed25519.pub >> ~/.ssh/authorized_keys
-        ls -al ~/.ssh
-        cat ~/.ssh/authorized_keys
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        python -m pip install -e .
+        pip install hatch
     - name: Test with pytest
       run: |
-        pytest -s -vv
+        hatch run test-cov -s -vv
+        hatch run cov-report
```

### Comparing `pisync-0.0.3/examples/run_backups.py` & `pisync-0.0.4/examples/run_backups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
+import sys
+
 from pisync import LocalConfig, RemoteConfig, backup
 
 # will need to be root to run rsync for a different users home dir
 
 log_file = "/home/ethan/.local/share/backup/rsync-backups.log"
 home_dir_exclude_file_patterns = [
-    "/home/*/.cache/",          # no need for cached files
-    "/home/*/.local/",          # nvim plugins and python packages are huge
-    "/home/*/.npm/",            # what is the crap in here?
-    "**/node_modules/",         # yikes
+    "/home/*/.cache/",  # no need for cached files
+    "/home/*/.local/",  # nvim plugins and python packages are huge
+    "/home/*/.npm/",  # what is the crap in here?
+    "**/node_modules/",  # yikes
 ]
 
 local_home_directories = LocalConfig(
     source_dir="/home/",
     destination_dir="/media/backup_drive_linux/home_directory_backups/",
     exclude_file_patterns=home_dir_exclude_file_patterns,
-    log_file=log_file
+    log_file=log_file,
 )
 
 local_large_harddrive = LocalConfig(
-    source_dir="/mnt/hd2",
-    destination_dir="/media/backup_drive_linux/hd2_backups/",
-    log_file=log_file
+    source_dir="/mnt/hd2", destination_dir="/media/backup_drive_linux/hd2_backups/", log_file=log_file
 )
 
 remote_home_directories = RemoteConfig(
     user_at_hostname="ethan@hydrogen.local",
     source_dir="/home/",
     destination_dir="/mnt/hd/sulfur_backups/home_directory_backups",
     exclude_file_patterns=home_dir_exclude_file_patterns,
-    log_file=log_file
+    log_file=log_file,
 )
 
 remote_large_harddrive = RemoteConfig(
     user_at_hostname="ethan@hydrogen.local",
     source_dir="/mnt/hd2/",
     destination_dir="/mnt/hd/sulfur_backups/hd2_backups",
-    log_file=log_file
+    log_file=log_file,
 )
 
 success = True
 
 try:
     backup(local_home_directories)
     backup(local_large_harddrive)
@@ -51,8 +51,8 @@
     backup(remote_home_directories)
     backup(remote_large_harddrive)
 except Exception as e:
     success = False
     print(e)
 
 if not success:
-    exit(1)
+    sys.exit(1)
```

### Comparing `pisync-0.0.3/src/pisync/backup.py` & `pisync-0.0.4/src/pisync/util/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-"""
-Author      : Ethan Rietz
-Date        : 2022-05-23
-Description : Incremental backups script using rsync.
-
-Notes:
-
-https://linuxconfig.org/how-to-create-incremental-backups-using-rsync-on-linux
-"""
-
-from typing import List
 import logging
 import shutil
 import subprocess
 import sys
 import time
+from datetime import datetime
 from pathlib import Path
+from typing import List
+
+from pisync.config.base_config import BackupType, BaseConfig
 
-from pisync.config.base_config import _BaseConfig
 
+class BackupFailedError(Exception):
+    pass
 
-def backup(config: _BaseConfig) -> str:
+
+def backup(config: BaseConfig) -> str:
     """
     Returns the path to the latest backup directory
     """
     enforce_system_requirements()
     configure_logging(config.log_file)
 
     latest_backup_path = config.generate_new_backup_dir_path()
@@ -37,68 +32,66 @@
 This would result a complete backup backup of
 {config.source_dir} rather than an incremental backup.
 This is probably not the intended behavior so we are aborting.
 Make sure that {config.destination_dir} is empty or manually
 create the necessary symlink at {config.link_dir}.
 """
         logging.error(msg)
-        raise Exception(msg)
+        raise BackupFailedError(msg)
 
     if prev_backup_exists:
-        logging.info(
-            f"Starting incremental backup from {config.resolve(config.link_dir)}")
+        backup_method = BackupType.Incremental
+        logging.info(f"Starting incremental backup from {config.resolve(config.link_dir)}")
     else:
+        backup_method = BackupType.Complete
         logging.info(f"No previous backup found at {config.destination_dir}")
-        logging.info(
-            f"Starting a fresh complete backup from {config.source_dir} "
-            "to {config.destination_dir}")
-
-    rsync_command = config.get_rsync_command(
-        latest_backup_path,
-        previous_backup_exists=prev_backup_exists
-    )
+        logging.info(f"Starting a fresh complete backup from {config.source_dir} to {config.destination_dir}")
+
+    rsync_command = config.get_rsync_command(latest_backup_path, backup_method=backup_method)
 
     exit_code = run_rsync(rsync_command)
 
     if exit_code == 0:
         logging.info("Finished backup successfully")
         if config.file_exists(config.link_dir):
             config.unlink(config.link_dir)
         config.symlink_to(config.link_dir, latest_backup_path)
-        logging.info(
-            f"Symlink created from {latest_backup_path} to {config.link_dir}")
+        logging.info(f"Symlink created from {latest_backup_path} to {config.link_dir}")
         return latest_backup_path
     else:
+        msg = f"Backup failed. Rsync exit code: {exit_code}"
+        logging.error(msg)
         # backup failed, we should delete the most recent backup
-        logging.error(f"Backup failed. Rsync exit code: {exit_code}")
         if config.file_exists(latest_backup_path):
             logging.info(f"Deleting failed backup at {latest_backup_path}")
-            shutil.rmtree(latest_backup_path)
-        return None
+            config.rmtree(latest_backup_path)
+        raise BackupFailedError(msg)
+
+
+def get_time_stamp() -> str:
+    now = datetime.now().astimezone()
+    stamp = now.strftime("%Y-%m-%d-%H-%M-%S")
+    return str(stamp)
 
 
 def configure_logging(filename: str):
-    filename = Path(filename)
-    if not filename.parent.exists():
-        filename.parent.mkdir(parents=True)
+    _filename = Path(filename)
+    if not _filename.parent.exists():
+        _filename.parent.mkdir(parents=True)
 
     logging.basicConfig(
-        filename=str(filename.resolve()),
+        filename=str(_filename.resolve()),
         filemode="a",
-        format='%(levelname)s\t%(asctime)s\t%(message)s',
-        datefmt='%m/%d/%Y %I:%M:%S %p',
-        level=logging.INFO
+        format="%(levelname)s\t%(asctime)s\t%(message)s",
+        datefmt="%m/%d/%Y %I:%M:%S %p",
+        level=logging.INFO,
     )
 
 
 def enforce_system_requirements() -> None:
-    if sys.version_info < (3, 6):
-        logging.critical("Requires Python 3.6 due to f strings")
-        sys.exit(1)
-
     if shutil.which("rsync") is None:
         logging.critical("rsync is not installed")
         sys.exit(1)
 
 
 def run_rsync(rsync_command: List[str]) -> int:
     logging.info(f"Running {rsync_command}")
```

### Comparing `pisync-0.0.3/src/pisync/config/base_config.py` & `pisync-0.0.4/src/pisync/config/base_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from abc import ABC, abstractmethod
-from typing import List
+from enum import Enum
+from typing import List, Optional
 
 
-class InvalidPath(Exception):
+class InvalidPathError(Exception):
     pass
 
 
-class _BaseConfig(ABC):
+class BackupType(Enum):
+    Complete = 1
+    Incremental = 2
+
+
+class BaseConfig(ABC):
     source_dir: str
     destination_dir: str
-    exclude_file_patterns: List[str]
+    exclude_file_patterns: Optional[List[str]]
     log_file: str
     link_dir: str
 
     @abstractmethod
     def is_symlink(self, path: str) -> bool:
         """returns true if path is a symbolic link"""
         pass
@@ -30,38 +36,43 @@
 
     @abstractmethod
     def unlink(self, path: str) -> None:
         """Remove this file or symbolic link."""
         pass
 
     @abstractmethod
+    def rmtree(self, path: str) -> None:
+        """Recursively delete directory tree"""
+        pass
+
+    @abstractmethod
     def symlink_to(self, symlink: str, file: str) -> None:
         """Make symlink a symbolic link to file."""
         pass
 
     @abstractmethod
     def resolve(self, path: str) -> str:
         """Make the path absolute, resolving any symlinks."""
         pass
 
     @abstractmethod
-    def ensure_dir_exists(self, path: str):
+    def ensure_dir_exists(self, path: str) -> None:
         """
         :returns: The Path object from the input path str
         :raises:
-            InvalidPath: If path does not exist or is not a directory
+            InvalidPathError: If path does not exist or is not a directory
         """
         pass
 
     @abstractmethod
     def generate_new_backup_dir_path(self) -> str:
         """
         :returns: The Path string of the directory where the new backup will be
         written.
         :raises:
-            InvalidPath: If the destination directory already exists
+            InvalidPathError: If the destination directory already exists
         """
         pass
 
     @abstractmethod
-    def get_rsync_command(self, new_backup_dir: str, previous_backup_exists: bool = False):
+    def get_rsync_command(self, new_backup_dir: str, backup_method: BackupType):
         pass
```

### Comparing `pisync-0.0.3/src/pisync/config/local_config.py` & `pisync-0.0.4/src/pisync/config/local_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import List
 from pathlib import Path
-from pisync.config.base_config import _BaseConfig, InvalidPath
+from shutil import rmtree
+from typing import List, Optional
+
+from pisync.config.base_config import BackupType, BaseConfig, InvalidPathError
 from pisync.util import get_time_stamp
 
 
-class LocalConfig(_BaseConfig):
+class LocalConfig(BaseConfig):
     def __init__(
         self,
         source_dir: str,
         destination_dir: str,
-        exclude_file_patterns: List[str] = None,
-        log_file: str = str(Path.home() / ".local/share/backup/rsync-backups.log")
+        exclude_file_patterns: Optional[List[str]] = None,
+        log_file: Optional[str] = None,
     ):
         self.ensure_dir_exists(source_dir)
         self.ensure_dir_exists(destination_dir)
         self.source_dir = source_dir
         self.destination_dir = destination_dir
         self.exclude_file_patterns = exclude_file_patterns
-        self.log_file = log_file
+        if log_file is None:
+            self.log_file = str(Path.home() / ".local/share/backup/rsync-backups.log")
+        else:
+            self.log_file = log_file
         self.link_dir = str(Path(self.destination_dir) / "latest")
         self._optionless_rsync_arguments = [
-            "--delete",     # delete extraneous files from dest dirs
-            "--archive",    # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
-            "--verbose",    # increase verbosity
+            "--delete",  # delete extraneous files from dest dirs
+            "--archive",  # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
+            "--verbose",  # increase verbosity
         ]
 
     def is_symlink(self, path: str) -> bool:
         return Path(path).is_symlink()
 
     def file_exists(self, path: str) -> bool:
         return Path(path).exists()
 
     def unlink(self, path: str) -> None:
         Path(path).unlink()
 
+    def rmtree(self, path: str) -> None:
+        """Recursively delete directory tree"""
+        rmtree(path)
+
     def symlink_to(self, symlink: str, file: str) -> None:
         Path(symlink).symlink_to(file)
 
     def resolve(self, path: str) -> str:
         """Make the path absolute, resolving any symlinks."""
         return str(Path(path).resolve())
 
     def is_empty_directory(self, path: str) -> bool:
         return not any(Path(path).iterdir())
 
     def ensure_dir_exists(self, path: str):
-        path = Path(path)
-        if not path.exists():
-            raise InvalidPath(f"{path} does not exist")
-        if not path.is_dir():
-            raise InvalidPath(f"{path} is not a directory")
+        _path = Path(path)
+        if not _path.exists():
+            msg = f"{_path} does not exist"
+            raise InvalidPathError(msg)
+        if not _path.is_dir():
+            msg = f"{_path} is not a directory"
+            raise InvalidPathError(msg)
 
     def generate_new_backup_dir_path(self) -> str:
         time_stamp = get_time_stamp()
         new_backup_dir = Path(self.destination_dir) / time_stamp
         if new_backup_dir.exists():
-            raise InvalidPath(
-                f"{new_backup_dir} already exists and will get overwritten"
-            )
+            msg = f"{new_backup_dir} already exists and will get overwritten"
+            raise InvalidPathError(msg)
         else:
             return str(new_backup_dir)
 
-    def get_rsync_command(
-            self,
-            new_backup_dir: str,
-            previous_backup_exists: bool = False
-    ) -> List[str]:
+    def get_rsync_command(self, new_backup_dir: str, backup_method: BackupType) -> List[str]:
         destination = new_backup_dir
         source = self.source_dir
         link_dest = self.link_dir
         option_arguments = []
 
-        if previous_backup_exists:
+        if backup_method == BackupType.Incremental:
             option_arguments.append(f"--link-dest={link_dest}")
 
         if self.exclude_file_patterns is not None:
             for pattern in self.exclude_file_patterns:
                 option_arguments.append(f"--exclude={pattern}")
 
-        return [
-            "rsync",
-            *self._optionless_rsync_arguments,
-            *option_arguments,
-            source,
-            destination
-        ]
+        return ["rsync", *self._optionless_rsync_arguments, *option_arguments, source, destination]
```

### Comparing `pisync-0.0.3/src/pisync/config/remote_config.py` & `pisync-0.0.4/src/pisync/config/remote_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,121 @@
-from typing import List
 from pathlib import Path
-from pisync.config.base_config import _BaseConfig, InvalidPath
-from pisync.util import get_time_stamp
+from typing import List, Optional
+
 from fabric import Connection
 
+from pisync.config.base_config import BackupType, BaseConfig, InvalidPathError
+from pisync.util import get_time_stamp
 
-class RemoteConfig(_BaseConfig):
+
+class RemoteConfig(BaseConfig):
     def __init__(
         self,
         user_at_hostname: str,
         source_dir: str,
         destination_dir: str,
-        exclude_file_patterns: List[str] = None,
-        log_file: str = Path.home() / ".local/share/backup/rsync-backups.log",
+        exclude_file_patterns: Optional[List[str]] = None,
+        log_file: Optional[str] = None,
     ):
         self.user_at_hostname = user_at_hostname
         self.connection: Connection = Connection(user_at_hostname)
         self._ensure_dir_exists_locally(source_dir)
         self.ensure_dir_exists(destination_dir)
         self.source_dir = source_dir
         self.destination_dir = destination_dir
         self.exclude_file_patterns = exclude_file_patterns
-        self.log_file = log_file
+        if log_file is None:
+            self.log_file = str(Path.home() / ".local/share/backup/rsync-backups.log")
+        else:
+            self.log_file = log_file
         self.link_dir = f"{self.destination_dir}/latest"
         self._optionless_rsync_arguments = [
-            "--delete",     # delete extraneous files from dest dirs
-            "--archive",    # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
-
+            "--delete",  # delete extraneous files from dest dirs
+            "--archive",  # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
             # NOTE: these options are linux specific and do not work on the
             # macOS version of rsync.
             # "--acls",       # preserve ACLs (implies --perms)
             # "--xattrs",     # preserve extended attributes
-
-            "--verbose",    # increase verbosity
+            "--verbose",  # increase verbosity
         ]
 
     def _ensure_dir_exists_locally(self, path: str):
-        path = Path(path)
-        if not path.exists():
-            raise InvalidPath(f"{path} does not exist")
-        if not path.is_dir():
-            raise InvalidPath(f"{path} is not a directory")
+        _path = Path(path)
+        if not _path.exists():
+            msg = f"{_path} does not exist"
+            raise InvalidPathError(msg)
+        if not _path.is_dir():
+            msg = f"{_path} is not a directory"
+            raise InvalidPathError(msg)
 
     def is_symlink(self, path: str) -> bool:
         """returns true if path is a symbolic link"""
-        result = self.connection.run(f"test -L {path}", warn=True)
-        return result.ok
+        return self.connection.run(f"test -L {path}", warn=True).ok
 
     def is_empty_directory(self, path: str) -> bool:
         """returns true if path is a directory and contains no files"""
-        result = self.connection.run(f'test -n "$(find {path} -maxdepth 0 -empty)"', warn=True)
-        return result.ok
+        return self.connection.run(f'test -z "$(ls -A {path})"', warn=True).ok
 
     def file_exists(self, path: str) -> bool:
         """returns true if the file or directory exists"""
         return (
-            self.connection.run(f"test -d {path}", warn=True).ok
-            or self.connection.run(f"test -f {path}", warn=True).ok
+            self.connection.run(f"test -d {path}", warn=True).ok or self.connection.run(f"test -f {path}", warn=True).ok
         )
 
     def unlink(self, path: str) -> None:
         """Remove this file or symbolic link."""
         result = self.connection.run(f"rm {path}", warn=True)
         if not result.ok:
-            raise FileNotFoundError(f"Failed to remove {path}")
+            msg = f"Failed to remove {path}"
+            raise FileNotFoundError(msg)
+
+    def rmtree(self, path: str) -> None:
+        """Recursively delete directory tree"""
+        return self.connection.run(f"rm -r {path}").ok
 
     def symlink_to(self, symlink: str, file: str) -> None:
         """Make symlink a symbolic link to file."""
-        result = self.connection.run(f"ln -s {file} {symlink}", warn=True)
-        return result.ok
+        return self.connection.run(f"ln -s {file} {symlink}", warn=True).ok
 
     def resolve(self, path: str) -> str:
         """Make the path absolute, resolving any symlinks."""
-        result = self.connection.run(f"realpath {path}", warn=True)
-        return result.stdout.strip()
+        return self.connection.run(f"realpath {path}", warn=True).stdout.rstrip()
 
-    def ensure_dir_exists(self, path: str) -> str:
+    def ensure_dir_exists(self, path: str) -> None:
         result = self.connection.run(f"test -d {path}", warn=True)
         if not result.ok:
-            raise InvalidPath(f"{path} is not a directory")
+            msg = f"{path} is not a directory"
+            raise InvalidPathError(msg)
 
     def _is_directory(self, path) -> bool:
-        result = self.connection.run(f"test -d {path}", warn=True)
-        return result.ok
+        return self.connection.run(f"test -d {path}", warn=True).ok
 
     def generate_new_backup_dir_path(self) -> str:
         """
         :returns: The Path string of the directory where the new backup will be
         written.
         :raises:
-            InvalidPath: If the destination directory already exists
+            InvalidPathError: If the destination directory already exists
         """
         time_stamp = get_time_stamp()
         new_backup_dir = f"{self.destination_dir}/{time_stamp}"
-        exists = self._is_directory(new_backup_dir) or self.file_exists(new_backup_dir)
+        exists = self._is_directory(new_backup_dir)
         if exists:
-            raise InvalidPath(
-                f"{new_backup_dir} already exists and will get overwritten"
-            )
+            msg = f"{new_backup_dir} already exists and will get overwritten"
+            raise InvalidPathError(msg)
         else:
             return str(new_backup_dir)
 
-    def get_rsync_command(
-            self,
-            new_backup_dir: str,
-            previous_backup_exists: bool = False
-    ) -> List[str]:
+    def get_rsync_command(self, new_backup_dir: str, backup_method: BackupType) -> List[str]:
         destination = f"{self.user_at_hostname}:{new_backup_dir}"
         source = self.source_dir
         link_dest = self.link_dir
         option_arguments = []
 
-        if previous_backup_exists:
+        if backup_method == BackupType.Incremental:
             option_arguments.append(f"--link-dest={link_dest}")
 
         if self.exclude_file_patterns is not None:
             for pattern in self.exclude_file_patterns:
                 option_arguments.append(f"--exclude={pattern}")
 
-        return [
-            "rsync",
-            *self._optionless_rsync_arguments,
-            *option_arguments,
-            source,
-            destination
-        ]
+        return ["rsync", *self._optionless_rsync_arguments, *option_arguments, source, destination]
```

### Comparing `pisync-0.0.3/tests/conftest.py` & `pisync-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.3/tests/test_backup.py` & `pisync-0.0.4/tests/test_backup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from time import sleep
-import unittest
+import getpass
 import os
 import tempfile
+import unittest
 from pathlib import Path
+from time import sleep
+from unittest.mock import Mock, patch
 
-from pisync.backup import backup, run_rsync
-from pisync.config import LocalConfig
+import pytest
 
+from pisync.config import LocalConfig, RemoteConfig
+from pisync.util import BackupFailedError, backup, run_rsync
 
-# class UtilityFunctionTests(unittest.TestCase):
-#     def test_directory_is_empty(self):
-#         with tempfile.TemporaryDirectory() as tmp:
-#             tmp_dir = Path(tmp)
-#             self.assertTrue(directory_is_empty(tmp_dir))
-
-#            new_file = tmp_dir / "new-file-name-here.txt"
-#            new_file.touch()
-#            self.assertFalse(directory_is_empty(tmp_dir))
+
+@pytest.fixture
+def user_at_localhost() -> str:
+    return f"{getpass.getuser()}@localhost"
 
 
 class RunRsyncTests(unittest.TestCase):
     def test_fake_command_exit_zero(self):
         rsync_command = ["ls", "-al"]
         exit_code = run_rsync(rsync_command)
         self.assertEqual(exit_code, 0)
 
     def test_fake_command_exit_non_zero(self):
-        rsync_command = ["ls", "-z"]    # there is no -z options for ls
+        rsync_command = ["ls", "-z"]  # there is no -z options for ls
         exit_code = run_rsync(rsync_command)
         self.assertNotEqual(exit_code, 0)
 
 
 class BackupTests(unittest.TestCase):
     def setUp(self):
         self.src_dir = tempfile.TemporaryDirectory()
@@ -53,56 +51,85 @@
             # act
             latest_backup_path = backup(self.config)
 
             # assert
             files_in_source = list(self.src_dir_path.iterdir())
             self.assertEqual(len(files_in_source), i)
             for source_file in files_in_source:
-                dest_file = self.dest_dir_path/latest_backup_path/source_file
+                dest_file = self.dest_dir_path / latest_backup_path / source_file
                 self.assertTrue(dest_file.exists())
 
             latest_link = self.dest_dir_path / "latest"
             self.assertTrue(latest_link.exists())
             self.assertTrue(latest_link.is_symlink())
             self.assertEqual(os.readlink(latest_link), latest_backup_path)
-            sleep(1)    # next time stamp (in seconds) must be unique
+            sleep(1)  # next time stamp (in seconds) must be unique
 
     def test_backup_saves_accidental_file_deletion_situation(self):
         # arrange
         file_names = [f"test{i}.txt" for i in range(5)]
         for name in file_names:
             file = self.src_dir_path / name
             file.touch()
 
         # act
         first_backup_path = Path(backup(self.config))
         file_to_delete = self.src_dir_path / file_names[3]
         file_to_delete.unlink()
-        sleep(1)    # cannot run two backups at same dest in same second
+        sleep(1)  # cannot run two backups at same dest in same second
         second_backup_path = Path(backup(self.config))
 
         # assert
         files_in_source = list(self.src_dir_path.iterdir())
-        files_in_first_backup = list(
-            (first_backup_path / self.src_dir_path.name).iterdir()
-        )
-        files_in_second_backup = list(
-            (second_backup_path / self.src_dir_path.name).iterdir()
-        )
+        files_in_first_backup = list((first_backup_path / self.src_dir_path.name).iterdir())
+        files_in_second_backup = list((second_backup_path / self.src_dir_path.name).iterdir())
 
         self.assertEqual(len(files_in_source), 4)
         self.assertEqual(len(files_in_first_backup), 5)
         self.assertEqual(len(files_in_second_backup), 4)
 
         # first backup contains all five files
         for name in file_names:
             file = first_backup_path / self.src_dir_path.name / name
             self.assertTrue(file.exists())
 
         # file at index 3 (aka test3.txt) is not in source
         self.assertNotIn(self.src_dir_path / file_names[3], files_in_source)
 
         # file at index 3 (aka test3.txt) is not in latest backup
-        self.assertNotIn(
-            second_backup_path / self.src_dir_path.name / file_names[3],
-            files_in_second_backup
-        )
+        self.assertNotIn(second_backup_path / self.src_dir_path.name / file_names[3], files_in_second_backup)
+
+
+@patch("pisync.util.run_rsync", Mock(return_value=1))
+def test_local_backup_rsync_fails_removes_previous_failed_backup(tmp_path):
+    source_dir = tmp_path / "source"
+    dest_dir = tmp_path / "dest"
+    source_dir.mkdir()
+    dest_dir.mkdir()
+
+    config = LocalConfig(source_dir, dest_dir)
+    config.rmtree = Mock()
+    config.file_exists = Mock()
+    config.unlink = Mock()
+    config.file_exists.return_value = True
+
+    with pytest.raises(BackupFailedError):
+        backup(config)
+        assert config.rmtree.called is True
+
+
+@patch("pisync.util.run_rsync", Mock(return_value=1))
+def test_remote_backup_rsync_fails_removes_previous_failed_backup(tmp_path, user_at_localhost):
+    source_dir = tmp_path / "source"
+    dest_dir = tmp_path / "dest"
+    source_dir.mkdir()
+    dest_dir.mkdir()
+
+    config = RemoteConfig(user_at_localhost, source_dir, dest_dir)
+    config.rmtree = Mock()
+    config.file_exists = Mock()
+    config.unlink = Mock()
+    config.file_exists.return_value = True
+
+    with pytest.raises(BackupFailedError):
+        backup(config)
+        assert config.rmtree.called is True
```

### Comparing `pisync-0.0.3/tests/test_local_config.py` & `pisync-0.0.4/tests/test_local_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,94 +1,86 @@
-import pytest
 from pathlib import Path
-from pisync.config import LocalConfig, InvalidPath
-from pisync.util import get_time_stamp
 from typing import Tuple
 
+import pytest
+
+from pisync.config import BackupType, InvalidPathError, LocalConfig
+from pisync.util import get_time_stamp
+
 
 @pytest.fixture
 def home() -> str:
     return str(Path("~/").expanduser())
 
 
 @pytest.fixture
-def tmp() -> str:
-    return "/tmp"
+def tmp(tmp_path) -> str:
+    return tmp_path
 
 
 @pytest.fixture
 def home_tmp_config(home, tmp) -> Tuple[str, str, LocalConfig]:
     return home, tmp, LocalConfig(home, tmp)
 
 
 class TestInitConfig:
     def test_valid_params_no_exceptions(self, home_tmp_config, optionless_arguments):
         home, tmp, config = home_tmp_config
         assert str(config.source_dir) == home
-        assert str(config.destination_dir) == tmp
+        assert str(config.destination_dir) == str(tmp)
         assert str(config.link_dir) == f"{tmp}/latest"
         assert config.exclude_file_patterns is None
         assert config._optionless_rsync_arguments == optionless_arguments
 
-    def test_source_does_not_exist_throws_invalid_path(self):
+    def test_source_does_not_exist_throws_invalid_path(self, tmp):
         source = "/bad/directory/path/here/does/not/exist"
-        dest = "/tmp"
-        with pytest.raises(InvalidPath):
+        dest = tmp
+        with pytest.raises(InvalidPathError):
             _ = LocalConfig(source, dest)
 
     def test_destination_does_not_exist_throws_invalid_path(self):
         source = str(Path("~/").expanduser())
         dest = "/bad/directory/path/here/does/not/exist"
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             _ = LocalConfig(source, dest)
 
 
 class TestGetRsyncCommand:
     def test_no_previous_backup(self, home_tmp_config, optionless_arguments):
         home, tmp, config = home_tmp_config
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=False)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Complete)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
         assert rsync_cmd == ["rsync", *optionless_arguments, home, new_backup_dir]
 
     def test_previous_backup_exists(self, home_tmp_config, optionless_arguments):
         home, tmp, config = home_tmp_config
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=True)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Incremental)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
-        assert rsync_cmd == [
-            "rsync",
-            *optionless_arguments,
-            f"--link-dest={tmp}/latest",
-            home,
-            new_backup_dir
-        ]
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
+        assert rsync_cmd == ["rsync", *optionless_arguments, f"--link-dest={tmp}/latest", home, new_backup_dir]
 
     def test_exclude_patterns(self, home, tmp, optionless_arguments):
-        exclude_file_patterns = [
-            "/exclude/path1",
-            "/exclude/path2",
-            "/exclude/path3/**/*.bak"
-        ]
+        exclude_file_patterns = ["/exclude/path1", "/exclude/path2", "/exclude/path3/**/*.bak"]
         config = LocalConfig(home, tmp, exclude_file_patterns)
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=False)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Complete)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
         assert rsync_cmd == [
             "rsync",
             *optionless_arguments,
-            *map(lambda p: f"--exclude={p}", exclude_file_patterns),
+            *(f"--exclude={p}" for p in exclude_file_patterns),
             home,
-            new_backup_dir
+            new_backup_dir,
         ]
 
 
 class TestPathOperations:
     def test_is_symlink(self, scratch_file_system, home_tmp_config):
         _, _, config = home_tmp_config
         assert config.is_symlink(scratch_file_system / "file1") is False
@@ -156,19 +148,19 @@
         fs = scratch_file_system
 
         # no exception thrown
         config.ensure_dir_exists(fs / "dir1")
 
         # not a dir
         assert (fs / "file1").exists()
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             config.ensure_dir_exists(fs / "file1")
 
         # non existent
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             config.ensure_dir_exists(fs / "dir")
 
     @pytest.mark.skip(reason="Time difference between the two statements sometimes causes fail")
     def test_generate_new_backup_dir_path(self, tmp_path, scratch_file_system):
         config = LocalConfig(scratch_file_system, tmp_path)
         # these two lines should be run within one second of each other
         new_backup_dir = config.generate_new_backup_dir_path()
@@ -180,9 +172,9 @@
         tmp_path,
         scratch_file_system,
     ):
         config = LocalConfig(scratch_file_system, tmp_path)
         time_stamp = get_time_stamp()
         (tmp_path / time_stamp).touch()
 
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             _ = config.generate_new_backup_dir_path()
```

### Comparing `pisync-0.0.3/tests/test_remote_config.py` & `pisync-0.0.4/tests/test_remote_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import getpass
-import pytest
 from pathlib import Path
-from pisync.config import RemoteConfig, InvalidPath
-from pisync.util import get_time_stamp
 from typing import Tuple
 
+import pytest
+
+from pisync.config import BackupType, InvalidPathError, RemoteConfig
+from pisync.util import get_time_stamp
+
 
 @pytest.fixture
 def home() -> str:
     return str(Path("~/").expanduser())
 
 
 @pytest.fixture
-def tmp() -> str:
-    return "/tmp"
+def tmp(tmp_path) -> str:
+    return tmp_path
 
 
 @pytest.fixture
 def user_at_localhost() -> str:
     return f"{getpass.getuser()}@localhost"
 
 
@@ -26,80 +28,71 @@
     return home, tmp, RemoteConfig(user_at_localhost, home, tmp)
 
 
 class TestInitConfig:
     def test_valid_params_no_exceptions(self, home_tmp_config, optionless_arguments):
         home, tmp, config = home_tmp_config
         assert str(config.source_dir) == home
-        assert str(config.destination_dir) == tmp
+        assert str(config.destination_dir) == str(tmp)
         assert str(config.link_dir) == f"{tmp}/latest"
         assert config.exclude_file_patterns is None
         assert config._optionless_rsync_arguments == optionless_arguments
 
-    def test_source_does_not_exist_throws_invalid_path(self, user_at_localhost):
+    def test_source_does_not_exist_throws_invalid_path(self, user_at_localhost, tmp):
         source = "/bad/directory/path/here/does/not/exist"
-        dest = "/tmp"
-        with pytest.raises(InvalidPath):
+        dest = tmp
+        with pytest.raises(InvalidPathError):
             _ = RemoteConfig(user_at_localhost, source, dest)
 
     def test_destination_does_not_exist_throws_invalid_path(self, user_at_localhost):
         source = str(Path("~/").expanduser())
         dest = "/bad/directory/path/here/does/not/exist"
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             _ = RemoteConfig(user_at_localhost, source, dest)
 
 
 class TestGetRsyncCommand:
     def test_no_previous_backup(self, home_tmp_config, optionless_arguments, user_at_localhost):
         home, tmp, config = home_tmp_config
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=False)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Complete)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
-        assert rsync_cmd == [
-            "rsync",
-            *optionless_arguments,
-            home,
-            f"{user_at_localhost}:{new_backup_dir}"
-        ]
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
+        assert rsync_cmd == ["rsync", *optionless_arguments, home, f"{user_at_localhost}:{new_backup_dir}"]
 
     def test_previous_backup_exists(self, home_tmp_config, optionless_arguments, user_at_localhost):
         home, tmp, config = home_tmp_config
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=True)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Incremental)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
         assert rsync_cmd == [
             "rsync",
             *optionless_arguments,
             f"--link-dest={tmp}/latest",
             home,
-            f"{user_at_localhost}:{new_backup_dir}"
+            f"{user_at_localhost}:{new_backup_dir}",
         ]
 
     def test_exclude_patterns(self, home, tmp, optionless_arguments, user_at_localhost):
-        exclude_file_patterns = [
-            "/exclude/path1",
-            "/exclude/path2",
-            "/exclude/path3/**/*.bak"
-        ]
+        exclude_file_patterns = ["/exclude/path1", "/exclude/path2", "/exclude/path3/**/*.bak"]
         config = RemoteConfig(user_at_localhost, home, tmp, exclude_file_patterns)
         new_backup_dir = config.generate_new_backup_dir_path()
-        rsync_cmd = config.get_rsync_command(new_backup_dir, previous_backup_exists=False)
+        rsync_cmd = config.get_rsync_command(new_backup_dir, backup_method=BackupType.Complete)
 
         # For example: /tmp/2023-07-14-17-24-23
-        assert new_backup_dir.startswith("/tmp/")
+        assert new_backup_dir.startswith(str(tmp.parts[0]))
         assert rsync_cmd == [
             "rsync",
             *optionless_arguments,
-            *map(lambda p: f"--exclude={p}", exclude_file_patterns),
+            *(f"--exclude={p}" for p in exclude_file_patterns),
             home,
-            f"{user_at_localhost}:{new_backup_dir}"
+            f"{user_at_localhost}:{new_backup_dir}",
         ]
 
 
 class TestPathOperations:
     def test_is_symlink(self, scratch_file_system, home_tmp_config):
         _, _, config = home_tmp_config
         assert config.is_symlink(scratch_file_system / "file1") is False
@@ -167,34 +160,31 @@
         fs = scratch_file_system
 
         # no exception thrown
         config.ensure_dir_exists(fs / "dir1")
 
         # not a dir
         assert (fs / "file1").exists()
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             config.ensure_dir_exists(fs / "file1")
 
         # non existent
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             config.ensure_dir_exists(fs / "dir")
 
     @pytest.mark.skip(reason="Time difference between the two statements sometimes causes fail")
     def test_generate_new_backup_dir_path(self, tmp_path, scratch_file_system, user_at_localhost):
         config = RemoteConfig(user_at_localhost, scratch_file_system, tmp_path)
         # these two lines should be run within one second of each other
         new_backup_dir = config.generate_new_backup_dir_path()
         time_stamp = get_time_stamp()
         assert new_backup_dir.split("/")[-1] == time_stamp
 
     def test_generate_new_backup_dir_throws_exception_on_overwrite(
-        self,
-        tmp_path,
-        scratch_file_system,
-        user_at_localhost
+        self, tmp_path, scratch_file_system, user_at_localhost
     ):
         config = RemoteConfig(user_at_localhost, scratch_file_system, tmp_path)
         time_stamp = get_time_stamp()
-        (tmp_path / time_stamp).touch()
+        (tmp_path / time_stamp).mkdir()
 
-        with pytest.raises(InvalidPath):
+        with pytest.raises(InvalidPathError):
             _ = config.generate_new_backup_dir_path()
```

### Comparing `pisync-0.0.3/LICENSE` & `pisync-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pisync-0.0.3/README.md` & `pisync-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 The unit/integration tests require password-less login to localhost as the
 "remote" machine.
 
 ```
 ssh-copy-id $USER@localhost
 git clone https://github.com/erietz/pisync
 cd pisync
-pip install -r dev-requirements.txt
+pip install -e .
 make test
 ```
 
 [rsync]: https://github.com/WayneD/rsync
 [python]: https://www.python.org/
 [fabric]: https://github.com/fabric/fabric
 [pi]: https://www.raspberrypi.com/
```

### Comparing `pisync-0.0.3/pyproject.toml` & `pisync-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pisync"
 dynamic = ["version"]
 description = 'Minimal incremental backup script using rsync '
 readme = "README.md"
 requires-python = ">=3.7"
-license = "MIT"
+license = "GPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "erietz", email = "ewrietz@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -56,14 +56,16 @@
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
+  "pytest",
+  "pisync"
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/pisync tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -73,14 +75,20 @@
   "style",
 ]
 all = [
   "style",
   "typing",
 ]
 
+[[tool.mypy.overrides]]
+module = [
+	"fabric"
+]
+ignore_missing_imports = true
+
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py37"
@@ -117,14 +125,16 @@
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  # I do not know how to fix this `subprocess` call: check for execution of untrusted input
+  "S603"
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
@@ -133,14 +143,17 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
+# allow print statement in example script
+"./examples/run_backups.py" = ["T201"]
+
 [tool.coverage.run]
 source_pkgs = ["pisync", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/pisync/__about__.py",
 ]
```

### Comparing `pisync-0.0.3/PKG-INFO` & `pisync-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pisync
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimal incremental backup script using rsync 
 Project-URL: Documentation, https://github.com/erietz/pisync#readme
 Project-URL: Issues, https://github.com/erietz/pisync/issues
 Project-URL: Source, https://github.com/erietz/pisync
 Author-email: erietz <ewrietz@gmail.com>
-License-Expression: MIT
+License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -99,15 +99,15 @@
 The unit/integration tests require password-less login to localhost as the
 "remote" machine.
 
 ```
 ssh-copy-id $USER@localhost
 git clone https://github.com/erietz/pisync
 cd pisync
-pip install -r dev-requirements.txt
+pip install -e .
 make test
 ```
 
 [rsync]: https://github.com/WayneD/rsync
 [python]: https://www.python.org/
 [fabric]: https://github.com/fabric/fabric
 [pi]: https://www.raspberrypi.com/
```

