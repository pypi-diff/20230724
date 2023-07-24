# Comparing `tmp/hcam_finder-1.3.1.tar.gz` & `tmp/hcam_finder-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_finder-1.3.1.tar", last modified: Mon Jul 24 09:58:09 2023, max compression
+gzip compressed data, was "hcam_finder-1.3.2.tar", last modified: Mon Jul 24 10:17:19 2023, max compression
```

## Comparing `hcam_finder-1.3.1.tar` & `hcam_finder-1.3.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710476 hcam_finder-1.3.1/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.1/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 09:58:09.710556 hcam_finder-1.3.1/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.1/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.698781 hcam_finder-1.3.1/docs/
--rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/docs/Makefile
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.692906 hcam_finder-1.3.1/docs/_build/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.693240 hcam_finder-1.3.1/docs/_build/html/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.700598 hcam_finder-1.3.1/docs/_build/html/_images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.1/docs/_build/html/_images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/_build/html/_images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/_build/html/_images/main.png
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.702165 hcam_finder-1.3.1/docs/_build/html/_static/
--rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/file.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.1/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.1/docs/conf.py
--rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.1/docs/hcam_finder.rst
--rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/hipercam.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.704509 hcam_finder-1.3.1/docs/images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.1/docs/images/main.png
--rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/index.rst
--rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/docs/make.bat
--rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.1/docs/modules.rst
--rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/ultracam.rst
--rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/docs/ultraspec.rst
--rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/docs/usage.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.706526 hcam_finder-1.3.1/hcam_finder/
--rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-24 09:57:47.000000 hcam_finder-1.3.1/hcam_finder/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/hcam_finder/config.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.709484 hcam_finder-1.3.1/hcam_finder/data/
--rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.1/hcam_finder/data/Lato-Black.ttf
--rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.1/hcam_finder/data/Lato-Regular.ttf
--rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.1/hcam_finder/data/README.rst
--rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/data/config
--rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/data/configspec.ini
--rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.1/hcam_finder/data/guider_hole_arcseconds.txt
--rw-r--r--   0 sl         (501) staff       (20)    21032 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/hcam_finder/finders.py
--rw-r--r--   0 sl         (501) staff       (20)     2802 2023-07-24 09:57:08.000000 hcam_finder-1.3.1/hcam_finder/finding_chart.py
--rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/hcam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.1/hcam_finder/panstarrs.py
--rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-21 10:53:55.000000 hcam_finder-1.3.1/hcam_finder/shapes.py
--rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.1/hcam_finder/skyview.py
--rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.1/hcam_finder/ucam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.1/hcam_finder/uspec_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.1/hcam_finder/ztf.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.707268 hcam_finder-1.3.1/hcam_finder.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-24 09:58:09.000000 hcam_finder-1.3.1/hcam_finder.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710107 hcam_finder-1.3.1/scripts/
--rw-r--r--   0 sl         (501) staff       (20)    12564 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/hfinder
--rw-r--r--   0 sl         (501) staff       (20)    10866 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/ufinder
--rw-r--r--   0 sl         (501) staff       (20)    11371 2023-02-23 13:46:51.000000 hcam_finder-1.3.1/scripts/usfinder
--rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-24 09:58:09.710830 hcam_finder-1.3.1/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-24 09:57:47.000000 hcam_finder-1.3.1/setup.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 09:58:09.710363 hcam_finder-1.3.1/tests/
--rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/tests/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.1/tests/test_hcam_finder.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.402256 hcam_finder-1.3.2/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.2/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 10:17:19.402558 hcam_finder-1.3.2/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.2/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.390494 hcam_finder-1.3.2/docs/
+-rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/docs/Makefile
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.384782 hcam_finder-1.3.2/docs/_build/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.384888 hcam_finder-1.3.2/docs/_build/html/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.392786 hcam_finder-1.3.2/docs/_build/html/_images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.2/docs/_build/html/_images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/_build/html/_images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/_build/html/_images/main.png
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.393797 hcam_finder-1.3.2/docs/_build/html/_static/
+-rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/plus.png
+-rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.2/docs/conf.py
+-rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.2/docs/hcam_finder.rst
+-rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/hipercam.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.395518 hcam_finder-1.3.2/docs/images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/images/main.png
+-rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/index.rst
+-rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/docs/make.bat
+-rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.2/docs/modules.rst
+-rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/ultracam.rst
+-rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/ultraspec.rst
+-rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/usage.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.397333 hcam_finder-1.3.2/hcam_finder/
+-rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-24 10:17:05.000000 hcam_finder-1.3.2/hcam_finder/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/hcam_finder/config.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.400687 hcam_finder-1.3.2/hcam_finder/data/
+-rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.2/hcam_finder/data/Lato-Black.ttf
+-rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.2/hcam_finder/data/Lato-Regular.ttf
+-rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.2/hcam_finder/data/README.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/data/config
+-rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/data/configspec.ini
+-rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.2/hcam_finder/data/guider_hole_arcseconds.txt
+-rw-r--r--   0 sl         (501) staff       (20)    21032 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/finders.py
+-rw-r--r--   0 sl         (501) staff       (20)     2808 2023-07-24 10:14:58.000000 hcam_finder-1.3.2/hcam_finder/finding_chart.py
+-rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/hcam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.2/hcam_finder/panstarrs.py
+-rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/shapes.py
+-rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.2/hcam_finder/skyview.py
+-rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.2/hcam_finder/ucam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/hcam_finder/uspec_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.2/hcam_finder/ztf.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.398487 hcam_finder-1.3.2/hcam_finder.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.401047 hcam_finder-1.3.2/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)    12564 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/hfinder
+-rw-r--r--   0 sl         (501) staff       (20)    10866 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/ufinder
+-rw-r--r--   0 sl         (501) staff       (20)    11371 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/usfinder
+-rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-24 10:17:19.403109 hcam_finder-1.3.2/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-24 10:17:05.000000 hcam_finder-1.3.2/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.401466 hcam_finder-1.3.2/tests/
+-rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/tests/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/tests/test_hcam_finder.py
```

### Comparing `hcam_finder-1.3.1/CONTRIBUTING.rst` & `hcam_finder-1.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/LICENSE` & `hcam_finder-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/PKG-INFO` & `hcam_finder-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_finder
-Version: 1.3.1
+Version: 1.3.2
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.1/README.rst` & `hcam_finder-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/Makefile` & `hcam_finder-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/_build/html/_images/compo.png` & `hcam_finder-1.3.2/docs/_build/html/_images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/_build/html/_images/inst.png` & `hcam_finder-1.3.2/docs/_build/html/_images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/_build/html/_images/main.png` & `hcam_finder-1.3.2/docs/_build/html/_images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/conf.py` & `hcam_finder-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/hcam_finder.rst` & `hcam_finder-1.3.2/docs/hcam_finder.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/hipercam.rst` & `hcam_finder-1.3.2/docs/hipercam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/images/compo.png` & `hcam_finder-1.3.2/docs/images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/images/inst.png` & `hcam_finder-1.3.2/docs/images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/images/main.png` & `hcam_finder-1.3.2/docs/images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/make.bat` & `hcam_finder-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/ultracam.rst` & `hcam_finder-1.3.2/docs/ultracam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/docs/usage.rst` & `hcam_finder-1.3.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/config.py` & `hcam_finder-1.3.2/hcam_finder/config.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/data/Lato-Black.ttf` & `hcam_finder-1.3.2/hcam_finder/data/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/data/Lato-Regular.ttf` & `hcam_finder-1.3.2/hcam_finder/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/data/config` & `hcam_finder-1.3.2/hcam_finder/data/config`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/data/configspec.ini` & `hcam_finder-1.3.2/hcam_finder/data/configspec.ini`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/data/guider_hole_arcseconds.txt` & `hcam_finder-1.3.2/hcam_finder/data/guider_hole_arcseconds.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/finders.py` & `hcam_finder-1.3.2/hcam_finder/finders.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/finding_chart.py` & `hcam_finder-1.3.2/hcam_finder/finding_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     )
     font_size = 5
     font_file = pkg_resources.resource_filename("hcam_finder", "data/Lato-Regular.ttf")
     text_x = 0.0
     while text_x / width < 0.4:
         font_size += 1
         font = ImageFont.truetype(font_file, font_size)
-        text_x, text_y = max((font.getbbox(txt) for txt in info_msg.splitlines()))
+        _, _, text_x, text_y = max((font.getbbox(txt) for txt in info_msg.splitlines()))
 
     nlines = len(info_msg.splitlines()) + 1
     rect_x, rect_y = int(1.1 * text_x), nlines * int(text_y)
     rectangle = Image.new("RGBA", (rect_x, rect_y), (255, 255, 255, 200))
 
     width, height = image.size
     x = width - rect_x
```

### Comparing `hcam_finder-1.3.1/hcam_finder/hcam_finder.py` & `hcam_finder-1.3.2/hcam_finder/hcam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/panstarrs.py` & `hcam_finder-1.3.2/hcam_finder/panstarrs.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/shapes.py` & `hcam_finder-1.3.2/hcam_finder/shapes.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/skyview.py` & `hcam_finder-1.3.2/hcam_finder/skyview.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/ucam_finder.py` & `hcam_finder-1.3.2/hcam_finder/ucam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/uspec_finder.py` & `hcam_finder-1.3.2/hcam_finder/uspec_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder/ztf.py` & `hcam_finder-1.3.2/hcam_finder/ztf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/hcam_finder.egg-info/PKG-INFO` & `hcam_finder-1.3.2/hcam_finder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-finder
-Version: 1.3.1
+Version: 1.3.2
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.1/hcam_finder.egg-info/SOURCES.txt` & `hcam_finder-1.3.2/hcam_finder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/scripts/hfinder` & `hcam_finder-1.3.2/scripts/hfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/scripts/ufinder` & `hcam_finder-1.3.2/scripts/ufinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/scripts/usfinder` & `hcam_finder-1.3.2/scripts/usfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.1/setup.py` & `hcam_finder-1.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_finder",
-    version="1.3.1",
+    version="1.3.2",
     description="Observation planning and finding charts for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_finder",
-    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.1.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz",
     packages=[
         "hcam_finder",
     ],
     package_dir={"hcam_finder": "hcam_finder"},
     include_package_data=True,
     scripts=scripts,
     install_requires=requirements,
```

### Comparing `hcam_finder-1.3.1/tests/test_hcam_finder.py` & `hcam_finder-1.3.2/tests/test_hcam_finder.py`

 * *Files identical despite different names*

