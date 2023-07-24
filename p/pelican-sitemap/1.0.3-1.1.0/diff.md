# Comparing `tmp/pelican_sitemap-1.0.3.tar.gz` & `tmp/pelican_sitemap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_sitemap-1.0.3.tar", max compression
+gzip compressed data, was "pelican_sitemap-1.1.0.tar", max compression
```

## Comparing `pelican_sitemap-1.0.3.tar` & `pelican_sitemap-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3409 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/README.md
--rw-r--r--   0        0        0       37 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/__init__.py
--rw-r--r--   0        0        0     9896 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/sitemap.py
--rw-r--r--   0        0        0      157 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/test_data/article1.md
--rw-r--r--   0        0        0      636 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/test_sitemap.py
--rw-r--r--   0        0        0     2678 2023-07-12 08:41:28.066763 pelican_sitemap-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 pelican_sitemap-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3409 2023-07-24 12:48:42.666008 pelican_sitemap-1.1.0/README.md
+-rw-r--r--   0        0        0       37 2023-07-24 12:48:42.666008 pelican_sitemap-1.1.0/pelican/plugins/sitemap/__init__.py
+-rw-r--r--   0        0        0     7535 2023-07-24 12:48:42.666008 pelican_sitemap-1.1.0/pelican/plugins/sitemap/sitemap.py
+-rw-r--r--   0        0        0      157 2023-07-24 12:48:42.666008 pelican_sitemap-1.1.0/pelican/plugins/sitemap/test_data/article1.md
+-rw-r--r--   0        0        0     1934 2023-07-24 12:48:42.666008 pelican_sitemap-1.1.0/pelican/plugins/sitemap/test_sitemap.py
+-rw-r--r--   0        0        0     2728 2023-07-24 12:48:54.202065 pelican_sitemap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 pelican_sitemap-1.1.0/PKG-INFO
```

### Comparing `pelican_sitemap-1.0.3/README.md` & `pelican_sitemap-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican_sitemap-1.0.3/pyproject.toml` & `pelican_sitemap-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-sitemap"
-version = "1.0.3"
+version = "1.1.0"
 description = "Pelican plugin to generate sitemap in plain-text or XML format"
 authors = ["Pelican Dev Team <authors@getpelican.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "sitemap"]
 repository = "https://github.com/pelican-plugins/sitemap"
 documentation = "https://docs.getpelican.com"
@@ -76,14 +76,15 @@
   "W",   # pycodestyle
   "YTT", # flake8-2020
 ]
 
 ignore = [
   "B010",    # `setattr` with a constant attribute value
   "D100",    # missing docstring in public module
+  "D102",    # missing docstring in public method
   "D104",    # missing docstring in public package
   "D203",    # blank line before class docstring
   "D213",    # multi-line docstring summary should start at the second line
   "PLR0912", # too many branches
   "PLR0913", # too many arguments to function call
   "RET505",  # unnecessary `else` after `return` statement
 ]
```

### Comparing `pelican_sitemap-1.0.3/PKG-INFO` & `pelican_sitemap-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-sitemap
-Version: 1.0.3
+Version: 1.1.0
 Summary: Pelican plugin to generate sitemap in plain-text or XML format
 Home-page: https://github.com/pelican-plugins/sitemap
 License: AGPL-3.0
 Keywords: pelican,plugin,sitemap
 Author: Pelican Dev Team
 Author-email: authors@getpelican.com
 Requires-Python: >=3.8.1,<4.0
```

