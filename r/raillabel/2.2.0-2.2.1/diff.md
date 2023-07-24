# Comparing `tmp/raillabel-2.2.0.tar.gz` & `tmp/raillabel-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raillabel-2.2.0.tar", last modified: Tue Jun  6 10:55:49 2023, max compression
+gzip compressed data, was "raillabel-2.2.1.tar", last modified: Mon Jul 24 11:57:09 2023, max compression
```

## Comparing `raillabel-2.2.0.tar` & `raillabel-2.2.1.tar`

### file list

```diff
@@ -1,210 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-06 10:55:31.000000 raillabel-2.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 10:55:31.000000 raillabel-2.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.810411 raillabel-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/build-test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-06 10:55:31.000000 raillabel-2.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-06 10:55:31.000000 raillabel-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-06 10:55:31.000000 raillabel-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-06 10:55:31.000000 raillabel-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-06 10:55:31.000000 raillabel-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/.license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-06 10:55:31.000000 raillabel-2.2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 10:55:49.838411 raillabel-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 10:55:31.000000 raillabel-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.814411 raillabel-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/_static/github-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howto.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/docs/source/howtos/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/1 Validating Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/2 Loading Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/3 Saving Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/howtos/4 Filtering Scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-06 10:55:31.000000 raillabel-2.2.0/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 10:55:31.000000 raillabel-2.2.0/git-conventional-commits.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/git-conventional-commits.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-06 10:55:31.000000 raillabel-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel/_filter_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_end.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_object_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_object_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_filter_classes/_filter_start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.822411 raillabel-2.2.0/raillabel/_understand_ai_t4_format/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/point_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/polygon_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/polyline_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/sensor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_understand_ai_t4_format/size_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.822411 raillabel-2.2.0/raillabel/_util/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/_util/_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/frame_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/intrinsics_pinhole.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/intrinsics_radar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/object_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/point3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/poly2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/poly3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/seg3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/sensor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/size2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/size3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/_loader_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/loader_raillabel_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/loader_understand_ai_t4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/translation.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/format_loaders/translation.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    41712 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/understand_ai_t4_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/schemas/understand_ai_t4_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-06 10:55:31.000000 raillabel-2.2.0/raillabel/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.818411 raillabel-2.2.0/raillabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 10:55:49.000000 raillabel-2.2.0/raillabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:55:49.838411 raillabel-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/master_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.826411 raillabel-2.2.0/tests/test_raillabel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.830411 raillabel-2.2.0/tests/test_raillabel/__test_assets__/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60789 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
--rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   295329 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_real_life.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_real_life.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_point_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polygon_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polyline_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_sensor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_size_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format/test_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_understand_ai_t4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:55:49.838411 raillabel-2.2.0/tests/test_raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/schemas/test_understand_ai_t4_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-06 10:55:31.000000 raillabel-2.2.0/tests/test_raillabel/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.806321 raillabel-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 11:56:49.000000 raillabel-2.2.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-24 11:56:49.000000 raillabel-2.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.774320 raillabel-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 11:56:49.000000 raillabel-2.2.1/.github/workflows/build-test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 11:56:49.000000 raillabel-2.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-24 11:56:49.000000 raillabel-2.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-24 11:56:49.000000 raillabel-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-24 11:56:49.000000 raillabel-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-24 11:56:49.000000 raillabel-2.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-24 11:56:49.000000 raillabel-2.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 11:56:49.000000 raillabel-2.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 11:56:49.000000 raillabel-2.2.1/LICENSES/.license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 11:56:49.000000 raillabel-2.2.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-24 11:56:49.000000 raillabel-2.2.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-24 11:57:09.806321 raillabel-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-24 11:56:49.000000 raillabel-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/_static/github-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/howto.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.782320 raillabel-2.2.1/docs/source/howtos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/howtos/1 Validating Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/howtos/2 Loading Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/howtos/3 Saving Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/howtos/4 Filtering Scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-24 11:56:49.000000 raillabel-2.2.1/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 11:56:49.000000 raillabel-2.2.1/git-conventional-commits.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/git-conventional-commits.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-24 11:56:49.000000 raillabel-2.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.786321 raillabel-2.2.1/raillabel/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.786321 raillabel-2.2.1/raillabel/_filter_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_annotation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_object_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_object_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_filter_classes/_filter_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.790320 raillabel-2.2.1/raillabel/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/bounding_box_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/bounding_box_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/point_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/polygon_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/polyline_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_understand_ai_t4_format/size_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.790320 raillabel-2.2.1/raillabel/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/_util/_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.794320 raillabel-2.2.1/raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/frame_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/intrinsics_pinhole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/intrinsics_radar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/object_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/point3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/poly2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/poly3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/seg3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/size2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/size3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.794320 raillabel-2.2.1/raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/_loader_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/loader_raillabel_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/loader_understand_ai_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/translation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/format_loaders/translation.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.794320 raillabel-2.2.1/raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    41712 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/schemas/raillabel_v2_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/schemas/raillabel_v2_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/schemas/understand_ai_t4_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/schemas/understand_ai_t4_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-24 11:56:49.000000 raillabel-2.2.1/raillabel/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.786321 raillabel-2.2.1/raillabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 11:57:09.000000 raillabel-2.2.1/raillabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:57:09.806321 raillabel-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.794320 raillabel-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.794320 raillabel-2.2.1/tests/test_raillabel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.798321 raillabel-2.2.1/tests/test_raillabel/__test_assets__/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.802321 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_cs_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar_stream_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/metadata_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/segmentation_3d_raillabel.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_camera.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/sensor_reference_lidar.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/metaschema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/metaschema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60789 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
+-rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   295329 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_real_life.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_real_life.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.806321 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_point_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_polygon_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_polyline_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_size_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.806321 raillabel-2.2.1/tests/test_raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/format/test_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.806321 raillabel-2.2.1/tests/test_raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/format_loaders/test_loader_understand_ai_t4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:09.806321 raillabel-2.2.1/tests/test_raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/schemas/test_understand_ai_t4_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-24 11:56:49.000000 raillabel-2.2.1/tests/test_raillabel/test_validate.py
```

### Comparing `raillabel-2.2.0/.github/workflows/build-test-publish.yml` & `raillabel-2.2.1/.github/workflows/build-test-publish.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/.github/workflows/docs.yml` & `raillabel-2.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/.github/workflows/lint.yml` & `raillabel-2.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/.gitignore` & `raillabel-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/.pre-commit-config.yaml` & `raillabel-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/CHANGELOG.md` & `raillabel-2.2.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,7 +49,11 @@
 ## 2.1.0
 - Added IntrinsicsRadar to the devkit and the json-schema
 
 ## 2.2.0
 - Raillabel schema is now more restrictive regarding intrinsic calibration
 - Support for understand.ai t4 format
 - Renaming of raillabel.format.Frame.data to frame_data
+
+### 2.2.1
+- Fixed bug, that prevented loading a understand ai file via raillabel.load()
+- Made the project_id field in the understand ai files less restrictive
```

### Comparing `raillabel-2.2.0/CONTRIBUTING.md` & `raillabel-2.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/LICENSE` & `raillabel-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/LICENSES/Apache-2.0.txt` & `raillabel-2.2.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/LICENSES/CC0-1.0.txt` & `raillabel-2.2.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/PKG-INFO` & `raillabel-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.2.0
+Version: 2.2.1
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.2.0/README.md` & `raillabel-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/Makefile` & `raillabel-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/make.bat` & `raillabel-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/_static/github-logo.svg` & `raillabel-2.2.1/docs/source/_static/github-logo.svg`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/conf.py` & `raillabel-2.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/howtos/1 Validating Annotation Files.rst` & `raillabel-2.2.1/docs/source/howtos/1 Validating Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/howtos/2 Loading Annotation Files.rst` & `raillabel-2.2.1/docs/source/howtos/2 Loading Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/howtos/3 Saving Annotation Files.rst` & `raillabel-2.2.1/docs/source/howtos/3 Saving Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/howtos/4 Filtering Scenes.rst` & `raillabel-2.2.1/docs/source/howtos/4 Filtering Scenes.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/index.rst` & `raillabel-2.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/docs/source/intro.rst` & `raillabel-2.2.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/pyproject.toml` & `raillabel-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/__init__.py` & `raillabel-2.2.1/raillabel/_filter_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_abc.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_abc.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_ids.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_annotation_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_annotation_types.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_annotation_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_attributes.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_attributes.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_end.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_end.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_frames.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_frames.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_object_ids.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_object_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_object_types.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_object_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_sensors.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_sensors.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_filter_classes/_filter_start.py` & `raillabel-2.2.1/raillabel/_filter_classes/_filter_start.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/__init__.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/_annotation.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/_translation.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/_translation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_2d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/bounding_box_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/bounding_box_3d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/bounding_box_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/coordinate_system.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/frame.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/frame.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/metadata.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/metadata.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/point_3d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/point_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/polygon_2d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/polygon_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/polyline_2d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/polyline_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/quaternion.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/quaternion.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/scene.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/scene.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/segmentation_3d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/sensor_reference.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/sensor_reference.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/_understand_ai_t4_format/size_3d.py` & `raillabel-2.2.1/raillabel/_understand_ai_t4_format/size_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/exceptions.py` & `raillabel-2.2.1/raillabel/exceptions.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/filter.py` & `raillabel-2.2.1/raillabel/filter.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/__init__.py` & `raillabel-2.2.1/raillabel/format/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/_annotation.py` & `raillabel-2.2.1/raillabel/format/_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/bbox.py` & `raillabel-2.2.1/raillabel/format/bbox.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/cuboid.py` & `raillabel-2.2.1/raillabel/format/cuboid.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/frame.py` & `raillabel-2.2.1/raillabel/format/frame.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/frame_interval.py` & `raillabel-2.2.1/raillabel/format/frame_interval.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/intrinsics_pinhole.py` & `raillabel-2.2.1/raillabel/format/intrinsics_pinhole.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/intrinsics_radar.py` & `raillabel-2.2.1/raillabel/format/intrinsics_radar.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/metadata.py` & `raillabel-2.2.1/raillabel/format/metadata.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/num.py` & `raillabel-2.2.1/raillabel/format/num.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/object.py` & `raillabel-2.2.1/raillabel/format/object.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/object_data.py` & `raillabel-2.2.1/raillabel/format/object_data.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/point2d.py` & `raillabel-2.2.1/raillabel/format/point2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/point3d.py` & `raillabel-2.2.1/raillabel/format/point3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/poly2d.py` & `raillabel-2.2.1/raillabel/format/poly2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/poly3d.py` & `raillabel-2.2.1/raillabel/format/poly3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/quaternion.py` & `raillabel-2.2.1/raillabel/format/quaternion.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/scene.py` & `raillabel-2.2.1/raillabel/format/scene.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/seg3d.py` & `raillabel-2.2.1/raillabel/format/seg3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/sensor.py` & `raillabel-2.2.1/raillabel/format/sensor.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/sensor_reference.py` & `raillabel-2.2.1/raillabel/format/sensor_reference.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format/transform.py` & `raillabel-2.2.1/raillabel/format/transform.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format_loaders/__init__.py` & `raillabel-2.2.1/raillabel/format_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format_loaders/_loader_abc.py` & `raillabel-2.2.1/raillabel/format_loaders/_loader_abc.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/format_loaders/loader_raillabel_v2.py` & `raillabel-2.2.1/raillabel/format_loaders/loader_raillabel_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,17 @@
 
         Returns
         -------
         bool:
             If True, the Loader class is suitable for the data.
         """
 
+        if "openlabel" not in data or "metadata" not in data["openlabel"]:
+            return False
+
         if "subschema_version" in data["openlabel"]["metadata"]:
             return (
                 "openlabel" in data
                 and "metadata" in data["openlabel"]
                 and "schema_version" in data["openlabel"]["metadata"]
                 and data["openlabel"]["metadata"]["subschema_version"].startswith("2.")
             )
```

### Comparing `raillabel-2.2.0/raillabel/format_loaders/loader_understand_ai_t4.py` & `raillabel-2.2.1/raillabel/format_loaders/loader_understand_ai_t4.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
         Returns
         -------
         scene: raillabel._understand_ai_t4_format.UAIScene
             The loaded scene with the data.
         """
 
+        self.warnings = []
+
         if validate:
             self.validate(data)
 
         data_converted_to_raillabel = uai_format.Scene.fromdict(data).to_raillabel()
 
         raillabel_scene = LoaderRailLabelV2().load(data_converted_to_raillabel, validate=False)
 
@@ -65,11 +67,10 @@
         bool:
             If True, the Loader class is suitable for the data.
         """
 
         return (
             "metadata" in data
             and "project_id" in data["metadata"]
-            and data["metadata"]["project_id"] == "trains_4"
             and "coordinateSystems" in data
             and "frames" in data
         )
```

### Comparing `raillabel-2.2.0/raillabel/format_loaders/translation.json` & `raillabel-2.2.1/raillabel/format_loaders/translation.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/load.py` & `raillabel-2.2.1/raillabel/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Parameters
     ----------
     path: str
         Path to the annotation file.
     validate: bool, optional
         If True, the annotation data is validated via the respective schema. This is highly
-        recommended, as not validating the data may lead to Errors during loading or while handling
+        recommended, as not validating the data may lead to errors during loading or while handling
         the scene. However, validating may increase the loading time. Default is False.
     show_warnings: bool, optional
         If True, any non-critical inconsistencies in the data are output as a warning. Default is
         True.
 
     Returns
     -------
```

### Comparing `raillabel-2.2.0/raillabel/save.py` & `raillabel-2.2.1/raillabel/save.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/schemas/raillabel_v2_schema.json` & `raillabel-2.2.1/raillabel/schemas/raillabel_v2_schema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/schemas/understand_ai_t4_schema.json` & `raillabel-2.2.1/raillabel/schemas/understand_ai_t4_schema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel/validate.py` & `raillabel-2.2.1/raillabel/validate.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/raillabel.egg-info/PKG-INFO` & `raillabel-2.2.1/raillabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.2.0
+Version: 2.2.1
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.2.0/raillabel.egg-info/SOURCES.txt` & `raillabel-2.2.1/raillabel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 raillabel/schemas/raillabel_v2_schema.json
 raillabel/schemas/raillabel_v2_schema.json.license
 raillabel/schemas/understand_ai_t4_schema.json
 raillabel/schemas/understand_ai_t4_schema.json.license
 tests/conftest.py
 tests/master_test.py
 tests/test_raillabel/test_filter.py
+tests/test_raillabel/test_load.py
 tests/test_raillabel/test_save.py
 tests/test_raillabel/test_validate.py
 tests/test_raillabel/__test_assets__/metaschema.json
 tests/test_raillabel/__test_assets__/metaschema.json.license
 tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
 tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
 tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
```

### Comparing `raillabel-2.2.0/tests/conftest.py` & `raillabel-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_2d_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/bounding_box_3d_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_camera_stream_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_lidar.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/coordinate_system_radar.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/frame_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polygon_2d_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/_understand_ai_t4_format/polyline_2d_raillabel.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/metaschema.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/metaschema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_real_life.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_real_life.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json` & `raillabel-2.2.1/tests/test_raillabel/__test_assets__/understand_ai_t4_short.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_2d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_3d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_bounding_box_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_coordinate_system.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_frame.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_frame.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_metadata.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_metadata.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_point_3d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_point_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polygon_2d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_polygon_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_polyline_2d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_polyline_2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_quaternion.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_scene.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_scene.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_segmentation_3d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_sensor_reference.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_sensor_reference.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/_understand_ai_t4_format/test_size_3d.py` & `raillabel-2.2.1/tests/test_raillabel/_understand_ai_t4_format/test_size_3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/format/test_annotation.py` & `raillabel-2.2.1/tests/test_raillabel/format/test_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py` & `raillabel-2.2.1/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/format_loaders/test_loader_understand_ai_t4.py` & `raillabel-2.2.1/tests/test_raillabel/format_loaders/test_loader_understand_ai_t4.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def test_supports_true(json_data, loader):
     assert loader.supports(json_data["understand_ai_real_life"])
 
 
 def test_supports_false(json_data, loader):
     data = json_data["understand_ai_real_life"]
-    data["metadata"]["project_id"] = "invalid"
+    del data["metadata"]["project_id"]
     assert not loader.supports(data)
 
 
 def test_load(json_data, loader):
     input_data_raillabel = remove_non_parsed_fields(json_data["openlabel_v1_short"])
     input_data_uai = json_data["understand_ai_t4_short"]
```

### Comparing `raillabel-2.2.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py` & `raillabel-2.2.1/tests/test_raillabel/schemas/test_raillabel_v2_schema.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/schemas/test_understand_ai_t4_schema.py` & `raillabel-2.2.1/tests/test_raillabel/schemas/test_understand_ai_t4_schema.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/test_filter.py` & `raillabel-2.2.1/tests/test_raillabel/test_filter.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/test_save.py` & `raillabel-2.2.1/tests/test_raillabel/test_save.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.2.0/tests/test_raillabel/test_validate.py` & `raillabel-2.2.1/tests/test_raillabel/test_validate.py`

 * *Files identical despite different names*

