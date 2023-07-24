# Comparing `tmp/Furious-GUI-0.1.0.tar.gz` & `tmp/Furious-GUI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.0.tar", last modified: Mon Jul 24 11:51:04 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.1.tar", last modified: Mon Jul 24 12:49:20 2023, max compression
```

## Comparing `Furious-GUI-0.1.0.tar` & `Furious-GUI-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.625865 Furious-GUI-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.541155 Furious-GUI-0.1.0/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.541155 Furious-GUI-0.1.0/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.556667 Furious-GUI-0.1.0/Furious/Core/
--rw-rw-rw-   0        0        0    19804 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.556667 Furious-GUI-0.1.0/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.556667 Furious-GUI-0.1.0/Furious/Utility/
--rw-rw-rw-   0        0        0      997 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.572246 Furious-GUI-0.1.0/Furious/Widget/
--rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.509714 Furious-GUI-0.1.0/Furious/data/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.572246 Furious-GUI-0.1.0/Furious/data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.572246 Furious-GUI-0.1.0/Furious/data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.594319 Furious-GUI-0.1.0/Furious/data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-24 11:35:24.000000 Furious-GUI-0.1.0/Furious/data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-24 11:51:04.625865 Furious-GUI-0.1.0/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6523 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 11:51:04.000000 Furious-GUI-0.1.0/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-24 11:48:32.000000 Furious-GUI-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6523 2023-07-24 11:51:04.625865 Furious-GUI-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5521 2023-07-24 11:47:44.000000 Furious-GUI-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 11:51:04.625865 Furious-GUI-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1998 2023-07-24 11:47:44.000000 Furious-GUI-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.070903 Furious-GUI-0.1.1/Furious/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.133483 Furious-GUI-0.1.1/Furious/Action/
+-rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.164902 Furious-GUI-0.1.1/Furious/Core/
+-rw-rw-rw-   0        0        0    19804 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.180019 Furious-GUI-0.1.1/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.258603 Furious-GUI-0.1.1/Furious/Utility/
+-rw-rw-rw-   0        0        0     1011 2023-07-24 12:48:19.000000 Furious-GUI-0.1.1/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-24 12:48:46.000000 Furious-GUI-0.1.1/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.320942 Furious-GUI-0.1.1/Furious/Widget/
+-rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.039841 Furious-GUI-0.1.1/Furious/data/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.336384 Furious-GUI-0.1.1/Furious/data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.352817 Furious-GUI-0.1.1/Furious/data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.383423 Furious-GUI-0.1.1/Furious/data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0     6568 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-24 11:48:32.000000 Furious-GUI-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6568 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5566 2023-07-24 12:41:32.000000 Furious-GUI-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1998 2023-07-24 11:58:03.000000 Furious-GUI-0.1.1/setup.py
```

### Comparing `Furious-GUI-0.1.0/Furious/Action/Connect.py` & `Furious-GUI-0.1.1/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Action/Export.py` & `Furious-GUI-0.1.1/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Action/Import.py` & `Furious-GUI-0.1.1/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Action/Language.py` & `Furious-GUI-0.1.1/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Action/Routing.py` & `Furious-GUI-0.1.1/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Action/Settings.py` & `Furious-GUI-0.1.1/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Core/Configuration.py` & `Furious-GUI-0.1.1/Furious/Core/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Core/Core.py` & `Furious-GUI-0.1.1/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.1/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Gui/Action.py` & `Furious-GUI-0.1.1/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Constants.py` & `Furious-GUI-0.1.1/Furious/Utility/Constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 import math
 import pathlib
 import platform
 
 APPLICATION_NAME = 'Furious'
 APPLICATION_VERSION = __version__
-# TODO
 APPLICATION_MACOS_SIGNATURE = 'com.furious'
-APPLICATION_ABOUT_PAGE = 'https://www.baidu.com/'
-APPLICATION_REPO_OWNER_NAME = 'xtls'
-APPLICATION_REPO_NAME = 'xray-core'
+APPLICATION_ABOUT_PAGE = 'https://github.com/LorenEteval/Furious/'
+APPLICATION_REPO_OWNER_NAME = 'LorenEteval'
+APPLICATION_REPO_NAME = 'Furious'
 
 ORGANIZATION_NAME = 'Furious'
 ORGANIZATION_DOMAIN = 'furious.network'
 
 PLATFORM = platform.system()
 
 LOCAL_SERVER_NAME = '891ad49d-8996-43cb-820c-d9baf42a04de'
```

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Process.py` & `Furious-GUI-0.1.1/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.1/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Resources.py` & `Furious-GUI-0.1.1/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Settings.py` & `Furious-GUI-0.1.1/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.1/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Theme.py` & `Furious-GUI-0.1.1/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Translator.py` & `Furious-GUI-0.1.1/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Utility/Utility.py` & `Furious-GUI-0.1.1/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/Application.py` & `Furious-GUI-0.1.1/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.1/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.1/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.1/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.1/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.1/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.1/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/Widget/Widget.py` & `Furious-GUI-0.1.1/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/__main__.py` & `Furious-GUI-0.1.1/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/data/font/CascadiaMono` & `Furious-GUI-0.1.1/Furious/data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.1/Furious/data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/data/hysteria/country.mmdb` & `Furious-GUI-0.1.1/Furious/data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/data/xray/geoip.dat` & `Furious-GUI-0.1.1/Furious/data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious/data/xray/geosite.dat` & `Furious-GUI-0.1.1/Furious/data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.1/Furious_GUI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -64,17 +64,17 @@
 
 ![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
 
 ![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
 
 ## Install
 
-> Note: Due to better binary files compatibility on Windows, if you are Windows user, you can skip this section and
-> download zip file in the release page that contains pre-built binaries. Otherwise you need to follow the instructions
-> below.
+> Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
+> download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
+> pre-built binaries. Otherwise you need to follow the instructions below.
 
 ### Core Building Tools
 
 > Note: These steps are the same in [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
 > or [hysteria-python](https://github.com/LorenEteval/hysteria-python) *Core Building Tools* steps.
 
 As mentioned above, cores are shipped as Python bindings to support cross-platform running. So to install Furious you
```

### Comparing `Furious-GUI-0.1.0/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.1/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/LICENSE` & `Furious-GUI-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.0/PKG-INFO` & `Furious-GUI-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -64,17 +64,17 @@
 
 ![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
 
 ![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
 
 ## Install
 
-> Note: Due to better binary files compatibility on Windows, if you are Windows user, you can skip this section and
-> download zip file in the release page that contains pre-built binaries. Otherwise you need to follow the instructions
-> below.
+> Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
+> download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
+> pre-built binaries. Otherwise you need to follow the instructions below.
 
 ### Core Building Tools
 
 > Note: These steps are the same in [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
 > or [hysteria-python](https://github.com/LorenEteval/hysteria-python) *Core Building Tools* steps.
 
 As mentioned above, cores are shipped as Python bindings to support cross-platform running. So to install Furious you
```

### Comparing `Furious-GUI-0.1.0/README.md` & `Furious-GUI-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
 ![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
 
 ![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
 
 ## Install
 
-> Note: Due to better binary files compatibility on Windows, if you are Windows user, you can skip this section and
-> download zip file in the release page that contains pre-built binaries. Otherwise you need to follow the instructions
-> below.
+> Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
+> download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
+> pre-built binaries. Otherwise you need to follow the instructions below.
 
 ### Core Building Tools
 
 > Note: These steps are the same in [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
 > or [hysteria-python](https://github.com/LorenEteval/hysteria-python) *Core Building Tools* steps.
 
 As mentioned above, cores are shipped as Python bindings to support cross-platform running. So to install Furious you
```

### Comparing `Furious-GUI-0.1.0/setup.py` & `Furious-GUI-0.1.1/setup.py`

 * *Files identical despite different names*

