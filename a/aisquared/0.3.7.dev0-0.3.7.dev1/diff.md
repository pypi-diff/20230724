# Comparing `tmp/aisquared-0.3.7.dev0.tar.gz` & `tmp/aisquared-0.3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisquared-0.3.7.dev0.tar", last modified: Fri Jun 30 12:14:20 2023, max compression
+gzip compressed data, was "aisquared-0.3.7.dev1.tar", last modified: Mon Jul 24 12:28:53 2023, max compression
```

## Comparing `aisquared-0.3.7.dev0.tar` & `aisquared-0.3.7.dev1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.952237 aisquared-0.3.7.dev0/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19558 2023-06-30 12:14:20.951951 aisquared-0.3.7.dev0/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19234 2023-06-30 12:11:56.000000 aisquared-0.3.7.dev0/README.md
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.929644 aisquared-0.3.7.dev0/aisquared/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-05-31 16:52:11.000000 aisquared-0.3.7.dev0/aisquared/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.933395 aisquared-0.3.7.dev0/aisquared/base/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/base/BaseObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      811 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/base/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3474 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/base/css.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/base/endpoints.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/aisquared/base/harvesting.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/base/platform.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/aisquared/base/preprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/base/rendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/base/stages.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.934408 aisquared-0.3.7.dev0/aisquared/config/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/CustomObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8935 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/GraphConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    21366 2023-05-31 16:41:03.000000 aisquared-0.3.7.dev0/aisquared/config/ModelConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.935751 aisquared-0.3.7.dev0/aisquared/config/analytic/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3293 2023-06-30 12:12:29.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/LocalAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/LocalModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5569 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/ReverseMLWorkflow.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.937279 aisquared-0.3.7.dev0/aisquared/config/feedback/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/BinaryFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/ModelFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/MulticlassFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/QualitativeFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/RegressionFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/SimpleFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.938549 aisquared-0.3.7.dev0/aisquared/config/harvesting/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/ImageHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/InputHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/QueryParameterHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/TextHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.939660 aisquared-0.3.7.dev0/aisquared/config/postprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/BinaryClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/MulticlassClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/ObjectDetection.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/Regression.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.939885 aisquared-0.3.7.dev0/aisquared/config/preprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.940657 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.941461 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.942128 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.945790 aisquared-0.3.7.dev0/aisquared/config/rendering/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5083 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/BarChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ContainerRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardReplacementRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DocumentRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5053 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DoughnutChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/FilterRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/HTMLTagRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ImageRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5036 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/LineChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ObjectRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5068 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/PieChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/SOSRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/TableRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5031 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/WordRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      754 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.946023 aisquared-0.3.7.dev0/aisquared/logging/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/logging/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.948222 aisquared-0.3.7.dev0/aisquared/platform/
--rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/AISquaredAPIException.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/AISquaredPlatformClient.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/NoResultsFoundError.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/platform/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/additional_utils.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/crudl.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/metrics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/sharing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/user_group.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.948843 aisquared-0.3.7.dev0/aisquared/serving/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/serving/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.7.dev0/aisquared/serving/deploy_model.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/serving/get_remote_prediction.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.949368 aisquared-0.3.7.dev0/aisquared/utils/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/utils/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/utils/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.930961 aisquared-0.3.7.dev0/aisquared.egg-info/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19558 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/SOURCES.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/dependency_links.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)      108 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/requires.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/top_level.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-06-30 12:14:20.952297 aisquared-0.3.7.dev0/setup.cfg
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/setup.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.951637 aisquared-0.3.7.dev0/tests/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_air.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1070 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_analytics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_base.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/tests/test_custom.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_harvesters.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_postprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_preprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    22069 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_renderers.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_simple.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.350650 aisquared-0.3.7.dev1/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19604 2023-07-24 12:28:53.350332 aisquared-0.3.7.dev1/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19280 2023-07-24 12:28:24.000000 aisquared-0.3.7.dev1/README.md
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.326949 aisquared-0.3.7.dev1/aisquared/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-07-24 12:13:08.000000 aisquared-0.3.7.dev1/aisquared/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.330015 aisquared-0.3.7.dev1/aisquared/base/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/base/BaseObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      811 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/base/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3474 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/base/css.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/base/endpoints.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev1/aisquared/base/harvesting.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/base/platform.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev1/aisquared/base/preprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/base/rendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/base/stages.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.331102 aisquared-0.3.7.dev1/aisquared/config/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/CustomObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8935 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/GraphConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    21366 2023-05-31 16:41:03.000000 aisquared-0.3.7.dev1/aisquared/config/ModelConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.332583 aisquared-0.3.7.dev1/aisquared/config/analytic/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3293 2023-06-30 12:12:29.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/DeployedAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/DeployedModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/LocalAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/LocalModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5569 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/ReverseMLWorkflow.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.7.dev1/aisquared/config/analytic/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.334195 aisquared-0.3.7.dev1/aisquared/config/feedback/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/BinaryFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/ModelFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/MulticlassFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/QualitativeFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/RegressionFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/SimpleFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/feedback/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.335302 aisquared-0.3.7.dev1/aisquared/config/harvesting/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/harvesting/ImageHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/config/harvesting/InputHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/harvesting/QueryParameterHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/config/harvesting/TextHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/harvesting/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.336601 aisquared-0.3.7.dev1/aisquared/config/postprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/postprocessing/BinaryClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/postprocessing/MulticlassClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/postprocessing/ObjectDetection.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/postprocessing/Regression.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/postprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.336850 aisquared-0.3.7.dev1/aisquared/config/preprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.337582 aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-07-24 12:08:58.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/ImagePreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.338452 aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-07-24 12:09:28.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.339682 aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-07-24 12:09:36.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/TextPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.343580 aisquared-0.3.7.dev1/aisquared/config/rendering/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5083 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/BarChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/ContainerRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/DashboardRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/DashboardReplacementRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/DocumentRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5053 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/DoughnutChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/FilterRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/HTMLTagRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/ImageRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5036 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/LineChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/ObjectRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5068 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/PieChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/SOSRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/TableRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5031 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/WordRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      754 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/aisquared/config/rendering/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.343816 aisquared-0.3.7.dev1/aisquared/logging/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/logging/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.346321 aisquared-0.3.7.dev1/aisquared/platform/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/AISquaredAPIException.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/AISquaredPlatformClient.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/NoResultsFoundError.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/platform/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/additional_utils.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/crudl.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/metrics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/sharing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/platform/user_group.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.346978 aisquared-0.3.7.dev1/aisquared/serving/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/serving/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.7.dev1/aisquared/serving/deploy_model.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/serving/get_remote_prediction.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.347558 aisquared-0.3.7.dev1/aisquared/utils/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/aisquared/utils/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/aisquared/utils/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.328041 aisquared-0.3.7.dev1/aisquared.egg-info/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19604 2023-07-24 12:28:53.000000 aisquared-0.3.7.dev1/aisquared.egg-info/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-07-24 12:28:53.000000 aisquared-0.3.7.dev1/aisquared.egg-info/SOURCES.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-07-24 12:28:53.000000 aisquared-0.3.7.dev1/aisquared.egg-info/dependency_links.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      101 2023-07-24 12:28:53.000000 aisquared-0.3.7.dev1/aisquared.egg-info/requires.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-07-24 12:28:53.000000 aisquared-0.3.7.dev1/aisquared.egg-info/top_level.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-07-24 12:28:53.350724 aisquared-0.3.7.dev1/setup.cfg
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev1/setup.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-07-24 12:28:53.349962 aisquared-0.3.7.dev1/tests/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/tests/test_air.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1070 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/tests/test_analytics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/tests/test_base.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev1/tests/test_custom.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/tests/test_feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/tests/test_harvesters.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/tests/test_postprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-07-24 12:12:58.000000 aisquared-0.3.7.dev1/tests/test_preprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    22069 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev1/tests/test_renderers.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev1/tests/test_simple.py
```

### Comparing `aisquared-0.3.7.dev0/PKG-INFO` & `aisquared-0.3.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.7.dev0
+Version: 0.3.7.dev1
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -334,7 +334,8 @@
 - Restricted TensorFlow version to below `2.12.0` to prevent import issues
 - Added `position` parameter to `WordRendering` class
 - Changed default CSS styling for rendering classes
 - Changed name of all `processor` classes to `processer`
 
 ## Version 0.3.7
 - Changed schema of the `DeployedAnalytic` class to include API key management
+- Changed JSON schema of Preprocesser classes
```

### Comparing `aisquared-0.3.7.dev0/README.md` & `aisquared-0.3.7.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -323,7 +323,8 @@
 - Restricted TensorFlow version to below `2.12.0` to prevent import issues
 - Added `position` parameter to `WordRendering` class
 - Changed default CSS styling for rendering classes
 - Changed name of all `processor` classes to `processer`
 
 ## Version 0.3.7
 - Changed schema of the `DeployedAnalytic` class to include API key management
+- Changed JSON schema of Preprocesser classes
```

### Comparing `aisquared-0.3.7.dev0/aisquared/base/BaseObject.py` & `aisquared-0.3.7.dev1/aisquared/base/BaseObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/base/__init__.py` & `aisquared-0.3.7.dev1/aisquared/base/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/base/css.py` & `aisquared-0.3.7.dev1/aisquared/base/css.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/base/endpoints.py` & `aisquared-0.3.7.dev1/aisquared/base/endpoints.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/base/rendering.py` & `aisquared-0.3.7.dev1/aisquared/base/rendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/CustomObject.py` & `aisquared-0.3.7.dev1/aisquared/config/CustomObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/GraphConfiguration.py` & `aisquared-0.3.7.dev1/aisquared/config/GraphConfiguration.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/ModelConfiguration.py` & `aisquared-0.3.7.dev1/aisquared/config/ModelConfiguration.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedAnalytic.py` & `aisquared-0.3.7.dev1/aisquared/config/analytic/DeployedAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedModel.py` & `aisquared-0.3.7.dev1/aisquared/config/analytic/DeployedModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/analytic/LocalAnalytic.py` & `aisquared-0.3.7.dev1/aisquared/config/analytic/LocalAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/analytic/LocalModel.py` & `aisquared-0.3.7.dev1/aisquared/config/analytic/LocalModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/analytic/ReverseMLWorkflow.py` & `aisquared-0.3.7.dev1/aisquared/config/analytic/ReverseMLWorkflow.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/BinaryFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/BinaryFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/ModelFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/ModelFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/MulticlassFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/MulticlassFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/QualitativeFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/QualitativeFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/RegressionFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/RegressionFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/feedback/SimpleFeedback.py` & `aisquared-0.3.7.dev1/aisquared/config/feedback/SimpleFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/harvesting/ImageHarvester.py` & `aisquared-0.3.7.dev1/aisquared/config/harvesting/ImageHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/harvesting/InputHarvester.py` & `aisquared-0.3.7.dev1/aisquared/config/harvesting/InputHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/harvesting/QueryParameterHarvester.py` & `aisquared-0.3.7.dev1/aisquared/config/harvesting/QueryParameterHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/harvesting/TextHarvester.py` & `aisquared-0.3.7.dev1/aisquared/config/harvesting/TextHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/postprocessing/BinaryClassification.py` & `aisquared-0.3.7.dev1/aisquared/config/postprocessing/BinaryClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/postprocessing/MulticlassClassification.py` & `aisquared-0.3.7.dev1/aisquared/config/postprocessing/MulticlassClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/postprocessing/ObjectDetection.py` & `aisquared-0.3.7.dev1/aisquared/config/postprocessing/ObjectDetection.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/postprocessing/Regression.py` & `aisquared-0.3.7.dev1/aisquared/config/postprocessing/Regression.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/ImagePreprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
             self.steps = self.steps + [step]
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'ImagePreprocesser',
+            'className': 'ImagePreprocessor',
             'steps': self.step_dict
         }
```

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/Steps.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/image/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/Steps.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/tabular/TabularPreprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,12 +55,12 @@
             self.steps = self.steps + [step]
 
     def to_dict(self):
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'TabularPreprocesser',
+            'className': 'TabularPreprocessor',
             'steps': [
                 step.to_dict() for step in self.steps
             ]
         }
```

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/Steps.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py` & `aisquared-0.3.7.dev1/aisquared/config/preprocessing/text/TextPreprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
             self.steps = self.steps + [step]
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'TextPreprocesser',
+            'className': 'TextPreprocessor',
             'steps': self.step_dict
         }
```

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/BarChartRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/BarChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/ContainerRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/ContainerRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/DashboardRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardReplacementRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/DashboardReplacementRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/DocumentRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/DocumentRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/DoughnutChartRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/DoughnutChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/FilterRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/FilterRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/HTMLTagRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/HTMLTagRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/ImageRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/ImageRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/LineChartRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/LineChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/ObjectRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/ObjectRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/PieChartRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/PieChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/SOSRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/SOSRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/TableRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/TableRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/WordRendering.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/WordRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/__init__.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/config/rendering/utils.py` & `aisquared-0.3.7.dev1/aisquared/config/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/AISquaredPlatformClient.py` & `aisquared-0.3.7.dev1/aisquared/platform/AISquaredPlatformClient.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/additional_utils.py` & `aisquared-0.3.7.dev1/aisquared/platform/additional_utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/crudl.py` & `aisquared-0.3.7.dev1/aisquared/platform/crudl.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/feedback.py` & `aisquared-0.3.7.dev1/aisquared/platform/feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/metrics.py` & `aisquared-0.3.7.dev1/aisquared/platform/metrics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/sharing.py` & `aisquared-0.3.7.dev1/aisquared/platform/sharing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/platform/user_group.py` & `aisquared-0.3.7.dev1/aisquared/platform/user_group.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/serving/__init__.py` & `aisquared-0.3.7.dev1/aisquared/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/serving/deploy_model.py` & `aisquared-0.3.7.dev1/aisquared/serving/deploy_model.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/serving/get_remote_prediction.py` & `aisquared-0.3.7.dev1/aisquared/serving/get_remote_prediction.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared/utils/utils.py` & `aisquared-0.3.7.dev1/aisquared/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/aisquared.egg-info/PKG-INFO` & `aisquared-0.3.7.dev1/aisquared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.7.dev0
+Version: 0.3.7.dev1
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -334,7 +334,8 @@
 - Restricted TensorFlow version to below `2.12.0` to prevent import issues
 - Added `position` parameter to `WordRendering` class
 - Changed default CSS styling for rendering classes
 - Changed name of all `processor` classes to `processer`
 
 ## Version 0.3.7
 - Changed schema of the `DeployedAnalytic` class to include API key management
+- Changed JSON schema of Preprocesser classes
```

### Comparing `aisquared-0.3.7.dev0/aisquared.egg-info/SOURCES.txt` & `aisquared-0.3.7.dev1/aisquared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/setup.py` & `aisquared-0.3.7.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_air.py` & `aisquared-0.3.7.dev1/tests/test_air.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_analytics.py` & `aisquared-0.3.7.dev1/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_base.py` & `aisquared-0.3.7.dev1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_feedback.py` & `aisquared-0.3.7.dev1/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_harvesters.py` & `aisquared-0.3.7.dev1/tests/test_harvesters.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_postprocessors.py` & `aisquared-0.3.7.dev1/tests/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_preprocessors.py` & `aisquared-0.3.7.dev1/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.7.dev0/tests/test_renderers.py` & `aisquared-0.3.7.dev1/tests/test_renderers.py`

 * *Files identical despite different names*

