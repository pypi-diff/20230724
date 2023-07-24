# Comparing `tmp/maestral-qt-1.8.0.dev0.tar.gz` & `tmp/maestral-qt-1.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-qt-1.8.0.dev0.tar", last modified: Sat Jul 22 15:41:37 2023, max compression
+gzip compressed data, was "maestral-qt-1.8.0.dev1.tar", last modified: Mon Jul 24 20:03:19 2023, max compression
```

## Comparing `maestral-qt-1.8.0.dev0.tar` & `maestral-qt-1.8.0.dev1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.237187 maestral-qt-1.8.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-22 15:41:37.237187 maestral-qt-1.8.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-22 15:41:37.237187 maestral-qt-1.8.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.217186 maestral-qt-1.8.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.225186 maestral-qt-1.8.0.dev0/src/maestral_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.229187 maestral-qt-1.8.0.dev0/src/maestral_qt/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/__pyinstaller/hook-maestral_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/activity_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/autostart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/bandwidth_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/dropbox_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    20646 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/relink_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.237187 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   204933 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/faceholder.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/file
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral.desktop
--rw-r--r--   0 runner    (1001) docker     (123)   842667 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral.icns
--rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-disconnected-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-error-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-error-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-idle-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-idle-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-info-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-info-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-paused-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-paused-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-syncing-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-syncing-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_bandwidth_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_dropbox_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_relink_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_selective_sync_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_settings_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_setup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_event_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_issue_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_issues_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_unlink_dialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20745 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/selective_sync_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/setup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/sync_issues_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21721 2023-07-22 15:41:23.000000 maestral-qt-1.8.0.dev0/src/maestral_qt/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:41:37.229187 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 15:41:37.000000 maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.208333 maestral-qt-1.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-24 20:03:19.208333 maestral-qt-1.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-24 20:03:19.208333 maestral-qt-1.8.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.196332 maestral-qt-1.8.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.200332 maestral-qt-1.8.0.dev1/src/maestral_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.200332 maestral-qt-1.8.0.dev1/src/maestral_qt/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/__pyinstaller/hook-maestral_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/activity_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/bandwidth_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/dropbox_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20646 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/relink_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.204332 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204933 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/faceholder.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/file
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)   842667 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-disconnected-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-error-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-error-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-idle-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-idle-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-info-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-info-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-paused-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-paused-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-syncing-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-syncing-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_bandwidth_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_dropbox_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_relink_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_selective_sync_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_setup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_event_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_issue_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_issues_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_unlink_dialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20745 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/selective_sync_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/setup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/sync_issues_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21721 2023-07-24 20:03:01.000000 maestral-qt-1.8.0.dev1/src/maestral_qt/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:03:19.200332 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 20:03:19.000000 maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/top_level.txt
```

### Comparing `maestral-qt-1.8.0.dev0/LICENSE.txt` & `maestral-qt-1.8.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/PKG-INFO` & `maestral-qt-1.8.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-qt
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: A Qt GUI for the Maestral daemon
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `maestral-qt-1.8.0.dev0/setup.cfg` & `maestral-qt-1.8.0.dev1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = maestral-qt
-version = 1.8.0.dev0
+version = 1.8.0.dev1
 author = Sam Schott
 author_email = sam.schott@outlook.com
 license = MIT
 description = A Qt GUI for the Maestral daemon
 url = https://maestral.app
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,15 +24,15 @@
 packages = find:
 package_dir = 
 	= src
 zip_safe = False
 setup_requires = wheel
 install_requires = 
 	click>=7.1.1
-	maestral>=1.8.0.dev0
+	maestral>=1.8.0.dev1
 	markdown2
 	packaging
 	PyQt6
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
```

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/activity_window.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/activity_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/autostart.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/bandwidth_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/bandwidth_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/dropbox_location_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/dropbox_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/main.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/main.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/relink_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/relink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/__init__.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # -*- coding: utf-8 -*-
 
 import os
 import os.path as osp
 import platform
-from importlib.resources import path
 
 from PyQt6 import QtWidgets, QtCore, QtGui
 
-_icon_provider = QtWidgets.QFileIconProvider()
-_tmp_file_for_ext = dict()
+try:
+    from importlib.resources import as_file, files  # type: ignore
+
+    def resource_path(resource: str) -> str:
+        return str(files("maestral_qt.resources") / resource)
 
+except ImportError:
+    from importlib.resources import path
 
-def resource_path(name):
-    """Returns the resource path as a string. Extracts the resource if necessary."""
-    return str(path("maestral_qt.resources", name).__enter__())
+    def resource_path(resource: str) -> str:
+        return str(path("maestral_qt.resources", resource).__enter__())
+
+_icon_provider = QtWidgets.QFileIconProvider()
+_tmp_file_for_ext = dict()
 
 
 APP_ICON_PATH = resource_path("maestral.png")
 FACEHOLDER_PATH = resource_path("faceholder.png")
 
 THEME_DARK = "dark"
 THEME_LIGHT = "light"
```

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/faceholder.png` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/faceholder.png`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral.icns` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral.icns`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral.png` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-disconnected-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-disconnected-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-error-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-error-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-error-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-error-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-idle-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-idle-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-idle-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-idle-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-info-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-info-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-info-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-info-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-paused-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-paused-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-paused-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-paused-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-syncing-dark.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-syncing-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/maestral_tray-syncing-light.svg` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/maestral_tray-syncing-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_bandwidth_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_bandwidth_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_dropbox_location_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_dropbox_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_relink_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_relink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_selective_sync_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_selective_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_settings_window.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_settings_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_setup_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_setup_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_event_widget.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_event_widget.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_issue_widget.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_issue_widget.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_sync_issues_window.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_sync_issues_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/resources/ui_unlink_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/resources/ui_unlink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/selective_sync_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/selective_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/settings_window.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/settings_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/setup_dialog.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/setup_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/sync_issues_window.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/sync_issues_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/utils.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/utils.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt/widgets.py` & `maestral-qt-1.8.0.dev1/src/maestral_qt/widgets.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/PKG-INFO` & `maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-qt
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: A Qt GUI for the Maestral daemon
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `maestral-qt-1.8.0.dev0/src/maestral_qt.egg-info/SOURCES.txt` & `maestral-qt-1.8.0.dev1/src/maestral_qt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

