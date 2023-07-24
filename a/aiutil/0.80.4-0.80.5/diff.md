# Comparing `tmp/aiutil-0.80.4.tar.gz` & `tmp/aiutil-0.80.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.80.4.tar", max compression
+gzip compressed data, was "aiutil-0.80.5.tar", max compression
```

## Comparing `aiutil-0.80.4.tar` & `aiutil-0.80.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-07-24 01:42:02.110247 aiutil-0.80.4/LICENSE
--rw-r--r--   0        0        0     1861 2023-07-24 01:42:02.110247 aiutil-0.80.4/README.md
--rw-r--r--   0        0        0       96 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/cv.py
--rw-r--r--   0        0        0     3246 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/dockerhub.py
--rw-r--r--   0        0        0    23197 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     9614 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2337 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/pdf.py
--rw-r--r--   0        0        0    10756 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/shebang.py
--rw-r--r--   0        0        0     4637 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/utils.py
--rw-r--r--   0        0        0     2541 2023-07-24 01:42:02.114246 aiutil-0.80.4/pyproject.toml
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-24 02:00:36.847561 aiutil-0.80.5/LICENSE
+-rw-r--r--   0        0        0     1861 2023-07-24 02:00:36.847561 aiutil-0.80.5/README.md
+-rw-r--r--   0        0        0       96 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    23197 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/filesystem.py
+-rw-r--r--   0        0        0       81 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/pdf.py
+-rw-r--r--   0        0        0    10890 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/shebang.py
+-rw-r--r--   0        0        0     4637 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/utils.py
+-rw-r--r--   0        0        0     2541 2023-07-24 02:00:36.855561 aiutil-0.80.5/pyproject.toml
+-rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.5/PKG-INFO
```

### Comparing `aiutil-0.80.4/LICENSE` & `aiutil-0.80.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/README.md` & `aiutil-0.80.5/README.md`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/collections.py` & `aiutil-0.80.5/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/cv.py` & `aiutil-0.80.5/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/dataframe.py` & `aiutil-0.80.5/aiutil/dataframe.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/datetime.py` & `aiutil-0.80.5/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/dockerhub.py` & `aiutil-0.80.5/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/filesystem.py` & `aiutil-0.80.5/aiutil/filesystem.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/hdfs.py` & `aiutil-0.80.5/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/kerberos.py` & `aiutil-0.80.5/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/log.py` & `aiutil-0.80.5/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/logf.py` & `aiutil-0.80.5/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.80.5/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.80.5/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/hash.py` & `aiutil-0.80.5/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/memory.py` & `aiutil-0.80.5/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/notebook/search.py` & `aiutil-0.80.5/aiutil/notebook/search.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/notebook/util.py` & `aiutil-0.80.5/aiutil/notebook/util.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/pdf.py` & `aiutil-0.80.5/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/poetry.py` & `aiutil-0.80.5/aiutil/poetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,17 @@
             f"The tag {tag} already exists! Please merge new changes to the {branch_release} branch first."
         )
     branch_old = dulwich.porcelain.active_branch(repo=repo).decode()
     # add tag to the release branch
     dulwich.porcelain.checkout_branch(repo=repo, target=branch_release)
     dulwich.porcelain.pull(repo=repo, refspecs=branch_release)
     dulwich.porcelain.tag_create(repo=repo, tag=tag, annotated=True)
-    dulwich.porcelain.push(repo=repo, refspecs=[f"refs/tags/{tag}"])
+    remote = dulwich.porcelain.get_branch_remote(repo=repo).decode()
+    sp.run(f"git push {remote} {tag}", shell=True, check=True)
+    # dulwich.porcelain.push(repo=repo, refspecs=[f"refs/tags/{tag}"])
     # switch back to the old branch
     dulwich.porcelain.checkout_branch(repo=repo, target=branch_old)
 
 
 def format_code(
     commit: bool = False,
     proj_dir: Optional[Path] = None,
```

### Comparing `aiutil-0.80.4/aiutil/pypi.py` & `aiutil-0.80.5/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/shebang.py` & `aiutil-0.80.5/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/shell.py` & `aiutil-0.80.5/aiutil/shell.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/sql.py` & `aiutil-0.80.5/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/url.py` & `aiutil-0.80.5/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/aiutil/utils.py` & `aiutil-0.80.5/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.4/pyproject.toml` & `aiutil-0.80.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.80.4"
+version = "0.80.5"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
```

### Comparing `aiutil-0.80.4/PKG-INFO` & `aiutil-0.80.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.80.4
+Version: 0.80.5
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
 Requires-Python: >=3.10,<3.12
```

