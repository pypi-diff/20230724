# Comparing `tmp/trycourier-4.5.0.tar.gz` & `tmp/trycourier-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-4.5.0.tar", last modified: Mon Jun 26 21:20:05 2023, max compression
+gzip compressed data, was "trycourier-4.6.0.tar", last modified: Mon Jul 24 18:18:14 2023, max compression
```

## Comparing `trycourier-4.5.0.tar` & `trycourier-4.6.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 21:19:49.000000 trycourier-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-06-26 21:20:05.131554 trycourier-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-06-26 21:19:49.000000 trycourier-4.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:20:05.131554 trycourier-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-26 21:19:49.000000 trycourier-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.127554 trycourier-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/trycourier/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/trycourier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.342455 trycourier-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 18:17:55.000000 trycourier-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-24 18:18:14.342455 trycourier-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-24 18:17:55.000000 trycourier-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:18:14.342455 trycourier-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 18:17:55.000000 trycourier-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.334454 trycourier-4.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.338454 trycourier-4.6.0/trycourier/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.338454 trycourier-4.6.0/trycourier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/top_level.txt
```

### Comparing `trycourier-4.5.0/LICENSE` & `trycourier-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/PKG-INFO` & `trycourier-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.5.0
+Version: 4.6.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trycourier-4.5.0/README.md` & `trycourier-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/setup.py` & `trycourier-4.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="trycourier",
-    version="4.5.0",
+    version="4.6.0",
     author="Courier",
     author_email="support@courier.com",
     description="A Python Package for communicating with the Courier REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/trycourier/courier-python",
     packages=setuptools.find_packages(),
```

### Comparing `trycourier-4.5.0/tests/test_audiences.py` & `trycourier-4.6.0/tests/test_audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_audit_events.py` & `trycourier-4.6.0/tests/test_audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_automations.py` & `trycourier-4.6.0/tests/test_automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_bulk.py` & `trycourier-4.6.0/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_client.py` & `trycourier-4.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_lists.py` & `trycourier-4.6.0/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_messages.py` & `trycourier-4.6.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_notifications.py` & `trycourier-4.6.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_profiles.py` & `trycourier-4.6.0/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/tests/test_session.py` & `trycourier-4.6.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/audiences.py` & `trycourier-4.6.0/trycourier/audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/audit_events.py` & `trycourier-4.6.0/trycourier/audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/automations.py` & `trycourier-4.6.0/trycourier/automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/bulk.py` & `trycourier-4.6.0/trycourier/bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/client.py` & `trycourier-4.6.0/trycourier/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from os import environ
 
+from .accounts import Accounts
 from .audiences import Audiences
 from .audit_events import AuditEvents
 from .automations import Automations
 from .bulk import Bulk
 from .exceptions import CourierAPIException
 from .session import CourierAPISession
 from .lists import Lists
 from .messages import Messages
 from .notifications import Notifications
 from .profiles import Profiles
 
-__version__ = '4.4.0'
+__version__ = '4.6.0'
 
 
 class Courier(object):
 
     def __init__(self,
                  base_url=None,
                  auth_token=None,
@@ -54,14 +55,15 @@
             self.session.init_basic_auth(username, password)
         elif 'COURIER_AUTH_USERNAME' in environ \
                 and 'COURIER_AUTH_PASSWORD' in environ:
             username = environ.get('COURIER_AUTH_USERNAME', None)
             password = environ.get('COURIER_AUTH_PASSWORD', None)
             self.session.init_basic_auth(username, password)
 
+        self.accounts = Accounts(self.base_url, self.session)
         self.audiences = Audiences(self.base_url, self.session)
         self.audit_events = AuditEvents(self.base_url, self.session)
         self.automations = Automations(self.base_url, self.session)
         self.bulk = Bulk(self.base_url, self.session)
         self.lists = Lists(self.base_url, self.session)
         self.messages = Messages(self.base_url, self.session)
         self.notifications = Notifications(self.base_url, self.session)
```

### Comparing `trycourier-4.5.0/trycourier/lists.py` & `trycourier-4.6.0/trycourier/lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/messages.py` & `trycourier-4.6.0/trycourier/messages.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/notifications.py` & `trycourier-4.6.0/trycourier/notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/profiles.py` & `trycourier-4.6.0/trycourier/profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier/session.py` & `trycourier-4.6.0/trycourier/session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.5.0/trycourier.egg-info/PKG-INFO` & `trycourier-4.6.0/trycourier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.5.0
+Version: 4.6.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trycourier-4.5.0/trycourier.egg-info/SOURCES.txt` & `trycourier-4.6.0/trycourier.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
+tests/test_accounts.py
 tests/test_audiences.py
 tests/test_audit_events.py
 tests/test_automations.py
 tests/test_bulk.py
 tests/test_client.py
 tests/test_exceptions.py
 tests/test_lists.py
 tests/test_messages.py
 tests/test_notifications.py
 tests/test_profiles.py
 tests/test_session.py
 trycourier/__init__.py
+trycourier/accounts.py
 trycourier/audiences.py
 trycourier/audit_events.py
 trycourier/automations.py
 trycourier/bulk.py
 trycourier/client.py
 trycourier/exceptions.py
 trycourier/lists.py
```

