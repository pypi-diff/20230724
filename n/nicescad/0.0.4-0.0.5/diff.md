# Comparing `tmp/nicescad-0.0.4.tar.gz` & `tmp/nicescad-0.0.5.tar.gz`

## Comparing `nicescad-0.0.4.tar` & `nicescad-0.0.5.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.4/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/openscad.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/process.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/profiler.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/version.py
--rw-r--r--   0        0        0    18742 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/webserver.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.4/nicescad/web/static/css/pygments.css
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/intersection.scad
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openjscad_logo.stl
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/GEB.scad
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/advance_intersection.scad
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/animation.scad
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/demo_cut.scad
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/difference.scad
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/fractal.scad
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/intersecting.scad
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/iteration.scad
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/module_recursion.scad
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/offset.scad
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/search.scad
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Advanced/translation.scad
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG-modules.scad
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG.scad
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/LetterBlock.scad
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/children.scad
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/children_indexed.scad
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_cube.scad
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_sphere.scad
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/intersection.scad
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/linear_extrude.scad
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo.scad
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo_and_text.scad
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/projection.scad
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/rotate_extrude.scad
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface.scad
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface_image.scad
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/text_on_cube.scad
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/translate.scad
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Basics/union.scad
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/cut_view.scad
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/fan_view.scad
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/text.scad
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Functions/functions.scad
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Functions/recursion.scad
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/chopped_blocks.scad
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/fence.scad
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/flat_body.scad
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/polyhedron.scad
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/rounded_box.scad
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/sphere.scad
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.4/scad_examples/openscad_examples/Shapes/tripod.scad
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/install
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/openscad_example_scraper.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.4/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/basetest.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_openscad.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_subprocess.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nicescad-0.0.4/tests/test_webserver.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.4/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.4/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nicescad-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.5/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.5/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.5/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/file_selector.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/openscad.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/process.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/profiler.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/version.py
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/webserver.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/web/static/css/pygments.css
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/intersection.scad
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openjscad_logo.stl
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/GEB.scad
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/advance_intersection.scad
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/animation.scad
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/demo_cut.scad
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/difference.scad
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/fractal.scad
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/intersecting.scad
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/iteration.scad
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/module_recursion.scad
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/offset.scad
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/search.scad
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/translation.scad
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG-modules.scad
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG.scad
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/LetterBlock.scad
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/children.scad
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/children_indexed.scad
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_cube.scad
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_sphere.scad
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/intersection.scad
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/linear_extrude.scad
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo.scad
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo_and_text.scad
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/projection.scad
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/rotate_extrude.scad
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface.scad
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface_image.scad
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/text_on_cube.scad
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/translate.scad
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/union.scad
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/cut_view.scad
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/fan_view.scad
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/text.scad
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Functions/functions.scad
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Functions/recursion.scad
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/chopped_blocks.scad
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/fence.scad
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/flat_body.scad
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/polyhedron.scad
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/rounded_box.scad
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/sphere.scad
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/tripod.scad
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/install
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/openscad_example_scraper.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/basetest.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_file_selector.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_openscad.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_subprocess.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.5/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nicescad-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.5/PKG-INFO
```

### Comparing `nicescad-0.0.4/.github/workflows/build.yml` & `nicescad-0.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.5/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/local_filepicker.py` & `nicescad-0.0.5/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/nicescad_cmd.py` & `nicescad-0.0.5/nicescad/nicescad_cmd.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/openscad.py` & `nicescad-0.0.5/nicescad/openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/process.py` & `nicescad-0.0.5/nicescad/process.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/profiler.py` & `nicescad-0.0.5/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/version.py` & `nicescad-0.0.5/nicescad/version.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/nicescad/web/static/css/pygments.css` & `nicescad-0.0.5/nicescad/web/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/intersection.scad` & `nicescad-0.0.5/scad_examples/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openjscad_logo.stl` & `nicescad-0.0.5/scad_examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/GEB.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/GEB.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/advance_intersection.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/advance_intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/animation.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/animation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/demo_cut.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/demo_cut.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/difference.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/difference.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/fractal.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/fractal.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/intersecting.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/intersecting.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/iteration.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/iteration.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/module_recursion.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/module_recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/offset.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/offset.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/search.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/search.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Advanced/translation.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/translation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG-modules.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG-modules.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/CSG.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/LetterBlock.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/LetterBlock.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/children.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/children.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/children_indexed.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/children_indexed.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_cube.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/difference_sphere.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/intersection.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/linear_extrude.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/linear_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/logo_and_text.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo_and_text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/projection.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/projection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/rotate_extrude.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/rotate_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/surface_image.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface_image.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/text_on_cube.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/text_on_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/translate.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/translate.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Basics/union.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Basics/union.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/cut_view.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/cut_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/fan_view.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/fan_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Extrusion/text.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Functions/functions.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Functions/functions.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Functions/recursion.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Functions/recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/chopped_blocks.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/chopped_blocks.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/fence.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/fence.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/flat_body.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/flat_body.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/polyhedron.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/polyhedron.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/rounded_box.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/rounded_box.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/sphere.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scad_examples/openscad_examples/Shapes/tripod.scad` & `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/tripod.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scripts/doc` & `nicescad-0.0.5/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/scripts/openscad_example_scraper.py` & `nicescad-0.0.5/scripts/openscad_example_scraper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/tests/basetest.py` & `nicescad-0.0.5/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/tests/test_openscad.py` & `nicescad-0.0.5/tests/test_openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/tests/test_subprocess.py` & `nicescad-0.0.5/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/.gitignore` & `nicescad-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/LICENSE` & `nicescad-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/README.md` & `nicescad-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/pyproject.toml` & `nicescad-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.4/PKG-INFO` & `nicescad-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

