# Comparing `tmp/parse-changelog-1.0.2.tar.gz` & `tmp/parse-changelog-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse-changelog-1.0.2.tar", last modified: Thu Dec  8 22:59:40 2022, max compression
+gzip compressed data, was "parse-changelog-1.0.3.tar", last modified: Mon Jul 24 21:42:33 2023, max compression
```

## Comparing `parse-changelog-1.0.2.tar` & `parse-changelog-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:40.314078 parse-changelog-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-08 22:59:29.000000 parse-changelog-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2022-12-08 22:59:40.314078 parse-changelog-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2022-12-08 22:59:29.000000 parse-changelog-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:40.314078 parse-changelog-1.0.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2022-12-08 22:59:29.000000 parse-changelog-1.0.2/bin/parse-changelog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:40.314078 parse-changelog-1.0.2/parse_changelog/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-08 22:59:29.000000 parse-changelog-1.0.2/parse_changelog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:40.314078 parse-changelog-1.0.2/parse_changelog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2022-12-08 22:59:40.000000 parse-changelog-1.0.2/parse_changelog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-08 22:59:40.000000 parse-changelog-1.0.2/parse_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 22:59:40.000000 parse-changelog-1.0.2/parse_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-08 22:59:40.000000 parse-changelog-1.0.2/parse_changelog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 22:59:40.318078 parse-changelog-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-12-08 22:59:29.000000 parse-changelog-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:42:33.796051 parse-changelog-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 21:42:20.000000 parse-changelog-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-24 21:42:33.796051 parse-changelog-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-24 21:42:20.000000 parse-changelog-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:42:33.792051 parse-changelog-1.0.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2023-07-24 21:42:20.000000 parse-changelog-1.0.3/bin/parse-changelog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:42:33.792051 parse-changelog-1.0.3/parse_changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 21:42:20.000000 parse-changelog-1.0.3/parse_changelog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:42:33.796051 parse-changelog-1.0.3/parse_changelog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-24 21:42:33.000000 parse-changelog-1.0.3/parse_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 21:42:33.000000 parse-changelog-1.0.3/parse_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:42:33.000000 parse-changelog-1.0.3/parse_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 21:42:33.000000 parse-changelog-1.0.3/parse_changelog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:42:33.796051 parse-changelog-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 21:42:20.000000 parse-changelog-1.0.3/setup.py
```

### Comparing `parse-changelog-1.0.2/LICENSE` & `parse-changelog-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parse-changelog-1.0.2/PKG-INFO` & `parse-changelog-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-changelog
-Version: 1.0.2
+Version: 1.0.3
 Summary: A very simplistic changelog parser/updater
 Home-page: https://github.com/cseelye/parse-changelog
 Author: Carl Seelye
 Author-email: cseelye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `parse-changelog-1.0.2/README.md` & `parse-changelog-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `parse-changelog-1.0.2/bin/parse-changelog` & `parse-changelog-1.0.3/bin/parse-changelog`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 current_release = title
                 current_content = []
                 if title.lower() == "[unreleased]": # Special case for Unreleased section
                     version = "prerelease"
                     rel_date = "unreleased"
                 else:
                     # Parse version and release date from the section title
-                    m =re.match(r"\[(\d+\.\d+\.\d+)\[-\.+0-9a-zA-Z]*]\s+-\s+(\d{4}-\d{2}-\d{2})", title)
+                    m =re.match(r"\[(\d+\.\d+\.\d+)[-\.+0-9a-zA-Z]*\]\s+-\s+(\d{4}-\d{2}-\d{2})", title)
                     if m:
                         version = m.group(1)
                         rel_date = m.group(2)
                     else:
                         version = "unknown"
                         rel_date = "unknown"
```

### Comparing `parse-changelog-1.0.2/parse_changelog.egg-info/PKG-INFO` & `parse-changelog-1.0.3/parse_changelog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-changelog
-Version: 1.0.2
+Version: 1.0.3
 Summary: A very simplistic changelog parser/updater
 Home-page: https://github.com/cseelye/parse-changelog
 Author: Carl Seelye
 Author-email: cseelye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `parse-changelog-1.0.2/setup.py` & `parse-changelog-1.0.3/setup.py`

 * *Files identical despite different names*

