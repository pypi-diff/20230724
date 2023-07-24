# Comparing `tmp/ncbi-genome-download-0.3.1.tar.gz` & `tmp/ncbi-genome-download-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi-genome-download-0.3.1.tar", last modified: Wed Dec  1 11:26:57 2021, max compression
+gzip compressed data, was "ncbi-genome-download-0.3.2.tar", last modified: Mon Jul 24 06:26:48 2023, max compression
```

## Comparing `ncbi-genome-download-0.3.1.tar` & `ncbi-genome-download-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 11:26:57.550479 ncbi-genome-download-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10308 2021-12-01 11:26:57.550479 ncbi-genome-download-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9638 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/README-CN.md
--rw-r--r--   0 runner    (1001) docker     (121)     9576 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 11:26:57.546479 ncbi-genome-download-0.3.1/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6113 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/contrib/gimme_taxa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 11:26:57.546479 ncbi-genome-download-0.3.1/ncbi_genome_download/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12014 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    29971 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/ncbi_genome_download/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 11:26:57.550479 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10308 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-01 11:26:57.000000 ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-12-01 11:26:57.550479 ncbi-genome-download-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 11:26:57.550479 ncbi-genome-download-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/assembly_status.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10561 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/noascii_summary.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/partial_summary.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/type_material.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/viral_summary.txt
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-12-01 11:26:44.000000 ncbi-genome-download-0.3.1/tests/weird_organism_name_summary.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/README-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.592561 ncbi-genome-download-0.3.2/contrib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6113 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/contrib/gimme_taxa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/ncbi_genome_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/assembly_status.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/new_format_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/noascii_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/partial_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/type_material.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/viral_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/weird_organism_name_summary.txt
```

### Comparing `ncbi-genome-download-0.3.1/LICENSE` & `ncbi-genome-download-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/PKG-INFO` & `ncbi-genome-download-0.3.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,9 @@
-Metadata-Version: 2.1
-Name: ncbi-genome-download
-Version: 0.3.1
-Summary: Download genome files from the NCBI FTP server.
-Home-page: https://github.com/kblin/ncbi-genome-download/
-Author: Kai Blin
-Author-email: kblin@biosustain.dtu.dk
-License: Apache Software License
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # NCBI Genome Downloading Scripts
 
-[![Build Status](https://github.drone.secondarymetabolites.org/api/badges/kblin/ncbi-genome-download/status.svg)](https://github.drone.secondarymetabolites.org/kblin/ncbi-genome-download)
 [![PyPI release](https://img.shields.io/pypi/v/ncbi-genome-download.svg)](https://pypi.python.org/pypi/ncbi-genome-download/)
 
 Some script to download bacterial and fungal genomes from NCBI after they
 restructured their FTP a while ago.
 
 Idea shamelessly stolen from [Mick Watson's Kraken downloader
 scripts](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/)
@@ -33,248 +12,301 @@
 scripts are ~~written in Perl~~ specific to actually building a Kraken database
 (as advertised).
 
 So this is a set of scripts that focuses on the actual genome downloading.
 
 ## Installation
 
-```
+```bash
 pip install ncbi-genome-download
 ```
 
 Alternatively, clone this repository from GitHub, then run (in a python virtual environment)
-```
+
+```bash
 pip install .
 ```
+
 If this fails on older versions of Python, try updating your `pip` tool first:
-```
+
+```bash
 pip install --upgrade pip
 ```
+
 and then rerun the `ncbi-genome-download` install.
 
 Alternatively, `ncbi-genome-download` is packaged in `conda`.
-Refer the the Anaconda/miniconda site to install a distribution (highly recommended) https://conda.io/miniconda.html
-With that installed one can do:
-```
+Refer the the Anaconda/[miniconda](https://conda.io/miniconda.html) site to
+install a distribution (highly recommended). With that installed one can do:
+
+```bash
 conda install -c bioconda ncbi-genome-download
 ```
 
-`ncbi-genome-download` is only developed and tested on Python releases still under active
-support by the Python project. At the moment, this means versions 3.5, 3.6, 3.7, and 3.8.
-Specifically, no attempt at testing under Python versions older than 3.5 is being made.
+`ncbi-genome-download` is only developed and tested on Python releases still
+under active support by the Python project. At the moment, this means versions
+3.7, 3.8, 3.9, 3.10 and 3.11.
+Specifically, no attempt at testing under Python versions older than 3.7 is
+being made.
 
 If your system is stuck on an older version of Python, consider using a tool like
 [Homebrew](http://brew.sh) to obtain a more up-to-date version.
 
 `ncbi-genome-download` 0.2.12 was the last version to support Python 2.
 
 ## Usage
 
 To download all bacterial RefSeq genomes in GenBank format from NCBI, run the following:
-```
+
+```bash
 ncbi-genome-download bacteria
 ```
 
 Downloading multiple groups is also possible:
-```
+
+```bash
 ncbi-genome-download bacteria,viral
 ```
 
-**Note**: To see all available groups, see `ncbi-genome-download --help`, or simply use `all` to check all groups.
-Naming a more specific group will reduce the download size and the time needed to find the sequences to download.
+**Note**: To see all available groups, see `ncbi-genome-download --help`, or
+simply use `all` to check all groups. Naming a more specific group will reduce
+the download size and the time needed to find the sequences to download.
 
-If you're on a reasonably fast connection, you might want to try running multiple downloads in parallel:
-```
+If you're on a reasonably fast connection, you might want to try running
+multiple downloads in parallel:
+
+```bash
 ncbi-genome-download bacteria --parallel 4
 ```
 
-
 To download all fungal GenBank genomes from NCBI in GenBank format, run:
-```
+
+```bash
 ncbi-genome-download --section genbank fungi
 ```
 
 To download all viral RefSeq genomes in FASTA format, run:
-```
+
+```bash
 ncbi-genome-download --formats fasta viral
 ```
 
-It is possible to download multiple formats by supplying a list of formats or simply download all formats:
-```
+It is possible to download multiple formats by supplying a list of formats or
+simply downloading all formats:
+
+```bash
 ncbi-genome-download --formats fasta,assembly-report viral
 ncbi-genome-download --formats all viral
 ```
 
 To download only completed bacterial RefSeq genomes in GenBank format, run:
-```
+
+```bash
 ncbi-genome-download --assembly-levels complete bacteria
 ```
 
 It is possible to download multiple assembly levels at once by supplying a list:
-```
+
+```bash
 ncbi-genome-download --assembly-levels complete,chromosome bacteria
 ```
 
 To download only bacterial reference genomes from RefSeq in GenBank format, run:
-```
+
+```bash
 ncbi-genome-download --refseq-categories reference bacteria
 ```
 
 To download bacterial RefSeq genomes of the genus _Streptomyces_, run:
-```
+
+```bash
 ncbi-genome-download --genera Streptomyces bacteria
 ```
+
 **Note**: This is a simple string match on the organism name provided by NCBI only.
 
-You can also use this with a slight trick to download genomes of a certain species as well:
-```
+You can also use this with a slight trick to download genomes of a certain
+species as well:
+
+```bash
 ncbi-genome-download --genera "Streptomyces coelicolor" bacteria
 ```
+
 **Note**: The quotes are important. Again, this is a simple string match on the organism
 name provided by the NCBI.
 
 Multiple genera is also possible:
-```
+
+```bash
 ncbi-genome-download --genera "Streptomyces coelicolor,Escherichia coli" bacteria
 ```
 
 You can also put genus names into a file, one organism per line, e.g.:
-```
+
+```bash
 Streptomyces
 Amycolatopsis
 ```
 
-Then, pass the path to that file (e.g. `my_genera.txt`) to the `--genera` option, like so:
-```
+Then, pass the path to that file (e.g. `my_genera.txt`) to the `--genera`
+option, like so:
+
+```bash
 ncbi-genome-download --genera my_genera.txt bacteria
 ```
-**Note**: The above command will download all _Streptomyces_ and _Amycolatopsis_ genomes from RefSeq.
 
-You can make the string match fuzzy using the `--fuzzy-genus` option. This can be handy if you need to match
-a value in the middle of the NCBI organism name, like so:
+**Note**: The above command will download all _Streptomyces_ and _Amycolatopsis_
+genomes from RefSeq.
 
-```
+You can make the string match fuzzy using the `--fuzzy-genus` option. This can
+be handy if you need to match a value in the middle of the NCBI organism name,
+like so:
+
+```bash
 ncbi-genome-download --genera coelicolor --fuzzy-genus bacteria
 ```
-**Note**: The above command will download all bacterial genomes containing "coelicolor" anywhere in their
-organism name from RefSeq.
+
+**Note**: The above command will download all bacterial genomes containing
+"coelicolor" anywhere in their organism name from RefSeq.
 
 To download bacterial RefSeq genomes based on their NCBI species taxonomy ID, run:
-```
+
+```bash
 ncbi-genome-download --species-taxids 562 bacteria
 ```
-**Note**: The above command will download all RefSeq genomes belonging to _Escherichia coli_.
+
+**Note**: The above command will download all RefSeq genomes belonging to
+_Escherichia coli_.
 
 To download a specific bacterial RefSeq genomes based on its NCBI taxonomy ID, run:
-```
+
+```bash
 ncbi-genome-download --taxids 511145 bacteria
 ```
-**Note**: The above command will download the RefSeq genome belonging to _Escherichia coli str. K-12 substr. MG1655_.
 
-It is also possible to download multiple species taxids or taxids by supplying the numbers in a comma-separated list:
-```
+**Note**: The above command will download the RefSeq genome belonging to
+_Escherichia coli str. K-12 substr. MG1655_.
+
+It is also possible to download multiple species taxids or taxids by supplying
+the numbers in a comma-separated list:
+
+```bash
 ncbi-genome-download --taxids 9606,9685 --assembly-level chromosome vertebrate_mammalian
 ```
+
 **Note**: The above command will download the reference genomes for cat and human.
 
 In addition, you can put multiple species taxids or taxids into a file, one per line
 and pass that filename to the `--species-taxids` or `--taxids` parameters, respectively.
 
 Assuming you had a file `my_taxids.txt` with the following contents:
-```
+
+```text
 9606
 9685
 ```
+
 You could download the reference genomes for cat and human like this:
-```
+
+```bash
 ncbi-genome-download --taxids my_taxids.txt --assembly-levels chromosome vertebrate_mammalian
 ```
 
-It is possible to also create a human-readable directory structure in parallel to mirroring
-the layout used by NCBI:
-```
+It is possible to also create a human-readable directory structure in parallel
+to mirroring the layout used by NCBI:
+
+```bash
 ncbi-genome-download --human-readable bacteria
 ```
+
 This will use links to point to the appropriate files in the NCBI directory structure,
-so it saves file space. Note that links are not supported on some Windows file systems and some
-older versions of Windows.
+so it saves file space. Note that links are not supported on some Windows file
+systems and some older versions of Windows.
 
 It is also possible to re-run a previous download with the `--human-readable` option.
-In this case, `ncbi-genome-download` will not download any new genome files, and just create
-human-readable directory structure. Note that if any files have been changed on the NCBI side,
-a file download will be triggered.
+In this case, `ncbi-genome-download` will not download any new genome files, and
+just create human-readable directory structure. Note that if any files have been
+changed on the NCBI side, a file download will be triggered.
 
-There is a "dry-run" option to show which accessions would be downloaded, given your filters:
-```
+There is a "dry-run" option to show which accessions would be downloaded, given
+your filters:
+
+```bash
 ncbi-genome-download --dry-run bacteria
 ```
 
 If you want to filter for the "relation to type material" column of the
 assembly summary file, you can use the `--type-materials` option. Possible
 values are "any", "all", "type", "reference", "synonym", "proxytype", and/or
 "neotype". "any" will include assemblies with no relation to type material
 value defined, "all" will download only assemblies with a defined value.
 Multiple values can be given, separated by comma:
-```
+
+```bash
 ncbi-genome-download --type-materials type,reference
 ```
 
-By default, ncbi-genome-download caches the assembly summary files for the respective taxonomic
-groups for one day. You can skip using the cache file by using the `--no-cache` option.
-The output of `--help` also shows the cache directory, should you want to remove any of the cached
-files.
+By default, ncbi-genome-download caches the assembly summary files for the
+respective taxonomic groups for one day. You can skip using the cache file by
+using the `--no-cache` option. The output of `--help` also shows the cache
+directory, should you want to remove any of the cached files.
 
 To get an overview of all options, run
-```
+
+```bash
 ncbi-genome-download --help
 ```
 
 ### As a method
-You can also use it as a method call. Pass the pythonised keyword arguments (`_` instead of `-`)
- as described above or in the `--help`:
-```
+
+You can also use it as a method call. Pass the pythonised keyword arguments
+(`_` instead of `-`) as described above or in the `--help`:
+
+```python
 import ncbi_genome_download as ngd
 ngd.download()
 ```
-**Note**: To specify a taxonomic group, like *bacteria*, use the `group` keyword.
 
+**Note**: To specify a taxonomic group, like _bacteria_, use the `group` keyword.
 
 ### Contributed Scripts: `gimme_taxa.py`
-This script lets you find out what TaxIDs to pass to `ngd`, and will write a simple one-item-per-line
-file to pass in to it. It utilises the `ete3` toolkit, so refer to their site to install the dependency
-if it's not already satisfied.
-
-You can query the database using a particular TaxID, or a scientific name. The primary function of the
-script is to return all the child taxa of the specified parent taxa. The script has various options
-for what information is written in the output.
+
+This script lets you find out what TaxIDs to pass to `ngd`, and will write a
+simple one-item-per-line file to pass in to it. It utilises the `ete3` toolkit,
+so refer to their site to install the dependency if it's not already satisfied.
+
+You can query the database using a particular TaxID, or a scientific name. The
+primary function of the script is to return all the child taxa of the specified
+parent taxa. The script has various options for what information is written in
+the output.
 
 A basic invocation may look like:
 
-```
+```bash
 # Fetch all descendent taxa for Escherichia (taxid 561):
 python gimme_taxa.py -o ~/mytaxafile.txt 561
 
 # Alternatively, just provide the taxon name
 python gimme_taxa.py -o all_descendent_taxids.txt Escherichia
 
 # You can provide multiple taxids and/or names
 python gimme_taxa.py -o all_descendent_taxids.txt 561,Methanobrevibacter
 ```
 
 On first use, a small sqlite database will be created in your home directory
-by default (change the location with the `--database` flag). You can update this database
-by using the `--update` flag. Note that if the database is not in your home directory,
-you must specify it with `--database` or a new database will be created in your home
-directory.
+by default (change the location with the `--database` flag). You can update this
+database by using the `--update` flag. Note that if the database is not in your
+home directory, you must specify it with `--database` or a new database will be
+created in your home directory.
 
 To see all help:
-```
+
+```bash
 python gimme_taxa.py
 python gimme_taxa.py -h
 python gimme_taxa.py --help
 ```
 
 ## License
+
 All code is available under the Apache License version 2, see the
 [`LICENSE`](LICENSE) file for details.
-
-
```

### Comparing `ncbi-genome-download-0.3.1/README-CN.md` & `ncbi-genome-download-0.3.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/contrib/gimme_taxa.py` & `ncbi-genome-download-0.3.2/contrib/gimme_taxa.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/__main__.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/__main__.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/config.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         ('genpept', '_protein.gpff.gz'),
         ('wgs', '_wgsmaster.gbff.gz'),
         ('cds-fasta', '_cds_from_genomic.fna.gz'),
         ('rna-fna', '_rna.fna.gz'),
         ('rna-fasta', '_rna_from_genomic.fna.gz'),
         ('assembly-report', '_assembly_report.txt'),
         ('assembly-stats', '_assembly_stats.txt'),
+        ('translated-cds', '_translated_cds.faa.gz'),
     ])
 
     _LEVELS = OrderedDict([
         ('complete', 'Complete Genome'),
         ('chromosome', 'Chromosome'),
         ('scaffold', 'Scaffold'),
         ('contig', 'Contig'),
```

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/core.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import argparse
 import codecs
 from datetime import datetime, timedelta
 import errno
 import hashlib
 import logging
 import os
+from pathlib import Path
 import sys
+import time
 from io import StringIO
 from multiprocessing import Pool
 from tqdm import tqdm
 
 import requests
 
 from .config import (
@@ -88,17 +90,21 @@
                              'A comma-separated list of taxids is also possible. For example: "9606,9685". '
                              '(default: %(default)s)')
     parser.add_argument('-A', '--assembly-accessions', dest='assembly_accessions',
                         default=NgdConfig.get_default('assembly_accessions'),
                         help='Only download sequences matching the provided NCBI assembly accession(s). '
                         'A comma-separated list of accessions is possible, as well as a path to a filename '
                         'containing one accession per line.')
+    parser.add_argument('--fuzzy-accessions', dest='fuzzy_accessions', action="store_true",
+                        default=NgdConfig.get_default('fuzzy_accessions'),
+                        help="Use a fuzzy search on the entry accession instead of an exact match.")
     parser.add_argument('-R', '--refseq-categories', dest='refseq_categories',
                         default=NgdConfig.get_default('refseq_categories'),
-                        help='Only download sequences of the provided refseq categories (default: %(default)s)')
+                        help='Only download sequences of the provided refseq categories [refrerence, representative, na]. '
+                             'A comma-separated list of categories is also possible. (default: download all categories)')
     parser.add_argument('--refseq-category', dest='refseq_categories',
                         action=DeprecatedAction, new_name="--refseq-categories",
                         help="Deprecated alias for --refseq-categories")
     parser.add_argument('-o', '--output-folder', dest='output',
                         default=NgdConfig.get_default('output'),
                         help='Create output hierarchy in specified folder (default: %(default)s)')
     parser.add_argument('--flat-output', dest="flat_output", action="store_true",
@@ -207,46 +213,51 @@
 
             return 0
 
         download_jobs = []
 
         mtable = metadata.get()
         if config.parallel == 1:
+            if config.progress_bar:
+                download_candidates = tqdm(download_candidates, desc="Checking assemblies", unit="entries")
             for entry, group in download_candidates:
                 curr_jobs = create_downloadjob(entry, group, config)
                 fill_metadata(curr_jobs, entry, mtable)
                 download_jobs.extend(curr_jobs)
             if config.progress_bar:
-                tqdm.write("start download. No parallel")
-                _download_jobs = tqdm(download_jobs)
+                _download_jobs = tqdm(download_jobs, desc="Downloading assemblies", unit="files")
             else:
                 _download_jobs = download_jobs
 
             for dl_job in _download_jobs:
                 worker(dl_job)
         else:  # pragma: no cover
             # Testing multiprocessing code is annoying
             with Pool(processes=config.parallel) as pool:
-                dl_jobs = pool.imap(
-                        downloadjob_creator_caller,
-                        [(entry, group, config) for entry, group in download_candidates],
-                    )
+                dl_jobs = [pool.apply_async(downloadjob_creator_caller, ((entry, group, config),))
+                           for entry, group in download_candidates]
+
+                if config.progress_bar:
+                    _dl_jobs = tqdm(dl_jobs, desc="Checking assemblies", unit="entries")
+                else:
+                    _dl_jobs = dl_jobs
+
+                dl_jobs = [_.get(0xFFFF) for _ in _dl_jobs]
 
                 for index, created_dl_job in enumerate(dl_jobs):
                     download_jobs.extend(created_dl_job)
                     # index is conserved from download_candidates with the use of imap
                     fill_metadata(created_dl_job, download_candidates[index][0], mtable)
 
                 jobs = [pool.apply_async(worker, (_,))
                         for _ in download_jobs]
                 try:
 
                     if config.progress_bar:
-                        tqdm.write("start download. Parallel=5")
-                        _jobs = tqdm(jobs)
+                        _jobs = tqdm(jobs, desc="Downloading assemblies", unit="files")
                     else:
                         _jobs = jobs
                     # add a wrapper for progress bar
                     # 0xFFFF is just "a really long time"
                     [_.get(0xFFFF) for _ in _jobs]
                 except KeyboardInterrupt:
                     # TODO: Actually test this once I figure out how to do this in py.test
@@ -436,21 +447,27 @@
     logger.info('Checking record %r', entry['assembly_accession'])
     full_output_dir = create_dir(entry, config.section, domain, config.output, config.flat_output)
 
     symlink_path = None
     if config.human_readable:
         symlink_path = create_readable_dir(entry, config.section, domain, config.output)
 
-    checksums = grab_checksums_file(entry)
-
     if not config.flat_output:
-        # TODO: Only write this when the checksums file changed
-        with open(os.path.join(full_output_dir, 'MD5SUMS'), 'w') as handle:
-            handle.write(checksums)
+        checksum_path = Path(full_output_dir) / 'MD5SUMS'
 
+        # if the MD5SUM file is missing or too old, redownload
+        if not checksum_path.exists() or checksum_path.stat().st_mtime + (24 * 60 * 60) < time.time():
+            checksums = grab_checksums_file(entry)
+            with checksum_path.open('w', encoding="utf-8") as handle:
+                handle.write(checksums)
+        else:
+            with checksum_path.open('r', encoding="utf-8") as handle:
+                checksums = handle.read()
+    else:
+        checksums = grab_checksums_file(entry)
     parsed_checksums = parse_checksums(checksums)
 
     download_jobs = []
     for fmt in config.file_formats:
         try:
             if has_file_changed(full_output_dir, parsed_checksums, fmt):
                 download_jobs.append(
```

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/jobs.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/jobs.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/metadata.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/metadata.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download/summary.py` & `ncbi-genome-download-0.3.2/ncbi_genome_download/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         self._file = infile
         self._lineno = 0
         line = ''
         while 'assembly_accession' not in line:
             line = self._file.readline().rstrip('\n')
             self._lineno += 1
 
-        if line.startswith('# '):
-            line = line[2:]
+        if line.startswith('#'):
+            line = line[1:].strip()
 
         self._fields = line.split('\t')
 
     def __iter__(self):
         return self
 
     def __next__(self):
```

### Comparing `ncbi-genome-download-0.3.1/ncbi_genome_download.egg-info/SOURCES.txt` & `ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 ncbi_genome_download.egg-info/PKG-INFO
 ncbi_genome_download.egg-info/SOURCES.txt
 ncbi_genome_download.egg-info/dependency_links.txt
 ncbi_genome_download.egg-info/entry_points.txt
 ncbi_genome_download.egg-info/requires.txt
 ncbi_genome_download.egg-info/top_level.txt
 tests/assembly_status.txt
+tests/new_format_summary.txt
 tests/noascii_summary.txt
 tests/partial_summary.txt
 tests/requirements.txt
 tests/type_material.txt
 tests/viral_summary.txt
 tests/weird_organism_name_summary.txt
```

### Comparing `ncbi-genome-download-0.3.1/setup.py` & `ncbi-genome-download-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/assembly_status.txt` & `ncbi-genome-download-0.3.2/tests/assembly_status.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/noascii_summary.txt` & `ncbi-genome-download-0.3.2/tests/noascii_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/partial_summary.txt` & `ncbi-genome-download-0.3.2/tests/partial_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/type_material.txt` & `ncbi-genome-download-0.3.2/tests/type_material.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/viral_summary.txt` & `ncbi-genome-download-0.3.2/tests/viral_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.1/tests/weird_organism_name_summary.txt` & `ncbi-genome-download-0.3.2/tests/weird_organism_name_summary.txt`

 * *Files identical despite different names*

