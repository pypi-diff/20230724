# Comparing `tmp/trycortex-1.0.6.tar.gz` & `tmp/trycortex-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-1.0.6.tar", max compression
+gzip compressed data, was "trycortex-1.0.7.tar", max compression
```

## Comparing `trycortex-1.0.6.tar` & `trycortex-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.6/README.md
--rw-r--r--   0        0        0      404 2023-07-13 23:19:17.596179 trycortex-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.6/trycortex/__init__.py
--rw-r--r--   0        0        0    12976 2023-07-13 23:17:13.600318 trycortex-1.0.6/trycortex/api.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.6/trycortex/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:53.816915 trycortex-1.0.6/trycortex/cli/callable/__init__.py
--rw-r--r--   0        0        0      204 2023-07-13 23:06:52.759994 trycortex-1.0.6/trycortex/cli/callable/commands.py
--rw-r--r--   0        0        0      308 2023-07-13 23:09:13.654204 trycortex-1.0.6/trycortex/cli/cli.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 trycortex-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.7/README.md
+-rw-r--r--   0        0        0      489 2023-07-24 19:09:04.145004 trycortex-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.7/trycortex/__init__.py
+-rw-r--r--   0        0        0    12976 2023-07-19 20:20:29.647945 trycortex-1.0.7/trycortex/api.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.7/trycortex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 22:58:20.969482 trycortex-1.0.7/trycortex/cli/callable/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-17 18:57:14.549510 trycortex-1.0.7/trycortex/cli/callable/callable_config.py
+-rw-r--r--   0        0        0     6858 2023-07-24 18:49:55.816281 trycortex-1.0.7/trycortex/cli/callable/commands.py
+-rw-r--r--   0        0        0      308 2023-07-13 23:09:13.654204 trycortex-1.0.7/trycortex/cli/cli.py
+-rw-r--r--   0        0        0     1522 2023-07-15 00:34:23.304330 trycortex-1.0.7/trycortex/cli/utils.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 trycortex-1.0.7/PKG-INFO
```

### Comparing `trycortex-1.0.6/trycortex/api.py` & `trycortex-1.0.7/trycortex/api.py`

 * *Files identical despite different names*

