# Comparing `tmp/nicescad-0.0.3.tar.gz` & `tmp/nicescad-0.0.4.tar.gz`

## Comparing `nicescad-0.0.3.tar` & `nicescad-0.0.4.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.3/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.3/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.3/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/openscad.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/process.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/profiler.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/version.py
--rw-r--r--   0        0        0    16337 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/webserver.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.3/nicescad/web/static/css/pygments.css
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/intersection.scad
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openjscad_logo.stl
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/GEB.scad
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/advance_intersection.scad
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/animation.scad
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/demo_cut.scad
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/difference.scad
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/fractal.scad
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/intersecting.scad
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/iteration.scad
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/module_recursion.scad
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/offset.scad
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/search.scad
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Advanced/translation.scad
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/CSG-modules.scad
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/CSG.scad
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/LetterBlock.scad
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/children.scad
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/children_indexed.scad
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/difference_cube.scad
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/difference_sphere.scad
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/intersection.scad
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/linear_extrude.scad
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/logo.scad
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/logo_and_text.scad
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/projection.scad
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/rotate_extrude.scad
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/surface.scad
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/surface_image.scad
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/text_on_cube.scad
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/translate.scad
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Basics/union.scad
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/cut_view.scad
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/fan_view.scad
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/text.scad
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Functions/functions.scad
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Functions/recursion.scad
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/chopped_blocks.scad
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/fence.scad
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/flat_body.scad
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/polyhedron.scad
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/rounded_box.scad
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/sphere.scad
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.3/scad_examples/openscad_examples/Shapes/tripod.scad
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.3/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.3/scripts/install
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.3/scripts/openscad_example_scraper.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.3/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.3/tests/basetest.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 nicescad-0.0.3/tests/test_openscad.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nicescad-0.0.3/tests/test_webserver.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.3/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.3/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nicescad-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.4/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.4/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.4/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/openscad.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/process.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/profiler.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/version.py
+-rw-r--r--   0        0        0    18742 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/webserver.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/web/static/css/pygments.css
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/intersection.scad
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openjscad_logo.stl
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/GEB.scad
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/advance_intersection.scad
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/animation.scad
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/demo_cut.scad
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/difference.scad
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/fractal.scad
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/intersecting.scad
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/iteration.scad
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/module_recursion.scad
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/offset.scad
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/search.scad
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/translation.scad
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG-modules.scad
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG.scad
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/LetterBlock.scad
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/children.scad
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/children_indexed.scad
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_cube.scad
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_sphere.scad
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/intersection.scad
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/linear_extrude.scad
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo.scad
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo_and_text.scad
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/projection.scad
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/rotate_extrude.scad
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface.scad
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface_image.scad
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/text_on_cube.scad
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/translate.scad
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/union.scad
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/cut_view.scad
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/fan_view.scad
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/text.scad
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Functions/functions.scad
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Functions/recursion.scad
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/chopped_blocks.scad
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/fence.scad
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/flat_body.scad
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/polyhedron.scad
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/rounded_box.scad
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/sphere.scad
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/tripod.scad
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/install
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/openscad_example_scraper.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/basetest.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_openscad.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_subprocess.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_webserver.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.4/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nicescad-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.4/PKG-INFO
```

### Comparing `nicescad-0.0.3/.github/workflows/build.yml` & `nicescad-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.4/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/nicescad/local_filepicker.py` & `nicescad-0.0.4/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/nicescad/nicescad_cmd.py` & `nicescad-0.0.4/nicescad/nicescad_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     parser = ArgumentParser(description=description, formatter_class=RawDescriptionHelpFormatter)
     parser.add_argument("-a","--about",help="show about info [default: %(default)s]",action="store_true")
     parser.add_argument("-c","--client", action="store_true", help="start client [default: %(default)s]")
     parser.add_argument("-d", "--debug", dest="debug", action="store_true", help="show debug info [default: %(default)s]")
     parser.add_argument("-l", "--local", dest="local", action="store_true", help="run with local file system access [default: %(default)s]")
     parser.add_argument("-i", "--input", help="input file")
     parser.add_argument("-rp", "--root_path",default=WebServer.examples_path(),help="path to scad files [default: %(default)s]")
+    parser.add_argument("-rol","--render_on_load", action="store_true", help="render on load [default: %(default)s]")
 
     parser.add_argument("--host", default="localhost",
                             help="the host to serve / listen from [default: %(default)s]")
     parser.add_argument("--port",type=int,default=9858,help="the port to serve from [default: %(default)s]")
     parser.add_argument("-s","--serve", action="store_true", help="start webserver [default: %(default)s]")
     parser.add_argument("-V", "--version", action='version', version=version_msg)
     return parser
 
-
 def main(argv=None): 
     '''main program.'''
 
     if argv is None:
         argv=sys.argv[1:]
         
     program_name = Version.name
```

### Comparing `nicescad-0.0.3/nicescad/openscad.py` & `nicescad-0.0.4/nicescad/openscad.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Created on 2023-07-19
 
 @author: wf
 
 This module contains the class OpenScad, a wrapper for OpenScad.
 """
-
-from typing import Dict
+from typing import Awaitable
 import tempfile
 import os
 import platform
 from nicescad.process import Subprocess
 
-from pygments.lexer import RegexLexer, bygroups
-from pygments.token import *
+from pygments.lexer import RegexLexer
+from pygments.token import Comment,Keyword,Name,Number,Operator, Punctuation,String,Text
 from pygments import highlight
 from pygments.formatters.html import HtmlFormatter
 
 class OpenSCADLexer(RegexLexer):
     """
     Lexer for OpenSCAD, a language for creating solid 3D CAD models.
     
@@ -109,69 +108,60 @@
                 self._try_executable('/usr/local/bin/openscad')
         elif platfm == 'Darwin':
             self._try_executable('/Applications/OpenSCAD.app/Contents/MacOS/OpenSCAD')
         elif platfm == 'Windows':
             self._try_executable(os.path.join(os.environ.get('Programfiles(x86)', 'C:'), 'OpenSCAD\\openscad.exe'))
             self._try_executable(os.path.join(os.environ.get('Programfiles', 'C:'), 'OpenSCAD\\openscad.exe'))
 
-
-    def write_to_tmp_file(self, openscad_str: str):
+    def write_to_tmp_file(self, openscad_str: str, do_prepend: bool=True):
         """
-        Writes an OpenSCAD string to a temporary file.
-
+        Writes an OpenSCAD string to a temporary file. 
+    
+        The `scad_prepend` string is prepended to the OpenSCAD code before writing, 
+        unless the OpenSCAD code contains the string '//!OpenSCAD', or `do_prepend` 
+        is set to `False`. In these cases, only the OpenSCAD code is written to the file.
+    
         Args:
             openscad_str (str): The OpenSCAD code.
+            do_prepend (bool, optional): If `True`, the `scad_prepend` string is 
+                                          prepended to the OpenSCAD code. Defaults to `True`.
         
         Returns:
-            scad_tmp_file: The temporary file path.
+            str: The path to the temporary file where the OpenSCAD code (and 
+                 possibly the `scad_prepend` string) was written.
         """
         scad_tmp_file = os.path.join(self.tmp_dir, 'tmp.scad')
         with open(scad_tmp_file, 'w') as of:
-            of.write(self.scad_prepend)
+            if do_prepend and '//!OpenSCAD' not in openscad_str:
+                of.write(self.scad_prepend)
             of.write(openscad_str)
         return scad_tmp_file
 
-    async def render_to_file_async(self, openscad_str: str, fl_name: str) -> Subprocess:
+
+    async def render_to_file_async(self, openscad_str: str, stl_path: str) -> Awaitable[Subprocess]:
         """
         Asynchronously renders an OpenSCAD string to a file.
 
         Args:
             openscad_str (str): The OpenSCAD code.
-            fl_name (str): The name of the output file.
+            stl_path(str): The path to the output file.
         
-        Raises:
+        Returns:
             Subprocess: the openscad execution result
         """
         scad_tmp_file = self.write_to_tmp_file(openscad_str)
 
         # now run openscad to generate stl:
-        cmd = [self.openscad_exec, '-o', fl_name, scad_tmp_file]
+        cmd = [self.openscad_exec, '-o', stl_path, scad_tmp_file]
+        self.saved_umask = os.umask(0o077)
         result = await Subprocess.run_async(cmd)
+        os.umask(self.saved_umask)
 
         self.cleanup_tmp_file(result, scad_tmp_file)
-        return result
-
-    def render_to_file(self, openscad_str: str, fl_name: str) -> Subprocess:
-        """
-        Renders an OpenSCAD string to a file.
-
-        Args:
-            openscad_str (str): The OpenSCAD code.
-            fl_name (str): The name of the output file.
-        
-        Raises:
-            Subprocess: the openscad execution result
-        """
-        scad_tmp_file = self.write_to_tmp_file(openscad_str)
-
-        # now run openscad to generate stl:
-        cmd = [self.openscad_exec, '-o', fl_name, scad_tmp_file]
-        result = Subprocess.run(cmd)
-
-        self.cleanup_tmp_file(result, scad_tmp_file)
+        result.stl_path=stl_path
         return result
 
     def cleanup_tmp_file(self, result, scad_tmp_file):
         """
         Cleanup temporary files after subprocess execution.
 
         Args:
@@ -180,58 +170,20 @@
         """
         if result.returncode == 0:
             if os.path.isfile(scad_tmp_file):
                 os.remove(scad_tmp_file)
         else:
             result.scad_tmp_file = scad_tmp_file
 
-    async def openscad_str_to_file_async(self, openscad_str: str, **kwargs) -> Subprocess:
-        """
-        Asynchronously renders the OpenSCAD code to a file.
-    
-        Args:
-            openscad_str (str): The OpenSCAD code.
-            **kwargs: Additional arguments, could include 'outfile' to specify the output file name.
-    
-        Returns:
-            Subprocess: The result of the subprocess run, encapsulated in a Subprocess object.
-        """
-        return await self.render_cleanup_wrapper(self.render_to_file_async, openscad_str, **kwargs)
-
-    def openscad_str_to_file(self, openscad_str: str, **kwargs) -> Subprocess:
+    async def openscad_str_to_file(self, openscad_str: str, stl_path:str) -> Subprocess:
         """
         Renders the OpenSCAD code to a file.
     
         Args:
             openscad_str (str): The OpenSCAD code.
-            **kwargs: Additional arguments, could include 'outfile' to specify the output file name.
+            stl_path(str): the path to the stl file
     
         Returns:
             Subprocess: The result of the subprocess run, encapsulated in a Subprocess object.
         """
-        return self.render_cleanup_wrapper(self.render_to_file, openscad_str, **kwargs)
-
-    def render_cleanup_wrapper(self, render_func, openscad_str: str, **kwargs):
-        """
-        Wrapper function to perform rendering and cleanup tasks.
-
-        Args:
-            render_func (function): The rendering function to use (either synchronous or asynchronous).
-            openscad_str (str): The OpenSCAD code.
-            **kwargs: Additional arguments, could include 'outfile' to specify the output file name.
-
-        Returns:
-            result: The result of the rendering function.
-        """
-        self.saved_umask = os.umask(0o077)
-        try:
-            if 'outfile' in kwargs:
-                openscad_out_file = kwargs['outfile']
-            else:
-                openscad_out_file = os.path.join(self.tmp_dir, 'tmp.stl')                    
-
-            result = render_func(openscad_str, openscad_out_file, **kwargs)
-
-            return result
-        finally:
-            os.umask(self.saved_umask)
-
+        result=await self.render_to_file_async(openscad_str, stl_path)
+        return result
```

### Comparing `nicescad-0.0.3/nicescad/process.py` & `nicescad-0.0.4/nicescad/process.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 import asyncio
 import subprocess
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Awaitable
 
 @dataclass
 class Subprocess:
     """A class representing a subprocess execution result."""
 
     stdout: str
     stderr: str
     cmd: List[str]
     returncode: int
     exception: Optional[BaseException] = None
 
     @staticmethod
-    async def run_async(cmd: List[str]):
+    async def run_async(cmd: List[str])->Awaitable["Subprocess"]:
         """
         Asynchronously runs a command as a subprocess and returns the result as an instance of this class.
         
         Args:
             cmd (List[str]): The command to run.
 
         Returns:
             Subprocess: An instance of this class representing the result of the subprocess execution.
         """
-        proc = await asyncio.create_subprocess_exec(
-            *cmd,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE
-        )
-        
-        stdout, stderr = await proc.communicate()
-
-        return Subprocess(
-            stdout=stdout.decode(), 
-            stderr=stderr.decode(), 
-            cmd=cmd, 
-            returncode=proc.returncode
-        )
+        try:
+            proc = await asyncio.create_subprocess_exec(
+                *cmd,
+                stdout=asyncio.subprocess.PIPE,
+                stderr=asyncio.subprocess.PIPE
+            )
+            
+            stdout, stderr = await proc.communicate()
+    
+            subprocess=Subprocess(
+                stdout=stdout.decode(), 
+                stderr=stderr.decode(), 
+                cmd=cmd, 
+                returncode=proc.returncode
+            )
+        except BaseException as ex:
+            subprocess=Subprocess(stdout='', stderr=str(ex), cmd=cmd, returncode=-1, exception=ex)
+        return subprocess    
 
     @staticmethod
-    def run(cmd: List[str]):
+    def run(cmd: List[str])->"Subprocess":
         """
         Runs a command as a subprocess and returns the result as an instance of this class.
         
         Args:
             cmd (List[str]): The command to run.
 
         Returns:
             Subprocess: An instance of this class representing the result of the subprocess execution.
         """
-        try:
-            proc = subprocess.run(cmd, capture_output=True, text=True)
-            return Subprocess(stdout=proc.stdout, stderr=proc.stderr, cmd=cmd, returncode=proc.returncode)
-        except subprocess.CalledProcessError as cpe:
-            return Subprocess(stdout=cpe.stdout, stderr=cpe.stderr, cmd=cmd, returncode=cpe.returncode, exception=cpe)
-        except Exception as e:
-            return Subprocess(stdout='', stderr=str(e), cmd=cmd, returncode=-1, exception=e)
+        subprocess=asyncio.run(Subprocess.run_async(cmd))
+        return subprocess
```

### Comparing `nicescad-0.0.3/nicescad/profiler.py` & `nicescad-0.0.4/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/nicescad/version.py` & `nicescad-0.0.4/nicescad/version.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/nicescad/webserver.py` & `nicescad-0.0.4/nicescad/webserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 """
 from typing import Dict, Optional, Union,List, Callable
 from nicescad.version import Version
 from nicescad.openscad import OpenScad
 from nicescad.local_filepicker import LocalFilePicker
 from nicegui import ui, app
 from pathlib import Path
+import inspect
 import os
 import sys
 import requests
 import traceback
-from nicegui.events import ValueChangeEventArguments
+from nicegui.events import ValueChangeEventArguments, ColorPickEventArguments
 
 class FileSelector():
     """
     example handling
     """
     def __init__(self,path:str,extension: str,handler:Callable=None):
         """
@@ -56,29 +57,31 @@
         
         for child in tree.get('children', []):
             found = self.file_by_id(child, id_to_find)
             if found:
                 return found
                 
         return None
-
     
-    def select_file(self,vcea:ValueChangeEventArguments):
+    async def select_file(self,vcea:ValueChangeEventArguments):
         """
         select the given file and call my handler on the file path of it
         
         Args:
             vcea(ValueChangeEventArguments): the tree selection event
         """
         id_to_find = vcea.value  # Assuming vcea.value contains the id
         file_path=self.file_by_id(self.tree_structure, id_to_find)
         if file_path is None:
             raise ValueError(f"No item with id {id_to_find} found in the tree structure.")
         if self.handler:
-            self.handler(file_path) 
+            if inspect.iscoroutinefunction(self.handler):
+                await self.handler(file_path)
+            else:
+                self.handler(file_path) 
 
     def get_dir_tree(self, path: str, extension: str, id_path: List[int]=[1], file_counter: int = 1) -> Optional[Dict[str, dict]]:
         """
         Recursive function to construct a directory tree.
     
         Args:
             path (str): The path to the directory to start building the tree from.
@@ -128,34 +131,37 @@
     Attributes:
         oscad (OpenScad): An OpenScad object that aids in performing OpenScad operations.
     """
 
     def __init__(self):
         """Constructs all the necessary attributes for the WebServer object."""
         self.oscad = OpenScad(scad_prepend="""//https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Other_Language_Features#$fa,_$fs_and_$fn
-// default number o facets for arc generation
-$fn=30;""")
+// default number of facets for arc generation
+$fn=30;
+""")
         self.code="""// nicescad example
 module example() {
   translate([0,0,15]) {
      cube(30,center=true);
      sphere(20);
   }
 }
 example();"""        
         self.input="example.scad"
+        self.stl_name="result.stl"
+        self.stl_object=None
         self.is_local=False
         app.add_static_files('/stl', self.oscad.tmp_dir)
         self.log_view=None
         self.do_trace=True
         self.html_view=None
  
         @ui.page('/')
-        def home():
-            self.home()
+        async def home():
+            await self.home()
             
         @ui.page('/settings')
         def settings():
             self.settings()
             
             
     @classmethod
@@ -176,35 +182,38 @@
             self.error_msg = str(e) + "\n" + traceback.format_exc()
         else:
             self.error_msg = str(e)
         if self.log_view:
             self.log_view.push(self.error_msg)
         print(self.error_msg,file=sys.stderr)
 
-    
-        
-    async def render(self, _click_args):
+    async def render(self, _click_args=None):
         """Renders the OpenScad string and updates the 3D scene with the result.
 
         Args:
             click_args (object): The click event arguments.
         """
         try:
             self.progress_view.visible = True
             ui.notify("rendering ...")
             with self.scene:
                 self.scene.clear()
+                self.stl_link.visible=False
+                self.color_picker_button.disable()
             openscad_str = self.code_area.value
-            render_result= await self.oscad.openscad_str_to_file_async(openscad_str)
+            stl_path=stl_path = os.path.join(self.oscad.tmp_dir, self.stl_name) 
+            render_result= await self.oscad.openscad_str_to_file(openscad_str,stl_path)
             # show render result in log
             self.log_view.push(render_result.stderr)
             if render_result.returncode==0:
                 ui.notify("stl created ... loading into scene")
+                self.stl_link.visible=True
+                self.color_picker_button.enable()
                 with self.scene:
-                    self.scene.stl("/stl/tmp.stl").move(x=0.0).scale(0.1)    
+                    self.stl_object=self.scene.stl(f"/stl/{self.stl_name}").move(x=0.0).scale(0.1)    
         except BaseException as ex:
             self.handle_exception(ex,self.do_trace)  
         self.progress_view.visible=False  
             
     def do_read_input(self, input_str: str):
         """Reads the given input.
 
@@ -220,27 +229,38 @@
         else:
             if os.path.exists(input_str):
                 with open(input_str, 'r') as file:
                     return file.read()
             else:
                 raise Exception(f'File does not exist: {input_str}')
     
-    def read_input(self, input: str):
+    async def read_and_optionally_render(self,input_str):
+        """Reads the given input and optionally renders the given input
+
+        Args:
+            input_str (str): The input string representing a URL or local file.
+        """
+        self.read_input(input_str)
+        if self.render_on_load:
+            await self.render(None)
+        
+    def read_input(self, input_str: str):
         """Reads the given input and handles any exceptions.
 
         Args:
-            input (str): The input string representing a URL or local file.
+            input_str (str): The input string representing a URL or local file.
         """
         try:
-            ui.notify(f"reading {input}")
-            self.code = self.do_read_input(input)
-            self.input_input.set_value(input)
+            ui.notify(f"reading {input_str}")
+            self.code = self.do_read_input(input_str)
+            self.input_input.set_value(input_str)
             self.code_area.set_value(self.code)
             self.log_view.clear()
             self.error_msg = None
+            self.stl_link.visible=False
         except BaseException as e:
             self.code = None
             self.handle_exception(e, self.do_trace)
             
     def save_file(self):
         """Saves the current code to the last input file, if it was a local path."""
         if self.is_local and self.input:
@@ -252,16 +272,15 @@
     
     async def open_file(self) -> None:
         """Opens a Local filer picker dialog and reads the selected input file."""
         if self.is_local:
             pick_list = await LocalFilePicker('~', multiple=False)
             if len(pick_list)>0:
                 input_file=pick_list[0]
-                ui.notify(f'Opening {input_file}')
-                self.read_input(input_file)
+                await self.read_and_optionally_render(input_file)
     pass
 
     async def reload_file(self):
         """
         reload the input file
         """
         allowed_urls=[
@@ -272,16 +291,15 @@
             allowed=False
             for allowed_url in allowed_urls:
                 if self.input.startswith(allowed_url):
                     allowed=True
         if not allowed:
             ui.notify("only white listed URLs are allowed")
         else:    
-            ui.notify(f"reloading {self.input} ...")
-            self.read_input(self.input)
+            await self.read_and_optionally_render(self.input)
             
     def select_example(self,ts):
         """
         """
         pass
     
     def link_button(self, name: str, target: str, icon_name: str):
@@ -370,58 +388,85 @@
                 self.html_view.visible=True
             else:
                 self.html_view.visible=False
                 self.code_area.visible=True
         except BaseException as ex:
             self.handle_exception(ex, self.do_trace)
         
-    def home(self):
+    async def pick_color(self,e:ColorPickEventArguments):
+        """
+        Asynchronously picks a color based on provided event arguments.
+    
+        This function changes the color of the 'color_picker_button' and the 'stl_object'
+        according to the color specified in the event arguments.
+    
+        Args:
+            e (ColorPickEventArguments): An object containing event-specific arguments.
+                The 'color' attribute of this object specifies the color to be applied.
+    
+        Note:
+            If 'stl_object' is None, the function will only change the color of 'color_picker_button'.
+            Otherwise, it changes the color of both 'color_picker_button' and 'stl_object'.
+        """
+        self.color_picker_button.style(f'background-color:{e.color}!important')
+        if self.stl_object:
+            self.stl_object.material(f'{e.color}')
+        pass
+        
+    async def home(self):
         """Generates the home page with a 3D viewer and a code editor."""
         self.setup_pygments()
         self.setup_menu()
         with ui.column():
             with ui.splitter() as splitter:
                 with splitter.before:
+                    self.color_picker = ui.color_picker(on_pick=self.pick_color)
+                    self.color_picker_button=ui.button(on_click=self.color_picker.open, icon='colorize')      
+                    self.color_picker_button.disable()
                     with ui.scene(width=1024, height=768).classes("w-full") as scene:
                         self.scene = scene
                         scene.spot_light(distance=100, intensity=0.2).move(-10, 0, 10)
                     with splitter.after:
                         with ui.element("div").classes("w-full"):
-                            self.example_selector=FileSelector(path=self.root_path,extension=".scad",handler=self.read_input)
+                            self.example_selector=FileSelector(path=self.root_path,extension=".scad",handler=self.read_and_optionally_render)
                             self.input_input=ui.input(
                                 value=self.input,
                                 on_change=self.input_changed).props("size=100")
-                            self.tool_button(name="highlight", icon="colorize", handler=self.highlight_code)    
+                            self.tool_button(name="highlight", icon="html", handler=self.highlight_code)    
                             if self.is_local:
                                 self.tool_button(name="save",icon="save",handler=self.save_file)
                             self.tool_button(name="reload",icon="refresh",handler=self.reload_file)
                             if self.is_local:
                                 self.tool_button(name="open",icon="file_open",handler=self.open_file)
                             self.tool_button(name="render",icon="play_circle",handler=self.render)
+                            self.stl_link=ui.link("stl result",f"/stl/{self.stl_name}",new_tab=True)
+                            self.stl_link.visible=False
                             self.progress_view = ui.spinner('dots', size='lg', color='blue')
                             self.progress_view.visible = False
                             self.code_area = ui.textarea(value=self.code,on_change=self.code_changed).props('clearable').props("rows=25")
                             self.html_view = ui.html()
                             self.html_view.visible=False
                             self.log_view = ui.log(max_lines=20).classes('w-full h-40')        
         self.setup_footer()        
         if self.args.input:
-            self.read_input(self.args.input)
+            await self.read_and_optionally_render(self.args.input)
         
     def settings(self):
         """Generates the settings page with a link to the project's GitHub page."""
         self.setup_menu()
-        v = ui.checkbox('debug with trace', value=True)
+        ui.checkbox('debug with trace', value=True).bind_value(self, "do_trace")
+        ui.checkbox('render on load',value=self.render_on_load).bind_value(self,"render_on_load")
         sp_input=ui.textarea("scad prepend",value=self.oscad.scad_prepend).props("cols=80")
         sp_input.bind_value(self.oscad,"scad_prepend")
         self.setup_footer()
        
     def run(self, args):
         """Runs the UI of the web server.
 
         Args:
             args (list): The command line arguments.
         """
         self.args=args
         self.is_local=args.local
         self.root_path=args.root_path 
+        self.render_on_load=args.render_on_load
         ui.run(title=Version.name, host=args.host, port=args.port, show=args.client,reload=False)
```

### Comparing `nicescad-0.0.3/nicescad/web/static/css/pygments.css` & `nicescad-0.0.4/nicescad/web/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/intersection.scad` & `nicescad-0.0.4/scad_examples/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openjscad_logo.stl` & `nicescad-0.0.4/scad_examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/GEB.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/GEB.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/advance_intersection.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/advance_intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/animation.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/animation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/demo_cut.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/demo_cut.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/difference.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/difference.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/fractal.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/fractal.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/intersecting.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/intersecting.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/iteration.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/iteration.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/module_recursion.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/module_recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/offset.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/offset.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/search.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/search.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Advanced/translation.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/translation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/CSG-modules.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG-modules.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/CSG.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/LetterBlock.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/LetterBlock.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/children.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/children.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/children_indexed.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/children_indexed.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/difference_cube.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/difference_sphere.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/intersection.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/linear_extrude.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/linear_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/logo.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/logo_and_text.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo_and_text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/projection.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/projection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/rotate_extrude.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/rotate_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/surface.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/surface_image.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface_image.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/text_on_cube.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/text_on_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/translate.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/translate.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Basics/union.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Basics/union.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/cut_view.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/cut_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/fan_view.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/fan_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Extrusion/text.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Functions/functions.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Functions/functions.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Functions/recursion.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Functions/recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/chopped_blocks.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/chopped_blocks.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/fence.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/fence.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/flat_body.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/flat_body.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/polyhedron.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/polyhedron.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/rounded_box.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/rounded_box.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/sphere.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scad_examples/openscad_examples/Shapes/tripod.scad` & `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/tripod.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scripts/doc` & `nicescad-0.0.4/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/scripts/openscad_example_scraper.py` & `nicescad-0.0.4/scripts/openscad_example_scraper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/tests/basetest.py` & `nicescad-0.0.4/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/tests/test_openscad.py` & `nicescad-0.0.4/tests/test_openscad.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 '''
 Created on 2023-07-19
 
 @author: wf
 '''
+import asyncio
+import os
 from tests.basetest import Basetest
 from nicescad.openscad import OpenScad
 
 class TestOpenScad(Basetest):
     """
     test openscad wrapper
     """
@@ -21,16 +23,23 @@
     def testRender(self):
         """
         test rendering a scad file
         """
         # openscad_exec="/Users/wf/bin/openscad"
         oscad=OpenScad()
         openscad_str="cube(5);"
-        stl=oscad.openscad_str_to_file(openscad_str)
-        print(stl)
+        stl_path = os.path.join(oscad.tmp_dir, 'cube5.stl') 
+        subprocess=asyncio.run(oscad.openscad_str_to_file(openscad_str,stl_path))
+        debug=self.debug
+        #debug=True
+        if debug:
+            print(subprocess)
+        self.assertEqual(0,subprocess.returncode)
+        self.assertEqual(stl_path,subprocess.stl_path)
+        self.assertTrue(os.path.isfile(stl_path))
         pass
     
     def test_highlight_code(self):
         """
         Tests the 'highlight_code' function by checking if the output starts with 
         the standard beginning of an HTML string outputted by Pygments.
         
@@ -44,10 +53,8 @@
         """
         oscad=OpenScad()
         test_code = 'module test() { echo("Hello, world!"); }'
         highlighted_code = oscad. highlight_code(test_code)
         debug=self.debug
         if debug:
             print(highlighted_code)
-        self.assertTrue(highlighted_code.startswith('<div'))
-
-        
+        self.assertTrue(highlighted_code.startswith('<div'))
```

### Comparing `nicescad-0.0.3/tests/test_webserver.py` & `nicescad-0.0.4/tests/test_webserver.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/.gitignore` & `nicescad-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/LICENSE` & `nicescad-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/README.md` & `nicescad-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/pyproject.toml` & `nicescad-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.3/PKG-INFO` & `nicescad-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

