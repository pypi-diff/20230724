# Comparing `tmp/mypy-boto3-cloudformation-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudformation-1.28.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
```

## Comparing `mypy-boto3-cloudformation-1.28.0.tar` & `mypy-boto3-cloudformation-1.28.10.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.098243 mypy-boto3-cloudformation-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-06 20:59:09.098243 mypy-boto3-cloudformation-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28292 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.094243 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65126 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    65028 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-07-06 20:35:09.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17308 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    90374 2023-07-06 20:35:12.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    90261 2023-07-06 20:35:10.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-06 20:35:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.098243 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:08.000000 mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.098243 mypy-boto3-cloudformation-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:35:06.000000 mypy-boto3-cloudformation-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28854 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66147 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66048 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    91414 2023-07-24 19:47:04.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91321 2023-07-24 19:47:03.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.28.0/LICENSE` & `mypy-boto3-cloudformation-1.28.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/PKG-INFO` & `mypy-boto3-cloudformation-1.28.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudFormation 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.CloudFormation 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,187 +580,201 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
+    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
+    ParameterOutputTypeDef,
+    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
+    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
-    GetTemplateSummaryInputRequestTypeDef,
+    TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    WarningsTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
+    ManagedExecutionOutputTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
-    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
     DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
     DescribeStackEventsOutputTypeDef,
     DescribeTypeOutputTypeDef,
     ListExportsOutputTypeDef,
+    GetTemplateSummaryInputRequestTypeDef,
     ListStackInstancesInputListStackInstancesPaginateTypeDef,
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
+    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
+    StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
@@ -770,21 +784,22 @@
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.0/README.md` & `mypy-boto3-cloudformation-1.28.10/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -548,187 +548,201 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
+    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
+    ParameterOutputTypeDef,
+    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
+    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
-    GetTemplateSummaryInputRequestTypeDef,
+    TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    WarningsTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
+    ManagedExecutionOutputTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
-    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
     DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
     DescribeStackEventsOutputTypeDef,
     DescribeTypeOutputTypeDef,
     ListExportsOutputTypeDef,
+    GetTemplateSummaryInputRequestTypeDef,
     ListStackInstancesInputListStackInstancesPaginateTypeDef,
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
+    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
+    StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
@@ -738,21 +752,22 @@
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/__main__.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudFormation 1.28.10\nVersion:         1.28.10\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.10")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     GetStackPolicyOutputTypeDef,
     GetTemplateOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     ImportStacksToStackSetOutputTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     ListStackSetOperationsOutputTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypeRegistrationsOutputTypeDef,
@@ -113,14 +114,15 @@
     ResourceToImportTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
+    TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
@@ -767,15 +769,16 @@
     def get_template_summary(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#get_template_summary)
         """
@@ -821,14 +824,33 @@
         """
         Lists all stacks that are importing an exported output value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#list_imports)
         """
 
+    def list_stack_instance_resource_drifts(
+        self,
+        *,
+        StackSetName: str,
+        StackInstanceAccount: str,
+        StackInstanceRegion: str,
+        OperationId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
+        CallAs: CallAsType = ...
+    ) -> ListStackInstanceResourceDriftsOutputTypeDef:
+        """
+        Returns drift information for resources in a stack instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#list_stack_instance_resource_drifts)
+        """
+
     def list_stack_instances(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     GetStackPolicyOutputTypeDef,
     GetTemplateOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     ImportStacksToStackSetOutputTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     ListStackSetOperationsOutputTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypeRegistrationsOutputTypeDef,
@@ -113,14 +114,15 @@
     ResourceToImportTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
+    TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
@@ -720,15 +722,16 @@
     def get_template_summary(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#get_template_summary)
         """
@@ -769,14 +772,32 @@
     def list_imports(self, *, ExportName: str, NextToken: str = ...) -> ListImportsOutputTypeDef:
         """
         Lists all stacks that are importing an exported output value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#list_imports)
         """
+    def list_stack_instance_resource_drifts(
+        self,
+        *,
+        StackSetName: str,
+        StackInstanceAccount: str,
+        StackInstanceRegion: str,
+        OperationId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
+        CallAs: CallAsType = ...
+    ) -> ListStackInstanceResourceDriftsOutputTypeDef:
+        """
+        Returns drift information for resources in a stack instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#list_stack_instance_resource_drifts)
+        """
     def list_stack_instances(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountFilterTypeType",
     "AccountGateStatusType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
@@ -101,15 +100,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
@@ -240,15 +238,15 @@
     "FAILED",
     "INOPERABLE",
     "PENDING",
     "RUNNING",
     "SKIPPED_SUSPENDED_ACCOUNT",
     "SUCCEEDED",
 ]
-StackInstanceFilterNameType = Literal["DETAILED_STATUS", "LAST_OPERATION_ID"]
+StackInstanceFilterNameType = Literal["DETAILED_STATUS", "DRIFT_STATUS", "LAST_OPERATION_ID"]
 StackInstanceStatusType = Literal["CURRENT", "INOPERABLE", "OUTDATED"]
 StackResourceDriftStatusType = Literal["DELETED", "IN_SYNC", "MODIFIED", "NOT_CHECKED"]
 StackRollbackCompleteWaiterName = Literal["stack_rollback_complete"]
 StackSetDriftDetectionStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PARTIAL_SUCCESS", "STOPPED"
 ]
 StackSetDriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKED"]
@@ -506,14 +504,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccountFilterTypeType",
     "AccountGateStatusType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
@@ -100,14 +101,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
@@ -238,15 +240,15 @@
     "FAILED",
     "INOPERABLE",
     "PENDING",
     "RUNNING",
     "SKIPPED_SUSPENDED_ACCOUNT",
     "SUCCEEDED",
 ]
-StackInstanceFilterNameType = Literal["DETAILED_STATUS", "LAST_OPERATION_ID"]
+StackInstanceFilterNameType = Literal["DETAILED_STATUS", "DRIFT_STATUS", "LAST_OPERATION_ID"]
 StackInstanceStatusType = Literal["CURRENT", "INOPERABLE", "OUTDATED"]
 StackResourceDriftStatusType = Literal["DELETED", "IN_SYNC", "MODIFIED", "NOT_CHECKED"]
 StackRollbackCompleteWaiterName = Literal["stack_rollback_complete"]
 StackSetDriftDetectionStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PARTIAL_SUCCESS", "STOPPED"
 ]
 StackSetDriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKED"]
@@ -504,14 +506,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,261 +92,245 @@
     "ListStackSetOperationResultsPaginator",
     "ListStackSetOperationsPaginator",
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
-
 class DescribeChangeSetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
-
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
-
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
-
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
-
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
-
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
-
 class ListStackInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
-
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
-
 class ListStackSetOperationResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
-
 class ListStackSetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
-
 class ListStackSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
-
 class ListStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
-
 class ListTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,245 +92,261 @@
     "ListStackSetOperationResultsPaginator",
     "ListStackSetOperationsPaginator",
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
+
 class DescribeChangeSetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
+
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
+
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
+
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
+
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
+
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
+
 class ListStackInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
+
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
+
 class ListStackSetOperationResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
+
 class ListStackSetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
+
 class ListStackSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
+
 class ListStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
+
 class ListTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,22 @@
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseMetadataTypeDef,
     OutputTypeDef,
+    ParameterOutputTypeDef,
     ParameterTypeDef,
     RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackDriftInformationResponseMetadataTypeDef,
     StackResourceDriftInformationResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -232,28 +234,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stack)
     """
 
     stack_id: str
     stack_name: str
     change_set_id: str
     description: str
-    parameters: List[ParameterTypeDef]
+    parameters: List[ParameterOutputTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
     rollback_configuration: RollbackConfigurationResponseMetadataTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
     role_arn: str
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     enable_termination_protection: bool
     parent_id: str
     root_id: str
     drift_information: StackDriftInformationResponseMetadataTypeDef
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,22 @@
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseMetadataTypeDef,
     OutputTypeDef,
+    ParameterOutputTypeDef,
     ParameterTypeDef,
     RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackDriftInformationResponseMetadataTypeDef,
     StackResourceDriftInformationResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -210,28 +212,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stack)
     """
 
     stack_id: str
     stack_name: str
     change_set_id: str
     description: str
-    parameters: List[ParameterTypeDef]
+    parameters: List[ParameterOutputTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
     rollback_configuration: RollbackConfigurationResponseMetadataTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
     role_arn: str
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     enable_termination_protection: bool
     parent_id: str
     root_id: str
     drift_information: StackDriftInformationResponseMetadataTypeDef
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -79,187 +79,201 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "AutoDeploymentOutputTypeDef",
     "AutoDeploymentTypeDef",
+    "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
+    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
+    "ParameterOutputTypeDef",
+    "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
+    "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
-    "GetTemplateSummaryInputRequestTypeDef",
+    "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "WarningsTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
+    "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
+    "ManagedExecutionOutputTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
+    "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseMetadataTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
-    "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
     "DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     "DescribeStackEventsOutputTypeDef",
     "DescribeTypeOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "GetTemplateSummaryInputRequestTypeDef",
     "ListStackInstancesInputListStackInstancesPaginateTypeDef",
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
+    "StackSetSummaryTypeDef",
     "ParameterDeclarationTypeDef",
+    "StackInstanceResourceDriftsSummaryTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
+    "RollbackConfigurationOutputTypeDef",
     "RollbackConfigurationResponseMetadataTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
@@ -269,21 +283,22 @@
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
+    "ListStackInstanceResourceDriftsOutputTypeDef",
     "DescribeStackResourceDriftsOutputTypeDef",
     "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
+    "StackTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
     "DescribeStackResourceOutputTypeDef",
     "DescribeStackResourcesOutputTypeDef",
@@ -299,51 +314,71 @@
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
         "StatusReason": str,
     },
-    total=False,
 )
 
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": str,
         "Value": int,
     },
-    total=False,
 )
 
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+AutoDeploymentOutputTypeDef = TypedDict(
+    "AutoDeploymentOutputTypeDef",
+    {
+        "Enabled": bool,
+        "RetainStacksOnAccountRemoval": bool,
     },
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
     total=False,
 )
 
+TypeConfigurationIdentifierOutputTypeDef = TypedDict(
+    "TypeConfigurationIdentifierOutputTypeDef",
+    {
+        "TypeArn": str,
+        "TypeConfigurationAlias": str,
+        "TypeConfigurationArn": str,
+        "Type": ThirdPartyTypeType,
+        "TypeName": str,
+    },
+)
+
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
@@ -359,15 +394,14 @@
         "Alias": str,
         "Configuration": str,
         "LastUpdated": datetime,
         "TypeArn": str,
         "TypeName": str,
         "IsDefaultConfiguration": bool,
     },
-    total=False,
 )
 
 _RequiredCancelUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredCancelUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -398,15 +432,14 @@
 ChangeSetHookResourceTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookResourceTargetDetailsTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "ResourceAction": ChangeActionType,
     },
-    total=False,
 )
 
 ChangeSetSummaryTypeDef = TypedDict(
     "ChangeSetSummaryTypeDef",
     {
         "StackId": str,
         "StackName": str,
@@ -417,15 +450,14 @@
         "StatusReason": str,
         "CreationTime": datetime,
         "Description": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
     },
-    total=False,
 )
 
 _RequiredContinueUpdateRollbackInputRequestTypeDef = TypedDict(
     "_RequiredContinueUpdateRollbackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -472,23 +504,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -505,46 +528,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -601,22 +600,14 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -630,29 +621,41 @@
 
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
 
+DeploymentTargetsOutputTypeDef = TypedDict(
+    "DeploymentTargetsOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AccountsUrl": str,
+        "OrganizationalUnitIds": List[str],
+        "AccountFilterType": AccountFilterTypeType,
+    },
+)
+
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -690,37 +693,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -735,121 +715,86 @@
 
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
 
-DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
-    "DescribeOrganizationsAccessInputRequestTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
-        "CallAs": CallAsType,
+        "ParameterKey": str,
+        "ParameterValue": str,
+        "UsePreviousValue": bool,
+        "ResolvedValue": str,
     },
-    total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
-DescribePublisherInputRequestTypeDef = TypedDict(
-    "DescribePublisherInputRequestTypeDef",
+DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
+    "DescribeOrganizationsAccessInputRequestTypeDef",
     {
-        "PublisherId": str,
+        "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
+DescribePublisherInputRequestTypeDef = TypedDict(
+    "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredStackEventTypeDef = TypedDict(
-    "_RequiredStackEventTypeDef",
+StackEventTypeDef = TypedDict(
+    "StackEventTypeDef",
     {
         "StackId": str,
         "EventId": str,
         "StackName": str,
-        "Timestamp": datetime,
-    },
-)
-_OptionalStackEventTypeDef = TypedDict(
-    "_OptionalStackEventTypeDef",
-    {
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
+        "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
         "ResourceStatusReason": str,
         "ResourceProperties": str,
         "ClientRequestToken": str,
         "HookType": str,
         "HookStatus": HookStatusType,
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
-    total=False,
 )
 
-
-class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
-    pass
-
-
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -952,23 +897,14 @@
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
 
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -983,43 +919,39 @@
         "VersionId": str,
         "PublisherId": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "LogRoleArn": str,
+        "LogGroupName": str,
+    },
+)
+
 RequiredActivatedTypeTypeDef = TypedDict(
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
     },
-    total=False,
 )
 
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -1033,53 +965,22 @@
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
 
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -1102,103 +1003,57 @@
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": Dict[str, Any],
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemplateSummaryInputRequestTypeDef = TypedDict(
-    "GetTemplateSummaryInputRequestTypeDef",
+TemplateSummaryConfigTypeDef = TypedDict(
+    "TemplateSummaryConfigTypeDef",
     {
-        "TemplateBody": str,
-        "TemplateURL": str,
-        "StackName": str,
-        "StackSetName": str,
-        "CallAs": CallAsType,
+        "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
 
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
-    total=False,
-)
-
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+WarningsTypeDef = TypedDict(
+    "WarningsTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "UnrecognizedResourceTypes": List[str],
     },
-    total=False,
 )
 
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1212,113 +1067,80 @@
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
 
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
+_RequiredListImportsInputRequestTypeDef = TypedDict(
+    "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
+_OptionalListImportsInputRequestTypeDef = TypedDict(
+    "_OptionalListImportsInputRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
     },
     total=False,
 )
 
 
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
+class ListImportsInputRequestTypeDef(
+    _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListImportsInputRequestTypeDef = TypedDict(
-    "_RequiredListImportsInputRequestTypeDef",
+_RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
     {
-        "ExportName": str,
+        "StackSetName": str,
+        "StackInstanceAccount": str,
+        "StackInstanceRegion": str,
+        "OperationId": str,
     },
 )
-_OptionalListImportsInputRequestTypeDef = TypedDict(
-    "_OptionalListImportsInputRequestTypeDef",
+_OptionalListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_OptionalListStackInstanceResourceDriftsInputRequestTypeDef",
     {
         "NextToken": str,
+        "MaxResults": int,
+        "StackInstanceResourceDriftStatuses": Sequence[StackResourceDriftStatusType],
+        "CallAs": CallAsType,
     },
     total=False,
 )
 
 
-class ListImportsInputRequestTypeDef(
-    _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
+class ListStackInstanceResourceDriftsInputRequestTypeDef(
+    _RequiredListStackInstanceResourceDriftsInputRequestTypeDef,
+    _OptionalListStackInstanceResourceDriftsInputRequestTypeDef,
 ):
     pass
 
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1341,37 +1163,14 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1388,44 +1187,25 @@
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
 
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1440,23 +1220,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1475,15 +1246,14 @@
         "VersionId": str,
         "IsDefaultVersion": bool,
         "Arn": str,
         "TimeCreated": datetime,
         "Description": str,
         "PublicVersionNumber": str,
     },
-    total=False,
 )
 
 TypeFiltersTypeDef = TypedDict(
     "TypeFiltersTypeDef",
     {
         "Category": CategoryType,
         "PublisherId": str,
@@ -1505,62 +1275,46 @@
         "OriginalTypeName": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
-    total=False,
 )
 
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
+ManagedExecutionOutputTypeDef = TypedDict(
+    "ManagedExecutionOutputTypeDef",
     {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Active": bool,
     },
 )
 
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
-    total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
     },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
 )
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
-    total=False,
 )
 
 PhysicalResourceIdContextKeyValuePairTypeDef = TypedDict(
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1584,22 +1338,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1628,48 +1374,28 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RollbackTriggerOutputTypeDef = TypedDict(
+    "RollbackTriggerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Type": str,
     },
 )
 
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
@@ -1695,22 +1421,14 @@
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
 
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1750,22 +1468,14 @@
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
 
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1779,155 +1489,84 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
+StackDriftInformationSummaryTypeDef = TypedDict(
+    "StackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
         "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStackDriftInformationSummaryTypeDef = TypedDict(
-    "_RequiredStackDriftInformationSummaryTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-    },
-)
-_OptionalStackDriftInformationSummaryTypeDef = TypedDict(
-    "_OptionalStackDriftInformationSummaryTypeDef",
-    {
-        "LastCheckTimestamp": datetime,
-    },
-    total=False,
-)
-
-
-class StackDriftInformationSummaryTypeDef(
-    _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
-):
-    pass
-
-
-_RequiredStackDriftInformationTypeDef = TypedDict(
-    "_RequiredStackDriftInformationTypeDef",
+StackDriftInformationTypeDef = TypedDict(
+    "StackDriftInformationTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
-    },
-)
-_OptionalStackDriftInformationTypeDef = TypedDict(
-    "_OptionalStackDriftInformationTypeDef",
-    {
         "LastCheckTimestamp": datetime,
     },
-    total=False,
 )
 
-
-class StackDriftInformationTypeDef(
-    _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
-):
-    pass
-
-
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
-    total=False,
-)
-
-_RequiredStackResourceDriftInformationTypeDef = TypedDict(
-    "_RequiredStackResourceDriftInformationTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-    },
-)
-_OptionalStackResourceDriftInformationTypeDef = TypedDict(
-    "_OptionalStackResourceDriftInformationTypeDef",
-    {
-        "LastCheckTimestamp": datetime,
-    },
-    total=False,
-)
-
-
-class StackResourceDriftInformationTypeDef(
-    _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
-):
-    pass
-
-
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+StackResourceDriftInformationTypeDef = TypedDict(
+    "StackResourceDriftInformationTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "_RequiredStackResourceDriftInformationSummaryTypeDef",
+StackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
-    },
-)
-_OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "_OptionalStackResourceDriftInformationSummaryTypeDef",
-    {
         "LastCheckTimestamp": datetime,
     },
-    total=False,
 )
 
-
-class StackResourceDriftInformationSummaryTypeDef(
-    _RequiredStackResourceDriftInformationSummaryTypeDef,
-    _OptionalStackResourceDriftInformationSummaryTypeDef,
-):
-    pass
-
-
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
         "DriftedStackInstancesCount": int,
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
-    total=False,
+)
+
+StackSetOperationPreferencesOutputTypeDef = TypedDict(
+    "StackSetOperationPreferencesOutputTypeDef",
+    {
+        "RegionConcurrencyType": RegionConcurrencyTypeType,
+        "RegionOrder": List[str],
+        "FailureToleranceCount": int,
+        "FailureTolerancePercentage": int,
+        "MaxConcurrentCount": int,
+        "MaxConcurrentPercentage": int,
+    },
 )
 
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
-    total=False,
 )
 
 _RequiredStopStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredStopStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
@@ -1953,77 +1592,36 @@
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
     },
-    total=False,
 )
 
 TestTypeInputRequestTypeDef = TypedDict(
     "TestTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -2035,24 +1633,14 @@
         "Account": str,
         "Region": str,
         "Status": StackSetOperationResultStatusType,
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
-    total=False,
-)
-
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
@@ -2089,22 +1677,313 @@
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
 
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": str,
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseMetadataTypeDef = TypedDict(
+    "ModuleInfoResponseMetadataTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackDriftInformationResponseMetadataTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
+        "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
     },
-    total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
         "TypeConfigurationIdentifiers": Sequence[TypeConfigurationIdentifierTypeDef],
     },
@@ -2112,23 +1991,22 @@
 
 ChangeSetHookTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookTargetDetailsTypeDef",
     {
         "TargetType": Literal["RESOURCE"],
         "ResourceTargetDetails": ChangeSetHookResourceTargetDetailsTypeDef,
     },
-    total=False,
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2302,30 +2180,14 @@
 
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
 
-StackSetSummaryTypeDef = TypedDict(
-    "StackSetSummaryTypeDef",
-    {
-        "StackSetName": str,
-        "StackSetId": str,
-        "Description": str,
-        "Status": StackSetStatusType,
-        "AutoDeployment": AutoDeploymentTypeDef,
-        "PermissionModel": PermissionModelsType,
-        "DriftStatus": StackDriftStatusType,
-        "LastDriftCheckTimestamp": datetime,
-        "ManagedExecution": ManagedExecutionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalUpdateStackSetInputRequestTypeDef = TypedDict(
@@ -2356,14 +2218,179 @@
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2467,15 +2494,15 @@
 
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2485,15 +2512,15 @@
         "IsDefaultVersion": bool,
         "TypeTestsStatus": TypeTestsStatusType,
         "TypeTestsStatusDescription": str,
         "Description": str,
         "Schema": str,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
-        "LoggingConfig": LoggingConfigTypeDef,
+        "LoggingConfig": LoggingConfigOutputTypeDef,
         "RequiredActivatedTypes": List[RequiredActivatedTypeTypeDef],
         "ExecutionRoleArn": str,
         "Visibility": VisibilityType,
         "SourceUrl": str,
         "DocumentationUrl": str,
         "LastUpdated": datetime,
         "TimeCreated": datetime,
@@ -2501,41 +2528,54 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateSummaryInputRequestTypeDef = TypedDict(
+    "GetTemplateSummaryInputRequestTypeDef",
+    {
+        "TemplateBody": str,
+        "TemplateURL": str,
+        "StackName": str,
+        "StackSetName": str,
+        "CallAs": CallAsType,
+        "TemplateSummaryConfig": TemplateSummaryConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2578,15 +2618,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2622,27 +2662,27 @@
 
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2658,118 +2698,129 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackSetSummaryTypeDef = TypedDict(
+    "StackSetSummaryTypeDef",
+    {
+        "StackSetName": str,
+        "StackSetId": str,
+        "Description": str,
+        "Status": StackSetStatusType,
+        "AutoDeployment": AutoDeploymentOutputTypeDef,
+        "PermissionModel": PermissionModelsType,
+        "DriftStatus": StackDriftStatusType,
+        "LastDriftCheckTimestamp": datetime,
+        "ManagedExecution": ManagedExecutionOutputTypeDef,
     },
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "ParameterType": str,
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
-    total=False,
 )
 
-_RequiredStackResourceDriftTypeDef = TypedDict(
-    "_RequiredStackResourceDriftTypeDef",
+StackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "StackInstanceResourceDriftsSummaryTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
         "ResourceType": str,
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "Timestamp": datetime,
     },
 )
-_OptionalStackResourceDriftTypeDef = TypedDict(
-    "_OptionalStackResourceDriftTypeDef",
+
+StackResourceDriftTypeDef = TypedDict(
+    "StackResourceDriftTypeDef",
     {
+        "StackId": str,
+        "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "ResourceType": str,
         "ExpectedProperties": str,
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-
-class StackResourceDriftTypeDef(
-    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
-):
-    pass
-
-
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
-    total=False,
+)
+
+RollbackConfigurationOutputTypeDef = TypedDict(
+    "RollbackConfigurationOutputTypeDef",
+    {
+        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
+        "MonitoringTimeInMinutes": int,
+    },
 )
 
 RollbackConfigurationResponseMetadataTypeDef = TypedDict(
     "RollbackConfigurationResponseMetadataTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-_RequiredStackSummaryTypeDef = TypedDict(
-    "_RequiredStackSummaryTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackSummaryTypeDef = TypedDict(
-    "_OptionalStackSummaryTypeDef",
+StackSummaryTypeDef = TypedDict(
+    "StackSummaryTypeDef",
     {
         "StackId": str,
+        "StackName": str,
         "TemplateDescription": str,
+        "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "DeletionTime": datetime,
+        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
-    total=False,
 )
 
-
-class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
-    pass
-
-
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2777,232 +2828,189 @@
         "StatusReason": str,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
-    total=False,
 )
 
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
-        "ParameterOverrides": List[ParameterTypeDef],
+        "ParameterOverrides": List[ParameterOutputTypeDef],
         "Status": StackInstanceStatusType,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
-    total=False,
 )
 
-_RequiredStackResourceDetailTypeDef = TypedDict(
-    "_RequiredStackResourceDetailTypeDef",
+StackResourceDetailTypeDef = TypedDict(
+    "StackResourceDetailTypeDef",
     {
+        "StackName": str,
+        "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceDetailTypeDef = TypedDict(
-    "_OptionalStackResourceDetailTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-
-class StackResourceDetailTypeDef(
-    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
-):
-    pass
-
-
-_RequiredStackResourceTypeDef = TypedDict(
-    "_RequiredStackResourceTypeDef",
+StackResourceTypeDef = TypedDict(
+    "StackResourceTypeDef",
     {
+        "StackName": str,
+        "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceTypeDef = TypedDict(
-    "_OptionalStackResourceTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-
-class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
-    pass
-
-
-_RequiredStackResourceSummaryTypeDef = TypedDict(
-    "_RequiredStackResourceSummaryTypeDef",
+StackResourceSummaryTypeDef = TypedDict(
+    "StackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceSummaryTypeDef = TypedDict(
-    "_OptionalStackResourceSummaryTypeDef",
-    {
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-
-class StackResourceSummaryTypeDef(
-    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
-):
-    pass
-
-
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
         "TemplateBody": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "StackSetARN": str,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "AutoDeployment": AutoDeploymentTypeDef,
+        "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
-        "ManagedExecution": ManagedExecutionTypeDef,
+        "ManagedExecution": ManagedExecutionOutputTypeDef,
         "Regions": List[str],
     },
-    total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
-    total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
         "RetainStacks": bool,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsTypeDef,
+        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
-    total=False,
 )
 
 ValidateTemplateOutputTypeDef = TypedDict(
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
-        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
+        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
         "FailureMode": HookFailureModeType,
         "TypeName": str,
         "TypeVersionId": str,
         "TypeConfigurationVersionId": str,
         "TargetDetails": ChangeSetHookTargetDetailsTypeDef,
     },
-    total=False,
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -3010,32 +3018,42 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Warnings": WarningsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
+    "ListStackInstanceResourceDriftsOutputTypeDef",
+    {
+        "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3044,15 +3062,42 @@
         "ResourceType": str,
         "Replacement": ReplacementType,
         "Scope": List[ResourceAttributeType],
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
+)
+
+StackTypeDef = TypedDict(
+    "StackTypeDef",
+    {
+        "StackId": str,
+        "StackName": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterOutputTypeDef],
+        "CreationTime": datetime,
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "StackStatus": StackStatusType,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagOutputTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+    },
 )
 
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
@@ -3157,53 +3202,14 @@
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
 
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
-    {
-        "StackId": str,
-        "ChangeSetId": str,
-        "Description": str,
-        "Parameters": List[ParameterTypeDef],
-        "DeletionTime": datetime,
-        "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
-        "StackStatusReason": str,
-        "DisableRollback": bool,
-        "NotificationARNs": List[str],
-        "TimeoutInMinutes": int,
-        "Capabilities": List[CapabilityType],
-        "Outputs": List[OutputTypeDef],
-        "RoleARN": str,
-        "Tags": List[TagTypeDef],
-        "EnableTerminationProtection": bool,
-        "ParentId": str,
-        "RootId": str,
-        "DriftInformation": StackDriftInformationTypeDef,
-    },
-    total=False,
-)
-
-
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
-    pass
-
-
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3260,137 +3266,136 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
-    total=False,
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -78,187 +78,201 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "AutoDeploymentOutputTypeDef",
     "AutoDeploymentTypeDef",
+    "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
+    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
+    "ParameterOutputTypeDef",
+    "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
+    "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
-    "GetTemplateSummaryInputRequestTypeDef",
+    "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "WarningsTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
+    "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
+    "ManagedExecutionOutputTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
+    "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseMetadataTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
-    "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
     "DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     "DescribeStackEventsOutputTypeDef",
     "DescribeTypeOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "GetTemplateSummaryInputRequestTypeDef",
     "ListStackInstancesInputListStackInstancesPaginateTypeDef",
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
+    "StackSetSummaryTypeDef",
     "ParameterDeclarationTypeDef",
+    "StackInstanceResourceDriftsSummaryTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
+    "RollbackConfigurationOutputTypeDef",
     "RollbackConfigurationResponseMetadataTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
@@ -268,21 +282,22 @@
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
+    "ListStackInstanceResourceDriftsOutputTypeDef",
     "DescribeStackResourceDriftsOutputTypeDef",
     "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
+    "StackTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
     "DescribeStackResourceOutputTypeDef",
     "DescribeStackResourcesOutputTypeDef",
@@ -298,51 +313,71 @@
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
         "StatusReason": str,
     },
-    total=False,
 )
 
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": str,
         "Value": int,
     },
-    total=False,
 )
 
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+AutoDeploymentOutputTypeDef = TypedDict(
+    "AutoDeploymentOutputTypeDef",
+    {
+        "Enabled": bool,
+        "RetainStacksOnAccountRemoval": bool,
     },
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
     total=False,
 )
 
+TypeConfigurationIdentifierOutputTypeDef = TypedDict(
+    "TypeConfigurationIdentifierOutputTypeDef",
+    {
+        "TypeArn": str,
+        "TypeConfigurationAlias": str,
+        "TypeConfigurationArn": str,
+        "Type": ThirdPartyTypeType,
+        "TypeName": str,
+    },
+)
+
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
@@ -358,15 +393,14 @@
         "Alias": str,
         "Configuration": str,
         "LastUpdated": datetime,
         "TypeArn": str,
         "TypeName": str,
         "IsDefaultConfiguration": bool,
     },
-    total=False,
 )
 
 _RequiredCancelUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredCancelUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -395,15 +429,14 @@
 ChangeSetHookResourceTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookResourceTargetDetailsTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "ResourceAction": ChangeActionType,
     },
-    total=False,
 )
 
 ChangeSetSummaryTypeDef = TypedDict(
     "ChangeSetSummaryTypeDef",
     {
         "StackId": str,
         "StackName": str,
@@ -414,15 +447,14 @@
         "StatusReason": str,
         "CreationTime": datetime,
         "Description": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
     },
-    total=False,
 )
 
 _RequiredContinueUpdateRollbackInputRequestTypeDef = TypedDict(
     "_RequiredContinueUpdateRollbackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -467,23 +499,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -500,46 +523,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -592,22 +591,14 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -619,29 +610,41 @@
 )
 
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
+DeploymentTargetsOutputTypeDef = TypedDict(
+    "DeploymentTargetsOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AccountsUrl": str,
+        "OrganizationalUnitIds": List[str],
+        "AccountFilterType": AccountFilterTypeType,
+    },
+)
+
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -677,35 +680,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -718,119 +700,86 @@
 )
 
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
-DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
-    "DescribeOrganizationsAccessInputRequestTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
-        "CallAs": CallAsType,
+        "ParameterKey": str,
+        "ParameterValue": str,
+        "UsePreviousValue": bool,
+        "ResolvedValue": str,
     },
-    total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
-DescribePublisherInputRequestTypeDef = TypedDict(
-    "DescribePublisherInputRequestTypeDef",
+DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
+    "DescribeOrganizationsAccessInputRequestTypeDef",
     {
-        "PublisherId": str,
+        "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
+DescribePublisherInputRequestTypeDef = TypedDict(
+    "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredStackEventTypeDef = TypedDict(
-    "_RequiredStackEventTypeDef",
+StackEventTypeDef = TypedDict(
+    "StackEventTypeDef",
     {
         "StackId": str,
         "EventId": str,
         "StackName": str,
-        "Timestamp": datetime,
-    },
-)
-_OptionalStackEventTypeDef = TypedDict(
-    "_OptionalStackEventTypeDef",
-    {
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
+        "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
         "ResourceStatusReason": str,
         "ResourceProperties": str,
         "ClientRequestToken": str,
         "HookType": str,
         "HookStatus": HookStatusType,
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
-    total=False,
 )
 
-class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
-    pass
-
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -925,23 +874,14 @@
 
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -956,43 +896,39 @@
         "VersionId": str,
         "PublisherId": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "LogRoleArn": str,
+        "LogGroupName": str,
+    },
+)
+
 RequiredActivatedTypeTypeDef = TypedDict(
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
     },
-    total=False,
 )
 
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -1004,53 +940,22 @@
 )
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -1071,101 +976,57 @@
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
+TemplateSummaryConfigTypeDef = TypedDict(
+    "TemplateSummaryConfigTypeDef",
     {
-        "TemplateBody": Dict[str, Any],
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemplateSummaryInputRequestTypeDef = TypedDict(
-    "GetTemplateSummaryInputRequestTypeDef",
-    {
-        "TemplateBody": str,
-        "TemplateURL": str,
-        "StackName": str,
-        "StackSetName": str,
-        "CallAs": CallAsType,
+        "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
 
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
-    total=False,
 )
 
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
+WarningsTypeDef = TypedDict(
+    "WarningsTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UnrecognizedResourceTypes": List[str],
     },
 )
 
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1177,50 +1038,22 @@
 )
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
@@ -1232,52 +1065,49 @@
 )
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
+_RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
+    {
+        "StackSetName": str,
+        "StackInstanceAccount": str,
+        "StackInstanceRegion": str,
+        "OperationId": str,
+    },
+)
+_OptionalListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_OptionalListStackInstanceResourceDriftsInputRequestTypeDef",
     {
-        "Imports": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxResults": int,
+        "StackInstanceResourceDriftStatuses": Sequence[StackResourceDriftStatusType],
+        "CallAs": CallAsType,
     },
+    total=False,
 )
 
+class ListStackInstanceResourceDriftsInputRequestTypeDef(
+    _RequiredListStackInstanceResourceDriftsInputRequestTypeDef,
+    _OptionalListStackInstanceResourceDriftsInputRequestTypeDef,
+):
+    pass
+
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1298,35 +1128,14 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1341,44 +1150,25 @@
 
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1393,23 +1183,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1428,15 +1209,14 @@
         "VersionId": str,
         "IsDefaultVersion": bool,
         "Arn": str,
         "TimeCreated": datetime,
         "Description": str,
         "PublicVersionNumber": str,
     },
-    total=False,
 )
 
 TypeFiltersTypeDef = TypedDict(
     "TypeFiltersTypeDef",
     {
         "Category": CategoryType,
         "PublisherId": str,
@@ -1458,62 +1238,46 @@
         "OriginalTypeName": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
-    total=False,
 )
 
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
+ManagedExecutionOutputTypeDef = TypedDict(
+    "ManagedExecutionOutputTypeDef",
     {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Active": bool,
     },
 )
 
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
-    total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
     },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
 )
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
-    total=False,
 )
 
 PhysicalResourceIdContextKeyValuePairTypeDef = TypedDict(
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1537,22 +1301,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1579,48 +1335,28 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RollbackTriggerOutputTypeDef = TypedDict(
+    "RollbackTriggerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Type": str,
     },
 )
 
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
@@ -1644,22 +1380,14 @@
 )
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1695,22 +1423,14 @@
 
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1724,147 +1444,84 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStackDriftInformationSummaryTypeDef = TypedDict(
-    "_RequiredStackDriftInformationSummaryTypeDef",
+StackDriftInformationSummaryTypeDef = TypedDict(
+    "StackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
-    },
-)
-_OptionalStackDriftInformationSummaryTypeDef = TypedDict(
-    "_OptionalStackDriftInformationSummaryTypeDef",
-    {
         "LastCheckTimestamp": datetime,
     },
-    total=False,
 )
 
-class StackDriftInformationSummaryTypeDef(
-    _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
-):
-    pass
-
-_RequiredStackDriftInformationTypeDef = TypedDict(
-    "_RequiredStackDriftInformationTypeDef",
+StackDriftInformationTypeDef = TypedDict(
+    "StackDriftInformationTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
-    },
-)
-_OptionalStackDriftInformationTypeDef = TypedDict(
-    "_OptionalStackDriftInformationTypeDef",
-    {
         "LastCheckTimestamp": datetime,
     },
-    total=False,
 )
 
-class StackDriftInformationTypeDef(
-    _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
-):
-    pass
-
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
-    total=False,
-)
-
-_RequiredStackResourceDriftInformationTypeDef = TypedDict(
-    "_RequiredStackResourceDriftInformationTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-    },
-)
-_OptionalStackResourceDriftInformationTypeDef = TypedDict(
-    "_OptionalStackResourceDriftInformationTypeDef",
-    {
-        "LastCheckTimestamp": datetime,
-    },
-    total=False,
 )
 
-class StackResourceDriftInformationTypeDef(
-    _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
-):
-    pass
-
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+StackResourceDriftInformationTypeDef = TypedDict(
+    "StackResourceDriftInformationTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "_RequiredStackResourceDriftInformationSummaryTypeDef",
+StackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
-    },
-)
-_OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "_OptionalStackResourceDriftInformationSummaryTypeDef",
-    {
         "LastCheckTimestamp": datetime,
     },
-    total=False,
 )
 
-class StackResourceDriftInformationSummaryTypeDef(
-    _RequiredStackResourceDriftInformationSummaryTypeDef,
-    _OptionalStackResourceDriftInformationSummaryTypeDef,
-):
-    pass
-
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
         "DriftedStackInstancesCount": int,
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
-    total=False,
+)
+
+StackSetOperationPreferencesOutputTypeDef = TypedDict(
+    "StackSetOperationPreferencesOutputTypeDef",
+    {
+        "RegionConcurrencyType": RegionConcurrencyTypeType,
+        "RegionOrder": List[str],
+        "FailureToleranceCount": int,
+        "FailureTolerancePercentage": int,
+        "MaxConcurrentCount": int,
+        "MaxConcurrentPercentage": int,
+    },
 )
 
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
-    total=False,
 )
 
 _RequiredStopStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredStopStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
@@ -1888,77 +1545,36 @@
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
     },
-    total=False,
 )
 
 TestTypeInputRequestTypeDef = TypedDict(
     "TestTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -1970,24 +1586,14 @@
         "Account": str,
         "Region": str,
         "Status": StackSetOperationResultStatusType,
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
-    total=False,
-)
-
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
@@ -2022,22 +1628,313 @@
 )
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": str,
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseMetadataTypeDef = TypedDict(
+    "ModuleInfoResponseMetadataTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackDriftInformationResponseMetadataTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
+        "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
     },
-    total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
         "TypeConfigurationIdentifiers": Sequence[TypeConfigurationIdentifierTypeDef],
     },
@@ -2045,23 +1942,22 @@
 
 ChangeSetHookTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookTargetDetailsTypeDef",
     {
         "TargetType": Literal["RESOURCE"],
         "ResourceTargetDetails": ChangeSetHookResourceTargetDetailsTypeDef,
     },
-    total=False,
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2223,30 +2119,14 @@
 )
 
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
-StackSetSummaryTypeDef = TypedDict(
-    "StackSetSummaryTypeDef",
-    {
-        "StackSetName": str,
-        "StackSetId": str,
-        "Description": str,
-        "Status": StackSetStatusType,
-        "AutoDeployment": AutoDeploymentTypeDef,
-        "PermissionModel": PermissionModelsType,
-        "DriftStatus": StackDriftStatusType,
-        "LastDriftCheckTimestamp": datetime,
-        "ManagedExecution": ManagedExecutionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalUpdateStackSetInputRequestTypeDef = TypedDict(
@@ -2275,14 +2155,169 @@
 )
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2382,15 +2417,15 @@
     pass
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2400,15 +2435,15 @@
         "IsDefaultVersion": bool,
         "TypeTestsStatus": TypeTestsStatusType,
         "TypeTestsStatusDescription": str,
         "Description": str,
         "Schema": str,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
-        "LoggingConfig": LoggingConfigTypeDef,
+        "LoggingConfig": LoggingConfigOutputTypeDef,
         "RequiredActivatedTypes": List[RequiredActivatedTypeTypeDef],
         "ExecutionRoleArn": str,
         "Visibility": VisibilityType,
         "SourceUrl": str,
         "DocumentationUrl": str,
         "LastUpdated": datetime,
         "TimeCreated": datetime,
@@ -2416,41 +2451,54 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateSummaryInputRequestTypeDef = TypedDict(
+    "GetTemplateSummaryInputRequestTypeDef",
+    {
+        "TemplateBody": str,
+        "TemplateURL": str,
+        "StackName": str,
+        "StackSetName": str,
+        "CallAs": CallAsType,
+        "TemplateSummaryConfig": TemplateSummaryConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
     _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2489,15 +2537,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2529,27 +2577,27 @@
     pass
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2565,114 +2613,129 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackSetSummaryTypeDef = TypedDict(
+    "StackSetSummaryTypeDef",
+    {
+        "StackSetName": str,
+        "StackSetId": str,
+        "Description": str,
+        "Status": StackSetStatusType,
+        "AutoDeployment": AutoDeploymentOutputTypeDef,
+        "PermissionModel": PermissionModelsType,
+        "DriftStatus": StackDriftStatusType,
+        "LastDriftCheckTimestamp": datetime,
+        "ManagedExecution": ManagedExecutionOutputTypeDef,
     },
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "ParameterType": str,
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
-    total=False,
 )
 
-_RequiredStackResourceDriftTypeDef = TypedDict(
-    "_RequiredStackResourceDriftTypeDef",
+StackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "StackInstanceResourceDriftsSummaryTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
         "ResourceType": str,
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "Timestamp": datetime,
     },
 )
-_OptionalStackResourceDriftTypeDef = TypedDict(
-    "_OptionalStackResourceDriftTypeDef",
+
+StackResourceDriftTypeDef = TypedDict(
+    "StackResourceDriftTypeDef",
     {
+        "StackId": str,
+        "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "ResourceType": str,
         "ExpectedProperties": str,
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-class StackResourceDriftTypeDef(
-    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
-):
-    pass
-
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
-    total=False,
+)
+
+RollbackConfigurationOutputTypeDef = TypedDict(
+    "RollbackConfigurationOutputTypeDef",
+    {
+        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
+        "MonitoringTimeInMinutes": int,
+    },
 )
 
 RollbackConfigurationResponseMetadataTypeDef = TypedDict(
     "RollbackConfigurationResponseMetadataTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-_RequiredStackSummaryTypeDef = TypedDict(
-    "_RequiredStackSummaryTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackSummaryTypeDef = TypedDict(
-    "_OptionalStackSummaryTypeDef",
+StackSummaryTypeDef = TypedDict(
+    "StackSummaryTypeDef",
     {
         "StackId": str,
+        "StackName": str,
         "TemplateDescription": str,
+        "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "DeletionTime": datetime,
+        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
-    total=False,
 )
 
-class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
-    pass
-
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2680,226 +2743,189 @@
         "StatusReason": str,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
-    total=False,
 )
 
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
-        "ParameterOverrides": List[ParameterTypeDef],
+        "ParameterOverrides": List[ParameterOutputTypeDef],
         "Status": StackInstanceStatusType,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
-    total=False,
 )
 
-_RequiredStackResourceDetailTypeDef = TypedDict(
-    "_RequiredStackResourceDetailTypeDef",
+StackResourceDetailTypeDef = TypedDict(
+    "StackResourceDetailTypeDef",
     {
+        "StackName": str,
+        "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceDetailTypeDef = TypedDict(
-    "_OptionalStackResourceDetailTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-class StackResourceDetailTypeDef(
-    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
-):
-    pass
-
-_RequiredStackResourceTypeDef = TypedDict(
-    "_RequiredStackResourceTypeDef",
+StackResourceTypeDef = TypedDict(
+    "StackResourceTypeDef",
     {
+        "StackName": str,
+        "StackId": str,
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceTypeDef = TypedDict(
-    "_OptionalStackResourceTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
-    pass
-
-_RequiredStackResourceSummaryTypeDef = TypedDict(
-    "_RequiredStackResourceSummaryTypeDef",
+StackResourceSummaryTypeDef = TypedDict(
+    "StackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
+        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceSummaryTypeDef = TypedDict(
-    "_OptionalStackResourceSummaryTypeDef",
-    {
-        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
 )
 
-class StackResourceSummaryTypeDef(
-    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
-):
-    pass
-
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
         "TemplateBody": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "StackSetARN": str,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "AutoDeployment": AutoDeploymentTypeDef,
+        "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
-        "ManagedExecution": ManagedExecutionTypeDef,
+        "ManagedExecution": ManagedExecutionOutputTypeDef,
         "Regions": List[str],
     },
-    total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
-    total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
         "RetainStacks": bool,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsTypeDef,
+        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
-    total=False,
 )
 
 ValidateTemplateOutputTypeDef = TypedDict(
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
-        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
+        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
         "FailureMode": HookFailureModeType,
         "TypeName": str,
         "TypeVersionId": str,
         "TypeConfigurationVersionId": str,
         "TargetDetails": ChangeSetHookTargetDetailsTypeDef,
     },
-    total=False,
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -2907,32 +2933,42 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Warnings": WarningsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
+    "ListStackInstanceResourceDriftsOutputTypeDef",
+    {
+        "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -2941,15 +2977,42 @@
         "ResourceType": str,
         "Replacement": ReplacementType,
         "Scope": List[ResourceAttributeType],
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
-    total=False,
+)
+
+StackTypeDef = TypedDict(
+    "StackTypeDef",
+    {
+        "StackId": str,
+        "StackName": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterOutputTypeDef],
+        "CreationTime": datetime,
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "StackStatus": StackStatusType,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagOutputTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+    },
 )
 
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
@@ -3048,51 +3111,14 @@
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
-    {
-        "StackId": str,
-        "ChangeSetId": str,
-        "Description": str,
-        "Parameters": List[ParameterTypeDef],
-        "DeletionTime": datetime,
-        "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
-        "StackStatusReason": str,
-        "DisableRollback": bool,
-        "NotificationARNs": List[str],
-        "TimeoutInMinutes": int,
-        "Capabilities": List[CapabilityType],
-        "Outputs": List[OutputTypeDef],
-        "RoleARN": str,
-        "Tags": List[TagTypeDef],
-        "EnableTerminationProtection": bool,
-        "ParentId": str,
-        "RootId": str,
-        "DriftInformation": StackDriftInformationTypeDef,
-    },
-    total=False,
-)
-
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
-    pass
-
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3147,137 +3173,136 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
-    total=False,
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudFormation 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.CloudFormation 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,187 +580,201 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
+    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
+    ParameterOutputTypeDef,
+    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
+    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
-    GetTemplateSummaryInputRequestTypeDef,
+    TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    WarningsTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
+    ManagedExecutionOutputTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
-    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
     DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
     DescribeStackEventsOutputTypeDef,
     DescribeTypeOutputTypeDef,
     ListExportsOutputTypeDef,
+    GetTemplateSummaryInputRequestTypeDef,
     ListStackInstancesInputListStackInstancesPaginateTypeDef,
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
+    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
+    StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
@@ -770,21 +784,22 @@
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.0/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.0/setup.py` & `mypy-boto3-cloudformation-1.28.10/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.28.0",
+    version="1.28.10",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFormation 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudFormation 1.28.10 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

