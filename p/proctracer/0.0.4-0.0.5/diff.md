# Comparing `tmp/proctracer-0.0.4.tar.gz` & `tmp/proctracer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.4.tar", last modified: Mon Jul 24 08:39:55 2023, max compression
+gzip compressed data, was "proctracer-0.0.5.tar", last modified: Mon Jul 24 08:43:28 2023, max compression
```

## Comparing `proctracer-0.0.4.tar` & `proctracer-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:39:55.800863 proctracer-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-24 07:17:55.000000 proctracer-0.0.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-23 09:50:38.000000 proctracer-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:39:55.800863 proctracer-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-24 06:59:39.000000 proctracer-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:39:55.800863 proctracer-0.0.4/proctracer/
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-24 08:39:51.000000 proctracer-0.0.4/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:39:55.800863 proctracer-0.0.4/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-24 06:38:58.000000 proctracer-0.0.4/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-07-24 08:35:41.000000 proctracer-0.0.4/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-07-23 10:51:33.000000 proctracer-0.0.4/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-24 06:47:49.000000 proctracer-0.0.4/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-24 06:38:37.000000 proctracer-0.0.4/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4793 2023-07-24 08:38:01.000000 proctracer-0.0.4/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 08:04:40.000000 proctracer-0.0.4/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:39:55.800863 proctracer-0.0.4/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 08:39:55.000000 proctracer-0.0.4/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-24 08:39:55.800863 proctracer-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-24 07:30:52.000000 proctracer-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:43:28.726563 proctracer-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-24 07:17:55.000000 proctracer-0.0.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-23 09:50:38.000000 proctracer-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:43:28.726563 proctracer-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-24 06:59:39.000000 proctracer-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:43:28.722563 proctracer-0.0.5/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-24 08:43:18.000000 proctracer-0.0.5/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:43:28.726563 proctracer-0.0.5/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-24 06:38:58.000000 proctracer-0.0.5/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-07-24 08:35:41.000000 proctracer-0.0.5/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-07-23 10:51:33.000000 proctracer-0.0.5/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-24 06:47:49.000000 proctracer-0.0.5/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-24 06:38:37.000000 proctracer-0.0.5/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4791 2023-07-24 08:42:52.000000 proctracer-0.0.5/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 08:04:40.000000 proctracer-0.0.5/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:43:28.722563 proctracer-0.0.5/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 08:43:28.000000 proctracer-0.0.5/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-24 08:43:28.726563 proctracer-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-24 07:30:52.000000 proctracer-0.0.5/setup.py
```

### Comparing `proctracer-0.0.4/LICENSE.md` & `proctracer-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/PKG-INFO` & `proctracer-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.4
+Version: 0.0.5
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.4/README.md` & `proctracer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/__init__.py` & `proctracer-0.0.5/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.5/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.5/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.5/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.5/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/plugin_base.py` & `proctracer-0.0.5/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.5/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.5/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.5/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.5/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/proctracer/proctracer.py` & `proctracer-0.0.5/proctracer/proctracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 pid_path: ~/proctracer.pid
 plugins:
     text_pipe:
         active: true
         period: 0.05
     pressure_cpu:
         active: true
-        period: 0.05
+        period: 0.5
     pressure_io:
         active: true
-        period: 0.1
+        period: 0.5
     pressure_memory:
         active: true
-        period: 0.2
+        period: 0.5
     stat:
         active: true
         period: 2.0
     pid_stat:
         active: true
-        period: 0.25
+        period: 2.0
     net_dev:
         active: true
         period: 1.0
     net_snmp_udp:
         active: true
         period: 1.0
     net_udp4: &x
```

### Comparing `proctracer-0.0.4/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.5/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.4
+Version: 0.0.5
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.4/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.5/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.4/setup.py` & `proctracer-0.0.5/setup.py`

 * *Files identical despite different names*

