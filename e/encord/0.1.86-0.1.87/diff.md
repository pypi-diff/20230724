# Comparing `tmp/encord-0.1.86.tar.gz` & `tmp/encord-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.86.tar", max compression
+gzip compressed data, was "encord-0.1.87.tar", max compression
```

## Comparing `encord-0.1.86.tar` & `encord-0.1.87.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    11330 2023-07-13 14:46:40.427879 encord-0.1.86/LICENSE
--rw-r--r--   0        0        0     2030 2023-07-13 14:46:40.427879 encord-0.1.86/README.md
--rw-r--r--   0        0        0      158 2023-07-13 14:46:40.447879 encord-0.1.86/encord/__init__.py
--rw-r--r--   0        0        0      100 2023-07-13 14:46:40.447879 encord-0.1.86/encord/_version.py
--rw-r--r--   0        0        0    49616 2023-07-13 14:46:40.447879 encord-0.1.86/encord/client.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/__init__.py
--rw-r--r--   0        0        0       45 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/constants.py
--rw-r--r--   0        0        0      508 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/enum.py
--rw-r--r--   0        0        0    10852 2023-07-13 14:46:40.447879 encord-0.1.86/encord/configs.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/enums.py
--rw-r--r--   0        0        0     3196 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/model.py
--rw-r--r--   0        0        0     4522 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-07-13 14:46:40.447879 encord-0.1.86/encord/dataset.py
--rw-r--r--   0        0        0     6355 2023-07-13 14:46:40.447879 encord-0.1.86/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/bundle.py
--rw-r--r--   0        0        0      319 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/common.py
--rw-r--r--   0        0        0      535 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/limits.py
--rw-r--r--   0        0        0     7886 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/querier.py
--rw-r--r--   0        0        0      747 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/query_methods.py
--rw-r--r--   0        0        0     1738 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/utils.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/__init__.py
--rw-r--r--   0        0        0     3447 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/api_client.py
--rw-r--r--   0        0        0      964 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/error_utils.py
--rw-r--r--   0        0        0      216 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/payloads.py
--rw-r--r--   0        0        0     2249 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/request_signer.py
--rw-r--r--   0        0        0      340 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/classification.py
--rw-r--r--   0        0        0    21796 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/frames.py
--rw-r--r--   0        0        0    22033 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   140628 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/project.py
--rw-r--r--   0        0        0     1622 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-07-13 14:46:40.451879 encord-0.1.86/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/__init__.py
--rw-r--r--   0        0        0      932 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/analytics.py
--rw-r--r--   0        0        0      982 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/api_key.py
--rw-r--r--   0        0        0      486 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/__init__.py
--rw-r--r--   0        0        0      337 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_interface.py
--rw-r--r--   0        0        0     1418 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v1.py
--rw-r--r--   0        0        0     1366 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v2.py
--rw-r--r--   0        0        0     5335 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32989 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/dataset.py
--rw-r--r--   0        0        0      829 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      256 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/formatter.py
--rw-r--r--   0        0        0     1241 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6667 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/model.py
--rw-r--r--   0        0        0      874 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/ontology.py
--rw-r--r--   0        0        0     8658 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/workflow.py
--rw-r--r--   0        0        0    41332 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    29036 2023-07-13 14:46:40.451879 encord-0.1.86/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1989 2023-07-13 14:46:40.451879 encord-0.1.86/pyproject.toml
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 encord-0.1.86/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-07-24 15:47:37.430500 encord-0.1.87/LICENSE
+-rw-r--r--   0        0        0     2027 2023-07-24 15:47:37.430500 encord-0.1.87/README.md
+-rw-r--r--   0        0        0      158 2023-07-24 15:47:37.446500 encord-0.1.87/encord/__init__.py
+-rw-r--r--   0        0        0      100 2023-07-24 15:47:37.446500 encord-0.1.87/encord/_version.py
+-rw-r--r--   0        0        0    49616 2023-07-24 15:47:37.446500 encord-0.1.87/encord/client.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/constants.py
+-rw-r--r--   0        0        0      508 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/enum.py
+-rw-r--r--   0        0        0    10852 2023-07-24 15:47:37.446500 encord-0.1.87/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16021 2023-07-24 15:47:37.446500 encord-0.1.87/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-07-24 15:47:37.446500 encord-0.1.87/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/common.py
+-rw-r--r--   0        0        0      535 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/limits.py
+-rw-r--r--   0        0        0     7886 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     3388 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0      964 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      223 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2249 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      340 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/classification.py
+-rw-r--r--   0        0        0    21796 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/frames.py
+-rw-r--r--   0        0        0    22033 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   140628 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/project.py
+-rw-r--r--   0        0        0     1622 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-07-24 15:47:37.446500 encord-0.1.87/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/api_key.py
+-rw-r--r--   0        0        0      486 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1418 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1481 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5335 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32993 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1241 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6667 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/model.py
+-rw-r--r--   0        0        0      874 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8658 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41332 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29036 2023-07-24 15:47:37.450501 encord-0.1.87/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1989 2023-07-24 15:47:37.450501 encord-0.1.87/pyproject.toml
+-rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 encord-0.1.87/PKG-INFO
```

### Comparing `encord-0.1.86/LICENSE` & `encord-0.1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/README.md` & `encord-0.1.87/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 First, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
 
 ```bash
 pip install encord
 ```
 
 Then, generate an public-private key pair, and upload the public key to [Encord website](https://www.encord.com/).
-Detailed guide can be found in the [dedicated manual](https://docs.encord.com/admins/settings/public-keys/).
+Detailed guide can be found in the [dedicated manual](https://docs.encord.com/docs/annotate-public-keys).
 
 Passing the private key to the factory, you can initialise the Encord client directly.
 
 ```python
 from encord import EncordUserClient
 
 user_client = EncordUserClient.create_with_ssh_private_key(
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
 Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
 //app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
 Getting Started For full documentation, please visit [Encord Python SDK](https:
 //python.docs.encord.com/). First, install Encord Python API Client using the
 [pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
 install encord ``` Then, generate an public-private key pair, and upload the
 public key to [Encord website](https://www.encord.com/). Detailed guide can be
-found in the [dedicated manual](https://docs.encord.com/admins/settings/public-
-keys/). Passing the private key to the factory, you can initialise the Encord
+found in the [dedicated manual](https://docs.encord.com/docs/annotate-public-
+keys). Passing the private key to the factory, you can initialise the Encord
 client directly. ```python from encord import EncordUserClient user_client =
 EncordUserClient.create_with_ssh_private_key( "", password="", ) ``` Once you
 have instantiated an Encord client, it is easy to fetch a project information
 and start working with the platform. ```py project = user_client.get_project
 ("") label_rows = project.list_label_rows_v2() ``` For detailed examples and
 API reference please refer to [Encord SDK documentation](https://
 python.docs.encord.com/) ## ð Troubleshooting Please report bugs to the
```

### Comparing `encord-0.1.86/encord/client.py` & `encord-0.1.87/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/configs.py` & `encord-0.1.87/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/constants/enums.py` & `encord-0.1.87/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/constants/model.py` & `encord-0.1.87/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/constants/model_weights.py` & `encord-0.1.87/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/constants/string_constants.py` & `encord-0.1.87/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/constants/test/test_enums.py` & `encord-0.1.87/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/dataset.py` & `encord-0.1.87/encord/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         file_path: Union[Path, str],
         title: Optional[str] = None,
         cloud_upload_settings: CloudUploadSettings = CloudUploadSettings(),
     ) -> Image:
         """
         Upload a single image to Encord storage. If your images are sequential we recommend creating an image group via
         the :meth:`.Dataset.create_image_group` function. For more information please compare
-        https://docs.encord.com/docs/annotate/editor/images and https://docs.encord.com/docs/annotate/editor/videos
+        https://docs.encord.com/docs/annotate-images and https://docs.encord.com/docs/annotate-videos
 
         Args:
             file_path: The file path to the image
             title: The image title. If unspecified, this will be the file name. This title should include an extension.
                 For example "encord_image.png".
             cloud_upload_settings:
                 Settings for uploading data into the cloud. Change this object to overwrite the default values.
```

### Comparing `encord-0.1.86/encord/exceptions.py` & `encord-0.1.87/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/bundle.py` & `encord-0.1.87/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/constants.py` & `encord-0.1.87/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/error_utils.py` & `encord-0.1.87/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/querier.py` & `encord-0.1.87/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/query_methods.py` & `encord-0.1.87/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/request.py` & `encord-0.1.87/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/utils.py` & `encord-0.1.87/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/v2/api_client.py` & `encord-0.1.87/encord/http/v2/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import platform
 from pathlib import Path
 from typing import Optional, Type, TypeVar
 from urllib.parse import urljoin
 
 import requests
 from requests import Response
-from requests.exceptions import JSONDecodeError
 
 from encord._version import __version__ as encord_version
 from encord.configs import UserConfig
 from encord.exceptions import RequestException
 from encord.http.common import (
     HEADER_CLOUD_TRACE_CONTEXT,
     HEADER_USER_AGENT,
@@ -84,9 +83,9 @@
             return result_type.from_dict(res_json)
 
     @staticmethod
     def _handle_error(response: Response, context: RequestContext):
         try:
             description = response.json()
             handle_error_response(response.status_code, context=context, message=description["message"])
-        except JSONDecodeError as e:
+        except Exception:
             handle_error_response(response.status_code, context=context)
```

### Comparing `encord-0.1.86/encord/http/v2/error_utils.py` & `encord-0.1.87/encord/http/v2/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/http/v2/request_signer.py` & `encord-0.1.87/encord/http/v2/request_signer.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/bitmask.py` & `encord-0.1.87/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/common.py` & `encord-0.1.87/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/coordinates.py` & `encord-0.1.87/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/frames.py` & `encord-0.1.87/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/internal_helpers.py` & `encord-0.1.87/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/ontology_labels_impl.py` & `encord-0.1.87/encord/objects/ontology_labels_impl.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/project.py` & `encord-0.1.87/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/objects/utils.py` & `encord-0.1.87/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/ontology.py` & `encord-0.1.87/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/analytics.py` & `encord-0.1.87/encord/orm/analytics.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/api_key.py` & `encord-0.1.87/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v1.py` & `encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v2.py` & `encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import Any, Dict, Type, TypeVar
 
+# TODO: invent some dependency version dependent type checking to get rid of this ignore
+from pydantic import ConfigDict  # type: ignore[attr-defined]
 from pydantic import BaseModel, ValidationError
 
 from encord.exceptions import EncordException
 from encord.objects.utils import _snake_to_camel
 from encord.orm.base_dto.base_dto_interface import BaseDTOInterface, T
 
 
 class BaseDTO(BaseDTOInterface, BaseModel):
-    class Config:
-        allow_extra = True
-        populate_by_name = True
-        alias_generator = _snake_to_camel
+    model_config = ConfigDict(extra="allow", populate_by_name=True, alias_generator=_snake_to_camel)
 
     @classmethod
     def from_dict(cls: Type[T], d: Dict[str, Any]) -> T:
         try:
             return cls.model_validate(d)  # type: ignore[attr-defined]
         except ValidationError as e:
             raise EncordException(message=str(e)) from e
@@ -24,18 +23,15 @@
         return self.model_dump(by_alias=True)  # type: ignore[attr-defined]
 
 
 DataT = TypeVar("DataT")
 
 
 class GenericBaseDTO(BaseDTOInterface, BaseModel):
-    class Config:
-        allow_extra = True
-        populate_by_name = True
-        alias_generator = _snake_to_camel
+    model_config = ConfigDict(extra="allow", populate_by_name=True, alias_generator=_snake_to_camel)
 
     @classmethod
     def from_dict(cls: Type[T], d: Dict[str, Any]) -> T:
         try:
             return cls.model_validate(d)  # type: ignore[attr-defined]
         except ValidationError as e:
             raise EncordException(message=str(e)) from e
```

### Comparing `encord-0.1.86/encord/orm/base_orm.py` & `encord-0.1.87/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/dataset.py` & `encord-0.1.87/encord/orm/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     @property
     def is_image_sequence(self) -> Optional[bool]:
         """
         If the data type is an :meth:`DataType.IMG_GROUP <encord.constants.enums.DataType.IMG_GROUP>`,
         returns whether this is an image sequence. Returns `None` for other data types.
 
         For more details refer to the
-        :ref:`documentation on image sequnces <https://docs.encord.com/datasets/supported-data/#image-sequences>`
+        :ref:`documentation on image sequnces <https://docs.encord.com/docs/annotate-supported-data#image-sequences>`
         """
         return self["is_optimised_image_group"]
 
     def refetch_data(
         self,
         *,
         signed_url: bool = False,
```

### Comparing `encord-0.1.86/encord/orm/dataset_with_user_role.py` & `encord-0.1.87/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/label_log.py` & `encord-0.1.87/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/label_row.py` & `encord-0.1.87/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/labeling_algorithm.py` & `encord-0.1.87/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/model.py` & `encord-0.1.87/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/ontology.py` & `encord-0.1.87/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/project.py` & `encord-0.1.87/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/project_api_key.py` & `encord-0.1.87/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/project_with_user_role.py` & `encord-0.1.87/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/orm/test/test_dataset.py` & `encord-0.1.87/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project.py` & `encord-0.1.87/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project_ontology/classification_attribute.py` & `encord-0.1.87/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project_ontology/classification_option.py` & `encord-0.1.87/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project_ontology/ontology.py` & `encord-0.1.87/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project_ontology/ontology_classification.py` & `encord-0.1.87/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/project_ontology/ontology_object.py` & `encord-0.1.87/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/user_client.py` & `encord-0.1.87/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/utilities/client_utilities.py` & `encord-0.1.87/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/utilities/label_utilities.py` & `encord-0.1.87/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/encord/utilities/project_user.py` & `encord-0.1.87/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.86/pyproject.toml` & `encord-0.1.87/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.86"
+version = "0.1.87"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["encord"]
 packages = [
     { include = "encord"},
 ]
```

### Comparing `encord-0.1.86/PKG-INFO` & `encord-0.1.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.86
+Version: 0.1.87
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.8,<4.0
@@ -54,15 +54,15 @@
 First, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
 
 ```bash
 pip install encord
 ```
 
 Then, generate an public-private key pair, and upload the public key to [Encord website](https://www.encord.com/).
-Detailed guide can be found in the [dedicated manual](https://docs.encord.com/admins/settings/public-keys/).
+Detailed guide can be found in the [dedicated manual](https://docs.encord.com/docs/annotate-public-keys).
 
 Passing the private key to the factory, you can initialise the Encord client directly.
 
 ```python
 from encord import EncordUserClient
 
 user_client = EncordUserClient.create_with_ssh_private_key(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.86 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.87 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -21,16 +21,16 @@
 Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
 //app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
 Getting Started For full documentation, please visit [Encord Python SDK](https:
 //python.docs.encord.com/). First, install Encord Python API Client using the
 [pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
 install encord ``` Then, generate an public-private key pair, and upload the
 public key to [Encord website](https://www.encord.com/). Detailed guide can be
-found in the [dedicated manual](https://docs.encord.com/admins/settings/public-
-keys/). Passing the private key to the factory, you can initialise the Encord
+found in the [dedicated manual](https://docs.encord.com/docs/annotate-public-
+keys). Passing the private key to the factory, you can initialise the Encord
 client directly. ```python from encord import EncordUserClient user_client =
 EncordUserClient.create_with_ssh_private_key( "", password="", ) ``` Once you
 have instantiated an Encord client, it is easy to fetch a project information
 and start working with the platform. ```py project = user_client.get_project
 ("") label_rows = project.list_label_rows_v2() ``` For detailed examples and
 API reference please refer to [Encord SDK documentation](https://
 python.docs.encord.com/) ## ð Troubleshooting Please report bugs to the
```

