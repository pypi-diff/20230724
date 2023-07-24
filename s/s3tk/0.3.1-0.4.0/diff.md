# Comparing `tmp/s3tk-0.3.1-py2.py3-none-any.whl.zip` & `tmp/s3tk-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9676 bytes, number of entries: 8
--rw-r--r--  2.0 unx    24777 b- defN 20-Aug-17 21:53 s3tk/__init__.py
+Zip file size: 14268 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    24800 b- defN 23-Jul-24 03:12 s3tk/__init__.py
 -rw-r--r--  2.0 unx     7446 b- defN 20-May-28 06:16 s3tk/checks.py
--rwxr-xr-x  2.0 unx      216 b- defN 20-Aug-17 21:56 s3tk-0.3.1.data/scripts/s3tk
--rw-r--r--  2.0 unx     1073 b- defN 20-Aug-17 21:56 s3tk-0.3.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      361 b- defN 20-Aug-17 21:56 s3tk-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Aug-17 21:56 s3tk-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 20-Aug-17 21:56 s3tk-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      603 b- defN 20-Aug-17 21:56 s3tk-0.3.1.dist-info/RECORD
-8 files, 34591 bytes uncompressed, 8634 bytes compressed:  75.0%
+-rwxr-xr-x  2.0 unx      216 b- defN 23-Jul-24 03:13 s3tk-0.4.0.data/scripts/s3tk
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-24 03:13 s3tk-0.4.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    16059 b- defN 23-Jul-24 03:13 s3tk-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 03:13 s3tk-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 03:13 s3tk-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      605 b- defN 23-Jul-24 03:13 s3tk-0.4.0.dist-info/RECORD
+8 files, 50314 bytes uncompressed, 13226 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: s3tk/__init__.py
 Comment: 
 
 Filename: s3tk/checks.py
 Comment: 
 
-Filename: s3tk-0.3.1.data/scripts/s3tk
+Filename: s3tk-0.4.0.data/scripts/s3tk
 Comment: 
 
-Filename: s3tk-0.3.1.dist-info/LICENSE.txt
+Filename: s3tk-0.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: s3tk-0.3.1.dist-info/METADATA
+Filename: s3tk-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: s3tk-0.3.1.dist-info/WHEEL
+Filename: s3tk-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: s3tk-0.3.1.dist-info/top_level.txt
+Filename: s3tk-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: s3tk-0.3.1.dist-info/RECORD
+Filename: s3tk-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## s3tk/__init__.py

```diff
@@ -1,22 +1,25 @@
-# -*- coding: utf-8 -*-
-
 import sys
 import os.path
 import json
 import fnmatch
 from collections import Counter, OrderedDict
+import warnings
 import boto3
 import botocore
 import click
 from joblib import Parallel, delayed
-from clint.textui import colored, puts, indent
 from .checks import AclCheck, PolicyCheck, PublicAccessCheck, LoggingCheck, VersioningCheck, EncryptionCheck, ObjectLoggingCheck
 
-__version__ = '0.3.1'
+# fix for https://github.com/kennethreitz-archive/clint/issues/185
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    from clint.textui import colored, puts, indent
+
+__version__ = '0.4.0'
 
 canned_acls = [
     {
         'acl': 'private',
         'grants': []
     },
     {
@@ -44,14 +47,15 @@
             {'Grantee': {'Type': 'CanonicalUser', 'DisplayName': 'za-team', 'ID': '6aa5a366c34c1cbe25dc49211496e913e0351eb0e8c37aa3477e40942ec6b97c'}, 'Permission': 'READ'}
         ]
     }
 ]
 
 cached_s3 = None
 
+
 def s3():
     # memoize
     global cached_s3
     if cached_s3 is None:
         cached_s3 = boto3.resource('s3')
     return cached_s3
 
@@ -62,18 +66,15 @@
 
 def abort(message):
     puts(colored.red(message))
     sys.exit(1)
 
 
 def unicode_key(key):
-    if sys.version_info[0] < 3 and isinstance(key, unicode):
-        return key.encode('utf-8')
-    else:
-        return key
+    return key
 
 
 def perform(check):
     check.perform()
 
     with indent(2):
         if check.status == 'passed':
@@ -269,15 +270,15 @@
     if versions:
         object_versions = bucket.object_versions.filter(Prefix=prefix) if prefix else bucket.object_versions.all()
         # delete markers have no size
         return Parallel(n_jobs=24)(delayed(fn)(bucket.name, ov.object_key, ov.id, *args) for ov in object_versions if object_matches(ov.object_key, only, _except) and not ov.is_latest and ov.size is not None)
     else:
         objects = bucket.objects.filter(Prefix=prefix) if prefix else bucket.objects.all()
 
-        if only and not '*' in only:
+        if only and '*' not in only:
             objects = [s3().Object(bucket, only)]
 
         return Parallel(n_jobs=24)(delayed(fn)(bucket.name, os.key, *args) for os in objects if object_matches(os.key, only, _except))
 
 
 def public_statement(bucket):
     return OrderedDict([
@@ -350,15 +351,15 @@
     if policy:
         policy = json.loads(policy, object_pairs_hook=OrderedDict)
 
     return policy
 
 
 def print_dns_bucket(name, buckets, found_buckets):
-    if not name in found_buckets:
+    if name not in found_buckets:
         puts(name)
         with indent(2):
             if name in buckets:
                 puts(colored.green('owned'))
             else:
                 puts(colored.red('not owned'))
 
@@ -427,15 +428,15 @@
 @cli.command()
 @click.argument('buckets', nargs=-1)
 @click.option('--log-bucket', multiple=True, help='Check log bucket(s)')
 @click.option('--log-prefix', help='Check log prefix')
 @click.option('--skip-logging', is_flag=True, help='Skip logging check')
 @click.option('--skip-versioning', is_flag=True, help='Skip versioning check')
 @click.option('--skip-default-encryption', is_flag=True, help='Skip default encryption check')
-@click.option('--default-encryption', is_flag=True) # no op, can't hide from help until click 7 released
+@click.option('--default-encryption', is_flag=True)  # no op, can't hide from help until click 7 released
 @click.option('--object-level-logging', is_flag=True)
 @click.option('--sns-topic', help='Send SNS notification for failures')
 def scan(buckets, log_bucket=None, log_prefix=None, skip_logging=False, skip_versioning=False, skip_default_encryption=False, default_encryption=True, object_level_logging=False, sns_topic=None):
     event_selectors = fetch_event_selectors() if object_level_logging else {}
 
     checks = []
     for bucket in fetch_buckets(buckets):
```

## Comparing `s3tk-0.3.1.dist-info/LICENSE.txt` & `s3tk-0.4.0.dist-info/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2020 Andrew Kane
+Copyright (c) 2017-2023 Andrew Kane
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
```

