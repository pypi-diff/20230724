# Comparing `tmp/idocker-1.2.0.tar.gz` & `tmp/idocker-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idocker-1.2.0.tar", last modified: Fri Jun 30 03:02:25 2023, max compression
+gzip compressed data, was "idocker-1.2.1.tar", last modified: Mon Jul 24 02:23:17 2023, max compression
```

## Comparing `idocker-1.2.0.tar` & `idocker-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.994943 idocker-1.2.0/
--rw-rw-r--   0 pon       (1001) pon       (1001)     2857 2023-06-30 03:02:24.994943 idocker-1.2.0/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)     2018 2023-06-28 07:08:12.000000 idocker-1.2.0/README.md
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.978943 idocker-1.2.0/idocker/
--rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-06-30 03:01:31.000000 idocker-1.2.0/idocker/__init__.py
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.994943 idocker-1.2.0/idocker/cli/
--rw-rw-r--   0 pon       (1001) pon       (1001)        0 2023-01-31 02:12:48.000000 idocker-1.2.0/idocker/cli/__init__.py
--rw-rw-r--   0 pon       (1001) pon       (1001)     4024 2023-06-30 03:01:24.000000 idocker-1.2.0/idocker/cli/main.py
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.986943 idocker-1.2.0/idocker.egg-info/
--rw-rw-r--   0 pon       (1001) pon       (1001)     2857 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)      280 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/SOURCES.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/dependency_links.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/entry_points.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/requires.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/top_level.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-06-30 03:02:24.994943 idocker-1.2.0/setup.cfg
--rw-rw-r--   0 pon       (1001) pon       (1001)     1305 2023-02-08 10:45:30.000000 idocker-1.2.0/setup.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.115595 idocker-1.2.1/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     1082 2023-07-21 07:30:42.000000 idocker-1.2.1/LICENSE
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 02:23:17.115595 idocker-1.2.1/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4018 2023-07-21 07:39:04.000000 idocker-1.2.1/README.md
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.111595 idocker-1.2.1/idocker/
+-rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-07-24 02:20:33.000000 idocker-1.2.1/idocker/__init__.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.115595 idocker-1.2.1/idocker.egg-info/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)      244 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/entry_points.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/requires.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/top_level.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-07-24 02:23:17.119595 idocker-1.2.1/setup.cfg
+-rw-rw-r--   0 pon       (1001) pon       (1001)     1290 2023-07-07 01:40:26.000000 idocker-1.2.1/setup.py
```

### Comparing `idocker-1.2.0/setup.py` & `idocker-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     maintainer_email='1729303158@qq.com',
     license='MIT License',
     platforms=["all"],
     description="docker cli with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ponponon/idocker",
-    packages=setuptools.find_packages(),
+    packages=['idocker'],
     entry_points={
         'console_scripts': [
             'idocker=idocker.cli.main:cli',
         ]
     },
     install_requires=[
         'docker',
```

