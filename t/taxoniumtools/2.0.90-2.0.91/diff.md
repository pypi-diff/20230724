# Comparing `tmp/taxoniumtools-2.0.90.tar.gz` & `tmp/taxoniumtools-2.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxoniumtools-2.0.90.tar", last modified: Fri Dec 30 19:07:54 2022, max compression
+gzip compressed data, was "taxoniumtools-2.0.91.tar", last modified: Sat Feb 11 12:48:17 2023, max compression
```

## Comparing `taxoniumtools-2.0.90.tar` & `taxoniumtools-2.0.91.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:54.730639 taxoniumtools-2.0.90/
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2022-12-30 19:07:54.730639 taxoniumtools-2.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      250 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      968 2022-12-30 19:07:54.730639 taxoniumtools-2.0.90/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:54.726639 taxoniumtools-2.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:54.726639 taxoniumtools-2.0.90/src/taxoniumtools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      162 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     6207 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/newick_to_taxonium.py
--rw-r--r--   0 runner    (1001) docker     (116)    15575 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/parsimony_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    11960 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/usher_to_taxonium.py
--rw-r--r--   0 runner    (1001) docker     (116)    15138 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/ushertools.py
--rw-r--r--   0 runner    (1001) docker     (116)     8248 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4640 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/src/taxoniumtools/view_taxonium.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:54.726639 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      731 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      183 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       99 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-12-30 19:07:54.000000 taxoniumtools-2.0.90/src/taxoniumtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 19:07:54.730639 taxoniumtools-2.0.90/test_data/
--rw-r--r--   0 runner    (1001) docker     (116)    69027 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/hu1.gb
--rw-r--r--   0 runner    (1001) docker     (116)   972124 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/mpox.pb
--rw-r--r--   0 runner    (1001) docker     (116)   200115 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/mpox_ref.fasta
--rw-r--r--   0 runner    (1001) docker     (116)       59 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/test.nwk
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/test_config.json
--rw-r--r--   0 runner    (1001) docker     (116)    22301 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/tfci.meta.tsv.gz
--rw-r--r--   0 runner    (1001) docker     (116)   323279 2022-12-30 19:07:40.000000 taxoniumtools-2.0.90/test_data/tfci.pb
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1348 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      968 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-11 12:48:17.366550 taxoniumtools-2.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/src/taxoniumtools/
+-rw-r--r--   0 runner    (1001) docker     (116)       51 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6207 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/newick_to_taxonium.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15575 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/parsimony_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11960 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/usher_to_taxonium.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15284 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/ushertools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8248 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4640 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/src/taxoniumtools/view_taxonium.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      731 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-11 12:48:17.000000 taxoniumtools-2.0.91/src/taxoniumtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-11 12:48:17.370550 taxoniumtools-2.0.91/test_data/
+-rw-r--r--   0 runner    (1001) docker     (116)    69027 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/hu1.gb
+-rw-r--r--   0 runner    (1001) docker     (116)   972124 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/mpox.pb
+-rw-r--r--   0 runner    (1001) docker     (116)   200115 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/mpox_ref.fasta
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/test.nwk
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (116)    22301 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/tfci.meta.tsv.gz
+-rw-r--r--   0 runner    (1001) docker     (116)   323279 2023-02-11 12:48:07.000000 taxoniumtools-2.0.91/test_data/tfci.pb
```

### Comparing `taxoniumtools-2.0.90/PKG-INFO` & `taxoniumtools-2.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxoniumtools
-Version: 2.0.90
+Version: 2.0.91
 Summary: Generate files for taxonium
 Home-page: https://github.com/theosanderson/taxonium
 Author: Theo Sanderson
 Author-email: theo@theo.io
 Project-URL: Bug Tracker, https://github.com/theosanderson/taxonium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `taxoniumtools-2.0.90/README.md` & `taxoniumtools-2.0.91/README.md`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/setup.cfg` & `taxoniumtools-2.0.91/setup.cfg`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/newick_to_taxonium.py` & `taxoniumtools-2.0.91/src/taxoniumtools/newick_to_taxonium.py`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/parsimony_pb2.py` & `taxoniumtools-2.0.91/src/taxoniumtools/parsimony_pb2.py`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/usher_to_taxonium.py` & `taxoniumtools-2.0.91/src/taxoniumtools/usher_to_taxonium.py`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/ushertools.py` & `taxoniumtools-2.0.91/src/taxoniumtools/ushertools.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,23 +230,27 @@
 
         self.annotate_mutations()
         self.annotate_clades(clade_types)
 
         self.expand_condensed_nodes()
         self.assign_num_tips()
         print(f"Loaded initial tree with {self.tree.root.num_tips} tips")
+        print("Ending early")
+        if genbank_file:
+            # We need to reconstruct root seq before shearing as shearing can mess it up
+
+            self.load_genbank_file(genbank_file)
+            self.get_root_sequence()
         if shear:
             print("Shearing tree...")
             self.shear_tree(shear_threshold)
         self.assign_num_tips()
         print(f"Tree to use now has {self.tree.root.num_tips} tips")
         self.set_branch_lengths()
         if genbank_file:
-            self.load_genbank_file(genbank_file)
-            self.get_root_sequence()
             self.perform_aa_analysis()
 
     def prune_node(self, node_to_prune):
         """Remove node from parent, then check if parent has zero descendants. If so remove it.
         If parent has a single descendant, then give the parent's mutations to the descendant, unless they
         conflict with the descendants own mutations. Also give the parent's clade annotations to the descendant,
         unless they conflict. Then prune the parent, and instead add this child to parent's parent."""
@@ -287,14 +291,15 @@
         """Hacky way of recording the root sequence"""
         ref_muts = []
         for i, character in enumerate(self.root_sequence):
             ref_muts.append(
                 NucMutation(one_indexed_position=i + 1,
                             mut_nuc=character,
                             par_nuc="X"))
+
         return ref_muts
 
     def annotate_clades(self, clade_types):
         if clade_types:
             for i, node in alive_it(list(
                     enumerate(preorder_traversal(self.tree.root))),
                                     title="Annotating clades"):
```

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/utils.py` & `taxoniumtools-2.0.91/src/taxoniumtools/utils.py`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools/view_taxonium.py` & `taxoniumtools-2.0.91/src/taxoniumtools/view_taxonium.py`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools.egg-info/PKG-INFO` & `taxoniumtools-2.0.91/src/taxoniumtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxoniumtools
-Version: 2.0.90
+Version: 2.0.91
 Summary: Generate files for taxonium
 Home-page: https://github.com/theosanderson/taxonium
 Author: Theo Sanderson
 Author-email: theo@theo.io
 Project-URL: Bug Tracker, https://github.com/theosanderson/taxonium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `taxoniumtools-2.0.90/src/taxoniumtools.egg-info/SOURCES.txt` & `taxoniumtools-2.0.91/src/taxoniumtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/test_data/hu1.gb` & `taxoniumtools-2.0.91/test_data/hu1.gb`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/test_data/mpox.pb` & `taxoniumtools-2.0.91/test_data/mpox.pb`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/test_data/mpox_ref.fasta` & `taxoniumtools-2.0.91/test_data/mpox_ref.fasta`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/test_data/tfci.meta.tsv.gz` & `taxoniumtools-2.0.91/test_data/tfci.meta.tsv.gz`

 * *Files identical despite different names*

### Comparing `taxoniumtools-2.0.90/test_data/tfci.pb` & `taxoniumtools-2.0.91/test_data/tfci.pb`

 * *Files identical despite different names*

