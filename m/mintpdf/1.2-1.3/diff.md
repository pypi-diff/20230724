# Comparing `tmp/mintpdf-1.2.tar.gz` & `tmp/mintpdf-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintpdf-1.2.tar", last modified: Sun Jul 23 15:34:17 2023, max compression
+gzip compressed data, was "mintpdf-1.3.tar", last modified: Mon Jul 24 09:05:36 2023, max compression
```

## Comparing `mintpdf-1.2.tar` & `mintpdf-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-23 15:34:17.676036 mintpdf-1.2/
--rw-r--r--   0 greta      (501) staff       (20)    35149 2023-07-23 15:08:42.000000 mintpdf-1.2/LICENSE
--rw-r--r--   0 greta      (501) staff       (20)      109 2023-07-23 15:34:17.675867 mintpdf-1.2/PKG-INFO
--rw-r--r--   0 greta      (501) staff       (20)       36 2023-07-23 15:08:08.000000 mintpdf-1.2/README.md
-drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-23 15:34:17.674668 mintpdf-1.2/mintpdf/
--rw-r--r--   0 greta      (501) staff       (20)       47 2023-07-23 15:31:23.000000 mintpdf-1.2/mintpdf/__init__.py
--rw-r--r--   0 greta      (501) staff       (20)       37 2023-07-23 15:05:20.000000 mintpdf-1.2/mintpdf/pdf2image.py
--rw-r--r--   0 greta      (501) staff       (20)       37 2023-07-23 15:04:35.000000 mintpdf-1.2/mintpdf/pdf2text.py
-drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-23 15:34:17.675617 mintpdf-1.2/mintpdf.egg-info/
--rw-r--r--   0 greta      (501) staff       (20)      109 2023-07-23 15:34:17.000000 mintpdf-1.2/mintpdf.egg-info/PKG-INFO
--rw-r--r--   0 greta      (501) staff       (20)      211 2023-07-23 15:34:17.000000 mintpdf-1.2/mintpdf.egg-info/SOURCES.txt
--rw-r--r--   0 greta      (501) staff       (20)        1 2023-07-23 15:34:17.000000 mintpdf-1.2/mintpdf.egg-info/dependency_links.txt
--rw-r--r--   0 greta      (501) staff       (20)        8 2023-07-23 15:34:17.000000 mintpdf-1.2/mintpdf.egg-info/top_level.txt
--rw-r--r--   0 greta      (501) staff       (20)       38 2023-07-23 15:34:17.676094 mintpdf-1.2/setup.cfg
--rw-r--r--   0 greta      (501) staff       (20)      220 2023-07-23 15:31:23.000000 mintpdf-1.2/setup.py
+drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-24 09:05:36.705757 mintpdf-1.3/
+-rw-r--r--   0 greta      (501) staff       (20)    35149 2023-07-23 15:08:42.000000 mintpdf-1.3/LICENSE
+-rw-r--r--   0 greta      (501) staff       (20)      109 2023-07-24 09:05:36.705580 mintpdf-1.3/PKG-INFO
+-rw-r--r--   0 greta      (501) staff       (20)       36 2023-07-23 15:08:08.000000 mintpdf-1.3/README.md
+drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-24 09:05:36.704424 mintpdf-1.3/mintpdf/
+-rw-r--r--   0 greta      (501) staff       (20)       47 2023-07-24 07:04:12.000000 mintpdf-1.3/mintpdf/__init__.py
+-rw-r--r--   0 greta      (501) staff       (20)       37 2023-07-23 15:05:20.000000 mintpdf-1.3/mintpdf/pdf2image.py
+-rw-r--r--   0 greta      (501) staff       (20)      396 2023-07-24 07:07:58.000000 mintpdf-1.3/mintpdf/pdf2text.py
+drwxr-xr-x   0 greta      (501) staff       (20)        0 2023-07-24 09:05:36.705318 mintpdf-1.3/mintpdf.egg-info/
+-rw-r--r--   0 greta      (501) staff       (20)      109 2023-07-24 09:05:36.000000 mintpdf-1.3/mintpdf.egg-info/PKG-INFO
+-rw-r--r--   0 greta      (501) staff       (20)      211 2023-07-24 09:05:36.000000 mintpdf-1.3/mintpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 greta      (501) staff       (20)        1 2023-07-24 09:05:36.000000 mintpdf-1.3/mintpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 greta      (501) staff       (20)        8 2023-07-24 09:05:36.000000 mintpdf-1.3/mintpdf.egg-info/top_level.txt
+-rw-r--r--   0 greta      (501) staff       (20)       38 2023-07-24 09:05:36.705816 mintpdf-1.3/setup.cfg
+-rw-r--r--   0 greta      (501) staff       (20)      220 2023-07-24 09:05:01.000000 mintpdf-1.3/setup.py
```

### Comparing `mintpdf-1.2/LICENSE` & `mintpdf-1.3/LICENSE`

 * *Files identical despite different names*

