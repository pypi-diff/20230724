# Comparing `tmp/pmotif_lib-1.0.1.tar.gz` & `tmp/pmotif_lib-1.0.2.tar.gz`

## Comparing `pmotif_lib-1.0.1.tar` & `pmotif_lib-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/requirements.txt
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/config.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/graphlet_occurence.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/graphlet_representation.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_motif_graph.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/randomization.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/result_transformer.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/__init__.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/graph_io.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/parsing.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/__init__.py
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_consolidation.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_processing.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_anchor_node_distance.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_degree.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_graph_module_participation.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric_result.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/.showcase_env
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/graphlet_detection.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/motif_detection.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/pgraphlet_detection.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/pmotif_detection.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/artifacts/karate_club.edgelist
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/LICENSE
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/__init__.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/graphlet_occurence.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/graphlet_representation.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_motif_graph.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/randomization.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/result_transformer.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/__init__.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/graph_io.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/parsing.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/__init__.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/metric_consolidation.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/metric_processing.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/p_anchor_node_distance.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/p_degree.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/p_graph_module_participation.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/p_metric.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pmotif_lib/p_metric/p_metric_result.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/showcase/graphlet_detection.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/showcase/motif_detection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/showcase/pgraphlet_detection.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/showcase/pmotif_detection.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/showcase/artifacts/karate_club.edgelist
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pmotif_lib-1.0.2/PKG-INFO
```

### Comparing `pmotif_lib-1.0.1/pmotif_lib/graphlet_occurence.py` & `pmotif_lib-1.0.2/pmotif_lib/graphlet_occurence.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/graphlet_representation.py` & `pmotif_lib-1.0.2/pmotif_lib/graphlet_representation.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_motif_graph.py` & `pmotif_lib-1.0.2/pmotif_lib/p_motif_graph.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/randomization.py` & `pmotif_lib-1.0.2/pmotif_lib/randomization.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/result_transformer.py` & `pmotif_lib-1.0.2/pmotif_lib/result_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from multiprocessing import Pool
 from pathlib import Path
 from typing import List, Callable
 import pandas as pd
 from tqdm import tqdm
 
 from pmotif_lib.p_motif_graph import PMotifGraph, PMotifGraphWithRandomization
-from pmotif_lib.config import WORKERS
 from pmotif_lib.p_metric.p_metric import RawMetric, PreComputation
 from pmotif_lib.p_metric.p_metric_result import PMetricResult
 
 
 ConsolidationMethod = Callable[[RawMetric, PreComputation], float]
 
 
@@ -111,26 +110,27 @@
         )
 
     @staticmethod
     def load_randomized_results(
         pmotif_graph: PMotifGraph,
         graphlet_size: int,
         supress_tqdm: bool = False,
+        workers: int = 1,
     ) -> List[ResultTransformer]:
         """Loads `graphlet_size`-graphlets and computed metrics which are present on disk."""
         pmotif_with_rand = PMotifGraphWithRandomization(
             pmotif_graph.edgelist_path, pmotif_graph.output_directory
         )
 
         input_args = [
             (swapped_graph, graphlet_size, supress_tqdm)
             for swapped_graph in pmotif_with_rand.swapped_graphs
         ]
 
-        with Pool(processes=WORKERS) as pool:
+        with Pool(processes=workers) as pool:
             pbar = tqdm(
                 input_args,
                 total=len(pmotif_with_rand.swapped_graphs),
                 desc="Loading Randomized Results",
             )
             return pool.starmap(
                 ResultTransformer._load_result,
```

### Comparing `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/graph_io.py` & `pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/graph_io.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/parsing.py` & `pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/parsing.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/wrapper.py` & `pmotif_lib-1.0.2/pmotif_lib/gtrieScanner/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # Therefore, we exclude those cases from py-linting:
 # pylint: disable=invalid-name, too-many-arguments
 import os
 from pathlib import Path
 from subprocess import Popen, PIPE
 import zipfile
 
-from pmotif_lib.config import GTRIESCANNER_EXECUTABLE
 from pmotif_lib.gtrieScanner.graph_io import read_edgelist
 
 
 def run_gtrieScanner(
     graph_edgelist: Path,
     graphlet_size: int,
     output_directory: Path,
-    gtrieScanner_executable: Path = GTRIESCANNER_EXECUTABLE,
+    gtrieScanner_executable: str,
     directed: bool = False,
     with_weights: bool = True,
 ):
     """
     Detects motifs for the given edge list and compresses the result
     """
     out_dir = output_directory / str(graphlet_size)
```

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_consolidation.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/metric_consolidation.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_processing.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/metric_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,35 @@
     Dict,
 )
 from multiprocessing import Pool
 from tqdm import tqdm
 import networkx as nx
 from pmotif_lib.graphlet_occurence import GraphletOccurrence
 from pmotif_lib.p_motif_graph import PMotifGraph
-from pmotif_lib.config import WORKERS
 from pmotif_lib.p_metric.p_metric import PMetric
 from pmotif_lib.p_metric.p_metric_result import PMetricResult
 
 
 def process_graphlet_occurrences(
     graph: nx.Graph,
     graphlet_occurrences: List[GraphletOccurrence],
     metrics: List[PMetric],
+    workers: int = 1,
 ) -> List[PMetricResult]:
     """Calculate motif positional metrics"""
 
     result: Dict[str, Dict] = {m.name: {} for m in metrics}
 
     # Pre-Compute for metrics
     metric: PMetric
     for metric in tqdm(metrics, desc="Pre-computing metrics", leave=False):
         result[metric.name]["pre_compute"] = metric.pre_computation(graph)
 
     # Calculate metrics
-    with Pool(processes=WORKERS) as pool:
+    with Pool(processes=workers) as pool:
         for metric in tqdm(metrics, desc="Calculating metrics", leave=False):
             result[metric.name]["graphlet_metrics"] = []
             args = [
                 (graph, g_oc.nodes, result[metric.name]["pre_compute"])
                 for g_oc in graphlet_occurrences
             ]
 
@@ -62,28 +62,29 @@
 
 
 def calculate_metrics(
     pmotif_graph: PMotifGraph,
     graphlet_size: int,
     metrics: List[PMetric],
     save_to_disk: bool = True,
+    workers: int = 1,
 ) -> List[PMetricResult]:
     """When pointed to a graph and a motif file, unzips the motif file, reads the graphs,
      and calculates given positional metrics.
      Can save results directly to disk.
     Returns a list of the results as PMetricResult objects."""
     graph = nx.readwrite.edgelist.read_edgelist(
         pmotif_graph.get_graph_path(), data=False, create_using=nx.Graph
     )
     graphlet_occurrences: List[GraphletOccurrence] = pmotif_graph.load_graphlet_pos_zip(
         graphlet_size
     )
 
     metric_result_lookup = process_graphlet_occurrences(
-        graph, graphlet_occurrences, metrics
+        graph, graphlet_occurrences, metrics, workers=workers,
     )
     if save_to_disk:
         metric_output = pmotif_graph.get_pmetric_directory(graphlet_size)
         makedirs(metric_output)
         for metric_result in metric_result_lookup:
             metric_result.save_to_disk(metric_output)
```

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_anchor_node_distance.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/p_anchor_node_distance.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_degree.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/p_degree.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_graph_module_participation.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/p_graph_module_participation.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/p_metric.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric_result.py` & `pmotif_lib-1.0.2/pmotif_lib/p_metric/p_metric_result.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/showcase/graphlet_detection.py` & `pmotif_lib-1.0.2/showcase/graphlet_detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 grouped by their isomorphic class (returns all graphlet occurrences)"""
 # Code in showcase intentionally duplicated, so examples can stand alone
 # pylint: disable=duplicate-code
 import shutil
 from pathlib import Path
 
 from pmotif_lib.p_motif_graph import PMotifGraph
-from pmotif_lib.config import DATASET_DIRECTORY, EXPERIMENT_OUT
 from pmotif_lib.gtrieScanner.wrapper import run_gtrieScanner
 
 
-DATASET = DATASET_DIRECTORY / "karate_club.edgelist"
+DATASET = Path("./artifacts") / "karate_club.edgelist"
 GRAPHLET_SIZE = 3
-OUTPUT = EXPERIMENT_OUT / "showcase_output"
+OUTPUT = Path("./artifacts") / "showcase_output"
+GTRIESCANNER_EXECUTABLE = "gtrieScanner"  # is in PATH
 
 
 def main(edgelist: Path, output: Path, graphlet_size: int):
     """Run a graphlet detection."""
     pmotif_graph = PMotifGraph(edgelist, output)
 
     run_gtrieScanner(
         graph_edgelist=pmotif_graph.get_graph_path(),
         graphlet_size=graphlet_size,
         output_directory=pmotif_graph.get_graphlet_directory(),
+        gtrieScanner_executable=GTRIESCANNER_EXECUTABLE,
     )
 
     graphlet_occurrences = pmotif_graph.load_graphlet_pos_zip(graphlet_size)
     print(graphlet_occurrences[0].graphlet_class, graphlet_occurrences[0].nodes)
 
 
 if __name__ == "__main__":
```

### Comparing `pmotif_lib-1.0.1/showcase/motif_detection.py` & `pmotif_lib-1.0.2/showcase/motif_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # Code in showcase intentionally duplicated, so examples can stand alone
 # pylint: disable=duplicate-code
 import shutil
 from pathlib import Path
 from statistics import mean, stdev
 
 from pmotif_lib.p_motif_graph import PMotifGraph, PMotifGraphWithRandomization
-from pmotif_lib.config import DATASET_DIRECTORY, EXPERIMENT_OUT
 from pmotif_lib.graphlet_representation import graphlet_class_to_name
 from pmotif_lib.gtrieScanner.wrapper import run_gtrieScanner
 
 
-DATASET = DATASET_DIRECTORY / "karate_club.edgelist"
+DATASET = Path("./artifacts") / "karate_club.edgelist"
 GRAPHLET_SIZE = 3
-OUTPUT = EXPERIMENT_OUT / "showcase_output"
+GTRIESCANNER_EXECUTABLE = "gtrieScanner"  # is in PATH
+OUTPUT = Path("./artifacts") / "showcase_output"
 NUMBER_OF_RANDOM_GRAPHS = 10
 
 
 def main(
     edgelist: Path, output: Path, graphlet_size: int, number_of_random_graphs: int
 ):
     """Run a motif detection."""
@@ -55,14 +55,15 @@
 
 def graphlet_detection(pgraph: PMotifGraph, graphlet_size: int):
     """Perform a graphlet detection and return the graphlet class frequencies."""
     run_gtrieScanner(
         graph_edgelist=pgraph.get_graph_path(),
         graphlet_size=graphlet_size,
         output_directory=pgraph.get_graphlet_directory(),
+        gtrieScanner_executable=GTRIESCANNER_EXECUTABLE,
     )
 
     graphlet_occurrences = pgraph.load_graphlet_pos_zip(graphlet_size)
     return graphlet_occurrences_to_class_frequencies(graphlet_occurrences)
 
 
 def graphlet_occurrences_to_class_frequencies(graphlet_occurrences):
```

### Comparing `pmotif_lib-1.0.1/showcase/pgraphlet_detection.py` & `pmotif_lib-1.0.2/showcase/pgraphlet_detection.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,37 +2,40 @@
 calculates each metric in `metrics` for each graphlet occurrence."""
 # Code in showcase intentionally duplicated, so examples can stand alone
 # pylint: disable=duplicate-code
 import shutil
 from pathlib import Path
 
 from pmotif_lib.p_motif_graph import PMotifGraph
-from pmotif_lib.config import DATASET_DIRECTORY, EXPERIMENT_OUT
 from pmotif_lib.gtrieScanner.wrapper import run_gtrieScanner
 from pmotif_lib.p_metric.p_degree import PDegree
 from pmotif_lib.p_metric.metric_processing import calculate_metrics
 
-DATASET = DATASET_DIRECTORY / "karate_club.edgelist"
+DATASET = Path("./artifacts") / "karate_club.edgelist"
 GRAPHLET_SIZE = 3
-OUTPUT = EXPERIMENT_OUT / "showcase_output"
+GTRIESCANNER_EXECUTABLE = "gtrieScanner"  # is in PATH
+OUTPUT = Path("./artifacts") / "showcase_output"
+
+WORKERS = 1
 
 
 def main(edgelist: Path, output: Path, graphlet_size: int):
     """Run a p-graphlet detection (based on the positional metric 'degree')."""
     pmotif_graph = PMotifGraph(edgelist, output)
 
     run_gtrieScanner(
         graph_edgelist=pmotif_graph.get_graph_path(),
         graphlet_size=graphlet_size,
         output_directory=pmotif_graph.get_graphlet_directory(),
+        gtrieScanner_executable=GTRIESCANNER_EXECUTABLE,
     )
 
     degree_metric = PDegree()
     metric_results = calculate_metrics(
-        pmotif_graph, graphlet_size, [degree_metric], True
+        pmotif_graph, graphlet_size, [degree_metric], True, workers=WORKERS,
     )
 
     graphlet_occurrences = pmotif_graph.load_graphlet_pos_zip(graphlet_size)
     print(graphlet_occurrences[0].graphlet_class, graphlet_occurrences[0].nodes)
     print(metric_results[0].graphlet_metrics[0])
```

### Comparing `pmotif_lib-1.0.1/showcase/pmotif_detection.py` & `pmotif_lib-1.0.2/showcase/pmotif_detection.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 import shutil
 from pathlib import Path
 from typing import List
 
 from scipy.stats import mannwhitneyu
 
 from pmotif_lib.p_motif_graph import PMotifGraph, PMotifGraphWithRandomization
-from pmotif_lib.config import DATASET_DIRECTORY, EXPERIMENT_OUT
 from pmotif_lib.graphlet_representation import graphlet_class_to_name
 from pmotif_lib.gtrieScanner.wrapper import run_gtrieScanner
 from pmotif_lib.p_metric.p_degree import PDegree
 from pmotif_lib.p_metric.p_metric import PMetric
 from pmotif_lib.p_metric.metric_processing import calculate_metrics
 
 
-DATASET = DATASET_DIRECTORY / "karate_club.edgelist"
+DATASET = Path("./artifacts") / "karate_club.edgelist"
+GTRIESCANNER_EXECUTABLE = "gtrieScanner"  # is in PATH
 GRAPHLET_SIZE = 3
+OUTPUT = Path("./artifacts") / "showcase_output"
 NUMBER_OF_RANDOM_GRAPHS = 10
-OUTPUT = EXPERIMENT_OUT / "showcase_output"
+
+WORKERS = 1
 
 
 def main(
     edgelist: Path, output: Path, graphlet_size: int, number_of_random_graphs: int
 ):
     """Run a p-motif detection (based on the positional metric 'degree') and basic analysis."""
     degree_metric = PDegree()
@@ -78,18 +80,19 @@
 ):
     """Perform a graphlet detection, calculate given metrics on detected graphlets, and
     return the metrics as a lookup from graphlet class and metric name to the metric values."""
     run_gtrieScanner(
         graph_edgelist=pgraph.get_graph_path(),
         graphlet_size=graphlet_size,
         output_directory=pgraph.get_graphlet_directory(),
+        gtrieScanner_executable=GTRIESCANNER_EXECUTABLE,
     )
 
     graphlet_occurrences = pgraph.load_graphlet_pos_zip(graphlet_size)
-    metric_results = calculate_metrics(pgraph, graphlet_size, metrics, True)
+    metric_results = calculate_metrics(pgraph, graphlet_size, metrics, True, workers=WORKERS)
 
     by_graphlet_class = {}
     for i, g_oc in enumerate(graphlet_occurrences):
         if g_oc.graphlet_class not in by_graphlet_class:
             by_graphlet_class[g_oc.graphlet_class] = {}
         for metric_result in metric_results:
             by_graphlet_class[g_oc.graphlet_class][
```

### Comparing `pmotif_lib-1.0.1/showcase/artifacts/karate_club.edgelist` & `pmotif_lib-1.0.2/showcase/artifacts/karate_club.edgelist`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/LICENSE` & `pmotif_lib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/README.md` & `pmotif_lib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.1/pyproject.toml` & `pmotif_lib-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pmotif_lib"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Tim Garrels", email="tim.garrels@protonmail.com" },
 ]
 description = "Perform motif detection, either with traditional frequency, or with positional metrics for each graphlet occurrence."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pmotif_lib-1.0.1/PKG-INFO` & `pmotif_lib-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmotif_lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Perform motif detection, either with traditional frequency, or with positional metrics for each graphlet occurrence.
 Project-URL: Homepage, https://github.com/timgarrels/pmotif_lib
 Project-URL: documentation, https://github.com/timgarrels/pmotif_lib/wiki
 Project-URL: Bug Tracker, https://github.com/timgarrels/pmotif_lib/issues
 Project-URL: Repository, https://github.com/timgarrels/pmotif_lib
 Author-email: Tim Garrels <tim.garrels@protonmail.com>
 License-File: LICENSE
```

