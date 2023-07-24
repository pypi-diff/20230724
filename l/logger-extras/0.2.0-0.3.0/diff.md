# Comparing `tmp/logger_extras-0.2.0.tar.gz` & `tmp/logger_extras-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_extras-0.2.0.tar", last modified: Sat Jul 22 22:53:06 2023, max compression
+gzip compressed data, was "logger_extras-0.3.0.tar", last modified: Mon Jul 24 19:38:35 2023, max compression
```

## Comparing `logger_extras-0.2.0.tar` & `logger_extras-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-22 22:52:52.000000 logger_extras-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-22 22:52:52.000000 logger_extras-0.2.0/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-22 22:52:52.000000 logger_extras-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-22 22:52:52.000000 logger_extras-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-22 22:52:52.000000 logger_extras-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-22 22:53:06.129033 logger_extras-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-22 22:52:52.000000 logger_extras-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/logger_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-22 22:52:52.000000 logger_extras-0.2.0/logger_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-22 22:52:52.000000 logger_extras-0.2.0/logger_extras/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-22 22:52:52.000000 logger_extras-0.2.0/logger_extras/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 22:52:52.000000 logger_extras-0.2.0/logger_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-22 22:52:52.000000 logger_extras-0.2.0/logger_extras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/logger_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 22:53:06.000000 logger_extras-0.2.0/logger_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-22 22:52:52.000000 logger_extras-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 22:53:06.129033 logger_extras-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:53:06.129033 logger_extras-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-22 22:52:52.000000 logger_extras-0.2.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.805817 logger_extras-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 19:38:14.000000 logger_extras-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.793817 logger_extras-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.797817 logger_extras-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-24 19:38:14.000000 logger_extras-0.3.0/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 19:38:14.000000 logger_extras-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 19:38:14.000000 logger_extras-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-24 19:38:14.000000 logger_extras-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-24 19:38:35.805817 logger_extras-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-24 19:38:14.000000 logger_extras-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.801817 logger_extras-0.3.0/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-24 19:38:14.000000 logger_extras-0.3.0/logger_extras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.805817 logger_extras-0.3.0/logger_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 19:38:35.000000 logger_extras-0.3.0/logger_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 19:38:14.000000 logger_extras-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:38:35.805817 logger_extras-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:38:35.805817 logger_extras-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-24 19:38:14.000000 logger_extras-0.3.0/tests/test_tools.py
```

### Comparing `logger_extras-0.2.0/.github/workflows/test_build.yml` & `logger_extras-0.3.0/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/.gitignore` & `logger_extras-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/LICENSE` & `logger_extras-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/PKG-INFO` & `logger_extras-0.3.0/logger_extras.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: logger_extras
-Version: 0.2.0
+Name: logger-extras
+Version: 0.3.0
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,26 +53,57 @@
 
 ```bash
 pip install logging-extras[mqtt]
 ```
 
 ## Tools
 
+- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `RelativeTimeFilter` - A logging filter that adds a relative time to the log record.
 - `DiffTimeFilter` - A logging filter that adds a time difference to the log record.
 - `TieredFormatter` - A logging formatter that allows for different formatting based on the log level.
 - `log_function_call` - A decorator that logs the arguments and return value of a function call.
 
 Upcomming tools:
 
-- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `MQTTSubscriber` - A logging listener that subscribes to an MQTT broker and logs messages.
 
 ## Examples
 
+### `MQTThandler`
+
+```python
+import logging
+
+from paho.mqtt.client import Client
+from logger_extras import MQTTConfig, MQTThandler
+
+handler = MQTThandler(
+    host="localhost",
+    topic="logs",
+    append_logger_name=True,
+)
+handler.setFormatter(logging.Formatter("%(levelname)s - %(message)s)"))
+
+logger = logging.getLogger(__name__)
+logger.addHandler(handler)
+logger.setLevel(logging.INFO)
+
+logger.info("Hello World!")
+
+# This will publish the following message to the MQTT broker on the topic "logs/__main__":
+# {
+#   "timestamp": 1690226241.740354,
+#   "message": "INFO - Hello World!",
+#   "raw_message": "Hello World!",
+#   "level": "INFO", "name": "__main__"
+# }
+
+```
+
 ### `RelativeTimeFilter`
 
 ```python
 import logging
 from time import sleep
 
 from logger_extras import RelativeTimeFilter
```

### Comparing `logger_extras-0.2.0/README.md` & `logger_extras-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,57 @@
 
 ```bash
 pip install logging-extras[mqtt]
 ```
 
 ## Tools
 
+- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `RelativeTimeFilter` - A logging filter that adds a relative time to the log record.
 - `DiffTimeFilter` - A logging filter that adds a time difference to the log record.
 - `TieredFormatter` - A logging formatter that allows for different formatting based on the log level.
 - `log_function_call` - A decorator that logs the arguments and return value of a function call.
 
 Upcomming tools:
 
-- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `MQTTSubscriber` - A logging listener that subscribes to an MQTT broker and logs messages.
 
 ## Examples
 
+### `MQTThandler`
+
+```python
+import logging
+
+from paho.mqtt.client import Client
+from logger_extras import MQTTConfig, MQTThandler
+
+handler = MQTThandler(
+    host="localhost",
+    topic="logs",
+    append_logger_name=True,
+)
+handler.setFormatter(logging.Formatter("%(levelname)s - %(message)s)"))
+
+logger = logging.getLogger(__name__)
+logger.addHandler(handler)
+logger.setLevel(logging.INFO)
+
+logger.info("Hello World!")
+
+# This will publish the following message to the MQTT broker on the topic "logs/__main__":
+# {
+#   "timestamp": 1690226241.740354,
+#   "message": "INFO - Hello World!",
+#   "raw_message": "Hello World!",
+#   "level": "INFO", "name": "__main__"
+# }
+
+```
+
 ### `RelativeTimeFilter`
 
 ```python
 import logging
 from time import sleep
 
 from logger_extras import RelativeTimeFilter
```

### Comparing `logger_extras-0.2.0/logger_extras/filters.py` & `logger_extras-0.3.0/logger_extras/filters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/logger_extras/formatters.py` & `logger_extras-0.3.0/logger_extras/formatters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/logger_extras/utils.py` & `logger_extras-0.3.0/logger_extras/utils.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/logger_extras.egg-info/PKG-INFO` & `logger_extras-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: logger-extras
-Version: 0.2.0
+Name: logger_extras
+Version: 0.3.0
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,26 +53,57 @@
 
 ```bash
 pip install logging-extras[mqtt]
 ```
 
 ## Tools
 
+- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `RelativeTimeFilter` - A logging filter that adds a relative time to the log record.
 - `DiffTimeFilter` - A logging filter that adds a time difference to the log record.
 - `TieredFormatter` - A logging formatter that allows for different formatting based on the log level.
 - `log_function_call` - A decorator that logs the arguments and return value of a function call.
 
 Upcomming tools:
 
-- `MQTThandler` - A logging handler that publishes logs to an MQTT broker.
 - `MQTTSubscriber` - A logging listener that subscribes to an MQTT broker and logs messages.
 
 ## Examples
 
+### `MQTThandler`
+
+```python
+import logging
+
+from paho.mqtt.client import Client
+from logger_extras import MQTTConfig, MQTThandler
+
+handler = MQTThandler(
+    host="localhost",
+    topic="logs",
+    append_logger_name=True,
+)
+handler.setFormatter(logging.Formatter("%(levelname)s - %(message)s)"))
+
+logger = logging.getLogger(__name__)
+logger.addHandler(handler)
+logger.setLevel(logging.INFO)
+
+logger.info("Hello World!")
+
+# This will publish the following message to the MQTT broker on the topic "logs/__main__":
+# {
+#   "timestamp": 1690226241.740354,
+#   "message": "INFO - Hello World!",
+#   "raw_message": "Hello World!",
+#   "level": "INFO", "name": "__main__"
+# }
+
+```
+
 ### `RelativeTimeFilter`
 
 ```python
 import logging
 from time import sleep
 
 from logger_extras import RelativeTimeFilter
```

### Comparing `logger_extras-0.2.0/pyproject.toml` & `logger_extras-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.2.0/tests/test_tools.py` & `logger_extras-0.3.0/tests/test_tools.py`

 * *Files identical despite different names*

