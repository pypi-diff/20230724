# Comparing `tmp/contact_magic-0.5.6.tar.gz` & `tmp/contact_magic-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.6.tar", max compression
+gzip compressed data, was "contact_magic-0.5.7.tar", max compression
```

## Comparing `contact_magic-0.5.6.tar` & `contact_magic-0.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.6/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.6/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.6/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.6/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5418 2023-07-20 15:24:39.359080 contact_magic-0.5.6/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2663 2023-07-20 16:08:38.910133 contact_magic-0.5.6/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3716 2023-07-20 14:30:01.195479 contact_magic-0.5.6/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.6/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2579 2023-07-20 16:08:38.513794 contact_magic-0.5.6/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1784 2023-07-20 14:41:42.621150 contact_magic-0.5.6/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.6/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.6/contact_magic/logger.py
--rw-r--r--   0        0        0    16920 2023-07-20 15:55:40.352110 contact_magic-0.5.6/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.6/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.6/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.6/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.6/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.6/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.6/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.6/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.6/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.6/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-07-20 16:00:56.144079 contact_magic-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.7/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.7/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.7/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.7/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5418 2023-07-20 15:24:39.359080 contact_magic-0.5.7/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2663 2023-07-20 16:08:38.910133 contact_magic-0.5.7/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-20 14:30:01.195479 contact_magic-0.5.7/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.7/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-24 08:11:52.431177 contact_magic-0.5.7/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1786 2023-07-24 08:11:09.776013 contact_magic-0.5.7/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.7/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.7/contact_magic/logger.py
+-rw-r--r--   0        0        0    16920 2023-07-20 15:55:40.352110 contact_magic-0.5.7/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.7/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.7/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.7/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.7/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.7/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.7/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.7/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.7/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.7/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-24 08:11:37.573552 contact_magic-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.7/PKG-INFO
```

### Comparing `contact_magic-0.5.6/README.md` & `contact_magic-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/asyncio.py` & `contact_magic-0.5.7/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/conf/settings.py` & `contact_magic-0.5.7/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/dict_utils.py` & `contact_magic-0.5.7/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/helpers.py` & `contact_magic-0.5.7/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.7/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.7/contact_magic/integrations/sales_scrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
                 return res.json()
             if res.status_code == 422:
                 validation_errors = res.json().get("detail")
                 for error in validation_errors:
                     if error.get("type") == "value_error.url.scheme":
                         error_key = error.get("loc")[1]
                         if error_key in data:
-                            data[error_key] = fix_website(data[error_key])
+                            params[error_key] = fix_website(data[error_key])
             await asyncio.sleep(1)
             retries += 1
         return None
     except Exception:
         return None
```

### Comparing `contact_magic-0.5.6/contact_magic/integrations/sheets.py` & `contact_magic-0.5.7/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/models.py` & `contact_magic-0.5.7/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/preprocessors.py` & `contact_magic-0.5.7/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/scripts/agency.py` & `contact_magic-0.5.7/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.5.7/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.7/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.5.7/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.7/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/contact_magic/utils.py` & `contact_magic-0.5.7/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.6/pyproject.toml` & `contact_magic-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.6"
+version = "0.5.7"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.6/PKG-INFO` & `contact_magic-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.6
+Version: 0.5.7
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

