# Comparing `tmp/mds_cashbook-6.0.27.tar.gz` & `tmp/mds_cashbook-6.8.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook-6.0.27.tar", last modified: Mon Mar  6 08:19:37 2023, max compression
+gzip compressed data, was "mds_cashbook-6.8.29.tar", last modified: Mon Jul 24 14:36:05 2023, max compression
```

## Comparing `mds_cashbook-6.0.27.tar` & `mds_cashbook-6.8.29.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:37.030711 mds_cashbook-6.0.27/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    10382 2023-03-06 08:19:37.030711 mds_cashbook-6.0.27/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7085 2023-03-06 08:02:22.000000 mds_cashbook-6.0.27/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1418 2023-02-27 09:04:56.000000 mds_cashbook-6.0.27/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    19429 2023-03-06 08:02:17.000000 mds_cashbook-6.0.27/book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    25813 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/book.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5262 2023-02-14 09:16:20.000000 mds_cashbook-6.0.27/category.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6152 2022-08-31 08:17:59.000000 mds_cashbook-6.0.27/category.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2244 2022-08-17 13:23:22.000000 mds_cashbook-6.0.27/cbreport.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      689 2022-08-17 11:02:47.000000 mds_cashbook-6.0.27/cbreport.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6923 2022-09-19 07:22:09.000000 mds_cashbook-6.0.27/configuration.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3777 2022-08-17 15:11:32.000000 mds_cashbook-6.0.27/configuration.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1387 2023-02-27 09:04:56.000000 mds_cashbook-6.0.27/currency.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:36.890712 mds_cashbook-6.0.27/docs/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      495 2023-03-06 08:02:17.000000 mds_cashbook-6.0.27/docs/settings.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1013 2022-08-17 15:04:54.000000 mds_cashbook-6.0.27/group.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:36.890712 mds_cashbook-6.0.27/icon/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3638 2022-08-05 09:29:25.000000 mds_cashbook-6.0.27/icon/notebook1.svg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      431 2022-08-05 09:40:25.000000 mds_cashbook-6.0.27/icon.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    42092 2023-03-06 08:02:18.000000 mds_cashbook-6.0.27/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    13101 2023-03-02 13:11:34.000000 mds_cashbook-6.0.27/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:36.918712 mds_cashbook-6.0.27/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    45516 2023-02-14 09:16:20.000000 mds_cashbook-6.0.27/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    42793 2023-02-14 09:16:20.000000 mds_cashbook-6.0.27/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:37.030711 mds_cashbook-6.0.27/mds_cashbook.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    10382 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1645 2023-03-06 08:19:36.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-03-06 08:19:35.000000 mds_cashbook-6.0.27/mds_cashbook.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5212 2023-02-14 09:16:20.000000 mds_cashbook-6.0.27/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7708 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/message.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7420 2023-02-27 09:04:56.000000 mds_cashbook-6.0.27/mixin.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     9404 2023-03-06 08:02:18.000000 mds_cashbook-6.0.27/model.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    17859 2023-02-27 09:04:57.000000 mds_cashbook-6.0.27/reconciliation.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     9715 2022-08-17 15:10:59.000000 mds_cashbook-6.0.27/reconciliation.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:36.930712 mds_cashbook-6.0.27/report/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    20379 2022-08-16 14:46:49.000000 mds_cashbook-6.0.27/report/cashbook.fods
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    52038 2022-08-17 13:50:10.000000 mds_cashbook-6.0.27/report/reconciliation.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-03-06 08:19:37.030711 mds_cashbook-6.0.27/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3715 2023-03-06 08:02:18.000000 mds_cashbook-6.0.27/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    10572 2023-02-27 09:04:57.000000 mds_cashbook-6.0.27/splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6109 2022-08-25 13:55:54.000000 mds_cashbook-6.0.27/splitline.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:36.986711 mds_cashbook-6.0.27/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1328 2023-02-27 09:04:57.000000 mds_cashbook-6.0.27/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    24603 2023-03-06 08:02:18.000000 mds_cashbook-6.0.27/tests/test_book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6852 2022-09-19 07:22:10.000000 mds_cashbook-6.0.27/tests/test_bookingwiz.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8368 2022-08-31 08:17:59.000000 mds_cashbook-6.0.27/tests/test_category.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6783 2022-10-04 14:48:13.000000 mds_cashbook-6.0.27/tests/test_config.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2813 2023-02-28 07:45:34.000000 mds_cashbook-6.0.27/tests/test_currency.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    71083 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/tests/test_line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    31148 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/tests/test_reconciliation.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    15058 2023-01-19 08:46:08.000000 mds_cashbook-6.0.27/tests/test_splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1605 2022-08-10 11:24:57.000000 mds_cashbook-6.0.27/tests/test_type.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      346 2023-03-06 08:02:22.000000 mds_cashbook-6.0.27/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1964 2023-02-27 09:04:57.000000 mds_cashbook-6.0.27/types.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3454 2022-08-17 15:11:12.000000 mds_cashbook-6.0.27/types.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)        1 2022-08-23 13:45:55.000000 mds_cashbook-6.0.27/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-03-06 08:19:37.026711 mds_cashbook-6.0.27/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2491 2023-02-23 08:54:51.000000 mds_cashbook-6.0.27/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      362 2023-01-03 08:06:04.000000 mds_cashbook-6.0.27/view/book_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      451 2023-01-03 08:06:04.000000 mds_cashbook-6.0.27/view/book_tree.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      450 2022-10-11 08:21:24.000000 mds_cashbook-6.0.27/view/cashbook_line_context_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      725 2022-09-22 12:49:04.000000 mds_cashbook-6.0.27/view/category_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      248 2022-08-31 08:17:59.000000 mds_cashbook-6.0.27/view/category_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      337 2022-08-31 08:17:59.000000 mds_cashbook-6.0.27/view/category_tree.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      999 2022-09-19 07:22:10.000000 mds_cashbook-6.0.27/view/configuration_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1048 2022-09-07 14:34:10.000000 mds_cashbook-6.0.27/view/enterbooking_start_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1867 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/view/line_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      583 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/view/line_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      555 2022-11-17 08:14:16.000000 mds_cashbook-6.0.27/view/line_recon_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1085 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/view/recon_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      447 2022-08-12 11:44:33.000000 mds_cashbook-6.0.27/view/recon_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      940 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/view/split_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      578 2023-01-23 07:52:37.000000 mds_cashbook-6.0.27/view/split_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      379 2023-01-02 09:23:42.000000 mds_cashbook-6.0.27/view/type_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      298 2023-01-02 09:23:43.000000 mds_cashbook-6.0.27/view/type_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      533 2022-08-09 08:07:29.000000 mds_cashbook-6.0.27/view/wizard_openline_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      923 2022-08-18 07:31:11.000000 mds_cashbook-6.0.27/view/wizard_runrepbook_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6810 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_booking.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      745 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_booking.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5564 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_openline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1614 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_openline.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     4651 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_runreport.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1221 2023-01-16 08:03:24.000000 mds_cashbook-6.0.27/wizard_runreport.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5272 2023-07-24 14:34:56.000000 mds_cashbook-6.8.29/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1419 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20418 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/book.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    25813 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/book.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5303 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/category.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/cbreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/cbreport.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7107 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/configuration.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/configuration.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1408 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/currency.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/docs/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/docs/settings.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/group.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/icon/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/icon/notebook1.svg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/icon.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    42989 2023-07-24 14:33:17.000000 mds_cashbook-6.8.29/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    13101 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    45516 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    42793 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/mds_cashbook.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1623 2023-07-24 14:36:05.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/menu.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7708 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/message.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/mixin.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9652 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/model.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    18296 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/reconciliation.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9715 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/reconciliation.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/report/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/report/cashbook.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/report/reconciliation.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3760 2023-07-24 14:33:03.000000 mds_cashbook-6.8.29/setup.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    11211 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/splitline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6109 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/splitline.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.140850 mds_cashbook-6.8.29/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      203 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    24904 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/book.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6777 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/bookingwiz.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8328 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6679 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/config.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2699 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/currency.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    74460 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/reconciliation.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    15377 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/splitline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      964 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/test_module.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/type.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      346 2023-07-24 14:33:46.000000 mds_cashbook-6.8.29/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2124 2023-07-24 14:33:17.000000 mds_cashbook-6.8.29/types.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/types.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      362 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      451 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/cashbook_line_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/configuration_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1048 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/enterbooking_start_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      583 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      555 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/recon_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      447 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/split_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      578 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/split_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/type_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/type_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/wizard_openline_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/wizard_runrepbook_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6894 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_booking.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_booking.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_openline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_openline.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4619 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_runreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_runreport.xml
```

### Comparing `mds_cashbook-6.0.27/README.rst` & `mds_cashbook-6.8.29/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Install
 =======
 
 pip install mds-cashbook
 
 Requires
 ========
-- Tryton 6.0
+- Tryton 6.8
 
 How to
 ======
 
 This module adds a cash book to Tryton. Each Tryton user can have
 any number of cash books. The cash books can be arranged hierarchically.
 A cash book contains simple postings, such as expense, revenue, transfer,
@@ -149,127 +149,14 @@
 If you have hierarchical cash books, the amounts of subordinate cash books with foreign
 currency are converted  into the display currency of the parent cash book.
 
 
 Changes
 =======
 
-*6.0.27 - 05.03.2023*
+*6.8.29 - 24.07.2023*
 
-- updt: optimize caching
-- add: settings for trytond.conf
+- fix: type of indexes
 
-*6.0.26 - 27.02.2023*
-
-- updt: cashbook-form optimized
-- add: caching
-
-*6.0.25 - 14.02.2023*
-
-- fix: possible exception by invalid date in context
-- updt: optimize table + icon
-
-*6.0.24 - 05.02.2023*
-
-- fix: rewrite of line-values
-
-*6.0.23 - 28.01.2023*
-
-- fix: selection of subordinate cash books for calculations
-
-*6.0.22 - 21.01.2023*
-
-- add: enable extension by investment-module
-- updt: optimize form/list-views
-
-*6.0.21 - 29.11.2022*
-
-- updt: remove 'reconcile' button from line-form
-- add: how to
-
-*6.0.20 - 16.11.2022*
-
-- add: new state 'reconciled' at line
-
-*6.0.19 - 19.10.2022*
-
-- fix: delete()
-
-*6.0.18 - 11.10.2022*
-
-- updt: optimized open/view of cashbook
-
-*6.0.17 - 10.10.2022*
-
-- add: colors for cashbook-lines
-- add: client stores tree-state of cashbook
-
-*6.0.16 - 07.10.2022*
-
-- add: open cashbook-lines from cashbook
-
-*6.0.15 - 04.10.2022*
-
-- updt: second-currency support optimized
-
-*6.0.14 - 30.09.2022*
-
-- fix: parameter
-
-*6.0.13 - 28.09.2022*
-
-- hierarchical ordering for cashbook
-- forms optimzed
-
-*6.0.12 - 18.09.2022*
-
-- add: selected cashbooks in 'enter-booking-dialog'
-
-*6.0.11 - 16.09.2022*
-
-- add: hierarchy for cashbooks
-
-*6.0.10 - 13.09.2022*
-
-- add: split-booking with transfer
-
-*6.0.9 - 08.09.2022*
-
-- updt: allow negative amounts
-
-*6.0.8 - 07.09.2022*
-
-- updt: enter-booking form optimized
-
-*6.0.7 - 07.09.2022*
-
-- add: enter-booking-wizard
-
-*6.0.6 - 06.09.2022*
-
-- updt: optimized form - line, line-context
-- updt: extended search in cashbook-lines
-
-*6.0.5 - 05.09.2022*
-
-- updt: view of book + line optimized
-
-*6.0.4 - 05.09.2022*
-
-- fix: write number at state-change 'check' -> 'done'
-- updt: speedup transaction view
-
-*6.0.3 - 31.08.2022*
-
-- updt: checks, sorting
-
-*6.0.2 - 25.08.2022*
-
-- add: split-booking
-
-*6.0.1 - 23.08.2022*
-
-- works
-
-*6.0.0 - 05.08.2022*
+*6.8.28 - 05.06.2023*
 
 - init
```

### Comparing `mds_cashbook-6.0.27/__init__.py` & `mds_cashbook-6.8.29/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .configuration import Configuration, UserConfiguration
 from .category import Category
 from .reconciliation import Reconciliation
 from .cbreport import ReconciliationReport
 from .currency import CurrencyRate
 from .model import MemCache
 
+
 def register():
     Pool.register(
         MemCache,
         Configuration,
         UserConfiguration,
         CurrencyRate,
         Type,
```

### Comparing `mds_cashbook-6.0.27/book.py` & `mds_cashbook-6.8.29/book.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import Workflow, ModelView, ModelSQL, fields, Check, tree
+from trytond.model import (
+    Workflow, ModelView, ModelSQL, fields, Check,
+    tree, Index)
 from trytond.pyson import Eval, Or, Bool, Id, Len
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.transaction import Transaction
 from trytond.pool import Pool
 from trytond.report import Report
 from trytond.config import config
@@ -16,24 +18,26 @@
 from sql.aggregate import Sum
 from sql.conditionals import Case
 from .model import order_name_hierarchical, sub_ids_hierarchical, \
     AnyInArray, CACHEKEY_CURRENCY
 
 
 # enable/disable caching of cachekey for 'currency.rate'
-if config.get('cashbook', 'cache_currency', default='yes').lower() in ['yes', '1', 'true']:
+if config.get(
+            'cashbook', 'cache_currency', default='yes'
+        ).lower() in ['yes', '1', 'true']:
     ENA_CURRKEY = True
-else :
+else:
     ENA_CURRKEY = False
 
 
 STATES = {
     'readonly': Eval('state', '') != 'open',
     }
-DEPENDS=['state']
+DEPENDS = ['state']
 
 # states in case of 'btype'!=None
 STATES2 = {
     'readonly': Or(
             Eval('state', '') != 'open',
             ~Bool(Eval('btype')),
         ),
@@ -51,114 +55,136 @@
     ]
 
 
 class Book(tree(separator='/'), Workflow, ModelSQL, ModelView):
     'Cashbook'
     __name__ = 'cashbook.book'
 
-    company = fields.Many2One(string='Company', model_name='company.company',
-        required=True, select=True, ondelete="RESTRICT")
-    name = fields.Char(string='Name', required=True,
-        states=STATES, depends=DEPENDS)
-    description = fields.Text(string='Description',
-        states=STATES, depends=DEPENDS)
-    btype = fields.Many2One(string='Type', select=True,
-        help='A cash book with type can contain postings. Without type is a view.',
+    company = fields.Many2One(
+        string='Company', model_name='company.company',
+        required=True, ondelete="RESTRICT")
+    name = fields.Char(
+        string='Name', required=True, states=STATES, depends=DEPENDS)
+    description = fields.Text(
+        string='Description', states=STATES, depends=DEPENDS)
+    btype = fields.Many2One(
+        string='Type',
+        help='A cash book with type can contain postings. ' +
+        'Without type is a view.',
         model_name='cashbook.type', ondelete='RESTRICT',
         states={
             'readonly': Or(
                     STATES['readonly'],
                     Len(Eval('lines')) > 0,
                 ),
         }, depends=DEPENDS+['lines'])
-    feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_feature')
-    owner = fields.Many2One(string='Owner', required=True, select=True,
+    owner = fields.Many2One(
+        string='Owner', required=True,
         model_name='res.user', ondelete='SET NULL',
         states=STATES, depends=DEPENDS)
-    reviewer = fields.Many2One(string='Reviewer', select=True,
+    reviewer = fields.Many2One(
+        string='Reviewer',
         help='Group of users who have write access to the cashbook.',
         model_name='res.group', ondelete='SET NULL',
         states=STATES, depends=DEPENDS)
-    observer = fields.Many2One(string='Observer', select=True,
+    observer = fields.Many2One(
+        string='Observer',
         help='Group of users who have read-only access to the cashbook.',
         model_name='res.group', ondelete='SET NULL',
         states=STATES, depends=DEPENDS)
-    lines = fields.One2Many(string='Lines', field='cashbook',
+    lines = fields.One2Many(
+        string='Lines', field='cashbook',
         model_name='cashbook.line',
         states=STATES, depends=DEPENDS)
-    reconciliations = fields.One2Many(string='Reconciliations',
+    reconciliations = fields.One2Many(
+        string='Reconciliations',
         field='cashbook', model_name='cashbook.recon',
         states=STATES2, depends=DEPENDS2)
-    number_sequ = fields.Many2One(string='Line numbering',
+    number_sequ = fields.Many2One(
+        string='Line numbering',
         help='Number sequence for numbering of the cash book lines.',
         model_name='ir.sequence',
         domain=[
-            ('sequence_type', '=', Id('cashbook', 'sequence_type_cashbook_line')),
+            ('sequence_type', '=',
+                Id('cashbook', 'sequence_type_cashbook_line')),
             ['OR',
                 ('company', '=', None),
-                ('company', '=', Eval('company', -1)),
-                ],
+                ('company', '=', Eval('company', -1))],
             ],
         states=STATES3, depends=DEPENDS2+['company'])
-    number_atcheck = fields.Boolean(string="number when 'Checking'",
-        help="The numbering of the lines is done in the step Check. If the check mark is inactive, this happens with Done.",
+    number_atcheck = fields.Boolean(
+        string="number when 'Checking'",
+        help="The numbering of the lines is done in the step Check. " +
+        "If the check mark is inactive, this happens with Done.",
         states=STATES2, depends=DEPENDS2)
-    start_date = fields.Date(string='Initial Date',
+    start_date = fields.Date(
+        string='Initial Date',
         states={
             'readonly': Or(
                 STATES2['readonly'],
                 Len(Eval('lines')) > 0,
                 ),
             'invisible': STATES2['invisible'],
             'required': ~STATES2['invisible'],
         }, depends=DEPENDS2+['lines'])
-    balance = fields.Function(fields.Numeric(string='Balance',
+    balance = fields.Function(fields.Numeric(
+        string='Balance',
         readonly=True, depends=['currency_digits'],
         help='Balance of bookings to date',
         digits=(16, Eval('currency_digits', 2))),
         'get_balance_cashbook', searcher='search_balance')
-    balance_all = fields.Function(fields.Numeric(string='Total balance',
+    balance_all = fields.Function(fields.Numeric(
+        string='Total balance',
         readonly=True, depends=['currency_digits'],
         help='Balance of all bookings',
         digits=(16, Eval('currency_digits', 2))),
         'get_balance_cashbook', searcher='search_balance')
 
-    balance_ref = fields.Function(fields.Numeric(string='Balance (Ref.)',
+    balance_ref = fields.Function(fields.Numeric(
+        string='Balance (Ref.)',
         help='Balance in company currency',
         readonly=True, digits=(16, Eval('company_currency_digits', 2)),
         states={
             'invisible': ~Bool(Eval('company_currency')),
         }, depends=['company_currency_digits', 'company_currency']),
         'get_balance_cashbook')
-    company_currency = fields.Function(fields.Many2One(readonly=True,
+    company_currency = fields.Function(fields.Many2One(
+        readonly=True,
         string='Company Currency', states={'invisible': True},
         model_name='currency.currency'),
         'on_change_with_company_currency')
     company_currency_digits = fields.Function(fields.Integer(
         string='Currency Digits (Ref.)', readonly=True),
         'on_change_with_currency_digits')
 
-    currency = fields.Many2One(string='Currency', select=True,
+    currency = fields.Many2One(
+        string='Currency',
         model_name='currency.currency',
         states={
             'readonly': Or(
                 STATES2['readonly'],
                 Len(Eval('lines', [])) > 0,
                 ),
         }, depends=DEPENDS2+['lines'])
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits',
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
-    state = fields.Selection(string='State', required=True,
+    state = fields.Selection(
+        string='State', required=True,
         readonly=True, selection=sel_state_book)
     state_string = state.translated('state')
 
-    parent = fields.Many2One(string="Parent",
+    parent = fields.Many2One(
+        string="Parent",
         model_name='cashbook.book', ondelete='RESTRICT')
-    childs = fields.One2Many(string='Children', field='parent',
+    childs = fields.One2Many(
+        string='Children', field='parent',
         model_name='cashbook.book')
 
     @classmethod
     def __register__(cls, module_name):
         super(Book, cls).__register__(module_name)
 
         table = cls.__table_handler__(module_name)
@@ -168,14 +194,40 @@
 
     @classmethod
     def __setup__(cls):
         super(Book, cls).__setup__()
         cls._order.insert(0, ('rec_name', 'ASC'))
         cls._order.insert(0, ('state', 'ASC'))
         t = cls.__table__()
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.btype, Index.Equality())),
+            Index(
+                t,
+                (t.parent, Index.Equality())),
+            Index(
+                t,
+                (t.company, Index.Equality())),
+            Index(
+                t,
+                (t.currency, Index.Equality())),
+            Index(
+                t,
+                (t.state, Index.Equality())),
+            Index(
+                t,
+                (t.owner, Index.Equality())),
+            Index(
+                t,
+                (t.reviewer, Index.Equality())),
+            Index(
+                t,
+                (t.observer, Index.Equality())),
+            })
         cls._sql_constraints.extend([
             ('state_val',
                 Check(t, t.state.in_(['open', 'closed', 'archive'])),
                 'cashbook.msg_book_wrong_state_value'),
             ])
         cls._transitions |= set((
                 ('open', 'closed'),
@@ -241,17 +293,16 @@
         Book2 = Pool().get('cashbook.book')
         tab_book = Book2.__table__()
         table, _ = tables[None]
 
         query = tab_book.select(
                 Case(
                     (tab_book.state == 'open', 0),
-                    else_ = 1),
-                where=tab_book.id==table.id
-                )
+                    else_=1),
+                where=tab_book.id == table.id)
         return [query]
 
     @staticmethod
     def order_rec_name(tables):
         """ order by pos
             a recursive sorting
         """
@@ -260,15 +311,17 @@
     def get_rec_name(self, name):
         """ name, balance, state
         """
         recname = super(Book, self).get_rec_name(name)
         if self.btype:
             return '%(name)s | %(balance)s %(symbol)s | %(state)s' % {
                 'name': recname or '-',
-                'balance': Report.format_number(self.balance or 0.0, None),
+                'balance': Report.format_number(
+                    self.balance or 0.0, None,
+                    digits=getattr(self.currency, 'digits', 2)),
                 'symbol': getattr(self.currency, 'symbol', '-'),
                 'state': self.state_string,
                 }
         return recname
 
     @classmethod
     def get_balance_of_cashbook_sql(cls):
@@ -282,57 +335,59 @@
         tab_book = Book2.__table__()
         context = Transaction().context
 
         query_date = context.get('date', IrDate.today())
 
         # deny invalid date in context
         if isinstance(query_date, str):
-            try :
-                dt1 = date.fromisoformat(query_date)
-            except :
+            try:
+                date.fromisoformat(query_date)
+            except Exception:
                 query_date = IrDate.today()
 
-        query = tab_book.join(tab_line,
-                condition=tab_book.id==tab_line.cashbook,
+        query = tab_book.join(
+                tab_line,
+                condition=tab_book.id == tab_line.cashbook,
             ).select(
                 tab_line.cashbook,
                 tab_book.currency,
                 Sum(Case(
-                    (tab_line.date <= query_date, tab_line.credit - tab_line.debit),
-                    else_ = Decimal('0.0'),
+                    (tab_line.date <= query_date,
+                        tab_line.credit - tab_line.debit),
+                    else_=Decimal('0.0'),
                 )).as_('balance'),
                 Sum(tab_line.credit - tab_line.debit).as_('balance_all'),
                 group_by=[tab_line.cashbook, tab_book.currency],
             )
         return (query, tab_line)
 
     @staticmethod
     def order_balance(tables):
         """ order by balance
         """
         Book2 = Pool().get('cashbook.book')
         (tab_book, tab2) = Book2.get_balance_of_cashbook_sql()
         table, _ = tables[None]
 
-        query = tab_book.select(tab_book.balance,
-                where=tab_book.cashbook==table.id,
-            )
+        query = tab_book.select(
+            tab_book.balance,
+            where=tab_book.cashbook == table.id)
         return [query]
 
     @staticmethod
     def order_balance_all(tables):
         """ order by balance-all
         """
         Book2 = Pool().get('cashbook.book')
         (tab_book, tab2) = Book2.get_balance_of_cashbook_sql()
         table, _ = tables[None]
 
-        query = tab_book.select(tab_book.balance_all,
-                where=tab_book.cashbook==table.id,
-            )
+        query = tab_book.select(
+            tab_book.balance_all,
+            where=tab_book.cashbook == table.id)
         return [query]
 
     @classmethod
     def search_balance(cls, name, clause):
         """ search in 'balance'
         """
         (tab_line, tab2) = cls.get_balance_of_cashbook_sql()
@@ -357,67 +412,71 @@
         MemCache = pool.get('cashbook.memcache')
         tab_book = Book2.__table__()
         tab_comp = Company.__table__()
         cursor = Transaction().connection.cursor()
         context = Transaction().context
 
         result = {
-            x:{y.id: Decimal('0.0') for y in cashbooks}
-                for x in ['balance', 'balance_all', 'balance_ref']}
+            x: {y.id: Decimal('0.0') for y in cashbooks}
+            for x in ['balance', 'balance_all', 'balance_ref']}
 
         # deny invalid date in context
         query_date = context.get('date', IrDate.today())
         if isinstance(query_date, str):
-            try :
-                dt1 = date.fromisoformat(query_date)
-            except :
+            try:
+                date.fromisoformat(query_date)
+            except Exception:
                 query_date = IrDate.today()
 
         cache_keys = {
-                x.id: MemCache.get_key_by_record(
-                    name = 'get_balance_cashbook',
-                    record = x,
-                    query = [{
-                            'model': 'cashbook.line',
-                            'query': [('cashbook.parent', 'child_of', [x.id])],
-                        }, {
-                            'model': 'currency.currency.rate',
-                            'query': [('currency.id', '=', x.currency.id)],
-                            'cachekey' if ENA_CURRKEY else 'disabled': CACHEKEY_CURRENCY % x.currency.id,
-                        }, ],
-                    addkeys = [query_date.isoformat()])
-                for x in cashbooks
-            }
+            x.id: MemCache.get_key_by_record(
+                name='get_balance_cashbook',
+                record=x,
+                query=[{
+                    'model': 'cashbook.line',
+                    'query': [('cashbook.parent', 'child_of', [x.id])],
+                    }, {
+                    'model': 'currency.currency.rate',
+                        'query': [('currency.id', '=', x.currency.id)],
+                        'cachekey' if ENA_CURRKEY
+                        else 'disabled': CACHEKEY_CURRENCY % x.currency.id,
+                    }, ],
+                addkeys=[query_date.isoformat()])
+            for x in cashbooks}
 
         # read from cache
         (todo_cashbook, result) = MemCache.read_from_cache(
             cashbooks, cache_keys, names, result)
         if len(todo_cashbook) == 0:
             return result
 
         # query balances of cashbooks and sub-cashbooks
         with Transaction().set_context({
-            'date': query_date,
-            }):
+                'date': query_date}):
             (tab_line, tab2) = cls.get_balance_of_cashbook_sql()
             tab_subids = sub_ids_hierarchical('cashbook.book')
-            query = tab_book.join(tab_subids,
-                    condition=tab_book.id==tab_subids.parent,
-                ).join(tab_comp,
-                    condition=tab_book.company==tab_comp.id,
-                ).join(tab_line,
-                    condition=tab_line.cashbook==AnyInArray(tab_subids.subids),
+            query = tab_book.join(
+                    tab_subids,
+                    condition=tab_book.id == tab_subids.parent,
+                ).join(
+                    tab_comp,
+                    condition=tab_book.company == tab_comp.id,
+                ).join(
+                    tab_line,
+                    condition=tab_line.cashbook == AnyInArray(
+                        tab_subids.subids),
                 ).select(
                     tab_book.id,
                     tab_book.currency.as_('to_currency'),
                     tab_line.currency.as_('from_currency'),
                     tab_comp.currency.as_('company_currency'),
                     Sum(tab_line.balance).as_('balance'),
                     Sum(tab_line.balance_all).as_('balance_all'),
-                    group_by=[tab_book.id, tab_line.currency, tab_comp.currency],
+                    group_by=[
+                        tab_book.id, tab_line.currency, tab_comp.currency],
                     where=tab_book.id.in_([x.id for x in todo_cashbook]),
                 )
             cursor.execute(*query)
             records = cursor.fetchall()
 
             for record in records:
                 result['balance'][record[0]] += Currency.compute(
@@ -492,50 +551,48 @@
         for books, values in zip(actions, actions):
             for book in books:
                 # deny btype-->None if lines not empty
                 if 'btype' in values.keys():
                     if (values['btype'] is None) and (len(book.lines) > 0):
                         raise UserError(gettext(
                             'cashbook.msg_book_btype_with_lines',
-                            cbname = book.rec_name,
-                            numlines = len(book.lines),
-                            ))
+                            cbname=book.rec_name,
+                            numlines=len(book.lines)))
 
                 if book.state != 'open':
                     # allow state-update, if its the only action
-                    if not (('state' in values.keys()) and (len(values.keys()) == 1)):
+                    if not (('state' in values.keys()) and
+                            (len(values.keys()) == 1)):
                         raise UserError(gettext(
                             'cashbook.msg_book_deny_write',
-                            bookname = book.rec_name,
-                            state_txt = book.state_string,
-                            ))
+                            bookname=book.rec_name,
+                            state_txt=book.state_string))
 
                 # if owner changes, remove book from user-config
                 if 'owner' in values.keys():
                     if book.owner.id != values['owner']:
-                        for x in ['defbook', 'book1', 'book2', 'book3',
-                            'book4', 'book5']:
+                        for x in [
+                                'defbook', 'book1', 'book2', 'book3',
+                                'book4', 'book5']:
                             cfg1 = ConfigUser.search([
                                     ('iduser.id', '=', book.owner.id),
-                                    ('%s.id' % x, '=', book.id),
-                                ])
+                                    ('%s.id' % x, '=', book.id)])
                             if len(cfg1) > 0:
-                                to_write_config.extend([ cfg1, {x: None} ])
+                                to_write_config.extend([cfg1, {x: None}])
         super(Book, cls).write(*args)
 
         if len(to_write_config) > 0:
             ConfigUser.write(*to_write_config)
 
     @classmethod
     def delete(cls, books):
         """ deny delete if book has lines
         """
         for book in books:
             if (len(book.lines) > 0) and (book.state != 'archive'):
                 raise UserError(gettext(
                     'cashbook.msg_book_deny_delete',
-                    bookname = book.rec_name,
-                    booklines = len(book.lines),
-                    ))
+                    bookname=book.rec_name,
+                    booklines=len(book.lines)))
         super(Book, cls).delete(books)
 
 # end Book
```

### Comparing `mds_cashbook-6.0.27/book.xml` & `mds_cashbook-6.8.29/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/category.py` & `mds_cashbook-6.8.29/category.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 
 class Category(tree(separator='/'), ModelSQL, ModelView):
     'Category'
     __name__ = 'cashbook.category'
 
     name = fields.Char(string='Name', required=True, translate=True)
     description = fields.Char(string='Description', translate=True)
-    cattype = fields.Selection(string='Type', required=True,
+    cattype = fields.Selection(
+        string='Type', required=True,
         help='Type of Category', selection=sel_categorytype,
         states={'readonly': Bool(Eval('parent_cattype'))},
         domain=[If(Bool(Eval('parent_cattype')),
                 ('cattype', '=', Eval('parent_cattype', '')),
                 ())],
         depends=['parent_cattype'])
-    parent_cattype = fields.Function(fields.Char(string='Parent Category Type',
+    parent_cattype = fields.Function(fields.Char(
+        string='Parent Category Type',
         readonly=True, states={'invisible': True}),
         'on_change_with_parent_cattype')
 
-    company = fields.Many2One(string='Company', model_name='company.company',
+    company = fields.Many2One(
+        string='Company', model_name='company.company',
         required=True, ondelete="RESTRICT")
-    parent = fields.Many2One(string="Parent",
+    parent = fields.Many2One(
+        string="Parent",
         model_name='cashbook.category', ondelete='RESTRICT')
-    childs = fields.One2Many(string='Children', field='parent',
+    childs = fields.One2Many(
+        string='Children', field='parent',
         model_name='cashbook.category')
 
     @classmethod
     def __register__(cls, module_name):
         super(Category, cls).__register__(module_name)
         table = cls.__table_handler__(module_name)
         table.drop_column('left')
@@ -57,15 +62,16 @@
         cls._order.insert(0, ('rec_name', 'ASC'))
         t = cls.__table__()
         cls._sql_constraints.extend([
                 ('name_uniq',
                     Unique(t, t.name, t.company, t.parent),
                     'cashbook.msg_category_name_unique'),
                 ('name2_uniq',
-                    Exclude(t,
+                    Exclude(
+                        t,
                         (t.name, Equal),
                         (t.cattype, Equal),
                         where=(t.parent == None)),
                     'cashbook.msg_category_name_unique'),
             ])
 
     @classmethod
@@ -102,17 +108,16 @@
         """ check if current category-type is equal to parent
         """
         for category in categories:
             if category.parent:
                 if category.parent.cattype != category.cattype:
                     raise UserError(gettext(
                         'cashbook.msg_category_type_not_like_parent',
-                        parentname = category.parent.rec_name,
-                        catname = category.rec_name,
-                        ))
+                        parentname=category.parent.rec_name,
+                        catname=category.rec_name,))
 
     @classmethod
     def create(cls, vlist):
         """ add debit/credit
         """
         records = super(Category, cls).create(vlist)
         cls.check_category_hierarchy(records)
```

### Comparing `mds_cashbook-6.0.27/category.xml` & `mds_cashbook-6.8.29/category.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/cbreport.py` & `mds_cashbook-6.8.29/cbreport.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     @classmethod
     def get_context(cls, records, header, data):
         """ update context
         """
         Company = Pool().get('company.company')
         context2 = Transaction().context
 
-        context = super(ReconciliationReport, cls).get_context(records, header, data)
+        context = super(
+            ReconciliationReport, cls).get_context(records, header, data)
         context['company'] = Company(context2['company'])
         return context
 
     @classmethod
     def execute(cls, ids, data):
         """ edit filename
         """
@@ -37,31 +38,29 @@
         elif data['model'] == 'cashbook.line':
             line_obj = pool.get(data['model'])(data['id'])
             rep_name = line_obj.cashbook.rec_name[:50]
         elif data['model'] == 'cashbook.recon':
             recon_obj = pool.get(data['model'])(data['id'])
             rep_name = gettext(
                 'cashbook.msg_rep_reconciliation_fname',
-                recname = recon_obj.cashbook.rec_name[:50],
-                date_from = recon_obj.date_from.isoformat(),
-                date_to = recon_obj.date_to.isoformat(),
-                )
-        else :
+                recname=recon_obj.cashbook.rec_name[:50],
+                date_from=recon_obj.date_from.isoformat(),
+                date_to=recon_obj.date_to.isoformat())
+        else:
             raise ValueError('invalid model')
 
-        (ext1, cont1, dirprint, title) = super(ReconciliationReport, cls).execute(ids, data)
+        (ext1, cont1, dirprint, title) = super(
+            ReconciliationReport, cls).execute(ids, data)
 
         return (
             ext1,
             cont1,
             dirprint,
             slugify('%(date)s-%(book)s-%(descr)s' % {
                 'date': IrDate.today().isoformat().replace('-', ''),
                 'book': gettext('cashbook.msg_name_cashbook'),
                 'descr': rep_name,
                 },
                 max_length=100, word_boundary=True, save_order=True),
             )
 
 # end ReconciliationReport
-
-
```

### Comparing `mds_cashbook-6.0.27/cbreport.xml` & `mds_cashbook-6.8.29/cbreport.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/configuration.py` & `mds_cashbook-6.8.29/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,87 +5,99 @@
 
 from trytond.model import ModelSingleton, ModelView, ModelSQL, fields
 from .model import UserMultiValueMixin, UserValueMixin
 from trytond.pyson import Eval, If
 from trytond.pool import Pool
 
 
-field_checked = fields.Boolean(string='Checked',
+field_checked = fields.Boolean(
+    string='Checked',
     help='Show cashbook lines in Checked-state.')
-field_done = fields.Boolean(string='Done',
+field_done = fields.Boolean(
+    string='Done',
     help='Show cashbook lines in Done-state.')
-field_catnamelong = fields.Boolean(string='Category: Show long name',
+field_catnamelong = fields.Boolean(
+    string='Category: Show long name',
     help='Shows the long name of the category in the Category field of a cash book line.')
 
 
 class Configuration(ModelSingleton, ModelSQL, ModelView, UserMultiValueMixin):
     'Configuration'
     __name__ = 'cashbook.configuration'
 
-    date_from = fields.MultiValue(fields.Date(string='Start Date', depends=['date_to'],
+    date_from = fields.MultiValue(fields.Date(
+        string='Start Date', depends=['date_to'],
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ]))
-    date_to = fields.MultiValue(fields.Date(string='End Date', depends=['date_from'],
+    date_to = fields.MultiValue(fields.Date(
+        string='End Date', depends=['date_from'],
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ]))
     checked = fields.MultiValue(field_checked)
     done = fields.MultiValue(field_done)
     catnamelong = fields.MultiValue(field_catnamelong)
-    defbook = fields.MultiValue(fields.Many2One(string='Default Cashbook',
+    defbook = fields.MultiValue(fields.Many2One(
+        string='Default Cashbook',
         help='The default cashbook is selected when you open the booking wizard.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
-    book1 = fields.MultiValue(fields.Many2One(string='Cashbook 1',
+    book1 = fields.MultiValue(fields.Many2One(
+        string='Cashbook 1',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
-    book2 = fields.MultiValue(fields.Many2One(string='Cashbook 2',
+    book2 = fields.MultiValue(fields.Many2One(
+        string='Cashbook 2',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
-    book3 = fields.MultiValue(fields.Many2One(string='Cashbook 3',
+    book3 = fields.MultiValue(fields.Many2One(
+        string='Cashbook 3',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
-    book4 = fields.MultiValue(fields.Many2One(string='Cashbook 4',
+    book4 = fields.MultiValue(fields.Many2One(
+        string='Cashbook 4',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
-    book5 = fields.MultiValue(fields.Many2One(string='Cashbook 5',
+    book5 = fields.MultiValue(fields.Many2One(
+        string='Cashbook 5',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None), ('state', '=', 'open'),
             ]))
 
     @classmethod
     def multivalue_model(cls, field):
         """ get model for value
         """
         pool = Pool()
 
-        if field in ['date_from', 'date_to', 'checked', 'done',
-            'catnamelong', 'defbook', 'book1', 'book2',
-            'book3', 'book4', 'book5']:
+        if field in [
+                'date_from', 'date_to', 'checked', 'done',
+                'catnamelong', 'defbook', 'book1', 'book2',
+                'book3', 'book4', 'book5']:
             return pool.get('cashbook.configuration_user')
         return super(Configuration, cls).multivalue_model(field)
 
     @classmethod
     def default_checked(cls, **pattern):
         return cls.multivalue_model('checked').default_checked()
 
@@ -100,70 +112,78 @@
 # end Configuration
 
 
 class UserConfiguration(ModelSQL, UserValueMixin):
     'User Configuration'
     __name__ = 'cashbook.configuration_user'
 
-    date_from = fields.Date(string='Start Date', depends=['date_to'],
+    date_from = fields.Date(
+        string='Start Date', depends=['date_to'],
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ])
-    date_to = fields.Date(string='End Date', depends=['date_from'],
+    date_to = fields.Date(
+        string='End Date', depends=['date_from'],
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ])
     checked = field_checked
     done = field_done
     catnamelong = field_catnamelong
-    defbook = fields.Many2One(string='Default Cashbook',
+    defbook = fields.Many2One(
+        string='Default Cashbook',
         help='The default cashbook is selected when you open the booking wizard.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
-    book1 = fields.Many2One(string='Cashbook 1',
+    book1 = fields.Many2One(
+        string='Cashbook 1',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
-    book2 = fields.Many2One(string='Cashbook 2',
+    book2 = fields.Many2One(
+        string='Cashbook 2',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
-    book3 = fields.Many2One(string='Cashbook 3',
+    book3 = fields.Many2One(
+        string='Cashbook 3',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
-    book4 = fields.Many2One(string='Cashbook 4',
+    book4 = fields.Many2One(
+        string='Cashbook 4',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
-    book5 = fields.Many2One(string='Cashbook 5',
+    book5 = fields.Many2One(
+        string='Cashbook 5',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
```

### Comparing `mds_cashbook-6.0.27/configuration.xml` & `mds_cashbook-6.8.29/configuration.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/currency.py` & `mds_cashbook-6.8.29/currency.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         MemCache = Pool().get('cashbook.memcache')
 
         super(CurrencyRate, cls).write(*args)
 
         actions = iter(args)
         for rates, values in zip(actions, actions):
             for rate in rates:
-                MemCache.record_update(CACHEKEY_CURRENCY % rate.currency.id, rate)
+                MemCache.record_update(
+                    CACHEKEY_CURRENCY % rate.currency.id, rate)
 
     @classmethod
     def delete(cls, records):
         """ set cache to None
         """
         MemCache = Pool().get('cashbook.memcache')
```

### Comparing `mds_cashbook-6.0.27/group.xml` & `mds_cashbook-6.8.29/group.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/icon/notebook1.svg` & `mds_cashbook-6.8.29/icon/notebook1.svg`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/line.py` & `mds_cashbook-6.8.29/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import ModelView, ModelSQL, Workflow, fields, Check
+from trytond.model import ModelView, ModelSQL, Workflow, fields, Check, Index
 from trytond.pool import Pool
 from trytond.pyson import Eval, If, Or, Bool, Date
 from trytond.transaction import Transaction
 from trytond.report import Report
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from decimal import Decimal
@@ -41,34 +41,40 @@
 
 STATES = {
     'readonly': Or(
             Eval('state', '') != 'edit',
             Eval('state_cashbook', '') != 'open',
         ),
     }
-DEPENDS=['state', 'state_cashbook']
+DEPENDS = ['state', 'state_cashbook']
 
 
 class Line(SecondCurrencyMixin, MemCacheIndexMx, Workflow, ModelSQL, ModelView):
     'Cashbook Line'
     __name__ = 'cashbook.line'
 
-    cashbook = fields.Many2One(string='Cashbook', required=True, select=True,
+    cashbook = fields.Many2One(
+        string='Cashbook', required=True,
         model_name='cashbook.book', ondelete='CASCADE', readonly=True,
         domain=[('btype', '!=', None)])
-    date = fields.Date(string='Date', required=True, select=True,
+    date = fields.Date(
+        string='Date', required=True,
         states=STATES, depends=DEPENDS)
-    month = fields.Function(fields.Integer(string='Month', readonly=True),
+    month = fields.Function(fields.Integer(
+        string='Month', readonly=True),
         'on_change_with_month', searcher='search_month')
     number = fields.Char(string='Number', readonly=True)
-    description = fields.Text(string='Description', select=True,
+    description = fields.Text(
+        string='Description',
         states=STATES, depends=DEPENDS)
-    descr_short = fields.Function(fields.Char(string='Description', readonly=True),
+    descr_short = fields.Function(fields.Char(
+        string='Description', readonly=True),
         'on_change_with_descr_short', searcher='search_descr_short')
-    category = fields.Many2One(string='Category', select=True,
+    category = fields.Many2One(
+        string='Category',
         model_name='cashbook.category', ondelete='RESTRICT',
         states={
             'readonly': Or(
                 STATES['readonly'],
                 Bool(Eval('bookingtype')) == False,
                 ),
             'required': Eval('bookingtype', '').in_(['in', 'out']),
@@ -76,110 +82,133 @@
         }, depends=DEPENDS+['bookingtype'],
         domain=[
             If(
                 Eval('bookingtype', '').in_(['in', 'mvin']),
                 ('cattype', '=', 'in'),
                 ('cattype', '=', 'out'),
             )])
-    category_view = fields.Function(fields.Char(string='Category', readonly=True),
+    category_view = fields.Function(fields.Char(
+        string='Category', readonly=True),
         'on_change_with_category_view', searcher='search_category_view')
-    feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_feature')
-    booktransf_feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    booktransf_feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_booktransf_feature')
 
-    bookingtype = fields.Selection(string='Type', required=True,
-        help='Type of Booking', selection=sel_bookingtype, select=True,
+    bookingtype = fields.Selection(
+        string='Type', required=True,
+        help='Type of Booking', selection=sel_bookingtype,
         states=STATES, depends=DEPENDS)
     bookingtype_string = bookingtype.translated('bookingtype')
-    amount = fields.Numeric(string='Amount', digits=(16, Eval('currency_digits', 2)),
+    amount = fields.Numeric(
+        string='Amount', digits=(16, Eval('currency_digits', 2)),
         required=True,
         states={
             'readonly': Or(
                 STATES['readonly'],
                 Eval('bookingtype', '').in_(['spin', 'spout']),
                 ),
         }, depends=DEPENDS+['currency_digits', 'bookingtype'])
-    debit = fields.Numeric(string='Debit', digits=(16, Eval('currency_digits', 2)),
+    debit = fields.Numeric(
+        string='Debit', digits=(16, Eval('currency_digits', 2)),
         required=True, readonly=True, depends=['currency_digits'])
-    credit = fields.Numeric(string='Credit', digits=(16, Eval('currency_digits', 2)),
+    credit = fields.Numeric(
+        string='Credit', digits=(16, Eval('currency_digits', 2)),
         required=True, readonly=True, depends=['currency_digits'])
 
     # party or cashbook as counterpart
-    booktransf = fields.Many2One(string='Source/Dest',
+    booktransf = fields.Many2One(
+        string='Source/Dest',
         ondelete='RESTRICT', model_name='cashbook.book',
         domain=[
             ('owner.id', '=', Eval('owner_cashbook', -1)),
             ('id', '!=', Eval('cashbook', -1)),
             ('btype', '!=', None),
             ],
         states={
             'readonly': STATES['readonly'],
             'invisible': ~Eval('bookingtype', '').in_(['mvin', 'mvout']),
             'required': Eval('bookingtype', '').in_(['mvin', 'mvout']),
         }, depends=DEPENDS+['bookingtype', 'owner_cashbook', 'cashbook'])
-    party = fields.Many2One(string='Party', model_name='party.party',
+    party = fields.Many2One(
+        string='Party', model_name='party.party',
         ondelete='RESTRICT',
         states={
             'readonly': STATES['readonly'],
-            'invisible': ~Eval('bookingtype', '').in_(['in', 'out', 'spin', 'spout']),
+            'invisible': ~Eval('bookingtype', '').in_(
+                ['in', 'out', 'spin', 'spout']),
         }, depends=DEPENDS+['bookingtype'])
-    payee = fields.Function(fields.Reference(string='Payee', readonly=True,
+    payee = fields.Function(fields.Reference(
+        string='Payee', readonly=True,
         selection=sel_payee), 'on_change_with_payee', searcher='search_payee')
 
     # link to lines created by this record
-    reference = fields.Many2One(string='Reference', readonly=True, select=True,
+    reference = fields.Many2One(
+        string='Reference', readonly=True,
         states={
             'invisible': ~Bool(Eval('reference')),
         }, model_name='cashbook.line', ondelete='CASCADE',
-        help='The current row was created by and is controlled by the reference row.')
-    references = fields.One2Many(string='References',
+        help='The current row was created by and is controlled ' +
+        'by the reference row.')
+    references = fields.One2Many(
+        string='References',
         model_name='cashbook.line',
         help='The rows are created and managed by the current record.',
         states={
             'invisible': ~Bool(Eval('references')),
         }, field='reference', readonly=True)
-    splitlines = fields.One2Many(string='Split booking lines',
+    splitlines = fields.One2Many(
+        string='Split booking lines',
         model_name='cashbook.split',
         help='Rows with different categories form the total sum of the booking',
         states={
             'invisible': ~Eval('bookingtype' '').in_(['spin', 'spout']),
             'readonly': Or(
                 ~Eval('bookingtype' '').in_(['spin', 'spout']),
                 STATES['readonly'],
                 ),
             'required': Eval('bookingtype' '').in_(['spin', 'spout']),
         }, field='line', depends=DEPENDS+['bookingtype'])
 
-    reconciliation = fields.Many2One(string='Reconciliation', readonly=True,
+    reconciliation = fields.Many2One(
+        string='Reconciliation', readonly=True,
         model_name='cashbook.recon', ondelete='SET NULL',
-        domain=[('cashbook.id', '=', Eval('cashbook'))],
+        domain=[('cashbook.id', '=', Eval('cashbook', -1))],
         depends=['cashbook'],
         states={
             'invisible': ~Bool(Eval('reconciliation')),
         })
 
-    balance = fields.Function(fields.Numeric(string='Balance',
+    balance = fields.Function(fields.Numeric(
+        string='Balance',
         digits=(16, Eval('currency_digits', 2)),
-        help='Balance of the cash book up to the current line, if the default sorting applies.',
+        help='Balance of the cash book up to the current line, ' +
+        'if the default sorting applies.',
         readonly=True, depends=['currency_digits']),
         'on_change_with_balance')
 
-    currency = fields.Function(fields.Many2One(model_name='currency.currency',
+    currency = fields.Function(fields.Many2One(
+        model_name='currency.currency',
         string="Currency", readonly=True), 'on_change_with_currency')
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits',
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
 
-    state = fields.Selection(string='State', required=True, readonly=True,
-        select=True, selection=sel_linetype)
+    state = fields.Selection(
+        string='State', required=True, readonly=True,
+        selection=sel_linetype)
     state_string = state.translated('state')
-    state_cashbook = fields.Function(fields.Selection(string='State of Cashbook',
+    state_cashbook = fields.Function(fields.Selection(
+        string='State of Cashbook',
         readonly=True, states={'invisible': True}, selection=sel_state_book),
         'on_change_with_state_cashbook', searcher='search_state_cashbook')
-    owner_cashbook = fields.Function(fields.Many2One(string='Owner', readonly=True,
+    owner_cashbook = fields.Function(fields.Many2One(
+        string='Owner', readonly=True,
         states={'invisible': True}, model_name='res.user'),
         'on_change_with_owner_cashbook')
 
     @classmethod
     def __register__(cls, module_name):
         super(Line, cls).__register__(module_name)
 
@@ -190,14 +219,38 @@
 
     @classmethod
     def __setup__(cls):
         super(Line, cls).__setup__()
         cls._order.insert(0, ('date', 'ASC'))
         cls._order.insert(0, ('state', 'ASC'))
         t = cls.__table__()
+
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.cashbook, Index.Equality())),
+            Index(
+                t,
+                (t.date, Index.Range(order='ASC'))),
+            Index(
+                t,
+                (t.description, Index.Similarity())),
+            Index(
+                t,
+                (t.category, Index.Equality())),
+            Index(
+                t,
+                (t.bookingtype, Index.Equality())),
+            Index(
+                t,
+                (t.state, Index.Equality())),
+            Index(
+                t,
+                (t.reference, Index.Equality())),
+            })
         cls._sql_constraints.extend([
             ('state_val2',
                 Check(t, t.state.in_(['edit', 'check', 'done', 'recon'])),
                 'cashbook.msg_line_wrong_state_value'),
             ])
         cls._transitions |= set((
                 ('edit', 'check'),
@@ -226,16 +279,15 @@
             })
 
     @classmethod
     def view_attributes(cls):
         return super().view_attributes() + [
             ('/tree', 'visual',
                 If(Eval('balance', 0) < 0, 'warning',
-                    If(Eval('date', Date()) > Date(), 'muted', '')
-                    )),
+                    If(Eval('date', Date()) > Date(), 'muted', ''))),
             ]
 
     @classmethod
     def migrate_amount_2nd_currency(cls):
         """ add amount-2nd-currency
         """
         pool = Pool()
@@ -243,21 +295,24 @@
         Book = pool.get('cashbook.book')
         Book2 = pool.get('cashbook.book')
         tab_line = Line2.__table__()
         tab_book = Book.__table__()         # cashbook of line
         tab_book2 = Book2.__table__()       # transfer-target
         cursor = Transaction().connection.cursor()
 
-        query = tab_line.join(tab_book,
+        query = tab_line.join(
+                tab_book,
                 condition=tab_line.cashbook == tab_book.id,
-            ).join(tab_book2,
-                condition=tab_line.booktransf== tab_book2.id,
-            ).select(tab_line.id,
-                where=tab_line.bookingtype.in_(['mvin', 'mvout']) & \
-                    (tab_line.amount_2nd_currency == None) & \
+            ).join(
+                tab_book2,
+                condition=tab_line.booktransf == tab_book2.id,
+            ).select(
+                tab_line.id,
+                where=tab_line.bookingtype.in_(['mvin', 'mvout']) &
+                    (tab_line.amount_2nd_currency == None) &
                     (tab_book.currency != tab_book2.currency)
             )
         lines = Line2.search([('id', 'in', query)])
         to_write = []
         for line in lines:
             values = Line2.add_2nd_currency({
                 'date': line.date,
@@ -266,17 +321,17 @@
                 }, line.currency)
             if 'amount_2nd_currency' in values.keys():
                 values['id'] = line.id
                 to_write.append(values)
 
         for line in to_write:
             qu1 = tab_line.update(
-                    columns = [tab_line.amount_2nd_currency],
-                    values = [line['amount_2nd_currency']],
-                    where = tab_line.id == line['id'],
+                    columns=[tab_line.amount_2nd_currency],
+                    values=[line['amount_2nd_currency']],
+                    where=tab_line.id == line['id'],
                 )
             cursor.execute(*qu1)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('edit')
     def wfedit(cls, lines):
@@ -284,27 +339,26 @@
         """
         pool = Pool()
         Line2 = pool.get('cashbook.line')
 
         to_delete_line = []
         for line in lines:
             if line.reference:
-                if Transaction().context.get('line.allow.wfedit', False) == False:
+                if Transaction().context.get(
+                        'line.allow.wfedit', False) == False:
                     raise UserError(gettext(
                         'cashbook.msg_line_denywf_by_reference',
-                        recname = line.reference.rec_name,
-                        cbook = line.reference.cashbook.rec_name,
-                        ))
+                        recname=line.reference.rec_name,
+                        cbook=line.reference.cashbook.rec_name))
             # delete references
             to_delete_line.extend(list(line.references))
 
         if len(to_delete_line) > 0:
             with Transaction().set_context({
-                'line.allow.wfedit': True,
-                }):
+                    'line.allow.wfedit': True}):
                 Line2.wfedit(to_delete_line)
             Line2.delete(to_delete_line)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('check')
     def wfcheck(cls, lines):
@@ -319,66 +373,66 @@
         for line in lines:
             # deny if date is in range of existing reconciliation
             # allow cashbook-line at range-limits
             if Recon.search_count([
                     ('state', 'in', ['check', 'done']),
                     ('cashbook.id', '=', line.cashbook.id),
                     ('date_from', '<', line.date),
-                    ('date_to', '>', line.date),
-                ]) > 0:
+                    ('date_to', '>', line.date)]) > 0:
                 raise UserError(gettext(
                     'cashbook.msg_line_err_write_to_reconciled',
-                    datetxt = Report.format_date(line.date),
+                    datetxt=Report.format_date(line.date),
                     ))
             # deny if date is at reconciliation limits and two
             # reconciliations exist
             if Recon.search_count([
                     ('state', 'in', ['check', 'done']),
                     ('cashbook.id', '=', line.cashbook.id),
                     ['OR',
                         ('date_from', '=', line.date),
-                        ('date_to', '=', line.date),
-                    ]
-                ]) > 1:
+                        ('date_to', '=', line.date)]]) > 1:
                 raise UserError(gettext(
                     'cashbook.msg_line_err_write_to_reconciled',
-                    datetxt = Report.format_date(line.date),
+                    datetxt=Report.format_date(line.date),
                     ))
 
             if line.reference is None:
                 if line.bookingtype in ['mvout', 'mvin']:
                     # in case of 'mvin' or 'mvout' - add counterpart
                     values = cls.get_counterpart_values(line)
                     values.update(cls.get_debit_credit(values))
                     to_create_line.append(values)
                 elif line.bookingtype in ['spout', 'spin']:
                     # splitbooking can have a transfer - add counterpart
                     for sp_line in line.splitlines:
                         if sp_line.splittype != 'tr':
                             continue
 
-                        values = cls.get_counterpart_values(line,
-                            splitline = sp_line,
-                            values = {
-                            'cashbook': sp_line.booktransf.id,
-                            'description': sp_line.description,
-                            'amount': sp_line.amount \
-                                if sp_line.currency.id == sp_line.booktransf.currency.id \
+                        values = cls.get_counterpart_values(
+                            line, splitline=sp_line,
+                            values={
+                                'cashbook': sp_line.booktransf.id,
+                                'description': sp_line.description,
+                                'amount': sp_line.amount
+                                if sp_line.currency.id == sp_line.
+                                booktransf.currency.id
                                 else sp_line.amount_2nd_currency,
-                            'amount_2nd_currency': sp_line.amount \
-                                if sp_line.currency.id != sp_line.booktransf.currency.id \
+                                'amount_2nd_currency': sp_line.amount
+                                if sp_line.currency.id != sp_line.
+                                booktransf.currency.id
                                 else None,
-                            'bookingtype': 'mvin' \
-                                if line.bookingtype.endswith('out') else 'mvout',
+                                'bookingtype': 'mvin'
+                                if line.bookingtype.endswith('out')
+                                else 'mvout',
                             })
                         values.update(cls.get_debit_credit(values))
                         to_create_line.append(values)
 
             # add number to line
-            if line.cashbook.number_atcheck == True:
+            if line.cashbook.number_atcheck is True:
                 if len(line.number or '') == 0:
                     to_write_line.extend([
                         [line],
                         {
                             'number': line.cashbook.number_sequ.get()
                         }])
 
@@ -453,51 +507,53 @@
         """ short + name
         """
         credit = self.credit if self.credit is not None else Decimal('0.0')
         debit = self.debit if self.debit is not None else Decimal('0.0')
         return '%(date)s|%(type)s|%(amount)s %(symbol)s|%(desc)s [%(category)s]' % {
             'date': Report.format_date(self.date),
             'desc': (self.description or '-')[:40],
-            'amount': Report.format_number(credit - debit, None),
+            'amount': Report.format_number(
+                credit - debit, None,
+                digits=getattr(self.currency, 'digits', 2)),
             'symbol': getattr(self.currency, 'symbol', '-'),
-            'category': self.category_view \
-                if self.bookingtype in ['in', 'out'] \
-                else getattr(self.booktransf, 'rec_name', '-'),
-            'type': gettext('cashbook.msg_line_bookingtype_%s' % self.bookingtype),
-            }
+            'category': self.category_view
+            if self.bookingtype in ['in', 'out']
+            else getattr(self.booktransf, 'rec_name', '-'),
+            'type': gettext(
+                'cashbook.msg_line_bookingtype_%s' %
+                self.bookingtype)}
 
     @staticmethod
     def order_state(tables):
         """ edit = 0, check/done = 1
         """
         Line = Pool().get('cashbook.line')
         tab_line = Line.__table__()
         table, _ = tables[None]
 
         query = tab_line.select(
                 Case(
                     (tab_line.state == 'edit', 1),
                     (tab_line.state.in_(['check', 'recon', 'done']), 0),
-                    else_ = 2),
-                where=tab_line.id==table.id
+                    else_=2),
+                where=tab_line.id == table.id
                 )
         return [query]
 
     @staticmethod
     def order_category_view(tables):
         """ order: name
         """
         table, _ = tables[None]
         Category = Pool().get('cashbook.category')
         tab_cat = Category.__table__()
 
-        tab2 = tab_cat.select(tab_cat.name,
-                where=tab_cat.id==table.category
-            )
-
+        tab2 = tab_cat.select(
+            tab_cat.name,
+            where=tab_cat.id == table.category)
         return [tab2]
 
     @staticmethod
     def order_descr_short(tables):
         """ order by 'description'
         """
         table, _ = tables[None]
@@ -505,16 +561,15 @@
 
     @classmethod
     def search_payee(cls, names, clause):
         """ search in payee for party or cashbook
         """
         return ['OR',
                 ('party.rec_name',) + tuple(clause[1:]),
-                ('booktransf.rec_name',) + tuple(clause[1:]),
-            ]
+                ('booktransf.rec_name',) + tuple(clause[1:])]
 
     @classmethod
     def search_category_view(cls, name, clause):
         """ search in category
         """
         return [('category.rec_name',) + tuple(clause[1:])]
 
@@ -525,18 +580,20 @@
         pool = Pool()
         Line = pool.get('cashbook.line')
         IrDate = pool.get('ir.date')
         tab_line = Line.__table__()
         Operator = fields.SQL_OPERATORS[clause[1]]
 
         dt1 = IrDate.today()
-        query = tab_line.select(tab_line.id,
+        query = tab_line.select(
+            tab_line.id,
             where=Operator(
-                Literal(12 * dt1.year + dt1.month) - \
-                (Literal(12) * DatePart('year', tab_line.date) + DatePart('month', tab_line.date)),
+                Literal(12 * dt1.year + dt1.month) -
+                (Literal(12) * DatePart('year', tab_line.date) +
+                    DatePart('month', tab_line.date)),
                 clause[2]),
             )
         return [('id', 'in', query)]
 
     @classmethod
     def search_state_cashbook(cls, names, clause):
         """ search in state of cashbook
@@ -549,41 +606,44 @@
         """
         return [('description',) + tuple(clause[1:])]
 
     @fields.depends('amount', 'splitlines')
     def on_change_splitlines(self):
         """ update amount if splitlines change
         """
-        self.amount = sum([x.amount for x in self.splitlines if x.amount is not None])
+        self.amount = sum([
+            x.amount for x in self.splitlines if x.amount is not None])
 
-    @fields.depends('bookingtype', 'category', 'splitlines', 'booktransf',\
+    @fields.depends(
+        'bookingtype', 'category', 'splitlines', 'booktransf',
         'currency2nd')
     def on_change_bookingtype(self):
         """ clear category if not valid type
         """
         types = {
             'in': ['in', 'mvin', 'spin'],
             'out': ['out', 'mvout', 'spout'],
             }
 
         if self.bookingtype:
             if self.category:
-                if not self.bookingtype in types.get(self.category.cattype, ''):
+                if self.bookingtype not in types.get(self.category.cattype, ''):
                     self.category = None
 
             if self.bookingtype.startswith('sp'):   # split booking
                 self.category = None
                 self.booktransf = None
                 for spline in self.splitlines:
-                    if not self.bookingtype in types.get(getattr(spline.category, 'cattype', '-'), ''):
+                    if self.bookingtype not in types.get(
+                            getattr(spline.category, 'cattype', '-'), ''):
                         spline.category = None
-            elif self.bookingtype.startswith('mv'): # transfer
+            elif self.bookingtype.startswith('mv'):     # transfer
                 self.splitlines = []
                 self.category = None
-            else :                                  # category
+            else:                                       # category
                 self.splitlines = []
                 self.booktransf = None
             self.currency2nd = self.on_change_with_currency2nd()
 
     @fields.depends('cashbook', '_parent_cashbook.btype')
     def on_change_with_feature(self, name=None):
         """ get feature-set
@@ -616,24 +676,24 @@
                     return 'party.party,%d' % self.party.id
             elif self.bookingtype in ['mvin', 'mvout']:
                 if self.booktransf:
                     return 'cashbook.book,%d' % self.booktransf.id
 
     @fields.depends('category')
     def on_change_with_category_view(self, name=None):
-        """ show optimizef form of category for list-view
+        """ show optimized form of category for list-view
         """
         Configuration = Pool().get('cashbook.configuration')
 
         if self.category:
             cfg1 = Configuration.get_singleton()
 
-            if getattr(cfg1, 'catnamelong', True) == True:
+            if getattr(cfg1, 'catnamelong', True) is True:
                 return self.category.rec_name
-            else :
+            else:
                 return self.category.name
 
     @fields.depends('date')
     def on_change_with_month(self, name=None):
         """ get difference of month to current date
         """
         IrDate = Pool().get('ir.date')
@@ -669,15 +729,17 @@
         """
         if self.cashbook:
             return self.cashbook.currency.digits
         else:
             return 2
 
     @classmethod
-    def get_balance_of_line(cls, line, field_name='amount', credit_name='credit', debit_name='debit'):
+    def get_balance_of_line(
+            cls, line, field_name='amount', credit_name='credit',
+            debit_name='debit'):
         """ get balance of current line,
             try to speed up by usage of last reconcilitaion
         """
         pool = Pool()
         Reconciliation = pool.get('cashbook.recon')
         Line2 = pool.get('cashbook.line')
 
@@ -695,16 +757,15 @@
                 ], order=[('date_from', 'DESC')], limit=1)
             if len(recons) > 0:
                 query2.append([
                         ('date', '>=', recons[0].date_to),
                         ('date', '<=', line2.date),
                         ['OR',
                             ('reconciliation', '=', None),
-                            ('reconciliation.id', '!=', recons[0]),
-                        ],
+                            ('reconciliation.id', '!=', recons[0])],
                     ])
                 end_value = getattr(recons[0], 'end_%s' % field_name)
             return (query2, end_value)
 
         if line.cashbook:
             query = [
                 ('cashbook.id', '=', line.cashbook.id),
@@ -715,21 +776,22 @@
             # this will speed up calculation of by-line-balance
             if line.date is not None:
                 if line.reconciliation:
                     if line.reconciliation.state == 'done':
                         query.append(
                             ('reconciliation.id', '=', line.reconciliation.id),
                             )
-                        balance = getattr(line.reconciliation, 'start_%s' % field_name)
-                    else :
+                        balance = getattr(
+                            line.reconciliation, 'start_%s' % field_name)
+                    else:
                         (query2, balance2) = get_from_last_recon(line)
                         query.extend(query2)
                         if balance2 is not None:
                             balance = balance2
-                else :
+                else:
                     (query2, balance2) = get_from_last_recon(line)
                     query.extend(query2)
                     if balance2 is not None:
                         balance = balance2
 
             lines = Line2.search(query)
             for line3 in lines:
@@ -739,41 +801,41 @@
                 if (line_credit is not None) or (line_debit is not None):
                     balance += line_credit - line_debit
 
                 if line3.id == line.id:
                     break
             return balance
 
-    @fields.depends('id', 'date', 'cashbook', \
-        '_parent_cashbook.id', 'reconciliation', \
-        '_parent_reconciliation.start_amount',\
-        '_parent_reconciliation.state')
+    @fields.depends(
+        'id', 'date', 'cashbook', '_parent_cashbook.id', 'reconciliation',
+        '_parent_reconciliation.start_amount', '_parent_reconciliation.state')
     def on_change_with_balance(self, name=None):
         """ compute balance until current line, with current sort order,
             try to use a reconciliation as start to speed up calculation
         """
         Line2 = Pool().get('cashbook.line')
-        return Line2.get_balance_of_line(self,
-            field_name='amount',
-            credit_name='credit',
+        return Line2.get_balance_of_line(
+            self, field_name='amount', credit_name='credit',
             debit_name='debit')
 
     @classmethod
     def clear_by_bookingtype(cls, values, line=None):
         """ clear some fields by value of bookingtype
         """
         values2 = {}
         values2.update(values)
 
-        bookingtype = values2.get('bookingtype', getattr(line, 'bookingtype', None))
+        bookingtype = values2.get(
+            'bookingtype', getattr(line, 'bookingtype', None))
         if (bookingtype in ['in', 'out', 'mvin', 'mvout']) and \
                 ('splitlines' not in values2.keys()):
             if line:
                 if len(line.splitlines) > 0:
-                    values2['splitlines'] = [('delete', [x.id for x in line.splitlines])]
+                    values2['splitlines'] = [
+                        ('delete', [x.id for x in line.splitlines])]
 
         if bookingtype in ['in', 'out']:
             values2['booktransf'] = None
 
         if bookingtype in ['spin', 'spout']:
             values2['category'] = None
             values2['booktransf'] = None
@@ -784,59 +846,56 @@
 
     @classmethod
     def get_counterpart_values(cls, line, splitline=None, values={}):
         """ get values to create counter-part of
             transfer booking
         """
         line_currency = getattr(line.currency, 'id', None)
-        booktransf_currency = getattr(getattr(line.booktransf, 'currency', {}), 'id', None)
+        booktransf_currency = getattr(getattr(
+            line.booktransf, 'currency', {}), 'id', None)
 
         result = {
             'cashbook': getattr(line.booktransf, 'id', None),
             'bookingtype': 'mvin' if line.bookingtype == 'mvout' else 'mvout',
             'date': line.date,
             'description': line.description,
             'booktransf': line.cashbook.id,
             'reference': line.id,
-            'amount': line.amount \
-                if line_currency == booktransf_currency \
-                else line.amount_2nd_currency,
-            'amount_2nd_currency': line.amount \
-                if line_currency != booktransf_currency \
-                else None,
-            }
+            'amount': line.amount
+            if line_currency == booktransf_currency
+            else line.amount_2nd_currency,
+            'amount_2nd_currency': line.amount
+            if line_currency != booktransf_currency else None}
         # update values from 'values'
         result.update(values)
         return result
 
     @classmethod
     def get_debit_credit(cls, values, line=None):
         """ compute debit/credit from amount
         """
         if isinstance(values, dict):
-            type_ = values.get('bookingtype', getattr(line, 'bookingtype', None))
+            type_ = values.get(
+                'bookingtype', getattr(line, 'bookingtype', None))
             amount = values.get('amount', None)
-        else :
-            type_ = getattr(values, 'bookingtype', getattr(line, 'bookingtype', None))
+        else:
+            type_ = getattr(
+                values, 'bookingtype', getattr(line, 'bookingtype', None))
             amount = getattr(values, 'amount', None)
 
         result = {}
         if type_:
             if amount is not None:
                 if type_ in ['in', 'mvin', 'spin']:
                     result.update({
-                        'debit': Decimal('0.0'),
-                        'credit': amount,
-                        })
+                        'debit': Decimal('0.0'), 'credit': amount})
                 elif type_ in ['out', 'mvout', 'spout']:
                     result.update({
-                        'debit': amount,
-                        'credit': Decimal('0.0'),
-                        })
-                else :
+                        'debit': amount, 'credit': Decimal('0.0')})
+                else:
                     raise ValueError('invalid "bookingtype"')
         return result
 
     @classmethod
     def validate(cls, lines):
         """ deny date before 'start_date' of cashbook
         """
@@ -847,120 +906,116 @@
             'out': ['out', 'mvout', 'spout'],
             }
 
         for line in lines:
             if line.date < line.cashbook.start_date:
                 raise UserError(gettext(
                     'cashbook.msg_line_date_before_book',
-                    datebook = Report.format_date(line.cashbook.start_date),
-                    recname = line.rec_name,
-                    ))
+                    datebook=Report.format_date(line.cashbook.start_date),
+                    recname=line.rec_name))
 
             # line: category <--> bookingtype?
             if line.category:
-                if not line.bookingtype in types[line.category.cattype]:
+                if line.bookingtype not in types[line.category.cattype]:
                     raise UserError(gettext(
                         'cashbook.msg_line_invalid_category',
-                        recname = line.rec_name,
-                        booktype = line.bookingtype_string,
-                        ))
+                        recname=line.rec_name,
+                        booktype=line.bookingtype_string))
 
             # splitline: category <--> bookingtype?
             for spline in line.splitlines:
                 if spline.splittype != 'cat':
                     continue
-                if not line.bookingtype in types[spline.category.cattype]:
+                if line.bookingtype not in types[spline.category.cattype]:
                     raise UserError(gettext(
                         'cashbook.msg_line_split_invalid_category',
-                        recname = line.rec_name,
-                        splitrecname = spline.rec_name,
-                        booktype = line.bookingtype_string,
-                        ))
+                        recname=line.rec_name,
+                        splitrecname=spline.rec_name,
+                        booktype=line.bookingtype_string))
 
     @classmethod
     def check_permission_write(cls, lines, values={}):
         """ deny update if cashbook.line!='open',
         """
         for line in lines:
             # deny write if cashbook is not open
             if line.cashbook.state != 'open':
                 raise UserError(gettext(
                     'cashbook.msg_book_deny_write',
-                    bookname = line.cashbook.rec_name,
-                    state_txt = line.cashbook.state_string,
-                    ))
+                    bookname=line.cashbook.rec_name,
+                    state_txt=line.cashbook.state_string))
 
             # deny write if reconciliation is 'check' or 'done'
             if line.reconciliation:
                 if line.reconciliation.state == 'done':
                     raise UserError(gettext(
                         'cashbook.msg_line_deny_write_by_reconciliation',
-                        recname = line.rec_name,
-                        reconame = line.reconciliation.rec_name,
-                        ))
+                        recname=line.rec_name,
+                        reconame=line.reconciliation.rec_name))
 
             # deny write if line is not 'Edit'
             if line.state != 'edit':
                 # allow state-update, if its the only action
-                if not ((len(set({'state', 'reconciliation', 'number'}).intersection(values.keys())) > 0) \
-                    and (len(values.keys()) == 1)):
+                if not ((len(set({
+                            'state', 'reconciliation', 'number'
+                        }).intersection(values.keys())) > 0)
+                        and (len(values.keys()) == 1)):
                     raise UserError(gettext(
                         'cashbook.msg_line_deny_write',
-                        recname = line.rec_name,
-                        state_txt = line.state_string,
-                        ))
+                        recname=line.rec_name,
+                        state_txt=line.state_string))
 
     @classmethod
     def check_permission_delete(cls, lines):
         """ deny delete if book is not 'open' or wf is not 'edit'
         """
         for line in lines:
             if line.cashbook.state == 'closed':
                 raise UserError(gettext(
                     'cashbook.msg_line_deny_delete1',
-                    linetxt = line.rec_name,
-                    bookname = line.cashbook.rec_name,
-                    bookstate = line.cashbook.state_string,
-                    ))
+                    linetxt=line.rec_name,
+                    bookname=line.cashbook.rec_name,
+                    bookstate=line.cashbook.state_string))
             if line.state != 'edit':
                 raise UserError(gettext(
                     'cashbook.msg_line_deny_delete2',
-                    linetxt = line.rec_name,
-                    linestate = line.state_string,
-                    ))
+                    linetxt=line.rec_name,
+                    linestate=line.state_string))
 
     @classmethod
     def update_values_by_splitlines(cls, lines):
         """ update amounts from split-lines
         """
         to_write = []
         for line in lines:
             amount = sum([x.amount for x in line.splitlines])
             if amount != line.amount:
-                to_write.extend([ [line], {'amount': amount,} ])
+                to_write.extend([[line], {'amount': amount}])
         return to_write
 
     @classmethod
     def add_values_from_splitlines(cls, values):
         """ add values for create to line by settings on splitlines
         """
         if ('splitlines' in values.keys()) and ('amount' not in values.keys()):
             for action in values['splitlines']:
                 if action[0] == 'create':
-                    values['amount'] = sum([x.get('amount', None) for x in action[1]])
+                    values['amount'] = sum([
+                        x.get('amount', None) for x in action[1]])
         return values
 
     @classmethod
     def add_2nd_unit_values(cls, values):
         """ extend create-values
         """
         Cashbook = Pool().get('cashbook.book')
         cashbook = values.get('cashbook', None)
         if cashbook:
-            values.update(cls.add_2nd_currency(values, Cashbook(cashbook).currency))
+            values.update(cls.add_2nd_currency(
+                values, Cashbook(cashbook).currency))
         return values
 
     @classmethod
     def get_fields_write_update(cls):
         """ get fields to update on write
         """
         return ['amount', 'bookingtype']
@@ -971,89 +1026,90 @@
         """
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('number', None)
         default.setdefault('state', cls.default_state())
-        return super(Line, cls).copy(moves, default=default)
+        return super(Line, cls).copy(lines, default=default)
 
     @classmethod
     def create(cls, vlist):
         """ add debit/credit
         """
         vlist = [x.copy() for x in vlist]
         for values in vlist:
             values.update(cls.add_values_from_splitlines(values))
             values.update(cls.get_debit_credit(values))
             values.update(cls.clear_by_bookingtype(values))
             values.update(cls.add_2nd_unit_values(values))
 
-            # deny add to reconciliation if state is not 'check', 'recon' or 'done'
+            # deny add to reconciliation if state is
+            # not 'check', 'recon' or 'done'
             if values.get('reconciliation', None):
                 if not values.get('state', '-') in ['check', 'done', 'recon']:
                     date_txt = '-'
                     if values.get('date', None):
                         date_txt = Report.format_date(values.get('date', None))
                     raise UserError(gettext(
                         'cashbook.msg_line_deny_recon_by_state',
-                        recname = '%(date)s|%(descr)s' % {
+                        recname='%(date)s|%(descr)s' % {
                             'date': date_txt,
-                            'descr': values.get('description', '-'),
-                            },
-                        ))
+                            'descr': values.get('description', '-')}))
         return super(Line, cls).create(vlist)
 
     @classmethod
     def write(cls, *args):
         """ deny update if cashbook.line!='open',
             add or update debit/credit
         """
         actions = iter(args)
         to_write = []
         for lines, values in zip(actions, actions):
             cls.check_permission_write(lines, values)
 
             for line in lines:
                 if line.reconciliation:
-                    # deny state-change to 'edit' if line is linked to reconciliation
+                    # deny state-change to 'edit' if line is
+                    # linked to reconciliation
                     if values.get('state', '-') == 'edit':
                         raise UserError(gettext(
                             'cashbook.msg_line_deny_stateedit_with_recon',
-                            recname = line.rec_name,
-                            ))
+                            recname=line.rec_name))
 
-            # deny add to reconciliation if state is not 'check', 'recon' or 'done'
+            # deny add to reconciliation if state is
+            # not 'check', 'recon' or 'done'
             if values.get('reconciliation', None):
                 for line in lines:
-                    if not line.state in ['check', 'done', 'recon']:
+                    if line.state not in ['check', 'done', 'recon']:
                         raise UserError(gettext(
                             'cashbook.msg_line_deny_recon_by_state',
-                            recname = line.rec_name
-                            ))
+                            recname=line.rec_name))
 
             # update debit / credit
             fields_update = cls.get_fields_write_update()
             if len(set(values.keys()).intersection(set(fields_update))) > 0:
                 for line in lines:
                     values2 = {}
                     values2.update(values)
                     values2.update(cls.clear_by_bookingtype(values, line))
 
                     # select required fields in case on 'bookingtype'
                     updt_fields = []
                     updt_fields.extend(values.keys())
                     if 'bookingtype' in values.keys():
-                        updt_fields.extend([x for x in fields_update if x not in values.keys()])
+                        updt_fields.extend([
+                            x for x in fields_update
+                            if x not in values.keys()])
 
                     values2.update(cls.get_debit_credit({
-                            x:values.get(x, getattr(line, x)) for x in updt_fields
-                        }, line=line))
+                            x: values.get(x, getattr(line, x))
+                            for x in updt_fields}, line=line))
                     to_write.extend([lines, values2])
-            else :
+            else:
                 to_write.extend([lines, values])
 
         super(Line, cls).write(*to_write)
 
     @classmethod
     def delete(cls, lines):
         """ deny delete if book is not 'open' or wf is not 'edit'
@@ -1064,31 +1120,35 @@
 # end Line
 
 
 class LineContext(ModelView):
     'Line Context'
     __name__ = 'cashbook.line.context'
 
-    date_from = fields.Date(string='Start Date', depends=['date_to'],
+    date_from = fields.Date(
+        string='Start Date', depends=['date_to'],
         help='Limits the date range for the displayed entries.',
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ])
-    date_to = fields.Date(string='End Date', depends=['date_from'],
+    date_to = fields.Date(
+        string='End Date', depends=['date_from'],
         help='Limits the date range for the displayed entries.',
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ])
-    checked = fields.Boolean(string='Checked',
+    checked = fields.Boolean(
+        string='Checked',
         help='Show account lines in Checked-state.')
-    done = fields.Boolean(string='Done',
+    done = fields.Boolean(
+        string='Done',
         help='Show account lines in Done-state.')
 
     @classmethod
     def default_date_from(cls):
         """ get default from context
         """
         context = Transaction().context
```

### Comparing `mds_cashbook-6.0.27/line.xml` & `mds_cashbook-6.8.29/line.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/locale/de.po` & `mds_cashbook-6.8.29/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/locale/en.po` & `mds_cashbook-6.8.29/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/mds_cashbook.egg-info/SOURCES.txt` & `mds_cashbook-6.8.29/mds_cashbook.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 ./docs/settings.txt
 ./icon/notebook1.svg
 ./locale/de.po
 ./locale/en.po
 ./report/cashbook.fods
 ./report/reconciliation.fods
 ./tests/__init__.py
-./tests/test_book.py
-./tests/test_bookingwiz.py
-./tests/test_category.py
-./tests/test_config.py
-./tests/test_currency.py
-./tests/test_line.py
-./tests/test_reconciliation.py
-./tests/test_splitline.py
-./tests/test_type.py
+./tests/book.py
+./tests/bookingwiz.py
+./tests/category.py
+./tests/config.py
+./tests/currency.py
+./tests/line.py
+./tests/reconciliation.py
+./tests/splitline.py
+./tests/test_module.py
+./tests/type.py
 ./view/book_form.xml
 ./view/book_list.xml
 ./view/book_tree.xml
 ./view/cashbook_line_context_form.xml
 ./view/category_form.xml
 ./view/category_list.xml
 ./view/category_tree.xml
```

### Comparing `mds_cashbook-6.0.27/menu.xml` & `mds_cashbook-6.8.29/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/message.xml` & `mds_cashbook-6.8.29/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/mixin.py` & `mds_cashbook-6.8.29/mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import fields
+from trytond.model import fields, Index
 from trytond.pyson import Eval, Bool, Or
 from trytond.pool import Pool
 from trytond.modules.currency.ir import rate_decimal
 from trytond.transaction import Transaction
 from decimal import Decimal
 
 
 STATES = {
     'readonly': Or(
             Eval('state', '') != 'edit',
             Eval('state_cashbook', '') != 'open',
         ),
     }
-DEPENDS=['state', 'state_cashbook']
+DEPENDS = ['state', 'state_cashbook']
 
 
 class SecondCurrencyMixin:
     """ two fields for 2nd currency: amount + rate
     """
-    amount_2nd_currency = fields.Numeric(string='Amount Second Currency',
+    __slots__ = ()
+
+    amount_2nd_currency = fields.Numeric(
+        string='Amount Second Currency',
         digits=(16, Eval('currency2nd_digits', 2)),
         states={
             'readonly': Or(
                     STATES['readonly'],
                     ~Bool(Eval('currency2nd'))
                 ),
             'required': Bool(Eval('currency2nd')),
             'invisible': ~Bool(Eval('currency2nd')),
         }, depends=DEPENDS+['currency2nd_digits', 'currency2nd'])
-    rate_2nd_currency = fields.Function(fields.Numeric(string='Rate',
+    rate_2nd_currency = fields.Function(fields.Numeric(
+        string='Rate',
         help='Exchange rate between the currencies of the participating cashbooks.',
         digits=(rate_decimal * 2, rate_decimal),
         states={
             'readonly': Or(
                     STATES['readonly'],
                     ~Bool(Eval('currency2nd'))
                 ),
             'required': Bool(Eval('currency2nd')),
             'invisible': ~Bool(Eval('currency2nd')),
         }, depends=DEPENDS+['currency2nd_digits', 'currency2nd']),
         'on_change_with_rate_2nd_currency', setter='set_rate_2nd_currency')
 
-    currency2nd = fields.Function(fields.Many2One(model_name='currency.currency',
+    currency2nd = fields.Function(fields.Many2One(
+        model_name='currency.currency',
         string="2nd Currency", readonly=True), 'on_change_with_currency2nd')
-    currency2nd_digits = fields.Function(fields.Integer(string='2nd Currency Digits',
+    currency2nd_digits = fields.Function(fields.Integer(
+        string='2nd Currency Digits',
         readonly=True), 'on_change_with_currency2nd_digits')
 
     @classmethod
     def add_2nd_currency(cls, values, from_currency):
         """ add second currency amount if missing
         """
         pool = Pool()
@@ -65,39 +71,44 @@
         amount_2nd_currency = values.get('amount_2nd_currency', None)
 
         if (amount is not None) and (booktransf is not None):
             if amount_2nd_currency is None:
                 booktransf = Cashbook(booktransf)
                 if from_currency.id != booktransf.currency.id:
                     with Transaction().set_context({
-                        'date': values.get('date', IrDate.today()),
-                        }):
+                            'date': values.get('date', IrDate.today())}):
                         values['amount_2nd_currency'] = Currency.compute(
                             from_currency,
                             amount,
                             booktransf.currency,
                             )
         return values
 
-    @fields.depends('booktransf', '_parent_booktransf.currency', \
-        'currency', 'amount', 'date', 'amount_2nd_currency', 'rate_2nd_currency')
+    @fields.depends(
+        'booktransf', '_parent_booktransf.currency',
+        'currency', 'amount', 'date', 'amount_2nd_currency',
+        'rate_2nd_currency')
     def on_change_booktransf(self):
         """ update amount_2nd_currency
         """
         self.on_change_rate_2nd_currency()
 
-    @fields.depends('booktransf', '_parent_booktransf.currency', \
-        'currency', 'amount', 'date', 'amount_2nd_currency', 'rate_2nd_currency')
+    @fields.depends(
+        'booktransf', '_parent_booktransf.currency',
+        'currency', 'amount', 'date', 'amount_2nd_currency',
+        'rate_2nd_currency')
     def on_change_amount(self):
         """ update amount_2nd_currency
         """
         self.on_change_rate_2nd_currency()
 
-    @fields.depends('booktransf', '_parent_booktransf.currency', \
-        'currency', 'amount', 'date', 'amount_2nd_currency', 'rate_2nd_currency')
+    @fields.depends(
+        'booktransf', '_parent_booktransf.currency',
+        'currency', 'amount', 'date', 'amount_2nd_currency',
+        'rate_2nd_currency')
     def on_change_rate_2nd_currency(self):
         """ update amount_2nd_currency + rate_2nd_currency
         """
         pool = Pool()
         IrDate = pool.get('ir.date')
         Currency = pool.get('currency.currency')
 
@@ -105,24 +116,24 @@
             self.amount_2nd_currency = None
             self.rate_2nd_currency = None
             return
 
         if self.rate_2nd_currency is None:
             # no rate set, use current rate of target-currency
             with Transaction().set_context({
-                'date': self.date or IrDate.today(),
-                }):
+                    'date': self.date or IrDate.today()}):
                 self.amount_2nd_currency = Currency.compute(
                     self.currency,
                     self.amount,
                     self.booktransf.currency
                     )
                 if self.amount != Decimal('0.0'):
-                    self.rate_2nd_currency = self.amount_2nd_currency / self.amount
-        else :
+                    self.rate_2nd_currency = \
+                        self.amount_2nd_currency / self.amount
+        else:
             self.amount_2nd_currency = self.booktransf.currency.round(
                     self.amount * self.rate_2nd_currency
                 )
 
     @classmethod
     def set_rate_2nd_currency(cls, lines, name, value):
         """ compute amount_2nd_currency, write to db
@@ -157,18 +168,18 @@
         """
         self.rate_2nd_currency = self.on_change_with_rate_2nd_currency()
 
     @fields.depends('amount', 'amount_2nd_currency')
     def on_change_with_rate_2nd_currency(self, name=None):
         """ get current rate from amount
         """
-        Rate =  Pool().get('currency.currency.rate')
+        Rate = Pool().get('currency.currency.rate')
 
         if (self.amount is not None) and \
-            (self.amount_2nd_currency is not None):
+                (self.amount_2nd_currency is not None):
             if self.amount != Decimal('0.0'):
                 exp = Decimal(Decimal(1) / 10 ** Rate.rate.digits[1])
                 return (self.amount_2nd_currency / self.amount).quantize(exp)
 
     @fields.depends('currency', 'booktransf', '_parent_booktransf.currency')
     def on_change_with_currency2nd(self, name=None):
         """ currency of transfer-target
@@ -189,17 +200,24 @@
 
 # end SecondCurrencyMixin
 
 
 class MemCacheIndexMx:
     """ add index to 'create_date' + 'write_date'
     """
+    __slots__ = ()
+
     @classmethod
     def __setup__(cls):
         super(MemCacheIndexMx, cls).__setup__()
+        t = cls.__table__()
         # add index
-        cls.write_date.select = True
-        cls.create_date.select = True
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.write_date, Index.Range())),
+            Index(
+                t,
+                (t.create_date, Index.Range())),
+            })
 
 # end MemCacheIndexMx
-
-
```

### Comparing `mds_cashbook-6.0.27/model.py` & `mds_cashbook-6.8.29/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import MultiValueMixin, ValueMixin, fields, Unique, Model
+from trytond.model import (
+    MultiValueMixin, ValueMixin, fields, Unique, Model, Index)
 from trytond.transaction import Transaction
 from trytond.pool import Pool
 from trytond.cache import MemoryCache
 from trytond.config import config
-from datetime import timedelta, datetime
+from datetime import timedelta
 from decimal import Decimal
-from sql import With, Literal
+from sql import With
 from sql.functions import Function
 from sql.conditionals import Coalesce
 import copy
 
-if config.get('cashbook', 'memcache', default='yes').lower() in ['yes', '1', 'true']:
+if config.get('cashbook', 'memcache', default='yes').lower() \
+        in ['yes', '1', 'true']:
     ENABLE_CACHE = True
 else:
     ENABLE_CACHE = False
 
-if config.get('cashbook', 'sync', default='yes').lower() in ['yes', '1', 'true']:
+if config.get('cashbook', 'sync', default='yes').lower() \
+        in ['yes', '1', 'true']:
     ENABLE_CACHESYNC = True
 else:
     ENABLE_CACHESYNC = False
 
 CACHEKEY_CURRENCY = 'currency-%s'
 
 
@@ -32,14 +35,15 @@
     """input values, including nulls, concatenated into an array.
     """
     __slots__ = ()
     _function = 'ARRAY_AGG'
 
 # end ArrayAgg
 
+
 class ArrayAppend(Function):
     """ sql: array_append
     """
     __slots__ = ()
     _function = 'ARRAY_APPEND'
 
 # end ArrayApppend
@@ -83,80 +87,81 @@
 class MemCache(Model):
     """ store values to cache
     """
     __name__ = 'cashbook.memcache'
 
     _cashbook_value_cache = MemoryCache(
         'cashbook.book.valuecache',
-        context = False,
-        duration = timedelta(seconds=60*60*4))
+        context=False,
+        duration=timedelta(seconds=60*60*4))
 
     @classmethod
     def read_value(cls, cache_key):
         """ read values from cache
         """
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return None
         return copy.deepcopy(cls._cashbook_value_cache.get(cache_key))
 
     @classmethod
     def store_result(cls, records, cache_keys, values, skip_records=[]):
         """ store result to cache
         """
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return
         for record in records:
             if record not in skip_records:
                 continue
-            data = {x:values[x][record.id]
-                        for x in values.keys()
-                            if record.id in values[x].keys()}
-            cls._cashbook_value_cache.set(cache_keys[record.id], copy.deepcopy(data))
-        if ENABLE_CACHESYNC == True:
+            data = {
+                x: values[x][record.id]
+                for x in values.keys() if record.id in values[x].keys()}
+            cls._cashbook_value_cache.set(
+                cache_keys[record.id], copy.deepcopy(data))
+        if ENABLE_CACHESYNC is True:
             cls._cashbook_value_cache.sync(Transaction())
 
     @classmethod
     def store_value(cls, cache_key, values):
         """ store values to cache
         """
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return
         cls._cashbook_value_cache.set(cache_key, copy.deepcopy(values))
 
     @classmethod
     def read_from_cache(cls, records, cache_keys, names, result):
         """ get stored values from memcache
         """
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return (records, result)
 
         todo_records = []
         for record in records:
             values = copy.deepcopy(cls.read_value(cache_keys[record.id]))
             if values:
                 for name in names:
                     if name not in values.keys():
                         continue
                     if values[name] is None:
                         continue
                     if result[name][record.id] is None:
                         result[name][record.id] = Decimal('0.0')
                     result[name][record.id] += values[name]
-            else :
+            else:
                 todo_records.append(record)
         return (todo_records, result)
 
     @classmethod
     def get_key_by_record(cls, name, record, query, addkeys=[]):
         """ read records to build a cache-key
         """
         pool = Pool()
         cursor = Transaction().connection.cursor()
 
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return '-'
 
         fname = [name, str(record.id)]
         fname.extend(addkeys)
 
         # query the last edited record for each item in 'query'
         for line in query:
@@ -169,35 +174,37 @@
                     fname.append(key)
                     continue
 
             Model = pool.get(line['model'])
             tab_model = Model.__table__()
 
             tab_query = Model.search(line['query'], query=True)
-            qu1 = tab_model.join(tab_query,
-                    condition=tab_query.id==tab_model.id,
+            qu1 = tab_model.join(
+                    tab_query,
+                    condition=tab_query.id == tab_model.id,
                 ).select(
                     tab_model.id,
                     tab_model.write_date,
                     tab_model.create_date,
-                    limit = 1,
-                    order_by = [
-                        Coalesce(tab_model.write_date, tab_model.create_date).desc,
+                    limit=1,
+                    order_by=[
+                        Coalesce(
+                            tab_model.write_date, tab_model.create_date).desc,
                         tab_model.id.desc,
                         ],
                 )
             cursor.execute(*qu1)
             records = cursor.fetchall()
             if len(records) > 0:
                 fname.append(cls.genkey(
                     records[0][0],
                     records[0][1],
                     records[0][2],
                     ))
-            else :
+            else:
                 fname.append('0')
 
             if 'cachekey' in line.keys():
                 key = cls.store_value(line['cachekey'], fname[-1])
         return '-'.join(fname)
 
     @classmethod
@@ -212,45 +219,45 @@
                 date_val.timestamp() if date_val is not None else '-'),
             ])
 
     @classmethod
     def record_update(cls, cache_key, record):
         """ update cache-value
         """
-        if ENABLE_CACHE == False:
+        if ENABLE_CACHE is False:
             return
-        cls.store_value(cache_key,
+        cls.store_value(
+            cache_key,
             cls.genkey(record.id, record.write_date, record.create_date)
-                if record is not None else None)
+            if record is not None else None)
 
 # end mem_cache
 
 
 def sub_ids_hierarchical(model_name):
     """ get table with id and sub-ids
     """
     Model2 = Pool().get(model_name)
     tab_mod = Model2.__table__()
     tab_mod2 = Model2.__table__()
 
     lines = With('parent', 'id', recursive=True)
     lines.query = tab_mod.select(
             tab_mod.id, tab_mod.id,
-        ) | tab_mod2.join(lines,
-            condition=lines.id==tab_mod2.parent,
-        ).select(
-            lines.parent, tab_mod2.id,
-        )
+        ) | tab_mod2.join(
+            lines,
+            condition=lines.id == tab_mod2.parent,
+        ).select(lines.parent, tab_mod2.id)
     lines.query.all_ = True
 
     query = lines.select(
             lines.parent,
             ArrayAgg(lines.id).as_('subids'),
             group_by=[lines.parent],
-            with_ = [lines])
+            with_=[lines])
     return query
 
 
 def order_name_hierarchical(model_name, tables):
     """ order by pos
         a recursive sorting
     """
@@ -258,38 +265,47 @@
     tab_mod = Model2.__table__()
     tab_mod2 = Model2.__table__()
     table, _ = tables[None]
 
     lines = With('id', 'name', 'name_path', recursive=True)
     lines.query = tab_mod.select(
             tab_mod.id, tab_mod.name, Array(tab_mod.name),
-            where = tab_mod.parent==None,
+            where=tab_mod.parent == None,
         )
-    lines.query |= tab_mod2.join(lines,
-            condition=lines.id==tab_mod2.parent,
+    lines.query |= tab_mod2.join(
+            lines,
+            condition=lines.id == tab_mod2.parent,
         ).select(
-            tab_mod2.id, tab_mod2.name, ArrayAppend(lines.name_path, tab_mod2.name),
+            tab_mod2.id,
+            tab_mod2.name,
+            ArrayAppend(lines.name_path, tab_mod2.name),
         )
     lines.query.all_ = True
 
     query = lines.select(
             ArrayToString(lines.name_path, '/').as_('rec_name'),
-            where = table.id==lines.id,
-            with_ = [lines])
+            where=table.id == lines.id,
+            with_=[lines])
     return [query]
 
 
 class UserValueMixin(ValueMixin):
-    iduser = fields.Many2One(model_name='res.user', string="User",
-        select=True, ondelete='CASCADE', required=True)
+    iduser = fields.Many2One(
+        model_name='res.user', string="User",
+        ondelete='CASCADE', required=True)
 
     @classmethod
     def __setup__(cls):
         super(UserValueMixin, cls).__setup__()
         tab_val = cls.__table__()
+        cls._sql_indexes.update({
+            Index(
+                tab_val,
+                (tab_val.iduser, Index.Equality())),
+            })
         cls._sql_constraints.extend([
             ('val_uniq',
                 Unique(tab_val, tab_val.iduser),
                 'cashbook.msg_setting_already_exists'),
             ])
 
 # end UserValueMixin
@@ -309,10 +325,11 @@
             pattern = self.updt_multivalue_pattern(pattern)
         return super(UserMultiValueMixin, self).get_multivalue(name, **pattern)
 
     def set_multivalue(self, name, value, **pattern):
         Value = self.multivalue_model(name)
         if issubclass(Value, UserValueMixin):
             pattern = self.updt_multivalue_pattern(pattern)
-        return super(UserMultiValueMixin, self).set_multivalue(name, value, **pattern)
+        return super(
+            UserMultiValueMixin, self).set_multivalue(name, value, **pattern)
 
 # end UserMultiValueMixin
```

### Comparing `mds_cashbook-6.0.27/reconciliation.py` & `mds_cashbook-6.8.29/reconciliation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import Workflow, ModelView, ModelSQL, fields
-from trytond.transaction import Transaction
-from trytond.pyson import Eval, If, Or, Bool
+from trytond.model import Workflow, ModelView, ModelSQL, fields, Index
+from trytond.pyson import Eval, If, Or
 from trytond.pool import Pool
 from trytond.report import Report
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from decimal import Decimal
-from sql.operators import Equal, Between
-from sql import Literal, Null
 from datetime import timedelta
 from .book import sel_state_book
 
 
 sel_reconstate = [
     ('edit', 'Edit'),
     ('check', 'Check'),
@@ -25,84 +22,98 @@
 
 STATES = {
     'readonly': Or(
             Eval('state', '') != 'edit',
             Eval('state_cashbook', '') != 'open',
         ),
     }
-DEPENDS=['state', 'state_cashbook']
+DEPENDS = ['state', 'state_cashbook']
 
 
 class Reconciliation(Workflow, ModelSQL, ModelView):
     'Cashbook Reconciliation'
     __name__ = 'cashbook.recon'
 
-    cashbook = fields.Many2One(string='Cashbook', required=True, select=True,
+    cashbook = fields.Many2One(
+        string='Cashbook', required=True,
         model_name='cashbook.book', ondelete='CASCADE', readonly=True)
-    date = fields.Date(string='Date', required=True, select=True,
+    date = fields.Date(
+        string='Date', required=True,
         states=STATES, depends=DEPENDS)
-    feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_feature')
 
-    date_from = fields.Date(string='Start Date',
+    date_from = fields.Date(
+        string='Start Date',
         required=True,
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ],
         states=STATES, depends=DEPENDS+['date_to'])
-    date_to = fields.Date(string='End Date',
-        required=True, select=True,
+    date_to = fields.Date(
+        string='End Date',
+        required=True,
         domain=[
             If(Eval('date_to') & Eval('date_from'),
                 ('date_from', '<=', Eval('date_to')),
                 ()),
             ],
         states=STATES, depends=DEPENDS+['date_from'])
-    start_amount = fields.Numeric(string='Start Amount', required=True,
+    start_amount = fields.Numeric(
+        string='Start Amount', required=True,
         readonly=True, digits=(16, Eval('currency_digits', 2)),
         depends=['currency_digits'])
-    end_amount = fields.Numeric(string='End Amount', required=True,
+    end_amount = fields.Numeric(
+        string='End Amount', required=True,
         readonly=True, digits=(16, Eval('currency_digits', 2)),
         depends=['currency_digits'])
 
-    lines = fields.One2Many(string='Lines', field='reconciliation',
+    lines = fields.One2Many(
+        string='Lines', field='reconciliation',
         model_name='cashbook.line', states=STATES,
         depends=DEPENDS+['date_from', 'date_to', 'cashbook'],
         add_remove=[
             ('cashbook', '=', Eval('cashbook')),
             ('state', 'in', ['check', 'recon', 'done']),
             ('date', '>=', Eval('date_from')),
             ('date', '<=', Eval('date_to')),
         ],
         domain=[
-            ('date', '>=', Eval('date_from')),
-            ('date', '<=', Eval('date_to')),
+            ('date', '>=', Eval('date_from', None)),
+            ('date', '<=', Eval('date_to', None)),
         ])
 
-    currency = fields.Function(fields.Many2One(model_name='currency.currency',
+    currency = fields.Function(fields.Many2One(
+        model_name='currency.currency',
         string="Currency"), 'on_change_with_currency')
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits'),
-            'on_change_with_currency_digits')
-    predecessor = fields.Function(fields.Many2One(string='Predecessor', readonly=True,
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits'),
+        'on_change_with_currency_digits')
+    predecessor = fields.Function(fields.Many2One(
+        string='Predecessor', readonly=True,
         model_name='cashbook.recon'),
         'on_change_with_predecessor')
 
-    state = fields.Selection(string='State', required=True, readonly=True,
-        select=True, selection=sel_reconstate)
+    state = fields.Selection(
+        string='State', required=True, readonly=True,
+        selection=sel_reconstate)
     state_string = state.translated('state')
-    state_cashbook = fields.Function(fields.Selection(string='State of Cashbook',
+    state_cashbook = fields.Function(fields.Selection(
+        string='State of Cashbook',
         readonly=True, states={'invisible': True}, selection=sel_state_book),
         'on_change_with_state_cashbook')
 
     @classmethod
     def __setup__(cls):
         super(Reconciliation, cls).__setup__()
         cls._order.insert(0, ('date_from', 'DESC'))
+        t = cls.__table__()
         cls._transitions |= set((
                 ('edit', 'check'),
                 ('check', 'done'),
                 ('check', 'edit'),
             ))
         cls._buttons.update({
             'wfedit': {
@@ -114,14 +125,31 @@
                 'depends': ['state'],
                 },
             'wfdone': {
                 'invisible': Eval('state') != 'check',
                 'depends': ['state'],
                 },
             })
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.cashbook, Index.Equality())),
+            Index(
+                t,
+                (t.date, Index.Range())),
+            Index(
+                t,
+                (t.date_to, Index.Range())),
+            Index(
+                t,
+                (t.date_from, Index.Range(order='DESC'))),
+            Index(
+                t,
+                (t.state, Index.Equality())),
+            })
 
     def check_overlap_dates(self):
         """ deny overlap of date_from/date_to between records of same cashbook
             allow: date_to=date_from
         """
         Recon = Pool().get('cashbook.recon')
 
@@ -136,41 +164,38 @@
                     [   # 'end' is inside of other record
                         ('date_from', '<', self.date_to),
                         ('date_to', '>=', self.date_to),
                     ],
                     [   # enclose other record
                         ('date_from', '>=', self.date_from),
                         ('date_to', '<=', self.date_to),
-                    ],
-                ],
-            ]
+                    ]]]
 
         if Recon.search_count(query) > 0:
             raise UserError(gettext('cashbook.msg_recon_err_overlap'))
 
     @classmethod
     def check_lines_not_checked(cls, reconciliations):
         """ deny lines in date-range not 'checked', w/o records at date-limit
         """
         Line = Pool().get('cashbook.line')
 
         for reconciliation in reconciliations:
             if Line.search_count([
-                ('date', '>', reconciliation.date_from),
-                ('date', '<', reconciliation.date_to),
-                ('cashbook.id', '=', reconciliation.cashbook.id),
-                ('state', 'not in', ['check', 'recon']),
-                ]) > 0:
+                    ('date', '>', reconciliation.date_from),
+                    ('date', '<', reconciliation.date_to),
+                    ('cashbook.id', '=', reconciliation.cashbook.id),
+                    ('state', 'not in', ['check', 'recon']),
+                    ]) > 0:
                 raise UserError(gettext(
                     'cashbook.mds_recon_deny_line_not_check',
-                    bookname = reconciliation.cashbook.rec_name,
-                    reconame = reconciliation.rec_name,
-                    datefrom = Report.format_date(reconciliation.date_from),
-                    dateto = Report.format_date(reconciliation.date_to),
-                    ))
+                    bookname=reconciliation.cashbook.rec_name,
+                    reconame=reconciliation.rec_name,
+                    datefrom=Report.format_date(reconciliation.date_from),
+                    dateto=Report.format_date(reconciliation.date_to)))
 
     @classmethod
     def get_values_wfedit(cls, reconciliation):
         """ get values for 'to_write' in wf-edit
         """
         values = {
             'start_amount': Decimal('0.0'),
@@ -187,15 +212,15 @@
         """ get values for 'to_write' in wf-check
         """
         Line = Pool().get('cashbook.line')
 
         values = {}
         if reconciliation.predecessor:
             values['start_amount'] = reconciliation.predecessor.end_amount
-        else :
+        else:
             values['start_amount'] = Decimal('0.0')
         values['end_amount'] = values['start_amount']
 
         # add 'checked'-lines to reconciliation
         lines = Line.search([
             ('date', '>=', reconciliation.date_from),
             ('date', '<=', reconciliation.date_to),
@@ -205,15 +230,16 @@
             ])
         if len(lines) > 0:
             values['lines'] = [('add', [x.id for x in lines])]
 
         # add amounts of new lines
         values['end_amount'] += sum([x.credit - x.debit for x in lines])
         # add amounts of already linked lines
-        values['end_amount'] += sum([x.credit - x.debit for x in reconciliation.lines])
+        values['end_amount'] += sum([
+            x.credit - x.debit for x in reconciliation.lines])
         return values
 
     @classmethod
     @ModelView.button
     @Workflow.transition('edit')
     def wfedit(cls, reconciliations):
         """ edit
@@ -244,26 +270,26 @@
         to_write = []
         for reconciliation in reconciliations:
             if reconciliation.predecessor:
                 # predecessor must be 'done'
                 if reconciliation.predecessor.state != 'done':
                     raise UserError(gettext(
                         'cashbook.msg_recon_predecessor_not_done',
-                        recname_p = reconciliation.predecessor.rec_name,
-                        recname_c = reconciliation.rec_name,
-                        ))
+                        recname_p=reconciliation.predecessor.rec_name,
+                        recname_c=reconciliation.rec_name))
 
                 # check if current.date_from == predecessor.date_to
-                if reconciliation.predecessor.date_to != reconciliation.date_from:
+                if reconciliation.predecessor.date_to != \
+                        reconciliation.date_from:
                     raise UserError(gettext(
                         'cashbook.msg_recon_date_from_to_mismatch',
-                        datefrom = Report.format_date(reconciliation.date_from),
-                        dateto = Report.format_date(reconciliation.predecessor.date_to),
-                        recname = reconciliation.rec_name,
-                        ))
+                        datefrom=Report.format_date(reconciliation.date_from),
+                        dateto=Report.format_date(
+                            reconciliation.predecessor.date_to),
+                        recname=reconciliation.rec_name))
 
             to_write.extend([
                 [reconciliation],
                 cls.get_values_wfcheck(reconciliation),
                 ])
 
         if len(to_write) > 0:
@@ -277,55 +303,57 @@
         """
         Line = Pool().get('cashbook.line')
 
         to_wfdone_line = []
         to_wfrecon_line = []
         for reconciliation in reconciliations:
             to_wfrecon_line.extend([
-                    x for x in reconciliation.lines \
-                        if x.state == 'check'
-                ])
+                    x for x in reconciliation.lines
+                    if x.state == 'check'])
             to_wfdone_line.extend([
-                    x for x in reconciliation.lines \
-                        if x.state == 'recon'
-                ])
+                    x for x in reconciliation.lines
+                    if x.state == 'recon'])
 
             # deny if there are lines not linked to reconciliation
             if Line.search_count([
                     ('cashbook.id', '=', reconciliation.cashbook.id),
                     ('reconciliation', '=', None),
                     ['OR',
                         [   # lines inside of date-range
                             ('date', '>', reconciliation.date_from),
                             ('date', '<', reconciliation.date_to),
                         ],
                         # lines at from-date must relate to a reconciliation
-                        ('date', '=', reconciliation.date_from),
-                    ],
-                ]) > 0:
+                        ('date', '=', reconciliation.date_from)],
+                    ]) > 0:
                 raise UserError(gettext(
                     'cashbook.msg_recon_lines_no_linked',
-                    date_from = Report.format_date(reconciliation.date_from),
-                    date_to = Report.format_date(reconciliation.date_to),
-                    ))
+                    date_from=Report.format_date(reconciliation.date_from),
+                    date_to=Report.format_date(reconciliation.date_to),))
 
         if len(to_wfrecon_line) > 0:
             Line.wfrecon(to_wfrecon_line)
             to_wfdone_line.extend(to_wfrecon_line)
         if len(to_wfdone_line) > 0:
             Line.wfdone(to_wfdone_line)
 
     def get_rec_name(self, name):
         """ short + name
         """
         return '%(from)s - %(to)s | %(start_amount)s %(symbol)s - %(end_amount)s %(symbol)s [%(num)s]' % {
-            'from': Report.format_date(self.date_from, None) if self.date_from is not None else '-',
-            'to': Report.format_date(self.date_to, None) if self.date_to is not None else '-',
-            'start_amount': Report.format_number(self.start_amount or 0.0, None),
-            'end_amount': Report.format_number(self.end_amount or 0.0, None),
+            'from': Report.format_date(self.date_from, None)
+            if self.date_from is not None else '-',
+            'to': Report.format_date(self.date_to, None)
+            if self.date_to is not None else '-',
+            'start_amount': Report.format_number(
+                self.start_amount or 0.0, None,
+                digits=getattr(self.currency, 'digits', 2)),
+            'end_amount': Report.format_number(
+                self.end_amount or 0.0, None,
+                digits=getattr(self.currency, 'digits', 2)),
             'symbol': getattr(self.currency, 'symbol', '-'),
             'num': len(self.lines),
             }
 
     @classmethod
     def default_date_from(cls):
         """ 1st day of current month
@@ -455,34 +483,31 @@
         actions = iter(args)
         for reconciliations, values in zip(actions, actions):
             # deny write if chashbook is not open
             for reconciliation in reconciliations:
                 if reconciliation.cashbook.state != 'open':
                     raise UserError(gettext(
                         'cashbook.msg_book_deny_write',
-                        bookname = reconciliation.cashbook.rec_name,
-                        state_txt = reconciliation.cashbook.state_string,
-                        ))
+                        bookname=reconciliation.cashbook.rec_name,
+                        state_txt=reconciliation.cashbook.state_string))
         super(Reconciliation, cls).write(*args)
 
     @classmethod
     def delete(cls, reconciliations):
         """ deny delete if book is not 'open' or wf is not 'edit'
         """
         for reconciliation in reconciliations:
             if reconciliation.cashbook.state == 'closed':
                 raise UserError(gettext(
                     'cashbook.msg_line_deny_delete1',
-                    linetxt = reconciliation.rec_name,
-                    bookname = reconciliation.cashbook.rec_name,
-                    bookstate = reconciliation.cashbook.state_string,
-                    ))
+                    linetxt=reconciliation.rec_name,
+                    bookname=reconciliation.cashbook.rec_name,
+                    bookstate=reconciliation.cashbook.state_string))
             if reconciliation.state != 'edit':
                 raise UserError(gettext(
                     'cashbook.msg_recon_deny_delete2',
-                    recontxt = reconciliation.rec_name,
-                    reconstate = reconciliation.state_string,
-                    ))
+                    recontxt=reconciliation.rec_name,
+                    reconstate=reconciliation.state_string))
 
         super(Reconciliation, cls).delete(reconciliations)
 
 # end Type
```

### Comparing `mds_cashbook-6.0.27/reconciliation.xml` & `mds_cashbook-6.8.29/reconciliation.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/report/cashbook.fods` & `mds_cashbook-6.8.29/report/cashbook.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/report/reconciliation.fods` & `mds_cashbook-6.8.29/report/reconciliation.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/setup.py` & `mds_cashbook-6.8.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 0
+minor_version = 8
 
 requires = ['python-slugify']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -85,14 +85,15 @@
     'Topic :: Office/Business :: Financial :: Accounting',
     'Natural Language :: German',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton cashbook',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_cashbook-6.0.27/splitline.py` & `mds_cashbook-6.8.29/splitline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 
-from trytond.model import ModelView, ModelSQL, Workflow, fields, Check
+from trytond.model import ModelView, ModelSQL, fields, Index
 from trytond.pool import Pool
 from trytond.pyson import Eval, If
 from trytond.report import Report
 from trytond.i18n import gettext
-from trytond.transaction import Transaction
-from .line import sel_linetype, sel_bookingtype, STATES, DEPENDS
+from .line import sel_bookingtype, STATES, DEPENDS
 from .book import sel_state_book
 from .mixin import SecondCurrencyMixin, MemCacheIndexMx
 
 
 sel_linetype = [
     ('cat', 'Category'),
     ('tr', 'Transfer'),
@@ -26,94 +25,133 @@
     ]
 
 
 class SplitLine(SecondCurrencyMixin, MemCacheIndexMx, ModelSQL, ModelView):
     'Split booking line'
     __name__ = 'cashbook.split'
 
-    line = fields.Many2One(string='Line', required=True,
-        select=True, ondelete='CASCADE', model_name='cashbook.line',
+    line = fields.Many2One(
+        string='Line', required=True,
+        ondelete='CASCADE', model_name='cashbook.line',
         readonly=True)
-    description = fields.Text(string='Description',
-        states=STATES, depends=DEPENDS)
-    splittype = fields.Selection(string='Type', required=True,
+    description = fields.Text(
+        string='Description', states=STATES, depends=DEPENDS)
+    splittype = fields.Selection(
+        string='Type', required=True,
         help='Type of split booking line', selection=sel_linetype,
-        states=STATES, depends=DEPENDS, select=True)
-    category = fields.Many2One(string='Category', select=True,
+        states=STATES, depends=DEPENDS)
+    category = fields.Many2One(
+        string='Category',
         model_name='cashbook.category', ondelete='RESTRICT',
         states={
             'readonly': STATES['readonly'],
             'required': Eval('splittype', '') == 'cat',
             'invisible': Eval('splittype', '') != 'cat',
         }, depends=DEPENDS+['bookingtype', 'splittype'],
         domain=[
             If(
                 Eval('bookingtype', '') == 'spin',
                 ('cattype', '=', 'in'),
                 ('cattype', '=', 'out'),
             )])
-    category_view = fields.Function(fields.Char(string='Category', readonly=True),
+    category_view = fields.Function(fields.Char(
+        string='Category', readonly=True),
         'on_change_with_category_view')
-    booktransf = fields.Many2One(string='Source/Dest',
+    booktransf = fields.Many2One(
+        string='Source/Dest',
         ondelete='RESTRICT', model_name='cashbook.book',
         domain=[
             ('owner.id', '=', Eval('owner_cashbook', -1)),
             ('id', '!=', Eval('cashbook', -1)),
             ('btype', '!=', None),
-            ], select=True,
+            ],
         states={
             'readonly': STATES['readonly'],
             'invisible': Eval('splittype', '') != 'tr',
             'required': Eval('splittype', '') == 'tr',
         }, depends=DEPENDS+['bookingtype', 'owner_cashbook', 'cashbook'])
 
-    amount = fields.Numeric(string='Amount', digits=(16, Eval('currency_digits', 2)),
+    amount = fields.Numeric(
+        string='Amount', digits=(16, Eval('currency_digits', 2)),
         required=True, states=STATES, depends=DEPENDS+['currency_digits'])
 
-    date = fields.Function(fields.Date(string='Date', readonly=True),
-        'on_change_with_date')
-    target = fields.Function(fields.Reference(string='Target', readonly=True,
+    date = fields.Function(fields.Date(
+        string='Date', readonly=True), 'on_change_with_date')
+    target = fields.Function(fields.Reference(
+        string='Target', readonly=True,
         selection=sel_target), 'on_change_with_target')
-    currency = fields.Function(fields.Many2One(model_name='currency.currency',
+    currency = fields.Function(fields.Many2One(
+        model_name='currency.currency',
         string="Currency", readonly=True), 'on_change_with_currency')
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits',
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
-    bookingtype = fields.Function(fields.Selection(string='Type', readonly=True,
+    bookingtype = fields.Function(fields.Selection(
+        string='Type', readonly=True,
         selection=sel_bookingtype), 'on_change_with_bookingtype')
-    state = fields.Function(fields.Selection(string='State', readonly=True,
+    state = fields.Function(fields.Selection(
+        string='State', readonly=True,
         selection=sel_linetype), 'on_change_with_state')
-    cashbook = fields.Function(fields.Many2One(string='Cashbook',
+    cashbook = fields.Function(fields.Many2One(
+        string='Cashbook',
         readonly=True, states={'invisible': True}, model_name='cashbook.book'),
         'on_change_with_cashbook')
-    feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_feature')
-    booktransf_feature = fields.Function(fields.Char(string='Feature', readonly=True,
+    booktransf_feature = fields.Function(fields.Char(
+        string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_booktransf_feature')
-    state_cashbook = fields.Function(fields.Selection(string='State of Cashbook',
+    state_cashbook = fields.Function(fields.Selection(
+        string='State of Cashbook',
         readonly=True, states={'invisible': True}, selection=sel_state_book),
         'on_change_with_state_cashbook')
-    owner_cashbook = fields.Function(fields.Many2One(string='Owner', readonly=True,
+    owner_cashbook = fields.Function(fields.Many2One(
+        string='Owner', readonly=True,
         states={'invisible': True}, model_name='res.user'),
         'on_change_with_owner_cashbook')
 
     @classmethod
+    def __setup__(cls):
+        super(SplitLine, cls).__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.line, Index.Equality())),
+            Index(
+                t,
+                (t.splittype, Index.Equality())),
+            Index(
+                t,
+                (t.category, Index.Equality())),
+            Index(
+                t,
+                (t.booktransf, Index.Equality())),
+            })
+
+    @classmethod
     def default_splittype(cls):
         """ default category
         """
         return 'cat'
 
     def get_rec_name(self, name):
         """ short + name
         """
         return '%(type)s|%(amount)s %(symbol)s|%(desc)s [%(target)s]' % {
             'desc': (self.description or '-')[:40],
-            'amount': Report.format_number(self.amount, None),
+            'amount': Report.format_number(
+                self.amount, None,
+                digits=getattr(self.currency, 'digits', 2)),
             'symbol': getattr(self.currency, 'symbol', '-'),
-            'target': self.category_view if self.splittype == 'cat' else self.booktransf.rec_name,
-            'type': gettext('cashbook.msg_line_bookingtype_%s' % self.line.bookingtype),
+            'target': self.category_view
+            if self.splittype == 'cat' else self.booktransf.rec_name,
+            'type': gettext(
+                'cashbook.msg_line_bookingtype_%s' % self.line.bookingtype),
             }
 
     @fields.depends('splittype', 'category', 'booktransf')
     def on_change_splittype(self):
         """ clear category if not valid type
         """
         if self.splittype:
@@ -147,17 +185,17 @@
         """ show optimizef form of category for list-view
         """
         Configuration = Pool().get('cashbook.configuration')
 
         if self.category:
             cfg1 = Configuration.get_singleton()
 
-            if getattr(cfg1, 'catnamelong', True) == True:
+            if getattr(cfg1, 'catnamelong', True) is True:
                 return self.category.rec_name
-            else :
+            else:
                 return self.category.name
 
     @fields.depends('line', '_parent_line.state')
     def on_change_with_state(self, name=None):
         """ get state
         """
         if self.line:
@@ -242,15 +280,15 @@
         vlist = [x.copy() for x in vlist]
         for values in vlist:
             values.update(cls.add_2nd_unit_values(values))
         records = super(SplitLine, cls).create(vlist)
 
         to_update_line = []
         for record in records:
-            if not record.line in to_update_line:
+            if record.line not in to_update_line:
                 to_update_line.append(record.line)
 
         to_write = Line2.update_values_by_splitlines(to_update_line)
         if len(to_write) > 0:
             Line2.write(*to_write)
         return records
 
@@ -264,15 +302,15 @@
         actions = iter(args)
         to_update_line = []
         for records, values in zip(actions, actions):
             Line2.check_permission_write([x.line for x in records])
 
             if 'amount' in values.keys():
                 for record in records:
-                    if not record.line in to_update_line:
+                    if record.line not in to_update_line:
                         to_update_line.append(record.line)
         super(SplitLine, cls).write(*args)
 
         to_write = Line2.update_values_by_splitlines(to_update_line)
         if len(to_write) > 0:
             Line2.write(*to_write)
```

### Comparing `mds_cashbook-6.0.27/splitline.xml` & `mds_cashbook-6.8.29/splitline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/tests/test_book.py` & `mds_cashbook-6.8.29/tests/book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 from datetime import date
 from decimal import Decimal
 
 
-class BookTestCase(ModuleTestCase):
-    'Test cashbook book module'
-    module = 'cashbook'
-
+class BookTestCase(object):
+    """ test cashbook
+    """
     def prep_sequence(self, name='Book Sequ'):
         """ create numbering-equence
         """
         pool = Pool()
         IrSequence = pool.get('ir.sequence')
         IrSequType = pool.get('ir.sequence.type')
 
@@ -86,27 +85,27 @@
                     'category': category.id,
                     'amount': Decimal('10.0'),
                     'party': party.id,
                 }])],
             }])
 
         with Transaction().set_context({
-                'date': date(2022, 5, 5),
-            }):
+                'date': date(2022, 5, 5)}):
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.currency.rec_name, 'usd')
             self.assertEqual(book.currency.rate, Decimal('1.05'))
             self.assertEqual(book.company_currency.rec_name, 'Euro')
             self.assertEqual(book.company_currency.rate, Decimal('1.0'))
 
             self.assertEqual(book.balance, Decimal('10.0'))
             self.assertEqual(book.balance_ref, Decimal('9.52'))
 
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|Amount in USD [Cat1]')
 
     @with_transaction()
     def test_book_create_2nd_currency_hierarchical(self):
         """ create cashbook-hierarchy, in 2nd currency,
             check balance-fields
         """
@@ -141,26 +140,27 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])],
             }])
 
         with Transaction().set_context({
-                'date': date(2022, 5, 5),
-            }):
+                'date': date(2022, 5, 5)}):
             self.assertEqual(book.rec_name, 'Book 1')
             self.assertEqual(book.currency.rec_name, 'Euro')
             self.assertEqual(book.currency.rate, Decimal('1.0'))
             self.assertEqual(book.company_currency, None)
             self.assertEqual(book.balance, Decimal('9.52'))
             self.assertEqual(book.balance_ref, Decimal('9.52'))
             self.assertEqual(len(book.lines), 0)
             self.assertEqual(len(book.childs), 1)
 
-            self.assertEqual(book.childs[0].rec_name, 'Book 1/Book 2 | 10.00 usd | Open')
+            self.assertEqual(
+                book.childs[0].rec_name,
+                'Book 1/Book 2 | 10.00 usd | Open')
             self.assertEqual(book.childs[0].currency.rec_name, 'usd')
             self.assertEqual(book.childs[0].currency.rate, Decimal('1.05'))
             self.assertEqual(book.childs[0].company_currency.rec_name, 'Euro')
             self.assertEqual(book.childs[0].balance, Decimal('10.0'))
             self.assertEqual(book.childs[0].balance_ref, Decimal('9.52'))
             self.assertEqual(len(book.childs[0].lines), 1)
 
@@ -184,15 +184,17 @@
                     'currency': company.currency.id,
                     'number_sequ': self.prep_sequence().id,
                 }])],
             }])
         self.assertEqual(book.name, 'Level 1')
         self.assertEqual(book.rec_name, 'Level 1')
         self.assertEqual(len(book.childs), 1)
-        self.assertEqual(book.childs[0].rec_name, 'Level 1/Level 2 | 0.00 usd | Open')
+        self.assertEqual(
+            book.childs[0].rec_name,
+            'Level 1/Level 2 | 0.00 usd | Open')
 
     @with_transaction()
     def test_book_deny_delete_open(self):
         """ create cashbook, add lines, try to delete in state 'open'
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -216,16 +218,18 @@
                 'amount': Decimal('1.0'),
                 'party': party.id,
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook 'Book 1 | 1.00 usd | Open' cannot be deleted because it contains 1 lines and is not in the status 'Archive'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook 'Book 1 | 1.00 usd | Open' cannot be deleted" +
+            " because it contains 1 lines and is not in the status 'Archive'.",
             Book.delete,
             [book])
 
     @with_transaction()
     def test_book_check_search_and_sort(self):
         """ create cashbook, check search on balance
         """
@@ -332,16 +336,18 @@
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.btype.rec_name, 'CAS - Cash')
         self.assertEqual(book.btype.feature, 'gen')
         self.assertEqual(book.feature, 'gen')
 
-        self.assertRaisesRegex(UserError,
-            "The type cannot be deleted on the cash book 'Book 1 | 1.00 usd | Open' because it still contains 1 lines.",
+        self.assertRaisesRegex(
+            UserError,
+            "The type cannot be deleted on the cash book 'Book 1 | " +
+            "1.00 usd | Open' because it still contains 1 lines.",
             Book.write,
             *[
                 [book],
                 {
                     'btype': None,
                 },
             ])
@@ -389,16 +395,19 @@
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         Book.wfclosed([book])
         self.assertEqual(book.state, 'closed')
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook 'Book 1 | 1.00 usd | Closed' cannot be deleted because it contains 1 lines and is not in the status 'Archive'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook 'Book 1 | 1.00 usd | Closed' cannot be " +
+            "deleted because it contains 1 lines and is not in the " +
+            "status 'Archive'.",
             Book.delete,
             [book])
 
     @with_transaction()
     def test_book_deny_delete_archive(self):
         """ create cashbook, add lines, try to delete in state 'archive'
         """
@@ -459,16 +468,18 @@
             }])
         self.assertEqual(book.name, 'Book 1a')
 
         # wf: open --> closed
         Book.wfclosed([book])
         self.assertEqual(book.state, 'closed')
 
-        self.assertRaisesRegex(UserError,
-            "The cash book 'Book 1a | 1.00 usd | Closed' is 'Closed' and cannot be changed.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cash book 'Book 1a | 1.00 usd | Closed' is 'Closed' " +
+            "and cannot be changed.",
             Book.write,
             *[
                 [book],
                 {
                     'name': 'Book 1b',
                 },
             ])
@@ -482,16 +493,18 @@
                 'name': 'Book 1c',
             }])
         self.assertEqual(book.name, 'Book 1c')
 
         Book.wfclosed([book])
         Book.wfarchive([book])
 
-        self.assertRaisesRegex(UserError,
-            "The cash book 'Book 1c | 0.00 usd | Archive' is 'Archive' and cannot be changed.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cash book 'Book 1c | 0.00 usd | Archive' is 'Archive'" +
+            " and cannot be changed.",
             Book.write,
             *[
                 [book],
                 {
                     'name': 'Book 1d',
                 },
             ])
@@ -533,40 +546,43 @@
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 0.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 0)
 
             # change to user 'frida' read/write book
             with Transaction().set_user(usr_lst[0].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 1)
-                self.assertEqual(books[0].rec_name, 'Fridas book | 0.00 usd | Open')
+                self.assertEqual(
+                    books[0].rec_name,
+                    'Fridas book | 0.00 usd | Open')
 
-                self.assertRaisesRegex(UserError,
+                self.assertRaisesRegex(
+                    UserError,
                     'You are not allowed to access "Cashbook.Name".',
                     Book.write,
                     *[
                         books,
                         {
                             'name': 'Book2',
                         },
                     ])
 
     @with_transaction()
     def test_book_permission_reviewer(self):
-        """ create book + 2x users + 1x reviewer-group, add users to group, check access
+        """ create book + 2x users + 1x reviewer-group,
+            add users to group, check access
         """
         pool = Pool()
         ResUser = pool.get('res.user')
         ResGroup = pool.get('res.group')
         Book = pool.get('cashbook.book')
 
         types = self.prep_type()
@@ -604,32 +620,34 @@
             'btype': types.id,
             'number_sequ': self.prep_sequence().id,
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 0.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 1)
                 self.assertEqual(len(books[0].reviewer.users), 1)
                 self.assertEqual(books[0].reviewer.users[0].rec_name, 'Diego')
 
             # change to user 'frida' read/write book
             with Transaction().set_user(usr_lst[0].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 1)
-                self.assertEqual(books[0].rec_name, 'Fridas book | 0.00 usd | Open')
+                self.assertEqual(
+                    books[0].rec_name,
+                    'Fridas book | 0.00 usd | Open')
 
     @with_transaction()
     def test_book_permission_observer(self):
-        """ create book + 2x users + 1x observer-group, add users to group, check access
+        """ create book + 2x users + 1x observer-group,
+            add users to group, check access
         """
         pool = Pool()
         ResUser = pool.get('res.user')
         ResGroup = pool.get('res.group')
         Book = pool.get('cashbook.book')
 
         types = self.prep_type()
@@ -667,23 +685,24 @@
             'btype': types.id,
             'number_sequ': self.prep_sequence().id,
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 0.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 1)
                 self.assertEqual(len(books[0].observer.users), 1)
                 self.assertEqual(books[0].observer.users[0].rec_name, 'Diego')
 
             # change to user 'frida' read/write book
             with Transaction().set_user(usr_lst[0].id):
                 books = Book.search([])
                 self.assertEqual(len(books), 1)
-                self.assertEqual(books[0].rec_name, 'Fridas book | 0.00 usd | Open')
+                self.assertEqual(
+                    books[0].rec_name,
+                    'Fridas book | 0.00 usd | Open')
 
 # end BookTestCase
```

### Comparing `mds_cashbook-6.0.27/tests/test_bookingwiz.py` & `mds_cashbook-6.8.29/tests/bookingwiz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.exceptions import UserError
 from datetime import date
 from decimal import Decimal
 from unittest.mock import MagicMock
 
 
-class BookingWizardTestCase(ModuleTestCase):
-    'Test cashbook booking wizard module'
-    module = 'cashbook'
-
+class BookingWizardTestCase(object):
+    """ test booking wizard
+    """
     @with_transaction()
     def test_bookwiz_expense(self):
         """ run booking-wizard to store expense
         """
         pool = Pool()
         BookingWiz = pool.get('cashbook.enterbooking', type='wizard')
         Book = pool.get('cashbook.book')
         Category = pool.get('cashbook.category')
         Party = pool.get('party.party')
         IrDate = pool.get('ir.date')
 
         company = self.prep_company()
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             types = self.prep_type()
             book, = Book.create([{
                 'name': 'Cash Book',
                 'btype': types.id,
                 'company': company.id,
                 'currency': company.currency.id,
                 'number_sequ': self.prep_sequence().id,
                 'start_date': date(2022, 1, 1),
                 }])
 
             party, = Party.create([{
                 'name': 'Foodshop Zehlendorf',
-                'addresses':[('create', [{}])],
+                'addresses': [('create', [{}])],
                 }])
 
             categories = Category.create([{
-                    'name':'Income',
+                    'name': 'Income',
                     'cattype': 'in',
                 }, {
                     'name': 'Food',
                     'cattype': 'out',
                 }])
 
             (sess_id, start_state, end_state) = BookingWiz.create()
@@ -84,31 +81,32 @@
 
             IrDate.today = MagicMock(return_value=date(2022, 5, 1))
             result = BookingWiz.execute(sess_id, {'start': r1}, 'save_')
             BookingWiz.delete(sess_id)
             IrDate.today = MagicMock(return_value=date.today())
 
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name, '05/01/2022|Exp|-10.00 usd|Test 1 [Food]')
+            self.assertEqual(
+                book.lines[0].rec_name,
+                '05/01/2022|Exp|-10.00 usd|Test 1 [Food]')
 
     @with_transaction()
     def test_bookwiz_transfer(self):
         """ run booking-wizard to store expense
         """
         pool = Pool()
         BookingWiz = pool.get('cashbook.enterbooking', type='wizard')
         Book = pool.get('cashbook.book')
         Category = pool.get('cashbook.category')
         Party = pool.get('party.party')
         IrDate = pool.get('ir.date')
 
         company = self.prep_company()
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             types = self.prep_type()
             books = Book.create([{
                 'name': 'Cash Book',
                 'btype': types.id,
                 'company': company.id,
                 'currency': company.currency.id,
                 'number_sequ': self.prep_sequence().id,
@@ -120,19 +118,19 @@
                 'currency': company.currency.id,
                 'number_sequ': self.prep_sequence().id,
                 'start_date': date(2022, 1, 1),
                 }])
 
             party, = Party.create([{
                 'name': 'Foodshop Zehlendorf',
-                'addresses':[('create', [{}])],
+                'addresses': [('create', [{}])],
                 }])
 
-            categories = Category.create([{
-                    'name':'Income',
+            Category.create([{
+                    'name': 'Income',
                     'cattype': 'in',
                 }, {
                     'name': 'Food',
                     'cattype': 'out',
                 }])
 
             (sess_id, start_state, end_state) = BookingWiz.create()
@@ -166,11 +164,12 @@
             IrDate.today = MagicMock(return_value=date(2022, 5, 1))
             result = BookingWiz.execute(sess_id, {'start': r1}, 'save_')
             BookingWiz.delete(sess_id)
             IrDate.today = MagicMock(return_value=date.today())
 
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[1].lines), 0)
-            self.assertEqual(books[0].lines[0].rec_name,
+            self.assertEqual(
+                books[0].lines[0].rec_name,
                 '05/01/2022|to|-10.00 usd|Test 1 [Bank | 0.00 usd | Open]')
 
 # end BookingWizardTestCase
```

### Comparing `mds_cashbook-6.0.27/tests/test_category.py` & `mds_cashbook-6.8.29/tests/category.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 
 
-class CategoryTestCase(ModuleTestCase):
-    'Test cashbook categoy module'
-    module = 'cashbook'
-
+class CategoryTestCase(object):
+    """ test category
+    """
     def prep_category(self, name='Cat1', cattype='out'):
         """ create category
         """
         pool = Pool()
-        Company = pool.get('company.company')
         Category = pool.get('cashbook.category')
 
         company = self.prep_company()
         category, = Category.create([{
             'company': company.id,
             'name': name,
             'cattype': cattype,
@@ -115,16 +113,18 @@
 
         self.assertEqual(category.rec_name, 'Level 1')
         self.assertEqual(category.cattype, 'in')
         self.assertEqual(len(category.childs), 1)
         self.assertEqual(category.childs[0].rec_name, 'Level 1/Level 2')
         self.assertEqual(category.childs[0].cattype, 'in')
 
-        self.assertRaisesRegex(UserError,
-            'The value for field "Type" in "Category" is not valid according to its domain.',
+        self.assertRaisesRegex(
+            UserError,
+            'The value "out" for field "Type" in "Level 1/Level 2" of ' +
+            '"Category" is not valid according to its domain.',
             Category.write,
             *[
                 [category.childs[0]],
                 {
                     'cattype': 'out',
                 },
             ])
@@ -136,27 +136,25 @@
             }])
         self.assertEqual(category.rec_name, 'Level 1')
         self.assertEqual(category.cattype, 'out')
         self.assertEqual(len(category.childs), 1)
         self.assertEqual(category.childs[0].rec_name, 'Level 1/Level 2')
         self.assertEqual(category.childs[0].cattype, 'out')
 
-
     @with_transaction()
     def test_category_create_nodupl_at_root(self):
         """ create category, duplicates are allowed at root-level
         """
         pool = Pool()
         Category = pool.get('cashbook.category')
 
         company = self.prep_company()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             cat1, = Category.create([{
                 'name': 'Test 1',
                 'description': 'Info',
                 'cattype': 'in',
                 }])
             self.assertEqual(cat1.name, 'Test 1')
             self.assertEqual(cat1.rec_name, 'Test 1')
@@ -173,15 +171,16 @@
             self.assertEqual(cat2.name, 'Test 1')
             self.assertEqual(cat2.rec_name, 'Test 1')
             self.assertEqual(cat2.description, 'Info')
             self.assertEqual(cat2.company.rec_name, 'm-ds')
             self.assertEqual(cat2.parent, None)
 
             # deny duplicate of same type
-            self.assertRaisesRegex(UserError,
+            self.assertRaisesRegex(
+                UserError,
                 'The category name already exists at this level.',
                 Category.create,
                 [{
                     'name': 'Test 1',
                     'description': 'Info',
                     'cattype': 'in',
                 }])
@@ -192,16 +191,15 @@
         """
         pool = Pool()
         Category = pool.get('cashbook.category')
 
         company = self.prep_company()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             cat1, = Category.create([{
                 'name': 'Test 1',
                 'description': 'Info',
                 'childs': [('create', [{
                     'name': 'Test 1',
                     }])],
                 }])
@@ -219,17 +217,17 @@
         """
         pool = Pool()
         Category = pool.get('cashbook.category')
 
         company = self.prep_company()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
-            self.assertRaisesRegex(UserError,
+                'company': company.id}):
+            self.assertRaisesRegex(
+                UserError,
                 'The category name already exists at this level.',
                 Category.create,
                 [{
                     'name': 'Test 1',
                     'description': 'Info',
                     'childs': [('create', [{
                             'name': 'Test 1',
```

### Comparing `mds_cashbook-6.0.27/tests/test_config.py` & `mds_cashbook-6.8.29/tests/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.exceptions import UserError
 from trytond.modules.company.tests import create_company
 from datetime import date
 from decimal import Decimal
 
 
-class ConfigTestCase(ModuleTestCase):
-    'Test config type module'
-    module = 'cashbook'
-
+class ConfigTestCase(object):
+    """ test config
+    """
     def prep_company(self):
         """ get/create company
         """
         Company = Pool().get('company.company')
 
         company = Company.search([])
         if len(company) > 0:
             company = company[0]
-        else :
+        else:
             company = create_company(name='m-ds')
         return company
 
     def prep_config(self):
         """ store config
         """
         Configuration = Pool().get('cashbook.configuration')
@@ -70,15 +68,15 @@
                 'name': 'Euro',
                 'symbol': '€',
                 'code': 'EUR',
                 'numeric_code': '978',
                 'rounding': Decimal('0.01'),
                 'digits': 2,
                 }])
-        else :
+        else:
             euro = euros[0]
 
         # set company-currency to euro
         self.assertEqual(company.currency.name, 'usd')
         Company.write(*[
             [company],
             {
@@ -165,16 +163,15 @@
             'groups': [('add', [grp_cb.id])],
             }])
         self.assertEqual(len(usr_lst), 2)
         self.assertEqual(usr_lst[0].name, 'Frida')
         self.assertEqual(usr_lst[1].name, 'Diego')
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'frida'
             with Transaction().set_user(usr_lst[0].id):
                 cfg1 = Configuration()
                 cfg1.save()
 
                 cfg2 = Configuration.get_singleton()
                 self.assertEqual(cfg2.date_from, None)
```

### Comparing `mds_cashbook-6.0.27/tests/test_currency.py` & `mds_cashbook-6.8.29/tests/currency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
-from trytond.transaction import Transaction
 from trytond.modules.cashbook.model import CACHEKEY_CURRENCY, ENABLE_CACHE
 from datetime import date
 from decimal import Decimal
 import time
 
 
-class CurrencyTestCase(ModuleTestCase):
-    'Test cache for currency'
-    module = 'cashbook'
-
+class CurrencyTestCase(object):
+    """ test currency
+    """
     @with_transaction()
     def test_currency_update_cache(self):
         """ add/update/del rate of currency, check cache
         """
         pool = Pool()
         MemCache = pool.get('cashbook.memcache')
         Currency = pool.get('currency.currency')
@@ -49,37 +47,36 @@
             }])
         self.assertEqual(len(currency.rates), 1)
 
         # expected key
         value = '%d-c%s' % (
             currency.rates[0].id,
             str(currency.rates[0].create_date.timestamp()))
-        if ENABLE_CACHE == True:
+        if ENABLE_CACHE is True:
             self.assertEqual(MemCache.read_value(cache_key), value)
-        else :
+        else:
             self.assertEqual(MemCache.read_value(cache_key), None)
         time.sleep(1.0)
 
         Currency.write(*[
             [currency],
             {
-                'rates': [('write',
-                    [currency.rates[0].id],
-                    {
+                'rates': [
+                    ('write', [currency.rates[0].id], {
                         'rate': Decimal('1.06'),
                     })],
             }])
         self.assertEqual(len(currency.rates), 1)
 
         value = '%d-w%s' % (
             currency.rates[0].id,
             str(currency.rates[0].write_date.timestamp()))
-        if ENABLE_CACHE == True:
+        if ENABLE_CACHE is True:
             self.assertEqual(MemCache.read_value(cache_key), value)
-        else :
+        else:
             self.assertEqual(MemCache.read_value(cache_key), None)
 
         Currency.write(*[
             [currency],
             {
                 'rates': [('delete', [currency.rates[0].id])],
             }])
```

### Comparing `mds_cashbook-6.0.27/tests/test_line.py` & `mds_cashbook-6.8.29/tests/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 from datetime import date
 from unittest.mock import MagicMock
 from decimal import Decimal
 
 
-class LineTestCase(ModuleTestCase):
-    'Test cashbook line module'
-    module = 'cashbook'
-
+class LineTestCase(object):
+    """ test lines
+    """
     @with_transaction()
     def test_line_check_add_amount2nd_currency(self):
         """ create cashbook, lines, add transfer without
             amount_2nd_currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -72,37 +71,41 @@
                         'description': 'Transfer USD --> EUR',
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR ' +
+            '[Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].amount, Decimal('10.0'))
         # auto-created
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('9.52'))
         self.assertEqual(books[0].lines[0].rate_2nd_currency, Decimal('0.952'))
         Lines.delete(books[0].lines)
 
-       # rate @ 2022-06-01: 1.02
+        # rate @ 2022-06-01: 1.02
         Book.write(*[
             [books[0]],
             {
                 'lines': [('create', [{
                         'date': date(2022, 6, 1),
                         'description': 'Transfer USD --> EUR',
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '06/01/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '06/01/2022|to|-10.00 usd|Transfer USD --> EUR ' +
+            '[Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].amount, Decimal('10.0'))
         # auto-created
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('9.80'))
         self.assertEqual(books[0].lines[0].rate_2nd_currency, Decimal('0.98'))
         Lines.delete(books[0].lines)
 
         Book.write(*[
@@ -114,16 +117,18 @@
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                         'amount_2nd_currency': Decimal('8.5'),
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 usd|Transfer USD --> ' +
+            'EUR [Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].amount, Decimal('10.0'))
         # manual set
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('8.5'))
         self.assertEqual(books[0].lines[0].rate_2nd_currency, Decimal('0.85'))
 
         # update rate to get new amount_2nd_currency
         Lines.write(*[
@@ -201,23 +206,25 @@
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 0)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 usd|Transfer USD --> ' +
+            'EUR [Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('9.52'))
 
         # clear field 'amount_2nd_currency' to prepare for migration
         clear_field = tab_line.update(
-                columns = [tab_line.amount_2nd_currency],
-                values = [None],
-                where = (tab_line.id == books[0].lines[0].id),
+                columns=[tab_line.amount_2nd_currency],
+                values=[None],
+                where=(tab_line.id == books[0].lines[0].id),
             )
         cursor.execute(*clear_field)
 
         # migrate
         Lines.migrate_amount_2nd_currency()
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('9.52'))
 
@@ -225,15 +232,14 @@
     def test_line_check_transfer_2nd_currency_out(self):
         """ create cashbook, lines, transfer amount between
             accounts with different currencies
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Lines = pool.get('cashbook.line')
-        Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
         company = self.prep_company()
 
         # add EURO, set company-currency to EURO
         (usd, euro) = self.prep_2nd_currency(company)
 
@@ -265,46 +271,51 @@
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 0)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 usd|Transfer USD --> ' +
+            'EUR [Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].amount_2nd_currency, Decimal('9.52'))
         self.assertEqual(books[0].lines[0].reference, None)
         self.assertEqual(len(books[0].lines[0].references), 0)
         self.assertEqual(books[0].lines[0].reconciliation, None)
 
         Lines.wfcheck([books[0].lines[0]])
 
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 1)
         self.assertEqual(books[0].lines[0].reference, None)
         self.assertEqual(len(books[0].lines[0].references), 1)
 
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 usd|Transfer USD --> EUR [Book EURO | 9.52 € | Open]')
-        self.assertEqual(books[1].lines[0].rec_name,
-            '05/05/2022|from|9.52 €|Transfer USD --> EUR [Book USD | -10.00 usd | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 usd|Transfer USD --> ' +
+            'EUR [Book EURO | 9.52 € | Open]')
+        self.assertEqual(
+            books[1].lines[0].rec_name,
+            '05/05/2022|from|9.52 €|Transfer USD --> ' +
+            'EUR [Book USD | -10.00 usd | Open]')
         self.assertEqual(books[0].balance, Decimal('-10.0'))
         self.assertEqual(books[0].currency.rec_name, 'usd')
         self.assertEqual(books[1].balance, Decimal('9.52'))
         self.assertEqual(books[1].currency.rec_name, 'Euro')
 
     @with_transaction()
     def test_line_check_transfer_2nd_currency_in(self):
         """ create cashbook, lines, transfer amount between
             accounts with different currencies
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Lines = pool.get('cashbook.line')
-        Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
         company = self.prep_company()
 
         # add EURO, set company-currency to EURO
         (usd, euro) = self.prep_2nd_currency(company)
 
@@ -336,46 +347,51 @@
                         'bookingtype': 'mvin',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 0)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|from|10.00 usd|Transfer USD <-- EUR [Book EURO | 0.00 € | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|from|10.00 usd|Transfer USD <-- ' +
+            'EUR [Book EURO | 0.00 € | Open]')
         self.assertEqual(books[0].lines[0].reference, None)
         self.assertEqual(len(books[0].lines[0].references), 0)
         self.assertEqual(books[0].lines[0].reconciliation, None)
 
         Lines.wfcheck([books[0].lines[0]])
 
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 1)
         self.assertEqual(books[0].lines[0].reference, None)
         self.assertEqual(len(books[0].lines[0].references), 1)
 
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|from|10.00 usd|Transfer USD <-- EUR [Book EURO | -9.52 € | Open]')
-        self.assertEqual(books[1].lines[0].rec_name,
-            '05/05/2022|to|-9.52 €|Transfer USD <-- EUR [Book USD | 10.00 usd | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|from|10.00 usd|Transfer USD <-- ' +
+            'EUR [Book EURO | -9.52 € | Open]')
+        self.assertEqual(
+            books[1].lines[0].rec_name,
+            '05/05/2022|to|-9.52 €|Transfer USD <-- ' +
+            'EUR [Book USD | 10.00 usd | Open]')
         self.assertEqual(books[0].balance, Decimal('10.0'))
         self.assertEqual(books[0].currency.rec_name, 'usd')
         self.assertEqual(books[1].balance, Decimal('-9.52'))
         self.assertEqual(books[1].currency.rec_name, 'Euro')
 
     @with_transaction()
     def test_line_check_transfer_2nd_currency_nocompany(self):
         """ create cashbook, lines, transfer amount between
             accounts with different currencies,
             both currencies are no company-currencies
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Lines = pool.get('cashbook.line')
-        Reconciliation = pool.get('cashbook.recon')
         Currency = pool.get('currency.currency')
         CurrencyRate = pool.get('currency.currency.rate')
 
         types = self.prep_type()
         company = self.prep_company()
 
         # add EURO, set company-currency to EURO
@@ -423,16 +439,18 @@
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'booktransf': books[1].id,
                     }])],
             }])
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[1].lines), 0)
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 CHF|Transfer CHF --> USD [Book USD | 0.00 usd | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 CHF|Transfer CHF --> ' +
+            'USD [Book USD | 0.00 usd | Open]')
         self.assertEqual(books[0].lines[0].reference, None)
         self.assertEqual(len(books[0].lines[0].references), 0)
         self.assertEqual(books[0].lines[0].reconciliation, None)
 
         Lines.wfcheck([books[0].lines[0]])
 
         self.assertEqual(len(books[0].lines), 1)
@@ -441,18 +459,22 @@
         self.assertEqual(len(books[0].lines[0].references), 1)
 
         # 10 CHF --> USD: USD = CHF * 1.05 / 1.04
         # 10 CHF = 10.0961538 USD
         #  EUR | USD | CHF
         # -----+-----+-----  @ 05/02/2022
         #  1.00| 1.05| 1.04
-        self.assertEqual(books[0].lines[0].rec_name,
-            '05/05/2022|to|-10.00 CHF|Transfer CHF --> USD [Book USD | 10.10 usd | Open]')
-        self.assertEqual(books[1].lines[0].rec_name,
-            '05/05/2022|from|10.10 usd|Transfer CHF --> USD [Book CHF | -10.00 CHF | Open]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/05/2022|to|-10.00 CHF|Transfer CHF --> ' +
+            'USD [Book USD | 10.10 usd | Open]')
+        self.assertEqual(
+            books[1].lines[0].rec_name,
+            '05/05/2022|from|10.10 usd|Transfer CHF --> ' +
+            'USD [Book CHF | -10.00 CHF | Open]')
         self.assertEqual(books[0].balance, Decimal('-10.0'))
         self.assertEqual(books[0].currency.rec_name, 'Swiss Franc')
         self.assertEqual(books[1].balance, Decimal('10.10'))
         self.assertEqual(books[1].currency.rec_name, 'usd')
 
     @with_transaction()
     def test_line_check_balance_by_line(self):
@@ -503,76 +525,105 @@
                     'bookingtype': 'in',
                     'amount': Decimal('1.0'),
                     'party': party.id,
                 }])],
             }])
 
         self.assertEqual(len(book.lines), 4)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].balance, Decimal('1.0'))
         self.assertEqual(book.lines[0].reconciliation, None)
         self.assertEqual(book.lines[0].state, 'edit')
         self.assertEqual(book.lines[0].feature, 'gen')
-        self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].balance, Decimal('2.0'))
         self.assertEqual(book.lines[1].reconciliation, None)
         self.assertEqual(book.lines[1].state, 'edit')
-        self.assertEqual(book.lines[2].rec_name, '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
+        self.assertEqual(
+            book.lines[2].rec_name,
+            '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
         self.assertEqual(book.lines[2].balance, Decimal('3.0'))
         self.assertEqual(book.lines[2].reconciliation, None)
         self.assertEqual(book.lines[2].state, 'edit')
-        self.assertEqual(book.lines[3].rec_name, '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
+        self.assertEqual(
+            book.lines[3].rec_name,
+            '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
         self.assertEqual(book.lines[3].balance, Decimal('4.0'))
         self.assertEqual(book.lines[3].reconciliation, None)
         self.assertEqual(book.lines[3].state, 'edit')
 
         Lines.wfcheck([book.lines[0], book.lines[1]])
         recon, = Reconciliation.create([{
-            'cashbook': book.id,
-            }])
-        self.assertEqual(recon.rec_name, '05/01/2022 - 05/02/2022 | 0.00 usd - 0.00 usd [0]')
+                'cashbook': book.id}])
+        self.assertEqual(
+            recon.rec_name,
+            '05/01/2022 - 05/02/2022 | 0.00 usd - 0.00 usd [0]')
 
         Reconciliation.wfcheck([recon])
-        self.assertEqual(recon.rec_name, '05/01/2022 - 05/02/2022 | 0.00 usd - 2.00 usd [2]')
+        self.assertEqual(
+            recon.rec_name,
+            '05/01/2022 - 05/02/2022 | 0.00 usd - 2.00 usd [2]')
 
         self.assertEqual(len(book.lines), 4)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].balance, Decimal('1.0'))
         self.assertEqual(book.lines[0].reconciliation.id, recon.id)
         self.assertEqual(book.lines[0].state, 'check')
-        self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].balance, Decimal('2.0'))
         self.assertEqual(book.lines[1].reconciliation.id, recon.id)
         self.assertEqual(book.lines[1].state, 'check')
-        self.assertEqual(book.lines[2].rec_name, '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
+        self.assertEqual(
+            book.lines[2].rec_name,
+            '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
         self.assertEqual(book.lines[2].balance, Decimal('3.0'))
         self.assertEqual(book.lines[2].reconciliation, None)
         self.assertEqual(book.lines[2].state, 'edit')
-        self.assertEqual(book.lines[3].rec_name, '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
+        self.assertEqual(
+            book.lines[3].rec_name,
+            '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
         self.assertEqual(book.lines[3].balance, Decimal('4.0'))
         self.assertEqual(book.lines[3].reconciliation, None)
         self.assertEqual(book.lines[3].state, 'edit')
 
         Reconciliation.wfdone([recon])
-        self.assertEqual(recon.rec_name, '05/01/2022 - 05/02/2022 | 0.00 usd - 2.00 usd [2]')
+        self.assertEqual(
+            recon.rec_name,
+            '05/01/2022 - 05/02/2022 | 0.00 usd - 2.00 usd [2]')
 
         self.assertEqual(len(book.lines), 4)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].balance, Decimal('1.0'))
         self.assertEqual(book.lines[0].reconciliation.id, recon.id)
         self.assertEqual(book.lines[0].state, 'done')
-        self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].balance, Decimal('2.0'))
         self.assertEqual(book.lines[1].reconciliation.id, recon.id)
         self.assertEqual(book.lines[1].state, 'done')
-        self.assertEqual(book.lines[2].rec_name, '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
+        self.assertEqual(
+            book.lines[2].rec_name,
+            '05/15/2022|Rev|1.00 usd|Text 3 [Cat1]')
         self.assertEqual(book.lines[2].balance, Decimal('3.0'))
         self.assertEqual(book.lines[2].reconciliation, None)
         self.assertEqual(book.lines[2].state, 'edit')
-        self.assertEqual(book.lines[3].rec_name, '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
+        self.assertEqual(
+            book.lines[3].rec_name,
+            '05/17/2022|Rev|1.00 usd|Text 4 [Cat1]')
         self.assertEqual(book.lines[3].balance, Decimal('4.0'))
         self.assertEqual(book.lines[3].reconciliation, None)
         self.assertEqual(book.lines[3].state, 'edit')
 
     @with_transaction()
     def test_line_set_number_with_done(self):
         """ create cashbook + line, write number to line
@@ -584,16 +635,15 @@
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
         category = self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             book, = Book.create([{
                 'name': 'Book 1',
                 'btype': types.id,
                 'company': company.id,
                 'currency': company.currency.id,
                 'number_sequ': self.prep_sequence().id,
                 'start_date': date(2022, 5, 1),
@@ -616,45 +666,55 @@
                 }])
             self.assertEqual(book.name, 'Book 1')
             self.assertEqual(book.btype.rec_name, 'CAS - Cash')
             self.assertEqual(book.state, 'open')
             self.assertEqual(book.number_atcheck, False)
             self.assertEqual(len(book.lines), 2)
             self.assertEqual(book.lines[0].date, date(2022, 5, 1))
-            self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+            self.assertEqual(
+                book.lines[0].rec_name,
+                '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
             self.assertEqual(book.lines[0].state_cashbook, 'open')
             self.assertEqual(book.lines[1].date, date(2022, 5, 2))
-            self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+            self.assertEqual(
+                book.lines[1].rec_name,
+                '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
 
             # add reconciliation
             Book.write(*[
                 [book],
                 {
                     'reconciliations': [('create', [{
                         'date': date(2022, 5, 1),
                         'date_from': date(2022, 5, 1),
                         'date_to': date(2022, 5, 30),
                         }])],
                 }])
             self.assertEqual(len(book.reconciliations), 1)
             self.assertEqual(len(book.reconciliations[0].lines), 0)
-            self.assertEqual(book.reconciliations[0].date_from, date(2022, 5, 1))
-            self.assertEqual(book.reconciliations[0].date_to, date(2022, 5, 30))
+            self.assertEqual(
+                book.reconciliations[0].date_from, date(2022, 5, 1))
+            self.assertEqual(
+                book.reconciliations[0].date_to, date(2022, 5, 30))
             self.assertEqual(book.reconciliations[0].state, 'edit')
 
             Lines.wfcheck(book.lines)
             self.assertEqual(book.lines[0].state, 'check')
             self.assertEqual(book.lines[0].number, None)
             self.assertEqual(book.lines[1].state, 'check')
             self.assertEqual(book.lines[1].number, None)
 
             Reconciliation.wfcheck(book.reconciliations)
             self.assertEqual(len(book.reconciliations[0].lines), 2)
-            self.assertEqual(book.reconciliations[0].lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
-            self.assertEqual(book.reconciliations[0].lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+            self.assertEqual(
+                book.reconciliations[0].lines[0].rec_name,
+                '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+            self.assertEqual(
+                book.reconciliations[0].lines[1].rec_name,
+                '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
             self.assertEqual(book.reconciliations[0].lines[0].number, None)
             self.assertEqual(book.reconciliations[0].lines[1].number, None)
 
             Reconciliation.wfdone(book.reconciliations)
             self.assertEqual(book.reconciliations[0].lines[0].number, '1')
             self.assertEqual(book.reconciliations[0].lines[0].state, 'done')
             self.assertEqual(book.reconciliations[0].lines[1].number, '2')
@@ -715,107 +775,179 @@
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.btype.rec_name, 'CAS - Cash')
         self.assertEqual(book.state, 'open')
         self.assertEqual(len(book.lines), 3)
         self.assertEqual(book.lines[0].date, date(2022, 5, 1))
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].state_cashbook, 'open')
         self.assertEqual(book.lines[1].date, date(2022, 5, 2))
-        self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[2].date, date(2022, 5, 3))
-        self.assertEqual(book.lines[2].rec_name, '05/03/2022|Rev/Sp|1.00 usd|Text 3 [-]')
+        self.assertEqual(
+            book.lines[2].rec_name, '05/03/2022|Rev/Sp|1.00 usd|Text 3 [-]')
 
-        self.assertEqual(Lines.search_count([('rec_name', '=', 'Text 1')]), 1)
-        self.assertEqual(Lines.search_count([('rec_name', '=', 'Text 1a')]), 0)
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', 'text%')]), 3)
+        self.assertEqual(
+            Lines.search_count([('rec_name', '=', 'Text 1')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', '=', 'Text 1a')]), 0)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', 'text%')]), 3)
         # search in category of split-line
-        self.assertEqual(Lines.search_count([('rec_name', '=', 'sp-cat1')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', '=', 'sp-cat1')]), 1)
         # search in description of split-line
-        self.assertEqual(Lines.search_count([('rec_name', '=', 'text3-spline1')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', '=', 'text3-spline1')]), 1)
         # ilike fails in fields.Text to find subtext...
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', '%spline%')]), 0)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', '%spline%')]), 0)
         # ...but it uses separator-chars
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', 'text3%')]), 1)
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', 'spline1')]), 1)
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', '%spline1')]), 1)
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', 'spline1%')]), 0)
-        self.assertEqual(Lines.search_count([('rec_name', 'ilike', 'text3')]), 1)
-
-        self.assertEqual(Lines.search_count([('state_cashbook', '=', 'open')]), 3)
-        self.assertEqual(Lines.search_count([('state_cashbook', '=', 'closed')]), 0)
-        self.assertEqual(Lines.search_count([('cashbook.state', '=', 'open')]), 3)
-        self.assertEqual(Lines.search_count([('cashbook.state', '=', 'closed')]), 0)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', 'text3%')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', 'spline1')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', '%spline1')]), 1)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', 'spline1%')]), 0)
+        self.assertEqual(
+            Lines.search_count([('rec_name', 'ilike', 'text3')]), 1)
+
+        self.assertEqual(
+            Lines.search_count([('state_cashbook', '=', 'open')]), 3)
+        self.assertEqual(
+            Lines.search_count([('state_cashbook', '=', 'closed')]), 0)
+        self.assertEqual(
+            Lines.search_count([('cashbook.state', '=', 'open')]), 3)
+        self.assertEqual(
+            Lines.search_count([('cashbook.state', '=', 'closed')]), 0)
 
         # sorting: date -> state -> id
         self.assertEqual(len(book.lines), 3)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].state, 'edit')
-        self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name, '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].state, 'edit')
-        self.assertEqual(book.lines[2].rec_name, '05/03/2022|Rev/Sp|1.00 usd|Text 3 [-]')
+        self.assertEqual(
+            book.lines[2].rec_name, '05/03/2022|Rev/Sp|1.00 usd|Text 3 [-]')
         self.assertEqual(book.lines[2].state, 'edit')
 
         # set to same date
         Lines.write(*[
             list(book.lines),
             {
                 'date': date(2022, 5, 1),
             }])
         # check again
         book, = Book.search([])
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].state, 'edit')
-        self.assertEqual(book.lines[1].rec_name, '05/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name, '05/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].state, 'edit')
-        self.assertEqual(book.lines[2].rec_name, '05/01/2022|Rev/Sp|1.00 usd|Text 3 [-]')
+        self.assertEqual(
+            book.lines[2].rec_name, '05/01/2022|Rev/Sp|1.00 usd|Text 3 [-]')
         self.assertEqual(book.lines[2].state, 'edit')
 
         # set to 'check', will sort first
         Lines.wfcheck([book.lines[1]])
         book, = Book.search([])
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[0].state, 'check')
-        self.assertEqual(book.lines[1].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[1].state, 'edit')
-        self.assertEqual(book.lines[2].rec_name, '05/01/2022|Rev/Sp|1.00 usd|Text 3 [-]')
+        self.assertEqual(
+            book.lines[2].rec_name, '05/01/2022|Rev/Sp|1.00 usd|Text 3 [-]')
         self.assertEqual(book.lines[2].state, 'edit')
 
     @with_transaction()
     def test_line_to_non_type_book(self):
         """ create cashbook w/o type
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
 
         category = self.prep_category(cattype='in')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': None,
             'company': company.id,
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
 
-        self.assertRaisesRegex(UserError,
-            'The value for field "Cashbook" in "Cashbook Line" is not valid according to its domain.',
+        self.assertRaisesRegex(
+            UserError,
+            r'The value "Book 1" for field "Cashbook" in "\d+" of ' +
+            r'"Cashbook Line" is not valid according to its domain.',
             Line.create,
             [{
                 'cashbook': book.id,
                 'date': date(2022, 5, 1),
                 'category': category.id,
                 'bookingtype': 'in',
                 'amount': Decimal('0.0'),
             }])
 
     @with_transaction()
+    def test_line_check_deny_delete_of_party(self):
+        """ create cashbook + line, delete party should fail
+        """
+        pool = Pool()
+        Book = pool.get('cashbook.book')
+        Party = pool.get('party.party')
+
+        types = self.prep_type()
+        category = self.prep_category(cattype='in')
+        company = self.prep_company()
+        party = self.prep_party()
+        book, = Book.create([{
+            'name': 'Book 1',
+            'btype': types.id,
+            'company': company.id,
+            'currency': company.currency.id,
+            'number_sequ': self.prep_sequence().id,
+            'start_date': date(2022, 5, 1),
+            'lines': [('create', [{
+                    'date': date(2022, 5, 1),
+                    'description': 'Text 1',
+                    'category': category.id,
+                    'bookingtype': 'in',
+                    'amount': Decimal('1.0'),
+                    'party': party.id,
+                }])],
+            }])
+        self.assertEqual(book.name, 'Book 1')
+        self.assertEqual(book.state, 'open')
+        self.assertEqual(len(book.lines), 1)
+        self.assertEqual(book.lines[0].party.rec_name, 'Party')
+        self.assertEqual(book.lines[0].party.id, party.id)
+
+        self.assertEqual(Party.search_count([('name', '=', 'Party')]), 1)
+
+        self.assertRaisesRegex(
+            UserError,
+            'The records could not be deleted because they are used by ' +
+            'field "Party" of "Cashbook Line".',
+            Party.delete,
+            [party])
+
+    @with_transaction()
     def test_line_create_check_deny_write(self):
         """ create cashbook + line, 'close' book, write to line
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
 
@@ -854,29 +986,33 @@
             [book.lines[0]],
             {
                 'description': 'works',
             }])
         Line.wfcheck([book.lines[0]])
         self.assertEqual(book.lines[0].state, 'check')
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook line '05/01/2022|1.00 usd|works [Cat1]' is 'Checked' and cannot be changed.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook line '05/01/2022|1.00 usd|works [Cat1]' is " +
+            "'Checked' and cannot be changed.",
             Line.write,
             *[
                 [book.lines[0]],
                 {
                     'description': 'denied by line.state',
                 },
             ])
 
         Book.wfclosed([book])
         self.assertEqual(book.state, 'closed')
 
-        self.assertRaisesRegex(UserError,
-            "The cash book 'Book | 2.00 usd | Closed' is 'Closed' and cannot be changed.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cash book 'Book | 2.00 usd | Closed' is 'Closed' " +
+            "and cannot be changed.",
             Line.write,
             *[
                 [book.lines[0]],
                 {
                     'description': 'should be denied',
                 },
             ])
@@ -952,21 +1088,20 @@
     @with_transaction()
     def test_line_check_bookingtype_mvout(self):
         """ create cashbook + line, bookingtype 'mvout'
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Category = pool.get('cashbook.category')
 
         types = self.prep_type()
-        category_in = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         category_out = self.prep_category(name='Out Category', cattype='out')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
 
         book2, = Book.create([{
             'name': 'Book 2',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -988,56 +1123,66 @@
                     'amount': Decimal('1.0'),
                     'booktransf': book2.id,
                 }])],
             }])
         self.assertEqual(book.rec_name, 'Book 1 | -1.00 usd | Open')
         self.assertEqual(len(book.lines), 1)
         self.assertEqual(len(book2.lines), 0)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 0.00 usd | Open]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 0.00 usd | Open]')
         self.assertEqual(len(book.lines[0].references), 0)
 
         # check counterpart
-        self.assertEqual(book.lines[0].booktransf.rec_name, 'Book 2 | 0.00 usd | Open')
+        self.assertEqual(
+            book.lines[0].booktransf.rec_name,
+            'Book 2 | 0.00 usd | Open')
         self.assertEqual(book.lines[0].booktransf.btype.feature, 'gen')
         self.assertEqual(book.lines[0].booktransf_feature, 'gen')
 
         # check payee
-        self.assertEqual(book.lines[0].payee.rec_name, 'Book 2 | 0.00 usd | Open')
+        self.assertEqual(
+            book.lines[0].payee.rec_name, 'Book 2 | 0.00 usd | Open')
         self.assertEqual(Line.search_count([('payee', 'ilike', 'book 2%')]), 1)
 
         # set line to 'checked', this creates the counterpart
         Line.wfcheck(list(book.lines))
 
         self.assertEqual(len(book.lines), 1)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 1.00 usd | Open]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 1.00 usd | Open]')
         self.assertEqual(book.lines[0].state, 'check')
         self.assertEqual(len(book.lines[0].references), 1)
         self.assertEqual(book.lines[0].reference, None)
         self.assertEqual(book.lines[0].references[0].id, book2.lines[0].id)
 
         self.assertEqual(len(book2.lines), 1)
-        self.assertEqual(book2.lines[0].rec_name, '05/01/2022|from|1.00 usd|Transfer Out [Book 1 | -1.00 usd | Open]')
+        self.assertEqual(
+            book2.lines[0].rec_name,
+            '05/01/2022|from|1.00 usd|Transfer Out [Book 1 | -1.00 usd | Open]')
         self.assertEqual(book2.lines[0].state, 'check')
-        self.assertEqual(book2.lines[0].reference.rec_name, '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 1.00 usd | Open]')
+        self.assertEqual(
+            book2.lines[0].reference.rec_name,
+            '05/01/2022|to|-1.00 usd|Transfer Out [Book 2 | 1.00 usd | Open]')
         self.assertEqual(len(book2.lines[0].references), 0)
 
     @with_transaction()
     def test_line_check_bookingtype_mvin(self):
         """ create cashbook + line, bookingtype 'mvin'
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Category = pool.get('cashbook.category')
 
         types = self.prep_type()
         category_in = self.prep_category(cattype='in')
-        category_out = self.prep_category(name='Out Category', cattype='out')
+        self.prep_category(name='Out Category', cattype='out')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
 
         book2, = Book.create([{
             'name': 'Book 2',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -1059,51 +1204,60 @@
                     'amount': Decimal('1.0'),
                     'booktransf': book2.id,
                 }])],
             }])
         self.assertEqual(book.rec_name, 'Book 1 | 1.00 usd | Open')
         self.assertEqual(len(book.lines), 1)
         self.assertEqual(len(book2.lines), 0)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|from|1.00 usd|Transfer In [Book 2 | 0.00 usd | Open]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|from|1.00 usd|Transfer In [Book 2 | 0.00 usd | Open]')
         self.assertEqual(len(book.lines[0].references), 0)
 
         # set line to 'checked', this creates the counterpart
         Line.wfcheck(list(book.lines))
 
         self.assertEqual(len(book.lines), 1)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd | Open]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd | Open]')
         self.assertEqual(book.lines[0].state, 'check')
         self.assertEqual(len(book.lines[0].references), 1)
         self.assertEqual(book.lines[0].reference, None)
         self.assertEqual(book.lines[0].references[0].id, book2.lines[0].id)
 
         self.assertEqual(len(book2.lines), 1)
-        self.assertEqual(book2.lines[0].rec_name, '05/01/2022|to|-1.00 usd|Transfer In [Book 1 | 1.00 usd | Open]')
+        self.assertEqual(
+            book2.lines[0].rec_name,
+            '05/01/2022|to|-1.00 usd|Transfer In [Book 1 | 1.00 usd | Open]')
         self.assertEqual(book2.lines[0].state, 'check')
-        self.assertEqual(book2.lines[0].reference.rec_name, '05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd | Open]')
+        self.assertEqual(
+            book2.lines[0].reference.rec_name,
+            '05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd | Open]')
         self.assertEqual(len(book2.lines[0].references), 0)
 
         # tryt wfedit to 'book2.lines[0]'
-        self.assertRaisesRegex(UserError,
-            "The current line is managed by the cashbook line '05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd | Open]', cashbook: 'Book 1 | 1.00 usd | Open'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The current line is managed by the cashbook line " +
+            "'05/01/2022|from|1.00 usd|Transfer In [Book 2 | -1.00 usd " +
+            "| Open]', cashbook: 'Book 1 | 1.00 usd | Open'.",
             Line.wfedit,
             [book2.lines[0]])
 
         Line.wfedit([book.lines[0]])
         self.assertEqual(len(book2.lines), 0)
 
     @with_transaction()
     def test_line_create_check_debit_credit(self):
         """ create cashbook + line, check calculation of debit/credit
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
-        Category = pool.get('cashbook.category')
 
         types = self.prep_type()
         category_in = self.prep_category(cattype='in')
         category_out = self.prep_category(name='Out Category', cattype='out')
         company = self.prep_company()
         party = self.prep_party()
 
@@ -1242,26 +1396,24 @@
 
     @with_transaction()
     def test_line_create_check_category_view(self):
         """ create cashbook + line, check 'category_view'
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
-        Line = pool.get('cashbook.line')
         Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
 
             category2, = Category.create([{
                 'company': company.id,
                 'name': 'Level1',
                 'cattype': 'in',
                 'childs': [('create', [{
                     'company': company.id,
@@ -1395,16 +1547,19 @@
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(len(book.lines), 2)
         self.assertEqual(book.state, 'open')
         Book.wfclosed([book])
         self.assertEqual(book.state, 'closed')
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook line '05/01/2022 Text 1' cannot be deleted because the Cashbook 'Book | 2.00 usd | Closed' is in state 'Closed'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook line '05/01/2022 Text 1' cannot be deleted " +
+            "because the Cashbook 'Book | 2.00 usd | Closed' is" +
+            " in state 'Closed'.",
             Lines.delete,
             [book.lines[0]])
 
     @with_transaction()
     def test_line_delete_with_line_in_check_state(self):
         """ create cashbook + line, line in state=check, delete a line
         """
@@ -1443,16 +1598,18 @@
         self.assertEqual(len(book.lines), 2)
         self.assertEqual(book.state, 'open')
 
         self.assertEqual(book.lines[0].state, 'edit')
         Lines.wfcheck([book.lines[0]])
         self.assertEqual(book.lines[0].state, 'check')
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook line '05/01/2022|1.00 usd|Test 1 [Cat1]' cannot be deleted, its in state 'Checked'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook line '05/01/2022|1.00 usd|Test 1 [Cat1]' " +
+            "cannot be deleted, its in state 'Checked'.",
             Lines.delete,
             [book.lines[0]])
 
     @with_transaction()
     def test_line_permission_owner(self):
         """ create book+line + 2x users, add users to group, check access
         """
@@ -1501,39 +1658,46 @@
                 'party': party.id,
                 }])],
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 1.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 0)
 
             # change to user 'frida' read/write book
             with Transaction().set_user(usr_lst[0].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 1)
-                self.assertEqual(lines[0].cashbook.rec_name, 'Fridas book | 1.00 usd | Open')
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
+                self.assertEqual(
+                    lines[0].cashbook.rec_name,
+                    'Fridas book | 1.00 usd | Open')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
 
                 Line.write(*[
                     lines,
                     {
                         'description': 'Test 2',
                     }])
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
-                self.assertEqual(lines[0].owner_cashbook.rec_name, 'Frida')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
+                self.assertEqual(
+                    lines[0].owner_cashbook.rec_name, 'Frida')
 
     @with_transaction()
     def test_line_permission_reviewer(self):
-        """ create book+line + 2x users + 1x reviewer-group, add users to group, check access
+        """ create book+line + 2x users + 1x reviewer-group,
+            add users to group, check access
         """
         pool = Pool()
         ResUser = pool.get('res.user')
         ResGroup = pool.get('res.group')
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
 
@@ -1583,45 +1747,55 @@
                 'party': party.id,
                 }])],
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 1.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 1)
                 self.assertEqual(len(lines[0].cashbook.reviewer.users), 1)
-                self.assertEqual(lines[0].cashbook.reviewer.users[0].rec_name, 'Diego')
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
+                self.assertEqual(
+                    lines[0].cashbook.reviewer.users[0].rec_name,
+                    'Diego')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
                 Line.write(*[
                     lines,
                     {
                         'description': 'Test 2',
                     }])
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
 
             # change to user 'frida' read/write line
             with Transaction().set_user(usr_lst[0].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 1)
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
                 Line.write(*[
                     lines,
                     {
                         'description': 'Test 3',
                     }])
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 3 [Cat1]')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 3 [Cat1]')
 
     @with_transaction()
     def test_line_permission_observer(self):
-        """ create book+line + 2x users + 1x observer-group, add users to group, check access
+        """ create book+line + 2x users + 1x observer-group,
+            add users to group, check access
         """
         pool = Pool()
         ResUser = pool.get('res.user')
         ResGroup = pool.get('res.group')
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
 
@@ -1671,40 +1845,51 @@
                 'party': party.id,
                 }])],
             }])
         self.assertEqual(book.rec_name, 'Fridas book | 1.00 usd | Open'),
         self.assertEqual(book.owner.rec_name, 'Frida'),
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             # change to user 'diego' , try access
             with Transaction().set_user(usr_lst[1].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 1)
                 self.assertEqual(len(lines[0].cashbook.observer.users), 1)
-                self.assertEqual(lines[0].cashbook.observer.users[0].rec_name, 'Diego')
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
-
-                self.assertRaisesRegex(UserError,
-                    'You are not allowed to write to records "[0-9]{1,}" of "Cashbook Line" because of at least one of these rules:\nOwners and reviewers: Cashbook line write - ',
+                self.assertEqual(
+                    lines[0].cashbook.observer.users[0].rec_name,
+                    'Diego')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
+
+                self.assertRaisesRegex(
+                    UserError,
+                    'You are not allowed to write to records ' +
+                    '"[0-9]{1,}" of "Cashbook Line" because of at least ' +
+                    'one of these rules:\nOwners and reviewers: ' +
+                    'Cashbook line write - ',
                     Line.write,
                     *[
                         lines,
                         {
                             'description': 'Test 2',
                         },
                     ])
 
             # change to user 'frida' read/write line
             with Transaction().set_user(usr_lst[0].id):
                 lines = Line.search([])
                 self.assertEqual(len(lines), 1)
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 1 [Cat1]')
                 Line.write(*[
                     lines,
                     {
                         'description': 'Test 2',
                     }])
-                self.assertEqual(lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
+                self.assertEqual(
+                    lines[0].rec_name,
+                    '05/01/2022|Rev|1.00 usd|Test 2 [Cat1]')
 
 # end LineTestCase
```

### Comparing `mds_cashbook-6.0.27/tests/test_reconciliation.py` & `mds_cashbook-6.8.29/tests/reconciliation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
-from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 from datetime import date
 from decimal import Decimal
 
 
-class ReconTestCase(ModuleTestCase):
-    'Test cashbook reconciliation module'
-    module = 'cashbook'
-
+class ReconTestCase(object):
+    """ test reconciliation
+    """
     @with_transaction()
     def test_recon_check_overlap_start(self):
         """ create, check deny of overlap date - date_from
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -37,26 +35,29 @@
                 'date': date(2022, 5, 1),
                 'date_from': date(2022, 5, 1),
                 'date_to': date(2022, 5, 31),
                 }])],
             }])
 
         Book.write(*[
-            [book],
-            {
-            'reconciliations': [('create', [{
+            [book], {'reconciliations': [('create', [{
                 'date': date(2022, 6, 1),
                 'date_from': date(2022, 6, 1),
                 'date_to': date(2022, 6, 30),
                 }])],
             }])
-        self.assertEqual(book.reconciliations[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-        self.assertEqual(book.reconciliations[1].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[1].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
-        self.assertRaisesRegex(UserError,
+        self.assertRaisesRegex(
+            UserError,
             'The date range overlaps with another reconciliation.',
             Reconciliation.write,
             *[
                 [book.reconciliations[0]],
                 {
                     'date_from': date(2022, 4, 15),
                     'date_to': date(2022, 5, 2),
@@ -68,15 +69,15 @@
         """ create, check deny of overlap date - date_to
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -85,26 +86,29 @@
                 'date': date(2022, 5, 1),
                 'date_from': date(2022, 5, 1),
                 'date_to': date(2022, 5, 31),
                 }])],
             }])
 
         Book.write(*[
-            [book],
-            {
-            'reconciliations': [('create', [{
+            [book], {'reconciliations': [('create', [{
                 'date': date(2022, 6, 1),
                 'date_from': date(2022, 6, 1),
                 'date_to': date(2022, 6, 30),
                 }])],
             }])
-        self.assertEqual(book.reconciliations[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-        self.assertEqual(book.reconciliations[1].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[1].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
-        self.assertRaisesRegex(UserError,
+        self.assertRaisesRegex(
+            UserError,
             'The date range overlaps with another reconciliation.',
             Reconciliation.write,
             *[
                 [book.reconciliations[0]],
                 {
                     'date_from': date(2022, 5, 30),
                 },
@@ -115,15 +119,15 @@
         """ create, check deny of overlap date - inside of period
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -132,26 +136,29 @@
                 'date': date(2022, 5, 1),
                 'date_from': date(2022, 5, 1),
                 'date_to': date(2022, 5, 31),
                 }])],
             }])
 
         Book.write(*[
-            [book],
-            {
-            'reconciliations': [('create', [{
+            [book], {'reconciliations': [('create', [{
                 'date': date(2022, 6, 1),
                 'date_from': date(2022, 6, 1),
                 'date_to': date(2022, 6, 30),
                 }])],
             }])
-        self.assertEqual(book.reconciliations[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-        self.assertEqual(book.reconciliations[1].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[1].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
-        self.assertRaisesRegex(UserError,
+        self.assertRaisesRegex(
+            UserError,
             'The date range overlaps with another reconciliation.',
             Reconciliation.write,
             *[
                 [book.reconciliations[0]],
                 {
                     'date_from': date(2022, 5, 5),
                     'date_to': date(2022, 5, 15),
@@ -163,15 +170,15 @@
         """ create, check deny of overlap date - enclose a period
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
@@ -180,26 +187,29 @@
                 'date': date(2022, 5, 1),
                 'date_from': date(2022, 5, 1),
                 'date_to': date(2022, 5, 31),
                 }])],
             }])
 
         Book.write(*[
-            [book],
-            {
-            'reconciliations': [('create', [{
+            [book], {'reconciliations': [('create', [{
                 'date': date(2022, 6, 1),
                 'date_from': date(2022, 6, 1),
                 'date_to': date(2022, 6, 30),
                 }])],
             }])
-        self.assertEqual(book.reconciliations[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-        self.assertEqual(book.reconciliations[1].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[1].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
-        self.assertRaisesRegex(UserError,
+        self.assertRaisesRegex(
+            UserError,
             'The date range overlaps with another reconciliation.',
             Reconciliation.write,
             *[
                 [book.reconciliations[1]],
                 {
                     'date_from': date(2022, 4, 25),
                     'date_to': date(2022, 6, 10),
@@ -226,19 +236,23 @@
             'reconciliations': [('create', [{
                     'date': date(2022, 5, 28),
                     'date_from': date(2022, 5, 1),
                     'date_to':  date(2022, 5, 31),
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
         self.assertEqual(book.reconciliations[0].feature, 'gen')
 
         Reconciliation.wfcheck(list(book.reconciliations))
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
     @with_transaction()
     def test_recon_set_start_amount_by_predecessor(self):
         """ set stat-amount from end_amount of predecessor
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -275,33 +289,41 @@
                     'description': 'Line 2',
                     'party': party.id,
                     'amount': Decimal('7.0'),
                 },])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(len(book.reconciliations), 1)
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
         self.assertEqual(len(book.reconciliations[0].lines), 0)
 
         Lines.wfcheck(list(book.lines))
         Reconciliation.wfcheck(list(book.reconciliations))
 
         self.assertEqual(book.reconciliations[0].state, 'check')
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 12.00 usd [2]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 12.00 usd [2]')
         Reconciliation.wfdone(list(book.reconciliations))
         self.assertEqual(book.reconciliations[0].state, 'done')
 
         recons = Reconciliation.create([{
             'cashbook': book.id,
             'date_from': date(2022, 5, 31),
             'date_to': date(2022, 6, 30),
             }])
-        self.assertEqual(recons[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            recons[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
         Reconciliation.wfcheck(recons)
-        self.assertEqual(recons[0].rec_name, '05/31/2022 - 06/30/2022 | 12.00 usd - 12.00 usd [0]')
+        self.assertEqual(
+            recons[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 12.00 usd - 12.00 usd [0]')
 
     @with_transaction()
     def test_recon_predecessor_done(self):
         """ predecessor must be done
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -321,30 +343,38 @@
                     'date_from': date(2022, 5, 1),
                     'date_to':  date(2022, 5, 31),
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         Reconciliation.wfcheck(list(book.reconciliations))
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
         self.assertEqual(book.reconciliations[0].state, 'check')
 
         recons = Reconciliation.create([{
             'cashbook': book.id,
             'date_from': date(2022, 5, 31),
             'date_to': date(2022, 6, 30),
             }])
-        self.assertRaisesRegex(UserError,
-            "The predecessor '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]' must be in the 'Done' state before you can check the current reconciliation '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The predecessor " +
+            "'05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]' " +
+            "must be in the 'Done' state before you can check the " +
+            "current reconciliation " +
+            "'05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]'.",
             Reconciliation.wfcheck,
             recons)
 
     @with_transaction()
     def test_recon_autoset_date_to(self):
-        """ create reconciliation, check: set date_to to last date of checked-line
+        """ create reconciliation, check:
+            set date_to to last date of checked-line
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
         Reconciliation = pool.get('cashbook.recon')
 
         types = self.prep_type()
@@ -379,18 +409,22 @@
         recon, = Reconciliation.create([{
                 'cashbook': book.id,
                 'date': date(2022, 5, 28),
                 'date_from': date(2022, 5, 5),
                 'date_to':  date(2022, 5, 31),
             }])
         # dates are updates by .create()
-        self.assertEqual(recon.rec_name, '05/01/2022 - 05/18/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            recon.rec_name,
+            '05/01/2022 - 05/18/2022 | 0.00 usd - 0.00 usd [0]')
 
         Reconciliation.wfcheck([recon])
-        self.assertEqual(recon.rec_name, '05/01/2022 - 05/18/2022 | 0.00 usd - 15.00 usd [2]')
+        self.assertEqual(
+            recon.rec_name,
+            '05/01/2022 - 05/18/2022 | 0.00 usd - 15.00 usd [2]')
 
     @with_transaction()
     def test_recon_autoset_date_from(self):
         """ create reconciliation, check: set date_from to end of predecessor
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -413,34 +447,42 @@
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         Reconciliation.wfcheck([book.reconciliations[0]])
         Reconciliation.wfdone([book.reconciliations[0]])
 
         # date_from is corrected by .create() to start_date of book
-        self.assertEqual(book.reconciliations[0].rec_name,
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
             '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
 
         r2, = Reconciliation.create([{
             'cashbook': book.id,
             'date_from': date(2022, 6, 10),
             'date_to': date(2022, 6, 30),
             }])
-        self.assertEqual(r2.rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            r2.rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
 
         # update 'date_from' to wrong value
         Reconciliation.write(*[
             [r2],
             {
                 'date_from': date(2022, 6, 1),
             }])
-        self.assertEqual(r2.rec_name, '06/01/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-
-        self.assertRaisesRegex(UserError,
-            "The start date '06/01/2022' of the current reconciliation '06/01/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]' must correspond to the end date '05/31/2022' of the predecessor.",
+        self.assertEqual(
+            r2.rec_name,
+            '06/01/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+
+        self.assertRaisesRegex(
+            UserError,
+            "The start date '06/01/2022' of the current reconciliation" +
+            " '06/01/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]' " +
+            "must correspond to the end date '05/31/2022' of the predecessor.",
             Reconciliation.wfcheck,
             [r2])
 
     @with_transaction()
     def test_recon_create_check_line_add_to_recon(self):
         """ create, booklines, add reconciliation
         """
@@ -480,22 +522,31 @@
                     'date_from': date(2022, 5, 1),
                     'date_to':  date(2022, 5, 31),
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         self.assertEqual(len(book.lines), 2)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
-        self.assertEqual(book.lines[1].rec_name, '05/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '05/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(len(book.reconciliations), 1)
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
         self.assertEqual(len(book.reconciliations[0].lines), 0)
 
-        self.assertRaisesRegex(UserError,
-            "For reconciliation, the line '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]' must be in the status 'Check' or 'Done'.",
+        self.assertRaisesRegex(
+            UserError,
+            "For reconciliation, the line " +
+            "'05/01/2022|Rev|1.00 usd|Text 1 [Cat1]' must be in the " +
+            "status 'Check' or 'Done'.",
             Lines.write,
             *[
                 [book.lines[0]],
                 {
                     'reconciliation': book.reconciliations[0].id,
                 }
             ])
@@ -504,16 +555,19 @@
         Lines.write(*[
             list(book.lines),
             {
                 'reconciliation': book.reconciliations[0].id,
             }])
         self.assertEqual(len(book.reconciliations[0].lines), 2)
 
-        self.assertRaisesRegex(UserError,
-            "The status cannot be changed to 'Edit' as long as the line '05/01/2022|1.00 usd|Text 1 [Cat1]' is associated with a reconciliation.",
+        self.assertRaisesRegex(
+            UserError,
+            "The status cannot be changed to 'Edit' as long as the line " +
+            "'05/01/2022|1.00 usd|Text 1 [Cat1]' is associated " +
+            "with a reconciliation.",
             Lines.wfedit,
             [book.lines[0]])
 
         # unlink lines from reconciliation
         self.assertEqual(book.reconciliations[0].state, 'edit')
         self.assertEqual(len(book.reconciliations[0].lines), 2)
         Reconciliation.wfcheck(list(book.reconciliations))
@@ -529,64 +583,78 @@
             {
                 'date': date(2022, 6, 1),
             }])
         # check reconciliation, this linkes the 1st line by date
         Reconciliation.wfcheck(list(book.reconciliations))
         self.assertEqual(book.reconciliations[0].state, 'check')
         self.assertEqual(len(book.reconciliations[0].lines), 1)
-        self.assertEqual(book.reconciliations[0].lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.reconciliations[0].lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].state, 'check')
-        self.assertEqual(book.lines[1].rec_name, '06/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '06/01/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[1].state, 'edit')
 
         # move 1st line into date-range of checked-reconciliation, wf-check
         Lines.write(*[
             [book.lines[1]],
             {
                 'date': date(2022, 5, 20),
             }])
-        self.assertRaisesRegex(UserError,
-            "For the date '05/20/2022' there is already a completed reconciliation. Use a different date.",
+        self.assertRaisesRegex(
+            UserError,
+            "For the date '05/20/2022' there is already a completed " +
+            "reconciliation. Use a different date.",
             Lines.wfcheck,
             [book.lines[1]])
 
         # set date to end of date-range of reconciliation
         # should work
         Lines.write(*[
             [book.lines[1]],
             {
                 'date': date(2022, 5, 31),
             }])
-        Lines.wfcheck([book.lines[1]]) # ok
+        Lines.wfcheck([book.lines[1]])  # ok
         Lines.wfedit([book.lines[1]])
         Lines.write(*[
             [book.lines[1]],
             {
                 'date': date(2022, 7, 1),
             }])
 
         # add 2nd reconciliation
         recon2, = Reconciliation.create([{
             'cashbook': book.id,
             'date_from': date(2022, 5, 31),
             'date_to': date(2022, 6, 30),
             }])
-        self.assertEqual(book.reconciliations[0].rec_name, '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
-        self.assertEqual(book.reconciliations[1].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 1.00 usd [1]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/31/2022 - 06/30/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[1].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 1.00 usd [1]')
         Reconciliation.wfdone([book.reconciliations[1]])
         Reconciliation.wfcheck([recon2])
 
         Lines.write(*[
             [book.lines[1]],
             {
                 'date': date(2022, 5, 31),
             }])
-        self.assertRaisesRegex(UserError,
-            "For the date '05/31/2022' there is already a completed reconciliation. Use a different date.",
+        self.assertRaisesRegex(
+            UserError,
+            "For the date '05/31/2022' there is already a completed " +
+            "reconciliation. Use a different date.",
             Lines.wfcheck,
             [book.lines[1]])
 
     @with_transaction()
     def test_recon_check_wfcheck_missing_lines(self):
         """ create, booklines, check missing line at wfcheck
         """
@@ -626,30 +694,39 @@
                     'date_from': date(2022, 5, 1),
                     'date_to':  date(2022, 5, 31),
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         self.assertEqual(len(book.lines), 2)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
-        self.assertEqual(book.lines[1].rec_name, '06/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '06/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
 
         Lines.wfcheck([book.lines[0]])
         Reconciliation.wfcheck([book.reconciliations[0]])
         self.assertEqual(len(book.reconciliations[0].lines), 1)
-        self.assertEqual(book.reconciliations[0].lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.reconciliations[0].lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
 
         Lines.write(*[
             [book.lines[1]],
             {
                 'date': date(2022, 5, 15),
             }])
 
-        self.assertRaisesRegex(UserError,
-            "In the date range from 05/01/2022 to 05/31/2022, there are still cashbook lines that do not belong to any reconciliation.",
+        self.assertRaisesRegex(
+            UserError,
+            "In the date range from 05/01/2022 to 05/31/2022, " +
+            "there are still cashbook lines that do not belong " +
+            "to any reconciliation.",
             Reconciliation.wfdone,
             [book.reconciliations[0]])
 
     @with_transaction()
     def test_recon_check_deny_delete(self):
         """ create, booklines, reconciliation, try delete
         """
@@ -687,28 +764,35 @@
         self.assertEqual(book.state, 'open')
 
         Lines.wfcheck(list(book.lines))
         Reconciliation.wfcheck(list(book.reconciliations))
         self.assertEqual(len(book.reconciliations), 1)
         self.assertEqual(len(book.reconciliations[0].lines), 1)
 
-        self.assertRaisesRegex(UserError,
-            "The reconciliation '05/01/2022 - 05/31/2022 | 0.00 - 0.00 usd [0]' cannot be deleted, its in state 'Check'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The reconciliation '05/01/2022 - 05/31/2022 " +
+            "| 0.00 - 0.00 usd [0]' cannot be deleted, its in state 'Check'.",
             Reconciliation.delete,
             list(book.reconciliations))
 
         Book.wfclosed([book])
 
-        self.assertRaisesRegex(UserError,
-            "The cashbook line '05/01/2022 - 05/31/2022: 0.00 usd' cannot be deleted because the Cashbook 'Book 1 | 1.00 usd | Closed' is in state 'Closed'.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cashbook line '05/01/2022 - 05/31/2022: 0.00 usd' " +
+            "cannot be deleted because the Cashbook " +
+            "'Book 1 | 1.00 usd | Closed' is in state 'Closed'.",
             Reconciliation.delete,
             list(book.reconciliations))
 
-        self.assertRaisesRegex(UserError,
-            "The cash book 'Book 1 | 1.00 usd | Closed' is 'Closed' and cannot be changed.",
+        self.assertRaisesRegex(
+            UserError,
+            "The cash book 'Book 1 | 1.00 usd | Closed' is 'Closed' " +
+            "and cannot be changed.",
             Reconciliation.write,
             *[
                 list(book.reconciliations),
                 {
                     'date': date(2022, 5, 29),
                 },
             ])
@@ -753,35 +837,49 @@
                     'date_from': date(2022, 5, 1),
                     'date_to':  date(2022, 5, 31),
                 }])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(book.state, 'open')
         self.assertEqual(len(book.lines), 2)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
-        self.assertEqual(book.lines[1].rec_name, '05/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[1].rec_name,
+            '05/05/2022|Rev|1.00 usd|Text 2 [Cat1]')
         self.assertEqual(book.lines[0].reconciliation, None)
         self.assertEqual(book.lines[1].reconciliation, None)
         self.assertEqual(len(book.reconciliations), 1)
-        self.assertEqual(book.reconciliations[0].rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
+        self.assertEqual(
+            book.reconciliations[0].rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]')
         self.assertEqual(len(book.reconciliations[0].lines), 0)
 
         # run wf, fail with lines not 'checked'
-        self.assertRaisesRegex(UserError,
-            "For the reconciliation '05/01/2022 - 05/31/2022 | 0.00 usd - 0.00 usd [0]' of the cashbook 'Book 1 | 2.00 usd | Open', all lines in the date range from '05/01/2022' to '05/31/2022' must be in the 'Check' state.",
+        self.assertRaisesRegex(
+            UserError,
+            "For the reconciliation '05/01/2022 - 05/31/2022 | " +
+            "0.00 usd - 0.00 usd [0]' of the cashbook " +
+            "'Book 1 | 2.00 usd | Open', all lines in the date range " +
+            "from '05/01/2022' to '05/31/2022' must be in the 'Check' state.",
             Reconciliation.wfcheck,
             list(book.reconciliations),
             )
 
         # edit --> check
         Lines.wfcheck(book.lines)
         Reconciliation.wfcheck(list(book.reconciliations))
         self.assertEqual(len(book.reconciliations[0].lines), 2)
-        self.assertEqual(book.lines[0].reconciliation.rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 2.00 usd [2]')
-        self.assertEqual(book.lines[1].reconciliation.rec_name, '05/01/2022 - 05/31/2022 | 0.00 usd - 2.00 usd [2]')
+        self.assertEqual(
+            book.lines[0].reconciliation.rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 2.00 usd [2]')
+        self.assertEqual(
+            book.lines[1].reconciliation.rec_name,
+            '05/01/2022 - 05/31/2022 | 0.00 usd - 2.00 usd [2]')
 
         # check --> edit
         Reconciliation.wfedit(list(book.reconciliations))
         self.assertEqual(len(book.reconciliations[0].lines), 0)
         self.assertEqual(book.lines[0].reconciliation, None)
         self.assertEqual(book.lines[1].reconciliation, None)
```

### Comparing `mds_cashbook-6.0.27/tests/test_splitline.py` & `mds_cashbook-6.8.29/tests/splitline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
-from trytond.transaction import Transaction
-from trytond.exceptions import UserError
 from datetime import date
-from unittest.mock import MagicMock
 from decimal import Decimal
 
 
-class SplitLineTestCase(ModuleTestCase):
-    'Test split line module'
-    module = 'cashbook'
+class SplitLineTestCase(object):
+    """ test split lines
+    """
 
     @with_transaction()
     def test_splitline_in_category(self):
         """ add book, check splitbooking - incoming
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
-        Line = pool.get('cashbook.line')
 
         types = self.prep_type()
         category1 = self.prep_category(cattype='in')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
         book, = Book.create([{
             'name': 'Book 1',
             'btype': types.id,
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
             'start_date': date(2022, 5, 1),
@@ -55,26 +51,30 @@
                         'splittype': 'cat',
                         'description': 'from cashbook',
                         'category': category1.id,
                         }])],
                     }])],
             }])
         self.assertEqual(len(book.lines), 1)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev/Sp|11.00 usd|- [-]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev/Sp|11.00 usd|- [-]')
         self.assertEqual(book.lines[0].category, None)
         self.assertEqual(len(book.lines[0].splitlines), 2)
 
         self.assertEqual(book.lines[0].splitlines[0].feature, 'gen')
         self.assertEqual(book.lines[0].splitlines[0].booktransf_feature, None)
         self.assertEqual(book.lines[0].splitlines[1].feature, 'gen')
         self.assertEqual(book.lines[0].splitlines[1].booktransf_feature, None)
 
-        self.assertEqual(book.lines[0].splitlines[0].rec_name,
+        self.assertEqual(
+            book.lines[0].splitlines[0].rec_name,
             'Rev/Sp|5.00 usd|from category [Cat1]')
-        self.assertEqual(book.lines[0].splitlines[1].rec_name,
+        self.assertEqual(
+            book.lines[0].splitlines[1].rec_name,
             'Rev/Sp|6.00 usd|from cashbook [Cat1]')
 
     @with_transaction()
     def test_splitline_category_and_transfer(self):
         """ add book, line, two split-lines,
             category + transfer
         """
@@ -107,15 +107,17 @@
             'company': company.id,
             'currency': company.currency.id,
             'number_sequ': self.prep_sequence().id,
             'start_date': date(2022, 5, 1),
             }])
         self.assertEqual(books[0].rec_name, 'Book 1 | 1.00 usd | Open')
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(books[1].rec_name, 'Book 2 | 0.00 usd | Open')
 
         Book.write(*[
             [books[0]],
             {
                 'lines': [('write', [books[0].lines[0]], {
                     'bookingtype': 'spin',
@@ -129,42 +131,51 @@
                         'splittype': 'tr',
                         'description': 'from cashbook',
                         'booktransf': books[1].id,
                         }])],
                     })]
             }])
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name, '05/01/2022|Rev/Sp|11.00 usd|Text 1 [-]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/01/2022|Rev/Sp|11.00 usd|Text 1 [-]')
         self.assertEqual(books[0].lines[0].category, None)
         self.assertEqual(len(books[0].lines[0].splitlines), 2)
-        self.assertEqual(books[0].lines[0].splitlines[0].rec_name,
+        self.assertEqual(
+            books[0].lines[0].splitlines[0].rec_name,
             'Rev/Sp|5.00 usd|from category [Cat1]')
-        self.assertEqual(books[0].lines[0].splitlines[1].rec_name,
+        self.assertEqual(
+            books[0].lines[0].splitlines[1].rec_name,
             'Rev/Sp|6.00 usd|from cashbook [Book 2 | 0.00 usd | Open]')
         self.assertEqual(len(books[1].lines), 0)
         self.assertEqual(books[0].lines[0].splitlines[0].feature, 'gen')
 
         self.assertEqual(books[0].lines[0].splitlines[0].feature, 'gen')
-        self.assertEqual(books[0].lines[0].splitlines[0].booktransf_feature, None)
+        self.assertEqual(
+            books[0].lines[0].splitlines[0].booktransf_feature, None)
         self.assertEqual(books[0].lines[0].splitlines[1].feature, 'gen')
-        self.assertEqual(books[0].lines[0].splitlines[1].booktransf_feature, 'gen')
+        self.assertEqual(
+            books[0].lines[0].splitlines[1].booktransf_feature, 'gen')
 
         # wf: edit -> check
         Line.wfcheck(books[0].lines)
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(books[0].lines[0].state, 'check')
         self.assertEqual(books[0].lines[0].number, '1')
         self.assertEqual(len(books[0].lines[0].references), 1)
-        self.assertEqual(books[0].lines[0].references[0].rec_name,
+        self.assertEqual(
+            books[0].lines[0].references[0].rec_name,
             '05/01/2022|to|-6.00 usd|from cashbook [Book 1 | 11.00 usd | Open]')
 
         self.assertEqual(len(books[1].lines), 1)
-        self.assertEqual(books[1].lines[0].reference.rec_name,
+        self.assertEqual(
+            books[1].lines[0].reference.rec_name,
             '05/01/2022|Rev/Sp|11.00 usd|Text 1 [-]')
-        self.assertEqual(books[1].lines[0].rec_name,
+        self.assertEqual(
+            books[1].lines[0].rec_name,
             '05/01/2022|to|-6.00 usd|from cashbook [Book 1 | 11.00 usd | Open]')
 
         # wf: check --> edit
         Line.wfedit(books[0].lines)
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[0].lines[0].references), 0)
         self.assertEqual(len(books[1].lines), 0)
@@ -205,15 +216,17 @@
             'company': company.id,
             'currency': usd.id,
             'number_sequ': self.prep_sequence().id,
             'start_date': date(2022, 5, 1),
             }])
         self.assertEqual(books[0].rec_name, 'Book 1 | -1.00 € | Open')
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name, '05/01/2022|Exp|-1.00 €|Text 1 [Cat1]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/01/2022|Exp|-1.00 €|Text 1 [Cat1]')
         self.assertEqual(books[1].rec_name, 'Book 2 | 0.00 usd | Open')
 
         # EUR --> USD
         Book.write(*[
             [books[0]],
             {
                 'lines': [('write', [books[0].lines[0]], {
@@ -228,41 +241,53 @@
                         'splittype': 'tr',
                         'description': 'to book2',
                         'booktransf': books[1].id,
                         }])],
                     })]
             }])
         self.assertEqual(len(books[0].lines), 1)
-        self.assertEqual(books[0].lines[0].rec_name, '05/01/2022|Exp/Sp|-11.00 €|Text 1 [-]')
+        self.assertEqual(
+            books[0].lines[0].rec_name,
+            '05/01/2022|Exp/Sp|-11.00 €|Text 1 [-]')
         self.assertEqual(books[0].lines[0].category, None)
         self.assertEqual(len(books[0].lines[0].splitlines), 2)
-        self.assertEqual(books[0].lines[0].splitlines[0].rec_name,
+        self.assertEqual(
+            books[0].lines[0].splitlines[0].rec_name,
             'Exp/Sp|5.00 €|to category [Cat1]')
-        self.assertEqual(books[0].lines[0].splitlines[0].amount_2nd_currency, None)
-        self.assertEqual(books[0].lines[0].splitlines[1].rec_name,
+        self.assertEqual(
+            books[0].lines[0].splitlines[0].amount_2nd_currency, None)
+        self.assertEqual(
+            books[0].lines[0].splitlines[1].rec_name,
             'Exp/Sp|6.00 €|to book2 [Book 2 | 0.00 usd | Open]')
-        self.assertEqual(books[0].lines[0].splitlines[1].amount_2nd_currency, Decimal('6.3'))
+        self.assertEqual(
+            books[0].lines[0].splitlines[1].amount_2nd_currency,
+            Decimal('6.3'))
         self.assertEqual(len(books[1].lines), 0)
 
         # wf: edit -> check
         Line.wfcheck(books[0].lines)
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(books[0].lines[0].state, 'check')
         self.assertEqual(books[0].lines[0].number, '1')
         self.assertEqual(len(books[0].lines[0].references), 1)
-        self.assertEqual(books[0].lines[0].references[0].rec_name,
+        self.assertEqual(
+            books[0].lines[0].references[0].rec_name,
             '05/01/2022|from|6.30 usd|to book2 [Book 1 | -11.00 € | Open]')
 
         self.assertEqual(len(books[1].lines), 1)
-        self.assertEqual(books[1].lines[0].reference.rec_name,
+        self.assertEqual(
+            books[1].lines[0].reference.rec_name,
             '05/01/2022|Exp/Sp|-11.00 €|Text 1 [-]')
-        self.assertEqual(books[1].lines[0].rec_name,
+        self.assertEqual(
+            books[1].lines[0].rec_name,
             '05/01/2022|from|6.30 usd|to book2 [Book 1 | -11.00 € | Open]')
-        self.assertEqual(books[1].lines[0].amount, Decimal('6.3'))
-        self.assertEqual(books[1].lines[0].amount_2nd_currency, Decimal('6.0'))
+        self.assertEqual(
+            books[1].lines[0].amount, Decimal('6.3'))
+        self.assertEqual(
+            books[1].lines[0].amount_2nd_currency, Decimal('6.0'))
 
         # wf: check --> edit
         Line.wfedit(books[0].lines)
         self.assertEqual(len(books[0].lines), 1)
         self.assertEqual(len(books[0].lines[0].references), 0)
         self.assertEqual(len(books[1].lines), 0)
 
@@ -294,15 +319,17 @@
                     'bookingtype': 'in',
                     'amount': Decimal('1.0'),
                     'party': party.id,
                 }])],
             }])
 
         self.assertEqual(len(book.lines), 1)
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|1.00 usd|Text 1 [Cat1]')
         self.assertEqual(book.lines[0].amount, Decimal('1.0'))
         self.assertEqual(book.lines[0].category.rec_name, 'Cat1')
 
         Lines.write(*[
             [book.lines[0]],
             {
                 'bookingtype': 'spin',
@@ -313,47 +340,56 @@
                     }, {
                     'amount': Decimal('2.0'),
                     'category': category2.id,
                     'description': 'line 2',
                     }])],
             }])
 
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev/Sp|7.00 usd|Text 1 [-]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev/Sp|7.00 usd|Text 1 [-]')
         self.assertEqual(book.lines[0].amount, Decimal('7.0'))
         self.assertEqual(book.lines[0].category, None)
 
         self.assertEqual(len(book.lines[0].splitlines), 2)
         self.assertEqual(book.lines[0].splitlines[0].amount, Decimal('5.0'))
         self.assertEqual(book.lines[0].splitlines[0].category.rec_name, 'Cat1')
         self.assertEqual(book.lines[0].splitlines[0].description, 'line 1')
-        self.assertEqual(book.lines[0].splitlines[0].rec_name, 'Rev/Sp|5.00 usd|line 1 [Cat1]')
+        self.assertEqual(
+            book.lines[0].splitlines[0].rec_name,
+            'Rev/Sp|5.00 usd|line 1 [Cat1]')
 
         self.assertEqual(book.lines[0].splitlines[1].amount, Decimal('2.0'))
         self.assertEqual(book.lines[0].splitlines[1].category.rec_name, 'Cat2')
         self.assertEqual(book.lines[0].splitlines[1].description, 'line 2')
-        self.assertEqual(book.lines[0].splitlines[1].rec_name, 'Rev/Sp|2.00 usd|line 2 [Cat2]')
+        self.assertEqual(
+            book.lines[0].splitlines[1].rec_name,
+            'Rev/Sp|2.00 usd|line 2 [Cat2]')
 
         Lines.write(*[
             [book.lines[0]],
             {
-                'splitlines': [('write',
-                    [book.lines[0].splitlines[0]],
-                    {
-                        'amount': Decimal('3.5'),
-                    })],
+                'splitlines': [
+                    ('write',
+                        [book.lines[0].splitlines[0]],
+                        {
+                            'amount': Decimal('3.5'),
+                        })],
             }])
         self.assertEqual(book.lines[0].splitlines[0].amount, Decimal('3.5'))
         self.assertEqual(book.lines[0].splitlines[1].amount, Decimal('2.0'))
         self.assertEqual(book.lines[0].amount, Decimal('5.5'))
 
         Lines.write(*[
             [book.lines[0]],
             {
                 'bookingtype': 'in',
                 'amount': Decimal('7.5'),
                 'category': category2.id,
             }])
-        self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|7.50 usd|Text 1 [Cat2]')
+        self.assertEqual(
+            book.lines[0].rec_name,
+            '05/01/2022|Rev|7.50 usd|Text 1 [Cat2]')
         self.assertEqual(book.lines[0].category.rec_name, 'Cat2')
         self.assertEqual(len(book.lines[0].splitlines), 0)
 
 # end SplitLineTestCase
```

### Comparing `mds_cashbook-6.0.27/tests/test_type.py` & `mds_cashbook-6.8.29/tests/type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 
 
-class TypeTestCase(ModuleTestCase):
-    'Test cashbook type module'
-    module = 'cashbook'
-
+class TypeTestCase(object):
+    """ test types
+    """
     def prep_type(self, name='Cash', short='CAS'):
         """ create book-type
         """
         AccType = Pool().get('cashbook.type')
 
         company = self.prep_company()
         at, = AccType.create([{
```

### Comparing `mds_cashbook-6.0.27/types.py` & `mds_cashbook-6.8.29/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import ModelView, ModelSQL, fields, Unique
+from trytond.model import ModelView, ModelSQL, fields, Unique, Index
 from trytond.transaction import Transaction
 from trytond.i18n import gettext
 
 
 class Type(ModelSQL, ModelView):
     'Cashbook Type'
     __name__ = 'cashbook.type'
 
     name = fields.Char(string='Name', required=True, translate=True)
     short = fields.Char(string='Abbreviation', required=True, size=3)
-    company = fields.Many2One(string='Company', model_name='company.company',
+    company = fields.Many2One(
+        string='Company', model_name='company.company',
         required=True, ondelete="RESTRICT")
-    feature = fields.Selection(string='Feature', required=True,
-        selection='get_sel_feature', select=True,
+    feature = fields.Selection(
+        string='Feature', required=True,
+        selection='get_sel_feature',
         help='Select feature set of the Cashbook.')
 
     @classmethod
     def __setup__(cls):
         super(Type, cls).__setup__()
         cls._order.insert(0, ('name', 'ASC'))
         t = cls.__table__()
         cls._sql_constraints.extend([
             ('code_uniq', Unique(t, t.short), 'cashbook.msg_type_short_unique'),
             ])
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.feature, Index.Equality())),
+            })
 
     @classmethod
     def default_feature(cls):
         """ default: general
         """
         return 'gen'
 
@@ -49,15 +56,16 @@
             'name': self.name or '-',
             }
 
     @classmethod
     def search_rec_name(cls, name, clause):
         """ search in name + short
         """
-        return ['OR',
+        return [
+            'OR',
             ('name',) + tuple(clause[1:]),
             ('short',) + tuple(clause[1:]),
             ]
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company') or None
```

### Comparing `mds_cashbook-6.0.27/types.xml` & `mds_cashbook-6.8.29/types.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/book_form.xml` & `mds_cashbook-6.8.29/view/book_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/category_form.xml` & `mds_cashbook-6.8.29/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/configuration_form.xml` & `mds_cashbook-6.8.29/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/enterbooking_start_form.xml` & `mds_cashbook-6.8.29/view/enterbooking_start_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/line_form.xml` & `mds_cashbook-6.8.29/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/line_list.xml` & `mds_cashbook-6.8.29/view/line_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/line_recon_list.xml` & `mds_cashbook-6.8.29/view/line_recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/recon_form.xml` & `mds_cashbook-6.8.29/view/recon_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/split_form.xml` & `mds_cashbook-6.8.29/view/split_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/split_list.xml` & `mds_cashbook-6.8.29/view/split_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/wizard_openline_form.xml` & `mds_cashbook-6.8.29/view/wizard_openline_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/view/wizard_runrepbook_form.xml` & `mds_cashbook-6.8.29/view/wizard_runrepbook_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/wizard_booking.py` & `mds_cashbook-6.8.29/wizard_booking.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,73 +3,82 @@
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import ModelView, fields
 from trytond.wizard import Wizard, StateView, StateTransition, Button
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.pyson import Eval, Bool, If, And
+from trytond.pyson import Eval, Bool, If
 from decimal import Decimal
 from .line import sel_bookingtype
 
 sel_booktypewiz = [x for x in sel_bookingtype if not x[0] in ['spin', 'spout']]
 
 
 class EnterBookingStart(ModelView):
     'Enter Booking'
     __name__ = 'cashbook.enterbooking.start'
 
-    cashbook = fields.Many2One(string='Cashbook', model_name='cashbook.book',
+    cashbook = fields.Many2One(
+        string='Cashbook', model_name='cashbook.book',
         domain=[('id', 'in', Eval('cashbooks', [])), ('btype', '!=', None)],
         depends=['cashbooks'], required=True)
-    cashbooks = fields.One2Many(string='Cashbooks', field=None,
+    cashbooks = fields.One2Many(
+        string='Cashbooks', field=None,
         model_name='cashbook.book', readonly=True,
         states={'invisible': True})
-    owner_cashbook = fields.Function(fields.Many2One(string='Owner', readonly=True,
+    owner_cashbook = fields.Function(fields.Many2One(
+        string='Owner', readonly=True,
         states={'invisible': True}, model_name='res.user'),
         'on_change_with_owner_cashbook')
-    currency = fields.Function(fields.Many2One(string='Currency',
+    currency = fields.Function(fields.Many2One(
+        string='Currency',
         model_name='currency.currency', states={'invisible': True}),
         'on_change_with_currency')
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits',
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits',
         readonly=True, states={'invisible': True}),
         'on_change_with_currency_digits')
-    bookingtype = fields.Selection(string='Type', required=True,
-        selection=sel_booktypewiz)
-    amount =  fields.Numeric(string='Amount',
+    bookingtype = fields.Selection(
+        string='Type', required=True, selection=sel_booktypewiz)
+    amount = fields.Numeric(
+        string='Amount',
         depends=['currency_digits', 'bookingtype'],
         digits=(16, Eval('currency_digits', 2)), required=True,
         domain=[('amount', '>=', Decimal('0.0'))])
     description = fields.Text(string='Description')
-    category = fields.Many2One(string='Category',
+    category = fields.Many2One(
+        string='Category',
         model_name='cashbook.category', depends=['bookingtype'],
         states={
             'readonly': Bool(Eval('bookingtype')) == False,
             'required': Eval('bookingtype', '').in_(['in', 'out']),
             'invisible': ~Eval('bookingtype', '').in_(['in', 'out']),
         },
         domain=[
             If(
                 Eval('bookingtype', '').in_(['in', 'mvin']),
                 ('cattype', '=', 'in'),
                 ('cattype', '=', 'out'),
             )])
 
     # party or cashbook as counterpart
-    booktransf = fields.Many2One(string='Source/Dest',
+    booktransf = fields.Many2One(
+        string='Source/Dest',
         model_name='cashbook.book',
         domain=[
             ('owner.id', '=', Eval('owner_cashbook', -1)),
             ('id', '!=', Eval('cashbook', -1)),
             ],
         states={
             'invisible': ~Eval('bookingtype', '').in_(['mvin', 'mvout']),
             'required': Eval('bookingtype', '').in_(['mvin', 'mvout']),
         }, depends=['bookingtype', 'owner_cashbook', 'cashbook'])
-    party = fields.Many2One(string='Party', model_name='party.party',
+    party = fields.Many2One(
+        string='Party', model_name='party.party',
         states={
             'invisible': ~Eval('bookingtype', '').in_(['in', 'out']),
         }, depends=['bookingtype'])
 
     @fields.depends('bookingtype', 'category')
     def on_change_bookingtype(self):
         """ clear category if not valid type
@@ -77,15 +86,15 @@
         types = {
             'in': ['in', 'mvin'],
             'out': ['out', 'mvout'],
             }
 
         if self.bookingtype:
             if self.category:
-                if not self.bookingtype in types.get(self.category.cattype, ''):
+                if self.bookingtype not in types.get(self.category.cattype, ''):
                     self.category = None
 
     @fields.depends('cashbook', '_parent_cashbook.owner')
     def on_change_with_owner_cashbook(self, name=None):
         """ get current owner
         """
         if self.cashbook:
@@ -100,26 +109,27 @@
 
     @fields.depends('cashbook', '_parent_cashbook.currency')
     def on_change_with_currency_digits(self, name=None):
         """ digits
         """
         if self.cashbook:
             return self.cashbook.currency.digits
-        else :
+        else:
             return 2
 
 # end EnterBookingStart
 
 
 class EnterBookingWizard(Wizard):
     'Enter Booking'
     __name__ = 'cashbook.enterbooking'
 
     start_state = 'start'
-    start = StateView('cashbook.enterbooking.start',
+    start = StateView(
+        'cashbook.enterbooking.start',
         'cashbook.enterbooking_start_form', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Save', 'save_', 'tryton-save', default=True),
             Button('Save & Next', 'savenext_', 'tryton-forward'),
             ])
     save_ = StateTransition()
     savenext_ = StateTransition()
```

### Comparing `mds_cashbook-6.0.27/wizard_booking.xml` & `mds_cashbook-6.8.29/wizard_booking.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/wizard_openline.py` & `mds_cashbook-6.8.29/wizard_openline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import ModelView, fields
 from trytond.pyson import PYSONEncoder
-from trytond.wizard import Wizard, StateView, StateTransition, StateAction, Button
+from trytond.wizard import Wizard, StateView, StateTransition, \
+    StateAction, Button
 from trytond.i18n import gettext
 from trytond.pool import Pool
 from trytond.exceptions import UserError
 from trytond.transaction import Transaction
 
 
 class OLineMixin:
@@ -24,32 +25,35 @@
             'pyson_context': PYSONEncoder().encode({
                 'cashbook': getattr(book, 'id', None),
                 'date_from': getattr(cfg1, 'date_from', None),
                 'date_to': getattr(cfg1, 'date_to', None),
                 'checked': getattr(cfg1, 'checked', None),
                 'done': getattr(cfg1, 'done', None),
                 }),
-            'name' : '%(name)s: %(cashbook)s' % {
+            'name': '%(name)s: %(cashbook)s' % {
                 'name': gettext('cashbook.msg_name_cashbook'),
                 'cashbook': getattr(book, 'rec_name', '-/-'),
                 },
             }
         return action
 
 # OLineMixin
 
 
 class OpenCashBookStart(ModelView):
     'Open Cashbook'
     __name__ = 'cashbook.open_lines.start'
 
-    cashbook = fields.Many2One(string='Cashbook', model_name='cashbook.book',
+    cashbook = fields.Many2One(
+        string='Cashbook', model_name='cashbook.book',
         required=True, domain=[('btype', '!=', None)])
-    checked = fields.Boolean(string='Checked', help="Show cashbook lines in Checked-state.")
-    done = fields.Boolean(string='Done', help="Show cashbook lines in Done-state")
+    checked = fields.Boolean(
+        string='Checked', help="Show cashbook lines in Checked-state.")
+    done = fields.Boolean(
+        string='Done', help="Show cashbook lines in Done-state")
     date_from = fields.Date(string='Start Date')
     date_to = fields.Date(string='End Date')
 
     @classmethod
     def default_checked(cls):
         return True
 
@@ -62,29 +66,29 @@
 
 class OpenCashBook(OLineMixin, Wizard):
     'Open Cashbook'
     __name__ = 'cashbook.open_lines'
 
     start_state = 'check'
     check = StateTransition()
-    askuser = StateView('cashbook.open_lines.start',
+    askuser = StateView(
+        'cashbook.open_lines.start',
         'cashbook.open_lines_view_form', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Open', 'open_', 'tryton-ok', default=True),
             ])
     open_ = StateAction('cashbook.act_line_view2')
 
     def transition_check(self):
         """ dont ask and open cashbook if user has 1x only
         """
         Book = Pool().get('cashbook.book')
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             books = Book.search([('btype', '!=', None)])
             if len(books) == 1:
                 return 'open_'
         return 'askuser'
 
     def default_askuser(self, fields):
         """ setup form
@@ -111,16 +115,15 @@
         if cfg1 is None:
             cfg1 = Configuration()
             cfg1.save()
 
         book = getattr(self.askuser, 'cashbook', None)
         if book is None:
             with Transaction().set_context({
-                '_check_access': True,
-                }):
+                    '_check_access': True}):
                 books = Book.search([('btype', '!=', None)])
                 if len(books) > 0:
                     book = books[0]
 
         # save settings
         cfg1.date_from = getattr(self.askuser, 'date_from', None)
         cfg1.date_to = getattr(self.askuser, 'date_to', None)
@@ -154,23 +157,21 @@
         if cfg1 is None:
             cfg1 = Configuration()
             cfg1.save()
 
         book = self.record
         if book is None:
             with Transaction().set_context({
-                '_check_access': True,
-                }):
+                    '_check_access': True}):
                 books = Book.search([('btype', '!=', None)])
                 if len(books) > 0:
                     book = books[0]
-        else :
+        else:
             if book.btype is None:
                 raise UserError(gettext(
                     'cashbook.msg_book_no_type_noopen',
-                    bookname = book.rec_name,
-                    ))
+                    bookname=book.rec_name))
 
         action.update(self.add_action_data(book))
         return action, {}
 
 # end OpenCashBookTree
```

### Comparing `mds_cashbook-6.0.27/wizard_openline.xml` & `mds_cashbook-6.8.29/wizard_openline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.0.27/wizard_runreport.py` & `mds_cashbook-6.8.29/wizard_runreport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds.de for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import ModelView, fields
-from trytond.pyson import PYSONEncoder
 from trytond.wizard import Wizard, StateView, StateReport, Button
 from trytond.pool import Pool
 from trytond.pyson import Eval, Bool
 from trytond.transaction import Transaction
 
 
 class RunCbReportStart(ModelView):
     'Cashbook Report'
     __name__ = 'cashbook.runrepbook.start'
 
-    cashbook = fields.Many2One(string='Cashbook', required=True,
+    cashbook = fields.Many2One(
+        string='Cashbook', required=True,
         model_name='cashbook.book', depends=['cashbooks'],
         domain=[('id', 'in', Eval('cashbooks', []))])
-    cashbooks = fields.One2Many(string='Cashbooks', model_name='cashbook.book',
+    cashbooks = fields.One2Many(
+        string='Cashbooks', model_name='cashbook.book',
         field=None, readonly=True, states={'invisible': True})
-    reconciliation = fields.Many2One(string='Reconciliation', required=True,
+    reconciliation = fields.Many2One(
+        string='Reconciliation', required=True,
         model_name='cashbook.recon', depends=['reconciliations'],
         states={
             'readonly': ~Bool(Eval('reconciliations')),
         }, domain=[('id', 'in', Eval('reconciliations', []))])
-    reconciliations = fields.Function(fields.One2Many(string='Reconciliations',
+    reconciliations = fields.Function(fields.One2Many(
+        string='Reconciliations',
         model_name='cashbook.recon', field=None, readonly=True,
         states={'invisible': True}),
         'on_change_with_reconciliations')
 
     @fields.depends('cashbook', 'reconciliations', 'reconciliation')
     def on_change_cashbook(self):
         """ update reconciliations
         """
         if self.cashbook:
             self.reconciliations = self.on_change_with_reconciliations()
             if len(self.reconciliations or []) > 0:
                 self.reconciliation = self.reconciliations[0]
-            else :
+            else:
                 self.reconciliation = None
-        else :
+        else:
             self.reconciliations = []
             self.reconciliation = None
 
     @fields.depends('cashbook')
     def on_change_with_reconciliations(self, name=None):
         """ get reconciliations of current cashbook
         """
@@ -60,22 +63,22 @@
 
 
 class RunCbReport(Wizard):
     'Cashbook Report'
     __name__ = 'cashbook.runrepbook'
 
     start_state = 'selrecon'
-    selrecon = StateView('cashbook.runrepbook.start',
+    selrecon = StateView(
+        'cashbook.runrepbook.start',
         'cashbook.runrepbook_view_form', [
             Button(string='Cancel', state='end', icon='tryton-cancel'),
-            Button(string='Report', state='report_', icon='tryton-ok', default=True,
-                states={
-                    'readonly': ~Bool(Eval('reconciliation')),
-                    }),
-            ])
+            Button(
+                string='Report', state='report_', icon='tryton-ok',
+                default=True,
+                states={'readonly': ~Bool(Eval('reconciliation'))})])
     report_ = StateReport('cashbook.reprecon')
 
     def default_selrecon(self, fields):
         """ setup form
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -83,20 +86,19 @@
         context = Transaction().context
 
         result = {}
         if context.get('active_model', '') == 'cashbook.book':
             result['cashbook'] = context.get('active_id', None)
         elif context.get('active_model', '') == 'cashbook.line':
             result['cashbook'] = context.get('cashbook', None)
-        else :
+        else:
             raise ValueError('invalid model')
 
         with Transaction().set_context({
-            '_check_access': True,
-            }):
+                '_check_access': True}):
             books = Book.search([])
             result['cashbooks'] = [x.id for x in books]
 
             if len(result['cashbooks']) > 0:
                 if result['cashbook'] is None:
                     result['cashbook'] = result['cashbooks'][0]
 
@@ -114,15 +116,15 @@
         # values for 'data' in report
         if self.selrecon.reconciliation:
             r1 = {
                 'model': self.selrecon.reconciliation.__name__,
                 'id': self.selrecon.reconciliation.id,
                 'ids': [self.selrecon.reconciliation.id],
                 }
-        else :
+        else:
             r1 = {'model': '', 'id': None, 'ids': []}
         return action, r1
 
     def transition_report_(self):
         return 'end'
 
 # end RunCbReport
```

### Comparing `mds_cashbook-6.0.27/wizard_runreport.xml` & `mds_cashbook-6.8.29/wizard_runreport.xml`

 * *Files identical despite different names*

