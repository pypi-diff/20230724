# Comparing `tmp/discord_json_database-0.1.0.tar.gz` & `tmp/discord-json-database-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_json_database-0.1.0.tar", last modified: Mon Jul 24 05:30:45 2023, max compression
+gzip compressed data, was "discord-json-database-0.1.1.tar", last modified: Mon Jul 24 06:05:16 2023, max compression
```

## Comparing `discord_json_database-0.1.0.tar` & `discord-json-database-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 05:30:45.395886 discord_json_database-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-07-23 22:51:58.000000 discord_json_database-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      425 2023-07-24 05:30:45.391472 discord_json_database-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2023-07-24 05:25:24.000000 discord_json_database-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 05:30:45.391472 discord_json_database-0.1.0/discord_json_database.egg-info/
--rw-rw-rw-   0        0        0      425 2023-07-24 05:30:45.000000 discord_json_database-0.1.0/discord_json_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-07-24 05:30:45.000000 discord_json_database-0.1.0/discord_json_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 05:30:45.000000 discord_json_database-0.1.0/discord_json_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 05:30:45.000000 discord_json_database-0.1.0/discord_json_database.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 05:30:45.395886 discord_json_database-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      544 2023-07-24 05:30:40.000000 discord_json_database-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:05:16.378506 discord-json-database-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-23 22:51:58.000000 discord-json-database-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      425 2023-07-24 06:05:16.376937 discord-json-database-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2023-07-24 05:25:24.000000 discord-json-database-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 06:05:16.352153 discord-json-database-0.1.1/discord_json_database/
+-rw-rw-rw-   0        0        0       30 2023-07-24 05:22:12.000000 discord-json-database-0.1.1/discord_json_database/__init__.py
+-rw-rw-rw-   0        0        0     3623 2023-07-24 04:57:50.000000 discord-json-database-0.1.1/discord_json_database/data.py
+-rw-rw-rw-   0        0        0     1554 2023-07-24 04:55:53.000000 discord-json-database-0.1.1/discord_json_database/database.py
+-rw-rw-rw-   0        0        0      330 2023-07-24 04:29:27.000000 discord-json-database-0.1.1/discord_json_database/error_tests.py
+-rw-rw-rw-   0        0        0     1475 2023-07-24 04:29:35.000000 discord-json-database-0.1.1/discord_json_database/errors.py
+-rw-rw-rw-   0        0        0      780 2023-07-24 04:58:21.000000 discord-json-database-0.1.1/discord_json_database/file_operations.py
+-rw-rw-rw-   0        0        0     3603 2023-07-24 04:37:13.000000 discord-json-database-0.1.1/discord_json_database/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:05:16.374857 discord-json-database-0.1.1/discord_json_database.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-07-24 06:05:16.000000 discord-json-database-0.1.1/discord_json_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-07-24 06:05:16.000000 discord-json-database-0.1.1/discord_json_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:05:16.000000 discord-json-database-0.1.1/discord_json_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 06:05:16.000000 discord-json-database-0.1.1/discord_json_database.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:05:16.378506 discord-json-database-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-07-24 06:05:07.000000 discord-json-database-0.1.1/setup.py
```

### Comparing `discord_json_database-0.1.0/LICENSE` & `discord-json-database-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_json_database-0.1.0/README.md` & `discord-json-database-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discord_json_database-0.1.0/setup.py` & `discord-json-database-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='discord_json_database',
-    version='0.1.0',
+    name='discord-json-database',
+    version='0.1.1',
     description='Easily manage a JSON database for a Discord bot',
     long_description='Quickly create a powerful json database for any application (although intended for Discord Bots.) Easily create database structures, and store data for thousands of members and servers. Code design encourages good database practises and SQL databases.',
     author='Cypress4382',
-    packages=find_packages(),
+    packages=['discord_json_database'],
     install_requires=[],
 )
```

