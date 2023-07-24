# Comparing `tmp/regulAS-2023.7.tar.gz` & `tmp/regulAS-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/regulAS-2023.7.tar", last modified: Mon Jul 17 07:23:39 2023, max compression
+gzip compressed data, was "dist/regulAS-2023.7.1.tar", last modified: Mon Jul 24 20:44:31 2023, max compression
```

## Comparing `regulAS-2023.7.tar` & `regulAS-2023.7.1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1073 2021-10-29 13:25:15.000000 regulAS-2023.7/LICENSE
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      544 2023-07-17 07:23:39.292879 regulAS-2023.7/PKG-INFO
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     9437 2023-07-17 07:16:15.000000 regulAS-2023.7/README.md
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.289545 regulAS-2023.7/regulAS/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      111 2023-07-16 22:00:41.000000 regulAS-2023.7/regulAS/__init__.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     4591 2021-11-04 21:58:43.000000 regulAS-2023.7/regulAS/app.py
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/regulAS/conf/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      187 2021-10-29 13:25:15.000000 regulAS-2023.7/regulAS/conf/default.yaml
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/regulAS/core/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)       29 2021-10-29 13:25:15.000000 regulAS-2023.7/regulAS/core/__init__.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    18948 2023-06-16 11:32:54.000000 regulAS-2023.7/regulAS/core/regulas.py
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/regulAS/persistence/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      338 2021-10-29 13:25:15.000000 regulAS-2023.7/regulAS/persistence/__init__.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     5310 2023-06-05 13:53:06.000000 regulAS-2023.7/regulAS/persistence/dao.py
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/regulAS/reports/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      330 2021-10-29 13:25:15.000000 regulAS-2023.7/regulAS/reports/__init__.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      380 2021-10-29 13:25:15.000000 regulAS-2023.7/regulAS/reports/base.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1189 2021-11-03 14:06:28.000000 regulAS-2023.7/regulAS/reports/export_textual.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    15425 2023-06-18 13:56:10.000000 regulAS-2023.7/regulAS/reports/export_visual.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    12125 2021-11-08 20:58:59.000000 regulAS-2023.7/regulAS/reports/export_visual_vis.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    10305 2023-06-18 13:52:48.000000 regulAS-2023.7/regulAS/reports/performance.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     8470 2023-06-18 13:59:47.000000 regulAS-2023.7/regulAS/reports/ranking.py
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.292879 regulAS-2023.7/regulAS/utils/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      174 2021-10-29 15:00:04.000000 regulAS-2023.7/regulAS/utils/__init__.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1209 2021-10-29 18:19:58.000000 regulAS-2023.7/regulAS/utils/base.py
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    18577 2023-06-24 15:57:45.000000 regulAS-2023.7/regulAS/utils/loader.py
-drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-17 07:23:39.289545 regulAS-2023.7/regulAS.egg-info/
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      544 2023-07-17 07:23:39.000000 regulAS-2023.7/regulAS.egg-info/PKG-INFO
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      635 2023-07-17 07:23:39.000000 regulAS-2023.7/regulAS.egg-info/SOURCES.txt
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)        1 2023-07-17 07:23:39.000000 regulAS-2023.7/regulAS.egg-info/dependency_links.txt
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      255 2023-07-17 07:23:39.000000 regulAS-2023.7/regulAS.egg-info/requires.txt
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)        8 2023-07-17 07:23:39.000000 regulAS-2023.7/regulAS.egg-info/top_level.txt
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)       38 2023-07-17 07:23:39.292879 regulAS-2023.7/setup.cfg
--rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1281 2023-07-17 07:22:16.000000 regulAS-2023.7/setup.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.717046 regulAS-2023.7.1/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1073 2021-10-29 13:25:15.000000 regulAS-2023.7.1/LICENSE
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     9988 2023-07-24 20:44:31.717046 regulAS-2023.7.1/PKG-INFO
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     9619 2023-07-24 20:44:23.000000 regulAS-2023.7.1/README.md
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.710379 regulAS-2023.7.1/regulAS/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      113 2023-07-24 20:43:18.000000 regulAS-2023.7.1/regulAS/__init__.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     4591 2021-11-04 21:58:43.000000 regulAS-2023.7.1/regulAS/app.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.713712 regulAS-2023.7.1/regulAS/conf/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      187 2021-10-29 13:25:15.000000 regulAS-2023.7.1/regulAS/conf/default.yaml
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.713712 regulAS-2023.7.1/regulAS/core/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)       29 2021-10-29 13:25:15.000000 regulAS-2023.7.1/regulAS/core/__init__.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    18948 2023-06-16 11:32:54.000000 regulAS-2023.7.1/regulAS/core/regulas.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.713712 regulAS-2023.7.1/regulAS/persistence/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      338 2021-10-29 13:25:15.000000 regulAS-2023.7.1/regulAS/persistence/__init__.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     5310 2023-06-05 13:53:06.000000 regulAS-2023.7.1/regulAS/persistence/dao.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.713712 regulAS-2023.7.1/regulAS/reports/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      330 2021-10-29 13:25:15.000000 regulAS-2023.7.1/regulAS/reports/__init__.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      380 2021-10-29 13:25:15.000000 regulAS-2023.7.1/regulAS/reports/base.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1189 2021-11-03 14:06:28.000000 regulAS-2023.7.1/regulAS/reports/export_textual.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    15425 2023-06-18 13:56:10.000000 regulAS-2023.7.1/regulAS/reports/export_visual.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    10305 2023-06-18 13:52:48.000000 regulAS-2023.7.1/regulAS/reports/performance.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     8470 2023-06-18 13:59:47.000000 regulAS-2023.7.1/regulAS/reports/ranking.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.717046 regulAS-2023.7.1/regulAS/utils/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      174 2021-10-29 15:00:04.000000 regulAS-2023.7.1/regulAS/utils/__init__.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1209 2021-10-29 18:19:58.000000 regulAS-2023.7.1/regulAS/utils/base.py
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)    17638 2023-07-23 21:41:41.000000 regulAS-2023.7.1/regulAS/utils/loader.py
+drwxr-xr-x   0 slipnitskaya  (1000) slipnitskaya  (1000)        0 2023-07-24 20:44:31.713712 regulAS-2023.7.1/regulAS.egg-info/
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     9988 2023-07-24 20:44:31.000000 regulAS-2023.7.1/regulAS.egg-info/PKG-INFO
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      598 2023-07-24 20:44:31.000000 regulAS-2023.7.1/regulAS.egg-info/SOURCES.txt
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)        1 2023-07-24 20:44:31.000000 regulAS-2023.7.1/regulAS.egg-info/dependency_links.txt
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)      255 2023-07-24 20:44:31.000000 regulAS-2023.7.1/regulAS.egg-info/requires.txt
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)        8 2023-07-24 20:44:31.000000 regulAS-2023.7.1/regulAS.egg-info/top_level.txt
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)       38 2023-07-24 20:44:31.717046 regulAS-2023.7.1/setup.cfg
+-rw-r--r--   0 slipnitskaya  (1000) slipnitskaya  (1000)     1222 2023-07-24 17:45:58.000000 regulAS-2023.7.1/setup.py
```

### Comparing `regulAS-2023.7/LICENSE` & `regulAS-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/README.md` & `regulAS-2023.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # regulAS
-## Machine learning pipeline for identification of alternative splicing regulators in large-scale RNA-seq data
-[![DOI](https://zenodo.org/badge/374424916.svg)](https://zenodo.org/badge/latestdoi/374424916)
+[![python](https://img.shields.io/badge/Python_3.7+-blue?logo=python&logoColor=white)](https://www.python.org/)
+[![sqlite](https://img.shields.io/badge/SQLite-%2307405e.svg?logo=sqlite&logoColor=white)](https://sqlite.org/)
+[![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/slipnitskaya/regulAS/blob/master/LICENSE)
+
+## A Bioinformatics Tool for the Integrative Analysis of Alternative Splicing Regulome using RNA-Seq data across cancer and tissue types
 
 ## Overview
 
 **regulAS** is a computational software for analysis of regulatory mechanisms of alternative splicing enabling to 
 dissect complex relationships between alternative splicing events and thousands of its prospective regulatory RBPs using large-scale RNA-seq data derived 
 from The Cancer Genome Atlas ([TCGA](https://www.cancer.gov/tcga)) and The Genotype-Tissue Expression ([GTEx](http://www.gtexportal.org/)) projects.
 
 
 **regulAS** is a powerful machine learning experiment management tool written in Python that combines
 flexible configuration system based on YAML and shell, fast and reliable data storage
 driven by SQLite relational database engine and an extension-friendly API compatible
 with `scikit-learn`.
 
 **regulAS** is designed to provide users with a "Low-Code" experiment management solution that is 
-dedicated for researchers of alternative splicing regulatory mechanisms to simplify typical data mining and machine learning, allowing them to alleviate the number of the prospective regulators of a splicing event of interest for the further in-depth bioinformatics and experimental analysis.
-
-
+dedicated for researchers of alternative splicing regulatory mechanisms to simplify computational workflow, 
+allowing them to alleviate the number of the prospective regulatory candidates of splicing changes for further 
+in-depth bioinformatics and experimental analysis.
  
 
 ## Structure
 
 **regulAS** is supplied with a set of pre-defined modules that introduce support for data
 acquisition, fitting of machine learning models, persistence and export of results.
 
 ### Workflow
 
 The **regulAS** package encapsulates ETL-, ML- and report generation workflows.
 ETL-workflow includes data Extraction, Transformation and Loading operations,
 thus preparing the input for the next step, namely Machine Learning (ML) part.
-The ML-workflow incorporates typical modeling-related tasks such as performance evaluation,
-hyper-parameters tuning and feature ranking for ....
-The ML-workflow output as well as the experimental setup serves as a source for report
-generators that can be run afterwards in order to produce summary of an experiment.
+The ML-workflow incorporates predictive modeling, hyper-parameter optimization, 
+performance evaluation and feature ranking tasks for identifying candidate 
+regulators of alternative splicing events across tumors and tissue types.
+The ML-workflow outputs can subsequently be utilized for generating summary reports in
+tabular and visual forms to support interpretation of the findings and knowledge sharing.
 
-![regulAS workflow](images/regulAS_workflow.png "regulAS workflow")
+![regulAS workflow](https://raw.githubusercontent.com/slipnitskaya/regulAS/master/images/regulAS_workflow.png "regulAS workflow")
 
 #### Data loading
 
 After the transformation step, **regulAS** loads the data into a [`pandas.DataFrame`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html),
 which is a default container to store intermediate results.
 Given an additional argument denoting the target for supervised model training,
 data loader splits the `DataFrame` into samples and targets that are used by the ML-part.
@@ -214,15 +218,15 @@
  * `Transformation` &ndash; contains details on ML-models and transformations
  * `HyperParameter` &ndash; contains hyper-parameters of models
  * `Prediction` &ndash; contains true and predicted values for target
  * `FeatureRanking` &ndash; contains feature importance scores
  * `TransformationSequence` &ndash; contains details on the use of models and transformations
  * `HyperParameterValue` &ndash; contains details on the specific values of hyper-parameters
 
-![regulAS database](images/regulAS_database.png "regulAS database")
+![regulAS database](https://raw.githubusercontent.com/slipnitskaya/regulAS/master/images/regulAS_database.png "regulAS database")
 
 ## Usage
 
 In order to use **regulAS** for experimental management, user should define a project directory
 containing YAML configuration files and data if necessary.
 The experiment then can be run from the command line.
 
@@ -230,17 +234,13 @@
 # install regulAS package from PyPi
 pip install regulAS
 # navigate to the user's project folder
 cd /path/to/the/project
 # run the experimental setup on different dataset files
 python -m regulAS.app --multirun \
 experiment=experiments/experiment_tasks \
-+dataset.path_to_file=data/data_gtex.pkl,data/data_tcga.pkl
++dataset.path_to_file=data/data_cNormal.pkl,data/data_cTumor.pkl
 ```
 
 After **regulAS** finishes all the tasks, an SQLite database file `regulAS.db` will be stored
 in the project directory as well as the reports if any was submitted to generate.
 
-## How to cite regulAS?
-When using **regulAS** in academic work, authors are encouraged to reference this work via Zenodo 
-([https://doi.org/10.5281/zenodo.8152782]). An example acknowledgment statement follows: The analysis used for the results 
-described in this manuscript were obtained using the regulAS tool.
```

### Comparing `regulAS-2023.7/regulAS/app.py` & `regulAS-2023.7.1/regulAS/app.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/core/regulas.py` & `regulAS-2023.7.1/regulAS/core/regulas.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/persistence/dao.py` & `regulAS-2023.7.1/regulAS/persistence/dao.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/reports/export_textual.py` & `regulAS-2023.7.1/regulAS/reports/export_textual.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/reports/export_visual.py` & `regulAS-2023.7.1/regulAS/reports/export_visual.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/reports/performance.py` & `regulAS-2023.7.1/regulAS/reports/performance.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/reports/ranking.py` & `regulAS-2023.7.1/regulAS/reports/ranking.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/utils/base.py` & `regulAS-2023.7.1/regulAS/utils/base.py`

 * *Files identical despite different names*

### Comparing `regulAS-2023.7/regulAS/utils/loader.py` & `regulAS-2023.7.1/regulAS/utils/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 from enum import auto, Enum
 from typing import List, Tuple, Optional
 
 from regulAS.utils import Loader
 
 
+FILENAME_CANDIDATE_GENE_IDS: str = 'gene_ids.txt'
+FILENAME_TARGET_JUNCTIONS: str = 'exon_junctions_data.csv'
+
+
 class ArgTypeMixin(Enum):
 
     @classmethod
     def argtype(cls, s: str) -> Enum:
         try:
             return cls[s]
         except KeyError:
@@ -156,39 +160,43 @@
                  cutoff_reads: int = 5,
                  ratio_nan_to_drop: float = 1.0,
                  log_transform: bool = False,
                  sample_size_per_tissue_min: int = 50,
                  pair_tissues: bool = True,
                  include_adjacent_tissues: bool = False,
                  objective: Optional[str] = None,
-                 meta: Optional[str] = None):
-
+                 meta: Optional[str] = None,
+                 filename_candidate_gene_ids: str = FILENAME_CANDIDATE_GENE_IDS,
+                 filename_target_junctions: Optional[str] = None
+                 ):
         self.gene_symbol = gene_symbol
         self.dir_to_data = os.path.join(hydra.utils.to_absolute_path(hydra.utils.get_original_cwd()), dir_to_data)
         self.out_dir = os.path.join(hydra.utils.to_absolute_path(hydra.utils.get_original_cwd()), out_dir)
         self.condition = Condition[condition]
         self.cutoff_reads = cutoff_reads
         self.ratio_nan_to_drop = ratio_nan_to_drop
         self.log_transform = log_transform
         self.sample_size_per_tissue_min = sample_size_per_tissue_min
         self.pair_tissues = pair_tissues
         self.include_adjacent_tissues = include_adjacent_tissues
+        self.filename_candidate_gene_ids = filename_candidate_gene_ids
+        self.filename_target_junctions = filename_target_junctions
 
         super(RawLoader, self).__init__(
             name=name,
             path_to_file='',
             objective=objective,
             meta=meta
         )
 
     def _init_data(self) -> pd.DataFrame:
         url_to_rnaseq = 'https://toil-xena-hub.s3.us-east-1.amazonaws.com/download/TcgaTargetGtex_rsem_gene_tpm.gz'
         url_to_metadata = 'https://toil-xena-hub.s3.us-east-1.amazonaws.com/download/TcgaTargetGTEX_phenotype.txt.gz'
         dir_to_junctions = os.path.join(self.dir_to_data, 'junctions')
-        path_to_gene_ids = os.path.join(self.dir_to_data, 'gene_ids.txt')
+        path_to_gene_ids = os.path.join(self.dir_to_data, self.filename_candidate_gene_ids)
 
         self.log(logging.INFO, f'Loading RNA-Seq and Junction data...')
         # load gene expression
         rnaseq = self.load_from_xena(url_to_rnaseq, self.dir_to_data)
 
         # load metadata
         metadata = self.load_from_xena(url_to_metadata, self.dir_to_data)
@@ -209,64 +217,44 @@
 
         # rename columns
         cols = {'_primary_site': 'tissue', '_study': 'cohort'}
         metadata = metadata[list(cols.keys())].rename(columns=cols)
 
         # load junctions
         try:
-            path_to_junctions = glob.glob(f'{dir_to_junctions}/{self.gene_symbol}*.csv')
+            if self.filename_target_junctions is not None:
+                path_to_junctions = [os.path.join(dir_to_junctions, self.filename_target_junctions)]
+            else:
+                path_to_junctions = glob.glob(os.path.join(dir_to_junctions, f'{self.gene_symbol}*.csv'))
             junctions = pd.read_csv(path_to_junctions[0], sep=',', index_col=0)
         except (FileNotFoundError, ValueError, IndexError) as ex:
             raise ex.__class__(f'Junction data are not found for {self.gene_symbol}.') from ex
 
         # load genes to subset
+        self.log(logging.INFO, 'Loading genes data...')
         gene_list = open(path_to_gene_ids, 'r').readlines()
         gene_list = list(map(lambda l: l.strip('\n'), gene_list))
 
         self.log(logging.INFO, f'Processing {self.gene_symbol} {self.condition.name.lower()} data...')
         # process junctions
-        psi = self.process_junctions(
-            junctions=junctions,
-            cutoff_reads=self.cutoff_reads
-        )
+        psi = self.process_junctions(junctions=junctions)
 
         # transpose data (samples x features)
         rnaseq = rnaseq.T
         psi = psi.T
 
         # process RNA-Seq
-        rnaseq = self.process_rnaseq(
-            rnaseq=rnaseq,
-            gene_ids=gene_list,
-            ratio_nan_to_drop=self.ratio_nan_to_drop,
-            log_transform=self.log_transform
-        )
+        rnaseq = self.process_rnaseq(rnaseq=rnaseq, gene_ids=gene_list)
 
         # combine data
-        data = self.prepare_data(
-            rnaseq=rnaseq,
-            psi=psi,
-            metadata=metadata,
-            condition=self.condition,
-            pair_tissues=self.pair_tissues,
-            sample_size_per_tissue_min=self.sample_size_per_tissue_min
-        )
-
+        data = self.prepare_data(rnaseq=rnaseq, psi=psi, metadata=metadata)
         self.log(logging.INFO, f'Data is processed for {data.shape[0]} samples and {data.shape[1] - 1} genes.')
 
         # save data
-        setup_id = self.get_setup_id(
-            condition=self.condition,
-            cutoff_reads=self.cutoff_reads,
-            log_transform=self.log_transform,
-            pair_tissues=self.pair_tissues,
-            include_adjacent_tissues=self.include_adjacent_tissues,
-            sample_size_per_tissue_min=self.sample_size_per_tissue_min,
-        )
-        filename = f'{self.gene_symbol}_{setup_id}.pkl'
+        filename = f'{self.gene_symbol}_{self.get_setup_id()}.pkl'
         path_to_data = os.path.join(self.out_dir, self.gene_symbol, filename)
         os.makedirs(os.path.dirname(path_to_data), exist_ok=True)
 
         self.log(logging.INFO, f'Saving data as `{filename}`...')
         pd.to_pickle(data, path_to_data)
         self.path_to_file = path_to_data
 
@@ -298,212 +286,177 @@
         psi = (inclusion / (inclusion + exclusion))
 
         sample_ids = reads.columns.values.tolist()
         psi = pd.DataFrame.from_records(psi, columns=sample_ids, index=['psi'])
 
         return psi
 
-    @classmethod
-    def filter_reads(
-            cls,
-            reads: pd.DataFrame,
-            cutoff_reads: float
-    ) -> pd.DataFrame:
+    def filter_reads(self, reads: pd.DataFrame) -> pd.DataFrame:
 
         # subset samples w.r.t. coverage of reads
-        if cutoff_reads == 0:
+        if self.cutoff_reads == 0:
             # remove samples with no reads (zeros in all junctions)
-            samples_coverage_low = reads.columns[(reads == cutoff_reads).all().values].values.tolist()
+            samples_coverage_low = reads.columns[(reads == self.cutoff_reads).all().values].values.tolist()
         else:
             # remove samples w.r.t. the defined cutoff
-            samples_coverage_low = reads.columns[(reads < cutoff_reads).all().values].values.tolist()
+            samples_coverage_low = reads.columns[(reads < self.cutoff_reads).all().values].values.tolist()
 
         if len(samples_coverage_low) > 0:
-            cls.log(logging.INFO,
-                          f'\tFiltering {len(samples_coverage_low)} low-coverage (cutoff={cutoff_reads}) samples...'
-                          )
+            self.log(
+                logging.INFO, f'\tFiltering {len(samples_coverage_low)} low-coverage (cutoff={self.cutoff_reads}) samples...'
+            )
 
         reads = reads.drop(samples_coverage_low, axis=1)
 
         if reads.empty:
             sys.exit(
                 'Program is terminated as no samples left in filtered reads data (all samples have low-coverage).'
-                'Try to update `cutoff_reads` parameter (minimize it or pass `None` to ignore the filtering)'
-                'and/or include more samples and/or analyse another data.')
+                'Try to update `cutoff_reads` parameter (minimize it or pass `None` to ignore the filtering) '
+                'and/or include more samples and/or analyse another data.'
+            )
         else:
             return reads
 
-    @classmethod
-    def process_junctions(
-            cls,
-            junctions: pd.DataFrame,
-            cutoff_reads: Optional[int] = 0
-    ) -> pd.DataFrame:
+    def process_junctions(self, junctions: pd.DataFrame) -> pd.DataFrame:
 
         junctions = junctions.fillna(0)
 
         # remove samples w.r.t. read coverage
-        if cutoff_reads >= 0:
-            junctions = cls.filter_reads(junctions, cutoff_reads)
+        if self.cutoff_reads >= 0:
+            junctions = self.filter_reads(junctions)
 
         # calculate PSI
-        psi = cls.calculate_psi(junctions)
+        psi = self.calculate_psi(junctions)
         psi.index = ['psi']
 
         # remove samples with missing values
         psi = psi.replace([np.inf, -np.inf], np.nan).dropna(axis=1)
 
         return psi
 
-    @classmethod
-    def process_rnaseq(
-            cls,
-            rnaseq: pd.DataFrame,
-            gene_ids: List,
-            ratio_nan_to_drop: Optional[float] = 1.0,
-            log_transform: bool = False
-    ) -> pd.DataFrame:
+    def process_rnaseq(self, rnaseq: pd.DataFrame, gene_ids: List) -> pd.DataFrame:
 
         # filter genes w.r.t. missing values
         mask_sparse: np.array = rnaseq.isna().values
         if mask_sparse.any():
-            if ratio_nan_to_drop is not None:
-                if ratio_nan_to_drop == 1.0:
+            if self.ratio_nan_to_drop is not None:
+                if self.ratio_nan_to_drop == 1.0:
                     mask_sparse = mask_sparse.any(axis=0)
                 else:
-                    mask_sparse = mask_sparse.mean(axis=0) > ratio_nan_to_drop
+                    mask_sparse = mask_sparse.mean(axis=0) > self.ratio_nan_to_drop
 
-                n_rbps_sparse = mask_sparse.sum()
+                n_genes_sparse = mask_sparse.sum()
                 genes_sparse = rnaseq.columns[mask_sparse]
                 rnaseq = rnaseq.drop(genes_sparse, axis=1)
 
-                cls.log(
+                self.log(
                     logging.INFO,
-                    '\tFiltering {} features (sparsity={:.1%})...'.format(n_rbps_sparse, 1.0 - ratio_nan_to_drop)
+                    '\tFiltering {} features (sparsity={:.1%})...'.format(n_genes_sparse, 1.0 - self.ratio_nan_to_drop)
                 )
-            if ratio_nan_to_drop != 1.0:
+            if self.ratio_nan_to_drop != 1.0:
                 rnaseq = rnaseq.fillna(0)
 
         # subset genes
         genes_found = list(set(gene_ids) & set(rnaseq.columns))
         if not genes_found:
             # format gene names to match
             sep_gene_ids = '.'
             gene_ids_all = rnaseq.columns.to_list()
             if any([sep_gene_ids in idx for idx in gene_ids]) or any([sep_gene_ids in idx for idx in gene_ids_all]):
                 gene_ids = [idx.split(sep_gene_ids)[0] for idx in gene_ids]
                 rnaseq.columns = [idx.split(sep_gene_ids)[0] for idx in gene_ids_all]
             genes_found = list(set(gene_ids) & set(rnaseq.columns))
         if genes_found:
             # subset genes
-            cls.log(logging.INFO, f'\tSelecting {len(genes_found)} genes...')
+            self.log(logging.INFO, f'\tSelecting {len(genes_found)} candidate genes...')
             rnaseq = rnaseq.reindex(genes_found, axis=1)
         else:
             sys.exit('Program is terminated as no gene IDs to subset are found in the RNA-Seq data.'
                      'Pass a list of another genes IDs as `gene_ids` and/or check whether Ensembl IDs are correct.')
 
         # log-transform values
-        if log_transform:
-            cls.log(logging.INFO, '\tLog-transforming expression values...')
+        if self.log_transform:
+            self.log(logging.INFO, '\tLog-transforming expression values...')
             rnaseq = rnaseq.apply(lambda x: np.log2(x + 1e-3))
 
             if rnaseq.isnull().sum().sum() > 0:
-                cls.log(logging.WARNING, 'Log-transformed data contain NaN values')
+                self.log(logging.WARNING, 'Log-transformed data contain NaN values')
 
         return rnaseq
 
-    @classmethod
     def prepare_data(
-            cls,
+            self,
             rnaseq: pd.DataFrame,
             psi: pd.DataFrame,
-            metadata: pd.DataFrame,
-            condition: Condition,
-            pair_tissues: Optional[bool] = None,
-            sample_size_per_tissue_min: Optional[int] = None
+            metadata: pd.DataFrame
     ) -> pd.DataFrame:
 
         # aggregate data
         data = rnaseq.join(psi, how='inner')
 
         # annotate data
         data = data.join(metadata, how='inner')
 
         # subset conditions and tissues
-        data = cls.subset_conditions(
-            data, condition=condition, pair_tissues=pair_tissues, sample_size_per_tissue_min=sample_size_per_tissue_min
-        )
+        data = self.subset_conditions(data)
 
         # remove annotation
         data = data.select_dtypes(include=[np.number])
 
         return data
 
-    @classmethod
-    def subset_conditions(
-            cls,
-            data_annotated: pd.DataFrame,
-            condition: Condition,
-            pair_tissues: Optional[bool] = False,
-            sample_size_per_tissue_min: Optional[bool] = False
-    ) -> pd.DataFrame:
+    def subset_conditions(self, data_annotated: pd.DataFrame) -> pd.DataFrame:
 
         # pair tissues in TCGA and GTEx data
-        if pair_tissues:
+        if self.pair_tissues:
             tissues_common = list(
                 set(data_annotated.loc[data_annotated['cohort'] == Cohort.TCGA.name, 'tissue']).intersection(
                     set(data_annotated.loc[data_annotated['cohort'] == Cohort.GTEX.name, 'tissue'])))
             data_annotated = data_annotated[data_annotated['tissue'].isin(tissues_common)]
-            cls.log(logging.INFO, f"\tSelecting {data_annotated['tissue'].nunique()} common tissues...")
+            self.log(logging.INFO, f"\tSelecting {data_annotated['tissue'].nunique()} common tissues...")
 
         # subset conditions
-        if condition != Condition.Combined:
+        if self.condition != Condition.Combined:
             try:
-                cohort_name: str = Cohort.TCGA.name if condition == Condition.Tumor else Cohort.GTEX.name
+                cohort_name: str = Cohort.TCGA.name if self.condition == Condition.Tumor else Cohort.GTEX.name
                 mask_subsets = data_annotated['cohort'].str.contains(cohort_name)
                 data_annotated = data_annotated[mask_subsets]
             except ValueError:
                 raise logging.warning(
-                    f'`{condition.name}` samples are not found. Check out data or/and Try another condition(s).')
+                    f'`{self.condition.name}` samples are not found. Check out data or/and Try another condition(s).')
 
         # subset tissues by sample size
         samples_per_tissue = data_annotated['tissue'].value_counts()
-        cond_tissues_with_small_sample_size = samples_per_tissue < sample_size_per_tissue_min
-        if sample_size_per_tissue_min is not None and np.any(cond_tissues_with_small_sample_size):
+        cond_tissues_with_small_sample_size = samples_per_tissue < self.sample_size_per_tissue_min
+        if self.sample_size_per_tissue_min is not None and np.any(cond_tissues_with_small_sample_size):
             tissues_to_be_filtered_out = samples_per_tissue[cond_tissues_with_small_sample_size].index.to_list()
             data_annotated = data_annotated.loc[~data_annotated['tissue'].isin(tissues_to_be_filtered_out), :]
-            cls.log(
+            self.log(
                 logging.INFO,
-                f"\tSelecting {data_annotated['tissue'].nunique()} tissues with at least {sample_size_per_tissue_min} samples..."
+                '\tSelecting {} tissues with at least {} samples...'.format(
+                    data_annotated['tissue'].nunique(), self.sample_size_per_tissue_min
+                )
             )
 
         return data_annotated
 
-    @staticmethod
-    def get_setup_id(
-            condition: Condition,
-            log_transform: bool,
-            pair_tissues: bool,
-            include_adjacent_tissues: bool,
-            cutoff_reads: Optional[int] = None,
-            sample_size_per_tissue_min: Optional[int] = None,
-    ) -> str:
+    def get_setup_id(self) -> str:
 
-        setup_id = f'r{cutoff_reads if cutoff_reads >= 0 else ""}'
-        setup_id += 'Log' if log_transform else ''
+        setup_id = f'r{self.cutoff_reads}' if (self.cutoff_reads is not None and self.cutoff_reads > 0) else ''
+        setup_id += 'Log' if self.log_transform else ''
 
         tissue_selection = ''
-        tissue_selection += 'A' if include_adjacent_tissues else ''
-        tissue_selection += 'P' if pair_tissues else ''
+        tissue_selection += 'A' if self.include_adjacent_tissues else ''
+        tissue_selection += 'P' if self.pair_tissues else ''
         setup_id += f't{tissue_selection}' if tissue_selection else ''
 
-        if sample_size_per_tissue_min is not None and sample_size_per_tissue_min > 0:
-            setup_id += f's{sample_size_per_tissue_min}'
+        if (self.sample_size_per_tissue_min is not None and self.sample_size_per_tissue_min > 0):
+            setup_id += f's{self.sample_size_per_tissue_min}'
 
-        setup_id += f'c{condition.name}'
+        setup_id += f'c{self.condition.name}'
 
         return setup_id
 
     @property
     def meta(self):
         return str({
             'gene_symbol': self.gene_symbol,
@@ -512,9 +465,9 @@
             'condition': self.condition,
             'cutoff_reads': self.cutoff_reads,
             'ratio_nan_to_drop': self.ratio_nan_to_drop,
             'log_transform': self.log_transform,
             'pair_tissues': self.pair_tissues,
             'include_adjacent_tissues': self.include_adjacent_tissues,
             'sample_size_per_tissue_min': self.sample_size_per_tissue_min,
-            'meta': super(RawLoader, self).meta
+            'meta': super().meta
         })
```

### Comparing `regulAS-2023.7/regulAS.egg-info/SOURCES.txt` & `regulAS-2023.7.1/regulAS.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,12 @@
 regulAS/core/regulas.py
 regulAS/persistence/__init__.py
 regulAS/persistence/dao.py
 regulAS/reports/__init__.py
 regulAS/reports/base.py
 regulAS/reports/export_textual.py
 regulAS/reports/export_visual.py
-regulAS/reports/export_visual_vis.py
 regulAS/reports/performance.py
 regulAS/reports/ranking.py
 regulAS/utils/__init__.py
 regulAS/utils/base.py
 regulAS/utils/loader.py
```

