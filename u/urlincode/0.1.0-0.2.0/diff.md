# Comparing `tmp/urlincode-0.1.0.tar.gz` & `tmp/urlincode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode-0.1.0.tar", last modified: Sun Jul 23 12:58:38 2023, max compression
+gzip compressed data, was "urlincode-0.2.0.tar", last modified: Mon Jul 24 07:49:58 2023, max compression
```

## Comparing `urlincode-0.1.0.tar` & `urlincode-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-23 12:58:38.615862 urlincode-0.1.0/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      183 2023-07-23 12:58:38.615862 urlincode-0.1.0/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-07-23 12:58:38.615862 urlincode-0.1.0/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      148 2023-07-23 12:55:01.000000 urlincode-0.1.0/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-23 12:58:38.615862 urlincode-0.1.0/urlincode.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      183 2023-07-23 12:58:38.000000 urlincode-0.1.0/urlincode.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-07-23 12:58:38.000000 urlincode-0.1.0/urlincode.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-23 12:58:38.000000 urlincode-0.1.0/urlincode.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-23 12:58:38.000000 urlincode-0.1.0/urlincode.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-24 07:49:58.240877 urlincode-0.2.0/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      222 2023-07-24 07:49:58.240877 urlincode-0.2.0/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-07-24 07:49:58.240877 urlincode-0.2.0/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      342 2023-07-24 07:40:46.000000 urlincode-0.2.0/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-24 07:49:58.240877 urlincode-0.2.0/urlincode.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      222 2023-07-24 07:49:58.000000 urlincode-0.2.0/urlincode.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-07-24 07:49:58.000000 urlincode-0.2.0/urlincode.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-24 07:49:58.000000 urlincode-0.2.0/urlincode.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-24 07:49:58.000000 urlincode-0.2.0/urlincode.egg-info/top_level.txt
```

