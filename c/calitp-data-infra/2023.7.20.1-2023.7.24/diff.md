# Comparing `tmp/calitp_data_infra-2023.7.20.1.tar.gz` & `tmp/calitp_data_infra-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2023.7.20.1.tar", max compression
+gzip compressed data, was "calitp_data_infra-2023.7.24.tar", max compression
```

## Comparing `calitp_data_infra-2023.7.20.1.tar` & `calitp_data_infra-2023.7.24.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-02-17 19:00:01.037081 calitp_data_infra-2023.7.20.1/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1200 2023-07-20 15:15:44.646986 calitp_data_infra-2023.7.20.1/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    26823 2023-07-20 17:16:14.968392 calitp_data_infra-2023.7.20.1/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      782 2023-07-20 17:13:01.037681 calitp_data_infra-2023.7.20.1/pyproject.toml
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 calitp_data_infra-2023.7.20.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 20:11:15.386888 calitp_data_infra-2023.7.24/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1200 2023-07-21 20:11:15.945810 calitp_data_infra-2023.7.24/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    25564 2023-07-24 20:02:57.924371 calitp_data_infra-2023.7.24/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      773 2023-07-24 20:07:34.347681 calitp_data_infra-2023.7.24/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 calitp_data_infra-2023.7.24/PKG-INFO
```

### Comparing `calitp_data_infra-2023.7.20.1/calitp_data_infra/auth.py` & `calitp_data_infra-2023.7.24/calitp_data_infra/auth.py`

 * *Files identical despite different names*

### Comparing `calitp_data_infra-2023.7.20.1/calitp_data_infra/storage.py` & `calitp_data_infra-2023.7.24/calitp_data_infra/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     get_type_hints,
 )
 
 import backoff
 import gcsfs  # type: ignore
 import humanize
 import pendulum
-from calitp_data.config import get_bucket, require_pipeline  # type: ignore
-from calitp_data.storage import get_fs  # type: ignore
 from google.cloud import storage  # type: ignore
 from pydantic import (
     BaseModel,
     ConstrainedStr,
     Extra,
     Field,
     HttpUrl,
@@ -44,71 +42,21 @@
 from requests import Request, Session
 from typing_extensions import Annotated, Literal
 
 JSONL_EXTENSION = ".jsonl"
 JSONL_GZIP_EXTENSION = f"{JSONL_EXTENSION}.gz"
 
 
-@require_pipeline("save_to_gcfs")
-def save_to_gcfs(
-    src_path,
-    dst_path,
-    gcs_project="cal-itp-data-infra",
-    bucket=None,
-    use_pipe=False,
-    verbose=True,
-    **kwargs,
-):
-    """Convenience function for saving files from disk to google cloud storage.
-
-    Arguments:
-        src_path: path to file being saved.
-        dst_path: path to bucket subdirectory (e.g. "path/to/dir").
-    """
-
-    bucket = get_bucket() if bucket is None else bucket
-
-    full_dst_path = bucket + "/" + str(dst_path)
-
-    fs = get_fs(gcs_project)
-
-    if verbose:
-        print("Saving to:", full_dst_path)
-
-    if not use_pipe:
-        fs.put(str(src_path), full_dst_path, **kwargs)
-    else:
-        fs.pipe(str(full_dst_path), src_path, **kwargs)
-
-    return full_dst_path
-
-
-def read_gcfs(src_path, dst_path=None, gcs_project="", bucket=None, verbose=True):
-    """
-    Arguments:
-        src_path: path to file being read from google cloud.
-        dst_path: optional path to save file directly on disk.
-    """
-
-    bucket = get_bucket() if bucket is None else bucket
-
-    fs = get_fs(gcs_project)
-
-    full_src_path = bucket + "/" + str(src_path)
-
-    if verbose:
-        print(f"Reading file: {full_src_path}")
-
-    if dst_path is None:
-        return fs.open(full_src_path)
+def get_fs(gcs_project="", **kwargs):
+    if os.environ.get("CALITP_AUTH") == "cloud":
+        return gcsfs.GCSFileSystem(project=gcs_project, token="cloud", **kwargs)
     else:
-        # TODO: in this case, dump directly to disk, rather opening
-        raise NotImplementedError()
-
-    return full_src_path
+        return gcsfs.GCSFileSystem(
+            project=gcs_project, token="google_default", **kwargs
+        )
 
 
 def make_name_bq_safe(name: str):
     """Replace non-word characters.
     See: https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#identifiers.
     """
     return str.lower(re.sub("[^\w]", "_", name))  # noqa: W605
```

### Comparing `calitp_data_infra-2023.7.20.1/pyproject.toml` & `calitp_data_infra-2023.7.24/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "calitp-data-infra"
-version = "2023.7.20.1"
+version = "2023.7.24"
 description = "Shared code for developing data pipelines that process Cal-ITP data."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 # Some of these are pinned oddly to play nicely with Composer
 pydantic = "~1.9"
 tqdm = "^4.64.1"
 pendulum = "^2.1.2"
 humanize = "^4.6.0"
 backoff = "^2.2.1"
 google-api-core = ">=1.31.4"
 typing-extensions = ">=3.10.0.2"
-calitp-data = "2023.2.15.1"
 google-cloud-secret-manager = "~1.0.0"
+gcsfs = "!=2022.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.0"
 hypothesis = "^6.68.0"
 types-requests = "^2.31.0.1"
```

### Comparing `calitp_data_infra-2023.7.20.1/PKG-INFO` & `calitp_data_infra-2023.7.24/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2023.7.20.1
+Version: 2023.7.24
 Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: calitp-data (==2023.2.15.1)
+Requires-Dist: gcsfs (!=2022.7.1)
 Requires-Dist: google-api-core (>=1.31.4)
 Requires-Dist: google-cloud-secret-manager (>=1.0.0,<1.1.0)
 Requires-Dist: humanize (>=4.6.0,<5.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.9,<1.10)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typing-extensions (>=3.10.0.2)
```

