# Comparing `tmp/wagtail-purge-0.2.0.tar.gz` & `tmp/wagtail-purge-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-purge-0.2.0.tar", last modified: Thu Jun 16 15:17:45 2022, max compression
+gzip compressed data, was "wagtail-purge-0.3.0.tar", last modified: Mon Jul 24 15:36:04 2023, max compression
```

## Comparing `wagtail-purge-0.2.0.tar` & `wagtail-purge-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/wagtail_purge/
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/wagtail_purge/templates/
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      929 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/wagtail_purge/templates/index.html
--rw-rw-r--   0 alexb     (1000) alexb     (1000)        0 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/wagtail_purge/__init__.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      212 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/wagtail_purge/admin_urls.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      100 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/wagtail_purge/apps.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      929 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/wagtail_purge/views.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      591 2022-06-16 15:10:07.000000 wagtail-purge-0.2.0/wagtail_purge/wagtail_hooks.py
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     1407 2022-06-16 15:17:44.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/PKG-INFO
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      446 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/SOURCES.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)        1 2022-06-16 15:17:44.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/dependency_links.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)        1 2022-01-24 16:35:51.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/not-zip-safe
--rw-rw-r--   0 alexb     (1000) alexb     (1000)       31 2022-06-16 15:17:44.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/requires.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)       14 2022-06-16 15:17:44.000000 wagtail-purge-0.2.0/wagtail_purge.egg-info/top_level.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      417 2022-06-16 15:11:43.000000 wagtail-purge-0.2.0/CHANGELOG.md
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     1066 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/LICENSE
--rw-rw-r--   0 alexb     (1000) alexb     (1000)       91 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/MANIFEST.in
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      534 2022-01-18 15:49:56.000000 wagtail-purge-0.2.0/README.md
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      108 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/setup.cfg
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     1135 2022-06-16 15:11:04.000000 wagtail-purge-0.2.0/setup.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     1407 2022-06-16 15:17:45.000000 wagtail-purge-0.2.0/PKG-INFO
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-24 15:36:04.021978 wagtail-purge-0.3.0/
+-rw-r--r--   0 nick       (502) staff       (20)      637 2023-07-24 15:27:10.000000 wagtail-purge-0.3.0/CHANGELOG.md
+-rw-r--r--   0 nick       (502) staff       (20)     1066 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/LICENSE
+-rw-r--r--   0 nick       (502) staff       (20)       91 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/MANIFEST.in
+-rw-r--r--   0 nick       (502) staff       (20)     1642 2023-07-24 15:36:04.022244 wagtail-purge-0.3.0/PKG-INFO
+-rw-r--r--   0 nick       (502) staff       (20)      534 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/README.md
+-rw-r--r--   0 nick       (502) staff       (20)      108 2023-07-24 15:36:04.022929 wagtail-purge-0.3.0/setup.cfg
+-rw-r--r--   0 nick       (502) staff       (20)     1428 2023-07-24 15:29:39.000000 wagtail-purge-0.3.0/setup.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-24 15:36:04.019883 wagtail-purge-0.3.0/wagtail_purge/
+-rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/__init__.py
+-rw-r--r--   0 nick       (502) staff       (20)      111 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/admin_urls.py
+-rw-r--r--   0 nick       (502) staff       (20)      100 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/apps.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-24 15:36:04.021383 wagtail-purge-0.3.0/wagtail_purge/templates/
+-rw-r--r--   0 nick       (502) staff       (20)      929 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/templates/index.html
+-rw-r--r--   0 nick       (502) staff       (20)      929 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/views.py
+-rw-r--r--   0 nick       (502) staff       (20)      515 2023-07-24 15:23:36.000000 wagtail-purge-0.3.0/wagtail_purge/wagtail_hooks.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-24 15:36:04.021020 wagtail-purge-0.3.0/wagtail_purge.egg-info/
+-rw-r--r--   0 nick       (502) staff       (20)     1642 2023-07-24 15:36:03.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (502) staff       (20)      446 2023-07-24 15:36:03.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (502) staff       (20)        1 2023-07-24 15:36:03.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (502) staff       (20)        1 2023-07-24 15:34:29.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/not-zip-safe
+-rw-r--r--   0 nick       (502) staff       (20)       18 2023-07-24 15:36:03.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/requires.txt
+-rw-r--r--   0 nick       (502) staff       (20)       14 2023-07-24 15:36:03.000000 wagtail-purge-0.3.0/wagtail_purge.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtail-purge-0.2.0/wagtail_purge/templates/index.html` & `wagtail-purge-0.3.0/wagtail_purge/templates/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-purge-0.2.0/wagtail_purge/views.py` & `wagtail-purge-0.3.0/wagtail_purge/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-purge-0.2.0/wagtail_purge/wagtail_hooks.py` & `wagtail-purge-0.3.0/wagtail_purge/wagtail_hooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-try:
-    from wagtail import hooks
-except ImportError:
-    # Wagtail<3.0
-    from wagtail.core import hooks
-from wagtail.admin.menu import AdminOnlyMenuItem
 from django.urls import include, reverse, path
-from . import admin_urls
+from wagtail.admin.menu import AdminOnlyMenuItem
 
+from wagtail import hooks
+    
+from . import admin_urls
 
 @hooks.register("register_admin_urls")
 def register_admin_urls():
     return [
         path(r"purge/", include(admin_urls)),
     ]
 
@@ -18,8 +15,8 @@
 @hooks.register("register_settings_menu_item")
 def register_purge_menu_item():
     return AdminOnlyMenuItem(
         "CDN purge",
         reverse("purge"),
         classnames="icon icon-collapse-down",
         order=1000,
-    )
+    )
```

### Comparing `wagtail-purge-0.2.0/wagtail_purge.egg-info/PKG-INFO` & `wagtail-purge-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-purge
-Version: 0.2.0
+Version: 0.3.0
 Summary: Purge individual URLs from the Wagtail admin
-Home-page: https://github.com/tomdyson/wagtail-purge
+Home-page: https://github.com/torchbox/wagtail-purge
 Author: Tom Dyson
 Author-email: tom+wagtailpurge@torchbox.com
 License: MIT
-Description: # Wagtail Purge
-        
-        A simple admin UI for removing individual pages from your CDN's cache. Assumes that your Wagtail site has already been configured with [frontend cache invalidation](https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html).
-        
-        ## Instructions
-        
-        1. Install this app with `pip install wagtail-purge`
-        2. Add `"wagtail_purge"` to your `INSTALLED_APPS`
-        3. Visit 'CDN purge' in your admin settings menu
-        
-        ![wagtail-purge screenshot](https://raw.githubusercontent.com/tomdyson/wagtail-purge/main/wagtail-purge.png)
 Keywords: development
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wagtail Purge
+
+A simple admin UI for removing individual pages from your CDN's cache. Assumes that your Wagtail site has already been configured with [frontend cache invalidation](https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html).
+
+## Instructions
+
+1. Install this app with `pip install wagtail-purge`
+2. Add `"wagtail_purge"` to your `INSTALLED_APPS`
+3. Visit 'CDN purge' in your admin settings menu
+
+![wagtail-purge screenshot](https://raw.githubusercontent.com/tomdyson/wagtail-purge/main/wagtail-purge.png)
```

### Comparing `wagtail-purge-0.2.0/LICENSE` & `wagtail-purge-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-purge-0.2.0/README.md` & `wagtail-purge-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-purge-0.2.0/setup.py` & `wagtail-purge-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="wagtail-purge",
-    version="0.2.0",
+    version="0.3.0",
     description="Purge individual URLs from the Wagtail admin",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/tomdyson/wagtail-purge",
+    url="https://github.com/torchbox/wagtail-purge",
     author="Tom Dyson",
     author_email="tom+wagtailpurge@torchbox.com",
     license="MIT",
     classifiers=[
         "Environment :: Web Environment",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 2",
-        "Framework :: Wagtail :: 3",
+        "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     keywords="development",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "wagtail>=2.15",
-        "django>=3.0,<4.0"
+        "wagtail>=4.1,<6.0",
     ],
 )
```

### Comparing `wagtail-purge-0.2.0/PKG-INFO` & `wagtail-purge-0.3.0/wagtail_purge.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-purge
-Version: 0.2.0
+Version: 0.3.0
 Summary: Purge individual URLs from the Wagtail admin
-Home-page: https://github.com/tomdyson/wagtail-purge
+Home-page: https://github.com/torchbox/wagtail-purge
 Author: Tom Dyson
 Author-email: tom+wagtailpurge@torchbox.com
 License: MIT
-Description: # Wagtail Purge
-        
-        A simple admin UI for removing individual pages from your CDN's cache. Assumes that your Wagtail site has already been configured with [frontend cache invalidation](https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html).
-        
-        ## Instructions
-        
-        1. Install this app with `pip install wagtail-purge`
-        2. Add `"wagtail_purge"` to your `INSTALLED_APPS`
-        3. Visit 'CDN purge' in your admin settings menu
-        
-        ![wagtail-purge screenshot](https://raw.githubusercontent.com/tomdyson/wagtail-purge/main/wagtail-purge.png)
 Keywords: development
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wagtail Purge
+
+A simple admin UI for removing individual pages from your CDN's cache. Assumes that your Wagtail site has already been configured with [frontend cache invalidation](https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html).
+
+## Instructions
+
+1. Install this app with `pip install wagtail-purge`
+2. Add `"wagtail_purge"` to your `INSTALLED_APPS`
+3. Visit 'CDN purge' in your admin settings menu
+
+![wagtail-purge screenshot](https://raw.githubusercontent.com/tomdyson/wagtail-purge/main/wagtail-purge.png)
```

