# Comparing `tmp/django-pydantic-field-0.2.7.tar.gz` & `tmp/django-pydantic-field-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.2.7.tar", last modified: Mon Jun 19 17:43:59 2023, max compression
+gzip compressed data, was "django-pydantic-field-0.2.8.tar", last modified: Mon Jul 24 08:15:36 2023, max compression
```

## Comparing `django-pydantic-field-0.2.7.tar` & `django-pydantic-field-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.601579 django-pydantic-field-0.2.7/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.601579 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_base_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_django_model_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_drf_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_e2e_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_form_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/django_pydantic_field/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 08:15:36.000000 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-24 08:15:36.000000 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:15:36.000000 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 08:15:36.000000 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 08:15:36.000000 django-pydantic-field-0.2.8/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:15:36.020557 django-pydantic-field-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_base_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_django_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_drf_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-24 08:15:24.000000 django-pydantic-field-0.2.8/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.7/LICENSE` & `django-pydantic-field-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/PKG-INFO` & `django-pydantic-field-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.7
+Version: 0.2.8
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.7/README.md` & `django-pydantic-field-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field/_migration_serializers.py` & `django-pydantic-field-0.2.8/django_pydantic_field/_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field/base.py` & `django-pydantic-field-0.2.8/django_pydantic_field/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import typing as t
 
 import pydantic
 from django.core.serializers.json import DjangoJSONEncoder
-from pydantic.config import get_config, inherit_config
 from pydantic.json import pydantic_encoder
 from pydantic.typing import display_as_type
 
-from .utils import get_local_namespace
+from .utils import get_local_namespace, inherit_configs
 
 __all__ = (
     "SchemaEncoder",
     "SchemaDecoder",
     "wrap_schema",
     "prepare_schema",
     "extract_export_kwargs",
@@ -130,19 +129,13 @@
 
 def _get_field_schema_name(schema) -> str:
     return f"FieldSchema[{display_as_type(schema)}]"
 
 
 def _get_field_schema_params(schema, config=None, allow_null=False, **kwargs) -> dict:
     root_model = t.Optional[schema] if allow_null else schema
-    params: t.Dict[str, t.Any] = dict(kwargs, __root__=(root_model, ...))
-    parent_config = getattr(schema, "Config", None)
-
-    if config is not None:
-        config = get_config(config)
-        if parent_config is not None:
-            config = inherit_config(config, parent_config)
-    else:
-        config = parent_config
-
-    params["__config__"] = config
+    params: t.Dict[str, t.Any] = dict(
+        kwargs,
+        __root__=(root_model, ...),
+        __config__=inherit_configs(schema, config),
+    )
     return params
```

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field/fields.py` & `django-pydantic-field-0.2.8/django_pydantic_field/fields.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field/forms.py` & `django-pydantic-field-0.2.8/django_pydantic_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field/rest_framework.py` & `django-pydantic-field-0.2.8/django_pydantic_field/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field.egg-info/PKG-INFO` & `django-pydantic-field-0.2.8/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.7
+Version: 0.2.8
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.7/django_pydantic_field.egg-info/SOURCES.txt` & `django-pydantic-field-0.2.8/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/pyproject.toml` & `django-pydantic-field-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.2.7"
+version = "0.2.8"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
```

### Comparing `django-pydantic-field-0.2.7/tests/test_base_marshalling.py` & `django-pydantic-field-0.2.8/tests/test_base_marshalling.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/tests/test_django_model_field.py` & `django-pydantic-field-0.2.8/tests/test_django_model_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/tests/test_drf_adapters.py` & `django-pydantic-field-0.2.8/tests/test_drf_adapters.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/tests/test_e2e_models.py` & `django-pydantic-field-0.2.8/tests/test_e2e_models.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/tests/test_form_field.py` & `django-pydantic-field-0.2.8/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.7/tests/test_sample_app_migrations.py` & `django-pydantic-field-0.2.8/tests/test_sample_app_migrations.py`

 * *Files identical despite different names*

