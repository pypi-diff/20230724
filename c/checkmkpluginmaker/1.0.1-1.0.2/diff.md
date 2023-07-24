# Comparing `tmp/checkmkpluginmaker-1.0.1.tar.gz` & `tmp/checkmkpluginmaker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmkpluginmaker-1.0.1.tar", max compression
+gzip compressed data, was "checkmkpluginmaker-1.0.2.tar", max compression
```

## Comparing `checkmkpluginmaker-1.0.1.tar` & `checkmkpluginmaker-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      335 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/README.md
--rw-r--r--   0        0        0      556 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      806 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
--rw-r--r--   0        0        0     1472 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      327 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
--rw-r--r--   0        0        0     1811 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     1175 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     4063 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     1058 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
--rw-r--r--   0        0        0      848 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
--rw-r--r--   0        0        0     1888 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
--rw-r--r--   0        0        0     1128 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 checkmkpluginmaker-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/README.md
+-rw-r--r--   0        0        0      556 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
+-rw-r--r--   0        0        0     1472 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      327 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
+-rw-r--r--   0        0        0     1811 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     1175 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     4063 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     1058 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
+-rw-r--r--   0        0        0      848 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
+-rw-r--r--   0        0        0     1888 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
+-rw-r--r--   0        0        0     1128 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 checkmkpluginmaker-1.0.2/PKG-INFO
```

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/__init__.py` & `checkmkpluginmaker-1.0.2/pluginmaker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Entry point of my coca tools
 """
 import os
 import sys
 from cookiecutter.main import cookiecutter
 
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('I am , welcome to CheckMK Plugin Maker')
```

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py` & `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.1/pyproject.toml` & `checkmkpluginmaker-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "checkmkpluginmaker"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["NhanDD3 <nhandd3@fpt.com>"]
 readme = "README.md"
 packages = [{include = "pluginmaker"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8"
 pre-commit = "^3.2.2"
 pylint = {extras = ["spelling"], version = "^2.17.2"}
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 bump2version = "^1.0.1"
 mkdocs = "^1.4.2"
 mkdocstrings = "^0.21.2"
```

### Comparing `checkmkpluginmaker-1.0.1/PKG-INFO` & `checkmkpluginmaker-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: checkmkpluginmaker
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: NhanDD3
 Author-email: nhandd3@fpt.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bump2version (>=1.0.1,<2.0.0)
 Requires-Dist: cookiecutter (>=2.2.3,<3.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0)
 Requires-Dist: mkdocs-glightbox (>=0.3.2,<0.4.0)
 Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
```

