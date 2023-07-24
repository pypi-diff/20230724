# Comparing `tmp/mtng-0.7.2.tar.gz` & `tmp/mtng-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtng-0.7.2.tar", max compression
+gzip compressed data, was "mtng-0.7.3.tar", max compression
```

## Comparing `mtng-0.7.2.tar` & `mtng-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.2/README.md
--rw-r--r--   0        0        0      820 2023-07-24 07:30:34.130095 mtng-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.2/src/mtng/__init__.py
--rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.2/src/mtng/cli.py
--rw-r--r--   0        0        0     8250 2023-07-12 09:34:45.825269 mtng-0.7.2/src/mtng/collect.py
--rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.2/src/mtng/generate.py
--rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.2/src/mtng/spec.py
--rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.2/src/mtng/template/base.tex
--rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.2/src/mtng/template/item.tex
--rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.2/src/mtng/template/item_context.tex
--rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.2/src/mtng/template/macros.tex
--rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.2/src/mtng/template/main.tex
--rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.2/src/mtng/template/preamble.tex
--rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.2/src/mtng/template/provides.tex
--rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.2/src/mtng/template/repo.tex
--rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.3/README.md
+-rw-r--r--   0        0        0      820 2023-07-24 16:09:02.585109 mtng-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.3/src/mtng/__init__.py
+-rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.3/src/mtng/cli.py
+-rw-r--r--   0        0        0     8344 2023-07-24 14:54:52.633604 mtng-0.7.3/src/mtng/collect.py
+-rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.3/src/mtng/generate.py
+-rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.3/src/mtng/spec.py
+-rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.3/src/mtng/template/base.tex
+-rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.3/src/mtng/template/item.tex
+-rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.3/src/mtng/template/item_context.tex
+-rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.3/src/mtng/template/macros.tex
+-rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.3/src/mtng/template/main.tex
+-rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.3/src/mtng/template/preamble.tex
+-rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.3/src/mtng/template/provides.tex
+-rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.3/src/mtng/template/repo.tex
+-rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.3/PKG-INFO
```

### Comparing `mtng-0.7.2/README.md` & `mtng-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/pyproject.toml` & `mtng-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mtng"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 packages = [
 { include = "mtng", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `mtng-0.7.2/src/mtng/cli.py` & `mtng-0.7.3/src/mtng/cli.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/collect.py` & `mtng-0.7.3/src/mtng/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,28 @@
     updated_at: datetime
     created_at: datetime
     closed_at: Optional[datetime]
 
     is_wip: bool = False
     is_stale: bool = False
 
+    draft: Optional[bool]
+
 
 class Issue(IssueBase):
     pull_request: Optional[Any] = None
 
     @property
     def is_pr(self) -> bool:
         return self.pull_request is not None
 
 
 class PullRequest(IssueBase):
     requested_reviewers: List[User] = pydantic.Field(default_factory=list)
     reviews: List[Review] = pydantic.Field(default_factory=list)
-    draft: bool
 
     @property
     def is_pr(self) -> bool:
         return True
 
 
 cache = diskcache.Cache(appdirs.user_cache_dir("mtng"))
@@ -268,15 +269,17 @@
 
                 data[repo.name]["recent_issues"] = recent_issues
 
         for prk in "open_prs", "merged_prs", "stale", "recent_issues":
             for pr in data[repo.name][prk]:
                 pr.is_wip = repo.wip_label in [l.name for l in pr.labels]
                 if pr.is_pr:
-                    pr.is_wip = pr.is_wip or pr.draft
+                    pr.is_wip = pr.is_wip or (
+                        pr.draft if pr.draft is not None else False
+                    )
                 pr.is_stale = repo.stale_label in [l.name for l in pr.labels]
 
         if repo.needs_discussion_label is not None:
             with Status("Getting items that need discussion"):
                 needs_discussion = await get_open_issues(
                     gh,
                     repo.name,
```

### Comparing `mtng-0.7.2/src/mtng/generate.py` & `mtng-0.7.3/src/mtng/generate.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/spec.py` & `mtng-0.7.3/src/mtng/spec.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/template/macros.tex` & `mtng-0.7.3/src/mtng/template/macros.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/template/main.tex` & `mtng-0.7.3/src/mtng/template/main.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/template/preamble.tex` & `mtng-0.7.3/src/mtng/template/preamble.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/src/mtng/template/repo.tex` & `mtng-0.7.3/src/mtng/template/repo.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.2/PKG-INFO` & `mtng-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtng
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

