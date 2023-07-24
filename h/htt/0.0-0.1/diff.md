# Comparing `tmp/htt-0.0.tar.gz` & `tmp/htt-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htt-0.0.tar", max compression
+gzip compressed data, was "htt-0.1.tar", max compression
```

## Comparing `htt-0.0.tar` & `htt-0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.0/htt/__init__.py
--rw-r--r--   0        0        0      254 2023-07-20 03:57:22.765339 htt-0.0/pyproject.toml
--rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 htt-0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.1/README.md
+-rw-r--r--   0        0        0       56 2023-07-24 03:20:03.214685 htt-0.1/htt/__init__.py
+-rw-r--r--   0        0        0     6985 2023-07-24 03:22:22.659792 htt-0.1/htt/app_utils.py
+-rw-r--r--   0        0        0      306 2023-07-24 03:24:40.600954 htt-0.1/pyproject.toml
+-rw-r--r--   0        0        0      366 1970-01-01 00:00:00.000000 htt-0.1/PKG-INFO
```

