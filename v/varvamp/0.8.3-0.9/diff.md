# Comparing `tmp/varvamp-0.8.3.tar.gz` & `tmp/varvamp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.8.3.tar", last modified: Mon Jun 26 16:09:33 2023, max compression
+gzip compressed data, was "varvamp-0.9.tar", last modified: Mon Jul 24 13:43:17 2023, max compression
```

## Comparing `varvamp-0.8.3.tar` & `varvamp-0.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-26 16:09:33.775199 varvamp-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-26 16:09:15.000000 varvamp-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:09:33.775199 varvamp-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 16:09:15.000000 varvamp-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.771199 varvamp-0.8.3/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.838111 varvamp-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-24 13:43:17.838111 varvamp-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 13:42:54.000000 varvamp-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:43:17.838111 varvamp-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 13:42:54.000000 varvamp-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.834111 varvamp-0.9/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.838111 varvamp-0.9/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.834111 varvamp-0.9/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.8.3/PKG-INFO` & `varvamp-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8.3
+Version: 0.9
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
-[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
 <img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
```

### Comparing `varvamp-0.8.3/README.md` & `varvamp-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
-[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
 <img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
```

### Comparing `varvamp-0.8.3/setup.py` & `varvamp-0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     packages=find_packages(),
     install_requires=[
         "biopython>=1.79",
         "matplotlib>=3.5.1",
         "primer3-py>=1.1.0",
         "pandas>=1.4.4",
         "numpy>=1.23.3",
-        "seqfold>=0.7.15"
+        "seqfold>=0.7.15",
     ],
     description='Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses',
     url='https://github.com/jonas-fuchs/varVAMP',
     author='Dr. Jonas Fuchs',
     author_email='jonas.fuchs@uniklinik-freiburg.de',
     classifiers=[
         "Programming Language :: Python :: 3.9",
```

### Comparing `varvamp-0.8.3/varvamp/command.py` & `varvamp-0.9/varvamp/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from varvamp.scripts import regions
 from varvamp.scripts import logging
 from varvamp.scripts import param_estimation
 from varvamp.scripts import primers
 from varvamp.scripts import qpcr
 from varvamp.scripts import reporting
 from varvamp.scripts import scheme
+from varvamp.scripts import blast
 from varvamp import __version__
 from . import _program
 
 
 def get_args(sysargs):
     """
     arg parsing for varvamp
@@ -84,14 +85,30 @@
             "-ml",
             "--max-length",
             help="max length of the amplicons",
             metavar="1500",
             type=int,
             default=1500
         )
+        par.add_argument(
+            "-db",
+            "--database",
+            help="location of the BLAST db",
+            metavar="None",
+            type=str,
+            default=None
+        )
+        par.add_argument(
+            "-th",
+            "--n-threads",
+            help="number of threads for the BLAST search",
+            metavar="1",
+            type=int,
+            default=1
+        )
     TILED_parser.add_argument(
         "-o",
         "--overlap",
         type=int,
         metavar="100",
         default=100,
         help="min overlap of the amplicons"
@@ -250,15 +267,15 @@
         job="Filtering for primers.",
         progress_text=f"{len(left_primer_candidates)} fw and {len(right_primer_candidates)} rw potential primers"
     )
 
     return alignment_cleaned, majority_consensus, ambiguous_consensus, primer_regions, left_primer_candidates, right_primer_candidates
 
 
-def sanger_and_tiled_shared_workflow(args, left_primer_candidates, right_primer_candidates, log_file):
+def sanger_and_tiled_shared_workflow(args, left_primer_candidates, right_primer_candidates, data_dir, log_file):
     """
     part of the workflow shared by the sanger and tiled mode
     """
 
     # find best primers and create primer dict
     all_primers = primers.find_best_primers(left_primer_candidates, right_primer_candidates)
     logging.varvamp_progress(
@@ -283,15 +300,29 @@
         )
     logging.varvamp_progress(
         log_file,
         progress=0.8,
         job="Finding potential amplicons.",
         progress_text=f"{len(amplicons)} potential amplicons"
     )
-    return all_primers, amplicons
+
+    if args.database is not None:
+        amplicons, off_target_amplicons = blast.sanger_or_tiled_blast(
+            all_primers,
+            data_dir,
+            args.database,
+            amplicons,
+            args.max_length,
+            args.n_threads,
+            log_file
+        )
+    else:
+        off_target_amplicons = []
+
+    return all_primers, amplicons, off_target_amplicons
 
 
 def sanger_workflow(args, amplicons, all_primers, log_file):
     """
     workflow part specific for sanger mode
     """
 
@@ -361,15 +392,15 @@
     # find regions for qPCR probes
     probe_regions = regions.find_regions(
         ambiguous_consensus,
         args.pn_ambig
     )
     if not probe_regions:
         logging.raise_error(
-            "no regions that fullfill probe criterias! lower threshold or increase number of ambiguous chars in probe\n",
+            "no regions that fullfill probe criteria! lower threshold or increase number of ambiguous chars in probe\n",
             log_file,
             exit=True
         )
 
     # digest probe regions
     probe_kmers = regions.produce_kmers(
         probe_regions,
@@ -431,30 +462,35 @@
 
     # start varVAMP
     args = get_args(sysargs)
     if not args.verbose:
         sys.stdout = open(os.devnull, 'w')
     start_time = time.process_time()
     results_dir, data_dir, log_file = logging.create_dir_structure(args.input[1])
+    # check if blast is installed
+    if args.mode == "tiled" or args.mode == "sanger":
+        if args.database is not None:
+            blast.check_BLAST_installation(log_file)
 
     # mode unspecific part of the workflow
     alignment_cleaned, majority_consensus, ambiguous_consensus, primer_regions, left_primer_candidates, right_primer_candidates = shared_workflow(args, log_file)
 
     # write files that are shared in all modes
     reporting.write_regions_to_bed(primer_regions, data_dir)
     reporting.write_alignment(data_dir, alignment_cleaned)
     reporting.write_fasta(data_dir, "majority_consensus", majority_consensus)
     reporting.write_fasta(results_dir, "ambiguous_consensus", ambiguous_consensus)
 
     # SANGER/TILED mode
     if args.mode == "tiled" or args.mode == "sanger":
-        all_primers, amplicons = sanger_and_tiled_shared_workflow(
+        all_primers, amplicons, off_target_amplicons = sanger_and_tiled_shared_workflow(
             args,
             left_primer_candidates,
             right_primer_candidates,
+            data_dir,
             log_file
         )
         if args.mode == "sanger":
             amplicon_scheme = sanger_workflow(
                 args,
                 amplicons,
                 all_primers,
@@ -466,14 +502,16 @@
                 amplicons,
                 left_primer_candidates,
                 right_primer_candidates,
                 all_primers,
                 ambiguous_consensus,
                 log_file
             )
+        if args.database is not None:
+            blast.write_BLAST_warning(off_target_amplicons, amplicon_scheme, log_file)
         # write files
         reporting.write_all_primers(data_dir, all_primers)
         reporting.write_scheme_to_files(
             results_dir,
             amplicon_scheme,
             ambiguous_consensus,
             args.mode
```

### Comparing `varvamp-0.8.3/varvamp/scripts/alignment.py` & `varvamp-0.9/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/config.py` & `varvamp-0.9/varvamp/scripts/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,17 +39,30 @@
 PRIMER_TM_PENALTY = 2  # temperature penalty
 PRIMER_GC_PENALTY = 0.2  # gc penalty
 PRIMER_SIZE_PENALTY = 0.5  # size penalty
 PRIMER_MAX_BASE_PENALTY = 8  # max base penalty for a primer
 PRIMER_3_PENALTY = (32, 16, 8, 4, 2)  # penalties for 3' mismatches
 PRIMER_PERMUTATION_PENALTY = 0.1  # penalty for the number of permutations
 
+# BLAST parameters (ref: PrimerBLAST (YE, Jian, et al. Primer-BLAST: a tool to design
+# target-specific primers for polymerase chain reaction. BMC bioinformatics, 2012, 13.
+# Jg., S. 1-11.)
+BLAST_SETTINGS = {  # blast settings for query search
+    "outfmt": "6 qseqid sseqid qlen length mismatch gapopen sstart send",  # do NOT change
+    "evalue": 5000,
+    "reward": 1,
+    "penalty": -1,
+    "gapopen": 2,
+    "gapextend": 1
+}
+BLAST_MAX_DIFF = 0.8  # allowed % differences between primer and BLAST hit
+BLAST_SIZE_MULTI = 2  # multiplier for the max_amp size of off targets (in relation to max amp size)
+BLAST_PENALTY = 50  # amplicon score increase -> considered only if no other possibilities
 
-# DO NOT CHANGE
-# nucleotide definitions
+# nucleotide definitions, do NOT change
 NUCS = set("atcg")
 AMBIG_NUCS = {
     "r": ["a", "g"],
     "y": ["c", "t"],
     "s": ["g", "c"],
     "w": ["a", "t"],
     "k": ["g", "t"],
```

### Comparing `varvamp-0.8.3/varvamp/scripts/consensus.py` & `varvamp-0.9/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/logging.py` & `varvamp-0.9/varvamp/scripts/logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import shutil
 import time
 import datetime
 
 # varVAMP
 from varvamp.scripts import config
+from varvamp import __version__
 
 
 def create_dir_structure(dir):
     """
     create output folders and log file
     """
     cwd = os.getcwd()
@@ -46,15 +47,15 @@
             flush=True
         )
         with open(log_file, 'w') as f:
             print(f"VARVAMP log \n\nMODE = {mode}\n", file=f)
     else:
         if progress == 1:
             stop_time = str(round(time.process_time() - start_time, 2))
-            progress_text = f"all done \n\n\rvarVAMP finished in {stop_time} sec!\n{datetime.datetime.now()}"
+            progress_text = f"all done \n\n\rvarVAMP {__version__} finished in {stop_time} sec!\n{datetime.datetime.now()}"
             job = "Finalizing output."
         print(
             "\rJob:\t\t " + job + "\nProgress: \t [{0}] {1}%".format("█"*block + "-"*(barLength-block), progress*100) + "\t" + progress_text,
             flush=True
         )
         with open(log_file, 'a') as f:
             print(
@@ -112,14 +113,21 @@
             )
         if args.opt_length < 0 or args.max_length < 0:
             raise_error(
                 "amplicon lengths can not be negative.",
                 log_file,
                 exit=True
             )
+        if args.database is not None:
+            if args.n_threads < 1:
+                raise_error(
+                    "number of threads cannot be smaller than 1.",
+                    log_file,
+                    exit=True
+                )
     # SANGER specific warnings
     if args.mode == "sanger":
         if args.report_n < 1:
             raise_error(
                 "number of reported amplicons cannot be below 1.",
                 log_file,
                 exit=True
@@ -236,14 +244,19 @@
             "QPROBE_GC_END",
             "QPRIMER_DIFF",
             "QPROBE_TEMP_DIFF",
             "QPROBE_DISTANCE",
             "QAMPLICON_LENGTH",
             "QAMPLICON_GC",
             "QAMPLICON_DEL_CUTOFF"
+        ),
+        (
+            "BLAST_MAX_DIFF",
+            "BLAST_SIZE_MULTI",
+            "BLAST_PENALTY"
         )
     ]
 
     for tup in all_vars:
         for var in tup:
             if var not in vars(config):
                 raise_error(
@@ -320,15 +333,18 @@
         ("dNTP concentration", config.PCR_DNTP_CONC),
         ("primer temperatur penalty", config.PRIMER_TM_PENALTY),
         ("primer gc penalty", config.PRIMER_GC_PENALTY),
         ("primer size penalty", config.PRIMER_SIZE_PENALTY),
         ("max base penalty", config.PRIMER_MAX_BASE_PENALTY),
         ("primer permutation penalty", config.PRIMER_PERMUTATION_PENALTY),
         ("qpcr flanking primer difference", config.QPRIMER_DIFF),
-        ("qpcr deletion size still considered for deltaG calculation", config.QAMPLICON_DEL_CUTOFF)
+        ("qpcr deletion size still considered for deltaG calculation", config.QAMPLICON_DEL_CUTOFF),
+        ("maximum difference between primer and blast db", config.BLAST_MAX_DIFF),
+        ("multiplier of the maximum length for non-specific amplicons", config.BLAST_SIZE_MULTI),
+        ("blast penalty for off targets", config.BLAST_PENALTY)
     ]
     for type, var in non_negative_var:
         if var < 0:
             raise_error(
                 f"{type} can not be negative!",
                 log_file
             )
@@ -369,14 +385,61 @@
             log_file
         )
     if config.PRIMER_GC_END[1] > 5 or config.QPROBE_GC_END[1] > 5:
         raise_error(
             "only the last 5 nucleotides of the 3' end are considered for GC 3'end calculation.",
             log_file
         )
+    if config.BLAST_MAX_DIFF > 1:
+        raise_error(
+            "max difference to the blast db should be between 0-1.",
+            log_file,
+            exit=True
+        )
+    if config.BLAST_SIZE_MULTI < 1:
+        raise_error(
+            "off-targets should be considered at least in the range of the maximal amplicon length.",
+            log_file,
+            exit=True
+        )
+    if config.BLAST_PENALTY < 10:
+        raise_error(
+            "giving a too small penalty could result in the selection of off-target producing amplicons in the final scheme.",
+            log_file,
+        )
+    # confirm proper BLAST settings in dictionary
+    if not isinstance(config.BLAST_SETTINGS, dict):
+        raise_error(
+            "BLAST settings have to be in a dictionary format!",
+            log_file,
+            exit=True
+        )
+    if config.BLAST_SETTINGS["outfmt"] != "6 qseqid sseqid qlen length mismatch gapopen sstart send":
+        raise_error(
+            "output format (outfmt) of BLAST settings is not correct",
+            log_file,
+            exit=True
+        )
+
+    # check all dict values
+    dict_values = ["evalue", "reward", "penalty", "gapopen", "gapextend"]
+
+    for blast_setting in dict_values:
+        if blast_setting not in config.BLAST_SETTINGS:
+            raise_error(
+                f"blast setting ({blast_setting}) is missing in BLAST dict",
+                log_file,
+                exit=True
+            )
+        if not isinstance(config.BLAST_SETTINGS[blast_setting], int):
+            raise_error(
+                f"blast setting ({blast_setting}) has to be an integer",
+                log_file,
+                exit=True
+            )
 
     # write all settings to file
     var_dic = vars(config)
     with open(log_file, 'a') as f:
         print(
             "\nARG SETTINGS\n",
             f"THRESHOLD = {args.threshold}",
@@ -387,14 +450,21 @@
         if args.mode in ("tiled", "sanger"):
             print(
                 f"AMPLICON_OPT_LENGTH = {args.opt_length}",
                 f"AMPLICON_MAX_LENGTH = {args.max_length}",
                 sep="\n",
                 file=f
             )
+            if args.database is not None:
+                print(
+                    f"BLAST_DATABASE = {args.database}",
+                    f"N_THREADS = {args.n_threads}",
+                    sep="\n",
+                    file=f
+                )
         if args.mode == "tiled":
             print(
                 f"MIN_OVERLAP = {args.overlap}",
                 sep="\n",
                 file=f
             )
         if args.mode == "sanger":
@@ -414,11 +484,15 @@
         print(
             "\nCONFIG SETTINGS\n",
             sep="\n",
             file=f
         )
         for var in all_vars[0]:
             print(f"{var} = {var_dic[var]}", file=f)
+        if args.mode in ("tiled", "sanger"):
+            if args.database is not None:
+                for var in all_vars[2]:
+                    print(f"{var} = {var_dic[var]}", file=f)
         if args.mode == "qpcr":
             for var in all_vars[1]:
                 print(f"{var} = {var_dic[var]}", file=f)
         print("\nPROGRESS", file=f)
```

### Comparing `varvamp-0.8.3/varvamp/scripts/param_estimation.py` & `varvamp-0.9/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/primers.py` & `varvamp-0.9/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/qpcr.py` & `varvamp-0.9/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/regions.py` & `varvamp-0.9/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/reporting.py` & `varvamp-0.9/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp/scripts/scheme.py` & `varvamp-0.9/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.3/varvamp.egg-info/PKG-INFO` & `varvamp-0.9/varvamp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8.3
+Version: 0.9
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
-[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
 <img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
```

### Comparing `varvamp-0.8.3/varvamp.egg-info/SOURCES.txt` & `varvamp-0.9/varvamp.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 varvamp.egg-info/dependency_links.txt
 varvamp.egg-info/entry_points.txt
 varvamp.egg-info/not-zip-safe
 varvamp.egg-info/requires.txt
 varvamp.egg-info/top_level.txt
 varvamp/scripts/__init__.py
 varvamp/scripts/alignment.py
+varvamp/scripts/blast.py
 varvamp/scripts/config.py
 varvamp/scripts/consensus.py
 varvamp/scripts/logging.py
 varvamp/scripts/param_estimation.py
 varvamp/scripts/primers.py
 varvamp/scripts/qpcr.py
 varvamp/scripts/regions.py
```

