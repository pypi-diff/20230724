# Comparing `tmp/d_geolib-1.0.1.tar.gz` & `tmp/d_geolib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_geolib-1.0.1.tar", max compression
+gzip compressed data, was "d_geolib-1.1.0.tar", max compression
```

## Comparing `d_geolib-1.0.1.tar` & `d_geolib-1.1.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0       97 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/__init__.py
--rw-r--r--   0        0        0      631 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/errors.py
--rw-r--r--   0        0        0       86 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/geometry/__init__.py
--rw-r--r--   0        0        0     1023 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/geometry/one.py
--rw-r--r--   0        0        0      510 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/models/__init__.py
--rw-r--r--   0        0        0    11570 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/models/base_model.py
--rw-r--r--   0        0        0      749 2023-06-14 13:51:06.904396 d_geolib-1.0.1/geolib/models/base_model_structure.py
--rw-r--r--   0        0        0      109 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/__init__.py
--rw-r--r--   0        0        0    12325 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_model.py
--rw-r--r--   0        0        0     1619 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_parserprovider.py
--rw-r--r--   0        0        0     3539 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_structures.py
--rw-r--r--   0        0        0    27768 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/internal.py
--rw-r--r--   0        0        0     3020 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/internal_soil.py
--rw-r--r--   0        0        0    19272 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/piles.py
--rw-r--r--   0        0        0     3958 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/profiles.py
--rw-r--r--   0        0        0      603 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/serializer.py
--rw-r--r--   0        0        0     4350 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
--rw-r--r--   0        0        0     4337 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
--rw-r--r--   0        0        0    27924 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dfoundations/templates/input.foi.j2
--rw-r--r--   0        0        0      114 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/__init__.py
--rw-r--r--   0        0        0    16831 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/dgeoflow_model.py
--rw-r--r--   0        0        0     4275 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/dgeoflow_parserprovider.py
--rw-r--r--   0        0        0      333 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/dgeoflow_validator.py
--rw-r--r--   0        0        0    31320 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/internal.py
--rw-r--r--   0        0        0     3513 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/serializer.py
--rw-r--r--   0        0        0      581 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dgeoflow/utils.py
--rw-r--r--   0        0        0    54527 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dseries_parser.py
--rw-r--r--   0        0        0      106 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/__init__.py
--rw-r--r--   0        0        0      301 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/drain_types.py
--rw-r--r--   0        0        0     5529 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/drains.py
--rw-r--r--   0        0        0    21412 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_model.py
--rw-r--r--   0        0        0     1518 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_parserprovider.py
--rw-r--r--   0        0        0     7147 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_structures.py
--rw-r--r--   0        0        0    34035 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/internal.py
--rw-r--r--   0        0        0     5500 2023-06-14 13:51:06.920017 d_geolib-1.0.1/geolib/models/dsettlement/internal_soil.py
--rw-r--r--   0        0        0     5960 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsettlement/loads.py
--rw-r--r--   0        0        0      233 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsettlement/probabilistic_calculation_types.py
--rw-r--r--   0        0        0      559 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsettlement/serializer.py
--rw-r--r--   0        0        0    18393 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsettlement/templates/input.sli.j2
--rw-r--r--   0        0        0     4965 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsettlement/templates/soil_template.j2
--rw-r--r--   0        0        0      110 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/__init__.py
--rw-r--r--   0        0        0    11250 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/calculation_options.py
--rw-r--r--   0        0        0    21608 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/constructions.py
--rw-r--r--   0        0        0    19431 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_model.py
--rw-r--r--   0        0        0     1528 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
--rw-r--r--   0        0        0     4647 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_structures.py
--rw-r--r--   0        0        0     3841 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_validator.py
--rw-r--r--   0        0        0    53609 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/internal.py
--rw-r--r--   0        0        0    15559 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/internal_partial_factors.py
--rw-r--r--   0        0        0     9894 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/loads.py
--rw-r--r--   0        0        0     1726 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/profiles.py
--rw-r--r--   0        0        0      561 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/serializer.py
--rw-r--r--   0        0        0     5062 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/settings.py
--rw-r--r--   0        0        0     3465 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/supports.py
--rw-r--r--   0        0        0     1700 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/surface.py
--rw-r--r--   0        0        0    35235 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/templates/input.shi.j2
--rw-r--r--   0        0        0      462 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dsheetpiling/water_level.py
--rw-r--r--   0        0        0      118 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dstability/__init__.py
--rw-r--r--   0        0        0    12506 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dstability/analysis.py
--rw-r--r--   0        0        0    36730 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dstability/dstability_model.py
--rw-r--r--   0        0        0     4189 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dstability/dstability_parserprovider.py
--rw-r--r--   0        0        0     2865 2023-06-14 13:51:06.935645 d_geolib-1.0.1/geolib/models/dstability/dstability_validator.py
--rw-r--r--   0        0        0    90749 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/internal.py
--rw-r--r--   0        0        0     2528 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/loads.py
--rw-r--r--   0        0        0     3435 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/reinforcements.py
--rw-r--r--   0        0        0     3525 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/serializer.py
--rw-r--r--   0        0        0     3331 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/states.py
--rw-r--r--   0        0        0      581 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/dstability/utils.py
--rw-r--r--   0        0        0      142 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/internal.py
--rw-r--r--   0        0        0     1781 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/meta.py
--rw-r--r--   0        0        0       89 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/model_enums.py
--rw-r--r--   0        0        0     1821 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/parsers.py
--rw-r--r--   0        0        0      840 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/serializers.py
--rw-r--r--   0        0        0     2433 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/utils.py
--rw-r--r--   0        0        0      314 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/models/validators.py
--rw-r--r--   0        0        0       55 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/service/__init__.py
--rw-r--r--   0        0        0     5849 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/service/main.py
--rw-r--r--   0        0        0      546 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/service/README.md
--rw-r--r--   0        0        0      797 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/soils/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/soils/layers.py
--rw-r--r--   0        0        0      592 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/soils/library.py
--rw-r--r--   0        0        0    37608 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/soils/soil.py
--rw-r--r--   0        0        0      775 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/soils/soil_utils.py
--rw-r--r--   0        0        0     1574 2023-06-14 13:51:06.951268 d_geolib-1.0.1/geolib/utils.py
--rw-r--r--   0        0        0     1086 2023-06-14 13:51:06.888769 d_geolib-1.0.1/LICENSE
--rw-r--r--   0        0        0     2018 2023-06-14 13:51:06.951268 d_geolib-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2955 2023-06-14 13:51:06.888769 d_geolib-1.0.1/README.rst
--rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 d_geolib-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/__init__.py
+-rw-r--r--   0        0        0      631 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/errors.py
+-rw-r--r--   0        0        0       86 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/geometry/__init__.py
+-rw-r--r--   0        0        0     1023 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/geometry/one.py
+-rw-r--r--   0        0        0      510 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/__init__.py
+-rw-r--r--   0        0        0    11570 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/base_model.py
+-rw-r--r--   0        0        0      749 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/base_model_structure.py
+-rw-r--r--   0        0        0      109 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/__init__.py
+-rw-r--r--   0        0        0    12325 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_model.py
+-rw-r--r--   0        0        0     1619 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_parserprovider.py
+-rw-r--r--   0        0        0     3539 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_structures.py
+-rw-r--r--   0        0        0    27768 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/internal.py
+-rw-r--r--   0        0        0     3020 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/internal_soil.py
+-rw-r--r--   0        0        0    19272 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/piles.py
+-rw-r--r--   0        0        0     3958 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/profiles.py
+-rw-r--r--   0        0        0      603 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/serializer.py
+-rw-r--r--   0        0        0     4350 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
+-rw-r--r--   0        0        0     4337 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
+-rw-r--r--   0        0        0    27924 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/templates/input.foi.j2
+-rw-r--r--   0        0        0      114 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/__init__.py
+-rw-r--r--   0        0        0    16831 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_model.py
+-rw-r--r--   0        0        0     4275 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
+-rw-r--r--   0        0        0      333 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_validator.py
+-rw-r--r--   0        0        0    31320 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/internal.py
+-rw-r--r--   0        0        0     3513 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dgeoflow/serializer.py
+-rw-r--r--   0        0        0      581 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dgeoflow/utils.py
+-rw-r--r--   0        0        0    54527 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dseries_parser.py
+-rw-r--r--   0        0        0      106 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/drain_types.py
+-rw-r--r--   0        0        0     5529 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/drains.py
+-rw-r--r--   0        0        0    21412 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_model.py
+-rw-r--r--   0        0        0     1518 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_parserprovider.py
+-rw-r--r--   0        0        0     7147 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_structures.py
+-rw-r--r--   0        0        0    34035 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/internal.py
+-rw-r--r--   0        0        0     5500 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/internal_soil.py
+-rw-r--r--   0        0        0     5960 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/loads.py
+-rw-r--r--   0        0        0      233 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/probabilistic_calculation_types.py
+-rw-r--r--   0        0        0      559 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/serializer.py
+-rw-r--r--   0        0        0    18393 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/templates/input.sli.j2
+-rw-r--r--   0        0        0     4965 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/templates/soil_template.j2
+-rw-r--r--   0        0        0      110 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/__init__.py
+-rw-r--r--   0        0        0    11250 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/calculation_options.py
+-rw-r--r--   0        0        0    21608 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/constructions.py
+-rw-r--r--   0        0        0    19431 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_model.py
+-rw-r--r--   0        0        0     1528 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
+-rw-r--r--   0        0        0     4647 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
+-rw-r--r--   0        0        0     3841 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
+-rw-r--r--   0        0        0    53609 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/internal.py
+-rw-r--r--   0        0        0    15559 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/internal_partial_factors.py
+-rw-r--r--   0        0        0     9894 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/loads.py
+-rw-r--r--   0        0        0     1726 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/profiles.py
+-rw-r--r--   0        0        0      561 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/serializer.py
+-rw-r--r--   0        0        0     5062 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/settings.py
+-rw-r--r--   0        0        0     3465 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/supports.py
+-rw-r--r--   0        0        0     1700 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/surface.py
+-rw-r--r--   0        0        0    35235 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/templates/input.shi.j2
+-rw-r--r--   0        0        0      462 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/water_level.py
+-rw-r--r--   0        0        0      118 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/__init__.py
+-rw-r--r--   0        0        0    12506 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/analysis.py
+-rw-r--r--   0        0        0    36730 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_model.py
+-rw-r--r--   0        0        0     4189 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_parserprovider.py
+-rw-r--r--   0        0        0     2865 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_validator.py
+-rw-r--r--   0        0        0    90867 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/internal.py
+-rw-r--r--   0        0        0     2931 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/loads.py
+-rw-r--r--   0        0        0     3435 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/reinforcements.py
+-rw-r--r--   0        0        0     3525 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/serializer.py
+-rw-r--r--   0        0        0     3331 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/states.py
+-rw-r--r--   0        0        0      581 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/utils.py
+-rw-r--r--   0        0        0      142 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/internal.py
+-rw-r--r--   0        0        0     1781 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/meta.py
+-rw-r--r--   0        0        0       89 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/model_enums.py
+-rw-r--r--   0        0        0     1821 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/parsers.py
+-rw-r--r--   0        0        0      840 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/serializers.py
+-rw-r--r--   0        0        0     2433 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/utils.py
+-rw-r--r--   0        0        0      314 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/validators.py
+-rw-r--r--   0        0        0       55 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/__init__.py
+-rw-r--r--   0        0        0     5849 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/main.py
+-rw-r--r--   0        0        0      546 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/README.md
+-rw-r--r--   0        0        0      797 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/__init__.py
+-rw-r--r--   0        0        0     1720 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/layers.py
+-rw-r--r--   0        0        0      592 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/library.py
+-rw-r--r--   0        0        0    37608 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/soil.py
+-rw-r--r--   0        0        0      775 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/soil_utils.py
+-rw-r--r--   0        0        0     1574 2023-07-24 14:30:47.452890 d_geolib-1.1.0/geolib/utils.py
+-rw-r--r--   0        0        0     1086 2023-07-24 14:30:47.374791 d_geolib-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2013 2023-07-24 14:30:47.452890 d_geolib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2955 2023-07-24 14:30:47.374791 d_geolib-1.1.0/README.rst
+-rw-r--r--   0        0        0     4037 1970-01-01 00:00:00.000000 d_geolib-1.1.0/PKG-INFO
```

### Comparing `d_geolib-1.0.1/geolib/errors.py` & `d_geolib-1.1.0/geolib/errors.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/geometry/one.py` & `d_geolib-1.1.0/geolib/geometry/one.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/base_model.py` & `d_geolib-1.1.0/geolib/models/base_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/base_model_structure.py` & `d_geolib-1.1.0/geolib/models/base_model_structure.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_model.py` & `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_parserprovider.py` & `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/dfoundations_structures.py` & `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/internal.py` & `d_geolib-1.1.0/geolib/models/dfoundations/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/internal_soil.py` & `d_geolib-1.1.0/geolib/models/dfoundations/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/piles.py` & `d_geolib-1.1.0/geolib/models/dfoundations/piles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/profiles.py` & `d_geolib-1.1.0/geolib/models/dfoundations/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/serializer.py` & `d_geolib-1.1.0/geolib/models/dfoundations/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv` & `d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv` & `d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dfoundations/templates/input.foi.j2` & `d_geolib-1.1.0/geolib/models/dfoundations/templates/input.foi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dgeoflow/dgeoflow_model.py` & `d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dgeoflow/dgeoflow_parserprovider.py` & `d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dgeoflow/internal.py` & `d_geolib-1.1.0/geolib/models/dgeoflow/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dgeoflow/serializer.py` & `d_geolib-1.1.0/geolib/models/dgeoflow/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dgeoflow/utils.py` & `d_geolib-1.1.0/geolib/models/dgeoflow/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dseries_parser.py` & `d_geolib-1.1.0/geolib/models/dseries_parser.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/drains.py` & `d_geolib-1.1.0/geolib/models/dsettlement/drains.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_model.py` & `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_parserprovider.py` & `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/dsettlement_structures.py` & `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/internal.py` & `d_geolib-1.1.0/geolib/models/dsettlement/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/internal_soil.py` & `d_geolib-1.1.0/geolib/models/dsettlement/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/loads.py` & `d_geolib-1.1.0/geolib/models/dsettlement/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/serializer.py` & `d_geolib-1.1.0/geolib/models/dsettlement/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/templates/input.sli.j2` & `d_geolib-1.1.0/geolib/models/dsettlement/templates/input.sli.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsettlement/templates/soil_template.j2` & `d_geolib-1.1.0/geolib/models/dsettlement/templates/soil_template.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/calculation_options.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/calculation_options.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/constructions.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/constructions.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_model.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_structures.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/dsheetpiling_validator.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/internal.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/internal_partial_factors.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/internal_partial_factors.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/loads.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/profiles.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/serializer.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/settings.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/settings.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/supports.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/supports.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/surface.py` & `d_geolib-1.1.0/geolib/models/dsheetpiling/surface.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dsheetpiling/templates/input.shi.j2` & `d_geolib-1.1.0/geolib/models/dsheetpiling/templates/input.shi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/analysis.py` & `d_geolib-1.1.0/geolib/models/dstability/analysis.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/dstability_model.py` & `d_geolib-1.1.0/geolib/models/dstability/dstability_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/dstability_parserprovider.py` & `d_geolib-1.1.0/geolib/models/dstability/dstability_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/dstability_validator.py` & `d_geolib-1.1.0/geolib/models/dstability/dstability_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/internal.py` & `d_geolib-1.1.0/geolib/models/dstability/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1092,26 +1092,28 @@
     LayerLoads: Optional[List[Optional[PersistableLayerLoad]]] = []
     LineLoads: Optional[List[Optional[PersistableLineLoad]]] = []
     Trees: Optional[List[Optional[PersistableTree]]] = []
     UniformLoads: Optional[List[Optional[PersistableUniformLoad]]] = []
 
     def add_load(
         self, load: "DStabilityLoad", consolidations: List["Consolidation"]
-    ) -> Union[PersistableUniformLoad, PersistableLineLoad, PersistableLayerLoad]:
+    ) -> Union[PersistableUniformLoad, PersistableLineLoad, PersistableLayerLoad, PersistableTree]:
         internal_datastructure = load.to_internal_datastructure()
 
         # Add consolidations if the load supports it
         if hasattr(internal_datastructure, "Consolidations"):
             internal_datastructure.Consolidations = [
                 c.to_internal_datastructure() for c in consolidations
             ]
 
         target = load.__class__.__name__
         if target == "Earthquake":
             setattr(self, target, internal_datastructure)
+        if target == "TreeLoad":
+            getattr(self, "Trees").append(internal_datastructure)
         else:
             target += "s"
             getattr(self, target).append(internal_datastructure)
 
         return internal_datastructure
 
     def add_layer_load(
```

### Comparing `d_geolib-1.0.1/geolib/models/dstability/loads.py` & `d_geolib-1.1.0/geolib/models/dstability/loads.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from geolib.models import BaseDataClass
 
 from ...geometry.one import Point
 from .internal import (
     PersistableConsolidation,
     PersistableLineLoad,
     PersistablePoint,
+    PersistableTree,
     PersistableUniformLoad,
 )
 
 
 class DStabilityLoad(BaseDataClass):
     """Base Class for Loads."""
 
@@ -76,19 +77,28 @@
             Spread=self.angle_of_distribution,
         )
 
 
 class TreeLoad(DStabilityLoad):
     """Inherits :class:`~geolib.models.dstability.loads.DStabilityLoad`."""
 
-    height: float
+    tree_top_location: Point
     wind_force: float
     width_of_root_zone: float
     angle_of_distribution: float
 
+    def to_internal_datastructure(self) -> PersistableTree:
+        return PersistableTree(
+            Label=self.label,
+            Location=PersistablePoint(X=self.tree_top_location.x, Z=self.tree_top_location.z),
+            Force=self.wind_force,
+            RootZoneWidth=self.width_of_root_zone,
+            Spread=self.angle_of_distribution,
+        )
+
 
 class Earthquake(DStabilityLoad):
     """Inherits :class:`~geolib.models.dstability.loads.DStabilityLoad`."""
 
     horizontal_factor: float
     vertical_factor: float
     free_water_factor: float
```

### Comparing `d_geolib-1.0.1/geolib/models/dstability/reinforcements.py` & `d_geolib-1.1.0/geolib/models/dstability/reinforcements.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/serializer.py` & `d_geolib-1.1.0/geolib/models/dstability/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/states.py` & `d_geolib-1.1.0/geolib/models/dstability/states.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/dstability/utils.py` & `d_geolib-1.1.0/geolib/models/dstability/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/meta.py` & `d_geolib-1.1.0/geolib/models/meta.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/parsers.py` & `d_geolib-1.1.0/geolib/models/parsers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/serializers.py` & `d_geolib-1.1.0/geolib/models/serializers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/models/utils.py` & `d_geolib-1.1.0/geolib/models/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/service/main.py` & `d_geolib-1.1.0/geolib/service/main.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/service/README.md` & `d_geolib-1.1.0/geolib/service/README.md`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/soils/__init__.py` & `d_geolib-1.1.0/geolib/soils/__init__.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/soils/layers.py` & `d_geolib-1.1.0/geolib/soils/layers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/soils/library.py` & `d_geolib-1.1.0/geolib/soils/library.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/soils/soil.py` & `d_geolib-1.1.0/geolib/soils/soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/soils/soil_utils.py` & `d_geolib-1.1.0/geolib/soils/soil_utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/geolib/utils.py` & `d_geolib-1.1.0/geolib/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/LICENSE` & `d_geolib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/pyproject.toml` & `d_geolib-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "d-geolib"
-version = "1.0.1"
+version = "1.1.0"
 description = "Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models"
 authors = ["Maarten Pronk <maarten.pronk@deltares.nl>", "Deltares"]
 license = "MIT"
 homepage = "https://deltares.github.io/GEOLib/"
 documentation = "https://deltares.github.io/GEOLib/"
 repository = "https://github.com/Deltares/GEOLib"
 readme = "README.rst"
 packages = [
     {include = "geolib"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-pydantic = {version = "^1.10.7", extras = ["dotenv"]}
+pydantic = "^1.10.7"
 zipp = "^3.15.0"
 fastapi = {version = "^0.95.1", optional = true}
 uvicorn = {version = "^0.21.1", optional = true}
 requests = "^2.29.0"
 jinja2 = "^3.1.2"
 httpx = {version = "^0.24.0", optional = true}
 starlette = "^0.26.1"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 teamcity-messages = "^1.32"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 devtools = "^0.11.0"
 pytest = "^7.3.1"
@@ -67,15 +68,15 @@
 force_grid_wrap=0
 use_parentheses=true
 line_length=90
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
+version = "1.1.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:^version",
     "tests/test_geolib.py",
     "geolib/__init__.py:__version__",
 ]
-annotated_tag = true
+annotated_tag = true
```

### Comparing `d_geolib-1.0.1/README.rst` & `d_geolib-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `d_geolib-1.0.1/PKG-INFO` & `d_geolib-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-geolib
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models
 Home-page: https://deltares.github.io/GEOLib/
 License: MIT
 Author: Maarten Pronk
 Author-email: maarten.pronk@deltares.nl
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: server
 Requires-Dist: fastapi (>=0.95.1,<0.96.0) ; extra == "server"
 Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "server"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "server"
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0) ; extra == "server"
 Requires-Dist: zipp (>=3.15.0,<4.0.0)
 Project-URL: Documentation, https://deltares.github.io/GEOLib/
 Project-URL: Repository, https://github.com/Deltares/GEOLib
 Description-Content-Type: text/x-rst
```

