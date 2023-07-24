# Comparing `tmp/plone.all_in_one_accessibility-1.0a3.tar.gz` & `tmp/plone.all_in_one_accessibility-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.all_in_one_accessibility-1.0a3.tar", last modified: Thu Jul 13 11:00:34 2023, max compression
+gzip compressed data, was "plone.all_in_one_accessibility-1.3.tar", last modified: Mon Jul 24 05:05:01 2023, max compression
```

## Comparing `plone.all_in_one_accessibility-1.0a3.tar` & `plone.all_in_one_accessibility-1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.785874 plone.all_in_one_accessibility-1.0a3/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      118 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/CHANGES.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       92 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/CONTRIBUTORS.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1338 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/DEVELOP.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)    18092 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/LICENSE.GPL
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      688 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/LICENSE.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      115 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/MANIFEST.in
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2209 2023-07-13 11:00:34.785874 plone.all_in_one_accessibility-1.0a3/PKG-INFO
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1220 2023-07-13 09:51:37.000000 plone.all_in_one_accessibility-1.0a3/README.md
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.753874 plone.all_in_one_accessibility-1.0a3/docs/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     8023 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/docs/conf.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      113 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/docs/index.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      340 2023-07-13 11:00:34.785874 plone.all_in_one_accessibility-1.0a3/setup.cfg
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2572 2023-07-13 10:59:53.000000 plone.all_in_one_accessibility-1.0a3/setup.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.741874 plone.all_in_one_accessibility-1.0a3/src/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.753874 plone.all_in_one_accessibility-1.0a3/src/plone/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       80 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.761874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      147 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      304 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      299 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/widget/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/widget/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:53:23.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/widget/configure.zcml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2657 2023-07-13 10:56:02.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/widget/get.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      635 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/overrides/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/overrides/.gitkeep
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.765874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/static/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/static/.gitkeep
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1499 2023-07-13 08:52:27.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.769874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/content/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/content/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2667 2023-07-13 09:49:04.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      276 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/interfaces.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.777874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      611 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/README.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.741874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/en/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.777874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       28 2023-07-13 08:58:49.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.mo
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.po
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/plone.all_in_one_accessibility.pot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1776 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/update.py
--rwxrwxr-x   0 skynet    (1000) skynet    (1000)      527 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/update.sh
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      442 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/permissions.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.741874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.777874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      213 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/browserlayer.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      105 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/catalog.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      319 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/metadata.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.781874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/registry/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      188 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/registry/main.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      371 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/rolemap.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.781874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/types/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3406 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      335 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/types.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.781874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/uninstall/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      140 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      811 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/setuphandlers.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1768 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/testing.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.785874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.785874 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/robot/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3268 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2051 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/robot/test_example.robot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2855 2023-07-13 08:49:35.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      935 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_robot.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2691 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_setup.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 11:00:34.761874 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2209 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3245 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      135 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/entry_points.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/namespace_packages.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 08:53:47.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/not-zip-safe
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      159 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/requires.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 11:00:34.000000 plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/top_level.txt
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      118 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/CHANGES.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       92 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/CONTRIBUTORS.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1338 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/DEVELOP.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)    18092 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/LICENSE.GPL
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      688 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/LICENSE.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      115 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/MANIFEST.in
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2181 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/PKG-INFO
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1194 2023-07-24 05:04:46.000000 plone.all_in_one_accessibility-1.3/README.md
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.136999 plone.all_in_one_accessibility-1.3/docs/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     8023 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/docs/conf.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      113 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/docs/index.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      340 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/setup.cfg
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2570 2023-07-24 05:00:30.000000 plone.all_in_one_accessibility-1.3/setup.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.132999 plone.all_in_one_accessibility-1.3/src/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.136999 plone.all_in_one_accessibility-1.3/src/plone/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       80 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      147 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      304 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      299 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/widget/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/widget/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:53:23.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/widget/configure.zcml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2657 2023-07-13 10:56:02.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/widget/get.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      635 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/overrides/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/overrides/.gitkeep
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/static/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/static/.gitkeep
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1499 2023-07-13 08:52:27.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/content/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/content/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2667 2023-07-13 09:49:04.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      276 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/interfaces.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.140999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      611 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/README.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.132999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/en/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       28 2023-07-13 08:58:49.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.mo
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.po
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/plone.all_in_one_accessibility.pot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1776 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/update.py
+-rwxrwxr-x   0 skynet    (1000) skynet    (1000)      527 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/update.sh
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      442 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/permissions.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.136999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      213 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/browserlayer.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      105 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/catalog.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      319 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/metadata.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/registry/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      188 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/registry/main.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      371 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/rolemap.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/types/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3406 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      335 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/types.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/uninstall/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      140 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      811 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/setuphandlers.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1768 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/testing.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.144999 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/robot/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3268 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2051 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/robot/test_example.robot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2855 2023-07-13 08:49:35.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      935 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_robot.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2691 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_setup.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-24 05:05:01.136999 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2181 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3245 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      135 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/entry_points.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/namespace_packages.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 08:53:47.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/not-zip-safe
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      159 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-24 05:05:01.000000 plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/top_level.txt
```

### Comparing `plone.all_in_one_accessibility-1.0a3/DEVELOP.rst` & `plone.all_in_one_accessibility-1.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/LICENSE.GPL` & `plone.all_in_one_accessibility-1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/LICENSE.rst` & `plone.all_in_one_accessibility-1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/PKG-INFO` & `plone.all_in_one_accessibility-1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.all_in_one_accessibility
-Version: 1.0a3
+Version: 1.3
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/plone.all_in_one_accessibility
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/plone.all_in_one_accessibility/
 Keywords: Python Plone CMS
@@ -21,15 +21,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 # All in One Accessibility
-- All in One Accessibility widget improves plone website ADA compliance and browser experience for WCAG 2.1, ATAG 2.0, ADA, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, and California Unruh standards.
+- All in One Accessibility widget improves plone website ADA compliance and browser experience for ADA, WCAG 2.1, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, California Unruh, Ontario AODA, Canada ACA, German BITV, and France RGAA standards.
 - 2 Minute installation
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your plone website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
@@ -47,9 +47,10 @@
     eggs =
         plone.all_in_one_accessibility
 
 
 and then running ``bin/buildout``
 
 
-.. Call API in frontend footer component and create a dynamic script tag 
+
+
```

### Comparing `plone.all_in_one_accessibility-1.0a3/README.md` & `plone.all_in_one_accessibility-1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # All in One Accessibility
-- All in One Accessibility widget improves plone website ADA compliance and browser experience for WCAG 2.1, ATAG 2.0, ADA, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, and California Unruh standards.
+- All in One Accessibility widget improves plone website ADA compliance and browser experience for ADA, WCAG 2.1, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, California Unruh, Ontario AODA, Canada ACA, German BITV, and France RGAA standards.
 - 2 Minute installation
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your plone website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
@@ -21,9 +21,10 @@
     eggs =
         plone.all_in_one_accessibility
 
 
 and then running ``bin/buildout``
 
 
-.. Call API in frontend footer component and create a dynamic script tag 
+
+
```

### Comparing `plone.all_in_one_accessibility-1.0a3/docs/conf.py` & `plone.all_in_one_accessibility-1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/setup.py` & `plone.all_in_one_accessibility-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # open('CONTRIBUTORS.rst').read(),
     # open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='plone.all_in_one_accessibility',
-    version='1.0a3',
+    version='1.3',
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/api/services/widget/get.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/api/services/widget/get.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/browser/configure.zcml` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/configure.zcml` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/README.rst` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/README.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/update.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/update.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/locales/update.sh` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/locales/update.sh`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/setuphandlers.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/testing.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/testing.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/robot/test_example.robot` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_robot.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone/all_in_one_accessibility/tests/test_setup.py` & `plone.all_in_one_accessibility-1.3/src/plone/all_in_one_accessibility/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/PKG-INFO` & `plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.all-in-one-accessibility
-Version: 1.0a3
+Version: 1.3
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/plone.all_in_one_accessibility
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/plone.all_in_one_accessibility/
 Keywords: Python Plone CMS
@@ -21,15 +21,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 # All in One Accessibility
-- All in One Accessibility widget improves plone website ADA compliance and browser experience for WCAG 2.1, ATAG 2.0, ADA, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, and California Unruh standards.
+- All in One Accessibility widget improves plone website ADA compliance and browser experience for ADA, WCAG 2.1, Section 508, Australian DDA, European EAA EN 301 549, UK Equality Act (EA), Israeli Standard 5568, California Unruh, Ontario AODA, Canada ACA, German BITV, and France RGAA standards.
 - 2 Minute installation
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your plone website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
@@ -47,9 +47,10 @@
     eggs =
         plone.all_in_one_accessibility
 
 
 and then running ``bin/buildout``
 
 
-.. Call API in frontend footer component and create a dynamic script tag 
+
+
```

### Comparing `plone.all_in_one_accessibility-1.0a3/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt` & `plone.all_in_one_accessibility-1.3/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

