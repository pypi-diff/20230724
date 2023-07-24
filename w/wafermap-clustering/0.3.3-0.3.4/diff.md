# Comparing `tmp/wafermap-clustering-0.3.3.tar.gz` & `tmp/wafermap-clustering-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.3.tar", last modified: Wed Jul 19 12:20:42 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.4.tar", last modified: Mon Jul 24 08:17:26 2023, max compression
```

## Comparing `wafermap-clustering-0.3.3.tar` & `wafermap-clustering-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.086670 wafermap-clustering-0.3.3/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-19 12:20:42.083503 wafermap-clustering-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 12:20:42.088137 wafermap-clustering-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-07-19 12:20:18.000000 wafermap-clustering-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.021721 wafermap-clustering-0.3.3/tests/
--rw-rw-rw-   0        0        0     9509 2023-07-19 09:46:50.000000 wafermap-clustering-0.3.3/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.026884 wafermap-clustering-0.3.3/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.059389 wafermap-clustering-0.3.3/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.3/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.064011 wafermap-clustering-0.3.3/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.3/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.078885 wafermap-clustering-0.3.3/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.3/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.3/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.3/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5621 2023-07-19 09:43:06.000000 wafermap-clustering-0.3.3/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:20:42.054852 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-19 12:20:41.000000 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-19 12:20:41.000000 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 12:20:41.000000 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-19 12:20:41.000000 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-19 12:20:41.000000 wafermap-clustering-0.3.3/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.167187 wafermap-clustering-0.3.4/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-24 08:17:26.165084 wafermap-clustering-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 08:17:26.168229 wafermap-clustering-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-07-24 08:17:03.000000 wafermap-clustering-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.088218 wafermap-clustering-0.3.4/tests/
+-rw-rw-rw-   0        0        0     9605 2023-07-24 08:04:37.000000 wafermap-clustering-0.3.4/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.094459 wafermap-clustering-0.3.4/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.130603 wafermap-clustering-0.3.4/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.4/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.135368 wafermap-clustering-0.3.4/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.4/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.157861 wafermap-clustering-0.3.4/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     6705 2023-07-24 08:15:55.000000 wafermap-clustering-0.3.4/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.124300 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.3/LICENSE.txt` & `wafermap-clustering-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.3/PKG-INFO` & `wafermap-clustering-0.3.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.3/setup.py` & `wafermap-clustering-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.3"
+version = "0.3.4"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.3/tests/test_clustering.py` & `wafermap-clustering-0.3.4/tests/test_clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     1: 1670,
                 },
             }
         ]
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(self.path_klarf_single_wafer)
+        results = clustering.apply_from_klarf_path(self.path_klarf_single_wafer)
 
         summary = [
             {
                 "result_timestamp": res.result_timestamp,
                 "lot_id": res.lot_id,
                 "step_id": res.step_id,
                 "wafer_id": res.wafer_id,
@@ -133,15 +133,15 @@
                     7: 3,
                 },
             }
         ]
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(
+        results = clustering.apply_from_klarf_path(
             self.path_klarf_single_wafer_large_klarf,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.FULL.value,
         )
 
         summary = [
             {
@@ -164,15 +164,15 @@
         # GIVEN
         output_path = ASSETS_OUPUT_PATH
 
         expected_clusters = [615]
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(
+        results = clustering.apply_from_klarf_path(
             klarf_path=self.path_klarf_single_wafer,
             output_directory=output_path,
             klarf_format=KlarfFormat.FULL.value,
             clustering_mode=ClusteringMode.HDBSCAN.value,
         )
 
         # THEN
@@ -218,15 +218,15 @@
                     6: 3,
                 },
             },
         ]
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(self.path_klarf_multi_wafers)
+        results = clustering.apply_from_klarf_path(self.path_klarf_multi_wafers)
 
         summary = [
             {
                 "result_timestamp": res.result_timestamp,
                 "lot_id": res.lot_id,
                 "step_id": res.step_id,
                 "wafer_id": res.wafer_id,
@@ -249,15 +249,15 @@
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_02_dbscan.000",
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_06_dbscan.000",
             ]
         )
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(
+        results = clustering.apply_from_klarf_path(
             klarf_path=self.path_klarf_multi_wafers,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.BABY.value,
         )
         results = sorted(results, key=lambda x: x.output_filename)
 
         # THEN
@@ -273,15 +273,15 @@
         # GIVEN
         saved_klarf_path = (
             ASSETS_PATH / "saved" / "klarf_full" / "J237DTA_3236_dbscan.000"
         )
 
         # WHEN
         clustering = Clustering(config=self.config, logger=self.logger)
-        results = clustering.apply(
+        results = clustering.apply_from_klarf_path(
             klarf_path=self.path_klarf_multi_wafers,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.FULL.value,
         )
         results = sorted(results, key=lambda x: x.output_filename)
 
         # THEN
```

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.4/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.4/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.4/wafermap_clustering/wafermap_clustering.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # MODULES
 import time
 from pathlib import Path
-from typing import List
+from typing import List, Tuple
 from logging import Logger
 
 # NUMPY
 import numpy as np
 
 # SCIKIT_LEARN
 from sklearn.cluster import DBSCAN
 
 # HDBSCAN
 from hdbscan import HDBSCAN
 
 # KLARF_READER
-from klarf_reader.klarf import Klarf
+from klarf_reader.klarf import Klarf, KlarfContent
 from klarf_reader.utils import klarf_convert
 
 # MODELS
 from .models.clustered_defect import ClusteredDefect
 from .models.clustering_performance import ClusteringPerformance
 from .models.clustering_result import ClusteringResult
 
@@ -34,25 +34,24 @@
         self,
         config: Config,
         logger: Logger = None,
     ) -> None:
         self.config = config
         self.logger = logger
 
-    def apply(
+    def apply_from_content(
         self,
-        klarf_path: Path,
+        content: Tuple[KlarfContent, List[str]],
         output_directory: Path = None,
+        original_klarf_name: str = None,
+        original_klarf_extension: str = None,
         klarf_format=KlarfFormat.BABY.value,
         clustering_mode=ClusteringMode.DBSCAN.value,
-    ) -> List[ClusteringResult]:
-
-        klarf_content, raw_content = Klarf.load_from_file_with_raw_content(
-            filepath=klarf_path
-        )
+    ):
+        klarf_content, raw_content = content
 
         match clustering_mode:
             case ClusteringMode.DBSCAN.value:
                 clustering = DBSCAN(
                     eps=self.config.clustering.dbscan.eps,
                     min_samples=self.config.clustering.dbscan.min_samples,
                 )
@@ -127,17 +126,26 @@
                 clustering_result.performance.output_timestamp = round(
                     output_timestamp, 3
                 )
 
             results.append(clustering_result)
 
         if klarf_format == KlarfFormat.FULL.value and output_directory is not None:
+            if original_klarf_name is None:
+                raise ValueError(
+                    f"<original_klarf_name> cannot be None to create full klarf."
+                )
+            if original_klarf_extension is None:
+                raise ValueError(
+                    f"<original_klarf_extension> cannot be None to create full klarf."
+                )
+
             output_filename = (
                 output_directory
-                / f"{klarf_path.stem}_{clustering_mode}{klarf_path.suffix}"
+                / f"{original_klarf_name}_{clustering_mode}{original_klarf_extension}"
             )
 
             output_timestamp = klarf_lib.write_full_klarf(
                 raw_klarf=raw_content,
                 clustering_results=results,
                 attribute=self.config.attribute,
                 output_filename=output_filename,
@@ -155,7 +163,26 @@
                 clusters = clustering_result.clusters
 
                 self.logger.info(
                     msg=f"({repr(clustering_result)}) was sucessfully processed [{defects=}, {clusters=}] with ({repr(clustering_result.performance)}) "
                 )
 
         return results
+
+    def apply_from_klarf_path(
+        self,
+        klarf_path: Path,
+        output_directory: str = None,
+        klarf_format=KlarfFormat.BABY.value,
+        clustering_mode=ClusteringMode.DBSCAN.value,
+    ) -> List[ClusteringResult]:
+
+        content = Klarf.load_from_file_with_raw_content(filepath=klarf_path)
+
+        return self.apply_from_content(
+            content=content,
+            output_directory=output_directory,
+            original_klarf_name=klarf_path.stem,
+            original_klarf_extension=klarf_path.suffix,
+            klarf_format=klarf_format,
+            clustering_mode=clustering_mode,
+        )
```

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.4/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.3/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.4/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

