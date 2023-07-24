# Comparing `tmp/salure_helpers_ftp-1.5.1.tar.gz` & `tmp/salure_helpers_ftp-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.5.1.tar", last modified: Tue May 30 13:05:06 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.5.2.tar", last modified: Mon Jul 24 14:07:04 2023, max compression
```

## Comparing `salure_helpers_ftp-1.5.1.tar` & `salure_helpers_ftp-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6259 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/setup.py
```

### Comparing `salure_helpers_ftp-1.5.1/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.5.2/salure_helpers/ftp/ftps.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_ftp-1.5.1/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.5.2/salure_helpers/ftp/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from paramiko.client import SSHClient, AutoAddPolicy
 from paramiko.pkey import PKey
+from paramiko import RSAKey
 from paramiko.sftp_attr import SFTPAttributes
 from typing import Union, List
 from salure_helpers.salureconnect import SalureConnect
 from stat import S_ISREG
 
 
 class SFTP(SalureConnect):
@@ -20,15 +21,15 @@
         if self.debug:
             print(credentials)
         self.host = credentials['host']
         self.port = 22 if credentials['port'] is None else credentials['port']
         self.username = credentials['username']
         self.password = credentials['password']
         # untested
-        self.private_key = PKey().from_private_key(open(credentials['private_key_path'], mode='r'), password=credentials['private_key_password']) if credentials['private_key_path'] is not None else None
+        self.private_key = RSAKey.from_private_key(open(credentials['private_key_path'], mode='r'), password=credentials['private_key_password']) if credentials['private_key_path'] is not None else None
         policy = AutoAddPolicy()
         self.client = SSHClient()
         self.client.set_missing_host_key_policy(policy)
 
     def upload_file(self, local_filepath, remote_filepath, confirm=True) -> SFTPAttributes:
         """
         Upload a single file to a remote location. If there is no Private key
```

