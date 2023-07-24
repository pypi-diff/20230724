# Comparing `tmp/resotolib-3.6.3.tar.gz` & `tmp/resotolib-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.6.3.tar", last modified: Mon Jul 24 12:21:04 2023, max compression
+gzip compressed data, was "resotolib-3.6.4.tar", last modified: Mon Jul 24 18:36:20 2023, max compression
```

## Comparing `resotolib-3.6.3.tar` & `resotolib-3.6.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.731754 resotolib-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 12:14:15.000000 resotolib-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 12:21:04.731754 resotolib-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 12:14:15.000000 resotolib-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 12:14:15.000000 resotolib-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.711754 resotolib-3.6.3/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.711754 resotolib-3.6.3/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.715754 resotolib-3.6.3/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.715754 resotolib-3.6.3/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.715754 resotolib-3.6.3/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.715754 resotolib-3.6.3/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23779 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.715754 resotolib-3.6.3/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.723754 resotolib-3.6.3/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-24 12:14:15.000000 resotolib-3.6.3/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.711754 resotolib-3.6.3/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 12:21:04.000000 resotolib-3.6.3/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-24 12:21:04.000000 resotolib-3.6.3/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:21:04.000000 resotolib-3.6.3/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:15:38.000000 resotolib-3.6.3/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 12:21:04.000000 resotolib-3.6.3/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 12:21:04.000000 resotolib-3.6.3/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 12:21:04.731754 resotolib-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:21:04.731754 resotolib-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 12:14:15.000000 resotolib-3.6.3/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.822485 resotolib-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 18:30:36.000000 resotolib-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 18:36:20.822485 resotolib-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 18:30:36.000000 resotolib-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 18:30:36.000000 resotolib-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.810484 resotolib-3.6.4/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23779 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.810484 resotolib-3.6.4/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.814484 resotolib-3.6.4/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:45.000000 resotolib-3.6.4/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 18:36:20.822485 resotolib-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.822485 resotolib-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_x509.py
```

### Comparing `resotolib-3.6.3/PKG-INFO` & `resotolib-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.3/README.md` & `resotolib-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/pyproject.toml` & `resotolib-3.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotolib"
-version = "3.6.3"
+version = "3.6.4"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto common library."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
```

### Comparing `resotolib-3.6.3/resotolib/args.py` & `resotolib-3.6.4/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/asynchronous/utils.py` & `resotolib-3.6.4/resotolib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/asynchronous/web/auth.py` & `resotolib-3.6.4/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/asynchronous/web/runner.py` & `resotolib-3.6.4/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.6.4/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/baseplugin.py` & `resotolib-3.6.4/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/baseresources.py` & `resotolib-3.6.4/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/config.py` & `resotolib-3.6.4/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/__init__.py` & `resotolib-3.6.4/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/actions.py` & `resotolib-3.6.4/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/ca.py` & `resotolib-3.6.4/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/config.py` & `resotolib-3.6.4/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/custom_command.py` & `resotolib-3.6.4/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/events.py` & `resotolib-3.6.4/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/model_check.py` & `resotolib-3.6.4/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/model_export.py` & `resotolib-3.6.4/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/progress.py` & `resotolib-3.6.4/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/search.py` & `resotolib-3.6.4/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/core/tasks.py` & `resotolib-3.6.4/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/durations.py` & `resotolib-3.6.4/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/event.py` & `resotolib-3.6.4/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/graph/__init__.py` & `resotolib-3.6.4/resotolib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/graph/graph_extensions.py` & `resotolib-3.6.4/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/json.py` & `resotolib-3.6.4/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/json_bender.py` & `resotolib-3.6.4/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/jwt.py` & `resotolib-3.6.4/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/lock.py` & `resotolib-3.6.4/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/logger.py` & `resotolib-3.6.4/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/parse_util.py` & `resotolib-3.6.4/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/proc.py` & `resotolib-3.6.4/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/threading.py` & `resotolib-3.6.4/resotolib/threading.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/tree.py` & `resotolib-3.6.4/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/utils.py` & `resotolib-3.6.4/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/__init__.py` & `resotolib-3.6.4/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/metrics.py` & `resotolib-3.6.4/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.6.4/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.6.4/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.6.4/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/favicon-16x16.png` & `resotolib-3.6.4/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/favicon-32x32.png` & `resotolib-3.6.4/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/index.html` & `resotolib-3.6.4/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/mstile-150x150.png` & `resotolib-3.6.4/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/web/static/picnic.min.css` & `resotolib-3.6.4/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib/x509.py` & `resotolib-3.6.4/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/resotolib.egg-info/PKG-INFO` & `resotolib-3.6.4/resotolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.3/resotolib.egg-info/SOURCES.txt` & `resotolib-3.6.4/resotolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_args.py` & `resotolib-3.6.4/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_baseresources.py` & `resotolib-3.6.4/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_config.py` & `resotolib-3.6.4/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_graph.py` & `resotolib-3.6.4/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_graph_extensions.py` & `resotolib-3.6.4/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_json.py` & `resotolib-3.6.4/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_jwt.py` & `resotolib-3.6.4/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_plugin.py` & `resotolib-3.6.4/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_tree.py` & `resotolib-3.6.4/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_utils.py` & `resotolib-3.6.4/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_web.py` & `resotolib-3.6.4/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.3/test/test_x509.py` & `resotolib-3.6.4/test/test_x509.py`

 * *Files identical despite different names*

