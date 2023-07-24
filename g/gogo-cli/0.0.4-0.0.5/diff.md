# Comparing `tmp/gogo_cli-0.0.4.tar.gz` & `tmp/gogo_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.4.tar", max compression
+gzip compressed data, was "gogo_cli-0.0.5.tar", max compression
```

## Comparing `gogo_cli-0.0.4.tar` & `gogo_cli-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2894 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0       69 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1054 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      473 2023-07-24 08:13:12.193700 gogo_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 08:13:12.193700 gogo_cli-0.0.4/readme.txt
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 gogo_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2894 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1054 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.5/PKG-INFO
```

### Comparing `gogo_cli-0.0.4/LICENSE` & `gogo_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.4/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.0.5/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.4/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.0.5/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.4/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.0.5/gogo_cli/core/utils/__menu__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.4/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.0.5/gogo_cli/core/utils/__player__.py`

 * *Files identical despite different names*

