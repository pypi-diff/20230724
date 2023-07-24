# Comparing `tmp/pydantic_appconfig-1.0.0.tar.gz` & `tmp/pydantic_appconfig-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_appconfig-1.0.0.tar", max compression
+gzip compressed data, was "pydantic_appconfig-2.0.0.tar", max compression
```

## Comparing `pydantic_appconfig-1.0.0.tar` & `pydantic_appconfig-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/LICENSE
--rw-r--r--   0        0        0     2639 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/README.rst
--rw-r--r--   0        0        0       54 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/pydantic_appconfig/__init__.py
--rw-r--r--   0        0        0     8222 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/pydantic_appconfig/app_config.py
--rw-r--r--   0        0        0        0 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/pydantic_appconfig/py.typed
--rw-r--r--   0        0        0     1511 2022-10-31 11:59:14.450578 pydantic_appconfig-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 pydantic_appconfig-1.0.0/setup.py
--rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 pydantic_appconfig-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3288 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/README.rst
+-rw-r--r--   0        0        0       54 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/pydantic_appconfig/__init__.py
+-rw-r--r--   0        0        0     8222 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/pydantic_appconfig/app_config.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/pydantic_appconfig/py.typed
+-rw-r--r--   0        0        0     1512 2023-07-24 09:52:54.600923 pydantic_appconfig-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 pydantic_appconfig-2.0.0/PKG-INFO
```

### Comparing `pydantic_appconfig-1.0.0/LICENSE` & `pydantic_appconfig-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_appconfig-1.0.0/README.rst` & `pydantic_appconfig-2.0.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 .. image:: https://badge.fury.io/py/pydantic-appconfig.svg
     :target: https://badge.fury.io/py/pydantic-appconfig
 
 .. image:: https://img.shields.io/pypi/pyversions/pydantic-appconfig
     :target: https://img.shields.io/pypi/pyversions/pydantic-appconfig
 
+.. image:: https://app.codacy.com/project/badge/Grade/7394b3a36fca46b38df857c415b3da3d
+    :target: https://www.codacy.com/gh/Validus-Risk-Management/aws-appconfig-pydantic/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Validus-Risk-Management/aws-appconfig-pydantic&amp;utm_campaign=Badge_Grade
+
+.. image:: https://app.codacy.com/project/badge/Coverage/7394b3a36fca46b38df857c415b3da3d
+    :target: https://www.codacy.com/gh/Validus-Risk-Management/aws-appconfig-pydantic/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Validus-Risk-Management/aws-appconfig-pydantic&amp;utm_campaign=Badge_Coverage
 
 Ever wanted to use
 `AWS AppConfig <https://aws.amazon.com/systems-manager/features/appconfig>`_
 for your Python app, but can't bear configs without
 `pydantic <https://pydantic-docs.helpmanual.io/>`_?
 
 Well, your days of using evil `.env` or `.ini` files, `ENVIRONMENT` variables or even custom providers is over!
```

### Comparing `pydantic_appconfig-1.0.0/pydantic_appconfig/app_config.py` & `pydantic_appconfig-2.0.0/pydantic_appconfig/app_config.py`

 * *Files identical despite different names*

### Comparing `pydantic_appconfig-1.0.0/pyproject.toml` & `pydantic_appconfig-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "pydantic_appconfig"
-version = "1.0.0"
+version = "2.0.0"
 description = "Helper package for using AWS App Config with Pydantic"
 include = ["pydantic_appconfig/py.typed"]
 authors = [
         "Validus Tech Team <techteam@validusrm.com>",
         "Fergus Strangways-Dixon <fergusdixon101@gmail.com>",
     ]
 readme = "README.rst"
 repository = "https://github.com/Validus-Risk-Management/aws-appconfig-pydantic"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.20.8"
 botocore = "^1.23.8"
 PyYAML = "^6.0"
-pydantic = "^1.8.2"
+pydantic = "^2.0.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2"
 pytest-mock = "^3.6.1"
 freezegun = "^1.1.0"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.13"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 flake8 = "^3.9"
-isort = "^5.9"
+isort = "^5.12"
 mypy = "^0.910"
 pre-commit = "^2.13"
 flake8-absolute-import = "^1.0"
 flake8-blind-except = "^0.2.0"
 flake8-breakpoint = "^1.1.0"
 flake8-bugbear = "^21.4.3"
 flake8-builtins = "^1.5.3"
@@ -41,15 +41,15 @@
 flake8-eradicate = "^1.1.0"
 flake8-implicit-str-concat = "^0.2.0"
 flake8-mutable = "^1.2.0"
 flake8-print = "^4.0.0"
 flake8-pytest-style = "^1.5.0"
 flake8-simplify = "^0.14.1"
 pep8-naming = "^0.12.1"
-types-PyYAML = "^5.4.10"
+types-PyYAML = "^6.0.12"
 boto3-stubs = "^1.20.8"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `pydantic_appconfig-1.0.0/setup.py` & `pydantic_appconfig-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydantic-appconfig
+Version: 2.0.0
+Summary: Helper package for using AWS App Config with Pydantic
+Home-page: https://github.com/Validus-Risk-Management/aws-appconfig-pydantic
+Author: Validus Tech Team
+Author-email: techteam@validusrm.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: boto3 (>=1.20.8,<2.0.0)
+Requires-Dist: botocore (>=1.23.8,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Project-URL: Repository, https://github.com/Validus-Risk-Management/aws-appconfig-pydantic
+Description-Content-Type: text/x-rst
 
-packages = \
-['pydantic_appconfig']
+Pydantic AWS AppConfig
+=======================
 
-package_data = \
-{'': ['*']}
+.. image:: https://badge.fury.io/py/pydantic-appconfig.svg
+    :target: https://badge.fury.io/py/pydantic-appconfig
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'boto3>=1.20.8,<2.0.0',
- 'botocore>=1.23.8,<2.0.0',
- 'pydantic>=1.8.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pydantic-appconfig',
-    'version': '1.0.0',
-    'description': 'Helper package for using AWS App Config with Pydantic',
-    'long_description': 'Pydantic AWS AppConfig\n=======================\n\n.. image:: https://badge.fury.io/py/pydantic-appconfig.svg\n    :target: https://badge.fury.io/py/pydantic-appconfig\n\n.. image:: https://img.shields.io/pypi/pyversions/pydantic-appconfig\n    :target: https://img.shields.io/pypi/pyversions/pydantic-appconfig\n\n\nEver wanted to use\n`AWS AppConfig <https://aws.amazon.com/systems-manager/features/appconfig>`_\nfor your Python app, but can\'t bear configs without\n`pydantic <https://pydantic-docs.helpmanual.io/>`_?\n\nWell, your days of using evil `.env` or `.ini` files, `ENVIRONMENT` variables or even custom providers is over!\n\nWith just a simple\n\n.. code-block:: shell\n\n    pip install pydantic-appconfig\n\nWith a lot of inspiration from this AWS `sample <https://github.com/aws-samples/sample-python-helper-aws-appconfig>`_.\n\n\nIntroducing `pydantic_appconfig`.\n\n#. Set yourself up with your favourite `pydantic.BaseModel`:\n\n    .. code-block:: python\n\n        class MyAppConfig(pydantic.BaseModel):\n            """My app config."""\n\n            test_field_string: str\n            test_field_int: int\n\n            class Config:\n                """The pydantic config, including title for the JSON schema."""\n\n                title = "MyAppConfig"\n\n#. Set up the config helper using your shiny config class:\n\n    .. code-block:: python\n\n        from pydantic_appconfig import AppConfigHelper\n\n        my_config: AppConfigHelper[MyAppConfig] = AppConfigHelper(\n            appconfig_application="AppConfig-App",\n            appconfig_environment="AppConfig-Env",\n            appconfig_profile="AppConfig-Profile",\n            max_config_age=15,\n            fetch_on_init=True,\n            config_schema_model=MyAppConfig,\n        )\n\n\n#. Use it:\n\n    .. code-block:: python\n\n        my_val = my_config.config.test_field_string\n\n\nAWS AppConfig also has support for `validators <https://docs.aws.amazon.com/appconfig/latest/userguide/appconfig-creating-configuration-and-profile-validators.html>`_.\n\nPydantic is able to generate a JSON schema for you to upload:\n\n   .. code-block:: python\n\n       print(MyAppConfig.schema_json(indent=2))\n\n   .. code-block:: JSON\n\n       {\n         "title": "MyAppConfig",\n         "description": "My app config.",\n         "type": "object",\n         "properties": {\n           "test_field_string": {\n             "title": "Test Field String",\n             "type": "string"\n           },\n           "test_field_int": {\n             "title": "Test Field Int",\n             "type": "integer"\n           }\n         },\n         "required": [\n           "test_field_string",\n           "test_field_int"\n         ]\n       }\n',
-    'author': 'Validus Tech Team',
-    'author_email': 'techteam@validusrm.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Validus-Risk-Management/aws-appconfig-pydantic',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+.. image:: https://img.shields.io/pypi/pyversions/pydantic-appconfig
+    :target: https://img.shields.io/pypi/pyversions/pydantic-appconfig
 
+.. image:: https://app.codacy.com/project/badge/Grade/7394b3a36fca46b38df857c415b3da3d
+    :target: https://www.codacy.com/gh/Validus-Risk-Management/aws-appconfig-pydantic/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Validus-Risk-Management/aws-appconfig-pydantic&amp;utm_campaign=Badge_Grade
+
+.. image:: https://app.codacy.com/project/badge/Coverage/7394b3a36fca46b38df857c415b3da3d
+    :target: https://www.codacy.com/gh/Validus-Risk-Management/aws-appconfig-pydantic/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Validus-Risk-Management/aws-appconfig-pydantic&amp;utm_campaign=Badge_Coverage
+
+Ever wanted to use
+`AWS AppConfig <https://aws.amazon.com/systems-manager/features/appconfig>`_
+for your Python app, but can't bear configs without
+`pydantic <https://pydantic-docs.helpmanual.io/>`_?
+
+Well, your days of using evil `.env` or `.ini` files, `ENVIRONMENT` variables or even custom providers is over!
+
+With just a simple
+
+.. code-block:: shell
+
+    pip install pydantic-appconfig
+
+With a lot of inspiration from this AWS `sample <https://github.com/aws-samples/sample-python-helper-aws-appconfig>`_.
+
+
+Introducing `pydantic_appconfig`.
+
+#. Set yourself up with your favourite `pydantic.BaseModel`:
+
+    .. code-block:: python
+
+        class MyAppConfig(pydantic.BaseModel):
+            """My app config."""
+
+            test_field_string: str
+            test_field_int: int
+
+            class Config:
+                """The pydantic config, including title for the JSON schema."""
+
+                title = "MyAppConfig"
+
+#. Set up the config helper using your shiny config class:
+
+    .. code-block:: python
+
+        from pydantic_appconfig import AppConfigHelper
+
+        my_config: AppConfigHelper[MyAppConfig] = AppConfigHelper(
+            appconfig_application="AppConfig-App",
+            appconfig_environment="AppConfig-Env",
+            appconfig_profile="AppConfig-Profile",
+            max_config_age=15,
+            fetch_on_init=True,
+            config_schema_model=MyAppConfig,
+        )
+
+
+#. Use it:
+
+    .. code-block:: python
+
+        my_val = my_config.config.test_field_string
+
+
+AWS AppConfig also has support for `validators <https://docs.aws.amazon.com/appconfig/latest/userguide/appconfig-creating-configuration-and-profile-validators.html>`_.
+
+Pydantic is able to generate a JSON schema for you to upload:
+
+   .. code-block:: python
+
+       print(MyAppConfig.schema_json(indent=2))
+
+   .. code-block:: JSON
+
+       {
+         "title": "MyAppConfig",
+         "description": "My app config.",
+         "type": "object",
+         "properties": {
+           "test_field_string": {
+             "title": "Test Field String",
+             "type": "string"
+           },
+           "test_field_int": {
+             "title": "Test Field Int",
+             "type": "integer"
+           }
+         },
+         "required": [
+           "test_field_string",
+           "test_field_int"
+         ]
+       }
 
-setup(**setup_kwargs)
```

