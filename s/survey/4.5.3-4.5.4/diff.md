# Comparing `tmp/survey-4.5.3.tar.gz` & `tmp/survey-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.5.3.tar", last modified: Thu Jul 20 20:10:26 2023, max compression
+gzip compressed data, was "survey-4.5.4.tar", last modified: Mon Jul 24 17:58:06 2023, max compression
```

## Comparing `survey-4.5.3.tar` & `survey-4.5.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.756712 survey-4.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.740712 survey-4.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.744712 survey-4.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 20:10:06.000000 survey-4.5.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-20 20:10:06.000000 survey-4.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 20:10:06.000000 survey-4.5.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-20 20:10:06.000000 survey-4.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-20 20:10:26.752712 survey-4.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 20:10:06.000000 survey-4.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.744712 survey-4.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 20:10:06.000000 survey-4.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.740712 survey-4.5.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.748712 survey-4.5.3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/graphics.lineprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/graphics.spinprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.done-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.fail-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.info-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.basket-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.basket-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.conceal-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.datetime-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.datetime-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.form-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.input-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.input-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.inquire-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.numeric-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.numeric-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.select-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.select-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/showcase-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/showcase-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-20 20:10:06.000000 survey-4.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 20:10:06.000000 survey-4.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 20:10:06.000000 survey-4.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 20:10:06.000000 survey-4.5.3/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:10:26.756712 survey-4.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 20:10:06.000000 survey-4.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 20:10:06.000000 survey-4.5.3/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    58184 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.572854 survey-4.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.560854 survey-4.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.564854 survey-4.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 17:57:51.000000 survey-4.5.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-24 17:57:51.000000 survey-4.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 17:57:51.000000 survey-4.5.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 17:57:51.000000 survey-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-24 17:58:06.572854 survey-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-24 17:57:51.000000 survey-4.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.564854 survey-4.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 17:57:51.000000 survey-4.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.564854 survey-4.5.4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.568854 survey-4.5.4/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/graphics.lineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/graphics.spinprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/printers.done-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/printers.fail-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/printers.info-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.basket-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.basket-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.conceal-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.datetime-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.datetime-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.form-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.input-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.input-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.inquire-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.numeric-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.numeric-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.select-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/routines.select-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/showcase-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-24 17:57:51.000000 survey-4.5.4/docs/_static/images/showcase-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-24 17:57:51.000000 survey-4.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 17:57:51.000000 survey-4.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 17:57:51.000000 survey-4.5.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 17:57:51.000000 survey-4.5.4/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:58:06.572854 survey-4.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 17:57:51.000000 survey-4.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.568854 survey-4.5.4/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-24 17:57:51.000000 survey-4.5.4/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.572854 survey-4.5.4/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58303 2023-07-24 17:57:51.000000 survey-4.5.4/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:06.568854 survey-4.5.4/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-24 17:58:06.000000 survey-4.5.4/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-24 17:58:06.000000 survey-4.5.4/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:58:06.000000 survey-4.5.4/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 17:58:06.000000 survey-4.5.4/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 17:58:06.000000 survey-4.5.4/survey.egg-info/top_level.txt
```

### Comparing `survey-4.5.3/.github/workflows/publish.yml` & `survey-4.5.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/.gitignore` & `survey-4.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/LICENSE` & `survey-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/PKG-INFO` & `survey-4.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.3
+Version: 4.5.4
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.3/README.rst` & `survey-4.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/Makefile` & `survey-4.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/graphics.lineprogress-1.gif` & `survey-4.5.4/docs/_static/images/graphics.lineprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/graphics.spinprogress-1.gif` & `survey-4.5.4/docs/_static/images/graphics.spinprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/printers.done-1.png` & `survey-4.5.4/docs/_static/images/printers.done-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/printers.fail-1.png` & `survey-4.5.4/docs/_static/images/printers.fail-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/printers.info-1.png` & `survey-4.5.4/docs/_static/images/printers.info-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.basket-1.gif` & `survey-4.5.4/docs/_static/images/routines.basket-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.basket-2.gif` & `survey-4.5.4/docs/_static/images/routines.basket-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.conceal-1.gif` & `survey-4.5.4/docs/_static/images/routines.conceal-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.datetime-1.gif` & `survey-4.5.4/docs/_static/images/routines.datetime-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.datetime-2.gif` & `survey-4.5.4/docs/_static/images/routines.datetime-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.form-1.gif` & `survey-4.5.4/docs/_static/images/routines.form-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.input-1.gif` & `survey-4.5.4/docs/_static/images/routines.input-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.input-2.gif` & `survey-4.5.4/docs/_static/images/routines.input-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.inquire-1.gif` & `survey-4.5.4/docs/_static/images/routines.inquire-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.numeric-1.gif` & `survey-4.5.4/docs/_static/images/routines.numeric-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.numeric-2.gif` & `survey-4.5.4/docs/_static/images/routines.numeric-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.select-1.gif` & `survey-4.5.4/docs/_static/images/routines.select-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/routines.select-2.gif` & `survey-4.5.4/docs/_static/images/routines.select-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/showcase-1.gif` & `survey-4.5.4/docs/_static/images/showcase-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/_static/images/showcase-2.gif` & `survey-4.5.4/docs/_static/images/showcase-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/conf.py` & `survey-4.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/index.rst` & `survey-4.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/make.bat` & `survey-4.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/docs/reference.rst` & `survey-4.5.4/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/setup.py` & `survey-4.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/__init__.py` & `survey-4.5.4/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_colors.py` & `survey-4.5.4/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_controls.py` & `survey-4.5.4/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/__init__.py` & `survey-4.5.4/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_ansi.py` & `survey-4.5.4/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_console.py` & `survey-4.5.4/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_cursor.py` & `survey-4.5.4/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_handle.py` & `survey-4.5.4/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_helpers.py` & `survey-4.5.4/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_intel.py` & `survey-4.5.4/survey/_core/_intel.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_io.py` & `survey-4.5.4/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_io_os.py` & `survey-4.5.4/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_io_os_nt.py` & `survey-4.5.4/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_io_os_posix.py` & `survey-4.5.4/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_render.py` & `survey-4.5.4/survey/_core/_render.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_screen.py` & `survey-4.5.4/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_core/_source.py` & `survey-4.5.4/survey/_core/_source.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_funnels.py` & `survey-4.5.4/survey/_funnels.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_graphics.py` & `survey-4.5.4/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_handle.py` & `survey-4.5.4/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_helpers.py` & `survey-4.5.4/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_mutates.py` & `survey-4.5.4/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_printers.py` & `survey-4.5.4/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_routines.py` & `survey-4.5.4/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_searches.py` & `survey-4.5.4/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_stage.py` & `survey-4.5.4/survey/_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
     }
 
     main_visual_point_latch = main_visual_point_latch_group[site]
     main_visual_point_index = main_visual_tiles.index(main_visual_point_latch)
     main_visual_point = [main_visual_point_index]
 
     main_funnel_leave_group = []
-    main_funnel_leave_entry = _funnels.text_max_dynamic(_system.cursor.measure)
-    main_funnel_leave_group.append(main_funnel_leave_entry)
+    # main_funnel_leave_entry = _funnels.text_max_dynamic(_system.cursor.measure)
+    # main_funnel_leave_group.append(main_funnel_leave_entry)
     main_funnel_leave = _helpers.chain_functions(*main_funnel_leave_group)
 
     main_visual = _visuals.Line.link(main_visual_tiles, main_visual_point, funnel_leave = main_funnel_leave)
 
     return main_visual
```

### Comparing `survey-4.5.3/survey/_system.py` & `survey-4.5.4/survey/_system.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_theme.py` & `survey-4.5.4/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_utils.py` & `survey-4.5.4/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_visuals.py` & `survey-4.5.4/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.3/survey/_widgets.py` & `survey-4.5.4/survey/_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,29 @@
 from . import _handle
 from . import _stage
 from . import _funnels
 from . import _searches
 from . import _theme
 
 
-__all__ = ('WidgetError', 'Widget', 'start', 
+__all__ = ('Abort', 'Escape', 'Widget', 'start', 
            'BaseText', 'Input', 'Numeric', 'Conceal', 'AutoSubmit', 'Inquire', 
            'BaseMesh', 'BaseList', 'Select', 'Basket', 'Count', 'DateTime',
            'Form')
 
 
 class Abort(_helpers.InfoErrorMixin, Exception):
 
     """
     Raised when an invokation needs to stop. May include a message.
     """
 
     __slots__ = ()
 
 
-
 class Escape(Exception):
 
     """
     Raised when the users pressed the ``Esc`` button.
     """
 
     __slots__ = ()
@@ -154,17 +153,19 @@
             return
 
         value = self._product
 
         if value is self._product_mark:
             value = self._product = self._resolve()
 
-        validate(value)
-        
-        self._product = self._product_mark
+        try:
+            validate(value)
+        except Abort:
+            self._product = self._product_mark
+            raise
 
     def _invoke(self, event, *args, **kwargs):
 
         if self._delegate and not self._delegate(event):
             return
 
         try:
@@ -712,17 +713,17 @@
 
     """
     A text editor that automatically submits a upon valid insertion.
 
     Resolves into a :class:`str`.
 
     :param evaluate:
-        Used with ``(result)`` before insertion, which can be prevented by raising :exc:`.Abort`.
+        Used with ``(result)`` before insertion, which can be prevented by raising :exc:`.Abort` (like :paramref:`.Widget.validate`).
     :param validate:
-        Used with ``(result)`` after to decide whether to submit.
+        Used with ``(result)`` after to decide whether to submit (should return :cls:`bool`).
     :param default:
         Used instead when attempting to submit without a value.
     :param transform:
         Used with ``(result)`` and should return a new ``result`` used for checks.
 
     Arguments directly passed to super-class:
```

### Comparing `survey-4.5.3/survey.egg-info/PKG-INFO` & `survey-4.5.4/survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.3
+Version: 4.5.4
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.3/survey.egg-info/SOURCES.txt` & `survey-4.5.4/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

