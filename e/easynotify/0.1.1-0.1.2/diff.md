# Comparing `tmp/easynotify-0.1.1.tar.gz` & `tmp/easynotify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easynotify-0.1.1.tar", last modified: Mon Jul 24 02:11:56 2023, max compression
+gzip compressed data, was "easynotify-0.1.2.tar", last modified: Mon Jul 24 02:21:04 2023, max compression
```

## Comparing `easynotify-0.1.1.tar` & `easynotify-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.294006 easynotify-0.1.1/
--rw-rw-rw-   0        0        0     1097 2021-09-26 07:25:25.000000 easynotify-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1025 2023-07-24 02:11:56.293020 easynotify-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-07-24 02:09:01.000000 easynotify-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.276078 easynotify-0.1.1/easynotify/
--rw-rw-rw-   0        0        0      105 2023-07-24 02:11:51.000000 easynotify-0.1.1/easynotify/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-07-24 02:07:05.000000 easynotify-0.1.1/easynotify/easynotify.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.291017 easynotify-0.1.1/easynotify.egg-info/
--rw-rw-rw-   0        0        0     1025 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-24 02:11:56.000000 easynotify-0.1.1/easynotify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 02:11:56.294006 easynotify-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-24 02:11:51.000000 easynotify-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:21:04.399083 easynotify-0.1.2/
+-rw-rw-rw-   0        0        0     1097 2021-09-26 07:25:25.000000 easynotify-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1025 2023-07-24 02:21:04.398085 easynotify-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2023-07-24 02:09:01.000000 easynotify-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 02:21:04.382079 easynotify-0.1.2/easynotify/
+-rw-rw-rw-   0        0        0      105 2023-07-24 02:21:01.000000 easynotify-0.1.2/easynotify/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-07-24 02:19:44.000000 easynotify-0.1.2/easynotify/easynotify.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:21:04.397084 easynotify-0.1.2/easynotify.egg-info/
+-rw-rw-rw-   0        0        0     1025 2023-07-24 02:21:04.000000 easynotify-0.1.2/easynotify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-24 02:21:04.000000 easynotify-0.1.2/easynotify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 02:21:04.000000 easynotify-0.1.2/easynotify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 02:21:04.000000 easynotify-0.1.2/easynotify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 02:21:04.000000 easynotify-0.1.2/easynotify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 02:21:04.400078 easynotify-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-07-24 02:21:01.000000 easynotify-0.1.2/setup.py
```

### Comparing `easynotify-0.1.1/LICENSE` & `easynotify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easynotify-0.1.1/PKG-INFO` & `easynotify-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easynotify
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/CauchyComplete/EasyNotify
 Author: CauchyComplete
 Author-email: corundum240@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easynotify-0.1.1/README.md` & `easynotify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easynotify-0.1.1/easynotify/easynotify.py` & `easynotify-0.1.2/easynotify/easynotify.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,9 +36,10 @@
         if icon_emoji is None:
             payload.pop("icon_emoji")
         if print_also:
             print_username = username if username is not None else "SlackBot"
             print(f"{print_username}: {text}")
 
         # Send POST request
-        requests.post(self.url, json=payload)
+        if self.url is not None:
+            requests.post(self.url, json=payload)
```

### Comparing `easynotify-0.1.1/easynotify.egg-info/PKG-INFO` & `easynotify-0.1.2/easynotify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easynotify
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/CauchyComplete/EasyNotify
 Author: CauchyComplete
 Author-email: corundum240@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easynotify-0.1.1/setup.py` & `easynotify-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='easynotify',
-    version='0.1.1',
+    version='0.1.2',
     descripton='This package allows you to post messages with bots easily.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/CauchyComplete/EasyNotify',
     author='CauchyComplete',
     author_email='corundum240@gmail.com',
     license='MIT',
```

