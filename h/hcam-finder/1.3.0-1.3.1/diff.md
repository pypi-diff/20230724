# Comparing `tmp/hcam_finder-1.3.0.tar.gz` & `tmp/hcam_finder-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_finder-1.3.0.tar", last modified: Fri Jul 21 10:55:37 2023, max compression
+gzip compressed data, was "hcam_finder-1.3.1.tar", last modified: Mon Jul 24 09:58:09 2023, max compression
```

## Comparing `hcam_finder-1.3.0.tar` & `hcam_finder-1.3.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.992409 hcam_finder-1.3.0/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.0/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-21 10:55:37.992471 hcam_finder-1.3.0/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.0/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.982507 hcam_finder-1.3.0/docs/
--rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/docs/Makefile
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.977881 hcam_finder-1.3.0/docs/_build/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.977979 hcam_finder-1.3.0/docs/_build/html/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.984081 hcam_finder-1.3.0/docs/_build/html/_images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.0/docs/_build/html/_images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/_build/html/_images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/_build/html/_images/main.png
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.984988 hcam_finder-1.3.0/docs/_build/html/_static/
--rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/file.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.0/docs/conf.py
--rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.0/docs/hcam_finder.rst
--rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/hipercam.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.986633 hcam_finder-1.3.0/docs/images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/images/main.png
--rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/index.rst
--rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/docs/make.bat
--rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.0/docs/modules.rst
--rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/ultracam.rst
--rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/ultraspec.rst
--rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/usage.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.989370 hcam_finder-1.3.0/hcam_finder/
--rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-21 10:55:19.000000 hcam_finder-1.3.0/hcam_finder/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/hcam_finder/config.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.991276 hcam_finder-1.3.0/hcam_finder/data/
--rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.0/hcam_finder/data/Lato-Black.ttf
--rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.0/hcam_finder/data/Lato-Regular.ttf
--rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.0/hcam_finder/data/README.rst
--rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/data/config
--rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/data/configspec.ini
--rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.0/hcam_finder/data/guider_hole_arcseconds.txt
--rw-r--r--   0 sl         (501) staff       (20)    21032 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/hcam_finder/finders.py
--rw-r--r--   0 sl         (501) staff       (20)     2632 2022-02-01 09:58:21.000000 hcam_finder-1.3.0/hcam_finder/finding_chart.py
--rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/hcam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.0/hcam_finder/panstarrs.py
--rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/shapes.py
--rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.0/hcam_finder/skyview.py
--rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.0/hcam_finder/ucam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/hcam_finder/uspec_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.0/hcam_finder/ztf.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.990022 hcam_finder-1.3.0/hcam_finder.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.991850 hcam_finder-1.3.0/scripts/
--rw-r--r--   0 sl         (501) staff       (20)    12564 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/hfinder
--rw-r--r--   0 sl         (501) staff       (20)    10866 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/ufinder
--rw-r--r--   0 sl         (501) staff       (20)    11371 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/usfinder
--rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-21 10:55:37.992703 hcam_finder-1.3.0/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-21 10:55:19.000000 hcam_finder-1.3.0/setup.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.992182 hcam_finder-1.3.0/tests/
--rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/tests/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/tests/test_hcam_finder.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710476 hcam_finder-1.3.1/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.1/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 09:58:09.710556 hcam_finder-1.3.1/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.1/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.698781 hcam_finder-1.3.1/docs/
+-rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/docs/Makefile
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.692906 hcam_finder-1.3.1/docs/_build/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.693240 hcam_finder-1.3.1/docs/_build/html/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.700598 hcam_finder-1.3.1/docs/_build/html/_images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.1/docs/_build/html/_images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/_build/html/_images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/_build/html/_images/main.png
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.702165 hcam_finder-1.3.1/docs/_build/html/_static/
+-rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/plus.png
+-rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.1/docs/conf.py
+-rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.1/docs/hcam_finder.rst
+-rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/hipercam.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.704509 hcam_finder-1.3.1/docs/images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/images/main.png
+-rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/index.rst
+-rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/docs/make.bat
+-rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.1/docs/modules.rst
+-rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/ultracam.rst
+-rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/ultraspec.rst
+-rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/usage.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.706526 hcam_finder-1.3.1/hcam_finder/
+-rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-24 09:57:47.000000 hcam_finder-1.3.1/hcam_finder/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/hcam_finder/config.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.709484 hcam_finder-1.3.1/hcam_finder/data/
+-rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.1/hcam_finder/data/Lato-Black.ttf
+-rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.1/hcam_finder/data/Lato-Regular.ttf
+-rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.1/hcam_finder/data/README.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/data/config
+-rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/data/configspec.ini
+-rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.1/hcam_finder/data/guider_hole_arcseconds.txt
+-rw-r--r--   0 sl         (501) staff       (20)    21032 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/hcam_finder/finders.py
+-rw-r--r--   0 sl         (501) staff       (20)     2802 2023-07-24 09:57:08.000000 hcam_finder-1.3.1/hcam_finder/finding_chart.py
+-rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/hcam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.1/hcam_finder/panstarrs.py
+-rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/shapes.py
+-rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.1/hcam_finder/skyview.py
+-rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.1/hcam_finder/ucam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/hcam_finder/uspec_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.1/hcam_finder/ztf.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.707268 hcam_finder-1.3.1/hcam_finder.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710107 hcam_finder-1.3.1/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)    12564 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/hfinder
+-rw-r--r--   0 sl         (501) staff       (20)    10866 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/ufinder
+-rw-r--r--   0 sl         (501) staff       (20)    11371 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/usfinder
+-rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-24 09:58:09.710830 hcam_finder-1.3.1/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-24 09:57:47.000000 hcam_finder-1.3.1/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710363 hcam_finder-1.3.1/tests/
+-rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/tests/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/tests/test_hcam_finder.py
```

### Comparing `hcam_finder-1.3.0/CONTRIBUTING.rst` & `hcam_finder-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/LICENSE` & `hcam_finder-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/PKG-INFO` & `hcam_finder-1.3.1/hcam_finder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: hcam_finder
-Version: 1.3.0
+Name: hcam-finder
+Version: 1.3.1
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.0/README.rst` & `hcam_finder-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/Makefile` & `hcam_finder-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/_build/html/_images/compo.png` & `hcam_finder-1.3.1/docs/_build/html/_images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/_build/html/_images/inst.png` & `hcam_finder-1.3.1/docs/_build/html/_images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/_build/html/_images/main.png` & `hcam_finder-1.3.1/docs/_build/html/_images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/conf.py` & `hcam_finder-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/hcam_finder.rst` & `hcam_finder-1.3.1/docs/hcam_finder.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/hipercam.rst` & `hcam_finder-1.3.1/docs/hipercam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/images/compo.png` & `hcam_finder-1.3.1/docs/images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/images/inst.png` & `hcam_finder-1.3.1/docs/images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/images/main.png` & `hcam_finder-1.3.1/docs/images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/make.bat` & `hcam_finder-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/ultracam.rst` & `hcam_finder-1.3.1/docs/ultracam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/docs/usage.rst` & `hcam_finder-1.3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/config.py` & `hcam_finder-1.3.1/hcam_finder/config.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/data/Lato-Black.ttf` & `hcam_finder-1.3.1/hcam_finder/data/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/data/Lato-Regular.ttf` & `hcam_finder-1.3.1/hcam_finder/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/data/config` & `hcam_finder-1.3.1/hcam_finder/data/config`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/data/configspec.ini` & `hcam_finder-1.3.1/hcam_finder/data/configspec.ini`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/data/guider_hole_arcseconds.txt` & `hcam_finder-1.3.1/hcam_finder/data/guider_hole_arcseconds.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/finders.py` & `hcam_finder-1.3.1/hcam_finder/finders.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/finding_chart.py` & `hcam_finder-1.3.1/hcam_finder/finding_chart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, absolute_import, unicode_literals, division
 import pkg_resources
 import six
 from os.path import expanduser
+
 if not six.PY3:
     import tkFileDialog as filedialog
 else:
     from tkinter import filedialog
 
 from . import __version__ as version
 
@@ -28,53 +29,68 @@
 
 def make_finder(logger, img_array, object_name, tel, ra, dec, pa, wins):
     """
     Make finding chart with object info overlaid
     """
     fname = filedialog.asksaveasfilename(
         initialdir=expanduser("~"),
-        defaultextension='.jpg',
-        filetypes=[('finding charts', '.jpg')],
-        title='Name of finding chart')
+        defaultextension=".jpg",
+        filetypes=[("finding charts", ".jpg")],
+        title="Name of finding chart",
+    )
 
     if have_pillow:
-        make_finder_pillow(logger, fname, img_array, object_name, tel, ra, dec, pa, wins)
+        make_finder_pillow(
+            logger, fname, img_array, object_name, tel, ra, dec, pa, wins
+        )
     elif have_opencv:
-        make_finder_opencv(logger, fname, img_array, object_name, tel, ra, dec, pa, wins)
+        make_finder_opencv(
+            logger, fname, img_array, object_name, tel, ra, dec, pa, wins
+        )
     else:
-        logger.error(msg='Cannot make finder, please install openCV or Pillow')
+        logger.error(msg="Cannot make finder, please install openCV or Pillow")
 
 
 def make_finder_opencv(logger, fname, img_array, object_name, tel, ra, dec, pa, wins):
-    logger.error(msg="openCV finding chart saving not implemented, please install Pillow")
+    logger.error(
+        msg="openCV finding chart saving not implemented, please install Pillow"
+    )
 
 
 def make_finder_pillow(logger, fname, img_array, object_name, tel, ra, dec, pa, wins):
     image = Image.fromarray(img_array)
     image = image.convert("RGB")
     width, height = image.size
     draw = ImageDraw.Draw(image)
     if not object_name:
-        raise ValueError('you should supply an object name')
+        raise ValueError("you should supply an object name")
 
-    info_msg = "{object_name} ({tel})\n{ra} {dec}\nPA = {pa:.1f}\n{wins:s}\nv{version}".format(
-        object_name=object_name, tel=tel, ra=ra, dec=dec, pa=pa, wins=wins, version=version
+    info_msg = (
+        "{object_name} ({tel})\n{ra} {dec}\nPA = {pa:.1f}\n{wins:s}\nv{version}".format(
+            object_name=object_name,
+            tel=tel,
+            ra=ra,
+            dec=dec,
+            pa=pa,
+            wins=wins,
+            version=version,
+        )
     )
     font_size = 5
-    font_file = pkg_resources.resource_filename('hcam_finder', 'data/Lato-Regular.ttf')
+    font_file = pkg_resources.resource_filename("hcam_finder", "data/Lato-Regular.ttf")
     text_x = 0.0
-    while text_x/width < 0.4:
+    while text_x / width < 0.4:
         font_size += 1
         font = ImageFont.truetype(font_file, font_size)
-        text_x, text_y = max((font.getsize(txt) for txt in info_msg.splitlines()))
+        text_x, text_y = max((font.getbbox(txt) for txt in info_msg.splitlines()))
 
     nlines = len(info_msg.splitlines()) + 1
-    rect_x, rect_y = int(1.1*text_x), nlines*int(text_y)
-    rectangle = Image.new('RGBA', (rect_x, rect_y), (255, 255, 255, 200))
+    rect_x, rect_y = int(1.1 * text_x), nlines * int(text_y)
+    rectangle = Image.new("RGBA", (rect_x, rect_y), (255, 255, 255, 200))
 
     width, height = image.size
     x = width - rect_x
     y = 0
     image.paste(rectangle, (x, y), rectangle)
-    x = width - 1.05*text_x
-    draw.text((x, y), info_msg, font=font, fill='rgb(255, 0, 0)')
+    x = width - 1.05 * text_x
+    draw.text((x, y), info_msg, font=font, fill="rgb(255, 0, 0)")
     image.save(fname)
```

### Comparing `hcam_finder-1.3.0/hcam_finder/hcam_finder.py` & `hcam_finder-1.3.1/hcam_finder/hcam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/panstarrs.py` & `hcam_finder-1.3.1/hcam_finder/panstarrs.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/shapes.py` & `hcam_finder-1.3.1/hcam_finder/shapes.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/skyview.py` & `hcam_finder-1.3.1/hcam_finder/skyview.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/ucam_finder.py` & `hcam_finder-1.3.1/hcam_finder/ucam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/uspec_finder.py` & `hcam_finder-1.3.1/hcam_finder/uspec_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder/ztf.py` & `hcam_finder-1.3.1/hcam_finder/ztf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/hcam_finder.egg-info/PKG-INFO` & `hcam_finder-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: hcam-finder
-Version: 1.3.0
+Name: hcam_finder
+Version: 1.3.1
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.0/hcam_finder.egg-info/SOURCES.txt` & `hcam_finder-1.3.1/hcam_finder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/scripts/hfinder` & `hcam_finder-1.3.1/scripts/hfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/scripts/ufinder` & `hcam_finder-1.3.1/scripts/ufinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/scripts/usfinder` & `hcam_finder-1.3.1/scripts/usfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.0/setup.py` & `hcam_finder-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_finder",
-    version="1.3.0",
+    version="1.3.1",
     description="Observation planning and finding charts for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_finder",
-    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz",
     packages=[
         "hcam_finder",
     ],
     package_dir={"hcam_finder": "hcam_finder"},
     include_package_data=True,
     scripts=scripts,
     install_requires=requirements,
```

### Comparing `hcam_finder-1.3.0/tests/test_hcam_finder.py` & `hcam_finder-1.3.1/tests/test_hcam_finder.py`

 * *Files identical despite different names*

