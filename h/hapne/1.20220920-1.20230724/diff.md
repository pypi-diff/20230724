# Comparing `tmp/HapNe-1.20220920.tar.gz` & `tmp/hapne-1.20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HapNe-1.20220920.tar", last modified: Tue Sep 20 15:49:57 2022, max compression
+gzip compressed data, was "hapne-1.20230724.tar", last modified: Mon Jul 24 15:29:05 2023, max compression
```

## Comparing `HapNe-1.20220920.tar` & `hapne-1.20230724.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.434826 HapNe-1.20220920/
--rw-r--r--   0 clz033   (37169) palamara (31067)    35149 2022-06-30 12:53:53.000000 HapNe-1.20220920/LICENSE
--rw-r--r--   0 clz033   (37169) palamara (31067)     6850 2022-09-20 15:49:57.435047 HapNe-1.20220920/PKG-INFO
--rw-r--r--   0 clz033   (37169) palamara (31067)     7317 2022-08-14 16:29:22.000000 HapNe-1.20220920/README.md
--rw-r--r--   0 clz033   (37169) palamara (31067)      104 2022-06-30 12:53:53.000000 HapNe-1.20220920/pyproject.toml
--rw-r--r--   0 clz033   (37169) palamara (31067)      961 2022-09-20 15:49:57.435962 HapNe-1.20220920/setup.cfg
--rw-r--r--   0 clz033   (37169) palamara (31067)       39 2022-08-01 08:48:38.000000 HapNe-1.20220920/setup.py
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.305849 HapNe-1.20220920/src/
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.342424 HapNe-1.20220920/src/HapNe.egg-info/
--rw-r--r--   0 clz033   (37169) palamara (31067)     6850 2022-09-20 15:49:56.000000 HapNe-1.20220920/src/HapNe.egg-info/PKG-INFO
--rw-r--r--   0 clz033   (37169) palamara (31067)      697 2022-09-20 15:49:57.000000 HapNe-1.20220920/src/HapNe.egg-info/SOURCES.txt
--rw-r--r--   0 clz033   (37169) palamara (31067)        1 2022-09-20 15:49:56.000000 HapNe-1.20220920/src/HapNe.egg-info/dependency_links.txt
--rw-r--r--   0 clz033   (37169) palamara (31067)       98 2022-09-20 15:49:57.000000 HapNe-1.20220920/src/HapNe.egg-info/requires.txt
--rw-r--r--   0 clz033   (37169) palamara (31067)        6 2022-09-20 15:49:57.000000 HapNe-1.20220920/src/HapNe.egg-info/top_level.txt
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.361478 HapNe-1.20220920/src/hapne/
--rw-r--r--   0 clz033   (37169) palamara (31067)       88 2022-08-01 08:36:58.000000 HapNe-1.20220920/src/hapne/__init__.py
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.413835 HapNe-1.20220920/src/hapne/backend/
--rw-r--r--   0 clz033   (37169) palamara (31067)    12891 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/backend/DemographicHistory.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     1024 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/backend/DemographicHistory2StatsModelAdapter.py
--rw-r--r--   0 clz033   (37169) palamara (31067)    14626 2022-08-14 16:29:22.000000 HapNe-1.20220920/src/hapne/backend/HapNe.py
--rw-r--r--   0 clz033   (37169) palamara (31067)    17686 2022-08-01 12:41:09.000000 HapNe-1.20220920/src/hapne/backend/IO.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     7393 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/backend/StatsModel.py
--rw-r--r--   0 clz033   (37169) palamara (31067)        0 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/backend/__init__.py
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.414970 HapNe-1.20220920/src/hapne/convert/
--rw-r--r--   0 clz033   (37169) palamara (31067)        0 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/convert/__init__.py
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.432596 HapNe-1.20220920/src/hapne/convert/mathii_scripts/
--rw-r--r--   0 clz033   (37169) palamara (31067)        0 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/convert/mathii_scripts/__init__.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     9597 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/convert/mathii_scripts/py3Eigenstrat.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     6413 2022-09-20 15:38:24.000000 HapNe-1.20220920/src/hapne/convert/tools.py
-drwxr-sr-x   0 clz033   (37169) palamara (31067)        0 2022-09-20 15:49:57.434428 HapNe-1.20220920/src/hapne/files/
--rw-r--r--   0 clz033   (37169) palamara (31067)     2380 2022-06-30 12:53:53.000000 HapNe-1.20220920/src/hapne/files/regions.txt
--rw-r--r--   0 clz033   (37169) palamara (31067)      314 2022-08-01 08:36:58.000000 HapNe-1.20220920/src/hapne/fit.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     1079 2022-08-01 08:36:58.000000 HapNe-1.20220920/src/hapne/ibd.py
--rw-r--r--   0 clz033   (37169) palamara (31067)    12009 2022-08-01 08:48:38.000000 HapNe-1.20220920/src/hapne/ld.py
--rw-r--r--   0 clz033   (37169) palamara (31067)     4024 2022-08-14 16:29:22.000000 HapNe-1.20220920/src/hapne/utils.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.987781 hapne-1.20230724/
+-rw-r--r--   0 romainfournier   (501) staff       (20)    35149 2023-04-24 08:33:59.000000 hapne-1.20230724/LICENSE
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7002 2023-07-24 15:29:05.987889 hapne-1.20230724/PKG-INFO
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7452 2023-07-24 14:05:01.000000 hapne-1.20230724/README.md
+-rw-r--r--   0 romainfournier   (501) staff       (20)      104 2023-04-24 08:33:59.000000 hapne-1.20230724/pyproject.toml
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6278 2023-07-24 14:05:01.000000 hapne-1.20230724/read_me.md
+-rw-r--r--   0 romainfournier   (501) staff       (20)      999 2023-07-24 15:29:05.988514 hapne-1.20230724/setup.cfg
+-rw-r--r--   0 romainfournier   (501) staff       (20)       39 2023-04-24 08:33:59.000000 hapne-1.20230724/setup.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.974085 hapne-1.20230724/src/
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.977811 hapne-1.20230724/src/HapNe.egg-info/
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7002 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/PKG-INFO
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1083 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/SOURCES.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)        1 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/dependency_links.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)      103 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/requires.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)        6 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/top_level.txt
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.980214 hapne-1.20230724/src/hapne/
+-rw-r--r--   0 romainfournier   (501) staff       (20)       88 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.982838 hapne-1.20230724/src/hapne/backend/
+-rw-r--r--   0 romainfournier   (501) staff       (20)    12891 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/DemographicHistory.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1024 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/DemographicHistory2StatsModelAdapter.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    20487 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/backend/HapNe.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    21198 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/backend/IO.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7393 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/StatsModel.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.983613 hapne-1.20230724/src/hapne/convert/
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.984290 hapne-1.20230724/src/hapne/convert/mathii_scripts/
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/mathii_scripts/__init__.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     9597 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/mathii_scripts/py3Eigenstrat.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6560 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/convert/tools.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.985091 hapne-1.20230724/src/hapne/files/
+-rw-r--r--   0 romainfournier   (501) staff       (20)     2380 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/files/regions_grch37.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)     2664 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/files/regions_grch38.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)      314 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/fit.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1194 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/ibd.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    16764 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/ld.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1727 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/output.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     5330 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/utils.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.987556 hapne-1.20230724/tests/
+-rw-r--r--   0 romainfournier   (501) staff       (20)      647 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_build_hist.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)      809 2023-07-24 12:29:12.000000 hapne-1.20230724/tests/test_compute_ld.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1314 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_eigenstrat2vcf.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1791 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_hapne.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     3550 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_time_het.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)      329 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_vcf2splitbed.py
```

### Comparing `HapNe-1.20220920/LICENSE` & `hapne-1.20230724/LICENSE`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/PKG-INFO` & `hapne-1.20230724/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: HapNe
-Version: 1.20220920
+Name: hapne
+Version: 1.20230724
 Summary: Haplotype-based inference of recent effective population size in modern and ancient DNA samples
 Home-page: https://github.com/PalamaraLab/HapNe
 Author: Romain Fournier (PalamaraLab, Department of Statistics, Oxford University)
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/PalamaraLab/HapNe/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -56,21 +58,23 @@
 [CONFIG]
 vcf_file=data
 keep=data.keep
 map=genetic_map_chr@_combined_b37.txt
 pseudo_diploid=False
 output_folder=HapNe/data
 population_name=POP
+genome_build=grch37
 ```
 * vcf_file: path to the vcf file (without the .vcf.gz extension)
 * keep (facultative): samples to keep, useful to filter out relatives 
 * map: path to the genetic maps
 * pseudo_diploid: False for modern data, true for ancient ones
 * output_folder: folder where the results will be saved
 * population_name: name of the analysis
+* genome_build: genome build used (grch37 (default) or grch38)
 
 The analysis can be run using a script like this one:
 ```python
 from configparser import ConfigParser
 import argparse
 
 from hapne.convert.tools import split_convert_vcf
@@ -125,14 +129,15 @@
 vcf_file=data
 keep=data.keep
 map=genetic_map_chr@_combined_b37.txt
 pseudo_diploid=False
 output_folder=HapNe/data
 population_name=POP
 ibd_files=FASTSMC_OUTPUT_FOLDER
+genome_build=grch37 # or grch38
 ```
 
 Using this config file, HapNe-IBD can be run using the following script:
 ```python
 from configparser import ConfigParser
 from hapne.ibd import build_hist
 
@@ -208,7 +213,9 @@
 If you use this software, please cite:
 
 R. Fournier, D. Reich, P. Palamara. Haplotype-based inference of recent effective population size in modern and ancient DNA samples. (preprint) bioRxiv, 2022.
 # Acknowledgments  
 Two scripts of the `convert` module were downloaded from the following repositories and edited to fit into this package:
 - "https://github.com/mathii/pyEigenstrat" 
 - "https://github.com/mathii/gdc"
+
+
```

### Comparing `HapNe-1.20220920/README.md` & `hapne-1.20230724/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,21 +55,23 @@
 [CONFIG]
 vcf_file=data
 keep=data.keep
 map=genetic_map_chr@_combined_b37.txt
 pseudo_diploid=False
 output_folder=HapNe/data
 population_name=POP
+genome_build=grch37
 ```
 * vcf_file: path to the vcf file (without the .vcf.gz extension)
 * keep (facultative): samples to keep, useful to filter out relatives 
-* map: path to the genetic maps
+* map: path to the genetic maps (note: if grch38 is used, genome_build must be set to grch38)
 * pseudo_diploid: False for modern data, true for ancient ones
 * output_folder: folder where the results will be saved
 * population_name: name of the analysis
+* genome_build: genome build used (grch37 or grch38)
 
 The analysis can be ran using a script like this one:
 ```python
 from configparser import ConfigParser
 import argparse
 
 from hapne.convert.tools import split_convert_vcf
```

### Comparing `HapNe-1.20220920/src/HapNe.egg-info/PKG-INFO` & `hapne-1.20230724/src/HapNe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: HapNe
-Version: 1.20220920
+Name: hapne
+Version: 1.20230724
 Summary: Haplotype-based inference of recent effective population size in modern and ancient DNA samples
 Home-page: https://github.com/PalamaraLab/HapNe
 Author: Romain Fournier (PalamaraLab, Department of Statistics, Oxford University)
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/PalamaraLab/HapNe/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -56,21 +58,23 @@
 [CONFIG]
 vcf_file=data
 keep=data.keep
 map=genetic_map_chr@_combined_b37.txt
 pseudo_diploid=False
 output_folder=HapNe/data
 population_name=POP
+genome_build=grch37
 ```
 * vcf_file: path to the vcf file (without the .vcf.gz extension)
 * keep (facultative): samples to keep, useful to filter out relatives 
 * map: path to the genetic maps
 * pseudo_diploid: False for modern data, true for ancient ones
 * output_folder: folder where the results will be saved
 * population_name: name of the analysis
+* genome_build: genome build used (grch37 (default) or grch38)
 
 The analysis can be run using a script like this one:
 ```python
 from configparser import ConfigParser
 import argparse
 
 from hapne.convert.tools import split_convert_vcf
@@ -125,14 +129,15 @@
 vcf_file=data
 keep=data.keep
 map=genetic_map_chr@_combined_b37.txt
 pseudo_diploid=False
 output_folder=HapNe/data
 population_name=POP
 ibd_files=FASTSMC_OUTPUT_FOLDER
+genome_build=grch37 # or grch38
 ```
 
 Using this config file, HapNe-IBD can be run using the following script:
 ```python
 from configparser import ConfigParser
 from hapne.ibd import build_hist
 
@@ -208,7 +213,9 @@
 If you use this software, please cite:
 
 R. Fournier, D. Reich, P. Palamara. Haplotype-based inference of recent effective population size in modern and ancient DNA samples. (preprint) bioRxiv, 2022.
 # Acknowledgments  
 Two scripts of the `convert` module were downloaded from the following repositories and edited to fit into this package:
 - "https://github.com/mathii/pyEigenstrat" 
 - "https://github.com/mathii/gdc"
+
+
```

### Comparing `HapNe-1.20220920/src/HapNe.egg-info/SOURCES.txt` & `hapne-1.20230724/src/HapNe.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 LICENSE
 README.md
 pyproject.toml
+read_me.md
 setup.cfg
 setup.py
 src/HapNe.egg-info/PKG-INFO
 src/HapNe.egg-info/SOURCES.txt
 src/HapNe.egg-info/dependency_links.txt
 src/HapNe.egg-info/requires.txt
 src/HapNe.egg-info/top_level.txt
 src/hapne/__init__.py
 src/hapne/fit.py
 src/hapne/ibd.py
 src/hapne/ld.py
+src/hapne/output.py
 src/hapne/utils.py
+src/hapne.egg-info/PKG-INFO
+src/hapne.egg-info/SOURCES.txt
+src/hapne.egg-info/dependency_links.txt
+src/hapne.egg-info/requires.txt
+src/hapne.egg-info/top_level.txt
 src/hapne/backend/DemographicHistory.py
 src/hapne/backend/DemographicHistory2StatsModelAdapter.py
 src/hapne/backend/HapNe.py
 src/hapne/backend/IO.py
 src/hapne/backend/StatsModel.py
 src/hapne/backend/__init__.py
 src/hapne/convert/__init__.py
 src/hapne/convert/tools.py
 src/hapne/convert/mathii_scripts/__init__.py
 src/hapne/convert/mathii_scripts/py3Eigenstrat.py
-src/hapne/files/regions.txt
+src/hapne/files/regions_grch37.txt
+src/hapne/files/regions_grch38.txt
+tests/test_build_hist.py
+tests/test_compute_ld.py
+tests/test_eigenstrat2vcf.py
+tests/test_hapne.py
+tests/test_time_het.py
+tests/test_vcf2splitbed.py
```

### Comparing `HapNe-1.20220920/src/hapne/backend/DemographicHistory.py` & `hapne-1.20230724/src/hapne/backend/DemographicHistory.py`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/src/hapne/backend/DemographicHistory2StatsModelAdapter.py` & `hapne-1.20230724/src/hapne/backend/DemographicHistory2StatsModelAdapter.py`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/src/hapne/backend/HapNe.py` & `hapne-1.20230724/src/hapne/backend/HapNe.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import numpy as np
 from scipy.optimize import minimize
 from numpy import log, exp
 import scipy
 import os
 import pandas as pd
 from hapne.utils import smoothing, LogBijection
+from hapne.output import plot_results
 import logging
+from tqdm import tqdm
+from pathlib import PurePath
+import matplotlib.pyplot as plt
+from scipy.stats import norm
 
 
 class HapNe:
     def __init__(self, config: ConfigParser):
         """
         Class HapNe allows to fit a demographic history based on summary statistics
         :param config: see example config file
@@ -25,25 +30,30 @@
         if verbose:
             logging.basicConfig(level=logging.INFO)
         # Method specific instances
         self.io = self.get_loader()
         self.stats_model = self.get_stats_model()
 
         # Parameter related to the model
-        self.parameter_grid = np.array([10.**(-5 + ii) for ii in range(0, 7)])
+        nb_points = 7 if self.method == "ld" else 8
+        start = -5 if self.method == "ld" else -6
+        self.parameter_grid = np.array([10.**(start + ii) for ii in range(0, nb_points)])
         self.u_min = self.get_default_u_min()  # Minimum value of u
         self.u_quantile = self.config.getfloat("CONFIG", "u_quantile", fallback=self.u_min)
         self.dt_min = max(0.25, self.config.getint("CONFIG", "dt_min", fallback=1))
         self.dt_max = self.config.getint("CONFIG", "dt_max", fallback=5000)
         self.t_max = self.config.getint("CONFIG", "t_max", fallback=125)
         self.buffer_time = self.t_max - 25  # the times averages the deep time effect
         # Parameters related to the fitting procedure
-        # this value can be tuned (tested between 2 and 24) to increase/reduce resolution
+        self.mode = self.config.get("CONFIG", "mode", fallback="regularised")
         pseudo_diploid = self.config.getboolean("CONFIG", "pseudo_diploid", fallback=False)
-        default_params = 16 if pseudo_diploid else 21
+        if self.mode == "regularised":
+            default_params = 16 if pseudo_diploid else 21
+        else:
+            default_params = 50
         self.nb_parameters = self.config.getint("CONFIG", "nb_parameters", fallback=default_params)
         self.random_restarts = 3
         self.eps = 1e-4
         self.ftol = 1e-3
         self.n_min = 1e2
         self.n_max = 1e9
         self.signal_threshold = 6.635 if self.config['CONFIG']['METHOD'] == "ld" else 9.210
@@ -105,27 +115,88 @@
         def local_loss(ne):
             n = np.ones(self.nb_parameters) * ne
             return self.sse(n)
         res = minimize(lambda x: local_loss(self.x2n(x)), np.log(10_000))
         return self.x2n(res.x)[0]
 
     def fit(self):
+        if self.mode == "regularised":
+            ne_boot = self.fit_regularized()
+        elif self.mode == "fixed":
+            ne_boot = self.fit_fixed()
+        elif self.mode == "mcmc":
+            raise NotImplementedError("MCMC mode is not implemented yet")
+            self.fit_mcmc()
+        else:
+            raise Exception("not implemented error", "mode must either be regularised, fixed or mcmc")
+        self.save_results(ne_boot)
+
+    def fit_fixed(self):
+        self.initialize_fixed_prior_procedure()
+        logging.info("Starting the fitting procedure")
+        output_folder = self.get_output_folder()
+        for _ in tqdm(range(self.nb_bootstraps)):
+            mu_boot, indices = self.io.bootstrap(return_indices=True)
+            self.stats_model.set_dataset(indices)
+            theta_hat = self.optimize_theta(mu_boot, self.sig2)
+            n_hat = self.x2n(theta_hat)
+            demohist = self.n2demohist(n_hat)
+            n_hat = demohist.n.ravel()
+            # append n_hat to results file
+            with open(output_folder / "hapne.boot", "a") as f:
+                f.write(",".join([f"{x:.0f}" for x in n_hat]) + "\n")
+        self.stats_model.set_dataset(np.arange(self.io.nb_regions()))
+        logging.info("Fitting procedure finished")
+        return pd.read_csv(output_folder / "hapne.boot", sep=",", header=None).values
+
+    def initialize_fixed_prior_procedure(self):
+        yearly_rate_growth = self.config.getfloat("CONFIG", "yearly_rate_growth", fallback=0.001)
+        logging.info(f"Fitting with a fixed prior (std of growth rate assumed to be {yearly_rate_growth})")
+        self.sig2 = ((1 + yearly_rate_growth) ** 29 - 1)**2
+        self.times = np.linspace(0, self.t_max, self.nb_parameters)
+        self.buffer_time = self.t_max - 25
+
+    def optimize_theta(self, mu, sig2):
+        self.times = np.linspace(0, self.t_max, self.nb_parameters)
+        theta_0_mean = np.random.normal(np.log(10000), 1, self.nb_parameters)
+        theta_0 = np.random.normal(theta_0_mean, 1, self.nb_parameters)
+        res = scipy.optimize.minimize(lambda theta: -self.log_p(theta, mu, sig2),
+                                      theta_0, method="L-BFGS-B", options={"ftol": 1e-4}
+                                      )
+        n_hat = self.x2n(res.x)
+        demohist = self.n2demohist(n_hat)
+        n_hat = demohist.n.ravel()
+        return res.x
+
+    def log_p(self, theta, mu, sig2):
+        n = self.x2n(theta)
+        pred = self.predict(n)
+        log_likelihood = self.stats_model.log_likelihood(mu, pred)
+        dt = np.diff(self.times)
+        pop_ratio = (1 - np.exp(np.abs(np.diff(theta)) / dt))
+        return log_likelihood - np.sum(dt * pop_ratio**2 / 2 / sig2)
+
+    def fit_regularized(self):
         """
         Perform HapNe fitting procedure and save the results.
         """
         # Step 1 : calibrate times and get MAP Ne and best regularisation
         logging.info("Starting the calibration step...")
         ne_hat, sig2 = self.calibrate_method()
         logging.info(f"Calibration step done, {sig2:.5f} selected!")
+        if sig2 < self.parameter_grid[2]:
+            sig2message = "The evidence for fluctuation is weak, the results may be unreliable (looking too constant)"
+            logging.warning(sig2message)
+            self.io.summary_message += "\n" + sig2message + "\n"
         # Step 2 : bootstrap results
         logging.info("Starting the bootstrapping procedure...")
         ne_bootstrap = self.bootstrap(ne_hat, sig2)
         # Step 3 : save results
         logging.info("Saving results...")
-        self.save_results(ne_bootstrap)
+        return ne_bootstrap
 
     def calibrate_method(self):
         """
         Find the best regularisation parameter and time intervals
         """
         nb_iterations = 5
         # Save the results of each iterations
@@ -276,53 +347,99 @@
 
     def predict(self, n):
         demo_hist = self.n2demohist(n, return_coefs=False)
         if self.io.time_heterogeneity is None:
             return self.stats_model.predict(self.io.bins, demo_hist)
         else:
             predictions = np.zeros((1, len(self.io.bins) - 1))
-            for t in np.arange(self.io.time_heterogeneity.t_end):
-                demo_hist_truncated = DemographicHistory2StatsModelAdapter(demo_hist.time[t:-1] - demo_hist.time[t],
-                                                                           demo_hist.n[t:])
-                predictions += self.io.time_heterogeneity.t_max_density[t] \
-                    * self.io.time_heterogeneity.offset_correction[t].reshape((1, -1)) \
-                    * self.stats_model.predict(self.io.bins, demo_hist_truncated).reshape((1, -1))
+            # Define the points at which to evaluate the function for Simpson integration
+            u_border = self.io.bins.reshape([1, -1])
+            u_center = (u_border[:, 1:] + u_border[:, :-1]) / 2
+
+            for ii, tau in enumerate(self.io.time_heterogeneity.taus.astype(int)):
+                demo_hist_truncated = DemographicHistory2StatsModelAdapter(demo_hist.time[tau:-1] - demo_hist.time[tau],
+                                                                           demo_hist.n[tau:])
+                prediction_at_border = self.stats_model._predict_integrand(u_border, demo_hist_truncated) * \
+                    self.io.time_heterogeneity.offset_correction_at_border[ii].reshape((1, -1))
+
+                prediction_at_center = self.stats_model._predict_integrand(u_center, demo_hist_truncated) * \
+                    self.io.time_heterogeneity.offset_correction_at_center[ii].reshape((1, -1))
+
+                predictions_for_tau = 1. / 6 * (1 * prediction_at_border[:, 1:] +
+                                                4 * prediction_at_center +
+                                                1 * prediction_at_border[:, :-1]
+                                                )
+                predictions += self.io.time_heterogeneity.tau_density[ii] \
+                    * predictions_for_tau.reshape((1, -1))
             return predictions.ravel()
 
     def bootstrap(self, ne_ini, sig2):
         """
         Sample chromosome arms with replacements to get an approximate CI for Ne
         """
         ne_boot = np.zeros((self.nb_bootstraps, self.t_max - 1), dtype=int)
-        update_times = self.config.getboolean("CONFIG", "bootstrap_time_update", fallback=False)
-        for ii in range(self.nb_bootstraps):
+        update_times = self.config.getboolean("CONFIG", "bootstrap_time_update", fallback=True)
+        for ii in tqdm(range(self.nb_bootstraps)):
             mu_boot, indices = self.io.bootstrap(return_indices=True)
             self.stats_model.set_dataset(indices)
             sig2_boot = sig2 * 10.**np.random.uniform(0, 1)
             ne_hat, _ = self.argmin_loss(ne_ini, sig2_boot, mu_boot)
             ne_boot[ii, :] = self.n2demohist(ne_hat).n.ravel()[:self.t_max - 1]
             if update_times:
                 self.update_times(ne_hat)
 
         self.stats_model.set_dataset(np.arange(self.io.nb_regions()))
         return ne_boot
 
     def save_results(self, n_boot: np.ndarray):
-        output_folder = self.config["CONFIG"]["output_folder"] + "/HapNe"
-        if not os.path.isdir(output_folder):
-            os.mkdir(output_folder)
+        output_folder = self.get_output_folder()
+        self.save_hapne(n_boot, output_folder)
+        self.plot_goodness_of_fit(np.median(n_boot, axis=0), output_folder)
+        with open(output_folder / "config.ini", "w") as f:
+            self.config.write(f)
+        with open(output_folder / "summary_mesages.txt", "w") as f:
+            f.write(self.io.summary_message)
 
+    def save_hapne(self, n_boot, output_folder):
         n_quantiles = np.quantile(n_boot, [0.025, 0.25, 0.5, 0.75, 0.975], axis=0).T
         times = np.arange(1, 1 + n_boot.shape[1]).reshape(-1, 1)
         to_save = np.concatenate([times, n_quantiles], axis=1).astype(int)
         df = pd.DataFrame(data=to_save, columns=["TIME", "Q0.025", "Q0.25", "Q0.5", "Q0.75", "Q0.975"])
         transformer = LogBijection()
         w = 20
         for key in ['Q0.025', 'Q0.25', 'Q0.5', 'Q0.75', 'Q0.975']:
             df[key] = smoothing(df[key], transformer, w)
         df = df.astype(int)
-
-        df.head(self.buffer_time).to_csv(f"{output_folder}/hapne.csv", index=False)
+        df.head(self.buffer_time).to_csv(output_folder / "hapne.csv", index=False)
 
         save_boot = self.config["CONFIG"].getboolean("save_bootstraps", fallback=False)
         if save_boot:
-            np.savetxt(f"{output_folder}/hapne.boot", n_boot)
+            np.savetxt(output_folder / "hapne.boot", n_boot)
+        plot_results(self.config, save_results=True)
+
+    def plot_goodness_of_fit(self, n, output_folder):
+        self.times = np.arange(len(n))
+        mu_hat = self.predict(n)
+        mu = self.io.mu
+        deviance_residuals = self.stats_model.residuals(mu, mu_hat)
+        fig, axs = plt.subplots(1, 2, figsize=(7, 2.3))
+        # plot the deviance residals against the quantiles of normal distribution
+        quantiles = np.linspace(0.0, 1, deviance_residuals.shape[1] + 2)[1:-1]
+        axs[0].plot(norm.ppf(quantiles), np.sort(deviance_residuals, axis=1).T, 'o--', markersize=1)
+        axs[0].set_ylabel("Deviance residuals")
+        axs[0].set_title("Normal Q-Q plot")
+        axs[1].plot(self.io.bins[:-1], mu.T, "-", color="black", alpha=0.5)
+        axs[1].plot(self.io.bins[:-1], mu_hat.T, "--", color="red", alpha=0.75)
+        axs[1].set_title("Predicted vs Observed")
+        axs[1].set_xlabel("Distance (cM)")
+        axs[1].set_ylabel("Pibd")
+        for ax in axs:
+            ax.spines.top.set_visible(False)
+            ax.spines.right.set_visible(False)
+        fig.tight_layout()
+        fig.savefig(f"{output_folder}/assessment.png", dpi=300, bbox_inches="tight")
+
+    def get_output_folder(self):
+        output_folder = PurePath(self.config.get("CONFIG", "output_folder")) / PurePath("HapNe")
+        if not os.path.isdir(output_folder):
+            os.makedirs(output_folder)
+        return output_folder
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HapNe-1.20220920/src/hapne/backend/IO.py` & `hapne-1.20230724/src/hapne/backend/IO.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, config: ConfigParser, suffix="", extension=""):
         """
         :param config: see example.ini in the repository to know which information are available in the config file
         """
         self.output_folder = str(config["CONFIG"]["output_folder"]).strip("'")
         self.config = config
 
-        self.genome_split = get_regions()
+        self.genome_split = get_regions(config.get('CONFIG', 'genome_build', fallback='grch37'))
 
         self.nb_chromosomes = self.genome_split.shape[0]  # legacy
 
         self.u_min = config['CONFIG'].getfloat('u_min', fallback=self.get_default_u_min())
         self.u_max = config['CONFIG'].getfloat('u_max', fallback=self.get_default_u_max())
 
         self.suffix = suffix
@@ -47,16 +47,19 @@
 
         default_loc = config["CONFIG"].get("output_folder")
         popname = config["CONFIG"].get("population_name")
         default_loc += f"/DATA/{popname}.age"
         self.time_heterogeneity_file = config['CONFIG'].get('age_samples', fallback=default_loc)
         if not exists(self.time_heterogeneity_file):
             self.time_heterogeneity_file = None
+        else:
+            self.time_heterogeneity_bin = config.getint("CONFIG", "age_samples_bin_width", fallback=1)
 
         self.apply_filter = config['CONFIG'].getboolean('filter_regions', fallback=True)
+        self.summary_message = ""
 
     def get_default_u_min(self):
         raise Exception("Not Implemented Error", "Data Handler should not be used directly")
 
     @property
     def mu(self):
         return self._mu[self.selected_regions, :]
@@ -136,78 +139,97 @@
         return str(self.genome_split.loc[index - 1, 'NAME']).strip()
 
 
 class LDLoader(DataHandler):
     def __init__(self, config: ConfigParser):
         super().__init__(config, suffix="_", extension="r2")
         self.ld = self.load_data('R2', apply_filter_u=False)
+        output_folder = get_ld_output_folder(config)
+        bias_filename = output_folder / f"{get_analysis_name(config)}.ccld"
         try:
-            output_folder = get_ld_output_folder(config)
-            bias_filename = output_folder + get_analysis_name(config) + ".ccld"
             data = pd.read_csv(bias_filename)
-            self.ccld = data.values[:, 2].mean()
-            self.bessel_cor = data.values[:, 4].mean()
-            _, self.pval_no_admixture = ttest_1samp(data.values[:, 2].astype(float) -
-                                                    data.values[:, 3].astype(float), 0)
+            region_1 = data.values[:, 0]
+            region_2 = data.values[:, 1]
+            # Select regions where the first 4 character do not match
+            valid_rows = np.array([region_1[i][:5] != region_2[i][:5] for i in range(len(region_1))])
+            self.ccld = data.values[valid_rows, 2].mean()
+            self.bessel_cor = data.values[valid_rows, 4].mean()
+            _, self.pval_no_admixture = ttest_1samp(data.values[valid_rows, 2].astype(float) -
+                                                    data.values[valid_rows, 3].astype(float), 0)
+            self.summary_message += f"CCLD: {self.ccld:.5f}. \n"
+            self.summary_message += f"The p-value associated with H0 = no structure is {self.pval_no_admixture:.3f}.\n"
+            logging.info(f"CCLD: {self.ccld:.5f}.")
+            logging.info(f"The p-value associated with H0 = no structure is {self.pval_no_admixture:.3f}.")
 
         except FileNotFoundError:
             logging.warning("Bias file not found, running HapNe-LD assuming no admixture LD and high coverage.")
+            logging.warning(f"Expected to read ccld file in {bias_filename}")
             self.missingness = config.getfloat("CONFIG", "missingness", fallback=0)
             n_eff = self.sample_size * (1 - self.missingness)
             self.ccld = 4 / (n_eff - 1.) ** 2
             self.bessel_cor = (n_eff / (n_eff - 1.)) ** 2
             self.pval_no_admixture = np.nan
 
         self._mu = self.ld_to_p_ibd(self.apply_filter_u(self.ld)).T
         # Combine bins if we are dealing with a small genotype or high missingness
         # self.merge_bins_if_required()
 
         # Discard suspicious Regions
-        self.filter_tolerance = config['CONFIG'].getfloat('filter_tol', fallback=6)
+        self.filter_tolerance = config['CONFIG'].getfloat('filter_tol', fallback=5e-4)
         if self.apply_filter:
             self.apply_region_filter()
         logging.info(f"Analyzing {self.mu.shape[0]} regions ")
 
         self.phi2 = np.var(self.mu, axis=0).reshape(-1)
-        self.sigma = np.diag(self.phi2)
+        self.sigma = np.cov(self.mu.T)
 
         if self.time_heterogeneity_file is not None:
             logging.info("Using time heterogeneity correction ")
-            self.time_heterogeneity = LDTimeIO(self.time_heterogeneity_file, self.bins)
+            self.time_heterogeneity = LDTimeIO(self.time_heterogeneity_file, self.bins, self.time_heterogeneity_bin)
         else:
             logging.info("No age of samples found, assuming they originate from the same generation...")
             self.time_heterogeneity = None
 
     def get_sample_size(self):
         pseudo_diploid = self.config.getboolean("CONFIG", "pseudo_diploid", fallback=None)
         if pseudo_diploid is None:
             pseudo_diploid = False
             logging.warning("[CONFIG]pseudo_diploid not found in config file, assuming diploid. \n \
                             If you are analysing aDNA, set the flag to True.")
-
-        region1 = get_region(1)
-        default_loc = self.config.get("CONFIG", "output_folder") + "/DATA/GENOTYPES"
-        genotypes_loc = self.config.get("CONFIG", "genotypes", fallback=default_loc)
-        fam_file = pd.read_csv(f"{genotypes_loc}/{region1['NAME']}.fam", header=None, sep="\t")
-        return (2 - pseudo_diploid) * fam_file.shape[0]
+        try:
+            region1 = get_region(1, self.config.get('CONFIG', 'genome_build', fallback='grch37'))
+            default_loc = self.config.get("CONFIG", "output_folder") + "/DATA/GENOTYPES"
+            genotypes_loc = self.config.get("CONFIG", "genotypes", fallback=default_loc)
+            fam_file = pd.read_csv(f"{genotypes_loc}/{region1['NAME']}.fam", header=None, sep="\t")
+            nb_individuals = fam_file.shape[0]
+        except FileNotFoundError:
+            nb_individuals = self.config.getint("CONFIG", "nb_individuals")
+        return (2 - pseudo_diploid) * nb_individuals
 
     def apply_region_filter(self):
         """
-        discard suspicious regions
+        discard regions with high LD
         :return:
         """
-        mu_med = np.median(self._mu, axis=0)
-        mu_std_up = np.quantile(self._mu, 0.16, axis=0)
-        mu_std_down = np.quantile(self._mu, 0.84, axis=0)
-        mu_std = np.abs(mu_std_down - mu_std_up) / 2.
-        mu_se = mu_std / np.sqrt(self._mu.shape[0]) * self.filter_tolerance
-        self.selected_regions = \
-            np.where((((self._mu > (mu_med - mu_se)).max(axis=1) == 1)
-                     * ((self._mu > (mu_med + mu_se)).min(axis=1) == 0))
-                     * ((np.abs(self._mu - mu_med) > self.filter_tolerance * mu_std).sum(axis=1) <= 1))[0]
+        nb_regions = self._mu.shape[0]
+        self.selected_regions = []
+        for ii in range(nb_regions):
+            jackknife = np.delete(self._mu, ii, axis=0)
+            median = np.median(jackknife, axis=0)
+            std = np.std(jackknife, axis=0, ddof=1)
+            sse = np.sum((self._mu[ii, :] - median) ** 2 / std ** 2)
+            ddof = self._mu.shape[1]
+            pval = 1 - chi2.cdf(sse, ddof)
+            if pval > self.filter_tolerance / nb_regions:
+                self.selected_regions.append(ii)
+            else:
+                logging.warning(f"Discarding region {self.get_region_name(ii + 1)} with pval {pval:.5f}")
+                self.summary_message += f"Discarding region {self.get_region_name(ii + 1)} with pval {pval:.5f}.\n"
+
+        self.selected_regions = np.array(self.selected_regions)
 
     def read_bins(self):
         region = self.get_region_name(1)
         bins = pd.read_csv(f"{self.input_files_location()}/{region}.{self.extension}",
                            sep=",").values[:, 1:3].T
         return bins
 
@@ -355,84 +377,124 @@
 
         def get_jackknife_r2(data, indices, index):
             res = get_jackknife_residuals(data, indices, index)
             return np.sum(res ** 2)
 
         discarded = []
         n_bins = len(self.bins) - 1
-        for iteration in range(2):
+        for _ in range(2):
             current_ibd = np.delete(self._mu, discarded, axis=0)
             indices = np.delete(np.arange(self.nb_regions()), discarded)
 
             for ii in range(len(indices)):
                 sse = get_jackknife_r2(current_ibd, indices, ii)
                 if min(chi2.cdf(sse, n_bins), 1 - chi2.cdf(sse, n_bins)) < 1e-12:
                     discarded.append(indices[ii])
 
         self.selected_regions = np.delete(self.selected_regions, discarded)
 
 
 class LDTimeIO:
-    def __init__(self, timefile, u=np.zeros(1)):
+    def __init__(self, timefile, u=np.zeros(1), bin_width=1):
         """
         Precompute
         :param timefile: file containing the age of the samples.
         :param u : time at which we compute the time offsets
+        :bin_width : Length of bins to compute the correction (the higher the faster)
         """
         u = u.reshape((1, -1))
 
-        self.times = pd.read_csv(timefile, sep=",")
-        self.times.columns = self.times.columns.str.replace(' ', '')
-        self.t_start = np.min(self.times["FROM"].values)
-        self.times -= self.t_start
-        self.t_end = np.max(self.times["TO"].values) + 1
-
-        self.age_density = self._compute_age_density()
-        self.t_max_density = self._compute_tmax_density()
-        # dt_density[ii, :] = P(Delta_t | tmax == ii)
-        self.dt_density = self._compute_dt_density()
-        # offset_correction[tmax, u] = E[exp(-dt u)|tmax]
-        self.offset_correction = self._compute_offset_correction(u)
+        self.samples_age_in_gen = pd.read_csv(timefile, sep=",")
+        self.samples_age_in_gen.columns = self.samples_age_in_gen.columns.str.replace(' ', '')
 
-    def _compute_age_density(self):
+        self.most_recent = np.min(self.samples_age_in_gen["FROM"].values)
+        self.oldest = np.max(self.samples_age_in_gen["TO"].values)
+        logging.info("Reading the age of the samples")
+        logging.info(f"Most recent sample: {self.most_recent} gen. bp")
+        logging.info(f"Oldest sample: {self.oldest} gen. bp")
+
+        try:
+            assert self.oldest - self.most_recent > bin_width
+        except AssertionError:
+            logging.warning("The bin_width is too large for the data, using the smallest bin_width possible")
+            bin_width = self.oldest - self.most_recent
+
+        self.bins = np.arange(self.most_recent, self.oldest + bin_width + 1, bin_width)
+        self.bin_width = bin_width
+        self.middle_bins = self.bins[:-1] + bin_width / 2
+        logging.info(f"HapNe will start predicting Ne from t={self.middle_bins[0]} gen bp")
+        self.bins -= self.most_recent
+        self.middle_bins -= self.most_recent
+
+        self.age_density_in_bin = self._compute_age_density_in_bin()
+
+        self.tau_density, self.dt_density = self._compute_pairwise_density()
+
+        self.delta_ts = np.array([ii * bin_width for ii in range(len(self.middle_bins))])
+        self.taus = self.middle_bins - self.middle_bins[0]
+
+        self.offset_correction_at_border = self._compute_offset_correction(u)
+        u_center = 0.5 * (u[0, 1:] + u[0, :-1]).reshape((1, -1))
+        self.offset_correction_at_center = self._compute_offset_correction(u_center)
+
+    def _compute_age_density_in_bin(self):
         """
         Convert a list of times at which individuals lived into the density of age of a ramdomly sampled individual
         :return:
         """
-        times = self.times.values
-        list_time = np.arange(self.t_end)
         # One row per samples. 1 when they are alive
-        samples_alive = np.zeros((times.shape[0], self.t_end))
-        for ii in range(times.shape[0]):
-            samples_alive[ii, :] = (list_time >= times[ii, 0]) * (list_time <= times[ii, 1])
-        return samples_alive.sum(axis=0) / samples_alive.sum()
-
-    def _compute_tmax_density(self):
-        tmax_cumulative = np.cumsum(self.age_density) ** 2
-        tmax_density = np.zeros_like(tmax_cumulative)
-        tmax_density[0] = tmax_cumulative[0]
-        tmax_density[1:] = np.diff(tmax_cumulative)
-        return tmax_density
-
-    def _compute_dt_density(self):
-        dt_density = np.zeros(shape=(self.t_end, self.t_end))
-        for ii in range(self.t_end):
-            dt_density[ii, :ii + 1] = np.flip(self.age_density[:ii + 1]) / np.sum(self.age_density[:ii + 1])
-        return dt_density
+        nb_samples = self.samples_age_in_gen.shape[0]
+        age_density = self._compute_age_density()
+        age_density_in_bin = np.zeros((nb_samples, len(self.middle_bins)))
+        for ii in range(nb_samples):
+            for jj in range(len(self.middle_bins)):
+                age_density_in_bin[ii, jj] = np.sum(age_density[ii, jj * self.bin_width:(jj + 1) * self.bin_width])
+        age_density_in_bin = age_density_in_bin / age_density_in_bin.sum(axis=1, keepdims=True)
+        return age_density_in_bin
+
+    def _compute_age_density(self):
+        t_low = self.samples_age_in_gen["FROM"].values - self.most_recent
+        t_high = self.samples_age_in_gen["TO"].values - self.most_recent
+        nb_gen = self.oldest - self.most_recent + 1
+        age_density = np.zeros((len(t_low) * 2, nb_gen))
+        for ii in range(len(t_low)):
+            age_density[2 * ii, t_low[ii]:t_high[ii] + 1] = 1
+            age_density[2 * ii + 1, t_low[ii]:t_high[ii] + 1] = 1
+        age_density = age_density / age_density.sum(axis=1, keepdims=True)
+        return age_density
+
+    def _compute_pairwise_density(self):
+        nb_bins = len(self.middle_bins)
+        s = self.samples_age_in_gen["FROM"].values.shape[0]
+        delta_t_density_binned = np.zeros((nb_bins, nb_bins))
+        n_terms = s * (s - 1)
+        for tau in range(nb_bins):
+            delta_t_density_binned[tau, 0] = 1 / n_terms * \
+                cross_terms(self.age_density_in_bin[:, tau], self.age_density_in_bin[:, tau])
+            for jj in range(0, tau):
+                delta_t_density_binned[tau, tau - jj] = 1 / n_terms * \
+                    2 * cross_terms(self.age_density_in_bin[:, tau], self.age_density_in_bin[:, jj])
+
+        tau_density_binned = np.sum(delta_t_density_binned, axis=1)
+        delta_t_density_binned = delta_t_density_binned / tau_density_binned[:, None]
+        return tau_density_binned, delta_t_density_binned
 
     def _compute_offset_correction(self, u):
-        list_times = np.arange(self.t_end).reshape((-1, 1))
+        delta_ts = self.delta_ts.reshape((-1, 1))
         u = u.reshape((1, -1))
-        exponential_decays = 1. / 6 * (1 * np.exp(-list_times * u[0, 1:].reshape((1, -1))) +
-                                       4 * np.exp(-list_times * u[0, :-1].reshape((1, -1))) +
-                                       1 * np.exp(-list_times * 0.5 * (u[0, 1:] + u[0, :-1]))
-                                       )
-        offset = np.zeros((self.t_end, u.shape[1] - 1))
-        for ii in range(self.t_end):
+        exponential_decays = np.exp(- (delta_ts - 0.75) * u)
+
+        offset = np.zeros((len(self.taus), u.shape[1]))
+        for ii in range(len(self.taus)):
             offset[ii, :] = (self.dt_density[ii].reshape((-1, 1)) * exponential_decays).sum(axis=0)
         return offset
 
 
 def compute_poisson_mean(data, region_length):
     p = data.sum(axis=0) / region_length.sum()
     mu = p.reshape((1, -1)) * region_length.reshape(-1, 1)
     return mu
+
+
+def cross_terms(f, g):
+    return 0.5 * (np.sum(f + g, axis=0) ** 2 -
+                  np.sum(f, axis=0) ** 2 - np.sum(g, axis=0) ** 2 - 2 * np.sum(f * g, axis=0))
```

### Comparing `HapNe-1.20220920/src/hapne/backend/StatsModel.py` & `hapne-1.20230724/src/hapne/backend/StatsModel.py`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/src/hapne/convert/mathii_scripts/py3Eigenstrat.py` & `hapne-1.20230724/src/hapne/convert/mathii_scripts/py3Eigenstrat.py`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/src/hapne/convert/tools.py` & `hapne-1.20230724/src/hapne/convert/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,28 +34,27 @@
         for ii, d in enumerate(data):
             this_snp = data.snp[ii]
             line = "\t".join([this_snp["CHR"], str(this_snp["POS"]), this_snp["ID"],
                               this_snp["REF"], this_snp["ALT"], "100", "PASS", ".", "GT"])
             line = line + "\t" + "\t".join([conversion[x] for x in d])
             f.write("\n" + line)
     command = f"plink --vcf {vcf_file} \
-        --recode vcf \
+        --export vcf \
         --const-fid \
         --out {get_vcf_location(config)}_tmp \
-        --threads 1 \
         --mind 0.8 \
         --geno 0.8 "
     os.system(command)
     # execute the gzip command to compress the file
     os.system(f"mv {get_vcf_location(config)}_tmp.vcf {vcf_file}")
     os.system("gzip " + vcf_file)
 
     # create the map from the .snp file
     save_maps_in = config.get("CONFIG", "output_folder") + "/DATA"
-    for _, region in get_regions().iterrows():
+    for _, region in get_regions(config.get('CONFIG', 'genome_build', fallback='grch37')).iterrows():
         chr = region["CHR"]
         chr_from = region["FROM_BP"]
         chr_to = region["TO_BP"]
 
         bim = pd.read_csv(eigen_root + ".snp", header=None, delim_whitespace=True)
         bim = bim[bim[1] == chr]
         map = bim[[3, 2, 2]]
@@ -101,15 +100,15 @@
     if not (0 <= index < 39):
         raise ValueError(f"index must be between 0 and 38, but index={index}")
 
     save_in = config.get("CONFIG", "output_folder") + "/DATA/GENOTYPES"
     if not os.path.isdir(save_in):
         os.makedirs(save_in)
 
-    region = get_region(index)
+    region = get_region(index, config.get('CONFIG', 'genome_build', fallback='grch37'))
     chr = region["CHR"]
     chr_from = region["FROM_BP"]
     chr_to = region["TO_BP"]
 
     eigen_root = config.get("CONFIG", "eigen_root", fallback=None)
     keep = None
     keep_command = ""
@@ -153,15 +152,15 @@
     if not (0 <= index < 39):
         raise ValueError(f"index must be between 0 and 38, but index={index}")
 
     save_in = config.get("CONFIG", "output_folder") + "/DATA/GENOTYPES"
     if not os.path.isdir(save_in):
         os.makedirs(save_in)
 
-    region = get_region(index)
+    region = get_region(index, config.get('CONFIG', 'genome_build', fallback='grch37'))
     chr = region["CHR"]
     chr_from = region["FROM_BP"]
     chr_to = region["TO_BP"]
     keep = config.get("CONFIG", "keep", fallback=None)
     if keep is not None:
         keep_command = f"--keep {keep}"
```

### Comparing `HapNe-1.20220920/src/hapne/files/regions.txt` & `hapne-1.20230724/src/hapne/files/regions_grch37.txt`

 * *Files identical despite different names*

### Comparing `HapNe-1.20220920/src/hapne/ibd.py` & `hapne-1.20230724/src/hapne/ibd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from configparser import ConfigParser
 import os
 from hapne.utils import get_region, get_regions
 
 
 def build_hist(config: ConfigParser):
-    for ii in range(get_regions.shape[0]):
+    for ii in range(get_regions(config.get('CONFIG', 'genome_build', fallback='grch37')).shape[0]):
         build_hist_in_parallel(ii, config)
 
 
 def build_hist_in_parallel(region_index: int, config: ConfigParser):
-    region = get_region(region_index)
+    region = get_region(region_index, config.get('CONFIG', 'genome_build', fallback='grch37'))
     name = region["NAME"]
 
     ibd_folder = config.get("CONFIG", "ibd_files")
     hist_folder = get_hist_folder(config)
     # needs for on macos instead of zcat *
     command = f"for IBDFILE in `ls {ibd_folder}/{name}.*.ibd.gz`" \
         + "; do " \
         + "gunzip -c $IBDFILE; " \
         + "done | " \
-        + "awk -F\"\\t|_\" '{l=sprintf(\"%d\", 2*$12); c[l]++;} END{ for (i=1; i<=40; i++) " \
+        + "awk -F\"\\t\" '{l=sprintf(\"%d\", 2*$10); c[l]++;} END{ for (i=1; i<=40; i++) " \
         + "print i/2/100 \"\\t\" (i+1)/2/100 \"\\t\" 0+c[i]; }'" \
         + f"> {hist_folder}/{name}.ibd.hist"
     os.system(command)
 
 
 def get_hist_folder(config: ConfigParser):
     output_folder = config.get("CONFIG", "output_folder") + "/IBD"
     if not os.path.isdir(output_folder):
-        os.mkdir(output_folder)
+        os.makedirs(output_folder)
     return output_folder
```

### Comparing `HapNe-1.20220920/src/hapne/ld.py` & `hapne-1.20230724/src/hapne/ld.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from numpy import sqrt
 from numba import njit
 import pandas_plink as pdp
 import pandas as pd
 import os
 import logging
+from pathlib import PurePath
 
 
 def get_analysis_name(config: ConfigParser):
     name = config.get("CONFIG", "population_name", fallback=None)
     if name is None:
         name = "hapne"
     return name
@@ -19,58 +20,88 @@
 def get_genotypes_location(config: ConfigParser):
     output_folder = config["CONFIG"].get("output_folder")
     default = output_folder + "/DATA/GENOTYPES"
     return config["CONFIG"].get("genotypes", fallback=default)
 
 
 def compute_ld(config: ConfigParser):
-    nb_regions = get_regions().shape[0]
+    nb_regions = get_regions(config.get('CONFIG', 'genome_build', fallback='grch37')).shape[0]
     for ii in range(nb_regions):
         compute_ld_in_parallel(ii, config)
 
 
+def compute_manhattan_ld(config: ConfigParser):
+    nb_regions = get_regions(config.get('CONFIG', 'genome_build', fallback='grch37')).shape[0]
+    for ii in range(nb_regions):
+        compute_manhattan_ld_in_parallel(ii, config)
+
+
 def compute_ccld(config: ConfigParser):
-    nb_regions = get_regions().shape[0]
+    nb_regions = get_regions(config.get('CONFIG', 'genome_build', fallback='grch37')).shape[0]
     nb_pairs = nb_regions * (nb_regions - 1) // 2
     create_cc_file(config)
     for ii in range(nb_pairs):
         compute_cc_quantities_in_parallel(ii, config)
 
 
 def compute_ld_in_parallel(region_index: int, config: ConfigParser):
     """ Compute the (biased) LD for a given region and save the results in a config['output']/region.r2 file.
     :param config : see readme for an example
     :param region : index of the region
     :param save_hist: if True, also save a .ld file, which can be use to filter out problematic regions or SNPs
     """
-    region = get_region(region_index)
+    region = get_region(region_index, config.get('CONFIG', 'genome_build', fallback='grch37'))
     maf = config.getfloat("CONFIG", "maf", fallback=0.25)
     genotype_folder = get_genotypes_location(config)
     genotype, chr_map = load_and_preprocess_file(genotype_folder + "/" + region["NAME"] + ".bed",
                                                  maf)
-
+    average_missing_prop = np.mean(np.isnan(genotype))
+    sample_size = genotype.shape[0] * (2 - config.getboolean("CONFIG", "pseudo_diploid", fallback=False))
+    if sample_size * (1 - average_missing_prop)**2 < 6:
+        raise ValueError(f"Region {region['NAME']} has too many missing values or too few individuals.")
+    else:
+        logging.info(f"Computing LD for region {region['NAME']}...")
     bins = get_bins()
 
     ld, weights = _compute_r2(genotype, chr_map, bins)
     save_ld_results(config, region["NAME"], ld, weights, bins)
 
 
+def compute_manhattan_ld_in_parallel(region_index: int, config: ConfigParser):
+    """ Compute the (biased) LD for a given region and save the results in a config['output']/region.r2 file.
+    :param config : see readme for an example
+    :param region : index of the region
+    :param save_hist: if True, also save a .ld file, which can be use to filter out problematic regions or SNPs
+    """
+    region = get_region(region_index, config.get('CONFIG', 'genome_build', fallback='grch37'))
+    maf = config.getfloat("CONFIG", "maf", fallback=0.25)
+    genotype_folder = get_genotypes_location(config)
+
+    bed_filename = genotype_folder + "/" + region["NAME"] + ".bed"
+    genotype, chr_map = load_and_preprocess_file(bed_filename, maf)
+
+    bins = get_bins()
+
+    r2_towers = _compute_manhattan_r2(genotype, chr_map, bins)
+    save_manhattan_ld_results(config, region["NAME"], r2_towers, bed_filename)
+
+
 def create_cc_file(config: ConfigParser):
     output_folder = get_ld_output_folder(config)
-    output_file = output_folder + get_analysis_name(config) + ".ccld"
+    output_file = output_folder / f"{get_analysis_name(config)}.ccld"
     with open(output_file, "w") as f:
         f.write("REGION1, REGION2, CCLD, CCLD_H0, BESSEL_FACTOR, S_CORR\n")
 
 
 def compute_cc_quantities_in_parallel(job_index: int, config: ConfigParser, nb_points=int(1e6)):
     """ Compute the (biased) bias computed from the two regions provided as parameter.
     :param config : see preprocess_ld.config for an example
     :param nb_points : number of points to consider when computing the cross-chromosome bias
     """
-    reg1, reg2 = get_regions_from_index(job_index)
+    reg1, reg2 = get_regions_from_index(job_index, config.get('CONFIG', 'genome_build', fallback='grch37'))
     maf = config.getfloat("CONFIG", "maf", fallback=0.25)
 
     try:
         pseudo_diploid = config.getboolean("CONFIG", "pseudo_diploid")
     except NoOptionError:
         pseudo_diploid = config.getboolean("CONFIG", "pseudo_diploid", fallback=False)
         logging.warning("[CONFIG]pseudo_diploid not found in config file, assuming diploid. \n \
@@ -79,15 +110,15 @@
     genotype1, _ = load_and_preprocess_file(folder + "/" + reg1 + ".bed", maf)
     genotype2, _ = load_and_preprocess_file(folder + "/" + reg2 + ".bed", maf)
 
     ccld, expected_ccld, bessel_factor, s_corr = _compute_cc_quantities(genotype1, genotype2,
                                                                         int(nb_points), pseudo_diploid)
 
     output_folder = get_ld_output_folder(config)
-    output_file = output_folder + get_analysis_name(config) + ".ccld"
+    output_file = output_folder / f"{get_analysis_name(config)}.ccld"
     with open(output_file, "a") as f:
         f.write(f"{reg1},{reg2},{ccld},{expected_ccld},{bessel_factor},{s_corr}\n")
 
 
 @njit(cache=True)
 def _compute_r2(genotype: np.ndarray, gen_map, bins: np.ndarray):
     """ For a given genotype, compute LD within the bins
@@ -117,29 +148,65 @@
                     r2_in_bin[bb] = (current_mean * weight_in_bin[bb] + observation * weight) \
                         / (weight_in_bin[bb] + weight)
                     weight_in_bin[bb] += weight
             index_y += 1
     return r2_in_bin, weight_in_bin
 
 
+@njit(cache=True)
+def _compute_manhattan_r2(genotype: np.ndarray, gen_map, bins: np.ndarray):
+    """ For a given genotype, compute the LD for each SNP within each bin
+    :param genotype: (nb ind x nb snps) unphased genotype
+    :param gen_map: distance between sites
+    :param bins: nb_bins x 2 corresponding to the start and the end of each bin, respectively
+    :return: r2 in each bin, r2 for each snp and bin, weights for each bin
+    """
+    nb_bins = bins.shape[0]
+    nb_snps = genotype.shape[1]
+
+    r2_for_snp_in_bin = np.zeros(shape=(nb_bins, nb_snps))
+    weight_in_bin = np.zeros_like(r2_for_snp_in_bin)
+
+    # Loop over all pairs of columns
+    for index_x in range(genotype.shape[1] - 2):
+        index_y = index_x + 1
+        delta_xy = genetic_distance(index_x, index_y, gen_map)
+        while delta_xy < np.max(bins[:, 1]) and index_y < np.shape(genotype)[1]:
+            delta_xy = genetic_distance(index_x, index_y, gen_map)
+            bb = get_bin_index(delta_xy, bins)
+            if bb is not None:
+                bb = int(bb)
+                valid_snps_x, valid_snps_y, weight = get_valid_xy(genotype[:, index_x],
+                                                                  genotype[:, index_y])
+                if weight > 0 and valid_snps_x.shape[0] > 1:
+                    observation = two_snp_correlation(valid_snps_x, valid_snps_y)
+                    for ii in [index_x, index_y]:
+                        current_mean = r2_for_snp_in_bin[bb, ii]
+                        r2_for_snp_in_bin[bb, ii] = (current_mean * weight_in_bin[bb, ii] + observation * weight) \
+                            / (weight_in_bin[bb, ii] + weight)
+                        weight_in_bin[bb, ii] += weight
+            index_y += 1
+    return r2_for_snp_in_bin
+
+
 def load_and_preprocess_file(bed_file: str, maf=0.25):
     """
     Load the bed file and apply the normalisation procedure.
     Variants under the maf threshold will be set to np.nan
     :param bed_file : path to the bed file, including the .bed
     :param maf : minor allele frequency threshold
     :return genotype and chromosome_map
     """
     genotype, chr_map = load_files(bed_file)
     genotype = preprocess_genotype(genotype, maf_filter=maf)
     return genotype, chr_map
 
 
-def get_regions_from_index(job_index: int):
-    region_list = get_regions().values[:, 3]
+def get_regions_from_index(job_index: int, build: str):
+    region_list = get_regions(build).values[:, 3]
     n = len(region_list)
     k = job_index
 
     # job_index corresponds to regions i and j
     # basically, this will map k to {(0, 1), (0, 2)... (1, 2), (1, 3) .. (37,38)}
     i = int(n - 2 - int(sqrt(-8 * k + 4 * n * (n - 1) - 7) / 2.0 - 0.5))
     j = int(k + i + 1 - n * (n - 1) / 2 + (n - i) * ((n - i) - 1) / 2)
@@ -169,24 +236,25 @@
 
     # Loop over all pairs of columns
     for _ in range(nb_points):
         index1 = np.random.randint(0, gen1.shape[1])
         index2 = np.random.randint(0, gen2.shape[1])
         valid_snps_x, valid_snps_y, weight = get_valid_xy(gen1[:, index1],
                                                           gen2[:, index2])
-        if weight > 0 and valid_snps_x.shape[0] > 1:
+        if weight > 0 and valid_snps_x.shape[0] > 2:
             # CCLD
             observation = two_snp_correlation(valid_snps_x, valid_snps_y)
             ccld += observation * weight
             # Expected CCLD (if no admixture is present)
             nx = np.sum(~np.isnan(gen1[:, index1])) * sample_size_factor
             ny = np.sum(~np.isnan(gen2[:, index2])) * sample_size_factor
             expected_ccld += 4. / (nx - 1) * 1. / (ny - 1) * weight
-            # Bessel correction factor
-            bessel_factor += nx / (nx - 1.) * ny / (ny - 1.) * weight
+            # "Bessel" correction factor (assuming IBD is present)
+            bessel_factor += ((nx ** 2 - nx + 2) / (nx ** 2 - 3 * nx + 2) *
+                              (ny ** 2 - ny + 2) / (ny ** 2 - 3 * ny + 2)) * weight
             # E[Gx2Gy2] - 1 for pseudo-diploid data
             s_corr += (np.mean((valid_snps_x * valid_snps_y * sample_size_factor)**2) / 4. - 1) * weight
             # Updating the weight
             total_weight += weight
     return ccld / total_weight, expected_ccld / total_weight, bessel_factor / total_weight, s_corr / total_weight
 
 
@@ -223,30 +291,37 @@
     :param genotype: (nb ind x nb snps)
     :param maf_filter: consider snp whose frequency satisfies |f-0.5|<maf_filter
     :return: (nb ind x nb snps) with  variance and 0 mean, nan for missing values
     """
     gen = genotype.copy()
 
     freq = np.nanmean(genotype, axis=0) / 2.
+    maf = np.minimum(freq, 1 - freq)
     # Apply MAF criteria ( must not be further away from 0.5 than the MAF )
-    gen[:, np.abs(freq - 0.5) > np.abs(maf_filter - 0.5)] = np.nan
+    gen[:, maf < maf_filter] = np.nan
     # normalise
     gen -= freq * 2
     gen /= np.sqrt(freq * (1 - freq) * 2)
 
     return gen
 
 
-def load_files(prefix):
+def load_files(prefix, maf=0.25, return_pos=False):
     """ Load binary plink files
     :param prefix: prefix of the files (prefix.bed, bim, fam must exist)
     :return : genotype (bed file), map (location of each SNP in Morgan)
     """
     genotype_object = pdp.read_plink1_bin(prefix)
-    return genotype_object.values, genotype_object.cm.values / 100.
+    freq = np.nanmean(genotype_object.values, axis=0) / 2.
+    freq = np.minimum(freq, 1 - freq)
+    if return_pos:
+        return genotype_object.values[:, freq >= maf],\
+            genotype_object.cm.values[freq >= maf] / 100.,\
+            genotype_object.pos.values[freq >= maf]
+    return genotype_object.values[:, freq >= maf], genotype_object.cm.values[freq >= maf] / 100.
 
 
 @njit(cache=True)
 def get_valid_xy(x, y):
     """ Return the non-missing entries of xy, together with the percentage of those values if return_percentage is True
     :param x: nb_individual, normalised value of SNP x
     :param y: nb_individual, normalised value of SNP y
@@ -278,21 +353,38 @@
     :param config: see the example config file
     :param region : name of the current genetic region
     :param r2: average r2 within each bin
     :param weights: total weight for the bin
     :param bins: nb_bins x 2 ndarray (bin_from, bin_to)
     """
     output_folder = get_ld_output_folder(config)
-    save_in = output_folder + region + ".r2"
+    save_in = output_folder / f"{region}.r2"
     to_be_saved = pd.DataFrame(columns=["BIN_FROM[M]", "BIN_TO[M]", "R2", "WEIGHT"])
     to_be_saved["BIN_FROM[M]"] = bins[:, 0]
     to_be_saved["BIN_TO[M]"] = bins[:, 1]
     to_be_saved["R2"] = r2
     to_be_saved["WEIGHT"] = weights
     to_be_saved.to_csv(save_in)
 
 
+def save_manhattan_ld_results(config: ConfigParser, region: str, r2: np.ndarray, filename: str):
+    """
+    :param config: see the example config file
+    :param region : name of the current genetic region
+    :param r2: average r2 within each bin (y axis) for each snp (x axis)
+    """
+    output_folder = get_ld_output_folder(config)
+    save_in = output_folder / f"{region}.manhattan.r2"
+    np.save(save_in, r2)
+
+    save_in = output_folder / f"{region}.manhattan.snp"
+    _, cm_maps, pos = load_files(filename, return_pos=True)
+    maps = np.vstack((pos, cm_maps))
+    np.save(save_in, maps)
+
+
 def get_ld_output_folder(config: ConfigParser):
-    output_folder = config["CONFIG"]["output_folder"] + "/LD/"
+    default_output_folder = config["CONFIG"]["output_folder"] + "/LD/"
+    output_folder = PurePath(config.get("CONFIG", "ld_files", fallback=default_output_folder))
     if not os.path.isdir(output_folder):
         os.makedirs(output_folder)
     return output_folder
```

### Comparing `HapNe-1.20220920/src/hapne/utils.py` & `hapne-1.20230724/src/hapne/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pkg_resources
 import pandas as pd
 import numpy as np
 from configparser import ConfigParser
 from os.path import exists
+from os import makedirs
 
 
-def get_regions():
+def get_regions(build="grch37"):
     """
     read the regions files
     :return: pandas dataframe
     """
-    stream = pkg_resources.resource_stream("hapne", 'files/regions.txt')
+    stream = pkg_resources.resource_stream("hapne", f"files/regions_{build}.txt")
     return pd.read_csv(stream, sep="\t")
 
 
-def get_region(region_index: int):
-    regions = get_regions()
+def get_region(region_index: int, build="grch37"):
+    regions = get_regions(build)
     return regions.iloc[region_index]
 
 
 def get_bins():
     """ Provide the bins for which we want to perform the analysis part
     NEXT : Read from a file instead
     """
@@ -36,44 +37,70 @@
     HapNe's input format, so that the individuals who did not pass the
     quality test are not included in the samples.age file.
 
     If a .fam file is found, the individuals from this file will be used,
     otherwise the individuals from the .keep file will be included.
     """
     years_per_gen = 29
+    age_from_bp, age_to_bp = get_age_samples_in_bp(config)
+
+    age_from = (age_from_bp / years_per_gen).reshape((-1, 1)).astype(int)
+    age_to = (age_to_bp / years_per_gen).reshape((-1, 1)).astype(int)
+    to_save = pd.DataFrame(np.concatenate((age_from, age_to), axis=1), columns=["FROM", "TO"])
+    save_as = config["CONFIG"].get("output_folder")
+    popname = config["CONFIG"].get("population_name")
+    save_as += "/DATA"
+    # Create folder if it does not exist
+    if not exists(save_as):
+        makedirs(save_as)
+    to_save.to_csv(save_as + f"/{popname}.age", index=False)
+
+
+def get_age_samples_in_bp(config: ConfigParser):
     anno_file = pd.read_csv(config.get("CONFIG", "anno_file"), sep="\t")
 
+    col_bp_index = config.getint("CONFIG", "anno_bp_column", fallback=8)
+    col_stdbp_index = col_bp_index + 1
+
+    # Convert the `col_bp` and `col_stdbp` columns to int
+    try:
+        anno_file[anno_file.columns[col_bp_index]] = anno_file[anno_file.columns[col_bp_index]].astype(int)
+        anno_file[anno_file.columns[col_stdbp_index]] = anno_file[anno_file.columns[col_stdbp_index]].astype(int)
+    except ValueError:
+        print("Columns referring to age of samples cannot be converted to int. Please check the anno_bp_column.")
+
     individuals_in_study = get_individuals_in_study(config)
     individuals_in_study.columns = [anno_file.columns[1]]
     anno = pd.merge(individuals_in_study, anno_file, how='inner', on=[anno_file.columns[1]]).values
-    col_bp = config.getint("CONFIG", "anno_bp_column", fallback=8)
-    col_stdbp = col_bp + 1
-    age_from = ((anno[:, col_bp] - 2 * anno[:, col_stdbp]) / years_per_gen).reshape((-1, 1)).astype(int)
-    age_to = ((anno[:, col_bp] + 2 * anno[:, col_stdbp]) / years_per_gen).reshape((-1, 1)).astype(int)
-    to_save = pd.DataFrame(np.concatenate((age_from, age_to), axis=1), columns=["FROM", "TO"])
-    save_as = config["CONFIG"].get("output_folder")
-    popname = config["CONFIG"].get("population_name")
-    save_as += f"/DATA/{popname}.age"
-    to_save.to_csv(save_as, index=False)
+
+    # Clip the uncertainty value to avoid having samples from the future
+    uncertainty = np.minimum(anno[:, col_bp_index], 2 * anno[:, col_stdbp_index])
+
+    age_from = (anno[:, col_bp_index] - uncertainty).reshape((-1, 1)).astype(int)
+    age_to = (anno[:, col_bp_index] + uncertainty).reshape((-1, 1)).astype(int)
+    return age_from, age_to
 
 
 def get_individuals_in_study(config: ConfigParser):
     """
     See get_age_from_anno
     """
     output_folder = config["CONFIG"].get("output_folder")
     # Check if a .fam file is present
     genotypes = config["CONFIG"].get("genotypes", fallback=None)
     if genotypes is None:
         genotypes = f"{output_folder}/DATA/GENOTYPES"
-    fam_path = f"{genotypes}/{get_region(1)['NAME']}.fam"
+    fam_path = f"{genotypes}/{get_region(1, config.get('CONFIG', 'genome_build', fallback='grch37'))['NAME']}.fam"
     if exists(fam_path):
         fam_file = pd.read_csv(fam_path, header=None, sep=" ")
         df = pd.DataFrame(fam_file[1])
-        df = df.applymap(lambda x: '_'.join(str(x).split('_')[1:]))
+        # Sometimes, all the individuals have the family ID as prefix, which we need to remove
+        all_samples_have_family_prefix = not df.applymap(lambda x: '_' not in str(x)).any().any()
+        if all_samples_have_family_prefix:
+            df = df.applymap(lambda x: '_'.join(str(x).split('_')[1:]))
         return df
     else:
         keep_inds = pd.read_csv(config.get("CONFIG", "keep"), header=None)
         return keep_inds
 
 
 class Bijection:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

