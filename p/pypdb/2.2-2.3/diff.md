# Comparing `tmp/pypdb-2.2.tar.gz` & `tmp/pypdb-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdb-2.2.tar", last modified: Thu Jul 14 10:20:07 2022, max compression
+gzip compressed data, was "pypdb-2.3.tar", last modified: Mon Jul 24 02:29:43 2023, max compression
```

## Comparing `pypdb-2.2.tar` & `pypdb-2.3.tar`

### file list

```diff
@@ -1,49 +1,58 @@
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.187080 pypdb-2.2/
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)     1082 2015-05-13 05:20:06.000000 pypdb-2.2/LICENSE
--rw-r--r--   0 williamgilpin   (502) staff       (20)      396 2022-07-14 10:20:07.187219 pypdb-2.2/PKG-INFO
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)     2456 2022-04-26 21:05:16.000000 pypdb-2.2/README.md
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.178071 pypdb-2.2/pypdb/
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)       49 2020-11-11 23:44:19.000000 pypdb-2.2/pypdb/__init__.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.179987 pypdb-2.2/pypdb/clients/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-11-15 12:33:00.000000 pypdb-2.2/pypdb/clients/__init__.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.180162 pypdb-2.2/pypdb/clients/data/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-11-16 23:58:14.000000 pypdb-2.2/pypdb/clients/data/__init__.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.181056 pypdb-2.2/pypdb/clients/fasta/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/fasta/__init__.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     2642 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/fasta/fasta_client.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     2511 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/fasta/fasta_client_test.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.181832 pypdb-2.2/pypdb/clients/pdb/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/pdb/__init__.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     2706 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/pdb/pdb_client.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     3703 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/pdb/pdb_client_test.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.182840 pypdb-2.2/pypdb/clients/search/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-11-16 23:57:57.000000 pypdb-2.2/pypdb/clients/search/__init__.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.185809 pypdb-2.2/pypdb/clients/search/operators/
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1555 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/chemical_operators.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1499 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/chemical_operators_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)      907 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/seqmotif_operators.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)      746 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/seqmotif_operators_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     2443 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/sequence_operators.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1480 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/sequence_operators_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1140 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/structure_operators.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1216 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/structure_operators_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     5864 2021-06-10 17:32:02.000000 pypdb-2.2/pypdb/clients/search/operators/text_operators.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)      764 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/clients/search/operators/text_operators_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)    12367 2022-07-14 10:00:54.000000 pypdb-2.2/pypdb/clients/search/search_client.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)    21180 2021-11-01 19:06:44.000000 pypdb-2.2/pypdb/clients/search/search_client_test.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)       57 2020-11-11 23:27:37.000000 pypdb-2.2/pypdb/conftest.py
--rwxr-xr-x   0 williamgilpin   (502) staff       (20)    34116 2022-07-14 10:13:23.000000 pypdb-2.2/pypdb/pypdb.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.186800 pypdb-2.2/pypdb/util/
--rw-r--r--   0 williamgilpin   (502) staff       (20)        0 2020-11-11 23:36:53.000000 pypdb-2.2/pypdb/util/__init__.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     1892 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/util/http_requests.py
--rw-r--r--   0 williamgilpin   (502) staff       (20)     4165 2020-12-30 00:23:06.000000 pypdb-2.2/pypdb/util/test_http_requests.py
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.179485 pypdb-2.2/pypdb.egg-info/
-drwxr-xr-x   0 williamgilpin   (502) staff       (20)        0 2022-07-14 10:20:07.179751 pypdb-2.2/pypdb.egg-info/.ipynb_checkpoints/
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)        1 2020-11-15 12:06:33.000000 pypdb-2.2/pypdb.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)      396 2022-07-14 10:20:06.000000 pypdb-2.2/pypdb.egg-info/PKG-INFO
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)     1309 2022-07-14 10:20:07.000000 pypdb-2.2/pypdb.egg-info/SOURCES.txt
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)        1 2022-07-14 10:20:06.000000 pypdb-2.2/pypdb.egg-info/dependency_links.txt
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)        9 2022-07-14 10:20:06.000000 pypdb-2.2/pypdb.egg-info/requires.txt
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)        6 2022-07-14 10:20:06.000000 pypdb-2.2/pypdb.egg-info/top_level.txt
--rwxrwxrwx   0 williamgilpin   (502) staff       (20)       79 2022-07-14 10:20:07.187661 pypdb-2.2/setup.cfg
--rwxr-xr-x   0 williamgilpin   (502) staff       (20)      749 2022-07-14 10:19:39.000000 pypdb-2.2/setup.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608676 pypdb-2.3/
+-rwxrwxrwx   0 william    (503) staff       (20)     1082 2015-05-13 05:20:06.000000 pypdb-2.3/LICENSE
+-rw-r--r--   0 william    (503) staff       (20)      351 2023-07-24 02:29:43.608725 pypdb-2.3/PKG-INFO
+-rwxr-xr-x   0 william    (503) staff       (20)     2578 2023-07-24 02:23:45.000000 pypdb-2.3/README.md
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.603598 pypdb-2.3/pypdb/
+-rwxrwxrwx   0 william    (503) staff       (20)       49 2020-11-11 23:44:19.000000 pypdb-2.3/pypdb/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604457 pypdb-2.3/pypdb/clients/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604750 pypdb-2.3/pypdb/clients/data/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/data/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     6236 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/data_types.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.605063 pypdb-2.3/pypdb/clients/data/graphql/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/data/graphql/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1126 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/graphql/graphql.py
+-rw-r--r--   0 william    (503) staff       (20)      976 2023-07-15 03:42:36.000000 pypdb-2.3/pypdb/clients/data/graphql/test_graphql.py
+-rw-r--r--   0 william    (503) staff       (20)     3980 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/test_data_types.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.605599 pypdb-2.3/pypdb/clients/fasta/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/fasta/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     2825 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/fasta/fasta_client.py
+-rw-r--r--   0 william    (503) staff       (20)     2527 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/fasta/fasta_client_test.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.606067 pypdb-2.3/pypdb/clients/pdb/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     2706 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/pdb_client.py
+-rw-r--r--   0 william    (503) staff       (20)     3703 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/pdb_client_test.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.606458 pypdb-2.3/pypdb/clients/search/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.607977 pypdb-2.3/pypdb/clients/search/operators/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-07-15 03:42:36.000000 pypdb-2.3/pypdb/clients/search/operators/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1555 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/chemical_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1499 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/chemical_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)      907 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators.py
+-rw-r--r--   0 william    (503) staff       (20)      746 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     2443 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/sequence_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1480 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/sequence_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     1140 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/structure_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1216 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/structure_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     5901 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/search/operators/text_operators.py
+-rw-r--r--   0 william    (503) staff       (20)      764 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/text_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)    12663 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/search/search_client.py
+-rw-r--r--   0 william    (503) staff       (20)    21180 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/search_client_test.py
+-rw-r--r--   0 william    (503) staff       (20)       57 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/conftest.py
+-rwxr-xr-x   0 william    (503) staff       (20)    34307 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/pypdb.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608329 pypdb-2.3/pypdb/util/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1892 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/http_requests.py
+-rw-r--r--   0 william    (503) staff       (20)     4165 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/test_http_requests.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604210 pypdb-2.3/pypdb.egg-info/
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604319 pypdb-2.3/pypdb.egg-info/.ipynb_checkpoints/
+-rwxrwxrwx   0 william    (503) staff       (20)        1 2020-11-15 12:06:33.000000 pypdb-2.3/pypdb.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rwxrwxrwx   0 william    (503) staff       (20)      351 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/PKG-INFO
+-rwxrwxrwx   0 william    (503) staff       (20)     1563 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/SOURCES.txt
+-rwxrwxrwx   0 william    (503) staff       (20)        1 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/dependency_links.txt
+-rwxrwxrwx   0 william    (503) staff       (20)       16 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/requires.txt
+-rwxrwxrwx   0 william    (503) staff       (20)        6 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/top_level.txt
+-rwxrwxrwx   0 william    (503) staff       (20)       79 2023-07-24 02:29:43.608904 pypdb-2.3/setup.cfg
+-rwxr-xr-x   0 william    (503) staff       (20)      793 2023-07-24 02:28:39.000000 pypdb-2.3/setup.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608467 pypdb-2.3/tests/
+-rw-r--r--   0 william    (503) staff       (20)     2397 2023-07-15 05:37:14.000000 pypdb-2.3/tests/test_pypdb.py
```

### Comparing `pypdb-2.2/LICENSE` & `pypdb-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/README.md` & `pypdb-2.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 # PyPDB
 
 A Python 3 toolkit for performing searches with the RCSB Protein Data Bank (PDB). This can be used to perform advanced searches for PDB IDs matching various criteria, as well as to look up information associated with specific PDB IDs. This tool allows standard operations that can be perfomed from within the PDB website (BLAST, PFAM lookup, etc.) to be performed from within Python scripts.
 
-Examples of each function and its associated output can be found in [`demos/demos.ipynb`](demos/demos.ipynb).
-
 If you use this module for any published work, please consider citing the accompanying paper
 
-      Gilpin, W. "PyPDB: A Python API for the Protein Data Bank." 
+      Gilpin, W. "PyPDB: A Python API for the Protein Data Bank."
       Bioinformatics, Oxford Journals, 2016.
 
-**We very much welcome contributors and pull requests**
-
 ## Installation
 
 Install using pip:
 
-	$ pip install pypdb
+    $ pip install pypdb
 
 To install the development version, which contains the latest features and fixes, install directly from GitHub using
 
-   	$ pip install git+git://github.com/williamgilpin/pypdb
+    $ pip install git+https://github.com/williamgilpin/pypdb
 
 If you need to  install directly from setup.py,
 
     $ python setup.py install
 
 Test the installation, and check that the code successfully connects to the PDB, navigate to the root directory and run
 
-	$ pytest 
+    $ pytest
 
 This code has been designed and tested for Python 3.
 
 ## Usage
 
-This package can be used to get lists of PDB IDs associated with specific search terms, experiment types, structures, and other common criteria.
-
-Given a list of PDBs, this package can be used to fetch any data associated with those PDBs, including their dates of deposition, lists of authors and associated publications, their sequences or structures, their top BLAST matches, and other query-specific attributes like lists of a ligands or chemical structure.
+### PDB Text Search
+This package can be used to get lists of PDB IDs associated with specific search terms, experiment types, structures, and other common criteria. To use the simple API, see the examples in [`demos/demos.ipynb`](demos/demos.ipynb). For advanced search and query logic, see the examples in [`search/EXAMPLES.md`](pypdb/clients/search/EXAMPLES.md).
 
-A set of demos is included in the iPython notebook **demos.ipynb**. A static version of this notebook (for viewing) is available as **demos.html**
+### PDB Data Fetch
+Given a list of PDBs, this package can be used to fetch data associated with those PDBs, including their dates of deposition, lists of authors and associated publications, their sequences or structures, their top BLAST matches, and other query-specific attributes like lists of a ligands or chemical structure.  To use the simple API, see the examples in [`demos/demos.ipynb`](demos/demos.ipynb). For advanced search and query logic, see the examples in [`data/EXAMPLES.md`](pypdb/clients/data/EXAMPLES.md).
 
 ## Issues and Feature Requests
 
 If you run into an issue, or if you find a workaround for an existing issue, we would very much appreciate it if you could post your question or code as a GitHub issue.
 
 If posting a feature request, please check that your request is possible using [the current GUI on current RCSB website](https://www.rcsb.org/search/advanced). If so, please perform your search, and then click the link that says `JSON` in the upper right hand corner of the Advanced Search box. Please post that JSON code with your feature request.
```

### Comparing `pypdb-2.2/pypdb/clients/fasta/fasta_client.py` & `pypdb-2.3/pypdb/clients/fasta/fasta_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,26 +47,30 @@
             FastaSequence(entity_id=entity_id,
                           chains=chains,
                           sequence=fasta_sequence,
                           fasta_header=fasta_header))
     return fasta_list
 
 
-def get_fasta_from_rcsb_entry(rcsb_id: str) -> List[FastaSequence]:
+def get_fasta_from_rcsb_entry(rcsb_id: str,
+                              verbosity: bool = True,
+                              ) -> List[FastaSequence]:
     """Fetches FASTA sequence associated with PDB structure from RCSB.
 
     Args:
       rcsb_id: RCSB accession code of the structure of interest. E.g. `"5RU3"`
+      verbosity: Print out the search query to the console (default: True)
 
     Returns:
       Dictionary containing FASTA result, from polymer entity id to the
       `FastaSequence` object associated with that entity.
     """
 
-    print("Querying RCSB for the '{}' FASTA file.".format(rcsb_id))
+    if verbosity:
+        print("Querying RCSB for the '{}' FASTA file.".format(rcsb_id))
     response = requests.get(FASTA_BASE_URL + rcsb_id)
 
     if not response.ok:
         warnings.warn("It appears request failed with:" + response.text)
         response.raise_for_status()
 
     return _parse_fasta_text_to_list(response.text)
```

### Comparing `pypdb-2.2/pypdb/clients/fasta/fasta_client_test.py` & `pypdb-2.3/pypdb/clients/fasta/fasta_client_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @mock.patch.object(fasta_client, "_parse_fasta_text_to_list")
     def test_get_fasta_file(self, mock_parse_fasta, mock_get):
         mock_response = mock.Mock()
         mock_response.ok = True
         mock_response.text = "fake_fasta_response"
         mock_get.return_value = mock_response
 
-        fasta_client.get_fasta_from_rcsb_entry("6TML")
+        fasta_client.get_fasta_from_rcsb_entry("6TML", verbosity=True)
         mock_get.assert_called_once_with(
             "https://www.rcsb.org/fasta/entry/6TML")
         mock_parse_fasta.assert_called_once_with("fake_fasta_response")
 
     def test_parse_fasta_file(self):
 
         test_fasta_raw_text = """
```

### Comparing `pypdb-2.2/pypdb/clients/pdb/pdb_client.py` & `pypdb-2.3/pypdb/clients/pdb/pdb_client.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/pdb/pdb_client_test.py` & `pypdb-2.3/pypdb/clients/pdb/pdb_client_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/chemical_operators.py` & `pypdb-2.3/pypdb/clients/search/operators/chemical_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/chemical_operators_test.py` & `pypdb-2.3/pypdb/clients/search/operators/chemical_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/seqmotif_operators.py` & `pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/seqmotif_operators_test.py` & `pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/sequence_operators.py` & `pypdb-2.3/pypdb/clients/search/operators/sequence_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/sequence_operators_test.py` & `pypdb-2.3/pypdb/clients/search/operators/sequence_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/structure_operators.py` & `pypdb-2.3/pypdb/clients/search/operators/structure_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/structure_operators_test.py` & `pypdb-2.3/pypdb/clients/search/operators/structure_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/operators/text_operators.py` & `pypdb-2.3/pypdb/clients/search/operators/text_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,16 @@
     negation: bool = False
 
     def _to_dict(self) -> Dict[str, Any]:
         return {
             "operator": "range",
             "attribute": self.attribute,
             "negation": self.negation,
-            "value": [self.from_value, self.to_value]
+            "value": {"from": self.from_value,
+                      "to": self.to_value},
         }
 
 
 @dataclass
 class ExistsOperator:
     attribute: str
```

### Comparing `pypdb-2.2/pypdb/clients/search/operators/text_operators_test.py` & `pypdb-2.3/pypdb/clients/search/operators/text_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/clients/search/search_client.py` & `pypdb-2.3/pypdb/clients/search/search_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,15 +128,16 @@
 
 
 def perform_search(
     search_operator: SearchOperator,
     return_type: ReturnType = ReturnType.ENTRY,
     request_options: Optional[RequestOptions] = None,
     return_with_scores: bool = False,
-    return_raw_json_dict: bool = False
+    return_raw_json_dict: bool = False,
+    verbosity: bool = True,
 ) -> Union[List[str], List[ScoredResult], RawJSONDictResponse]:
     """Performs search specified by `search_operator`.
     Returns entity strings of type `return_type` that match the resulting hits.
 
     Strictly a subset of the functionality exposed in
     `perform_search_with_graph`, this function does not support searching on
     multiple conditions at once.
@@ -152,14 +153,15 @@
         return_with_scores: Whether or not to return the entity results with
             their associated scores. For example, you might want to do this to
             get
             the top X hits that are similar to a certain protein sequence.
             (if this is true, returns List[ScoredResult] instead of List[str])
         return_raw_json_dict: If True, this function returns the raw JSON
             response from RCSB, instead of a
+        verbosity: Print out the search query to the console (default: True)
 
     Returns:
         List of entity ids, corresponding to entities that match the given
         query.
 
         If `return_with_scores=True`, returns a list of ScoredResult instead.
         If `return_raw_json_dict=True`, returns the raw JSON response from RCSB.
@@ -180,28 +182,30 @@
     ```
     """
 
     return perform_search_with_graph(query_object=search_operator,
                                      return_type=return_type,
                                      request_options=request_options,
                                      return_with_scores=return_with_scores,
-                                     return_raw_json_dict=return_raw_json_dict)
+                                     return_raw_json_dict=return_raw_json_dict,
+                                     verbosity=verbosity)
 
 
 _SEARCH_OPERATORS = text_operators.TEXT_SEARCH_OPERATORS + [
     SequenceOperator, StructureOperator, SeqMotifOperator
 ]
 
 
 def perform_search_with_graph(
     query_object: Union[SearchOperator, QueryGroup],
     return_type: ReturnType = ReturnType.ENTRY,
     request_options: Optional[RequestOptions] = None,
     return_with_scores: bool = False,
-    return_raw_json_dict: bool = False
+    return_raw_json_dict: bool = False,
+    verbosity: bool = True,
 ) -> Union[List[str], RawJSONDictResponse, List[ScoredResult]]:
     """Performs specified search using RCSB's search node logic.
 
     Essentially, this allows you to ask multiple questions in one RCSB query.
 
     For example, you can ask for structures that satisfy all of the following
     conditions at once:
@@ -218,14 +222,15 @@
             object corresponding to the desired search.
         return_type: Type of entities to return.
         return_with_scores: Whether or not to return the entity results with
             their associated scores. For example, you might want to do this to
             get the top X hits that are similar to a certain protein sequence.
         return_raw_json_dict: Whether to return raw JSON response.
             (for example, to analyze the scores of various matches)
+        verbosity: Print out the search query to the console (default: True)
 
     Returns:
         List of strings, corresponding to hits in the database. Will be of the
         format specified by the `return_type`.
 
         If `return_with_scores=True`, returns a list of ScoredResult instead.
         If `return_raw_json_dict=True`, returns the raw JSON response from RCSB.
@@ -243,16 +248,17 @@
 
     rcsb_query_dict = {
         "query": cast_query_object._to_dict(),
         "request_options": request_options_dict,
         "return_type": return_type.value
     }
 
-    print("Querying RCSB Search using the following parameters:\n %s \n" %
-          json.dumps(rcsb_query_dict))
+    if verbosity:
+        print("Querying RCSB Search using the following parameters:\n %s \n" %
+              json.dumps(rcsb_query_dict))
 
     response = requests.post(url=SEARCH_URL_ENDPOINT,
                              data=json.dumps(rcsb_query_dict))
 
     # If your search queries are failing here, it could be that your attribute
     # doesn't support the SearchOperator you're using.
     # See: https://search.rcsb.org/search-attributes.html
```

### Comparing `pypdb-2.2/pypdb/clients/search/search_client_test.py` & `pypdb-2.3/pypdb/clients/search/search_client_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/pypdb.py` & `pypdb-2.3/pypdb/pypdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
     Gilpin, W. "PyPDB: A Python API for the Protein Data Bank."
     Bioinformatics, Oxford Journals, 2015.
 
 '''
 from collections import OrderedDict, Counter
 from itertools import repeat, chain
-import requests
 import time
 import re
 import json
 import warnings
 
 from pypdb.util import http_requests
 from pypdb.clients.fasta import fasta_client
@@ -135,14 +134,17 @@
             query_subtype = "author"
         elif query_type == "OrganismQuery":
             query_type = "text"
             query_subtype = "organism"
         elif query_type == "pfam":
             query_type = "text"
             query_subtype = "pfam"
+        elif query_type == "uniprot":
+            query_type = "text"
+            query_subtype = "uniprot"
         else:
             query_subtype = None
 
         assert query_type in {
             "full_text", "text", "structure", "sequence", "seqmotif", "chemical"
         }, "Query type %s not recognized." % query_type
 
@@ -254,14 +256,22 @@
                     query_params['parameters'] = {
                         "operator": "exact_match",
                         "negation": False,
                         "value": str(search_term),
                         "attribute":
                         "rcsb_polymer_entity_annotation.annotation_id"
                     }
+                if query_subtype == "uniprot":
+                    query_params['parameters'] = {
+                        "operator": "exact_match",
+                        "negation": False,
+                        "value": str(search_term),
+                        "attribute": 
+                        "rcsb_polymer_entity_container_identifiers.reference_sequence_identifiers.database_accession"
+                        }
 
             self.scan_params = dict()
             self.scan_params["query"] = query_params
             self.scan_params["return_type"] = return_type
             self.scan_params["request_options"] = {"results_verbosity": "verbose"} # v2
 
             if return_type == "entry":
@@ -485,61 +495,55 @@
     """
 
     warnings.warn(
         "The `get_pdb_file` function within pypdb.py is deprecated."
         "See `pypdb/clients/pdb/pdb_client.py` for a near-identical "
         "function to use", DeprecationWarning)
 
-    if filetype is 'pdb':
+    if filetype == 'pdb':
         filetype_enum = pdb_client.PDBFileType.PDB
-    elif filetype is 'cif':
+    elif filetype == 'cif':
         filetype_enum = pdb_client.PDBFileType.CIF
-    elif filetype is 'xml':
+    elif filetype == 'xml':
         filetype_enum = pdb_client.PDBFileType.XML
-    elif filetype is 'structfact':
+    elif filetype == 'structfact':
         filetype_enum = pdb_client.PDBFileType.STRUCTFACT
     else:
         warnings.warn(
             "Filetype specified to `get_pdb_file` appears to be invalid")
 
     return pdb_client.get_pdb_file(pdb_id, filetype_enum, compression)
 
 
 # https://data.rcsb.org/migration-guide.html#chem-comp-description
-# def describe_chemical(chem_id):
+def describe_chemical(chem_id):
 #     """
 
 #     Parameters
 #     ----------
 
 #     chem_id : string
-#         A 4 character string representing the full chemical sequence of interest (ie, NAG)
+#         A 3 character string representing the full chemical sequence of interest (ie, NAG)
 
 #     Returns
 #     -------
 
 #     out : dict
 #         A dictionary containing the chemical description associated with the PDB ID
 
 #     Examples
 #     --------
 #     >>> chem_desc = describe_chemical('NAG')
-#     >>> print(chem_desc)
-#     {'describeHet': {'ligandInfo': {'ligand': {'@molecularWeight': '221.208',
-#     'InChIKey': 'OVRNDRQMDRJTHS-FMDGEEDCSA-N', '@type': 'D-saccharide',
-#     'chemicalName': 'N-ACETYL-D-GLUCOSAMINE', '@chemicalID': 'NAG',
-#     'smiles': 'CC(=O)N[C@@H]1[C@H]([C@@H]([C@H](O[C@H]1O)CO)O)O', '
-#     InChI': 'InChI=1S/C8H15NO6/c1-3(11)9-5-7(13)6(12)4(2-10)15-8(5)14/
-#     h4-8,10,12-14H,2H2,1H3,(H,9,11)/t4-,5-,6-,7-,8-/m1/s1',
-#     'formula': 'C8 H15 N O6'}}}}
-
+#     >>> print(chem_desc["rcsb_chem_comp_descriptor"]["smiles"])
+#     'CC(=O)NC1C(C(C(OC1O)CO)O)O'
 #     """
-#     out = get_info(chem_id, url_root = 'http://www.rcsb.org/pdb/rest/describeHet?chemicalID=')
-#     out = to_dict(out)
-#     return out
+    if (len(chem_id) > 3):
+        raise Exception("Ligand id with more than 3 characters provided")
+
+    return get_info(chem_id, url_root = 'https://data.rcsb.org/rest/v1/core/chemcomp/')
 
 # def get_ligands(pdb_id):
 #     """Return ligands of given PDB ID
 
 #     Parameters
 #     ----------
 
@@ -649,15 +653,15 @@
 
 #     url_root = 'http://www.rcsb.org/pdb/rest/sequenceCluster?structureId='
 #     out = get_info(pdb_id_chain, url_root = url_root)
 #     out = to_dict(out)
 #     return remove_at_sign(out['sequenceCluster'])
 
 
-def get_blast(pdb_id, chain_id='A', identity_cutoff=0.99):
+def get_blast(pdb_id, chain_id='A', identity_cutoff=0.99, verbosity=True):
     """
     ---
     WARNING: this function is deprecated and slated to be deleted due to RCSB
     API changes.
 
     See `pypdb/clients/search/EXAMPLES.md` for examples to use a
     `SequenceOperator` search to similar effect
```

### Comparing `pypdb-2.2/pypdb/util/http_requests.py` & `pypdb-2.3/pypdb/util/http_requests.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb/util/test_http_requests.py` & `pypdb-2.3/pypdb/util/test_http_requests.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.2/pypdb.egg-info/SOURCES.txt` & `pypdb-2.3/pypdb.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,36 @@
 pypdb.egg-info/SOURCES.txt
 pypdb.egg-info/dependency_links.txt
 pypdb.egg-info/requires.txt
 pypdb.egg-info/top_level.txt
 pypdb.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
 pypdb/clients/__init__.py
 pypdb/clients/data/__init__.py
+pypdb/clients/data/data_types.py
+pypdb/clients/data/test_data_types.py
+pypdb/clients/data/graphql/__init__.py
+pypdb/clients/data/graphql/graphql.py
+pypdb/clients/data/graphql/test_graphql.py
 pypdb/clients/fasta/__init__.py
 pypdb/clients/fasta/fasta_client.py
 pypdb/clients/fasta/fasta_client_test.py
 pypdb/clients/pdb/__init__.py
 pypdb/clients/pdb/pdb_client.py
 pypdb/clients/pdb/pdb_client_test.py
 pypdb/clients/search/__init__.py
 pypdb/clients/search/search_client.py
 pypdb/clients/search/search_client_test.py
+pypdb/clients/search/operators/__init__.py
 pypdb/clients/search/operators/chemical_operators.py
 pypdb/clients/search/operators/chemical_operators_test.py
 pypdb/clients/search/operators/seqmotif_operators.py
 pypdb/clients/search/operators/seqmotif_operators_test.py
 pypdb/clients/search/operators/sequence_operators.py
 pypdb/clients/search/operators/sequence_operators_test.py
 pypdb/clients/search/operators/structure_operators.py
 pypdb/clients/search/operators/structure_operators_test.py
 pypdb/clients/search/operators/text_operators.py
 pypdb/clients/search/operators/text_operators_test.py
 pypdb/util/__init__.py
 pypdb/util/http_requests.py
-pypdb/util/test_http_requests.py
+pypdb/util/test_http_requests.py
+tests/test_pypdb.py
```

### Comparing `pypdb-2.2/setup.py` & `pypdb-2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 modules_list = [
     "pypdb",
     "pypdb.util",
     "pypdb.clients",
     "pypdb.clients.search",
     "pypdb.clients.search.operators",
     "pypdb.clients.data",
+    "pypdb.clients.data.graphql",
     "pypdb.clients.fasta",
     "pypdb.clients.pdb",
 ]
 
 setup(
     name='pypdb',
     packages=modules_list,  # same as 'name'
     py_modules=modules_list,
-    version='2.02',
-    install_requires=['requests'],
+    version='2.03',
+    install_requires=['requests', 'pandas'],
     description='A Python wrapper for the RCSB Protein Data Bank (PDB) API',
     author='William Gilpin',
     author_email='firstnamelastname@gmail.com',
     url='https://github.com/williamgilpin/pypdb',
     download_url='https://github.com/williamgilpin/pypdb/tarball/0.6',
     keywords=['protein', 'data', 'RESTful', 'api'],
     classifiers=[],
```

