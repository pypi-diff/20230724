# Comparing `tmp/proctracer-0.0.2.tar.gz` & `tmp/proctracer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.2.tar", last modified: Mon Jul 24 07:36:13 2023, max compression
+gzip compressed data, was "proctracer-0.0.3.tar", last modified: Mon Jul 24 08:06:15 2023, max compression
```

## Comparing `proctracer-0.0.2.tar` & `proctracer-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:36:13.222608 proctracer-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-24 07:17:55.000000 proctracer-0.0.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-23 09:50:38.000000 proctracer-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 07:36:13.222608 proctracer-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-24 06:59:39.000000 proctracer-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:36:13.222608 proctracer-0.0.2/proctracer/
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-24 07:36:00.000000 proctracer-0.0.2/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:36:13.222608 proctracer-0.0.2/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-24 06:38:58.000000 proctracer-0.0.2/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4241 2023-07-24 06:47:05.000000 proctracer-0.0.2/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-07-23 10:51:33.000000 proctracer-0.0.2/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-24 06:47:49.000000 proctracer-0.0.2/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-24 06:38:37.000000 proctracer-0.0.2/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4205 2023-07-24 06:36:32.000000 proctracer-0.0.2/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-23 12:02:11.000000 proctracer-0.0.2/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:36:13.222608 proctracer-0.0.2/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 07:36:13.000000 proctracer-0.0.2/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-24 07:36:13.222608 proctracer-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-24 07:30:52.000000 proctracer-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:15.906780 proctracer-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-24 07:17:55.000000 proctracer-0.0.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-23 09:50:38.000000 proctracer-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:06:15.906780 proctracer-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-24 06:59:39.000000 proctracer-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:15.906780 proctracer-0.0.3/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-24 08:06:04.000000 proctracer-0.0.3/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:15.906780 proctracer-0.0.3/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-24 06:38:58.000000 proctracer-0.0.3/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4241 2023-07-24 06:47:05.000000 proctracer-0.0.3/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-07-23 10:51:33.000000 proctracer-0.0.3/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-24 06:47:49.000000 proctracer-0.0.3/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-24 06:38:37.000000 proctracer-0.0.3/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4205 2023-07-24 06:36:32.000000 proctracer-0.0.3/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 08:04:40.000000 proctracer-0.0.3/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:15.906780 proctracer-0.0.3/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 08:06:15.000000 proctracer-0.0.3/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-24 08:06:15.906780 proctracer-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-24 07:30:52.000000 proctracer-0.0.3/setup.py
```

### Comparing `proctracer-0.0.2/LICENSE.md` & `proctracer-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/PKG-INFO` & `proctracer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.2
+Version: 0.0.3
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.2/README.md` & `proctracer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/__init__.py` & `proctracer-0.0.3/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.3/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.3/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.3/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.3/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/plugin_base.py` & `proctracer-0.0.3/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.3/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.3/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.3/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.3/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer/proctracer.py` & `proctracer-0.0.3/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.3/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.2
+Version: 0.0.3
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.2/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.3/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.2/setup.py` & `proctracer-0.0.3/setup.py`

 * *Files identical despite different names*

