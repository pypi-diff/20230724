# Comparing `tmp/mine-4.1.tar.gz` & `tmp/mine-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-4.1.tar", max compression
+gzip compressed data, was "mine-4.2.tar", max compression
```

## Comparing `mine-4.1.tar` & `mine-4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.1/LICENSE.md
--rw-r--r--   0        0        0     2841 2023-07-20 03:59:49.514562 mine-4.1/README.md
--rw-r--r--   0        0        0      340 2023-07-20 16:16:17.756329 mine-4.1/mine/__init__.py
--rw-r--r--   0        0        0     6947 2023-07-22 17:36:25.564173 mine-4.1/mine/cli.py
--rw-r--r--   0        0        0     2889 2023-07-20 03:59:49.515236 mine-4.1/mine/common.py
--rw-r--r--   0        0        0      738 2023-07-22 17:00:58.306091 mine-4.1/mine/daemon.py
--rw-r--r--   0        0        0     6572 2023-07-21 15:47:11.834590 mine-4.1/mine/manager.py
--rw-r--r--   0        0        0      217 2023-07-20 03:59:49.515737 mine-4.1/mine/models/__init__.py
--rw-r--r--   0        0        0     1095 2023-07-20 03:59:49.516054 mine-4.1/mine/models/application.py
--rw-r--r--   0        0        0     2256 2023-07-20 17:01:39.723214 mine-4.1/mine/models/computer.py
--rw-r--r--   0        0        0     3849 2023-07-20 16:44:45.581239 mine-4.1/mine/models/config.py
--rw-r--r--   0        0        0     5504 2023-07-22 17:26:46.814498 mine-4.1/mine/models/data.py
--rw-r--r--   0        0        0     5851 2023-07-22 17:26:02.306292 mine-4.1/mine/models/status.py
--rw-r--r--   0        0        0      882 2023-07-20 03:59:49.517420 mine-4.1/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2633 2023-07-21 15:47:11.835482 mine-4.1/mine/services.py
--rw-r--r--   0        0        0      578 2023-07-20 03:59:49.517606 mine-4.1/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.1/mine/tests/__init__.py
--rw-r--r--   0        0        0     1044 2023-07-22 16:40:54.685419 mine-4.1/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     4331 2023-07-22 17:37:18.341856 mine-4.1/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3493 2023-07-20 03:59:49.518427 mine-4.1/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.1/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     2259 2023-07-20 17:04:31.061085 mine-4.1/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0     3129 2023-07-20 17:03:59.687664 mine-4.1/mine/tests/test_models_config.py
--rw-r--r--   0        0        0     1317 2023-07-22 17:32:29.302799 mine-4.1/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4953 2023-07-21 16:23:58.330586 mine-4.1/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.1/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3283 2023-07-21 15:47:11.836361 mine-4.1/mine/tests/test_services.py
--rw-r--r--   0        0        0     2238 2023-07-22 17:06:03.413807 mine-4.1/pyproject.toml
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 mine-4.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-10-23 17:27:35.488744 mine-4.2/LICENSE.md
+-rw-r--r--   0        0        0     2841 2023-07-20 03:45:18.010837 mine-4.2/README.md
+-rw-r--r--   0        0        0      340 2023-07-22 21:08:12.320173 mine-4.2/mine/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-22 21:08:30.570000 mine-4.2/mine/cli.py
+-rw-r--r--   0        0        0     2889 2023-07-22 21:08:12.321547 mine-4.2/mine/common.py
+-rw-r--r--   0        0        0      738 2023-07-22 21:08:30.569778 mine-4.2/mine/daemon.py
+-rw-r--r--   0        0        0     6572 2023-07-22 21:08:30.569577 mine-4.2/mine/manager.py
+-rw-r--r--   0        0        0      217 2023-07-22 21:08:12.326238 mine-4.2/mine/models/__init__.py
+-rw-r--r--   0        0        0      954 2023-07-23 22:26:19.222130 mine-4.2/mine/models/application.py
+-rw-r--r--   0        0        0     2256 2023-07-22 21:08:12.326496 mine-4.2/mine/models/computer.py
+-rw-r--r--   0        0        0     3849 2023-07-22 21:08:30.569361 mine-4.2/mine/models/config.py
+-rw-r--r--   0        0        0     5670 2023-07-23 22:31:32.374401 mine-4.2/mine/models/data.py
+-rw-r--r--   0        0        0     5851 2023-07-22 21:08:30.568931 mine-4.2/mine/models/status.py
+-rw-r--r--   0        0        0      882 2023-07-22 21:08:12.326960 mine-4.2/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2673 2023-07-22 21:08:30.568665 mine-4.2/mine/services.py
+-rw-r--r--   0        0        0      578 2023-07-22 21:08:12.321813 mine-4.2/mine/settings.py
+-rw-r--r--   0        0        0       34 2023-07-22 21:08:12.323714 mine-4.2/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-22 21:08:12.322810 mine-4.2/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2020-10-23 17:27:35.492167 mine-4.2/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2020-10-23 17:27:35.492276 mine-4.2/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2020-10-23 17:27:35.492361 mine-4.2/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     4331 2023-07-22 21:08:12.324565 mine-4.2/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3493 2023-07-22 21:08:12.324242 mine-4.2/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1002 2023-07-22 21:08:12.323965 mine-4.2/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     2259 2023-07-22 21:08:12.325663 mine-4.2/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0     3129 2023-07-22 21:08:12.325136 mine-4.2/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0     1191 2023-07-23 22:44:50.953149 mine-4.2/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4953 2023-07-22 21:08:12.323130 mine-4.2/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-07-22 21:08:12.325399 mine-4.2/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3283 2023-07-22 21:08:12.323490 mine-4.2/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2238 2023-07-23 22:28:33.324956 mine-4.2/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 mine-4.2/PKG-INFO
```

### Comparing `mine-4.1/LICENSE.md` & `mine-4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-4.1/README.md` & `mine-4.2/README.md`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/cli.py` & `mine-4.2/mine/cli.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/common.py` & `mine-4.2/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/daemon.py` & `mine-4.2/mine/daemon.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/manager.py` & `mine-4.2/mine/manager.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/models/application.py` & `mine-4.2/mine/models/application.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 @dataclass
 class Properties:
     """Dictionary of application management settings."""
 
     auto_queue: bool = False
     single_instance: bool = False
+    keep_running: bool = False
 
 
 @dataclass
 class Application:
     """Dictionary of application information."""
 
     name: str
@@ -35,15 +36,7 @@
         return str(self).lower() == str(other).lower()
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __lt__(self, other):
         return str(self).lower() < str(other).lower()
-
-    @property
-    def auto_queue(self):
-        return self.properties.auto_queue
-
-    @property
-    def no_wait(self):
-        return not self.properties.single_instance
```

### Comparing `mine-4.1/mine/models/computer.py` & `mine-4.2/mine/models/computer.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/models/config.py` & `mine-4.2/mine/models/config.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/models/data.py` & `mine-4.2/mine/models/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,28 +50,31 @@
                     computer.timestamp.started = 0
                     computer.timestamp.stopped = 0
 
     def queue_all_applications(self, computer: Computer):
         """Queue applications for launch."""
         log.info("Queuing applications for launch...")
         for application in self.config.applications:
-            if application.auto_queue:
+            if application.properties.auto_queue:
                 log.debug("Queuing %s on %s...", application, computer)
                 self.status.queue(application, computer)
 
     def launch_queued_applications(self, computer: Computer, manager: Manager):
         """Launch applications that have been queued."""
         log.info("Launching queued applications...")
         for status in self.status.applications:
             if status.next:
                 application = self.config.get_application(status.application)
                 print(crayons.yellow(f"{application} is queued for {status.next}"))
                 if status.next == computer:
                     latest = self.status.get_latest(application)
-                    if latest in (computer, None) or application.no_wait:
+                    if (
+                        latest in (computer, None)
+                        or not application.properties.single_instance
+                    ):
                         if not manager.is_running(application):
                             manager.start(application)
                         status.next = None
                     else:
                         print(
                             crayons.yellow(
                                 f"{application} is still running on {latest}"
@@ -80,15 +83,16 @@
                 elif manager.is_running(application):
                     manager.stop(application)
 
     def close_all_applications(self, manager: Manager):
         """Close all applications running on this computer."""
         log.info("Closing all applications on this computer...")
         for application in self.config.applications:
-            manager.stop(application)
+            if not application.properties.keep_running:
+                manager.stop(application)
 
     def update_status(self, computer: Computer, manager: Manager):
         """Update each application's status."""
         log.info("Recording application status...")
         for application in self.config.applications:
             latest = self.status.get_latest(application)
             if manager.is_running(application):
```

### Comparing `mine-4.1/mine/models/status.py` & `mine-4.2/mine/models/status.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/models/timestamp.py` & `mine-4.2/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/services.py` & `mine-4.2/mine/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     for dirname, _, filenames in os.walk(root):
         for filename in filenames:
             if regex.match(filename):
                 count += 1
                 path = os.path.join(dirname, filename)
                 if force:
                     os.remove(path)
-                print(path)
+                if not config_only:
+                    print(path)
 
     if count and not force:
         print(f"\nRun again with '--force' to delete these {count} conflict(s)")
         return 0
 
     return count
```

### Comparing `mine-4.1/mine/settings.py` & `mine-4.2/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/conftest.py` & `mine-4.2/mine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/files/mine-in.yml` & `mine-4.2/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/files/mine-out.yml` & `mine-4.2/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_cli.py` & `mine-4.2/mine/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_manager.py` & `mine-4.2/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_models_application.py` & `mine-4.2/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_models_computer.py` & `mine-4.2/mine/tests/test_models_computer.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_models_config.py` & `mine-4.2/mine/tests/test_models_config.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_models_data.py` & `mine-4.2/mine/tests/test_models_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from mine.models import Data
 
 
 def describe_data():
     @pytest.fixture
     def data(monkeypatch):
         monkeypatch.setattr(datafiles.settings, "HOOKS_ENABLED", False)
-        return Data("../../tests/files/mine.yml")
+        return Data("tmp/mine.yml")
 
     def describe_repr():
         def it_should_always_be_a_simple_name(data: Data):
             assert "settings" == repr(data)
 
     def describe_modified():
         def is_false_initially(data: Data):
@@ -30,17 +30,15 @@
 
             print(data.modified)
 
             assert False is data.modified
 
     def describe_prune_status():
         def it_can_preserve_counter(data: Data):
-            data.datafile.load()  # type: ignore
-            assert data.status.counter > 0
+            data.status.counter = 1
             data.prune_status()
             assert data.status.counter > 0
 
         def it_can_reset_counter(data: Data):
-            data.datafile.load()  # type: ignore
-            assert data.status.counter > 0
+            data.status.counter = 1
             data.prune_status(reset_counter=True)
             assert data.status.counter == 0
```

### Comparing `mine-4.1/mine/tests/test_models_status.py` & `mine-4.2/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_models_timestamp.py` & `mine-4.2/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/mine/tests/test_services.py` & `mine-4.2/mine/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `mine-4.1/pyproject.toml` & `mine-4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "4.1"
+version = "4.2"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `mine-4.1/PKG-INFO` & `mine-4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 4.1
+Version: 4.2
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

