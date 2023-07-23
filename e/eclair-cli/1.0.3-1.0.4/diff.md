# Comparing `tmp/eclair-cli-1.0.3.tar.gz` & `tmp/eclair-cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclair-cli-1.0.3.tar", last modified: Sat Jul 22 13:47:00 2023, max compression
+gzip compressed data, was "eclair-cli-1.0.4.tar", last modified: Sun Jul 23 22:43:26 2023, max compression
```

## Comparing `eclair-cli-1.0.3.tar` & `eclair-cli-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:47:00.843720 eclair-cli-1.0.3/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2813 2023-07-22 13:47:00.843586 eclair-cli-1.0.3/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2537 2023-07-22 11:27:21.000000 eclair-cli-1.0.3/README.md
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:47:00.842558 eclair-cli-1.0.3/eclair_cli.egg-info/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2813 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      333 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/entry_points.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/requires.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-22 13:47:00.000000 eclair-cli-1.0.3/eclair_cli.egg-info/top_level.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-22 13:47:00.843761 eclair-cli-1.0.3/setup.cfg
--rw-r--r--   0 abhinavmir   (501) staff       (20)      756 2023-07-22 13:46:59.000000 eclair-cli-1.0.3/setup.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:47:00.843386 eclair-cli-1.0.3/src/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.3/src/ABI_class.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.3/src/__init__.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.3/src/get_all_files.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)     3555 2023-07-22 13:37:11.000000 eclair-cli-1.0.3/src/main.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.3/src/sol_to_json.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.3/src/templating_logic.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.951424 eclair-cli-1.0.4/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6405 2023-07-23 22:43:26.951284 eclair-cli-1.0.4/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6129 2023-07-23 22:43:06.000000 eclair-cli-1.0.4/README.md
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.949609 eclair-cli-1.0.4/eclair_cli.egg-info/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6405 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      333 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/entry_points.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/requires.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/top_level.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-23 22:43:26.951465 eclair-cli-1.0.4/setup.cfg
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      756 2023-07-23 22:43:23.000000 eclair-cli-1.0.4/setup.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.950957 eclair-cli-1.0.4/src/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.4/src/ABI_class.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.4/src/__init__.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.4/src/get_all_files.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     3555 2023-07-22 13:37:11.000000 eclair-cli-1.0.4/src/main.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.4/src/sol_to_json.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.4/src/templating_logic.py
```

### Comparing `eclair-cli-1.0.3/setup.py` & `eclair-cli-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='eclair-cli',
-    version='1.0.3',
+    version='1.0.4',
     author='August Radjoe',
     author_email='atg271@gmail.com',
     description='A tool to create library wrappers for Blockchain Business Logic code.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['src'],
     entry_points={
```

### Comparing `eclair-cli-1.0.3/src/ABI_class.py` & `eclair-cli-1.0.4/src/ABI_class.py`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.3/src/main.py` & `eclair-cli-1.0.4/src/main.py`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.3/src/templating_logic.py` & `eclair-cli-1.0.4/src/templating_logic.py`

 * *Files identical despite different names*

