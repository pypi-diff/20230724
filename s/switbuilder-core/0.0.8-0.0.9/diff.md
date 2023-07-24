# Comparing `tmp/switbuilder_core-0.0.8.tar.gz` & `tmp/switbuilder_core-0.0.9.tar.gz`

## Comparing `switbuilder_core-0.0.8.tar` & `switbuilder_core-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.DS_Store
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/build.sh
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/constants.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/logger.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/lokalise.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/__init__.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/activity_router.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/dependencies.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/exceptions.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/constants.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/exception.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/models.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/oauth2.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/repository.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/schemas.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_oauth2.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_path_resolver.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_router.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/build.sh
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    22527 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/constants.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/logger.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/lokalise.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/exception.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/models.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/oauth2.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/schemas.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/tests/test_oauth2.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/tests/test_path_resolver.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/tests/test_router.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/tests/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.9/PKG-INFO
```

### Comparing `switbuilder_core-0.0.8/.DS_Store` & `switbuilder_core-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/requirements.txt` & `switbuilder_core-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/.idea/workspace.xml` & `switbuilder_core-0.0.9/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `switbuilder_core-0.0.8/.idea/workspace.xml` & `switbuilder_core-0.0.9/.idea/workspace.xml`

```diff
@@ -1,15 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="first commit">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/switcore/action/schemas.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/action/schemas.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/switcore/auth/models.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/auth/models.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_path_resolver.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_path_resolver.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -57,15 +60,15 @@
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/switcore"/>
       <recent name="$PROJECT_DIR$/apis/v1"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/switbuilder-core"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.Python tests for test_router.RouterTest.test_router03">
+  <component name="RunManager" selected="Python tests.Python tests for test_oauth2.OAuth2Test">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -95,71 +98,71 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_oauth2.OAuth2Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_path_resolver.PathResolverTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest&quot;"/>
+      <option name="_new_target" value="&quot;test_path_resolver.PathResolverTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest.test_router03" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest.test_router03&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest.test_router_without_view_id" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest.test_router03" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest.test_router_without_view_id&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest.test_router03&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest.test_router_without_view_ids" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest.test_router_without_view_id" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest.test_router_without_view_ids&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest.test_router_without_view_id&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -262,19 +265,19 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router03"/>
+        <item itemvalue="Python tests.Python tests for test_oauth2.OAuth2Test"/>
+        <item itemvalue="Python tests.Python tests for test_path_resolver.PathResolverTest"/>
         <item itemvalue="Python tests.Python tests for test_router.RouterTest"/>
+        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router03"/>
         <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router_without_view_id"/>
-        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router_without_view_ids"/>
-        <item itemvalue="Python tests.Python tests for test_oauth2.OAuth2Test"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment=""/>
@@ -307,15 +310,15 @@
       <workItem from="1690017519765" duration="343000"/>
       <workItem from="1690059954555" duration="24000"/>
       <workItem from="1690155177421" duration="4996000"/>
       <workItem from="1690160472435" duration="247000"/>
       <workItem from="1690160722459" duration="29000"/>
       <workItem from="1690160759296" duration="452000"/>
       <workItem from="1690161233838" duration="114000"/>
-      <workItem from="1690161356699" duration="17199000"/>
+      <workItem from="1690161356699" duration="18453000"/>
     </task>
     <task id="LOCAL-00001" summary="first commit">
       <option name="closed" value="true"/>
       <created>1689566168015</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -410,24 +413,19 @@
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/venv/lib/python3.10/site-packages/httpx_oauth/oauth2.py</url>
           <line>47</line>
           <option name="timeStamp" value="28"/>
         </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/switcore/action/activity_handler_abc.py</url>
-          <line>82</line>
-          <option name="timeStamp" value="43"/>
-        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
     <watches-manager>
       <configuration name="tests">
         <watch expression="unquote(response.headers[&quot;location&quot;])" language="Python"/>
       </configuration>
     </watches-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
-    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1690182109684" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1690183793351" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `switbuilder_core-0.0.8/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/logger.py` & `switbuilder_core-0.0.9/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/lokalise.py` & `switbuilder_core-0.0.9/switcore/lokalise.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/action/activity_handler_abc.py` & `switbuilder_core-0.0.9/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/action/activity_router.py` & `switbuilder_core-0.0.9/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/action/schemas.py` & `switbuilder_core-0.0.9/switcore/action/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,14 @@
     attachments: AttachmentView | None
     reference_view_id: str | None
 
 
 class BaseState(BaseModel):
     autoincrement_id: int = 1
 
-    @staticmethod
-    def from_bytes(byte: bytes) -> 'BaseState':
+    @classmethod
+    def from_bytes(cls, byte: bytes):
         d = json.loads(bz2.decompress(base64.b64decode(byte)).decode("utf-8"))
-        return BaseState(**d)
+        return cls(**d)
 
     def to_bytes(self) -> bytes:
         return base64.b64encode(bz2.compress(json.dumps(self.dict()).encode("utf-8"), 1))
```

### Comparing `switbuilder_core-0.0.8/switcore/auth/dependencies.py` & `switbuilder_core-0.0.9/switcore/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/exception.py` & `switbuilder_core-0.0.9/switcore/auth/exception.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/models.py` & `switbuilder_core-0.0.9/switcore/auth/models.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/oauth2.py` & `switbuilder_core-0.0.9/switcore/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/repository.py` & `switbuilder_core-0.0.9/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/router.py` & `switbuilder_core-0.0.9/switcore/auth/router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/auth/utils.py` & `switbuilder_core-0.0.9/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/ui/collection_entry.py` & `switbuilder_core-0.0.9/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/switcore/ui/file.py` & `switbuilder_core-0.0.9/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/tests/test_oauth2.py` & `switbuilder_core-0.0.9/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/tests/test_path_resolver.py` & `switbuilder_core-0.0.9/tests/test_path_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from switcore.action.activity_router import PathResolver
 from tests.utils import ActionIdTypes
 
 
 class PathResolverTest(unittest.TestCase):
     def test_combined_path(self):
         path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id01, ["a"])
-        self.assertEqual(path_resolver.combined_path, "test_action_id/a")
-        self.assertEqual(path_resolver.id, "test_action_id")
+        self.assertEqual(path_resolver.combined_path, "test_action_id01/a")
+        self.assertEqual(path_resolver.id, "test_action_id01")
 
         path_resolver._paths.append("b")
-        self.assertEqual(path_resolver.combined_path, "test_action_id/a/b")
-        self.assertEqual(path_resolver.id, "test_action_id")
+        self.assertEqual(path_resolver.combined_path, "test_action_id01/a/b")
+        self.assertEqual(path_resolver.id, "test_action_id01")
 
     def test_from_combined(self):
-        path_resolver: PathResolver = PathResolver.from_combined("test_action_id/a/b")
-        self.assertEqual(path_resolver.combined_path, "test_action_id/a/b")
-        self.assertEqual(path_resolver.id, "test_action_id")
+        path_resolver: PathResolver = PathResolver.from_combined("test_action_id01/a/b")
+        self.assertEqual(path_resolver.combined_path, "test_action_id01/a/b")
+        self.assertEqual(path_resolver.id, "test_action_id01")
         self.assertEqual(path_resolver._paths, ["a", "b"])
 
     def test_convert_int(self):
         path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id01, [1, "a"])
-        self.assertEqual(path_resolver.combined_path, "test_action_id/1/a")
+        self.assertEqual(path_resolver.combined_path, "test_action_id01/1/a")
         self.assertEqual(path_resolver.paths, [1, "a"])
 
     def test_escape(self):
         path_resolver: PathResolver = PathResolver(ActionIdTypes.test_escape_action_id, ["a"])
         self.assertEqual(path_resolver.combined_path, "test_escape_action_id\escape/a")
         self.assertEqual(path_resolver.id, "test_escape_action_id\escape")
         self.assertEqual(path_resolver.paths, ["a"])
```

### Comparing `switbuilder_core-0.0.8/tests/test_router.py` & `switbuilder_core-0.0.9/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/tests/utils.py` & `switbuilder_core-0.0.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.8/pyproject.toml` & `switbuilder_core-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `switbuilder_core-0.0.8/PKG-INFO` & `switbuilder_core-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switbuilder-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <el.lee@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

