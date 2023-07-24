# Comparing `tmp/mypy-boto3-ce-1.28.0.tar.gz` & `tmp/mypy-boto3-ce-1.28.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
```

## Comparing `mypy-boto3-ce-1.28.0.tar` & `mypy-boto3-ce-1.28.10.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.594235 mypy-boto3-ce-1.28.0/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31896 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-07-06 20:34:26.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-06 20:34:26.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63440 2023-07-06 20:34:29.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63371 2023-07-06 20:34:28.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18167 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68270 2023-07-24 19:46:58.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68211 2023-07-24 19:46:57.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/setup.py
```

### Comparing `mypy-boto3-ce-1.28.0/LICENSE` & `mypy-boto3-ce-1.28.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.0/PKG-INFO` & `mypy-boto3-ce-1.28.10/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-ce
-Version: 1.28.0
-Summary: Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ce type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,110 +298,128 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
+    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
+    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
+    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalTypeDef,
+    DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
+    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
+    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
+    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
+    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
+    RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
+    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
+    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -442,35 +428,38 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
     CreateCostCategoryDefinitionRequestRequestTypeDef,
     UpdateCostCategoryDefinitionRequestRequestTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.0/README.md` & `mypy-boto3-ce-1.28.10/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-ce
+Version: 1.28.10
+Summary: Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 ce type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,110 +330,128 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
+    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
+    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
+    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalTypeDef,
+    DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
+    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
+    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
+    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
+    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
+    RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
+    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
+    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -410,35 +460,38 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
     CreateCostCategoryDefinitionRequestRequestTypeDef,
     UpdateCostCategoryDefinitionRequestRequestTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CostExplorer 1.28.10\nVersion:         1.28.10\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
     GetDimensionValuesResponseTypeDef,
     GetReservationCoverageResponseTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     GetSavingsPlansPurchaseRecommendationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetTagsResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     GroupDefinitionTypeDef,
@@ -458,14 +459,24 @@
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_rightsizing_recommendation)
         """
 
+    def get_savings_plan_purchase_recommendation_details(
+        self, *, RecommendationDetailId: str
+    ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
+        """
+        Retrieves the details for a Savings Plan recommendation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plan_purchase_recommendation_details)
+        """
+
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
@@ -677,15 +688,15 @@
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
         ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
-        Updates an existing cost anomaly monitor subscription.
+        Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
 
     def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
     GetDimensionValuesResponseTypeDef,
     GetReservationCoverageResponseTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     GetSavingsPlansPurchaseRecommendationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetTagsResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     GroupDefinitionTypeDef,
@@ -431,14 +432,23 @@
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_rightsizing_recommendation)
         """
+    def get_savings_plan_purchase_recommendation_details(
+        self, *, RecommendationDetailId: str
+    ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
+        """
+        Retrieves the details for a Savings Plan recommendation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plan_purchase_recommendation_details)
+        """
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
@@ -635,15 +645,15 @@
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
         ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
-        Updates an existing cost anomaly monitor subscription.
+        Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
     def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
     ) -> UpdateCostAllocationTagsStatusResponseTypeDef:
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,14 +394,15 @@
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

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,15 @@
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

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -53,113 +53,130 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AnomalyDateIntervalTypeDef",
+    "AnomalyMonitorOutputTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
+    "SubscriberOutputTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
+    "CostCategoryInheritedValueDimensionOutputTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
+    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
-    "DateIntervalTypeDef",
+    "DateIntervalOutputTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "TagValuesTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagValuesOutputTypeDef",
+    "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
+    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
+    "EC2SpecificationOutputTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
+    "TagValuesTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
+    "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
+    "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
+    "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
+    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
+    "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
+    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
-    "GetCostForecastRequestRequestTypeDef",
-    "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExpressionTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetCostForecastRequestRequestTypeDef",
+    "GetUsageForecastRequestRequestTypeDef",
+    "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
+    "ServiceSpecificationOutputTypeDef",
     "ServiceSpecificationTypeDef",
+    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -168,35 +185,38 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
     "CreateCostCategoryDefinitionRequestRequestTypeDef",
     "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
@@ -223,20 +243,33 @@
     "_OptionalAnomalyDateIntervalTypeDef",
     {
         "EndDate": str,
     },
     total=False,
 )
 
-
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
+AnomalyMonitorOutputTypeDef = TypedDict(
+    "AnomalyMonitorOutputTypeDef",
+    {
+        "MonitorArn": str,
+        "MonitorName": str,
+        "CreationDate": str,
+        "LastUpdatedDate": str,
+        "LastEvaluatedDate": str,
+        "MonitorType": MonitorTypeType,
+        "MonitorDimension": Literal["SERVICE"],
+        "MonitorSpecification": "ExpressionOutputTypeDef",
+        "DimensionalValueCount": int,
+    },
+)
 
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
@@ -251,69 +284,64 @@
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionTypeDef",
         "DimensionalValueCount": int,
     },
     total=False,
 )
 
-
 class AnomalyMonitorTypeDef(_RequiredAnomalyMonitorTypeDef, _OptionalAnomalyMonitorTypeDef):
     pass
 
-
 AnomalyScoreTypeDef = TypedDict(
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
 
+SubscriberOutputTypeDef = TypedDict(
+    "SubscriberOutputTypeDef",
+    {
+        "Address": str,
+        "Type": SubscriberTypeType,
+        "Status": SubscriberStatusType,
+    },
+)
+
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
     total=False,
 )
 
-_RequiredImpactTypeDef = TypedDict(
-    "_RequiredImpactTypeDef",
+ImpactTypeDef = TypedDict(
+    "ImpactTypeDef",
     {
         "MaxImpact": float,
-    },
-)
-_OptionalImpactTypeDef = TypedDict(
-    "_OptionalImpactTypeDef",
-    {
         "TotalImpact": float,
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
-    total=False,
 )
 
-
-class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
-    pass
-
-
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
         "LinkedAccountName": str,
     },
-    total=False,
 )
 
 CostAllocationTagStatusEntryTypeDef = TypedDict(
     "CostAllocationTagStatusEntryTypeDef",
     {
         "TagKey": str,
         "Status": CostAllocationTagStatusType,
@@ -325,14 +353,22 @@
     {
         "TagKey": str,
         "Type": CostAllocationTagTypeType,
         "Status": CostAllocationTagStatusType,
     },
 )
 
+CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
+    "CostCategoryInheritedValueDimensionOutputTypeDef",
+    {
+        "DimensionName": CostCategoryInheritedValueDimensionNameType,
+        "DimensionKey": str,
+    },
+)
+
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
     total=False,
@@ -340,114 +376,120 @@
 
 CostCategoryProcessingStatusTypeDef = TypedDict(
     "CostCategoryProcessingStatusTypeDef",
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
-    total=False,
+)
+
+CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
+    {
+        "Type": Literal["ALLOCATION_PERCENTAGES"],
+        "Values": List[str],
+    },
 )
 
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
+CostCategoryValuesOutputTypeDef = TypedDict(
+    "CostCategoryValuesOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+)
+
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalTypeDef = TypedDict(
-    "DateIntervalTypeDef",
+DateIntervalOutputTypeDef = TypedDict(
+    "DateIntervalOutputTypeDef",
     {
         "Start": str,
         "End": str,
     },
 )
 
 CoverageCostTypeDef = TypedDict(
     "CoverageCostTypeDef",
     {
         "OnDemandCost": str,
     },
-    total=False,
 )
 
 CoverageHoursTypeDef = TypedDict(
     "CoverageHoursTypeDef",
     {
         "OnDemandHours": str,
         "ReservedHours": str,
         "TotalRunningHours": str,
         "CoverageHoursPercentage": str,
     },
-    total=False,
 )
 
 CoverageNormalizedUnitsTypeDef = TypedDict(
     "CoverageNormalizedUnitsTypeDef",
     {
         "OnDemandNormalizedUnits": str,
         "ReservedNormalizedUnits": str,
         "TotalRunningNormalizedUnits": str,
         "CoverageNormalizedUnitsPercentage": str,
     },
-    total=False,
 )
 
 ResourceTagTypeDef = TypedDict(
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+TagValuesOutputTypeDef = TypedDict(
+    "TagValuesOutputTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
     },
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
     {
-        "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
+        "Start": str,
+        "End": str,
     },
-    total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
@@ -463,44 +505,42 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveOn": str,
     },
     total=False,
 )
 
-
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+DimensionValuesOutputTypeDef = TypedDict(
+    "DimensionValuesOutputTypeDef",
+    {
+        "Key": DimensionType,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+)
 
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
@@ -510,52 +550,48 @@
 
 DimensionValuesWithAttributesTypeDef = TypedDict(
     "DimensionValuesWithAttributesTypeDef",
     {
         "Value": str,
         "Attributes": Dict[str, str],
     },
-    total=False,
 )
 
 DiskResourceUtilizationTypeDef = TypedDict(
     "DiskResourceUtilizationTypeDef",
     {
         "DiskReadOpsPerSecond": str,
         "DiskWriteOpsPerSecond": str,
         "DiskReadBytesPerSecond": str,
         "DiskWriteBytesPerSecond": str,
     },
-    total=False,
 )
 
 EBSResourceUtilizationTypeDef = TypedDict(
     "EBSResourceUtilizationTypeDef",
     {
         "EbsReadOpsPerSecond": str,
         "EbsWriteOpsPerSecond": str,
         "EbsReadBytesPerSecond": str,
         "EbsWriteBytesPerSecond": str,
     },
-    total=False,
 )
 
 EC2InstanceDetailsTypeDef = TypedDict(
     "EC2InstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "AvailabilityZone": str,
         "Platform": str,
         "Tenancy": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 EC2ResourceDetailsTypeDef = TypedDict(
     "EC2ResourceDetailsTypeDef",
     {
         "HourlyOnDemandRate": str,
         "InstanceType": str,
@@ -563,26 +599,31 @@
         "Region": str,
         "Sku": str,
         "Memory": str,
         "NetworkPerformance": str,
         "Storage": str,
         "Vcpu": str,
     },
-    total=False,
 )
 
 NetworkResourceUtilizationTypeDef = TypedDict(
     "NetworkResourceUtilizationTypeDef",
     {
         "NetworkInBytesPerSecond": str,
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
-    total=False,
+)
+
+EC2SpecificationOutputTypeDef = TypedDict(
+    "EC2SpecificationOutputTypeDef",
+    {
+        "OfferingClass": OfferingClassType,
+    },
 )
 
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
@@ -594,40 +635,47 @@
     {
         "InstanceClass": str,
         "InstanceSize": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 ElastiCacheInstanceDetailsTypeDef = TypedDict(
     "ElastiCacheInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+)
+
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
+    },
     total=False,
 )
 
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
         "EstimatedCompletionTime": str,
     },
-    total=False,
 )
 
 _RequiredTotalImpactFilterTypeDef = TypedDict(
     "_RequiredTotalImpactFilterTypeDef",
     {
         "NumericOperator": NumericOperatorType,
         "StartValue": float,
@@ -637,21 +685,19 @@
     "_OptionalTotalImpactFilterTypeDef",
     {
         "EndValue": float,
     },
     total=False,
 )
 
-
 class TotalImpactFilterTypeDef(
     _RequiredTotalImpactFilterTypeDef, _OptionalTotalImpactFilterTypeDef
 ):
     pass
 
-
 GetAnomalyMonitorsRequestRequestTypeDef = TypedDict(
     "GetAnomalyMonitorsRequestRequestTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "NextPageToken": str,
         "MaxResults": int,
     },
@@ -674,61 +720,53 @@
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
     total=False,
 )
 
+GroupDefinitionOutputTypeDef = TypedDict(
+    "GroupDefinitionOutputTypeDef",
+    {
+        "Type": GroupDefinitionTypeType,
+        "Key": str,
+    },
+)
+
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalSortDefinitionTypeDef = TypedDict(
     "_OptionalSortDefinitionTypeDef",
     {
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
-    total=False,
 )
 
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
     },
-    total=False,
 )
 
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": str,
         "UtilizationPercentageInUnits": str,
@@ -744,45 +782,57 @@
         "AmortizedUpfrontFee": str,
         "AmortizedRecurringFee": str,
         "TotalAmortizedFee": str,
         "RICostForUnusedHours": str,
         "RealizedSavings": str,
         "UnrealizedSavings": str,
     },
-    total=False,
 )
 
 RightsizingRecommendationConfigurationTypeDef = TypedDict(
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
     },
 )
 
+RightsizingRecommendationConfigurationOutputTypeDef = TypedDict(
+    "RightsizingRecommendationConfigurationOutputTypeDef",
+    {
+        "RecommendationTarget": RecommendationTargetType,
+        "BenefitsConsidered": bool,
+    },
+)
+
 RightsizingRecommendationMetadataTypeDef = TypedDict(
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
     },
-    total=False,
 )
 
 RightsizingRecommendationSummaryTypeDef = TypedDict(
     "RightsizingRecommendationSummaryTypeDef",
     {
         "TotalRecommendationCount": str,
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
-    total=False,
+)
+
+GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
+    {
+        "RecommendationDetailId": str,
+    },
 )
 
 _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     {
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
@@ -797,41 +847,27 @@
         "NextPageToken": str,
         "PageSize": int,
         "Filter": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
-    total=False,
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
@@ -839,27 +875,25 @@
         "DatabaseEngine": str,
         "DatabaseEdition": str,
         "DeploymentOption": str,
         "LicenseModel": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 RedshiftInstanceDetailsTypeDef = TypedDict(
     "RedshiftInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 ListCostAllocationTagsRequestRequestTypeDef = TypedDict(
     "ListCostAllocationTagsRequestRequestTypeDef",
     {
         "Status": CostAllocationTagStatusType,
         "TagKeys": Sequence[str],
@@ -894,89 +928,84 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ResourceTagOutputTypeDef = TypedDict(
+    "ResourceTagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ProvideAnomalyFeedbackRequestRequestTypeDef = TypedDict(
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
+RecommendationDetailHourlyMetricsTypeDef = TypedDict(
+    "RecommendationDetailHourlyMetricsTypeDef",
     {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTime": str,
+        "EstimatedOnDemandCost": str,
+        "CurrentCoverage": str,
+        "EstimatedCoverage": str,
+        "EstimatedNewCommitmentUtilization": str,
     },
 )
 
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
-    total=False,
 )
 
 SavingsPlansAmortizedCommitmentTypeDef = TypedDict(
     "SavingsPlansAmortizedCommitmentTypeDef",
     {
         "AmortizedRecurringCommitment": str,
         "AmortizedUpfrontCommitment": str,
         "TotalAmortizedCommitment": str,
     },
-    total=False,
 )
 
 SavingsPlansCoverageDataTypeDef = TypedDict(
     "SavingsPlansCoverageDataTypeDef",
     {
         "SpendCoveredBySavingsPlans": str,
         "OnDemandCost": str,
         "TotalCost": str,
         "CoveragePercentage": str,
     },
-    total=False,
 )
 
 SavingsPlansDetailsTypeDef = TypedDict(
     "SavingsPlansDetailsTypeDef",
     {
         "Region": str,
         "InstanceFamily": str,
         "OfferingId": str,
     },
-    total=False,
 )
 
 SavingsPlansPurchaseRecommendationSummaryTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     {
         "EstimatedROI": str,
         "CurrencyCode": str,
@@ -986,45 +1015,32 @@
         "TotalRecommendationCount": str,
         "DailyCommitmentToPurchase": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedSavingsPercentage": str,
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedOnDemandCostWithCurrentCommitment": str,
     },
-    total=False,
 )
 
 SavingsPlansSavingsTypeDef = TypedDict(
     "SavingsPlansSavingsTypeDef",
     {
         "NetSavings": str,
         "OnDemandCostEquivalent": str,
     },
-    total=False,
 )
 
 SavingsPlansUtilizationTypeDef = TypedDict(
     "SavingsPlansUtilizationTypeDef",
     {
         "TotalCommitment": str,
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
-    total=False,
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
@@ -1041,63 +1057,40 @@
     "_OptionalUpdateAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
     },
     total=False,
 )
 
-
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+AnomalySubscriptionOutputTypeDef = TypedDict(
+    "AnomalySubscriptionOutputTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "MonitorArnList": List[str],
+        "Subscribers": List[SubscriberOutputTypeDef],
+        "Threshold": float,
+        "Frequency": AnomalySubscriptionFrequencyType,
+        "SubscriptionName": str,
+        "ThresholdExpression": "ExpressionOutputTypeDef",
     },
 )
 
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
@@ -1113,21 +1106,19 @@
         "AccountId": str,
         "Threshold": float,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class AnomalySubscriptionTypeDef(
     _RequiredAnomalySubscriptionTypeDef, _OptionalAnomalySubscriptionTypeDef
 ):
     pass
 
-
 _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalySubscriptionRequestRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1139,61 +1130,49 @@
         "Subscribers": Sequence[SubscriberTypeDef],
         "SubscriptionName": str,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredAnomalyTypeDef = TypedDict(
-    "_RequiredAnomalyTypeDef",
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
     {
         "AnomalyId": str,
-        "AnomalyScore": AnomalyScoreTypeDef,
-        "Impact": ImpactTypeDef,
-        "MonitorArn": str,
-    },
-)
-_OptionalAnomalyTypeDef = TypedDict(
-    "_OptionalAnomalyTypeDef",
-    {
         "AnomalyStartDate": str,
         "AnomalyEndDate": str,
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
+        "AnomalyScore": AnomalyScoreTypeDef,
+        "Impact": ImpactTypeDef,
+        "MonitorArn": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
-    total=False,
 )
 
-
-class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
-    pass
-
-
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
+CostCategoryRuleOutputTypeDef = TypedDict(
+    "CostCategoryRuleOutputTypeDef",
     {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Value": str,
+        "Rule": "ExpressionOutputTypeDef",
+        "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
+        "Type": CostCategoryRuleTypeType,
     },
 )
 
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
@@ -1212,15 +1191,24 @@
         "EffectiveStart": str,
         "EffectiveEnd": str,
         "NumberOfRules": int,
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
-    total=False,
+)
+
+CostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Source": str,
+        "Targets": List[str],
+        "Method": CostCategorySplitChargeMethodType,
+        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
+    },
 )
 
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
@@ -1231,32 +1219,184 @@
     "_OptionalCostCategorySplitChargeRuleTypeDef",
     {
         "Parameters": Sequence[CostCategorySplitChargeRuleParameterTypeDef],
     },
     total=False,
 )
 
-
 class CostCategorySplitChargeRuleTypeDef(
     _RequiredCostCategorySplitChargeRuleTypeDef, _OptionalCostCategorySplitChargeRuleTypeDef
 ):
     pass
 
-
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
+)
+
+CoverageTypeDef = TypedDict(
+    "CoverageTypeDef",
+    {
+        "CoverageHours": CoverageHoursTypeDef,
+        "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
+        "CoverageCost": CoverageCostTypeDef,
+    },
+)
+
+_RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
+    {
+        "AnomalyMonitor": AnomalyMonitorTypeDef,
+    },
+)
+_OptionalCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
     total=False,
 )
 
+class CreateAnomalyMonitorRequestRequestTypeDef(
+    _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
+    _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
+):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+)
+
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1266,21 +1406,19 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
-
 class GetCostForecastRequestRequestTypeDef(
     _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1290,128 +1428,95 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
-
 class GetUsageForecastRequestRequestTypeDef(
     _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
 ):
     pass
 
-
-CoverageTypeDef = TypedDict(
-    "CoverageTypeDef",
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
     {
-        "CoverageHours": CoverageHoursTypeDef,
-        "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
-        "CoverageCost": CoverageCostTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
-    {
-        "AnomalyMonitor": AnomalyMonitorTypeDef,
-    },
-)
-_OptionalCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
-    {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateAnomalyMonitorRequestRequestTypeDef(
-    _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
-    _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
-):
-    pass
-
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-)
-
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
-    {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
+        "Or": List[Dict[str, Any]],
+        "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
+        "Dimensions": DimensionValuesOutputTypeDef,
+        "Tags": TagValuesOutputTypeDef,
+        "CostCategories": CostCategoryValuesOutputTypeDef,
     },
-    total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
     },
-    total=False,
 )
 
 EC2ResourceUtilizationTypeDef = TypedDict(
     "EC2ResourceUtilizationTypeDef",
     {
         "MaxCpuUtilizationPercentage": str,
         "MaxMemoryUtilizationPercentage": str,
         "MaxStorageUtilizationPercentage": str,
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
-    total=False,
+)
+
+ServiceSpecificationOutputTypeDef = TypedDict(
+    "ServiceSpecificationOutputTypeDef",
+    {
+        "EC2Specification": EC2SpecificationOutputTypeDef,
+    },
 )
 
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
+    {
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
+        "Not": Dict[str, Any],
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
+    },
+    total=False,
+)
+
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1425,21 +1530,19 @@
         "TotalImpact": TotalImpactFilterTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetAnomaliesRequestRequestTypeDef(
     _RequiredGetAnomaliesRequestRequestTypeDef, _OptionalGetAnomaliesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetCostAndUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Metrics": Sequence[str],
     },
@@ -1450,21 +1553,19 @@
         "Filter": "ExpressionTypeDef",
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostAndUsageRequestRequestTypeDef(
     _RequiredGetCostAndUsageRequestRequestTypeDef, _OptionalGetCostAndUsageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
     },
@@ -1475,22 +1576,20 @@
         "Metrics": Sequence[str],
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostAndUsageWithResourcesRequestRequestTypeDef(
     _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef,
     _OptionalGetCostAndUsageWithResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCostCategoriesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostCategoriesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetCostCategoriesRequestRequestTypeDef = TypedDict(
@@ -1502,21 +1601,19 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostCategoriesRequestRequestTypeDef(
     _RequiredGetCostCategoriesRequestRequestTypeDef, _OptionalGetCostCategoriesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetDimensionValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDimensionValuesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Dimension": DimensionType,
     },
 )
@@ -1529,22 +1626,20 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetDimensionValuesRequestRequestTypeDef(
     _RequiredGetDimensionValuesRequestRequestTypeDef,
     _OptionalGetDimensionValuesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetReservationCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationCoverageRequestRequestTypeDef = TypedDict(
@@ -1557,22 +1652,20 @@
         "NextPageToken": str,
         "SortBy": SortDefinitionTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetReservationCoverageRequestRequestTypeDef(
     _RequiredGetReservationCoverageRequestRequestTypeDef,
     _OptionalGetReservationCoverageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetReservationUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationUtilizationRequestRequestTypeDef = TypedDict(
@@ -1584,22 +1677,20 @@
         "SortBy": SortDefinitionTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetReservationUtilizationRequestRequestTypeDef(
     _RequiredGetReservationUtilizationRequestRequestTypeDef,
     _OptionalGetReservationUtilizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
@@ -1612,22 +1703,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansCoverageRequestRequestTypeDef(
     _RequiredGetSavingsPlansCoverageRequestRequestTypeDef,
     _OptionalGetSavingsPlansCoverageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
@@ -1638,22 +1727,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansUtilizationDetailsRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
@@ -1662,22 +1749,20 @@
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansUtilizationRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTagsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetTagsRequestRequestTypeDef = TypedDict(
@@ -1689,39 +1774,35 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetTagsRequestRequestTypeDef(
     _RequiredGetTagsRequestRequestTypeDef, _OptionalGetTagsRequestRequestTypeDef
 ):
     pass
 
-
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
-    total=False,
 )
 
 ReservationUtilizationGroupTypeDef = TypedDict(
     "ReservationUtilizationGroupTypeDef",
     {
         "Key": str,
         "Value": str,
         "Attributes": Dict[str, str],
         "Utilization": ReservationAggregatesTypeDef,
     },
-    total=False,
 )
 
 _RequiredGetRightsizingRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetRightsizingRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -1733,42 +1814,81 @@
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetRightsizingRecommendationRequestRequestTypeDef(
     _RequiredGetRightsizingRecommendationRequestRequestTypeDef,
     _OptionalGetRightsizingRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceDetailsTypeDef = TypedDict(
     "InstanceDetailsTypeDef",
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
-    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommendationDetailDataTypeDef = TypedDict(
+    "RecommendationDetailDataTypeDef",
+    {
+        "AccountScope": AccountScopeType,
+        "LookbackPeriodInDays": LookbackPeriodInDaysType,
+        "SavingsPlansType": SupportedSavingsPlansTypeType,
+        "TermInYears": TermInYearsType,
+        "PaymentOption": PaymentOptionType,
+        "AccountId": str,
+        "CurrencyCode": str,
+        "InstanceFamily": str,
+        "Region": str,
+        "OfferingId": str,
+        "GenerationTimestamp": str,
+        "LatestUsageTimestamp": str,
+        "CurrentAverageHourlyOnDemandSpend": str,
+        "CurrentMaximumHourlyOnDemandSpend": str,
+        "CurrentMinimumHourlyOnDemandSpend": str,
+        "EstimatedAverageUtilization": str,
+        "EstimatedMonthlySavingsAmount": str,
+        "EstimatedOnDemandCost": str,
+        "EstimatedOnDemandCostWithCurrentCommitment": str,
+        "EstimatedROI": str,
+        "EstimatedSPCost": str,
+        "EstimatedSavingsAmount": str,
+        "EstimatedSavingsPercentage": str,
+        "ExistingHourlyCommitment": str,
+        "HourlyCommitmentToPurchase": str,
+        "UpfrontCost": str,
+        "CurrentAverageCoverage": str,
+        "EstimatedAverageCoverage": str,
+        "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
+    },
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
     },
-    total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
         "SavingsPlansDetails": SavingsPlansDetailsTypeDef,
         "AccountId": str,
@@ -1782,81 +1902,62 @@
         "EstimatedSavingsPercentage": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
+        "RecommendationDetailId": str,
     },
-    total=False,
 )
 
-_RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
+SavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "SavingsPlansUtilizationAggregatesTypeDef",
     {
         "Utilization": SavingsPlansUtilizationTypeDef,
-    },
-)
-_OptionalSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "_OptionalSavingsPlansUtilizationAggregatesTypeDef",
-    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
-
-class SavingsPlansUtilizationAggregatesTypeDef(
-    _RequiredSavingsPlansUtilizationAggregatesTypeDef,
-    _OptionalSavingsPlansUtilizationAggregatesTypeDef,
-):
-    pass
-
-
-_RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "_RequiredSavingsPlansUtilizationByTimeTypeDef",
+SavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "SavingsPlansUtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
-    },
-)
-_OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "_OptionalSavingsPlansUtilizationByTimeTypeDef",
-    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
-
-class SavingsPlansUtilizationByTimeTypeDef(
-    _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
-):
-    pass
-
-
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -1866,75 +1967,53 @@
     "_OptionalCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCostCategoryTypeDef = TypedDict(
-    "_RequiredCostCategoryTypeDef",
+CostCategoryTypeDef = TypedDict(
+    "CostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
+        "EffectiveEnd": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": List[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCostCategoryTypeDef = TypedDict(
-    "_OptionalCostCategoryTypeDef",
-    {
-        "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
+        "Rules": List[CostCategoryRuleOutputTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
-    total=False,
 )
 
-
-class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
-    pass
-
-
 _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -1946,22 +2025,20 @@
         "DefaultValue": str,
         "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -1972,55 +2049,51 @@
         "EffectiveStart": str,
         "DefaultValue": str,
         "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": CoverageTypeDef,
     },
-    total=False,
 )
 
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "EC2ResourceUtilization": EC2ResourceUtilizationTypeDef,
     },
-    total=False,
 )
 
 _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -2037,41 +2110,37 @@
         "ServiceSpecification": ServiceSpecificationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetReservationPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetReservationPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
-    total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
-    total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
     "ReservationPurchaseRecommendationDetailTypeDef",
     {
         "AccountId": str,
         "InstanceDetails": InstanceDetailsTypeDef,
@@ -2089,23 +2158,31 @@
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedMonthlySavingsPercentage": str,
         "EstimatedMonthlyOnDemandCost": str,
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
-    total=False,
+)
+
+GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
+    {
+        "RecommendationDetailId": str,
+        "RecommendationDetailData": RecommendationDetailDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2116,188 +2193,181 @@
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
         "SavingsPlansPurchaseRecommendationSummary": (
             SavingsPlansPurchaseRecommendationSummaryTypeDef
         ),
     },
-    total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
-    total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesTypeDef],
+        "Tags": List[TagValuesOutputTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
         "CurrencyCode": str,
     },
-    total=False,
 )
 
 TargetInstanceTypeDef = TypedDict(
     "TargetInstanceTypeDef",
     {
         "EstimatedMonthlyCost": str,
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
         "DefaultTargetInstance": bool,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ExpectedResourceUtilization": ResourceUtilizationTypeDef,
         "PlatformDifferences": List[PlatformDifferenceType],
     },
-    total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionTypeDef],
+        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionTypeDef],
+        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
-        "ServiceSpecification": ServiceSpecificationTypeDef,
+        "ServiceSpecification": ServiceSpecificationOutputTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
-    total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
     },
-    total=False,
 )
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
         "CurrentInstance": CurrentInstanceTypeDef,
         "RightsizingType": RightsizingTypeType,
         "ModifyRecommendationDetail": ModifyRecommendationDetailTypeDef,
         "TerminateRecommendationDetail": TerminateRecommendationDetailTypeDef,
         "FindingReasonCodes": List[FindingReasonCodeType],
     },
-    total=False,
 )
 
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
-        "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,112 +53,131 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AnomalyDateIntervalTypeDef",
+    "AnomalyMonitorOutputTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
+    "SubscriberOutputTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
+    "CostCategoryInheritedValueDimensionOutputTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
+    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
-    "DateIntervalTypeDef",
+    "DateIntervalOutputTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "TagValuesTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagValuesOutputTypeDef",
+    "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
+    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
+    "EC2SpecificationOutputTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
+    "TagValuesTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
+    "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
+    "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
+    "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
+    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
+    "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
+    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
-    "GetCostForecastRequestRequestTypeDef",
-    "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExpressionTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetCostForecastRequestRequestTypeDef",
+    "GetUsageForecastRequestRequestTypeDef",
+    "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
+    "ServiceSpecificationOutputTypeDef",
     "ServiceSpecificationTypeDef",
+    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -167,35 +186,38 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
     "CreateCostCategoryDefinitionRequestRequestTypeDef",
     "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
@@ -222,19 +244,36 @@
     "_OptionalAnomalyDateIntervalTypeDef",
     {
         "EndDate": str,
     },
     total=False,
 )
 
+
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
+
+AnomalyMonitorOutputTypeDef = TypedDict(
+    "AnomalyMonitorOutputTypeDef",
+    {
+        "MonitorArn": str,
+        "MonitorName": str,
+        "CreationDate": str,
+        "LastUpdatedDate": str,
+        "LastEvaluatedDate": str,
+        "MonitorType": MonitorTypeType,
+        "MonitorDimension": Literal["SERVICE"],
+        "MonitorSpecification": "ExpressionOutputTypeDef",
+        "DimensionalValueCount": int,
+    },
+)
+
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -248,65 +287,66 @@
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionTypeDef",
         "DimensionalValueCount": int,
     },
     total=False,
 )
 
+
 class AnomalyMonitorTypeDef(_RequiredAnomalyMonitorTypeDef, _OptionalAnomalyMonitorTypeDef):
     pass
 
+
 AnomalyScoreTypeDef = TypedDict(
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
 
+SubscriberOutputTypeDef = TypedDict(
+    "SubscriberOutputTypeDef",
+    {
+        "Address": str,
+        "Type": SubscriberTypeType,
+        "Status": SubscriberStatusType,
+    },
+)
+
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
     total=False,
 )
 
-_RequiredImpactTypeDef = TypedDict(
-    "_RequiredImpactTypeDef",
+ImpactTypeDef = TypedDict(
+    "ImpactTypeDef",
     {
         "MaxImpact": float,
-    },
-)
-_OptionalImpactTypeDef = TypedDict(
-    "_OptionalImpactTypeDef",
-    {
         "TotalImpact": float,
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
-    total=False,
 )
 
-class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
-    pass
-
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
         "LinkedAccountName": str,
     },
-    total=False,
 )
 
 CostAllocationTagStatusEntryTypeDef = TypedDict(
     "CostAllocationTagStatusEntryTypeDef",
     {
         "TagKey": str,
         "Status": CostAllocationTagStatusType,
@@ -318,14 +358,22 @@
     {
         "TagKey": str,
         "Type": CostAllocationTagTypeType,
         "Status": CostAllocationTagStatusType,
     },
 )
 
+CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
+    "CostCategoryInheritedValueDimensionOutputTypeDef",
+    {
+        "DimensionName": CostCategoryInheritedValueDimensionNameType,
+        "DimensionKey": str,
+    },
+)
+
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
     total=False,
@@ -333,114 +381,120 @@
 
 CostCategoryProcessingStatusTypeDef = TypedDict(
     "CostCategoryProcessingStatusTypeDef",
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
-    total=False,
+)
+
+CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
+    {
+        "Type": Literal["ALLOCATION_PERCENTAGES"],
+        "Values": List[str],
+    },
 )
 
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
+CostCategoryValuesOutputTypeDef = TypedDict(
+    "CostCategoryValuesOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+)
+
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalTypeDef = TypedDict(
-    "DateIntervalTypeDef",
+DateIntervalOutputTypeDef = TypedDict(
+    "DateIntervalOutputTypeDef",
     {
         "Start": str,
         "End": str,
     },
 )
 
 CoverageCostTypeDef = TypedDict(
     "CoverageCostTypeDef",
     {
         "OnDemandCost": str,
     },
-    total=False,
 )
 
 CoverageHoursTypeDef = TypedDict(
     "CoverageHoursTypeDef",
     {
         "OnDemandHours": str,
         "ReservedHours": str,
         "TotalRunningHours": str,
         "CoverageHoursPercentage": str,
     },
-    total=False,
 )
 
 CoverageNormalizedUnitsTypeDef = TypedDict(
     "CoverageNormalizedUnitsTypeDef",
     {
         "OnDemandNormalizedUnits": str,
         "ReservedNormalizedUnits": str,
         "TotalRunningNormalizedUnits": str,
         "CoverageNormalizedUnitsPercentage": str,
     },
-    total=False,
 )
 
 ResourceTagTypeDef = TypedDict(
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+TagValuesOutputTypeDef = TypedDict(
+    "TagValuesOutputTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
     },
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
     {
-        "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
+        "Start": str,
+        "End": str,
     },
-    total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
@@ -456,43 +510,45 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveOn": str,
     },
     total=False,
 )
 
+
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
+DimensionValuesOutputTypeDef = TypedDict(
+    "DimensionValuesOutputTypeDef",
+    {
+        "Key": DimensionType,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+)
+
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -501,52 +557,48 @@
 
 DimensionValuesWithAttributesTypeDef = TypedDict(
     "DimensionValuesWithAttributesTypeDef",
     {
         "Value": str,
         "Attributes": Dict[str, str],
     },
-    total=False,
 )
 
 DiskResourceUtilizationTypeDef = TypedDict(
     "DiskResourceUtilizationTypeDef",
     {
         "DiskReadOpsPerSecond": str,
         "DiskWriteOpsPerSecond": str,
         "DiskReadBytesPerSecond": str,
         "DiskWriteBytesPerSecond": str,
     },
-    total=False,
 )
 
 EBSResourceUtilizationTypeDef = TypedDict(
     "EBSResourceUtilizationTypeDef",
     {
         "EbsReadOpsPerSecond": str,
         "EbsWriteOpsPerSecond": str,
         "EbsReadBytesPerSecond": str,
         "EbsWriteBytesPerSecond": str,
     },
-    total=False,
 )
 
 EC2InstanceDetailsTypeDef = TypedDict(
     "EC2InstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "AvailabilityZone": str,
         "Platform": str,
         "Tenancy": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 EC2ResourceDetailsTypeDef = TypedDict(
     "EC2ResourceDetailsTypeDef",
     {
         "HourlyOnDemandRate": str,
         "InstanceType": str,
@@ -554,26 +606,31 @@
         "Region": str,
         "Sku": str,
         "Memory": str,
         "NetworkPerformance": str,
         "Storage": str,
         "Vcpu": str,
     },
-    total=False,
 )
 
 NetworkResourceUtilizationTypeDef = TypedDict(
     "NetworkResourceUtilizationTypeDef",
     {
         "NetworkInBytesPerSecond": str,
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
-    total=False,
+)
+
+EC2SpecificationOutputTypeDef = TypedDict(
+    "EC2SpecificationOutputTypeDef",
+    {
+        "OfferingClass": OfferingClassType,
+    },
 )
 
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
@@ -585,40 +642,47 @@
     {
         "InstanceClass": str,
         "InstanceSize": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 ElastiCacheInstanceDetailsTypeDef = TypedDict(
     "ElastiCacheInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+)
+
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
+    },
     total=False,
 )
 
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
         "EstimatedCompletionTime": str,
     },
-    total=False,
 )
 
 _RequiredTotalImpactFilterTypeDef = TypedDict(
     "_RequiredTotalImpactFilterTypeDef",
     {
         "NumericOperator": NumericOperatorType,
         "StartValue": float,
@@ -628,19 +692,21 @@
     "_OptionalTotalImpactFilterTypeDef",
     {
         "EndValue": float,
     },
     total=False,
 )
 
+
 class TotalImpactFilterTypeDef(
     _RequiredTotalImpactFilterTypeDef, _OptionalTotalImpactFilterTypeDef
 ):
     pass
 
+
 GetAnomalyMonitorsRequestRequestTypeDef = TypedDict(
     "GetAnomalyMonitorsRequestRequestTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "NextPageToken": str,
         "MaxResults": int,
     },
@@ -663,59 +729,55 @@
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
     total=False,
 )
 
+GroupDefinitionOutputTypeDef = TypedDict(
+    "GroupDefinitionOutputTypeDef",
+    {
+        "Type": GroupDefinitionTypeType,
+        "Key": str,
+    },
+)
+
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalSortDefinitionTypeDef = TypedDict(
     "_OptionalSortDefinitionTypeDef",
     {
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
+
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
-    total=False,
 )
 
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
     },
-    total=False,
 )
 
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": str,
         "UtilizationPercentageInUnits": str,
@@ -731,45 +793,57 @@
         "AmortizedUpfrontFee": str,
         "AmortizedRecurringFee": str,
         "TotalAmortizedFee": str,
         "RICostForUnusedHours": str,
         "RealizedSavings": str,
         "UnrealizedSavings": str,
     },
-    total=False,
 )
 
 RightsizingRecommendationConfigurationTypeDef = TypedDict(
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
     },
 )
 
+RightsizingRecommendationConfigurationOutputTypeDef = TypedDict(
+    "RightsizingRecommendationConfigurationOutputTypeDef",
+    {
+        "RecommendationTarget": RecommendationTargetType,
+        "BenefitsConsidered": bool,
+    },
+)
+
 RightsizingRecommendationMetadataTypeDef = TypedDict(
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
     },
-    total=False,
 )
 
 RightsizingRecommendationSummaryTypeDef = TypedDict(
     "RightsizingRecommendationSummaryTypeDef",
     {
         "TotalRecommendationCount": str,
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
-    total=False,
+)
+
+GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
+    {
+        "RecommendationDetailId": str,
+    },
 )
 
 _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     {
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
@@ -784,39 +858,29 @@
         "NextPageToken": str,
         "PageSize": int,
         "Filter": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
-    total=False,
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
@@ -824,27 +888,25 @@
         "DatabaseEngine": str,
         "DatabaseEdition": str,
         "DeploymentOption": str,
         "LicenseModel": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 RedshiftInstanceDetailsTypeDef = TypedDict(
     "RedshiftInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
-    total=False,
 )
 
 ListCostAllocationTagsRequestRequestTypeDef = TypedDict(
     "ListCostAllocationTagsRequestRequestTypeDef",
     {
         "Status": CostAllocationTagStatusType,
         "TagKeys": Sequence[str],
@@ -879,89 +941,84 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ResourceTagOutputTypeDef = TypedDict(
+    "ResourceTagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ProvideAnomalyFeedbackRequestRequestTypeDef = TypedDict(
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
+RecommendationDetailHourlyMetricsTypeDef = TypedDict(
+    "RecommendationDetailHourlyMetricsTypeDef",
     {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTime": str,
+        "EstimatedOnDemandCost": str,
+        "CurrentCoverage": str,
+        "EstimatedCoverage": str,
+        "EstimatedNewCommitmentUtilization": str,
     },
 )
 
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
-    total=False,
 )
 
 SavingsPlansAmortizedCommitmentTypeDef = TypedDict(
     "SavingsPlansAmortizedCommitmentTypeDef",
     {
         "AmortizedRecurringCommitment": str,
         "AmortizedUpfrontCommitment": str,
         "TotalAmortizedCommitment": str,
     },
-    total=False,
 )
 
 SavingsPlansCoverageDataTypeDef = TypedDict(
     "SavingsPlansCoverageDataTypeDef",
     {
         "SpendCoveredBySavingsPlans": str,
         "OnDemandCost": str,
         "TotalCost": str,
         "CoveragePercentage": str,
     },
-    total=False,
 )
 
 SavingsPlansDetailsTypeDef = TypedDict(
     "SavingsPlansDetailsTypeDef",
     {
         "Region": str,
         "InstanceFamily": str,
         "OfferingId": str,
     },
-    total=False,
 )
 
 SavingsPlansPurchaseRecommendationSummaryTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     {
         "EstimatedROI": str,
         "CurrencyCode": str,
@@ -971,45 +1028,32 @@
         "TotalRecommendationCount": str,
         "DailyCommitmentToPurchase": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedSavingsPercentage": str,
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedOnDemandCostWithCurrentCommitment": str,
     },
-    total=False,
 )
 
 SavingsPlansSavingsTypeDef = TypedDict(
     "SavingsPlansSavingsTypeDef",
     {
         "NetSavings": str,
         "OnDemandCostEquivalent": str,
     },
-    total=False,
 )
 
 SavingsPlansUtilizationTypeDef = TypedDict(
     "SavingsPlansUtilizationTypeDef",
     {
         "TotalCommitment": str,
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
-    total=False,
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
@@ -1026,61 +1070,42 @@
     "_OptionalUpdateAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
     },
     total=False,
 )
 
+
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
-    total=False,
-)
-
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
+AnomalySubscriptionOutputTypeDef = TypedDict(
+    "AnomalySubscriptionOutputTypeDef",
     {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "MonitorArnList": List[str],
+        "Subscribers": List[SubscriberOutputTypeDef],
+        "Threshold": float,
+        "Frequency": AnomalySubscriptionFrequencyType,
+        "SubscriptionName": str,
+        "ThresholdExpression": "ExpressionOutputTypeDef",
     },
 )
 
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
@@ -1096,19 +1121,21 @@
         "AccountId": str,
         "Threshold": float,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class AnomalySubscriptionTypeDef(
     _RequiredAnomalySubscriptionTypeDef, _OptionalAnomalySubscriptionTypeDef
 ):
     pass
 
+
 _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalySubscriptionRequestRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1120,57 +1147,51 @@
         "Subscribers": Sequence[SubscriberTypeDef],
         "SubscriptionName": str,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAnomalyTypeDef = TypedDict(
-    "_RequiredAnomalyTypeDef",
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
     {
         "AnomalyId": str,
-        "AnomalyScore": AnomalyScoreTypeDef,
-        "Impact": ImpactTypeDef,
-        "MonitorArn": str,
-    },
-)
-_OptionalAnomalyTypeDef = TypedDict(
-    "_OptionalAnomalyTypeDef",
-    {
         "AnomalyStartDate": str,
         "AnomalyEndDate": str,
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
+        "AnomalyScore": AnomalyScoreTypeDef,
+        "Impact": ImpactTypeDef,
+        "MonitorArn": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
-    total=False,
 )
 
-class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
-    pass
-
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
+CostCategoryRuleOutputTypeDef = TypedDict(
+    "CostCategoryRuleOutputTypeDef",
     {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Value": str,
+        "Rule": "ExpressionOutputTypeDef",
+        "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
+        "Type": CostCategoryRuleTypeType,
     },
 )
 
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
@@ -1189,15 +1210,24 @@
         "EffectiveStart": str,
         "EffectiveEnd": str,
         "NumberOfRules": int,
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
-    total=False,
+)
+
+CostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Source": str,
+        "Targets": List[str],
+        "Method": CostCategorySplitChargeMethodType,
+        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
+    },
 )
 
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
@@ -1208,30 +1238,188 @@
     "_OptionalCostCategorySplitChargeRuleTypeDef",
     {
         "Parameters": Sequence[CostCategorySplitChargeRuleParameterTypeDef],
     },
     total=False,
 )
 
+
 class CostCategorySplitChargeRuleTypeDef(
     _RequiredCostCategorySplitChargeRuleTypeDef, _OptionalCostCategorySplitChargeRuleTypeDef
 ):
     pass
 
+
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
+)
+
+CoverageTypeDef = TypedDict(
+    "CoverageTypeDef",
+    {
+        "CoverageHours": CoverageHoursTypeDef,
+        "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
+        "CoverageCost": CoverageCostTypeDef,
+    },
+)
+
+_RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
+    {
+        "AnomalyMonitor": AnomalyMonitorTypeDef,
+    },
+)
+_OptionalCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
     total=False,
 )
 
+
+class CreateAnomalyMonitorRequestRequestTypeDef(
+    _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
+    _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
+):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+)
+
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1241,19 +1429,21 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
+
 class GetCostForecastRequestRequestTypeDef(
     _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1263,124 +1453,97 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
+
 class GetUsageForecastRequestRequestTypeDef(
     _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
 ):
     pass
 
-CoverageTypeDef = TypedDict(
-    "CoverageTypeDef",
-    {
-        "CoverageHours": CoverageHoursTypeDef,
-        "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
-        "CoverageCost": CoverageCostTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
-    {
-        "AnomalyMonitor": AnomalyMonitorTypeDef,
-    },
-)
-_OptionalCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
-    {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-class CreateAnomalyMonitorRequestRequestTypeDef(
-    _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
-    _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
-):
-    pass
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-)
 
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
     {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
+        "Or": List[Dict[str, Any]],
+        "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
+        "Dimensions": DimensionValuesOutputTypeDef,
+        "Tags": TagValuesOutputTypeDef,
+        "CostCategories": CostCategoryValuesOutputTypeDef,
     },
-    total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
     },
-    total=False,
 )
 
 EC2ResourceUtilizationTypeDef = TypedDict(
     "EC2ResourceUtilizationTypeDef",
     {
         "MaxCpuUtilizationPercentage": str,
         "MaxMemoryUtilizationPercentage": str,
         "MaxStorageUtilizationPercentage": str,
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
-    total=False,
+)
+
+ServiceSpecificationOutputTypeDef = TypedDict(
+    "ServiceSpecificationOutputTypeDef",
+    {
+        "EC2Specification": EC2SpecificationOutputTypeDef,
+    },
 )
 
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
+    {
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
+        "Not": Dict[str, Any],
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
+    },
+    total=False,
+)
+
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1394,19 +1557,21 @@
         "TotalImpact": TotalImpactFilterTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetAnomaliesRequestRequestTypeDef(
     _RequiredGetAnomaliesRequestRequestTypeDef, _OptionalGetAnomaliesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetCostAndUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Metrics": Sequence[str],
     },
@@ -1417,19 +1582,21 @@
         "Filter": "ExpressionTypeDef",
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostAndUsageRequestRequestTypeDef(
     _RequiredGetCostAndUsageRequestRequestTypeDef, _OptionalGetCostAndUsageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
     },
@@ -1440,20 +1607,22 @@
         "Metrics": Sequence[str],
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostAndUsageWithResourcesRequestRequestTypeDef(
     _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef,
     _OptionalGetCostAndUsageWithResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCostCategoriesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostCategoriesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetCostCategoriesRequestRequestTypeDef = TypedDict(
@@ -1465,19 +1634,21 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostCategoriesRequestRequestTypeDef(
     _RequiredGetCostCategoriesRequestRequestTypeDef, _OptionalGetCostCategoriesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetDimensionValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDimensionValuesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Dimension": DimensionType,
     },
 )
@@ -1490,20 +1661,22 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetDimensionValuesRequestRequestTypeDef(
     _RequiredGetDimensionValuesRequestRequestTypeDef,
     _OptionalGetDimensionValuesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetReservationCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationCoverageRequestRequestTypeDef = TypedDict(
@@ -1516,20 +1689,22 @@
         "NextPageToken": str,
         "SortBy": SortDefinitionTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetReservationCoverageRequestRequestTypeDef(
     _RequiredGetReservationCoverageRequestRequestTypeDef,
     _OptionalGetReservationCoverageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetReservationUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationUtilizationRequestRequestTypeDef = TypedDict(
@@ -1541,20 +1716,22 @@
         "SortBy": SortDefinitionTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetReservationUtilizationRequestRequestTypeDef(
     _RequiredGetReservationUtilizationRequestRequestTypeDef,
     _OptionalGetReservationUtilizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
@@ -1567,20 +1744,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansCoverageRequestRequestTypeDef(
     _RequiredGetSavingsPlansCoverageRequestRequestTypeDef,
     _OptionalGetSavingsPlansCoverageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
@@ -1591,20 +1770,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansUtilizationDetailsRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
@@ -1613,20 +1794,22 @@
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansUtilizationRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTagsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetTagsRequestRequestTypeDef = TypedDict(
@@ -1638,37 +1821,37 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetTagsRequestRequestTypeDef(
     _RequiredGetTagsRequestRequestTypeDef, _OptionalGetTagsRequestRequestTypeDef
 ):
     pass
 
+
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
-    total=False,
 )
 
 ReservationUtilizationGroupTypeDef = TypedDict(
     "ReservationUtilizationGroupTypeDef",
     {
         "Key": str,
         "Value": str,
         "Attributes": Dict[str, str],
         "Utilization": ReservationAggregatesTypeDef,
     },
-    total=False,
 )
 
 _RequiredGetRightsizingRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetRightsizingRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -1680,40 +1863,83 @@
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetRightsizingRecommendationRequestRequestTypeDef(
     _RequiredGetRightsizingRecommendationRequestRequestTypeDef,
     _OptionalGetRightsizingRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceDetailsTypeDef = TypedDict(
     "InstanceDetailsTypeDef",
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
-    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommendationDetailDataTypeDef = TypedDict(
+    "RecommendationDetailDataTypeDef",
+    {
+        "AccountScope": AccountScopeType,
+        "LookbackPeriodInDays": LookbackPeriodInDaysType,
+        "SavingsPlansType": SupportedSavingsPlansTypeType,
+        "TermInYears": TermInYearsType,
+        "PaymentOption": PaymentOptionType,
+        "AccountId": str,
+        "CurrencyCode": str,
+        "InstanceFamily": str,
+        "Region": str,
+        "OfferingId": str,
+        "GenerationTimestamp": str,
+        "LatestUsageTimestamp": str,
+        "CurrentAverageHourlyOnDemandSpend": str,
+        "CurrentMaximumHourlyOnDemandSpend": str,
+        "CurrentMinimumHourlyOnDemandSpend": str,
+        "EstimatedAverageUtilization": str,
+        "EstimatedMonthlySavingsAmount": str,
+        "EstimatedOnDemandCost": str,
+        "EstimatedOnDemandCostWithCurrentCommitment": str,
+        "EstimatedROI": str,
+        "EstimatedSPCost": str,
+        "EstimatedSavingsAmount": str,
+        "EstimatedSavingsPercentage": str,
+        "ExistingHourlyCommitment": str,
+        "HourlyCommitmentToPurchase": str,
+        "UpfrontCost": str,
+        "CurrentAverageCoverage": str,
+        "EstimatedAverageCoverage": str,
+        "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
+    },
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
     },
-    total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
         "SavingsPlansDetails": SavingsPlansDetailsTypeDef,
         "AccountId": str,
@@ -1727,77 +1953,62 @@
         "EstimatedSavingsPercentage": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
+        "RecommendationDetailId": str,
     },
-    total=False,
 )
 
-_RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
+SavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "SavingsPlansUtilizationAggregatesTypeDef",
     {
         "Utilization": SavingsPlansUtilizationTypeDef,
-    },
-)
-_OptionalSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "_OptionalSavingsPlansUtilizationAggregatesTypeDef",
-    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
-class SavingsPlansUtilizationAggregatesTypeDef(
-    _RequiredSavingsPlansUtilizationAggregatesTypeDef,
-    _OptionalSavingsPlansUtilizationAggregatesTypeDef,
-):
-    pass
-
-_RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "_RequiredSavingsPlansUtilizationByTimeTypeDef",
+SavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "SavingsPlansUtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
-    },
-)
-_OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "_OptionalSavingsPlansUtilizationByTimeTypeDef",
-    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
-class SavingsPlansUtilizationByTimeTypeDef(
-    _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
-):
-    pass
-
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
-    total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -1807,71 +2018,55 @@
     "_OptionalCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCostCategoryTypeDef = TypedDict(
-    "_RequiredCostCategoryTypeDef",
+CostCategoryTypeDef = TypedDict(
+    "CostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
+        "EffectiveEnd": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": List[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCostCategoryTypeDef = TypedDict(
-    "_OptionalCostCategoryTypeDef",
-    {
-        "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
+        "Rules": List[CostCategoryRuleOutputTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
-    total=False,
 )
 
-class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
-    pass
-
 _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -1883,20 +2078,22 @@
         "DefaultValue": str,
         "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -1907,53 +2104,53 @@
         "EffectiveStart": str,
         "DefaultValue": str,
         "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": CoverageTypeDef,
     },
-    total=False,
 )
 
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "EC2ResourceUtilization": EC2ResourceUtilizationTypeDef,
     },
-    total=False,
 )
 
 _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -1970,39 +2167,39 @@
         "ServiceSpecification": ServiceSpecificationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetReservationPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetReservationPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
-    total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
-    total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
     "ReservationPurchaseRecommendationDetailTypeDef",
     {
         "AccountId": str,
         "InstanceDetails": InstanceDetailsTypeDef,
@@ -2020,23 +2217,31 @@
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedMonthlySavingsPercentage": str,
         "EstimatedMonthlyOnDemandCost": str,
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
-    total=False,
+)
+
+GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
+    {
+        "RecommendationDetailId": str,
+        "RecommendationDetailData": RecommendationDetailDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2047,188 +2252,181 @@
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
         "SavingsPlansPurchaseRecommendationSummary": (
             SavingsPlansPurchaseRecommendationSummaryTypeDef
         ),
     },
-    total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
+        "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
-    total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesTypeDef],
+        "Tags": List[TagValuesOutputTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
         "CurrencyCode": str,
     },
-    total=False,
 )
 
 TargetInstanceTypeDef = TypedDict(
     "TargetInstanceTypeDef",
     {
         "EstimatedMonthlyCost": str,
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
         "DefaultTargetInstance": bool,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ExpectedResourceUtilization": ResourceUtilizationTypeDef,
         "PlatformDifferences": List[PlatformDifferenceType],
     },
-    total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionTypeDef],
+        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionTypeDef],
+        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
-        "ServiceSpecification": ServiceSpecificationTypeDef,
+        "ServiceSpecification": ServiceSpecificationOutputTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
-    total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
     },
-    total=False,
 )
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
         "CurrentInstance": CurrentInstanceTypeDef,
         "RightsizingType": RightsizingTypeType,
         "ModifyRecommendationDetail": ModifyRecommendationDetailTypeDef,
         "TerminateRecommendationDetail": TerminateRecommendationDetailTypeDef,
         "FindingReasonCodes": List[FindingReasonCodeType],
     },
-    total=False,
 )
 
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
-        "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.0
-Summary: Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,110 +330,128 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
+    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
+    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
+    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalTypeDef,
+    DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
+    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
+    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
+    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
+    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
+    RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
+    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
+    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -442,35 +460,38 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
     CreateCostCategoryDefinitionRequestRequestTypeDef,
     UpdateCostCategoryDefinitionRequestRequestTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.0/setup.py` & `mypy-boto3-ce-1.28.10/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.28.0",
+    version="1.28.10",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

