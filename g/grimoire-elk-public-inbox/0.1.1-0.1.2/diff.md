# Comparing `tmp/grimoire_elk_public_inbox-0.1.1.tar.gz` & `tmp/grimoire_elk_public_inbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoire_elk_public_inbox-0.1.1.tar", max compression
+gzip compressed data, was "grimoire_elk_public_inbox-0.1.2.tar", max compression
```

## Comparing `grimoire_elk_public_inbox-0.1.1.tar` & `grimoire_elk_public_inbox-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       50 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/AUTHORS
--rw-r--r--   0        0        0    35149 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/LICENSE
--rw-r--r--   0        0        0      513 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/NEWS
--rw-r--r--   0        0        0     1620 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/__init__.py
--rw-r--r--   0        0        0       86 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/_version.py
--rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/__init__.py
--rw-r--r--   0        0        0      925 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/public_inbox.py
--rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/__init__.py
--rw-r--r--   0        0        0     2200 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/public_inbox.py
--rw-r--r--   0        0        0     1071 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/utils.py
--rw-r--r--   0        0        0     1459 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 grimoire_elk_public_inbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/AUTHORS
+-rw-r--r--   0        0        0    35149 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/LICENSE
+-rw-r--r--   0        0        0      676 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/NEWS
+-rw-r--r--   0        0        0     1620 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/_version.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/enriched/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/enriched/public_inbox.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/raw/__init__.py
+-rw-r--r--   0        0        0     2200 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/raw/public_inbox.py
+-rw-r--r--   0        0        0     1071 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/utils.py
+-rw-r--r--   0        0        0     1459 2023-07-24 10:07:02.935143 grimoire_elk_public_inbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 grimoire_elk_public_inbox-0.1.2/PKG-INFO
```

### Comparing `grimoire_elk_public_inbox-0.1.1/LICENSE` & `grimoire_elk_public_inbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.1/NEWS` & `grimoire_elk_public_inbox-0.1.2/NEWS`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+## grimoirelab-elk-public-inbox 0.1.2 - (2023-07-24)
+
+**Dependencies updateds:**
+
+ * Update dependencies\
+   Dependencies updated to support GrimoireLab 0.13.0.
+
+
 ## grimoirelab-elk-public-inbox 0.1.1 - (2023-07-19)
 
 **Dependencies updateds:**
 
  * Update dependencies\
    Dependencies updated to support GrimoireLab 0.12.0.
```

### Comparing `grimoire_elk_public_inbox-0.1.1/README.md` & `grimoire_elk_public_inbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/public_inbox.py` & `grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/enriched/public_inbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/public_inbox.py` & `grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/raw/public_inbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/utils.py` & `grimoire_elk_public_inbox-0.1.2/grimoire_elk_public_inbox/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.1/pyproject.toml` & `grimoire_elk_public_inbox-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoire-elk-public-inbox"
-version = "0.1.1"
+version = "0.1.2"
 description = "GrimoireELK plugic for public-inbox."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoire_elk_public_inbox-0.1.1/PKG-INFO` & `grimoire_elk_public_inbox-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoire-elk-public-inbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: GrimoireELK plugic for public-inbox.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

