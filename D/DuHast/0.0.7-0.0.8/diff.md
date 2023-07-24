# Comparing `tmp/DuHast-0.0.7.tar.gz` & `tmp/DuHast-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DuHast-0.0.7.tar", last modified: Sun Jul 23 12:29:59 2023, max compression
+gzip compressed data, was "DuHast-0.0.8.tar", last modified: Mon Jul 24 10:42:36 2023, max compression
```

## Comparing `DuHast-0.0.7.tar` & `DuHast-0.0.8.tar`

### file list

```diff
@@ -1,476 +1,493 @@
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.976572 DuHast-0.0.7/
--rw-r--r--   0 janchristel   (501) staff       (20)       66 2023-07-23 08:19:28.000000 DuHast-0.0.7/MANIFEST.in
--rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-23 12:29:59.976797 DuHast-0.0.7/PKG-INFO
--rw-r--r--   0 janchristel   (501) staff       (20)      407 2023-07-12 08:39:01.000000 DuHast-0.0.7/README.md
--rw-r--r--   0 janchristel   (501) staff       (20)      643 2023-07-23 08:17:02.000000 DuHast-0.0.7/pyproject.toml
--rw-r--r--   0 janchristel   (501) staff       (20)      394 2023-07-23 12:29:59.977592 DuHast-0.0.7/setup.cfg
--rw-r--r--   0 janchristel   (501) staff       (20)      474 2023-07-12 08:39:01.000000 DuHast-0.0.7/setup.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.717942 DuHast-0.0.7/src/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.736434 DuHast-0.0.7/src/DuHast.egg-info/
--rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-23 12:29:59.000000 DuHast-0.0.7/src/DuHast.egg-info/PKG-INFO
--rw-r--r--   0 janchristel   (501) staff       (20)    18294 2023-07-23 12:29:59.000000 DuHast-0.0.7/src/DuHast.egg-info/SOURCES.txt
--rw-r--r--   0 janchristel   (501) staff       (20)        1 2023-07-23 12:29:59.000000 DuHast-0.0.7/src/DuHast.egg-info/dependency_links.txt
--rw-r--r--   0 janchristel   (501) staff       (20)        7 2023-07-23 12:29:59.000000 DuHast-0.0.7/src/DuHast.egg-info/top_level.txt
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.736894 DuHast-0.0.7/src/duHast/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.738489 DuHast-0.0.7/src/duHast/Data/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.739980 DuHast-0.0.7/src/duHast/Data/Objects/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.742822 DuHast-0.0.7/src/duHast/Data/Objects/Properties/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.745192 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7149 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2144 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3723 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3136 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2823 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3339 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_design_set_option.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4205 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_element_geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3092 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_instance_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3218 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_level.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3075 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_phasing.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2897 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_revit_model.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3218 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_type_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6000 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/data_ceiling.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5422 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Objects/data_room.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.748239 DuHast-0.0.7/src/duHast/Data/Utils/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/Utils/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2455 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Utils/data_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2871 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Utils/data_export.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6204 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Utils/data_import.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2735 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/Utils/data_to_file.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10866 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/data_to_shapely.py
--rw-r--r--   0 janchristel   (501) staff       (20)    22887 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Data/process_ceilings_to_rooms.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.750506 DuHast-0.0.7/src/duHast/Revit/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.761051 DuHast-0.0.7/src/duHast/Revit/Annotation/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.764721 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1296 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2612 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1278 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7001 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.766079 DuHast-0.0.7/src/duHast/Revit/Annotation/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3696 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3081 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5152 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/arrow_heads.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4372 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/dimensions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3687 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/generic_annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3081 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6458 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7455 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6138 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3982 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/multi_ref_annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12895 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4337 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/spot_dimensions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2882 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/stair_path.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3663 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Annotation/text.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.768052 DuHast-0.0.7/src/duHast/Revit/BIM360/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/BIM360/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5107 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BIM360/bim_360.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4375 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BIM360/util_bim_360.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.769872 DuHast-0.0.7/src/duHast/Revit/BuildingPads/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.771217 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2047 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.773826 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     3953 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2324 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5679 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/building_pads.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4790 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.775663 DuHast-0.0.7/src/duHast/Revit/Categories/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.778486 DuHast-0.0.7/src/duHast/Revit/Categories/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12627 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10651 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4711 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.780704 DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3055 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/categories_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6772 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.784998 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7333 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12564 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2769 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_property_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12743 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10421 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3675 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/change_family_category.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13463 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Categories/family_sub_categories.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.786858 DuHast-0.0.7/src/duHast/Revit/Ceilings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.787893 DuHast-0.0.7/src/duHast/Revit/Ceilings/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Export/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6363 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.788864 DuHast-0.0.7/src/duHast/Revit/Ceilings/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3239 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Geometry/geometry.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.789763 DuHast-0.0.7/src/duHast/Revit/Ceilings/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1221 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.791994 DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2330 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3013 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6721 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/ceilings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6184 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.804353 DuHast-0.0.7/src/duHast/Revit/Common/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.806578 DuHast-0.0.7/src/duHast/Revit/Common/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    24242 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Geometry/geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2318 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Geometry/solids.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.808971 DuHast-0.0.7/src/duHast/Revit/Common/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2033 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Reporting/groups_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2022 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Reporting/worksets_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2740 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15681 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/common.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4954 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4276 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter_actions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4551 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter_tests.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5122 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5636 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/design_set_options.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7991 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/element_filtering.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11442 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/file_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8015 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/groups.py
--rw-r--r--   0 janchristel   (501) staff       (20)    19927 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/parameter_get_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4360 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/parameter_grouping.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9998 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/parameter_set_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2274 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/phases.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8919 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/purge_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)      289 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/revit_version.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3522 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/transaction.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15172 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Common/worksets.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.810468 DuHast-0.0.7/src/duHast/Revit/DetailItems/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.811369 DuHast-0.0.7/src/duHast/Revit/DetailItems/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1207 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.812680 DuHast-0.0.7/src/duHast/Revit/DetailItems/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2673 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6438 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/detail_items.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8656 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.815031 DuHast-0.0.7/src/duHast/Revit/Exports/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.822382 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7956 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8071 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8108 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13564 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13567 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2308 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14056 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2108 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2834 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/export.py
--rw-r--r--   0 janchristel   (501) staff       (20)    17685 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/export_ifc.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10792 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Exports/export_navis.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.829625 DuHast-0.0.7/src/duHast/Revit/Family/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.841049 DuHast-0.0.7/src/duHast/Revit/Family/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7892 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15524 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11956 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4386 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12685 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
--rw-r--r--   0 janchristel   (501) staff       (20)    16818 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    23832 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_category_data_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10975 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_data_collector.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6758 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7795 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_files.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8669 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8086 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)    19924 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/family_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2349 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_action.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4281 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9219 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_processor.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.842092 DuHast-0.0.7/src/duHast/Revit/Family/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10442 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/Utility/loadable_family_categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3785 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_element_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1734 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_load_option.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5740 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_parameter_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7611 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_reference_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9409 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_reload.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5996 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_rename_files_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    16259 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/family_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7404 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Family/purge_unused_family_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.844236 DuHast-0.0.7/src/duHast/Revit/Floors/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.845123 DuHast-0.0.7/src/duHast/Revit/Floors/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Export/__init__.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.845837 DuHast-0.0.7/src/duHast/Revit/Floors/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1213 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Reporting/floors_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.847682 DuHast-0.0.7/src/duHast/Revit/Floors/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2376 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Utility/floors_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2993 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6966 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/floors.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5625 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Floors/purge_unused_floor_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.851306 DuHast-0.0.7/src/duHast/Revit/Grids/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.853174 DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2852 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2062 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/grids_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8259 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/grids.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14879 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/grids_appearance.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6617 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/grids_worksets.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3459 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Grids/purge_unused_grid_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7652 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/LICENSE
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.855970 DuHast-0.0.7/src/duHast/Revit/Levels/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.858068 DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2024 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/levels_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2917 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4732 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/levels.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14801 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/levels_appearance.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4499 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Levels/purge_unused_level_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.862894 DuHast-0.0.7/src/duHast/Revit/LinePattern/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2224 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/fill_patterns.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12830 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7540 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4315 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10624 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/line_patterns.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3363 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/LinePattern/line_styles.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.866842 DuHast-0.0.7/src/duHast/Revit/Links/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.869983 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2065 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5071 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2124 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/links_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5075 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Reporting/links_report_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.871229 DuHast-0.0.7/src/duHast/Revit/Links/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1562 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/Utility/link_path.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9375 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/cad_links.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3458 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/cad_links_geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5382 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/image_links.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11466 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/links.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3415 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Links/purge_unused_image_link_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.876971 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.878043 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1979 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.881772 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     2490 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3488 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3817 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3766 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6510 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6369 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/cable_trays.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6281 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/conduits.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6369 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/ducts.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6483 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/flex_ducts.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6152 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/pipes.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11395 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14334 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.882611 DuHast-0.0.7/src/duHast/Revit/Materials/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.884447 DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2067 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/materials_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3474 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Materials/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3557 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Materials/materials.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.885376 DuHast-0.0.7/src/duHast/Revit/ModelHealth/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.887022 DuHast-0.0.7/src/duHast/Revit/ModelHealth/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/ModelHealth/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5675 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/ModelHealth/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    27455 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/ModelHealth/model_health.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.889557 DuHast-0.0.7/src/duHast/Revit/Purge/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Purge/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3738 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Purge/purge_action.py
--rw-r--r--   0 janchristel   (501) staff       (20)    25813 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Purge/purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7872 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Purge/purge_unused_e_transmit.py
--rw-r--r--   0 janchristel   (501) staff       (20)      402 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/README.md
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.891672 DuHast-0.0.7/src/duHast/Revit/Railings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.892652 DuHast-0.0.7/src/duHast/Revit/Railings/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2027 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Reporting/railings_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.896560 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2490 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/merge_lists.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2434 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railing_categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2233 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railing_family_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4330 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railings_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3776 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7018 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/balusters.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7825 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8388 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Railings/railings.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.898327 DuHast-0.0.7/src/duHast/Revit/Ramps/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.899254 DuHast-0.0.7/src/duHast/Revit/Ramps/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2016 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.901430 DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     1996 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2359 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3592 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4005 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3591 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Ramps/ramps.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.903969 DuHast-0.0.7/src/duHast/Revit/Revisions/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Revisions/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6701 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Revisions/new_revision.py
--rw-r--r--   0 janchristel   (501) staff       (20)    18324 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Revisions/revisions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4527 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Revisions/sequence.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.905275 DuHast-0.0.7/src/duHast/Revit/Roofs/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.906501 DuHast-0.0.7/src/duHast/Revit/Roofs/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2016 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.909520 DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     2124 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3038 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3719 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5651 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/purge_unused_roof_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6315 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Roofs/roofs.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.911100 DuHast-0.0.7/src/duHast/Revit/Rooms/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.912158 DuHast-0.0.7/src/duHast/Revit/Rooms/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Export/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6048 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Export/to_data_room.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.913282 DuHast-0.0.7/src/duHast/Revit/Rooms/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5568 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Geometry/geometry.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.914354 DuHast-0.0.7/src/duHast/Revit/Rooms/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1194 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3701 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/room_tags.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4476 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Rooms/rooms.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.919913 DuHast-0.0.7/src/duHast/Revit/SharedParameters/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.921522 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)     5298 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7836 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5767 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.923001 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4835 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2077 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13905 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_add.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5298 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8096 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8196 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10845 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6670 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1215 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.927387 DuHast-0.0.7/src/duHast/Revit/Stairs/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.928374 DuHast-0.0.7/src/duHast/Revit/Stairs/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2022 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.929693 DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2448 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/stairs_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3607 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2210 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/cut_marks.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2223 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/landings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2574 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/path.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15680 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/purge_unused_stair_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2170 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/runs.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5819 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/stairs.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2539 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Stairs/stringers_carriages.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.936446 DuHast-0.0.7/src/duHast/Revit/Views/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.940400 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7429 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/schedules_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6828 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/sheets_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3144 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/view_property_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2544 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/view_property_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7505 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/views_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4727 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Reporting/views_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.942063 DuHast-0.0.7/src/duHast/Revit/Views/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2742 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Utility/data_category_override.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1527 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/Utility/view_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9097 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5923 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/filters.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15057 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/referencing.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3622 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/schedules.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5904 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/sheets.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7019 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/templates.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6548 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/views.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8148 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/views_purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4852 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Views/visibility_graphics_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.946363 DuHast-0.0.7/src/duHast/Revit/Walls/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.948077 DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3909 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/walls_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1299 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/walls_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.949933 DuHast-0.0.7/src/duHast/Revit/Walls/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2052 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Utility/walls_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2967 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9609 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/curtain_wall_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3207 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/curtain_walls.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5681 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7760 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/purge_unused_wall_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2912 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/stacked_walls.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6331 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Walls/walls.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.952891 DuHast-0.0.7/src/duHast/Revit/Warnings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.954641 DuHast-0.0.7/src/duHast/Revit/Warnings/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4864 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/Data/warnings_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3728 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/Data/warnings_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5501 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/solver.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5493 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/solver_duplicate_mark.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3644 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2413 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/Warnings/warnings.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Revit/__init__.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.960524 DuHast-0.0.7/src/duHast/UI/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.7/src/duHast/UI/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3004 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/file_item.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9641 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/UI/file_list.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3243 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/file_select_settings.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13350 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/script.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7559 2023-07-12 08:39:01.000000 DuHast-0.0.7/src/duHast/UI/ui.xaml
--rw-r--r--   0 janchristel   (501) staff       (20)     4910 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/ui_file_select.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3285 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/workload_bucket.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4352 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/UI/workloader.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.973214 DuHast-0.0.7/src/duHast/Utilities/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-23 12:29:59.975753 DuHast-0.0.7/src/duHast/Utilities/Objects/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/Utilities/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2875 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/Objects/base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4899 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/Objects/result.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3672 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/Objects/timer.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.7/src/duHast/Utilities/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    30001 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/batch_processor_log_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3503 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/compare.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4919 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/console_out.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4821 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/date_stamps.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5346 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/directory_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12864 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_combine.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5428 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_csv.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8434 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_get.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8553 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3816 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_json.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5064 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/files_tab.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5056 2023-07-23 08:28:07.000000 DuHast-0.0.7/src/duHast/Utilities/padding.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8758 2023-07-23 08:28:07.000000 DuHast-0.0.7/src/duHast/Utilities/solibri_ifc_optimizer.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7528 2023-07-23 08:28:07.000000 DuHast-0.0.7/src/duHast/Utilities/system_process.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2668 2023-07-23 08:28:07.000000 DuHast-0.0.7/src/duHast/Utilities/unit_conversion.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3776 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/util_batch_p.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6654 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/utility.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9175 2023-07-23 08:28:08.000000 DuHast-0.0.7/src/duHast/Utilities/worksharing_monitor_process.py
--rw-r--r--   0 janchristel   (501) staff       (20)      246 2023-07-12 08:39:08.000000 DuHast-0.0.7/src/duHast/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.434000 DuHast-0.0.8/
+-rw-r--r--   0 janchristel   (501) staff       (20)       66 2023-07-23 12:58:56.000000 DuHast-0.0.8/MANIFEST.in
+-rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-24 10:42:36.434285 DuHast-0.0.8/PKG-INFO
+-rw-r--r--   0 janchristel   (501) staff       (20)      407 2023-07-12 08:39:01.000000 DuHast-0.0.8/README.md
+-rw-r--r--   0 janchristel   (501) staff       (20)      643 2023-07-24 10:21:13.000000 DuHast-0.0.8/pyproject.toml
+-rw-r--r--   0 janchristel   (501) staff       (20)      394 2023-07-24 10:42:36.435286 DuHast-0.0.8/setup.cfg
+-rw-r--r--   0 janchristel   (501) staff       (20)      474 2023-07-12 08:39:01.000000 DuHast-0.0.8/setup.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.170902 DuHast-0.0.8/src/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.194741 DuHast-0.0.8/src/DuHast.egg-info/
+-rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/PKG-INFO
+-rw-r--r--   0 janchristel   (501) staff       (20)    19041 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/SOURCES.txt
+-rw-r--r--   0 janchristel   (501) staff       (20)        1 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/dependency_links.txt
+-rw-r--r--   0 janchristel   (501) staff       (20)        7 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/top_level.txt
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.195283 DuHast-0.0.8/src/duHast/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.196517 DuHast-0.0.8/src/duHast/Data/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.198106 DuHast-0.0.8/src/duHast/Data/Objects/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.202705 DuHast-0.0.8/src/duHast/Data/Objects/Properties/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.205420 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7146 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2144 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3720 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3133 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2820 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3336 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_design_set_option.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4202 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_element_geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3089 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_instance_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_level.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3072 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_phasing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2894 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_revit_model.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_type_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5997 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/data_ceiling.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5419 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/data_room.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.207578 DuHast-0.0.8/src/duHast/Data/Utils/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Utils/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2452 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2868 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_export.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6201 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_import.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2732 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_to_file.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10863 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/data_to_shapely.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    22884 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/process_ceilings_to_rooms.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.208870 DuHast-0.0.8/src/duHast/Revit/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.214277 DuHast-0.0.8/src/duHast/Revit/Annotation/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.217563 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1296 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2609 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1278 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7001 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.218670 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3693 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5149 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/arrow_heads.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4369 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/dimensions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3684 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/generic_annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6455 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7452 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6135 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3979 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/multi_ref_annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12895 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4334 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/spot_dimensions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2879 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/stair_path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3660 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/text.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.220493 DuHast-0.0.8/src/duHast/Revit/BIM360/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5104 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/bim_360.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4372 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/util_bim_360.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.222185 DuHast-0.0.8/src/duHast/Revit/BuildingPads/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.223357 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2044 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.225274 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     3950 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2324 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5676 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/building_pads.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4787 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.227538 DuHast-0.0.8/src/duHast/Revit/Categories/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.230039 DuHast-0.0.8/src/duHast/Revit/Categories/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12624 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10648 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4708 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.232110 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3052 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6769 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.235307 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7330 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12561 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2766 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_property_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12740 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10421 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3675 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/change_family_category.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13460 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/family_sub_categories.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.237104 DuHast-0.0.8/src/duHast/Revit/Ceilings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.238221 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6363 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.239337 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3239 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/geometry.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.241657 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1221 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.243544 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2330 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3013 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6718 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/ceilings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6184 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.254776 DuHast-0.0.8/src/duHast/Revit/Common/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.256463 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    24242 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2318 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/solids.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.259231 DuHast-0.0.8/src/duHast/Revit/Common/Objects/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3085 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/colour_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2270 2023-07-24 10:28:32.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_cut.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3379 2023-07-24 10:32:37.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_graphic_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2298 2023-07-24 10:32:43.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_projection.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2322 2023-07-24 10:33:04.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_background.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2322 2023-07-24 10:33:10.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_foreground.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3425 2023-07-24 10:33:17.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_graphic_base.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.260539 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2030 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/groups_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2737 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15678 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/common.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4951 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4273 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_actions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4548 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_tests.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5119 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5636 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/design_set_options.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7988 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/element_filtering.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11442 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/file_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8015 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/groups.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    19924 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_get_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4357 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_grouping.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9995 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_set_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2274 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/phases.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8916 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/purge_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)      289 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/revit_version.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3519 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/transaction.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15172 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/worksets.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.261502 DuHast-0.0.8/src/duHast/Revit/DetailItems/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.262321 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1207 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.262966 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2673 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6435 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/detail_items.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8656 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.265019 DuHast-0.0.8/src/duHast/Revit/Exports/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.270825 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7953 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8068 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8105 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13561 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13564 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2305 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14053 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2105 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Exports/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2831 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    17682 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export_ifc.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10789 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export_navis.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.277020 DuHast-0.0.8/src/duHast/Revit/Family/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.290265 DuHast-0.0.8/src/duHast/Revit/Family/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7889 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15521 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11953 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4383 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12682 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    16815 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    23829 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_category_data_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10972 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_data_collector.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6755 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7792 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_files.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8666 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8083 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    19921 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2346 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_action.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4278 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9216 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_processor.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.291359 DuHast-0.0.8/src/duHast/Revit/Family/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10439 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Utility/loadable_family_categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3782 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_element_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1734 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_load_option.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5737 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_parameter_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7608 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_reference_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9406 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_reload.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5993 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_rename_files_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    16256 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7401 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/purge_unused_family_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.292872 DuHast-0.0.8/src/duHast/Revit/Floors/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.293520 DuHast-0.0.8/src/duHast/Revit/Floors/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Export/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.294548 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1213 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/floors_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.296369 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2376 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2993 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6963 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Floors/floors.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5625 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/purge_unused_floor_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.299346 DuHast-0.0.8/src/duHast/Revit/Grids/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.301052 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2849 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2059 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grids_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Grids/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8256 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14876 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids_appearance.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6624 2023-07-24 10:32:46.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids_worksets.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3456 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/purge_unused_grid_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7652 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/LICENSE
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.303732 DuHast-0.0.8/src/duHast/Revit/Levels/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.305407 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2021 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2914 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4732 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/levels.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14798 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/levels_appearance.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4496 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/purge_unused_level_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.309670 DuHast-0.0.8/src/duHast/Revit/LinePattern/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2221 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/fill_patterns.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12827 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7537 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4312 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10621 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_patterns.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3360 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_styles.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.313221 DuHast-0.0.8/src/duHast/Revit/Links/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.316383 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2062 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5068 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5072 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.317616 DuHast-0.0.8/src/duHast/Revit/Links/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1562 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Utility/link_path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9372 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/cad_links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3455 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/cad_links_geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5379 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/image_links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11463 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3412 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/purge_unused_image_link_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.322653 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.323739 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1976 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.327184 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3485 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3814 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3763 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6507 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/cable_trays.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6278 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/conduits.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/ducts.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6480 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/flex_ducts.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6149 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/pipes.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11392 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14331 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.328059 DuHast-0.0.8/src/duHast/Revit/Materials/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.332934 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2064 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3471 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Materials/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3554 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/materials.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.333974 DuHast-0.0.8/src/duHast/Revit/ModelHealth/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.335107 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5675 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    27455 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/model_health.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.337739 DuHast-0.0.8/src/duHast/Revit/Purge/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Purge/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3735 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_action.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    25813 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7869 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused_e_transmit.py
+-rw-r--r--   0 janchristel   (501) staff       (20)      402 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/README.md
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.339855 DuHast-0.0.8/src/duHast/Revit/Railings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.340849 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2024 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/railings_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.344234 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/merge_lists.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2431 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2230 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_family_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4327 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7015 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/balusters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7825 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8385 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/railings.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.345843 DuHast-0.0.8/src/duHast/Revit/Ramps/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.346872 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.349417 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     1993 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2356 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3589 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4005 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3588 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/ramps.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.351814 DuHast-0.0.8/src/duHast/Revit/Revisions/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6698 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/new_revision.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    18321 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/revisions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4524 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/sequence.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.352842 DuHast-0.0.8/src/duHast/Revit/Roofs/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.353461 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.354838 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3035 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3716 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5651 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/purge_unused_roof_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6312 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/roofs.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.355717 DuHast-0.0.8/src/duHast/Revit/Rooms/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.356321 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6045 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/to_data_room.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.356935 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5565 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/geometry.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.357559 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1194 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3698 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/room_tags.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4473 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/rooms.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.360234 DuHast-0.0.8/src/duHast/Revit/SharedParameters/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.361247 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)     5295 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7833 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5764 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.362206 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4832 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2074 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13905 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_add.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5295 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8096 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8193 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10845 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6667 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1215 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.365415 DuHast-0.0.8/src/duHast/Revit/Stairs/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.366302 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.367774 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2448 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3604 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2210 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/cut_marks.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2223 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/landings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2574 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15680 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/purge_unused_stair_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2170 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/runs.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5819 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/stairs.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2539 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/stringers_carriages.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.373472 DuHast-0.0.8/src/duHast/Revit/Views/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.377072 DuHast-0.0.8/src/duHast/Revit/Views/Objects/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3700 2023-07-24 10:35:01.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/category_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2596 2023-07-24 10:34:10.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_category.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2299 2023-07-24 10:34:15.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3822 2023-07-24 10:34:40.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_cut.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3996 2023-07-24 10:34:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_projection.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3983 2023-07-24 10:34:50.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/view_graphics_settings.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.380661 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7426 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/schedules_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6825 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/sheets_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3141 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2541 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7502 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4724 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.382220 DuHast-0.0.8/src/duHast/Revit/Views/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2795 2023-07-24 10:40:32.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/data_view.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1527 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/view_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9094 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5923 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/filters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15057 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/referencing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3619 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/schedules.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5901 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/sheets.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7016 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/templates.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6545 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/views.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8145 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/views_purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4849 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/visibility_graphics_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.386049 DuHast-0.0.8/src/duHast/Revit/Walls/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.387640 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3909 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1299 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.389226 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2052 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2967 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9609 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/curtain_wall_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3207 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/curtain_walls.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5681 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7760 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_wall_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2912 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/stacked_walls.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6331 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/walls.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.412592 DuHast-0.0.8/src/duHast/Revit/Warnings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.413629 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4861 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3725 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5498 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5490 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver_duplicate_mark.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3641 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2413 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/warnings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.419415 DuHast-0.0.8/src/duHast/UI/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/UI/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3001 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/file_item.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9641 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/UI/file_list.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3240 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/file_select_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13347 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/script.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7559 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/UI/ui.xaml
+-rw-r--r--   0 janchristel   (501) staff       (20)     4907 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/ui_file_select.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3282 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/workload_bucket.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4349 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/workloader.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.431136 DuHast-0.0.8/src/duHast/Utilities/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.433444 DuHast-0.0.8/src/duHast/Utilities/Objects/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2872 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4896 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/result.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3669 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/timer.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/Utilities/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    29998 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/batch_processor_log_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3500 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/compare.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4916 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/console_out.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4818 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/date_stamps.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5343 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/directory_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12861 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_combine.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5425 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_csv.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8431 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_get.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8550 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3813 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_json.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5061 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_tab.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5053 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/padding.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8755 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/solibri_ifc_optimizer.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7525 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/system_process.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2665 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/unit_conversion.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/util_batch_p.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6651 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/utility.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9172 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/worksharing_monitor_process.py
+-rw-r--r--   0 janchristel   (501) staff       (20)      246 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/__init__.py
```

### Comparing `DuHast-0.0.7/PKG-INFO` & `DuHast-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DuHast
-Version: 0.0.7
+Version: 0.0.8
 Summary: Revit API sample snippets and Revit Batch Processor flows.
 Home-page: UNKNOWN
 Author: Jan Christel
 Author-email: jan.r.christel@gmail.com
 License: BSD-3-Clause
 Description: # Code samples for the Revit Batch Processor
         This repository contains code samples for the [Revit Batch Processor](https://github.com/bvn-architecture/RevitBatchProcessor)
```

### Comparing `DuHast-0.0.7/pyproject.toml` & `DuHast-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires = ["setuptools==43.0.0", "wheel==0.33.6"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/jchristel/SampleCodeRevitBatchProcessor"
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `DuHast-0.0.7/src/DuHast.egg-info/PKG-INFO` & `DuHast-0.0.8/src/DuHast.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DuHast
-Version: 0.0.7
+Version: 0.0.8
 Summary: Revit API sample snippets and Revit Batch Processor flows.
 Home-page: UNKNOWN
 Author: Jan Christel
 Author-email: jan.r.christel@gmail.com
 License: BSD-3-Clause
 Description: # Code samples for the Revit Batch Processor
         This repository contains code samples for the [Revit Batch Processor](https://github.com/bvn-architecture/RevitBatchProcessor)
```

### Comparing `DuHast-0.0.7/src/DuHast.egg-info/SOURCES.txt` & `DuHast-0.0.8/src/DuHast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,22 @@
 src/duHast/Revit/Common/purge_utils.py
 src/duHast/Revit/Common/revit_version.py
 src/duHast/Revit/Common/transaction.py
 src/duHast/Revit/Common/worksets.py
 src/duHast/Revit/Common/Geometry/__init__.py
 src/duHast/Revit/Common/Geometry/geometry.py
 src/duHast/Revit/Common/Geometry/solids.py
+src/duHast/Revit/Common/Objects/__init__.py
+src/duHast/Revit/Common/Objects/colour_base.py
+src/duHast/Revit/Common/Objects/line_cut.py
+src/duHast/Revit/Common/Objects/line_graphic_base.py
+src/duHast/Revit/Common/Objects/line_projection.py
+src/duHast/Revit/Common/Objects/pattern_background.py
+src/duHast/Revit/Common/Objects/pattern_foreground.py
+src/duHast/Revit/Common/Objects/pattern_graphic_base.py
 src/duHast/Revit/Common/Reporting/__init__.py
 src/duHast/Revit/Common/Reporting/groups_report_header.py
 src/duHast/Revit/Common/Reporting/worksets_report_header.py
 src/duHast/Revit/Common/Reporting/worksets_report_utils.py
 src/duHast/Revit/DetailItems/__init__.py
 src/duHast/Revit/DetailItems/detail_items.py
 src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
@@ -318,23 +326,30 @@
 src/duHast/Revit/Views/referencing.py
 src/duHast/Revit/Views/schedules.py
 src/duHast/Revit/Views/sheets.py
 src/duHast/Revit/Views/templates.py
 src/duHast/Revit/Views/views.py
 src/duHast/Revit/Views/views_purge_unused.py
 src/duHast/Revit/Views/visibility_graphics_utils.py
+src/duHast/Revit/Views/Objects/__init__.py
+src/duHast/Revit/Views/Objects/category_base.py
+src/duHast/Revit/Views/Objects/override_by_category.py
+src/duHast/Revit/Views/Objects/override_by_filter.py
+src/duHast/Revit/Views/Objects/override_cut.py
+src/duHast/Revit/Views/Objects/override_projection.py
+src/duHast/Revit/Views/Objects/view_graphics_settings.py
 src/duHast/Revit/Views/Reporting/__init__.py
 src/duHast/Revit/Views/Reporting/schedules_report.py
 src/duHast/Revit/Views/Reporting/sheets_report.py
 src/duHast/Revit/Views/Reporting/view_property_filter.py
 src/duHast/Revit/Views/Reporting/view_property_utils.py
 src/duHast/Revit/Views/Reporting/views_report.py
 src/duHast/Revit/Views/Reporting/views_report_header.py
 src/duHast/Revit/Views/Utility/__init__.py
-src/duHast/Revit/Views/Utility/data_category_override.py
+src/duHast/Revit/Views/Utility/data_view.py
 src/duHast/Revit/Views/Utility/view_types.py
 src/duHast/Revit/Walls/__init__.py
 src/duHast/Revit/Walls/curtain_wall_elements.py
 src/duHast/Revit/Walls/curtain_walls.py
 src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
 src/duHast/Revit/Walls/purge_unused_wall_types.py
 src/duHast/Revit/Walls/stacked_walls.py
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_design_set_option.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_design_set_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_element_geometry.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_element_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_instance_properties.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_instance_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_level.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_phasing.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_phasing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_revit_model.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_revit_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/Properties/data_type_properties.py` & `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_type_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/data_ceiling.py` & `DuHast-0.0.8/src/duHast/Data/Objects/data_ceiling.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Objects/data_room.py` & `DuHast-0.0.8/src/duHast/Data/Objects/data_room.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Utils/data_base.py` & `DuHast-0.0.8/src/duHast/Data/Utils/data_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Utils/data_export.py` & `DuHast-0.0.8/src/duHast/Data/Utils/data_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Utils/data_import.py` & `DuHast-0.0.8/src/duHast/Data/Utils/data_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/Utils/data_to_file.py` & `DuHast-0.0.8/src/duHast/Data/Utils/data_to_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/data_to_shapely.py` & `DuHast-0.0.8/src/duHast/Data/data_to_shapely.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Data/process_ceilings_to_rooms.py` & `DuHast-0.0.8/src/duHast/Data/process_ceilings_to_rooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/annotation.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/arrow_heads.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/arrow_heads.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/dimensions.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/dimensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/generic_annotation.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/generic_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_modify_properties.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_modify_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/multi_ref_annotation.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/multi_ref_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/purge_unused_annotation_types.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/purge_unused_annotation_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/spot_dimensions.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/spot_dimensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/stair_path.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/stair_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Annotation/text.py` & `DuHast-0.0.8/src/duHast/Revit/Annotation/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BIM360/bim_360.py` & `DuHast-0.0.8/src/duHast/Revit/BIM360/bim_360.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BIM360/util_bim_360.py` & `DuHast-0.0.8/src/duHast/Revit/BIM360/util_bim_360.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py` & `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py` & `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/BuildingPads/building_pads.py` & `DuHast-0.0.8/src/duHast/Revit/BuildingPads/building_pads.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py` & `DuHast-0.0.8/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data_processor.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Data/category_data_purge_unused.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_purge_unused.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/categories_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Reporting/categories_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Utility/category_property_names.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_property_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/categories.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/change_family_category.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/change_family_category.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Categories/family_sub_categories.py` & `DuHast-0.0.8/src/duHast/Revit/Categories/family_sub_categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/Geometry/geometry.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/ceilings.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/ceilings.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py` & `DuHast-0.0.8/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/Geometry/geometry.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/Geometry/solids.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Geometry/solids.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/Reporting/groups_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/groups_report_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/Reporting/worksets_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grids_report_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any worksets reports. 
+This module contains the header row for any grids reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -24,8 +24,15 @@
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # -------------------------------------------- common variables --------------------
 #: header used in reports
-REPORT_WORKSETS_HEADER = ["HOSTFILE", "ID", "NAME", "ISVISIBLEBYDEFAULT"]
+REPORT_GRIDS_HEADER = [
+    "HOSTFILE",
+    "ID",
+    "NAME",
+    "WORKSETNAME",
+    "EXTENTMAX",
+    "EXTENTMIN",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/Reporting/worksets_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/common.py` & `DuHast-0.0.8/src/duHast/Revit/Common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter_actions.py` & `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/custom_element_filter_tests.py` & `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/delete.py` & `DuHast-0.0.8/src/duHast/Revit/Common/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/design_set_options.py` & `DuHast-0.0.8/src/duHast/Revit/Common/design_set_options.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/element_filtering.py` & `DuHast-0.0.8/src/duHast/Revit/Common/element_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/file_io.py` & `DuHast-0.0.8/src/duHast/Revit/Common/file_io.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/groups.py` & `DuHast-0.0.8/src/duHast/Revit/Common/groups.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/parameter_get_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Common/parameter_get_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/parameter_grouping.py` & `DuHast-0.0.8/src/duHast/Revit/Common/parameter_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/parameter_set_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Common/parameter_set_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/phases.py` & `DuHast-0.0.8/src/duHast/Revit/Common/phases.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/purge_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Common/purge_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/transaction.py` & `DuHast-0.0.8/src/duHast/Revit/Common/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Common/worksets.py` & `DuHast-0.0.8/src/duHast/Revit/Common/worksets.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/DetailItems/detail_items.py` & `DuHast-0.0.8/src/duHast/Revit/DetailItems/detail_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py` & `DuHast-0.0.8/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_settings.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/export.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/export_ifc.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/export_ifc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Exports/export_navis.py` & `DuHast-0.0.8/src/duHast/Revit/Exports/export_navis.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_missing_families.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_missing_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_processor.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_base_data_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_category_data_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_category_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_data_collector.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_data_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_files.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_find_host_families.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_find_host_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_rename_loaded_families.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_loaded_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/family_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_report_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_action.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_data.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Data/ifamily_processor.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/Utility/loadable_family_categories.py` & `DuHast-0.0.8/src/duHast/Revit/Family/Utility/loadable_family_categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_element_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_element_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_load_option.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_load_option.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_parameter_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_parameter_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_reference_elements.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_reference_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_reload.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_reload.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_rename_files_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_rename_files_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/family_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Family/family_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Family/purge_unused_family_types.py` & `DuHast-0.0.8/src/duHast/Revit/Family/purge_unused_family_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Floors/Reporting/floors_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/floors_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Floors/Utility/floors_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Floors/Utility/floors_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Floors/floors.py` & `DuHast-0.0.8/src/duHast/Revit/Floors/floors.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Floors/purge_unused_floor_types.py` & `DuHast-0.0.8/src/duHast/Revit/Floors/purge_unused_floor_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/grid_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grid_report_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/Reporting/grids_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any grids reports. 
+This module contains the header row for any Revit roofs reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -24,15 +24,8 @@
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # -------------------------------------------- common variables --------------------
 #: header used in reports
-REPORT_GRIDS_HEADER = [
-    "HOSTFILE",
-    "ID",
-    "NAME",
-    "WORKSETNAME",
-    "EXTENTMAX",
-    "EXTENTMIN",
-]
+REPORT_ROOFS_HEADER = ["HOSTFILE", "ROOFTYPEID", "ROOFTYPENAME"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/grids.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/grids.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/grids_appearance.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/grids_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/grids_worksets.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/grids_worksets.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -59,24 +59,26 @@
             gridsResults.update(grids)
     return gridsResults
 
 
 def modify_grid_worksets_by_type_name(doc, worksetRules):
     """
     Workset modifier method. Moves grids matching type condition to a particular workset
+    
     defaultWorksetTypeRules_ = [
         ['model name',[
             [ModifyGridWorkSetsByTypeName,[
                 ['workset name', util.ConDoesNotEqual, 'grid type name'],
                 ['workset name', util.ConDoesEqual, 'grid type name']
                 ]
             ]
             ]
         ]
     ]
+    
     :param doc: _description_
     :type doc: _type_
     :param worksetRules: _description_
     :type worksetRules: _type_
     :return: returns a result object
     :rtype: _type_
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Grids/purge_unused_grid_types.py` & `DuHast-0.0.8/src/duHast/Revit/Grids/purge_unused_grid_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LICENSE` & `DuHast-0.0.8/src/duHast/Revit/LICENSE`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/levels_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Levels/Reporting/levels_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Levels/levels.py` & `DuHast-0.0.8/src/duHast/Revit/Levels/levels.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Levels/levels_appearance.py` & `DuHast-0.0.8/src/duHast/Revit/Levels/levels_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Levels/purge_unused_level_types.py` & `DuHast-0.0.8/src/duHast/Revit/Levels/purge_unused_level_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/fill_patterns.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/fill_patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data_processor.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/line_patterns.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/LinePattern/line_styles.py` & `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/Reporting/cad_links_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/Reporting/links_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/Reporting/links_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/Utility/link_path.py` & `DuHast-0.0.8/src/duHast/Revit/Links/Utility/link_path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/cad_links.py` & `DuHast-0.0.8/src/duHast/Revit/Links/cad_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/cad_links_geometry.py` & `DuHast-0.0.8/src/duHast/Revit/Links/cad_links_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/image_links.py` & `DuHast-0.0.8/src/duHast/Revit/Links/image_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/links.py` & `DuHast-0.0.8/src/duHast/Revit/Links/links.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Links/purge_unused_image_link_types.py` & `DuHast-0.0.8/src/duHast/Revit/Links/purge_unused_image_link_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/cable_trays.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/cable_trays.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/conduits.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/conduits.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/ducts.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/ducts.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/flex_ducts.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/flex_ducts.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/pipes.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/pipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py` & `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/materials_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Materials/Reporting/materials_report_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Materials/materials.py` & `DuHast-0.0.8/src/duHast/Revit/Materials/materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py` & `DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/ModelHealth/model_health.py` & `DuHast-0.0.8/src/duHast/Revit/ModelHealth/model_health.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Purge/purge_action.py` & `DuHast-0.0.8/src/duHast/Revit/Purge/purge_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Purge/purge_unused.py` & `DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Purge/purge_unused_e_transmit.py` & `DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused_e_transmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Reporting/railings_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any Revit railing reports. 
+This module contains the header row for any (future) stair reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -24,8 +24,8 @@
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # -------------------------------------------- common variables --------------------
 #: header used in reports
-REPORT_RAILINGS_HEADER = ["HOSTFILE", "RAILINGTYPEID", "RAILINGTYPENAME"]
+REPORT_STAIRS_HEADER = ["HOSTFILE", "STAIRTYPEID", "STAIRTYPENAME"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Utility/merge_lists.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/merge_lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railing_categories.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railing_family_names.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_family_names.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railings_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/Utility/railings_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_type_sorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/balusters.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/balusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Railings/railings.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/railings.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/purge_unused_ramp_types.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/purge_unused_ramp_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Ramps/ramps.py` & `DuHast-0.0.8/src/duHast/Revit/Ramps/ramps.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Revisions/new_revision.py` & `DuHast-0.0.8/src/duHast/Revit/Revisions/new_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Revisions/revisions.py` & `DuHast-0.0.8/src/duHast/Revit/Revisions/revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Revisions/sequence.py` & `DuHast-0.0.8/src/duHast/Revit/Revisions/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any Revit roofs reports. 
+This module contains the header row for any Revit shared parameter reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -22,10 +22,17 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
+
 # -------------------------------------------- common variables --------------------
-#: header used in reports
-REPORT_ROOFS_HEADER = ["HOSTFILE", "ROOFTYPEID", "ROOFTYPENAME"]
+#: headers used in reports
+REPORT_SHARED_PARAMETERS_HEADER = [
+    "HOSTFILE",
+    "GUID",
+    "ID",
+    "NAME",
+    "PARAMETERBINDINGS",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/purge_unused_roof_types.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/purge_unused_roof_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Roofs/roofs.py` & `DuHast-0.0.8/src/duHast/Revit/Roofs/roofs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Rooms/Export/to_data_room.py` & `DuHast-0.0.8/src/duHast/Revit/Rooms/Export/to_data_room.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Rooms/Geometry/geometry.py` & `DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Rooms/room_tags.py` & `DuHast-0.0.8/src/duHast/Revit/Rooms/room_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Rooms/rooms.py` & `DuHast-0.0.8/src/duHast/Revit/Rooms/rooms.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_header.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any Revit shared parameter reports. 
+This module contains the header row for any worksets reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -22,17 +22,10 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-
 # -------------------------------------------- common variables --------------------
-#: headers used in reports
-REPORT_SHARED_PARAMETERS_HEADER = [
-    "HOSTFILE",
-    "GUID",
-    "ID",
-    "NAME",
-    "PARAMETERBINDINGS",
-]
+#: header used in reports
+REPORT_WORKSETS_HEADER = ["HOSTFILE", "ID", "NAME", "ISVISIBLEBYDEFAULT"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_add.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_add.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_data.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_swap.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_swap.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters_delete.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py` & `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/railings_report_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the header row for any (future) stair reports. 
+This module contains the header row for any Revit railing reports. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -24,8 +24,8 @@
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # -------------------------------------------- common variables --------------------
 #: header used in reports
-REPORT_STAIRS_HEADER = ["HOSTFILE", "STAIRTYPEID", "STAIRTYPENAME"]
+REPORT_RAILINGS_HEADER = ["HOSTFILE", "RAILINGTYPEID", "RAILINGTYPENAME"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/stairs_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/cut_marks.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/cut_marks.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/landings.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/landings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/path.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/purge_unused_stair_types.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/purge_unused_stair_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/runs.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/runs.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/stairs.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/stairs.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Stairs/stringers_carriages.py` & `DuHast-0.0.8/src/duHast/Revit/Stairs/stringers_carriages.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/schedules_report.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/schedules_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/sheets_report.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/sheets_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/view_property_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/view_property_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/views_report.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Reporting/views_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Utility/data_category_override.py` & `DuHast-0.0.8/src/duHast/Revit/Common/Objects/colour_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Category override data storage class.
+A base class used to store colour values.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+Stores colour values as rgb.
+
 """
+
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -23,39 +29,54 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import json
-from duHast.Utilities.Objects import base
 
+from duHast.Utilities.Objects import base
 
-class DataCategoryOverride(base.Base):
-    def __init__(self, data_type, j={}):
+class ColourBase(base.Base):
+    data_type = "colour"
+    
+    def __init__(self,j={},**kwargs):
         """
-        Class constructor
+        Class constructor.
 
-        :param j:  json formatted dictionary of this class, defaults to {}
-        :type j: dict, optional
         """
 
-        # store data type  in base class
-        super(DataCategoryOverride, self).__init__()
+        super(ColourBase, self).__init__(**kwargs)
 
         # check if any data was past in with constructor!
         if j != None and len(j) > 0:
             # check type of data that came in:
             if type(j) == str:
                 # a string
                 j = json.loads(j)
             elif type(j) == dict:
                 # no action required
                 pass
             else:
-                print("j", j)
                 raise ValueError(
                     "Argument supplied must be of type string or type dictionary"
                 )
-
+            
+            # load overrides
+            if "red" in j:
+                self.red = j["red"]
+            else:
+                self.red = 0
+            
+            if "green" in j:
+                self.green = j["green"]
+            else:
+                self.green = 0
+            
+            if "blue" in j:
+                self.blue = j["blue"]
+            else:
+                self.blue = 0
         else:
-            pass
+            self.red = 0
+            self.green = 0 
+            self.blue = 0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/Utility/view_types.py` & `DuHast-0.0.8/src/duHast/Revit/Views/Utility/view_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/delete.py` & `DuHast-0.0.8/src/duHast/Revit/Views/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/filters.py` & `DuHast-0.0.8/src/duHast/Revit/Views/filters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/referencing.py` & `DuHast-0.0.8/src/duHast/Revit/Views/referencing.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/schedules.py` & `DuHast-0.0.8/src/duHast/Revit/Views/schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/sheets.py` & `DuHast-0.0.8/src/duHast/Revit/Views/sheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/templates.py` & `DuHast-0.0.8/src/duHast/Revit/Views/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/views.py` & `DuHast-0.0.8/src/duHast/Revit/Views/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/views_purge_unused.py` & `DuHast-0.0.8/src/duHast/Revit/Views/views_purge_unused.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Views/visibility_graphics_utils.py` & `DuHast-0.0.8/src/duHast/Revit/Views/visibility_graphics_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/walls_report.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/Reporting/walls_report_header.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/Utility/walls_filter.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/Utility/walls_type_sorting.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/curtain_wall_elements.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/curtain_wall_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/curtain_walls.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/curtain_walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/purge_unused_wall_types.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_wall_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/stacked_walls.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/stacked_walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Walls/walls.py` & `DuHast-0.0.8/src/duHast/Revit/Walls/walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/Data/warnings_data.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/Data/warnings_data_processor.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/solver.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/solver_duplicate_mark.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/solver_duplicate_mark.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/solver_room_tag_to_room.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/solver_room_tag_to_room.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Revit/Warnings/warnings.py` & `DuHast-0.0.8/src/duHast/Revit/Warnings/warnings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/UI/file_item.py` & `DuHast-0.0.8/src/duHast/UI/file_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/UI/file_list.py` & `DuHast-0.0.8/src/duHast/UI/file_list.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/UI/file_select_settings.py` & `DuHast-0.0.8/src/duHast/UI/file_select_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/UI/script.py` & `DuHast-0.0.8/src/duHast/UI/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/UI/ui.xaml` & `DuHast-0.0.8/src/duHast/UI/ui.xaml`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.7/src/duHast/UI/ui_file_select.py` & `DuHast-0.0.8/src/duHast/UI/ui_file_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/UI/workload_bucket.py` & `DuHast-0.0.8/src/duHast/UI/workload_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/UI/workloader.py` & `DuHast-0.0.8/src/duHast/UI/workloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/Objects/base.py` & `DuHast-0.0.8/src/duHast/Utilities/Objects/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/Objects/result.py` & `DuHast-0.0.8/src/duHast/Utilities/Objects/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/Objects/timer.py` & `DuHast-0.0.8/src/duHast/Utilities/Objects/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/batch_processor_log_utils.py` & `DuHast-0.0.8/src/duHast/Utilities/batch_processor_log_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/compare.py` & `DuHast-0.0.8/src/duHast/Utilities/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/console_out.py` & `DuHast-0.0.8/src/duHast/Utilities/console_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/date_stamps.py` & `DuHast-0.0.8/src/duHast/Utilities/date_stamps.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/directory_io.py` & `DuHast-0.0.8/src/duHast/Utilities/directory_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_combine.py` & `DuHast-0.0.8/src/duHast/Utilities/files_combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_csv.py` & `DuHast-0.0.8/src/duHast/Utilities/files_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_get.py` & `DuHast-0.0.8/src/duHast/Utilities/files_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_io.py` & `DuHast-0.0.8/src/duHast/Utilities/files_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_json.py` & `DuHast-0.0.8/src/duHast/Utilities/files_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/files_tab.py` & `DuHast-0.0.8/src/duHast/Utilities/files_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/padding.py` & `DuHast-0.0.8/src/duHast/Utilities/padding.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/solibri_ifc_optimizer.py` & `DuHast-0.0.8/src/duHast/Utilities/solibri_ifc_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/system_process.py` & `DuHast-0.0.8/src/duHast/Utilities/system_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/unit_conversion.py` & `DuHast-0.0.8/src/duHast/Utilities/unit_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/util_batch_p.py` & `DuHast-0.0.8/src/duHast/Utilities/util_batch_p.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/utility.py` & `DuHast-0.0.8/src/duHast/Utilities/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DuHast-0.0.7/src/duHast/Utilities/worksharing_monitor_process.py` & `DuHast-0.0.8/src/duHast/Utilities/worksharing_monitor_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright © 2023, Jan Christel
+# Copyright 2023, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

