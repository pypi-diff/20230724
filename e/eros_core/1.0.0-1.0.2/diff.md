# Comparing `tmp/eros_core-1.0.0.tar.gz` & `tmp/eros_core-1.0.2.tar.gz`

## Comparing `eros_core-1.0.0.tar` & `eros_core-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 eros_core-1.0.0/pytest.ini
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 eros_core-1.0.0/requirements.txt
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 eros_core-1.0.0/.github/workflows/test_installation.yml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 eros_core-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 eros_core-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 eros_core-1.0.0/demo/demo_interactive_serial.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 eros_core-1.0.0/demo/demo_serial_logging.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/eros_cli.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/eros_cli_client.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/eros_cli_client_test.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/eros_zmq_test.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/log_color.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 eros_core-1.0.0/examples/package_test.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/__init__.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/eros_analytics.py
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/eros_layers.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/eros_terminal.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/main.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_generic.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_loopback.py
--rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_serial.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_serial_sim.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_tcp.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_udp.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_udp_sim.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/transport/drv_zmq.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 eros_core-1.0.0/src/eros_core/utils/request_response.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/tcp_echo.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/test_drv_tcp.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/test_drv_uart.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/test_eros.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/test_eros_layers.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 eros_core-1.0.0/tests/test_eros_perf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 eros_core-1.0.0/.gitignore
--rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 eros_core-1.0.0/LICENCE
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eros_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 eros_core-1.0.0/readme.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 eros_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 eros_core-1.0.2/pytest.ini
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 eros_core-1.0.2/.github/workflows/test_installation.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 eros_core-1.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 eros_core-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 eros_core-1.0.2/demo/demo_interactive_serial.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 eros_core-1.0.2/demo/demo_serial_logging.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/eros_cli.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/eros_cli_client.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/eros_cli_client_test.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/eros_zmq_test.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/log_color.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 eros_core-1.0.2/examples/package_test.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/__init__.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/eros_analytics.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/eros_layers.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/eros_terminal.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/main.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_generic.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_loopback.py
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_serial.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_serial_sim.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_tcp.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_udp.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_udp_sim.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/transport/drv_zmq.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 eros_core-1.0.2/src/eros_core/utils/request_response.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/tcp_echo.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/test_drv_tcp.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/test_drv_uart.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/test_eros.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/test_eros_layers.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 eros_core-1.0.2/tests/test_eros_perf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 eros_core-1.0.2/.gitignore
+-rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 eros_core-1.0.2/LICENCE
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 eros_core-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 eros_core-1.0.2/readme.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 eros_core-1.0.2/PKG-INFO
```

### Comparing `eros_core-1.0.0/.github/workflows/test_installation.yml` & `eros_core-1.0.2/.github/workflows/test_installation.yml`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/.vscode/launch.json` & `eros_core-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/.vscode/settings.json` & `eros_core-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/demo/demo_serial_logging.py` & `eros_core-1.0.2/demo/demo_serial_logging.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/examples/eros_cli.py` & `eros_core-1.0.2/examples/eros_cli.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/examples/eros_cli_client.py` & `eros_core-1.0.2/examples/eros_cli_client.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/examples/eros_cli_client_test.py` & `eros_core-1.0.2/examples/eros_cli_client_test.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/examples/log_color.py` & `eros_core-1.0.2/examples/log_color.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/eros_analytics.py` & `eros_core-1.0.2/src/eros_core/eros_analytics.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/eros_layers.py` & `eros_core-1.0.2/src/eros_core/eros_layers.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/eros_terminal.py` & `eros_core-1.0.2/src/eros_core/eros_terminal.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/main.py` & `eros_core-1.0.2/src/eros_core/main.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_generic.py` & `eros_core-1.0.2/src/eros_core/transport/drv_generic.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_loopback.py` & `eros_core-1.0.2/src/eros_core/transport/drv_loopback.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_serial.py` & `eros_core-1.0.2/src/eros_core/transport/drv_serial.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_serial_sim.py` & `eros_core-1.0.2/src/eros_core/transport/drv_serial_sim.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_tcp.py` & `eros_core-1.0.2/src/eros_core/transport/drv_tcp.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_udp.py` & `eros_core-1.0.2/src/eros_core/transport/drv_udp.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_udp_sim.py` & `eros_core-1.0.2/src/eros_core/transport/drv_udp_sim.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/transport/drv_zmq.py` & `eros_core-1.0.2/src/eros_core/transport/drv_zmq.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/src/eros_core/utils/request_response.py` & `eros_core-1.0.2/src/eros_core/utils/request_response.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/tcp_echo.py` & `eros_core-1.0.2/tests/tcp_echo.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/test_drv_tcp.py` & `eros_core-1.0.2/tests/test_drv_tcp.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/test_drv_uart.py` & `eros_core-1.0.2/tests/test_drv_uart.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/test_eros.py` & `eros_core-1.0.2/tests/test_eros.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/test_eros_layers.py` & `eros_core-1.0.2/tests/test_eros_layers.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/tests/test_eros_perf.py` & `eros_core-1.0.2/tests/test_eros_perf.py`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/LICENCE` & `eros_core-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `eros_core-1.0.0/pyproject.toml` & `eros_core-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "eros_core"
 authors = [
     {name = "Floris Vernieuwe", email = "floris@vernieuwe.eu"},
 ]
 description = "EROS-core Package"
 
 readme = "readme.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `eros_core-1.0.0/PKG-INFO` & `eros_core-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: eros_core
-Version: 1.0.0
+Version: 1.0.2
 Summary: EROS-core Package
 Author-email: Floris Vernieuwe <floris@vernieuwe.eu>
 License-File: LICENCE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: bitstruct==8.17.0
 Requires-Dist: cobs==1.2.0
 Requires-Dist: pyserial==3.5
 Requires-Dist: pyzmq==25.1.0
 Description-Content-Type: text/markdown
 
 
 ## EROS-core
 
 Build test
 
 [![Python test package installation](https://github.com/Florioo/eros-core-python/actions/workflows/test_installation.yml/badge.svg)](https://github.com/Florioo/eros-core-python/actions/workflows/test_installation.yml)
-
-
-## Documentation -> TODO
```

