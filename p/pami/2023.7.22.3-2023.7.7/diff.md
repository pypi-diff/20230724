# Comparing `tmp/pami-2023.7.22.3.tar.gz` & `tmp/pami-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.7.22.3.tar", last modified: Mon Jul 24 05:50:17 2023, max compression
+gzip compressed data, was "pami-2023.7.7.tar", last modified: Tue Jul 18 12:23:34 2023, max compression
```

## Comparing `pami-2023.7.22.3.tar` & `pami-2023.7.7.tar`

### file list

```diff
@@ -1,12 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 05:50:17.274302 pami-2023.7.22.3/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 05:45:43.000000 pami-2023.7.22.3/LICENSE
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      459 2023-07-24 05:50:17.274206 pami-2023.7.22.3/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    38368 2023-07-24 05:45:44.000000 pami-2023.7.22.3/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 05:50:17.274047 pami-2023.7.22.3/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      459 2023-07-24 05:50:17.000000 pami-2023.7.22.3/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      165 2023-07-24 05:50:17.000000 pami-2023.7.22.3/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 05:50:17.000000 pami-2023.7.22.3/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      109 2023-07-24 05:50:17.000000 pami-2023.7.22.3/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 05:50:17.000000 pami-2023.7.22.3/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-24 05:50:17.274338 pami-2023.7.22.3/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      952 2023-07-24 05:50:12.000000 pami-2023.7.22.3/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.306139 pami-2023.7.7/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.7/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213420 pami-2023.7.7/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213780 pami-2023.7.7/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215229 pami-2023.7.7/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215381 pami-2023.7.7/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.216924 pami-2023.7.7/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.217089 pami-2023.7.7/PAMI/coveragePatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.218352 pami-2023.7.7/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.219319 pami-2023.7.7/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221044 pami-2023.7.7/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221516 pami-2023.7.7/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.223716 pami-2023.7.7/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.225281 pami-2023.7.7/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.227961 pami-2023.7.7/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231441 pami-2023.7.7/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231576 pami-2023.7.7/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231920 pami-2023.7.7/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.232234 pami-2023.7.7/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233791 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2280 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2257 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2509 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2124 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2075 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233937 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235273 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235589 pami-2023.7.7/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.237534 pami-2023.7.7/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.238433 pami-2023.7.7/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.240335 pami-2023.7.7/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.241160 pami-2023.7.7/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.242453 pami-2023.7.7/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243543 pami-2023.7.7/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243784 pami-2023.7.7/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.244809 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245067 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245890 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.246160 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247438 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247699 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.248928 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249301 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249802 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.250466 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251507 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251792 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.252874 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.254340 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255007 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255910 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256357 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256630 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257531 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257812 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261273 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261803 pami-2023.7.7/PAMI/highUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.264098 pami-2023.7.7/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265044 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16481 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265480 pami-2023.7.7/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.266895 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267687 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267930 pami-2023.7.7/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269128 pami-2023.7.7/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269369 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270382 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270633 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271619 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271849 pami-2023.7.7/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.273903 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.274936 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.275960 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.276849 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277438 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277755 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278324 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278541 pami-2023.7.7/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279293 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279512 pami-2023.7.7/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.281487 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.282417 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.283856 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19727 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.284826 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285069 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285761 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286394 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286673 pami-2023.7.7/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287396 pami-2023.7.7/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287636 pami-2023.7.7/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288407 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288643 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289267 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289510 pami-2023.7.7/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.290707 pami-2023.7.7/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291328 pami-2023.7.7/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291420 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.292688 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293628 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293913 pami-2023.7.7/PAMI/streams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294014 pami-2023.7.7/PAMI/streams/frequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294626 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31851 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7792 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295292 pami-2023.7.7/PAMI/streams/highUtility/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295424 pami-2023.7.7/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298349 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298597 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.299797 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300033 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300646 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300913 pami-2023.7.7/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.301700 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302005 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302627 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.303017 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.304367 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.305978 pami-2023.7.7/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34480 2023-07-07 08:24:43.000000 pami-2023.7.7/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.305715 pami-2023.7.7/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15099 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      102 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-18 12:23:34.306190 pami-2023.7.7/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1289 2023-07-18 12:22:32.000000 pami-2023.7.7/setup.py
```

### Comparing `pami-2023.7.22.3/LICENSE` & `pami-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.7.22.3/README.md` & `pami-2023.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: pami
+Version: 2023.7.7
+Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
+Home-page: https://github.com/udayRage/PAMI
+Author: Rage Uday Kiran
+Author-email: uday.rage@gmail.com
+License: GPLv3
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+Provides-Extra: spark
+License-File: LICENSE
+
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -19,21 +37,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -59,106 +77,106 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
 | STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
@@ -294,36 +312,20 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__   
      
      
+
+
```

### Comparing `pami-2023.7.22.3/setup.py` & `pami-2023.7.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='pami',
-    version='2023.07.22.3',
-    url='https://github.com/udayLab/PAMI',
+    name = 'pami',
+    version = '2023.07.07',
+    author = 'Rage Uday Kiran',
+    author_email = 'uday.rage@gmail.com',
+    description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
+    packages=setuptools.find_packages(),
+    url = 'https://github.com/udayRage/PAMI',
     license='GPLv3',
     install_requires=[            # All necessary packages utilized by our PAMI software
         'psutil',
         'pandas',
         'plotly',
         'matplotlib',
         'resource',
         'validators',
         'urllib3',
         'Pillow',
         'numpy',
     ],
-    extras_require={
-        'gpu':  ['cupy', 'pycuda'],
+    extras_require = {
+        'gpu':  ['cupy'],
         'spark': ['pyspark'],
     },
-    classifiers=[
-        'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    classifiers = [
+        'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.5',
+    python_requires = '>=3.5',
 )
```

