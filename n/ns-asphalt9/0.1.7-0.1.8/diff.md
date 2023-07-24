# Comparing `tmp/ns_asphalt9-0.1.7.tar.gz` & `tmp/ns_asphalt9-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.1.7.tar", last modified: Mon Jul 24 10:41:19 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.1.8.tar", last modified: Mon Jul 24 10:57:11 2023, max compression
```

## Comparing `ns_asphalt9-0.1.7.tar` & `ns_asphalt9-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.839697 ns_asphalt9-0.1.7/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 10:41:19.000000 ns_asphalt9-0.1.7/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 10:41:19.847697 ns_asphalt9-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:41:19.843697 ns_asphalt9-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 10:41:06.000000 ns_asphalt9-0.1.7/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.650570 ns_asphalt9-0.1.8/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 10:57:11.658570 ns_asphalt9-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/tests/test_pages.py
```

### Comparing `ns_asphalt9-0.1.7/LICENSE` & `ns_asphalt9-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/PKG-INFO` & `ns_asphalt9-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.7/README.md` & `ns_asphalt9-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/process_race.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,15 @@
                 break
         else:
             page = ocr.OCR.get_page()
             if page.name == consts.loading_race:
                 track = ocr.OCR.get_track()
                 if track:
                     logger.info(f"Current track is {track['trackcn']}")
-            if page.name in [
-                consts.race_score,
-                consts.race_results,
-                consts.race_reward,
-                consts.system_error,
-                consts.connect_error,
-                consts.no_connection,
-            ]:
+            if ocr.OCR.has_next():
                 break
 
         pro.press_button(Buttons.Y, 0.7)
         pro.press_button(Buttons.Y, 0)
 
     globals.FINISHED_COUNT += 1
     logger.info(f"Already finished {globals.FINISHED_COUNT} times loop count = {i}.")
```

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9/main.py` & `ns_asphalt9-0.1.8/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.8/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.7/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.8/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.7/setup.cfg` & `ns_asphalt9-0.1.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.7
+version = 0.1.8
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.1.7/tests/test_pages.py` & `ns_asphalt9-0.1.8/tests/test_pages.py`

 * *Files identical despite different names*

