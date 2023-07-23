# Comparing `tmp/gmailsorter-0.1.0.tar.gz` & `tmp/gmailsorter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmailsorter-0.1.0.tar", last modified: Sun Jul  9 23:09:30 2023, max compression
+gzip compressed data, was "gmailsorter-0.1.1.tar", last modified: Sun Jul 23 23:18:45 2023, max compression
```

## Comparing `gmailsorter-0.1.0.tar` & `gmailsorter-0.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.719474 gmailsorter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-09 23:09:30.719474 gmailsorter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.719474 gmailsorter-0.1.0/gmailsorter/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-09 23:09:30.719474 gmailsorter-0.1.0/gmailsorter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.695473 gmailsorter-0.1.0/gmailsorter/base/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/base/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/base/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.695473 gmailsorter-0.1.0/gmailsorter/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/daemon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/daemon/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/daemon/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/daemon/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.699473 gmailsorter-0.1.0/gmailsorter/google/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/google/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/google/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/google/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/google/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.703473 gmailsorter-0.1.0/gmailsorter/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/ml/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/ml/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/ml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.707473 gmailsorter-0.1.0/gmailsorter/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/googleapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.683473 gmailsorter-0.1.0/gmailsorter/webapp/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.707473 gmailsorter-0.1.0/gmailsorter/webapp/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9241 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/css/main.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    83821 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/css/util.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.683473 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.715474 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/
--rwxr-xr-x   0 runner    (1001) docker     (123)   139056 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Black.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   155956 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-BlackItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   141260 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Bold.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   160224 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-BoldItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   140220 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBold.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   158708 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   147952 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLight.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   170912 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   167140 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   146472 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Light.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   168944 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-LightItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   143516 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Medium.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   165512 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-MediumItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   145312 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   142148 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBold.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   161896 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   148976 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Thin.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)   172308 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.715474 gmailsorter-0.1.0/gmailsorter/webapp/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)   114272 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/images/bg-01.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.715474 gmailsorter-0.1.0/gmailsorter/webapp/static/images/icons/
--rwxr-xr-x   0 runner    (1001) docker     (123)    32038 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/static/images/icons/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.715474 gmailsorter-0.1.0/gmailsorter/webapp/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/templates/login.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/templates/user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/gmailsorter/webapp/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.691473 gmailsorter-0.1.0/gmailsorter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/gmailsorter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-09 23:09:30.719474 gmailsorter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-09 23:09:30.000000 gmailsorter-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:09:30.715474 gmailsorter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/tests/test_google_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-09 23:09:27.000000 gmailsorter-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/base/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/base/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/daemon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/daemon/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/daemon/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/daemon/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/google/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/google/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/google/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/google/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/ml/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/ml/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/ml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/googleapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.892754 gmailsorter-0.1.1/gmailsorter/webapp/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.900754 gmailsorter-0.1.1/gmailsorter/webapp/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9241 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/css/main.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83821 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/css/util.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.892754 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   139056 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Black.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   155956 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-BlackItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   141260 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Bold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   160224 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-BoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140220 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   158708 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   147952 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLight.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   170912 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   167140 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   146472 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Light.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   168944 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-LightItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   143516 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Medium.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165512 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-MediumItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   145312 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   142148 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   161896 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   148976 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Thin.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   172308 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/webapp/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114272 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/images/bg-01.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/webapp/static/images/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32038 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/static/images/icons/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/gmailsorter/webapp/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/templates/login.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1864 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/templates/user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/gmailsorter/webapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.896754 gmailsorter-0.1.1/gmailsorter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/gmailsorter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-23 23:18:45.000000 gmailsorter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:18:45.904754 gmailsorter-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/tests/test_google_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-23 23:18:42.000000 gmailsorter-0.1.1/versioneer.py
```

### Comparing `gmailsorter-0.1.0/LICENSE` & `gmailsorter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/__main__.py` & `gmailsorter-0.1.1/gmailsorter/__main__.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/base/database.py` & `gmailsorter-0.1.1/gmailsorter/base/database.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/base/message.py` & `gmailsorter-0.1.1/gmailsorter/base/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,19 @@
         return None
     if email_date.count(",") >= 2:
         email_date = ", ".join(email_date.split(", ")[-2:])
     if email_date[-3:-2].isalpha():
         email_date = " ".join(email_date.split()[:-1])
     if email_date[-1].isalpha():
         email_date = email_date[:-1]
-    if email_date[:3].isalpha() and email_date[-3] != ":":
+    if email_date[:3].isalpha() and email_date[-3] != ":" and email_date[-6] == "_":
+        return datetime.strptime(email_date.split(".")[0], "%a, %d %b %Y %H:%M:%S %z")
+    elif email_date[:3].isalpha() and email_date[-3] != ":" and "(" in email_date:
+        return datetime.strptime(email_date.split(" (")[0], "%a, %d %b %Y %H:%M:%S %z")
+    elif email_date[:3].isalpha() and email_date[-3] != ":":
         return datetime.strptime(email_date, "%a, %d %b %Y %H:%M:%S %z")
     elif email_date[-3] == ":":
         return datetime.strptime(email_date, "%a, %d %b %Y %H:%M:%S")
     elif email_date.count("-") == 2:
         return datetime.strptime(email_date, "%d-%m-%Y")
     else:
         return datetime.strptime(email_date, "%d %b %Y %H:%M:%S %z")
```

### Comparing `gmailsorter-0.1.0/gmailsorter/daemon/__main__.py` & `gmailsorter-0.1.1/gmailsorter/daemon/__main__.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/daemon/daemon.py` & `gmailsorter-0.1.1/gmailsorter/daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/daemon/shared.py` & `gmailsorter-0.1.1/gmailsorter/daemon/shared.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/daemon/tasks.py` & `gmailsorter-0.1.1/gmailsorter/daemon/tasks.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/google/authentication.py` & `gmailsorter-0.1.1/gmailsorter/google/authentication.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/google/database.py` & `gmailsorter-0.1.1/gmailsorter/google/database.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/google/mail.py` & `gmailsorter-0.1.1/gmailsorter/google/mail.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/google/message.py` & `gmailsorter-0.1.1/gmailsorter/google/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return self.text.getvalue()
 
 
 def get_email_dict(message):
     try:
         return Message(message_dict=message).to_dict()
     except ValueError as e:
-        print(message, e.message)
+        print(message, str(e))
         return None
 
 
 class Message(AbstractMessage):
     def __init__(self, message_dict):
         self._message_dict = message_dict
```

### Comparing `gmailsorter-0.1.0/gmailsorter/local.py` & `gmailsorter-0.1.1/gmailsorter/local.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/ml/database.py` & `gmailsorter-0.1.1/gmailsorter/ml/database.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/ml/encoding.py` & `gmailsorter-0.1.1/gmailsorter/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/ml/model.py` & `gmailsorter-0.1.1/gmailsorter/ml/model.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/app.py` & `gmailsorter-0.1.1/gmailsorter/webapp/app.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/config.py` & `gmailsorter-0.1.1/gmailsorter/webapp/config.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/database.py` & `gmailsorter-0.1.1/gmailsorter/webapp/database.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/googleapi.py` & `gmailsorter-0.1.1/gmailsorter/webapp/googleapi.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/css/main.css` & `gmailsorter-0.1.1/gmailsorter/webapp/static/css/main.css`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/css/util.css` & `gmailsorter-0.1.1/gmailsorter/webapp/static/css/util.css`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Black.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-BlackItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Bold.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-BoldItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBold.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLight.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Italic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Light.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-LightItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Medium.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-MediumItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Regular.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBold.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-Thin.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/fonts/poppins/Poppins-ThinItalic.ttf` & `gmailsorter-0.1.1/gmailsorter/webapp/static/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/images/bg-01.jpg` & `gmailsorter-0.1.1/gmailsorter/webapp/static/images/bg-01.jpg`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/static/images/icons/favicon.ico` & `gmailsorter-0.1.1/gmailsorter/webapp/static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/templates/login.html` & `gmailsorter-0.1.1/gmailsorter/webapp/templates/login.html`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/templates/user.html` & `gmailsorter-0.1.1/gmailsorter/webapp/templates/user.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
-	<title>Gmailsorter.com</title>
+	<title>Gmailsorte</title>
 	<meta charset="UTF-8">
 	<meta name="viewport" content="width=device-width, initial-scale=1">
 	<link rel="icon" type="image/png" href="/static/images/icons/favicon.ico"/>
 	<link rel="stylesheet" type="text/css" href="/static/css/util.css">
 	<link rel="stylesheet" type="text/css" href="/static/css/main.css">
 </head>
 <body>
@@ -14,15 +14,15 @@
 		<div class="container-login100" style="background-image: url('/static/images/bg-01.jpg');">
 			<div class="wrap-login100 p-l-55 p-r-55 p-t-65 p-b-54">
                 <span class="login100-form-title p-b-49">
                     Gmailsorter.com
                 </span>
                 Hello, {{ username }}!<br />
                 <br />
-                Status of your Gmailsorter.com account:
+                Status of your Gmailsorter account:
                 <ul>
                     {% for list_item in item_list %}
                     <li>{{ list_item |safe }}</li>
                     {% endfor %}
                 </ul>
                 <br />
                 {% if enable_reset %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
  Gmailsorter.com  Hello, {{ username }}!
 
-Status of your Gmailsorter.com account:
+Status of your Gmailsorter account:
     * {% for list_item in item_list %}
     * {{ list_item |safe }}
     * {% endfor %}
 
 {% if enable_reset %}
  Reset Status
```

### Comparing `gmailsorter-0.1.0/gmailsorter/webapp/user.py` & `gmailsorter-0.1.1/gmailsorter/webapp/user.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/gmailsorter.egg-info/SOURCES.txt` & `gmailsorter-0.1.1/gmailsorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/setup.py` & `gmailsorter-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,25 +23,25 @@
             'webapp/static/fonts/poppins/*.ttf',
             'webapp/static/images/*.jpg',
             'webapp/static/images/icons/*.ico',
             'webapp/templates/*.html'
         ],
     },
     install_requires=[
-        "google-api-python-client>=2.92.0",
-        "google-auth>=2.21.0",
+        "google-api-python-client>=2.94.0",
+        "google-auth>=2.22.0",
         "google-auth-oauthlib>=1.0.0",
         "numpy>=1.25.1",
         "tqdm>=4.65.0",
         "pandas>=2.0.3",
         "scikit-learn>=1.3.0",
-        "sqlalchemy>=2.0.18",
+        "sqlalchemy>=2.0.19",
     ],
     extras_require={
-        "webapp": ['gunicorn>=20.1.0', "flask>=2.3.2", "flask-login>=0.6.2"],
+        "webapp": ['gunicorn>=21.2.0', "flask>=2.3.2", "flask-login>=0.6.2"],
     },
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
             "console_scripts": [
                 'gmailsorter=gmailsorter.__main__:command_line_parser',
                 'gmailsorter-daemon=gmailsorter.daemon.__main__:command_line_parser',
                 'gmailsorter-app=gmailsorter.webapp.app:run_app'
```

### Comparing `gmailsorter-0.1.0/tests/test_database.py` & `gmailsorter-0.1.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/tests/test_google_message.py` & `gmailsorter-0.1.1/tests/test_google_message.py`

 * *Files identical despite different names*

### Comparing `gmailsorter-0.1.0/versioneer.py` & `gmailsorter-0.1.1/versioneer.py`

 * *Files identical despite different names*

