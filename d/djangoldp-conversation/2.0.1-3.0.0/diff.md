# Comparing `tmp/djangoldp_conversation-2.0.1.tar.gz` & `tmp/djangoldp_conversation-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_conversation-2.0.1.tar", last modified: Tue Dec 15 18:25:48 2020, max compression
+gzip compressed data, was "djangoldp_conversation-3.0.0.tar", last modified: Mon Jul 24 21:20:06 2023, max compression
```

## Comparing `djangoldp_conversation-2.0.1.tar` & `djangoldp_conversation-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      612 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      432 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1019 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      342 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       61 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      342 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/
--rw-rw-rw-   0 root         (0) root         (0)     1603 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/models.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1260 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0003_auto_20200522_1521.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0005_auto_20200619_0817.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0006_auto_20200723_1312.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0007_auto_20200926_0911.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0004_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0002_auto_20190917_1056.py
--rw-rw-rw-   0 root         (0) root         (0)     1705 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:25:48.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      763 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/management/commands/mock_conversation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-15 18:25:35.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2020-12-15 18:25:46.000000 djangoldp_conversation-2.0.1/djangoldp_conversation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/djangoldp_conversation/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-24 21:20:03.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/djangoldp_conversation/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/djangoldp_conversation/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/management/commands/mock_conversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0002_auto_20190917_1056.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0003_auto_20200522_1521.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0004_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0005_auto_20200619_0817.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0006_auto_20200723_1312.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0007_auto_20200926_0911.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/djangoldp_conversation/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-24 21:20:06.000000 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-24 21:20:06.000000 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:20:06.000000 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-24 21:20:06.000000 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-24 21:20:06.000000 djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-24 21:20:06.717485 djangoldp_conversation-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:19:47.000000 djangoldp_conversation-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_conversation-2.0.1/setup.cfg` & `djangoldp_conversation-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = matthieu@happy-dev.fr
 description = djangoldp package for conversation data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.0
+	djangoldp~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation.egg-info/SOURCES.txt` & `djangoldp_conversation-3.0.0/djangoldp_conversation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/models.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/factories.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0003_auto_20200522_1521.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0003_auto_20200522_1521.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0005_auto_20200619_0817.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0005_auto_20200619_0817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0006_auto_20200723_1312.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0006_auto_20200723_1312.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0007_auto_20200926_0911.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0007_auto_20200926_0911.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0004_auto_20200610_1323.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0004_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0002_auto_20190917_1056.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0002_auto_20190917_1056.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/migrations/0001_initial.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_conversation-2.0.1/djangoldp_conversation/management/commands/mock_conversation.py` & `djangoldp_conversation-3.0.0/djangoldp_conversation/management/commands/mock_conversation.py`

 * *Files identical despite different names*

