# Comparing `tmp/checkatlas-0.4.0.tar.gz` & `tmp/checkatlas-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.4.0.tar", max compression
+gzip compressed data, was "checkatlas-0.4.1.tar", max compression
```

## Comparing `checkatlas-0.4.0.tar` & `checkatlas-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1506 2023-07-23 12:12:35.502042 checkatlas-0.4.0/LICENSE
--rw-r--r--   0        0        0     4882 2023-07-23 12:12:35.502042 checkatlas-0.4.0/README.md
--rw-r--r--   0        0        0      111 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/__init__.py
--rw-r--r--   0        0        0     4674 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/__main__.py
--rw-r--r--   0        0        0    24921 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/atlas.py
--rw-r--r--   0        0        0     9019 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/cellranger.py
--rw-r--r--   0        0        0    11502 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     2913 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0       45 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      254 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4124 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/seurat.py
--rw-r--r--   0        0        0        6 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/VERSION
--rw-r--r--   0        0        0      107 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4523 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     4239 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/checkatlas_workflow_arguments.py
--rw-r--r--   0        0        0     2760 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-23 12:12:35.502042 checkatlas-0.4.0/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1427 2023-07-23 12:12:35.710046 checkatlas-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6275 1970-01-01 00:00:00.000000 checkatlas-0.4.0/setup.py
--rw-r--r--   0        0        0     5825 1970-01-01 00:00:00.000000 checkatlas-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-24 15:48:48.763803 checkatlas-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4384 2023-07-24 15:48:48.763803 checkatlas-0.4.1/README.md
+-rw-r--r--   0        0        0      111 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4674 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24921 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/atlas.py
+-rw-r--r--   0        0        0     9019 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/cellranger.py
+-rw-r--r--   0        0        0    11502 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     2913 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0       45 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      254 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4124 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/seurat.py
+-rw-r--r--   0        0        0        6 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/VERSION
+-rw-r--r--   0        0        0      107 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4523 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     4239 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/checkatlas_workflow_arguments.py
+-rw-r--r--   0        0        0     2760 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-24 15:48:48.763803 checkatlas-0.4.1/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1427 2023-07-24 15:48:48.991802 checkatlas-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5741 1970-01-01 00:00:00.000000 checkatlas-0.4.1/setup.py
+-rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 checkatlas-0.4.1/PKG-INFO
```

### Comparing `checkatlas-0.4.0/LICENSE` & `checkatlas-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/README.md` & `checkatlas-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: checkatlas
+Version: 0.4.1
+Summary: One liner tool to check the quality of your single-cell atlases.
+Home-page: https://checkatlas.readthedocs.io/
+License: BSD 3-Clause
+Author: becavin-lab
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
+Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
+Requires-Dist: rpy2 (==3.5.10)
+Requires-Dist: scanpy (>=1.9.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: types-pyyaml (>=6.0.12.6,<7.0.0.0)
+Project-URL: Documentation, https://checkatlas.readthedocs.io/
+Project-URL: Repository, https://github.com/becavin-lab/checkatlas/
+Description-Content-Type: text/markdown
+
 # ![CheckAtlas](docs/images/checkatlas_logo.png) 
 
 
 ![PyPI](https://img.shields.io/pypi/v/checkatlas)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)
 ![PyPI - License](https://img.shields.io/pypi/l/checkatlas)
 ![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)
@@ -12,131 +36,96 @@
 [![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)
 
 ![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)
 ![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)
 ![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)
 
 CheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the
-quality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,
+quality control tables and figures which can be then processed by multiqc. CheckAtlas is able to check the quality of Scanpy, Seurat,
 and CellRanger files.
 
+More information on the [read the doc page](https://checkatlas.readthedocs.io/en/latest/)
 
-## Summary
 
-### Parse Scanpy, Seurat and CellRanger objects
+## Summary
 
-The checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.
+Powered by nextflow, checkatlas can be ran in one command line:
 
+```bash
+nextflow run nf-core-checkatlas --path search_folder/
+```
 
-### Create checkatlas summary files
+The checkatlas workflow start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.
 
-Go through all atlas files and produce summary information:
+Then, it goes through all atlas files and produce summary information:
 
 - All basic QC (nRNA, nFeature, ratio_mito)
 - General information (nbcells, nbgenes, nblayers)
 - All elements in atlas files (obs, obsm, uns, var, varm)
 - Reductions (pca, umap, tsne)
 - All metrics (clustering, annotation, dimreduction, specificity)
 
-### Parse checkatlas files in MultiQC
+All tables and figs are saved in the **checkatlas_files** folder in your search folder.
 
-   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas
+A single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.
 
-https://checkatlas.readthedocs.io/en/latest/
+![Checkatlas workflow](docs/checkatlas_workflow.png)
 
-## Examples
 
-### Example 1 - Evaluate and compare heterogenous scanpy atlases
+## Examples
 
-Evaluate and compare different atlases:
+- Evaluate and compare different scanpy atlases:
 [Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)
 
-### Example 2 - Evaluate different version of the same atlas
-
-Evaluate different version of your atlas:
+- Evaluate different version of one atlas:
 [Example 2](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_2/Checkatlas_MultiQC.html)
 
-### Example 3 - Evaluate Scanpy, Seurat and CellRanger atlases
-
-Evaluate Scanpy, Seurat and CellRanger objects in your folder:
+- Evaluate Scanpy, Seurat and CellRanger objects in your folder:
 [Example 3](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_3/Checkatlas_MultiQC.html)
 
-### Example 4 - Evaluate post-process and raw atlases
-
-Evaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:
+- Evaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:
 [Example 4](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_4/Checkatlas_MultiQC.html)
 
-### Example 5 - Avaluate different cellranger version atlases
-Evaluate different Cellranger atlases with multiple chemistry version and cellranger version:
+- Evaluate different Cellranger atlases with multiple chemistry version and cellranger version:
 [Example 5](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_5/Checkatlas_MultiQC.html)
 
 
 ## Installation
 
-CheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.
+CheckAtlas is in two parts. The checkatlas pythn module which can be downloaded with PyPi, and the checkatlas workflow which can be downloaded with nextflow.
 
-### Install checkatlas development version
+```bash
+pip install checkatlas
+```
 
 ```bash
-git clone git@github.com:becavin-lab/checkatlas.git
-pip install checkatlas/.
+nextflow pull becavin-lab/nf-core-checkatlas
 ```
 
-Install MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.
+You need also to install a version of MultiQC with checkatlas capability (for the moment). This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.
 
 ```bash
 git clone git@github.com:becavin-lab/MultiQC.git
 cd MultiQC/
 git checkout checkatlas
 pip install .
 ```
 
-### Install it from PyPI
-
-```bash
-pip install checkatlas
-```
-
-### Install Seurat
-
-To be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.
-
-```bash
-conda create -n checkatlas python=3.9
-pip install checkatlas
-conda install -c bioconda r-seurat
-```
-
-Or, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.
+Finally, checkatlas comes with rpy2 to perform the interface between python and R. But, it does not automatically install Seurat. So if you want to screen Seurat atlases you need to perfrom this last installation
 
 ```bash
 % R
 > install.packages('Seurat')
 > library(Seurat)
 ```
 
 
-## Usage
-
-The one liner way to run checkatlas is the following: 
-
-```bash
-$ cd your_search_folder/
-$ python -m checkatlas .
-#or
-$ checkatlas .
-```
-
-Or run it inside your python workflow.
-
-```py
-from checkatlas import checkatlas
-checkatlas.run(path, atlas_list, multithread, n_cpus)
-```
-
-
 ## Development
 
+This project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.
+
 Read the [CONTRIBUTING.md](docs/contributing.md) file.
 
+
 Project developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)
 
+
```

### Comparing `checkatlas-0.4.0/checkatlas/__main__.py` & `checkatlas-0.4.1/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/atlas.py` & `checkatlas-0.4.1/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/cellranger.py` & `checkatlas-0.4.1/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/checkatlas.py` & `checkatlas-0.4.1/checkatlas/checkatlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/checkatlas_workflow.py` & `checkatlas-0.4.1/checkatlas/checkatlas_workflow.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.4.1/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/metrics.py` & `checkatlas-0.4.1/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.4.1/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.4.1/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.4.1/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.4.1/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/seurat.py` & `checkatlas-0.4.1/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.4.1/checkatlas/utils/checkatlas_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/utils/checkatlas_workflow_arguments.py` & `checkatlas-0.4.1/checkatlas/utils/checkatlas_workflow_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/utils/files.py` & `checkatlas-0.4.1/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/utils/folders.py` & `checkatlas-0.4.1/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.4.1/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.0/pyproject.toml` & `checkatlas-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.4.0"
+version = "0.4.1"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf","pyproject.toml"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.4.0/setup.py` & `checkatlas-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
-    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n### Example 1 - Evaluate and compare heterogenous scanpy atlases\n\nEvaluate and compare different atlases:\n[Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)\n\n### Example 2 - Evaluate different version of the same atlas\n\nEvaluate different version of your atlas:\n[Example 2](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_2/Checkatlas_MultiQC.html)\n\n### Example 3 - Evaluate Scanpy, Seurat and CellRanger atlases\n\nEvaluate Scanpy, Seurat and CellRanger objects in your folder:\n[Example 3](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_3/Checkatlas_MultiQC.html)\n\n### Example 4 - Evaluate post-process and raw atlases\n\nEvaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:\n[Example 4](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_4/Checkatlas_MultiQC.html)\n\n### Example 5 - Avaluate different cellranger version atlases\nEvaluate different Cellranger atlases with multiple chemistry version and cellranger version:\n[Example 5](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_5/Checkatlas_MultiQC.html)\n\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
+    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to check the quality of Scanpy, Seurat,\nand CellRanger files.\n\nMore information on the [read the doc page](https://checkatlas.readthedocs.io/en/latest/)\n\n\n## Summary\n\nPowered by nextflow, checkatlas can be ran in one command line:\n\n```bash\nnextflow run nf-core-checkatlas --path search_folder/\n```\n\nThe checkatlas workflow start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\nThen, it goes through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\nAll tables and figs are saved in the **checkatlas_files** folder in your search folder.\n\nA single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.\n\n![Checkatlas workflow](docs/checkatlas_workflow.png)\n\n\n## Examples\n\n- Evaluate and compare different scanpy atlases:\n[Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)\n\n- Evaluate different version of one atlas:\n[Example 2](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_2/Checkatlas_MultiQC.html)\n\n- Evaluate Scanpy, Seurat and CellRanger objects in your folder:\n[Example 3](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_3/Checkatlas_MultiQC.html)\n\n- Evaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:\n[Example 4](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_4/Checkatlas_MultiQC.html)\n\n- Evaluate different Cellranger atlases with multiple chemistry version and cellranger version:\n[Example 5](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_5/Checkatlas_MultiQC.html)\n\n\n## Installation\n\nCheckAtlas is in two parts. The checkatlas pythn module which can be downloaded with PyPi, and the checkatlas workflow which can be downloaded with nextflow.\n\n```bash\npip install checkatlas\n```\n\n```bash\nnextflow pull becavin-lab/nf-core-checkatlas\n```\n\nYou need also to install a version of MultiQC with checkatlas capability (for the moment). This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\nFinally, checkatlas comes with rpy2 to perform the interface between python and R. But, it does not automatically install Seurat. So if you want to screen Seurat atlases you need to perfrom this last installation\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Development\n\nThis project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
```

