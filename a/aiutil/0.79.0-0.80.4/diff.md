# Comparing `tmp/aiutil-0.79.0.tar.gz` & `tmp/aiutil-0.80.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.79.0.tar", max compression
+gzip compressed data, was "aiutil-0.80.4.tar", max compression
```

## Comparing `aiutil-0.79.0.tar` & `aiutil-0.80.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-12 05:21:15.154671 aiutil-0.79.0/LICENSE
--rw-r--r--   0        0        0     1825 2023-06-12 05:21:15.154671 aiutil-0.79.0/README.md
--rw-r--r--   0        0        0       96 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/cv.py
--rw-r--r--   0        0        0     3246 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/dockerhub.py
--rw-r--r--   0        0        0    22905 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     9614 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2337 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/pdf.py
--rw-r--r--   0        0        0    10562 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/shebang.py
--rw-r--r--   0        0        0     4504 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/utils.py
--rw-r--r--   0        0        0     2508 2023-06-12 05:21:15.158671 aiutil-0.79.0/pyproject.toml
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 aiutil-0.79.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-24 01:42:02.110247 aiutil-0.80.4/LICENSE
+-rw-r--r--   0        0        0     1861 2023-07-24 01:42:02.110247 aiutil-0.80.4/README.md
+-rw-r--r--   0        0        0       96 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    23197 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/filesystem.py
+-rw-r--r--   0        0        0       81 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/pdf.py
+-rw-r--r--   0        0        0    10756 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/shebang.py
+-rw-r--r--   0        0        0     4637 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-07-24 01:42:02.110247 aiutil-0.80.4/aiutil/utils.py
+-rw-r--r--   0        0        0     2541 2023-07-24 01:42:02.114246 aiutil-0.80.4/pyproject.toml
+-rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.4/PKG-INFO
```

### Comparing `aiutil-0.79.0/LICENSE` & `aiutil-0.80.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/README.md` & `aiutil-0.80.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# [aiutil](https://github.com/legendu-net/aiutil): Data Science Utils
+# AI/ML Utils  |  [@GitHub](https://github.com/legendu-net/aiutil)  |  [@PyPI](https://pypi.org/project/aiutil/)
 
-This is a Python pacakage that contains misc utils for Data Science.
+This is a Python pacakage that contains misc utils for AI/ML.
 
 1. Misc enhancement of Python's built-in functionalities.
     - string
     - collections
     - pandas DataFrame
     - datetime
 2. Misc other tools
```

### Comparing `aiutil-0.79.0/aiutil/collections.py` & `aiutil-0.80.4/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/cv.py` & `aiutil-0.80.4/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/dataframe.py` & `aiutil-0.80.4/aiutil/dataframe.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/datetime.py` & `aiutil-0.80.4/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/dockerhub.py` & `aiutil-0.80.4/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/filesystem.py` & `aiutil-0.80.4/aiutil/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """Filesystem related util functions.
 """
 from __future__ import annotations
 from typing import Optional, Union, Iterable, Callable
+import itertools
 import os
 import sys
 import re
 import shutil
 import math
 from pathlib import Path
 import subprocess as sp
@@ -55,35 +56,43 @@
     try:
         os.symlink(src, dst, target_is_directory=target_is_directory)
         return True
     except Exception:
         return False
 
 
-def count_path(paths: Iterable[str], ascending=False) -> pd.Series:
+def count_path(
+    paths: Iterable[str],
+    weights: Iterable[int | float] | None = None,
+    ascending: bool | None = False,
+) -> pd.Series:
     """Count frequence of paths and their parent paths.
 
     :param paths: An iterable collection of paths.
     :param ascending: If true, sort paths according to their frequencies in ascending order,
         vice versa.
     :return: A pandas Series with paths as index and frequencies of paths as value.
     """
-    freq = {}
-    for path in paths:
-        _count_path_helper(path, freq)
-    freq = pd.Series(freq, name="count").sort_values(ascending=ascending)
-    return freq
 
+    def _count_path_helper(path: str, weight: int | float, freq: dict) -> None:
+        fields = path.rstrip("/").split("/")[:-1]
+        path = ""
+        for field in fields:
+            path = path + field + "/"
+            freq[path] = freq.get(path, 0) + weight
 
-def _count_path_helper(path: str, freq: dict) -> None:
-    fields = path.rstrip("/").split("/")[:-1]
-    path = ""
-    for field in fields:
-        path = path + field + "/"
-        freq[path] = freq.get(path, 0) + 1
+    freq = {}
+    if weights is None:
+        weights = itertools.repeat(1)
+    for path, weight in zip(paths, weights):
+        _count_path_helper(path, weight, freq)
+    freq = pd.Series(freq, name="count")
+    if ascending is None:
+        return freq
+    return freq.sort_values(ascending=ascending)
 
 
 def zip_subdirs(root: Union[str, Path]) -> None:
     """Compress subdirectories into zip files.
 
     :param root: The root directory whose subdirs are to be zipped.
     """
@@ -395,15 +404,15 @@
 
 def replace_patterns(
     path: Path,
     pattern: Union[str, Iterable[str]],
     repl: Union[str, Iterable[str]],
     regex: bool = True,
 ) -> None:
-    """Update a text file using regular expression substitution.
+    """Update a text file by replacing patterns with specified substitutions.
 
     :param path: A Path object to the file to be updated.
     :param pattern: A (list of) patterns to replace.
     :param repl: A (list of) replacements.
         or a function to map patterns to replacements.
     :param regex: If true, treat patterns as regular expression pattern;
         otherwise, perform exact matches.
@@ -580,15 +589,15 @@
         header = fin.readline().split(delimiter)
         index = []
         columns_full = []
         for idx, field in enumerate(header):
             if field in columns:
                 index.append(idx)
                 columns_full.append(field)
-        with (open(output, "w", encoding="utf-8") if output else sys.stdout) as fout:
+        with open(output, "w", encoding="utf-8") if output else sys.stdout as fout:
             fout.write(delimiter.join(columns_full) + "\n")
             for line in fin:
                 fields = line.split(delimiter)
                 fout.write(delimiter.join([fields[idx] for idx in index]) + "\n")
 
 
 def prune_json(input: Union[str, Path], output: Union[str, Path] = ""):
```

### Comparing `aiutil-0.79.0/aiutil/hadoop/hdfs.py` & `aiutil-0.80.4/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hadoop/kerberos.py` & `aiutil-0.80.4/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hadoop/log.py` & `aiutil-0.80.4/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hadoop/logf.py` & `aiutil-0.80.4/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.80.4/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.80.4/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/hash.py` & `aiutil-0.80.4/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/memory.py` & `aiutil-0.80.4/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/notebook/search.py` & `aiutil-0.80.4/aiutil/notebook/search.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/notebook/util.py` & `aiutil-0.80.4/aiutil/notebook/util.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/pdf.py` & `aiutil-0.80.4/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/poetry.py` & `aiutil-0.80.4/aiutil/poetry.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from typing import Optional, Union, Iterable
 from pathlib import Path
 import os
 import shutil
 import subprocess as sp
 import toml
 from loguru import logger
-import git
 import pathspec
+import dulwich
+from dulwich.contrib.paramiko_vendor import ParamikoSSHVendor
 from .filesystem import replace_patterns
 
 DIST = "dist"
 README = "README.md"
 TOML = "pyproject.toml"
+dulwich.client.get_ssh_vendor = ParamikoSSHVendor
 
 
 def _project_dir() -> Path:
     """Get the root directory of the Poetry project.
 
     :return: The root directory of the Poetry project.
     :raises RuntimeError: Raises RuntimeError if the current directory is not under a Python Poetry project.
@@ -112,58 +114,49 @@
     :param proj_dir: The root directory of the Poetry project.
     """
     if proj_dir is None:
         proj_dir = _project_dir()
     if ver:
         _update_version(ver=ver, proj_dir=proj_dir)
         if commit:
-            repo = git.Repo(proj_dir)
-            repo.git.add(".")
-            repo.index.commit("bump up version")
-            for remote in repo.remotes:
-                remote.push(repo.active_branch)
+            repo = dulwich.repo.Repo(proj_dir)
+            dulwich.porcelain.add(repo=repo)
+            dulwich.porcelain.commit(repo=repo, message="bump up version")
+            dulwich.porcelain.push(repo=repo)
     else:
         print(_project_version(proj_dir))
 
 
-def _get_tag(proj_dir):
-    if proj_dir is None:
-        proj_dir = _project_dir()
-    return "v" + _project_version(proj_dir)
-
-
 def add_tag_release(
-    proj_dir: Union[str, Path, None] = None, tag: str = "", release_branch: str = "main"
+    proj_dir: Union[str, Path, None] = None, tag: str = "", branch_release: str = "main"
 ) -> None:
     """Add a tag to the latest commit on the release branch for releasing.
     The tag is decided based on the current version of the project.
 
     :param proj_dir: The root directory of the Poetry project.
     :param tag: The tag (defaults to the current version of the package) to use.
-    :param release_branch: The branch for releasing.
+    :param branch_release: The branch for releasing.
     :raises ValueError: If the tag to create already exists.
     """
-    repo = git.Repo(proj_dir)
-    current_branch = repo.active_branch
-    # add tag to the release branch
-    repo.git.checkout(release_branch)
-    for remote in repo.remotes:
-        remote.pull(repo.active_branch)
-    tag = tag if tag else _get_tag(proj_dir)
-    try:
-        repo.create_tag(tag)
-    except git.GitCommandError as err:
-        repo.git.checkout(current_branch)
+    if proj_dir is None:
+        proj_dir = _project_dir()
+    tag = tag if tag else ("v" + _project_version(proj_dir))
+    repo = dulwich.repo.Repo(proj_dir)
+    if tag.encode() in dulwich.porcelain.tag_list(repo):
         raise ValueError(
-            f"The tag {tag} already exists! Please merge new changes to the {release_branch} branch first."
-        ) from err
-    for remote in repo.remotes:
-        remote.push(tag)
+            f"The tag {tag} already exists! Please merge new changes to the {branch_release} branch first."
+        )
+    branch_old = dulwich.porcelain.active_branch(repo=repo).decode()
+    # add tag to the release branch
+    dulwich.porcelain.checkout_branch(repo=repo, target=branch_release)
+    dulwich.porcelain.pull(repo=repo, refspecs=branch_release)
+    dulwich.porcelain.tag_create(repo=repo, tag=tag, annotated=True)
+    dulwich.porcelain.push(repo=repo, refspecs=[f"refs/tags/{tag}"])
     # switch back to the old branch
-    repo.git.checkout(current_branch)
+    dulwich.porcelain.checkout_branch(repo=repo, target=branch_old)
 
 
 def format_code(
     commit: bool = False,
     proj_dir: Optional[Path] = None,
     files: Iterable[Union[Path, str]] = (),
 ) -> None:
@@ -184,20 +177,19 @@
     else:
         if proj_dir is None:
             proj_dir = _project_dir()
         cmd += str(proj_dir)
     logger.info("Formatting code using black ...")
     sp.run(cmd, shell=True, check=False, stdout=sp.PIPE)
     if commit:
-        repo = git.Repo(proj_dir)
-        repo.git.add(".")
-        repo.index.commit("format code")
-        for remote in repo.remotes:
-            remote.push(repo.active_branch)
-        print(repo.git.status())
+        repo = dulwich.repo.Repo(proj_dir)
+        dulwich.porcelain.add(repo=repo)
+        dulwich.porcelain.commit(repo=repo, message="format code")
+        dulwich.porcelain.push(repo=repo)
+        print(dulwich.porcelain.status())
 
 
 def _lint_code(proj_dir: Union[Path, None], linter: Union[str, list[str]]):
     funcs = {
         "pylint": _lint_code_pylint,
         "flake8": _lint_code_flake8,
         "pytype": _lint_code_pytype,
```

### Comparing `aiutil-0.79.0/aiutil/pypi.py` & `aiutil-0.80.4/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/shebang.py` & `aiutil-0.80.4/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/shell.py` & `aiutil-0.80.4/aiutil/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,18 +47,23 @@
     :param skip: Indexes of rows to skip.
     :param lines: The output of the shell command.
     :param split_by_header: If true, the headers are splitted by a regular expression
         and the columns are splitted by the right-most position of the headers.
         Otherwise, all lines are splitted by the specified regular expression.
     :return: A pandas DataFrame.
     """
+
+    def _reg_skip(skip, n) -> set[int]:
+        if isinstance(skip, int):
+            skip = [skip]
+        return set(idx % n for idx in skip)
+
     if not lines:
         lines = sp.check_output(cmd, shell=True).decode().strip().split("\n")
-    if isinstance(skip, int):
-        skip = [skip]
+    skip = _reg_skip(skip, len(lines))
     lines = [line for idx, line in enumerate(lines) if idx not in skip]
     if split_by_header:
         return _to_frame_title(split=split, lines=lines)
     return _to_frame_space(split=split, header=header, lines=lines)
 
 
 def _to_frame_space(
```

### Comparing `aiutil-0.79.0/aiutil/sql.py` & `aiutil-0.80.4/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/url.py` & `aiutil-0.80.4/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/aiutil/utils.py` & `aiutil-0.80.4/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.79.0/pyproject.toml` & `aiutil-0.80.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.79.0"
+version = "0.80.4"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
 
@@ -22,15 +22,14 @@
 pathspec = ">=0.8.1"
 dateparser = ">=0.7.1"
 numba = ">=0.53.0rc1.post1"
 pandas = ">=1.2.0"
 ydata-profiling = ">=4.2.0"
 loguru = ">=0.3.2"
 toml = ">=0.10.0"
-GitPython = ">=3.0.0"
 notifiers = ">=1.2.1"
 PyYAML = ">=5.3.1"
 python-magic = ">=0.4.0"
 tqdm = ">=4.59.0"
 pytest = ">=3.0"
 # admin
 psutil = { version = ">=5.7.3", optional = true}
@@ -42,17 +41,18 @@
 docker = { version = ">=4.4.0", optional = true }
 requests = { version = ">=2.20.0", optional = true }
 # pdf
 PyPDF2 = { version = ">=1.26.0", optional = true }
 # jupyter
 nbformat = { version = ">=5.0.7", optional = true }
 nbconvert = { version = ">=5.6.1", optional = true }
-black = "^22.12.0"
+black = {extras = ["jupyter"], version = ">=23.7.0"}
 dulwich = ">=0.20.24"
 scikit-image = ">=0.18.3"
+paramiko = ">=3.2.0"
 
 [tool.poetry.extras]
 cv = ["opencv-python", "pillow"]
 docker = ["docker", "networkx", "requests"]
 pdf = ["PyPDF2"]
 jupyter = ["nbformat", "nbconvert", "black"]
 admin = ["psutil"]
```

### Comparing `aiutil-0.79.0/PKG-INFO` & `aiutil-0.80.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.79.0
+Version: 0.80.4
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
 Requires-Python: >=3.10,<3.12
@@ -14,46 +14,46 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: admin
 Provides-Extra: all
 Provides-Extra: cv
 Provides-Extra: docker
 Provides-Extra: jupyter
 Provides-Extra: pdf
-Requires-Dist: GitPython (>=3.0.0)
 Requires-Dist: PyPDF2 (>=1.26.0) ; extra == "pdf" or extra == "all"
 Requires-Dist: PyYAML (>=5.3.1)
-Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: black[jupyter] (>=23.7.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: dateparser (>=0.7.1)
 Requires-Dist: docker (>=4.4.0) ; extra == "docker" or extra == "all"
 Requires-Dist: dulwich (>=0.20.24)
 Requires-Dist: loguru (>=0.3.2)
 Requires-Dist: nbconvert (>=5.6.1) ; extra == "jupyter" or extra == "all"
 Requires-Dist: nbformat (>=5.0.7) ; extra == "jupyter" or extra == "all"
 Requires-Dist: networkx (>=2.5) ; extra == "docker" or extra == "all"
 Requires-Dist: notifiers (>=1.2.1)
 Requires-Dist: numba (>=0.53.0rc1.post1)
 Requires-Dist: opencv-python (>=4.0.0.0) ; extra == "cv" or extra == "all"
 Requires-Dist: pandas (>=1.2.0)
+Requires-Dist: paramiko (>=3.2.0)
 Requires-Dist: pathspec (>=0.8.1)
 Requires-Dist: pillow (>=7.0.0) ; extra == "cv" or extra == "all"
 Requires-Dist: psutil (>=5.7.3) ; extra == "admin" or extra == "all"
 Requires-Dist: pytest (>=3.0)
 Requires-Dist: python-magic (>=0.4.0)
 Requires-Dist: requests (>=2.20.0) ; extra == "docker" or extra == "all"
 Requires-Dist: scikit-image (>=0.18.3)
 Requires-Dist: sqlparse (>=0.4.1)
 Requires-Dist: toml (>=0.10.0)
 Requires-Dist: tqdm (>=4.59.0)
 Requires-Dist: ydata-profiling (>=4.2.0)
 Project-URL: Repository, https://github.com/legendu-net/aiutil
 Description-Content-Type: text/markdown
 
-# [aiutil](https://github.com/legendu-net/aiutil): Data Science Utils
+# AI/ML Utils  |  [@GitHub](https://github.com/legendu-net/aiutil)  |  [@PyPI](https://pypi.org/project/aiutil/)
 
-This is a Python pacakage that contains misc utils for Data Science.
+This is a Python pacakage that contains misc utils for AI/ML.
 
 1. Misc enhancement of Python's built-in functionalities.
     - string
     - collections
     - pandas DataFrame
     - datetime
 2. Misc other tools
```

