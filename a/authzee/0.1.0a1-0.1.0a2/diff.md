# Comparing `tmp/authzee-0.1.0a1.tar.gz` & `tmp/authzee-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authzee-0.1.0a1.tar", last modified: Tue Jul  4 01:17:17 2023, max compression
+gzip compressed data, was "authzee-0.1.0a2.tar", last modified: Mon Jul 24 04:17:17 2023, max compression
```

## Comparing `authzee-0.1.0a1.tar` & `authzee-0.1.0a2.tar`

### file list

```diff
@@ -1,15 +1,39 @@
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-04 01:17:17.643887 authzee-0.1.0a1/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      503 2023-03-01 03:13:42.000000 authzee-0.1.0a1/CHANGELOG.md
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       39 2023-03-01 03:21:06.000000 authzee-0.1.0a1/MANIFEST.in
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1733 2023-07-04 01:17:17.643887 authzee-0.1.0a1/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2021-04-26 04:13:47.000000 authzee-0.1.0a1/pyproject.toml
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1475 2023-07-04 01:17:17.643887 authzee-0.1.0a1/setup.cfg
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-04 01:17:17.639886 authzee-0.1.0a1/src/
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-04 01:17:17.639886 authzee-0.1.0a1/src/authzee/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      113 2023-07-04 00:53:22.000000 authzee-0.1.0a1/src/authzee/__init__.py
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-04 01:17:17.643887 authzee-0.1.0a1/src/authzee.egg-info/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1733 2023-07-04 01:17:17.000000 authzee-0.1.0a1/src/authzee.egg-info/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      247 2023-07-04 01:17:17.000000 authzee-0.1.0a1/src/authzee.egg-info/SOURCES.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2023-07-04 01:17:17.000000 authzee-0.1.0a1/src/authzee.egg-info/dependency_links.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      141 2023-07-04 01:17:17.000000 authzee-0.1.0a1/src/authzee.egg-info/requires.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        8 2023-07-04 01:17:17.000000 authzee-0.1.0a1/src/authzee.egg-info/top_level.txt
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.752862 authzee-0.1.0a2/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      638 2023-07-24 04:05:20.000000 authzee-0.1.0a2/CHANGELOG.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       39 2023-03-01 03:21:06.000000 authzee-0.1.0a2/MANIFEST.in
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    25829 2023-07-24 04:17:17.752862 authzee-0.1.0a2/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    23976 2023-07-24 04:05:00.000000 authzee-0.1.0a2/README.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2021-04-26 04:13:47.000000 authzee-0.1.0a2/pyproject.toml
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1473 2023-07-24 04:17:17.752862 authzee-0.1.0a2/setup.cfg
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.744862 authzee-0.1.0a2/src/
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.748862 authzee-0.1.0a2/src/authzee/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      660 2023-07-24 04:04:08.000000 authzee-0.1.0a2/src/authzee/__init__.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    59152 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/authzee.py
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.748862 authzee-0.1.0a2/src/authzee/compute/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      370 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/__init__.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    12527 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/compute_backend.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     2889 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/general.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     6260 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/main_process_compute.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    23134 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/multiprocess_compute.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    23234 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/compute/threaded_compute.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1190 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/exceptions.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      808 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/grant.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       88 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/grant_effect.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     2714 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/grant_iter.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      213 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/grants_page.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     3767 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/jmespath_custom_functions.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       56 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/logging_config.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      279 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/resource_action.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1436 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/resource_authz.py
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.752862 authzee-0.1.0a2/src/authzee/storage/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      420 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/storage/__init__.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     2821 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/storage/memory_storage.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    13547 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/storage/sql_storage.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     2653 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/storage/sql_storage_models.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    10108 2023-07-24 03:49:35.000000 authzee-0.1.0a2/src/authzee/storage/storage_backend.py
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-07-24 04:17:17.748862 authzee-0.1.0a2/src/authzee.egg-info/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    25829 2023-07-24 04:17:17.000000 authzee-0.1.0a2/src/authzee.egg-info/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      956 2023-07-24 04:17:17.000000 authzee-0.1.0a2/src/authzee.egg-info/SOURCES.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2023-07-24 04:17:17.000000 authzee-0.1.0a2/src/authzee.egg-info/dependency_links.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      139 2023-07-24 04:17:17.000000 authzee-0.1.0a2/src/authzee.egg-info/requires.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        8 2023-07-24 04:17:17.000000 authzee-0.1.0a2/src/authzee.egg-info/top_level.txt
```

### Comparing `authzee-0.1.0a1/setup.cfg` & `authzee-0.1.0a2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 version = attr: authzee.__version__
 description = Authorization framework that uses a querying grant and revoke system.
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 author = Brandon Temple Paul
 author_email = btemplepgit@gmail.com
 url = https://github.com/btemplep/authzee
+project_urls = 
+	Repository = https://github.com/btemplep/authzee
 classifiers = 
 	Development Status :: 3 - Alpha
-	License :: OSI Approved :: Apache Software License
+	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: POSIX :: Linux
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Internet
-license = Apache License 2.0
+license = MIT
 license_files = 
 	License
 keywords = 
 	auth
 	authz
 	authorization
 	framework
@@ -46,15 +47,15 @@
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 sql = 
-	SQLAlchemy >= 2.0.0
+	SQLAlchemy ~= 2.0
 all = authzee[sql]
 dev = 
 	build
 	coverage
 	nox
 	piccolo-theme
 	pytest
```

