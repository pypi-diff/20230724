# Comparing `tmp/werk24-1.5.1.tar.gz` & `tmp/werk24-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/werk24-1.5.1.tar", last modified: Sat Jun  3 15:30:23 2023, max compression
+gzip compressed data, was "dist/werk24-1.6.0.tar", last modified: Mon Jul 24 13:11:18 2023, max compression
```

## Comparing `werk24-1.5.1.tar` & `werk24-1.6.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 15:30:13.000000 werk24-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 15:30:13.000000 werk24-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-03 15:30:13.000000 werk24-1.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-03 15:30:23.000000 werk24-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-03 15:30:13.000000 werk24-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:30:23.000000 werk24-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-03 15:30:13.000000 werk24-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/fonts/STIX2Text-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/fonts/STIX_2.0.2_license.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/favicon-24x24.png
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/favicon-256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/favicon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/assets/images/logo-625.png
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/cli/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/cli/w24cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/event_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/event_illustrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/gdt_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/measure_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/w24gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/gui/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    28737 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/depth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/models/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/feature/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/feature/knurl.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/file_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/general_tolerances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/geometric_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/leader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/paper_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/part_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/physical_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24/models/property/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/cleanness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/corrosion_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/hardness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/material.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/surface_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/property/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/revision_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/roughness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/size.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/thread_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/title_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/typed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/value.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/models/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    29423 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/techread_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/techread_client_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/techread_client_wss.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-03 15:30:13.000000 werk24-1.5.1/werk24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 15:30:23.000000 werk24-1.5.1/werk24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 13:10:49.000000 werk24-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 13:10:49.000000 werk24-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 13:10:49.000000 werk24-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 13:11:18.000000 werk24-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-24 13:10:49.000000 werk24-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:11:18.000000 werk24-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 13:10:49.000000 werk24-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/fonts/STIX2Text-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/fonts/STIX_2.0.2_license.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/logo-625.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/w24cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/event_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/event_illustrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/gdt_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/measure_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/w24gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28765 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/depth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/knurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/general_tolerances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/geometric_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/helpdesk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/leader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/paper_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/part_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/physical_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/cleanness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/corrosion_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/surface_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/revision_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/roughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/thread_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/title_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/typed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32337 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client_wss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/top_level.txt
```

### Comparing `werk24-1.5.1/PKG-INFO` & `werk24-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.5.1
+Version: 1.6.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.5.1 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.6.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
```

### Comparing `werk24-1.5.1/README.md` & `werk24-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/setup.py` & `werk24-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/fonts/STIX2Text-Regular.otf` & `werk24-1.6.0/werk24/assets/fonts/STIX2Text-Regular.otf`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/fonts/STIX_2.0.2_license.pdf` & `werk24-1.6.0/werk24/assets/fonts/STIX_2.0.2_license.pdf`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/images/favicon-256x256.png` & `werk24-1.6.0/werk24/assets/images/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/images/favicon-32x32.png` & `werk24-1.6.0/werk24/assets/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/images/favicon-48x48.png` & `werk24-1.6.0/werk24/assets/images/favicon-48x48.png`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/assets/images/logo-625.png` & `werk24-1.6.0/werk24/assets/images/logo-625.png`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/auth_client.py` & `werk24-1.6.0/werk24/auth_client.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/cli/auth.py` & `werk24-1.6.0/werk24/cli/auth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/cli/techread.py` & `werk24-1.6.0/werk24/cli/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/cli/utils.py` & `werk24-1.6.0/werk24/cli/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/cli/w24cli.py` & `werk24-1.6.0/werk24/cli/w24cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,93 @@
 """ Command Line Interface for W24
 """
 import argparse
 import asyncio
 from dotenv import load_dotenv
 import werk24.cli.techread
 import werk24.cli.auth
+import werk24.cli.support
 
 load_dotenv(".werk24")
 
 
 def main() -> None:
 
     parser = argparse.ArgumentParser(prog="w24cli")
     subparsers = parser.add_subparsers(
-        dest="command",
-        help="Subcommand. Currently supported: techread")
+        dest="service",
+        help="Service. Currently supported: techread, auth, support")
     subparsers.required = True
 
+    _add_auth_parser(subparsers)
+    _add_support_parser(subparsers)
+    _add_techread_parser(subparsers)
+
+    args = parser.parse_args()
+    if args.service == "techread":
+        asyncio.run(werk24.cli.techread.main(args))
+
+    elif args.service == "auth":
+        asyncio.run(werk24.cli.auth.main(args))
+
+    elif args.service == "support":
+        asyncio.run(werk24.cli.support.main(args))
+
+
+def _add_support_parser(subparsers):
+    support_parser = subparsers.add_parser(
+        "support",
+        help="Support Service")
+
+    support_subparsers = support_parser.add_subparsers(
+        dest="command",
+        help="Command. Currently supported: create-helpdesk-task",
+        required=True)
+
+    create_parser = support_subparsers.add_parser(
+        "create-helpdesk-task",
+        help="Create a new help desk task")
+
+    create_parser.add_argument(
+        "--request-id",
+        action="store",
+        required=True)
+
+    create_parser.add_argument(
+        "--observed-outcome",
+        action="store",
+        required=True)
+
+    create_parser.add_argument(
+        "--expected-outcome",
+        action="store",
+        required=True)
+
+    create_parser.add_argument(
+        "--comment",
+        action="store")
+
+    create_parser.add_argument(
+        "--importance",
+        action="store",
+        required=True)
+
+
+def _add_auth_parser(subparsers):
+    parser_auth = subparsers.add_parser(
+        "auth",
+        help="Interact with the authentication service")
+
+    parser_auth.add_argument(
+        '--ask-jwt-token',
+        help="Obtain a valid JWT token",
+        action="store_true")
+
+
+def _add_techread_parser(subparsers):
     parser_techread = subparsers.add_parser(
         "techread",
         help="Submit a Technical Drawing to Werk24 for analysis")
 
     parser_techread.add_argument(
         "input_file",
         help="path to the file that is to be analyzed")
@@ -98,26 +165,10 @@
         action="store_true")
 
     parser_techread.add_argument(
         "--ask-titleblock",
         help="ask for the Title Block",  # noqa
         action="store_true")
 
-    parser_auth = subparsers.add_parser(
-        "auth",
-        help="Interact with the authentication service")
-
-    parser_auth.add_argument(
-        '--ask-jwt-token',
-        help="Obtain a valid JWT token",
-        action="store_true")
-
-    args = parser.parse_args()
-    if args.command == "techread":
-        asyncio.run(werk24.cli.techread.main(args))
-
-    elif args.command == "auth":
-        asyncio.run(werk24.cli.auth.main(args))
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `werk24-1.5.1/werk24/exceptions.py` & `werk24-1.6.0/werk24/exceptions.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/event_feed.py` & `werk24-1.6.0/werk24/gui/event_feed.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/event_illustrator.py` & `werk24-1.6.0/werk24/gui/event_illustrator.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/gdt_table.py` & `werk24-1.6.0/werk24/gui/gdt_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/measure_table.py` & `werk24-1.6.0/werk24/gui/measure_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/w24gui.py` & `werk24-1.6.0/werk24/gui/w24gui.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/gui/worker.py` & `werk24-1.6.0/werk24/gui/worker.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/angle.py` & `werk24-1.6.0/werk24/models/angle.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/ask.py` & `werk24-1.6.0/werk24/models/ask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Definition of all W24Ask types that are understood by the Werk24 API.
 """
-from werk24.models.process import W24Process
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from pydantic import UUID4, BaseModel, HttpUrl
 
 from werk24.models.note import W24Note
 from werk24.models.part_family import W24PartFamilyCharacterization
+from werk24.models.process import W24Process
 
 from .angle import W24Angle
 from .file_format import W24FileFormatThumbnail, W24FileFormatVariantCAD
 from .gdt import W24GDT
 from .general_tolerances import W24GeneralTolerances
 from .geometric_shape import W24GeometricShapeCuboid, W24GeometricShapeCylinder
 from .leader import W24Leader
@@ -842,14 +842,15 @@
     W24AskVariantLeaders,
     W24AskVariantMaterial,
     W24AskVariantMeasures,
     W24AskVariantRadii,
     W24AskVariantRoughnesses,
     W24AskVariantThreadElements,
     W24AskInternalScreening,
+    W24AskVariantProcesses
     # W24AskVariantToleranceElements
 ]
 """Union of all W24Asks to ensure proper de-serialization """
 
 
 def deserialize_ask(
     raw: Union[Dict[str, Any], W24Ask],
```

### Comparing `werk24-1.5.1/werk24/models/base_feature.py` & `werk24-1.6.0/werk24/models/base_feature.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/chamfer.py` & `werk24-1.6.0/werk24/models/chamfer.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/depth.py` & `werk24-1.6.0/werk24/models/depth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/feature/base.py` & `werk24-1.6.0/werk24/models/feature/base.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/feature/knurl.py` & `werk24-1.6.0/werk24/models/feature/knurl.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/file_format.py` & `werk24-1.6.0/werk24/models/file_format.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/gdt.py` & `werk24-1.6.0/werk24/models/gdt.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/general_tolerances.py` & `werk24-1.6.0/werk24/models/general_tolerances.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional, Union
+
 from pydantic import BaseModel, validator
 
+from werk24.models.unit import W24UnitLength
+
 from .base_feature import W24BaseFeatureModel
 
 
 class W24GeneralTolerancesStandard(str, Enum):
     """ Enum of all supported
     General Tolerance Standards
     """
     DIN_7168 = "DIN 7168"
     ISO_2768 = "ISO 2768"
     ISO_4759_1 = "ISO 4759-1"
-    DEFINED_ON_SHEET = "DEFINED_ON_SHEET"
+    TOLERANCE_NOTE = "TOLERANCE_NOTE"
 
 
 class W24ToleranceProperty(str, Enum):
     """ Enum of all attributes that can
     be described by general tolerances
     """
     ANGULAR = "ANGULAR"
@@ -34,15 +37,50 @@
     """ Enum of the supported General Tolerance
     Principles.
     """
     INDEPENDENCE = "INDEPENDENCE"
     ENVELOPE = "ENVELOPE"
 
 
+class W24IntervalEnd(str, Enum):
+    """
+    Enum for handling the interval ends.
+    Open for  `<`
+    Close for `<=`
+    """
+    OPEN = "OPEN"
+    CLOSE = "CLOSE"
+
+
 class W24ToleranceTableItem(BaseModel):
+    """
+    Tolerance Table Item.
+
+    Attributes:
+        nominal_min: Lower bound of the nominal value
+        nominal_min_end: Interval end of the lower bound
+        nominal_max: Upper bound of the nominal value
+        nominal_max_end: Interval end of the upper bound
+        decimal_places: Number of decimal places. This is
+            required for US-type tolerances.
+        deviation_min: Lower bound of the deviation
+        deviation_max: Upper bound of the deviation
+    """
+
+    nominal_min: Optional[Decimal]
+    nominal_min_end: W24IntervalEnd = W24IntervalEnd.OPEN
+    nominal_max: Optional[Decimal]
+    nominal_max_end: W24IntervalEnd = W24IntervalEnd.CLOSE
+
+    decimal_places: Optional[int] = None
+
+    deviation_min: Optional[Decimal]
+    deviation_max: Optional[Decimal]
+
+    unit: Optional[W24UnitLength] = None
 
     @validator('nominal_min', pre=True)
     def nominal_min_validator(  # NOQA
         cls,
         raw: Union[str, float, None]
     ) -> Optional[Decimal]:
         """ Ensure the proper conversion of the the
@@ -60,15 +98,15 @@
         """
         return cls._convert_decimal(raw)
 
     @staticmethod
     def _convert_decimal(
         raw: Union[str, float, None]
     ) -> Optional[Decimal]:
-        """ Handle the decimal converstion
+        """ Handle the decimal conversion
 
         Args:
             raw (Union[str, float, None]): Raw value
 
         Raises:
             ValueError: raised when the data type
                 does not match the understood types
@@ -111,19 +149,14 @@
         # enforce zero to be positive
         if decimal == Decimal('-0'):
             return Decimal('0')
 
         # accept the value
         return decimal
 
-    nominal_min: Optional[Decimal]
-    nominal_max: Optional[Decimal]
-    deviation_min: Optional[Decimal]
-    deviation_max: Optional[Decimal]
-
 
 class W24ToleranceClass(BaseModel):
     """ Tolerance Class which matches an individual attribute
     of the General Tolerances to a tolerance property and
     tolerance table
 
     Attributes:
@@ -131,59 +164,41 @@
 
         property: Property that is being tolerated
 
         table: Rows of the tolerance table that correspond
             to the selected tolerance class
     """
     blurb: str
-
     property: W24ToleranceProperty
-
     table: List[W24ToleranceTableItem]
 
 
 class W24GeneralTolerances(W24BaseFeatureModel):
-    """ Object representing the General Tolerances indicated
-    on the Title Block of the Technical Drawing.
     """
+    General Tolerances on the Title Block of the Technical Drawing.
 
-    blurb: str
-    """ Blurb of the general tolerances for human consumption
-    """
+    Attributes:
+        blurb: Blurb of the general tolerances for human consumption.
+        tolerance_standard: General Tolerance Standard that was defined
+            in the Drawing
+        principle: Principle that is annotated on the general tolerance
+            by "-E" (or the lack of if).
+        angular_class: Angular toleration class
+        flatness_class: Flatness toleration class
+        straightness_class: Straightness toleration class
+        linear_class: Linear toleration class
+        radius_class: Radius and chamfer toleration class
+        symmetry_class: Symmetry toleration class
+        perpendicularity_class: Perpendicularity toleration class
 
-    tolerance_standard: W24GeneralTolerancesStandard
-    """ GeneralTolerance Standard that was defined
-    in the Drawing
     """
-
+    blurb: str
+    tolerance_standard: W24GeneralTolerancesStandard
     principle: Optional[W24GeneralTolerancesPrinciple]
-    """ Principle that is annotated on the general
-    tolerance by "-E" (or the lack of if).
-
-    NOTE: some general tolerance standards do not define
-    a default principle. If it is not stated explicitly
-    on the drawing, the `principle` value is set to `None`.
-    """
-
     angular_class: Optional[W24ToleranceClass]
-    """ Angular toleration class """
-
     flatness_class: Optional[W24ToleranceClass]
-    """ Flatness toleration class """
-
     straightness_class: Optional[W24ToleranceClass]
-    """ Straightness toleration class """
-
     linear_class: Optional[W24ToleranceClass]
-    """ Linear toleration class """
-
     radius_class: Optional[W24ToleranceClass]
-    """ Radius and chamfer toleration class """
-
     runout_class: Optional[W24ToleranceClass]
-    """ Runout toleration class """
-
     symmetry_class: Optional[W24ToleranceClass]
-    """ Symmetry toleration class """
-
     perpendicularity_class: Optional[W24ToleranceClass]
-    """ Perpendicularity toleration class - not defined in DIN7168 """
```

### Comparing `werk24-1.5.1/werk24/models/geometric_shape.py` & `werk24-1.6.0/werk24/models/geometric_shape.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/leader.py` & `werk24-1.6.0/werk24/models/leader.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/location.py` & `werk24-1.6.0/werk24/models/location.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/material.py` & `werk24-1.6.0/werk24/models/material.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/measure.py` & `werk24-1.6.0/werk24/models/measure.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/note.py` & `werk24-1.6.0/werk24/models/note.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/paper_size.py` & `werk24-1.6.0/werk24/models/paper_size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/part_family.py` & `werk24-1.6.0/werk24/models/part_family.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/physical_quantity.py` & `werk24-1.6.0/werk24/models/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/cleanness.py` & `werk24-1.6.0/werk24/models/property/cleanness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/color.py` & `werk24-1.6.0/werk24/models/property/color.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/corrosion_resistance.py` & `werk24-1.6.0/werk24/models/property/corrosion_resistance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/hardness.py` & `werk24-1.6.0/werk24/models/property/hardness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/material.py` & `werk24-1.6.0/werk24/models/property/material.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/surface_area.py` & `werk24-1.6.0/werk24/models/property/surface_area.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/property/weight.py` & `werk24-1.6.0/werk24/models/property/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/radius.py` & `werk24-1.6.0/werk24/models/radius.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/revision_table.py` & `werk24-1.6.0/werk24/models/revision_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/roughness.py` & `werk24-1.6.0/werk24/models/roughness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/size.py` & `werk24-1.6.0/werk24/models/size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/techread.py` & `werk24-1.6.0/werk24/models/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/test_dimension.py` & `werk24-1.6.0/werk24/models/test_dimension.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/thread.py` & `werk24-1.6.0/werk24/models/thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         as individual types will be deprecated. Their information
         individual `threads_per_inch` information will be stored
         in the corresponding variable.
     """
     ISO_METRIC = "ISO_METRIC"
     WHITWORTH = "WHITWORTH"
     UTS = "UTS"
+    SM = "SM"
+    NPT = "NPT"
+    ACME = "ACME"
 
     # !!! DEPRECATED
     UTS_COARSE = "UTS_COARSE"
 
     # !!! DEPRECATED
     UTS_FINE = "UTS_FINE"
 
@@ -173,14 +176,32 @@
 
     female_major_diameter_tolerance: Optional[W24Tolerance]
     female_pitch_diameter_tolerance: Optional[W24Tolerance]
     male_major_diameter_tolerance: Optional[W24Tolerance]
     male_pitch_diameter_tolerance: Optional[W24Tolerance]
 
 
+class W24ThreadSM(W24Thread):
+
+    """ Sewing Machine Threads (SM)
+        SM thread is used in sewing machine, 
+        recently it is also being used in Optical Industry. 
+
+    Attributes:
+        sm_size: Only few sizes are available (05,1,1.5,2,3)
+            Examples: SM05, SM1, etc
+
+        threads_per_inch: Threads per inch is fixed to 40.
+
+    """
+    thread_type = W24ThreadType.SM
+
+    sm_size: Decimal
+
+
 class W24ThreadUTS(W24Thread):
 
     """ Unified Thread Standard (UTS) base class for
     * UNC - Unified National Coarse Thread
     * UNF - Unified National Fine Thread
     * UNEF - Unified National Extrafine Thread
 
@@ -205,14 +226,63 @@
 
     uts_size: str
     uts_series: str
 
     tolerance_class: str
 
 
+class W24ThreadACME(W24Thread):
+
+    """ American Corps of Mechanical Engineering (ACME)  defines
+    * ACME - American Corps of Mechanical Engineering Thread
+    * STUB ACME - STUB American Corps of Mechanical Engineering Thread
+
+    Attributes:
+        acme_size: ACME size as string representation.
+            Threads diameter in inch are represented as decimal or fractions
+                with a tailing '"'
+            Examples: 2", 1 3/4"
+
+        acme_series (str): ACME series following ASME B1.8-1977.
+            Valid values include ACME, STUB ACME
+
+        threads_per_inch: Threads per inch. can be Decimal / Fraction.
+
+    """
+    thread_type = W24ThreadType.ACME
+
+    acme_size: str
+    acme_series: str
+
+
+class W24ThreadNPT(W24Thread):
+
+    """ American National Standard Pipe Thread standards, 
+        often called National Pipe Thread (NPT) standards.  
+    * NPT - National pipe taper
+    * NPS - National pipe straight
+
+    Attributes:
+        npt_size: NPT size as string representation.
+            Threads diameter in inch are represented as decimal or fractions
+                with a tailing '"'
+            Examples: 2", 1 3/4"
+
+        npt_series (str): NPT series following ANSI B 1.20.1.
+            Valid values include NPT, NPTF, NPSC, NPSF, NPSL, NPSM
+
+        threads_per_inch: Threads per inch. can be Decimal / Fraction.
+
+    """
+    thread_type = W24ThreadType.NPT
+
+    npt_size: str
+    npt_series: str
+
+
 class W24ThreadUTSCoarse(W24ThreadUTS):
     """ Unified National Coarse Thread
 
     NOTE: will be deprecated in favor of W24ThreadUTS
     """
     thread_type = W24ThreadType.UTS_COARSE
 
@@ -320,15 +390,18 @@
     Raises:
         ValueError: Raised if ask type is unknown
 
     Returns:
         str: Name of the AskObject
     """
     class_ = {
+        "ACME": W24ThreadACME,
         "ISO_METRIC": W24ThreadISOMetric,
+        "NPT": W24ThreadNPT,
+        "SM": W24ThreadSM,
         "WHITWORTH": W24ThreadWhitworth,
         "UTS": W24ThreadUTS,
     }.get(thread_type, None)
 
     if class_ is None:
         raise ValueError(f"Unknown Ask Type '{thread_type}'")
```

### Comparing `werk24-1.5.1/werk24/models/thread_element.py` & `werk24-1.6.0/werk24/models/thread_element.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from pydantic import BaseModel, validator
 from decimal import Decimal
 from typing import Optional, List, Dict, Any, Union, Type
 
 from .gender import W24Gender
-from .thread import W24Thread, W24ThreadISOMetric, W24ThreadUTS, W24ThreadWhitworth
-
+from .thread import (
+    W24Thread,
+    W24ThreadISOMetric,
+    W24ThreadSM,
+    W24ThreadUTS,
+    W24ThreadWhitworth,
+    W24ThreadACME,
+    W24ThreadNPT
+)
 
 
 def deserialize_thread(
     raw: Union[Dict[str, Any], W24Thread],
 ) -> W24Thread:
     """ Deserialize a specific ask in its raw form
 
@@ -24,14 +31,15 @@
         return ask_type.parse_obj(raw)
 
     if isinstance(raw, W24Thread):
         return raw
 
     raise ValueError(f"Unsupported value type '{type(raw)}'")
 
+
 def _deserialize_thread_type(
     ask_type: str
 ) -> Type[W24Thread]:
     """ Get the Ask Class from the ask type
 
     Args:
         ask_type (str): Ask type in question
@@ -39,15 +47,18 @@
     Raises:
         ValueError: Raised if ask type is unknown
 
     Returns:
         str: Name of the AskObject
     """
     class_ = {
+        "ACME": W24ThreadACME,
         "ISO_METRIC": W24ThreadISOMetric,
+        "NPT": W24ThreadNPT,
+        "SM": W24ThreadSM,
         "WHITWORTH": W24ThreadWhitworth,
         "UTS": W24ThreadUTS,
     }.get(ask_type, None)
 
     if class_ is None:
         raise ValueError(f"Unknown Ask Type '{ask_type}'")
```

### Comparing `werk24-1.5.1/werk24/models/title_block.py` & `werk24-1.6.0/werk24/models/title_block.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/tolerance.py` & `werk24-1.6.0/werk24/models/tolerance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/typed_model.py` & `werk24-1.6.0/werk24/models/typed_model.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/unit.py` & `werk24-1.6.0/werk24/models/unit.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/value.py` & `werk24-1.6.0/werk24/models/value.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/view.py` & `werk24-1.6.0/werk24/models/view.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/models/weight.py` & `werk24-1.6.0/werk24/models/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/techread_client.py` & `werk24-1.6.0/werk24/techread_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     BadRequestException,
     LicenseError,
     RequestTooLargeException,
     ServerException,
     UnsupportedMediaType,
 )
 from werk24.models.ask import W24Ask
+from werk24.models.helpdesk import W24HelpdeskTask
 from werk24.models.techread import (
     W24TechreadAction,
     W24TechreadBaseResponse,
     W24TechreadException,
     W24TechreadExceptionLevel,
     W24TechreadExceptionType,
     W24TechreadInitResponse,
@@ -69,15 +70,15 @@
     "W24TECHREAD_VERSION",
     "W24TECHREAD_AUTH_CLIENT_ID",
     "W24TECHREAD_AUTH_CLIENT_SECRET",
     "W24TECHREAD_AUTH_IDENTITY_POOL_ID",
     "W24TECHREAD_AUTH_USER_POOL_ID",
     "W24TECHREAD_AUTH_USERNAME",
     "W24TECHREAD_AUTH_PASSWORD",
-    "W24TECHREAD_AUTH_REGION"
+    "W24TECHREAD_AUTH_REGION",
 ]
 """ List of the environment variables used by the
 client """
 
 
 EXCEPTION_MAP = {
     RequestTooLargeException:
@@ -88,14 +89,15 @@
 """ Map to translate the local exceptions to official
 W24Exceptions. This allows us to mock consistent responses
 even when the files are rejected before they reach the API
 """
 
 DEFAULT_AUTH_REGION = "eu-central-1"
 DEFAULT_SERVER_WSS = "ws-api.w24.co"
+DEFAULT_SUPPORT_BASE_URL = "support.w24.co"
 
 
 LICENSE_ERROR_TEXT = """
 
 ////////////////////////////////////////////////////////////////////////////////
 
 ,.'xWWx'.,kWWd'.;0O,..'',,,,:Ox'..',,'',:lOWNo..:0MXd,.'lKWMNOc'.,;;'....';,....
@@ -149,15 +151,16 @@
     Drawings.
     """
 
     def __init__(
         self,
         techread_server_wss: str,
         techread_version: str,
-        development_key: str = None
+        development_key: str = None,
+        support_base_url: str = DEFAULT_SUPPORT_BASE_URL
     ):
         """ Initialize a new W24TechreadClient. If you wonder
         about any of the attributes, have a look at the .env
         file that we provided to you. They contain all the
         information that you will need.
 
         Arguments:
@@ -179,15 +182,16 @@
         self._development_key = development_key
 
         # Create an empty reference to the authentication
         # service (currently AWS Cognito)
         self._auth_client: Optional[AuthClient] = None
 
         # Initialize an instance of the HTTPS client
-        self._techread_client_https = TechreadClientHttps(techread_version)
+        self._techread_client_https = TechreadClientHttps(
+            techread_version, support_base_url)
 
         # Initialize an instance of the WEBSOCKET client
         self._techread_client_wss = TechreadClientWss(
             techread_server_wss, techread_version)
 
     async def __aenter__(
             self
@@ -235,15 +239,16 @@
         self,
         cognito_region: str,
         cognito_identity_pool_id: str,
         cognito_user_pool_id: str,
         cognito_client_id: str,
         cognito_client_secret: str,
         username: str,
-        password: str
+        password: str,
+
     ) -> None:
         """
         Register with the authentication
         service (i.e., lazy login)
 
         Arguments:
             cognito_region {str} -- Physical region
@@ -263,28 +268,30 @@
             cognito_client_id,
             cognito_client_secret)
 
         # register username and password
         self._auth_client.register(username, password)
 
         # tell the techread clients about it
-        self._techread_client_https.register_auth_client(self._auth_client)
+        self._techread_client_https.register_auth_client(
+            self._auth_client)
         self._techread_client_wss.register_auth_client(self._auth_client)
 
         # ensure that we have a token
         try:
             self._auth_client.login()  # type: ignore
         except AttributeError as exc:
             raise RuntimeError(
                 "No connection to the authentication service was " +
                 "established. Please call register()") from exc
 
     @property
     def username(self) -> Optional[str]:
-        """ Make the username accessible to the CLI and GUI
+        """
+        Make the username accessible to the CLI and GUI.
 
         Returns:
             str: username of the currently registered user
         """
         if self._auth_client is None:
             return None
 
@@ -295,17 +302,16 @@
         drawing: bytes,
         asks: List[W24Ask],
         model: bytes = None,
         max_pages: int = 1,
         drawing_filename: Optional[str] = None,
         sub_account: Optional[UUID4] = None
     ) -> AsyncIterator[W24TechreadBaseResponse]:
-        """ Send a Technical Drawing to the W24 API to have it automatically
-        interpreted and read. The API will return
-
+        """
+        Send a Technical Drawing to the W24 API to read it.
 
         Arguments:
             drawing (bytes): binary representation of a technical drawing.
                 Please refer to the API - documentation to learn which mime
                 types are supported.
 
             model (bytes): binary representation of the 3d model (typically
@@ -364,36 +370,67 @@
 
         # tell us when a development key is being used
         if self._development_key:  # pragma: no cover
             logger.info("Using development key %s***",
                         self._development_key[:8])
 
         # send the initiation command
-        init_response = await self._send_command_init(
+        init_response = await self.init_request(
             asks,
             max_pages,
             drawing_filename,
             sub_account)
 
         # stop if the response is unsuccessful.
         if not init_response.is_successful:
             yield init_response
             return
 
+        # Start reading the file
+        async for message in self.read_request(init_response, asks, drawing, model):
+            yield message
+
+    async def read_request(
+        self,
+        init_response: W24TechreadInitResponse,
+        asks: List[W24Ask],
+        drawing: bytes,
+        model: Optional[bytes] = None
+    ) -> None:
+        """
+        Read the request after obtaining the init_response.
+
+        This is helpful when we want to perform the reading
+        in the background or in a separate thread.
+
+        Arguments:
+            init_response (W24TechreadInitResponse): InitResponse that
+                was obtained from the init_request method
+            asks (List[W24Ask]): List of asks that we are asking for.
+                This is only used for error handling here.
+            drawing (bytes): Drawing bytes that shall be uploaded
+            model (Optional[bytes], optional): Optional model bytes.
+                Defaults to None.
+
+        Yields:
+            W24TechreadMessage: Messages that are received after the
+                request was submitted
+        """
         # upload drawing and model. We can do that in parallel.
         # If your user uploads them separately, you could also
         # upload them separately to Werk24.
         try:
-            await gather(
-                self._techread_client_https.upload_associated_file(
-                    init_response.drawing_presigned_post,
-                    drawing),
-                self._techread_client_https.upload_associated_file(
-                    init_response.model_presigned_post,
-                    model))
+            upload_drawing = self._techread_client_https.upload_associated_file(
+                init_response.drawing_presigned_post,
+                drawing)
+            upload_model = self._techread_client_https.upload_associated_file(
+                init_response.model_presigned_post,
+                model)
+
+            await gather(upload_drawing, upload_model)
 
         # explicitly reraise the exception if the payload is too
         # large
         except (BadRequestException, RequestTooLargeException) as exception:
             async for message in self._trigger_asks_exception(asks, exception):
                 yield message
             return
@@ -408,23 +445,26 @@
         # from the upload and read stages, you'll need to
         # find a way of handing over the tcp connection :)
         # PS: The AWS API Gateway for websockets might help you
         # here.
         async for message in self._send_command_read():
             yield message
 
-    async def _send_command_init(
+    async def init_request(
         self,
         asks: List[W24Ask],
         max_pages: int,
         drawing_filename: Optional[str],
         sub_account: Optional[UUID4]
     ) -> W24TechreadInitResponse:
-        """ Send the initiation command to the backend
-        and return the associated response
+        """
+        Initialize a new techread request.
+
+        This method is useful if you want to separate the
+        initialization from the upload and read stages.
 
         This achieves two things:
         1. The server has a couple of 100ms to
            reserves some resources for you, and
         2. The server will create a new request_id
            that you will need when uploading the
            associated files
@@ -704,27 +744,27 @@
             async for message in self.read_drawing(
                     drawing_bytes,
                     asks_list,
                     max_pages=max_pages,
                     drawing_filename=drawing_filename,
                     sub_account=sub_account):
 
-                await self._call_hooks_for_message(message, hooks)
+                await self.call_hooks_for_message(message, hooks)
 
         # explicitly reraise server exceptions
         except ServerException:  # pylint: disable=try-except-raise
             raise
 
-    async def _call_hooks_for_message(
-            self,
-            message: W24TechreadMessage,
-            hooks: List[Hook]
+    async def call_hooks_for_message(
+        self,
+        message: W24TechreadMessage,
+        hooks: List[Hook]
     ) -> None:
-        """ Find the correct hook for the read response and
-        call the corresponding hook.
+        """
+        Call the hook function for the response message.
 
         Arguments:
             message {W24TechreadMessage} -- Message returned from the
                 read_drawing method
 
             hooks {List[Hook]} -- List of hooks from which we need to
                 pick the suited one
@@ -758,19 +798,19 @@
         if iscoroutinefunction(hook_function):
             await hook_function(message)
         else:
             hook_function(message)
 
     @staticmethod
     def _get_hook_function_for_message(
-            message: W24TechreadMessage,
-            hooks: List[Hook]
+        message: W24TechreadMessage,
+        hooks: List[Hook]
     ) -> Optional[Callable]:
-        """ Get the hook function that corresponds to the message
-        type.
+        """
+        Get the hook function that corresponds to the message type.
 
         Arguments:
             message {W24TechreadMessage} -- Message returned from the
                 read_drawing method
 
             hooks {List[Hook]} -- List of hooks from which we need to
                 pick the suited one
@@ -779,33 +819,77 @@
             Optional[Callable] -- Hook function that should be called
         """
 
         # because we allow the user to define the ask in the hook,
         # we need to make some extra effort when filtering
         if message.message_type == W24TechreadMessageType.ASK:
             def hook_filter(hook: Hook) -> bool:
-                return hook.ask is not None \
-                    and message.message_subtype.value \
+                return (
+                    hook.ask is not None
+                    and message.message_subtype.value
                     == hook.ask.ask_type.value
+                )
 
         # if the message is of any other type, we just need to
         # compare the the message_type and message_subtype
         else:
             def hook_filter(hook: Hook) -> bool:
-                return hook.message_type is not None \
-                    and hook.message_subtype is not None \
-                    and message.message_type == hook.message_type \
+                return (
+                    hook.message_type is not None
+                    and hook.message_subtype is not None
+                    and message.message_type == hook.message_type
                     and message.message_subtype == hook.message_subtype
+                )
 
         # return the first positive case
         for cur_hook in filter(hook_filter, hooks):
             return cur_hook.function
 
         # if we are still here, we have an unknown message type, which
         # probably is being caused by an API update. We want to ensure
         # that the user is being informed, but we do not want to break
         # the existing functionality -> warning
         logger.warning(
             "Ignoring message of type %s:%s - no hook registered",  # noqa
             message.message_type,
             message.message_subtype)
         return None
+
+    async def create_helpdesk_task(
+        self,
+        task: W24HelpdeskTask
+    ) -> W24HelpdeskTask:
+        """
+        Create a Helpdesk ticket.
+
+        Args:
+            task (W24HelpdeskTask): Helpdesk task to be created
+
+        Raises:
+            BadRequestException: Raised when the request body
+                cannot be interpreted. This normally indicates
+                that the API version has been updated and that
+                we missed a corner case. If you encounter this
+                exception, it is very likely our mistake. Please
+                get in touch!
+
+            UnauthorizedException: Raised when the token
+                or the requested file have expired
+
+            ResourceNotFoundException: Raised when you are requesting
+                an endpoint that does not exist. Again, you should
+                not encounter this, but if you do, let us know.
+
+            RequestTooLargeException: Raised when the status
+                code was 413
+
+            UnsupportedMediaTypException: Raised when the file you
+                submitted cannot be read(because its media type
+                is not supported by the API).
+
+            ServerException: Raised for all other status codes
+                that are not 2xx
+
+        Returns:
+            W24HelpdeskTask: Created helpdesk task with an updated task_id.
+        """
+        return await self._techread_client_https.create_helpdesk_task(task)
```

### Comparing `werk24-1.5.1/werk24/techread_client_https.py` & `werk24-1.6.0/werk24/techread_client_https.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """ HTTPS-part of the Werk24 client
 """
+import urllib.parse
 from types import TracebackType
-from typing import Optional, Type
+from typing import Dict, Optional, Type
 
 import aiohttp
 from pydantic import HttpUrl
 
 from werk24.exceptions import (
     BadRequestException,
     RequestTooLargeException,
     ResourceNotFoundException,
     ServerException,
     UnauthorizedException,
     UnsupportedMediaType,
 )
+from werk24.models.helpdesk import W24HelpdeskTask
 from werk24.models.techread import W24PresignedPost
 
 from .auth_client import AuthClient
 
 
 class TechreadClientHttps:
 
     """ Translation map from the server response
     to the W24TechreadArchitectureStatus enum
     """
 
-    def __init__(self, techread_version: str):
+    def __init__(self, techread_version: str, support_base_url: str):
         """
         Initialize a new session with the https server.
 
         Arguments:
             techread_server_https {str} -- Domain of the Techread https server
             techread_version {str} -- Techread Version
+            support_base_url {str} -- Base URL for support requests
         """
         self._techread_version = techread_version
         self._techread_session_https: Optional[aiohttp.ClientSession] = None
         self._auth_client: Optional[AuthClient] = None
+        self._support_base_url = support_base_url
 
     async def __aenter__(
             self
     ) -> 'TechreadClientHttps':
         """ Create a new HTTP session that is being used for the whole
         connection. Be sure to keep the session alive.
 
@@ -198,16 +202,16 @@
                 ResourceNotFoundException):
             raise
 
         # otherwise return the response text
         return await response.content.read()
 
     async def _get(
-            self,
-            url: str
+        self,
+        url: str
     ) -> aiohttp.ClientResponse:
         """ Send a GET request request and return the
         response object. The method automatically
         injects the authentication token into the
         request.
 
         Arguments:
@@ -306,15 +310,15 @@
         if status_code == 400:
             raise BadRequestException()
 
         # raise an unauthorized exception if the
         # status code is
         # * 401 (Unauthorized) or
         # * 403 (Forbidden)
-        if status_code in [401, 403]:
+        if status_code in {401, 403}:
             raise UnauthorizedException()
 
         # NOTE: a 404 does not occur, as the
         # server does not want to tell you
         # whether the file does not exist
         # or whether your token is wrong.
         # Makes brute force attacks more expensive.
@@ -335,7 +339,79 @@
 
         # If the resposne code is anything other
         # than unauthorized or 200 (OK), we trigger
         # a ServerException.
         if not 200 <= status_code <= 299:
             raise ServerException(
                 f"Request failed '{url}' with code {status_code}")
+
+    async def create_helpdesk_task(
+        self,
+        task: W24HelpdeskTask
+    ) -> W24HelpdeskTask:
+        """
+        Create a Helpdesk ticket.
+
+        Args:
+            task (W24HelpdeskTask): Helpdesk task to be created
+
+        Raises:
+            BadRequestException: Raised when the request body
+                cannot be interpreted. This normally indicates
+                that the API version has been updated and that
+                we missed a corner case. If you encounter this
+                exception, it is very likely our mistake. Please
+                get in touch!
+
+            UnauthorizedException: Raised when the token
+                or the requested file have expired
+
+            ResourceNotFoundException: Raised when you are requesting
+                an endpoint that does not exist. Again, you should
+                not encounter this, but if you do, let us know.
+
+            RequestTooLargeException: Raised when the status
+                code was 413
+
+            UnsupportedMediaTypException: Raised when the file you
+                submitted cannot be read(because its media type
+                is not supported by the API).
+
+            ServerException: Raised for all other status codes
+                that are not 2xx
+
+        Returns:
+            W24HelpdeskTask: Created helpdesk task with an updated task_id.
+        """
+        headers = self._make_helpdesk_headers()
+        url = self._make_support_url("helpdesk/create-task")
+        async with aiohttp.ClientSession(headers=headers) as session:
+            response = await session.post(url, json=task.json())
+            self._raise_for_status(url, response.status)
+
+        # return the updated task
+        return W24HelpdeskTask.parse_raw(await response.text())
+
+    def _make_support_url(self, path: str) -> str:
+        """ Make the support url for the help desk requests.
+
+        Arguments:
+            path {str} -- Path to the endpoint
+
+        Returns:
+            str -- URL to the endpoint
+        """
+        return urllib.parse.urljoin(f"https://{self._support_base_url}", path)
+
+    def _make_helpdesk_headers(self) -> Dict[str, str]:
+        """
+        Make the headers for the help desk requests.
+
+        Simply the authorization header at this stage.
+
+        Returns:
+            Dict[str, str]: Help desk headers
+        """
+        headers = {
+            "Authorization": f"Bearer {self._auth_client.token}"
+        }
+        return headers
```

### Comparing `werk24-1.5.1/werk24/techread_client_wss.py` & `werk24-1.6.0/werk24/techread_client_wss.py`

 * *Files identical despite different names*

### Comparing `werk24-1.5.1/werk24/utils.py` & `werk24-1.6.0/werk24/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 from werk24 import Hook, W24TechreadClient
 
 
 async def w24_read_async(
     document_bytes: bytes,
     hooks:  List[Hook],
-    max_pages: int = 1
+    max_pages: int = 5
 ) -> None:
-    """ Convenient handler to submit an asyncronous request to the
+    """ Convenient handler to submit an asynchronous request to the
     Werk24 TechRead API.
 
     Args:
         document_bytes (bytes): Document bytes
         hooks (List[Hook]): List of Hooks that you want to
             submit.
     """
     async with W24TechreadClient.make_from_env() as session:
         await session.read_drawing_with_hooks(document_bytes, hooks, max_pages)
 
 
 def w24_read_sync(
     document_bytes: bytes,
     hooks:  List[Hook],
-    max_pages: int = 1
+    max_pages: int = 5
 ) -> None:
-    """ Convenient handler to submit a syncronous request to the
+    """ Convenient handler to submit a synchronous request to the
     Werk24 TechRead API.
 
     Args:
         document_bytes (bytes): Document bytes
         hooks (List[Hook]): List of Hooks that you want to
             submit.
     """
```

### Comparing `werk24-1.5.1/werk24.egg-info/PKG-INFO` & `werk24-1.6.0/werk24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.5.1
+Version: 1.6.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.5.1 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.6.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
```

### Comparing `werk24-1.5.1/werk24.egg-info/SOURCES.txt` & `werk24-1.6.0/werk24.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 werk24/assets/images/favicon-24x24.png
 werk24/assets/images/favicon-256x256.png
 werk24/assets/images/favicon-32x32.png
 werk24/assets/images/favicon-48x48.png
 werk24/assets/images/logo-625.png
 werk24/cli/__init__.py
 werk24/cli/auth.py
+werk24/cli/support.py
 werk24/cli/techread.py
 werk24/cli/utils.py
 werk24/cli/w24cli.py
 werk24/gui/__init__.py
 werk24/gui/event_feed.py
 werk24/gui/event_illustrator.py
 werk24/gui/gdt_table.py
@@ -48,14 +49,15 @@
 werk24/models/depth.py
 werk24/models/file_format.py
 werk24/models/fraction.py
 werk24/models/gdt.py
 werk24/models/gender.py
 werk24/models/general_tolerances.py
 werk24/models/geometric_shape.py
+werk24/models/helpdesk.py
 werk24/models/language.py
 werk24/models/leader.py
 werk24/models/location.py
 werk24/models/material.py
 werk24/models/measure.py
 werk24/models/note.py
 werk24/models/paper_size.py
```

