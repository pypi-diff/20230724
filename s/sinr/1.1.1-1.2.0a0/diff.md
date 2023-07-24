# Comparing `tmp/sinr-1.1.1.tar.gz` & `tmp/sinr-1.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinr-1.1.1.tar", max compression
+gzip compressed data, was "sinr-1.2.0a0.tar", max compression
```

## Comparing `sinr-1.1.1.tar` & `sinr-1.2.0a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    21782 2023-02-15 12:35:06.708647 sinr-1.1.1/LICENSE
--rw-r--r--   0        0        0     5534 2023-02-20 11:47:45.914651 sinr-1.1.1/README.rst
--rw-r--r--   0        0        0     2436 2023-02-15 12:35:06.756647 sinr-1.1.1/build.py
--rw-r--r--   0        0        0     1802 2023-02-20 11:54:07.527979 sinr-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      152 2023-01-09 14:49:38.151957 sinr-1.1.1/sinr/__init__.py
--rw-r--r--   0        0        0    38394 2023-02-18 13:10:10.312731 sinr-1.1.1/sinr/graph_embeddings.py
--rw-r--r--   0        0        0     1039 2023-02-15 12:43:35.422387 sinr-1.1.1/sinr/how_to_install.md
--rw-r--r--   0        0        0      315 2023-01-09 14:49:38.155957 sinr-1.1.1/sinr/logger.py
--rw-r--r--   0        0        0     4333 2023-02-15 15:26:52.019336 sinr-1.1.1/sinr/nfm.py
--rw-r--r--   0        0        0     1161 2023-02-15 15:25:29.531064 sinr-1.1.1/sinr/strategy_loader.py
--rw-r--r--   0        0        0       47 2023-02-16 12:55:30.828198 sinr-1.1.1/sinr/tests/__init__.py
--rw-r--r--   0        0        0     2213 2023-01-09 14:49:38.167957 sinr-1.1.1/sinr/tests/test_sinr_nfm.py
--rw-r--r--   0        0        0     5086 2023-01-09 14:49:38.167957 sinr-1.1.1/sinr/tests/test_sinr_workflow.py
--rw-r--r--   0        0        0       88 2023-02-16 12:55:17.388156 sinr-1.1.1/sinr/text/__init__.py
--rw-r--r--   0        0        0     2300 2023-02-15 15:26:31.983270 sinr-1.1.1/sinr/text/cooccurrence.py
--rwxr-xr-x   0        0        0   211128 2023-02-20 11:52:20.000000 sinr-1.1.1/sinr/text/cooccurrence_cython.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0        0        0     9181 2023-02-15 15:26:31.979270 sinr-1.1.1/sinr/text/cooccurrence_cython.pyx
--rw-r--r--   0        0        0     4808 2023-02-16 13:00:59.689232 sinr-1.1.1/sinr/text/pmi.py
--rw-r--r--   0        0        0     9725 2023-02-16 10:59:41.630259 sinr-1.1.1/sinr/text/preprocess.py
--rw-r--r--   0        0        0     1927 2023-02-17 14:31:46.228438 sinr-1.1.1/sinr/viz.py
--rw-r--r--   0        0        0     7230 1970-01-01 00:00:00.000000 sinr-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    21782 2023-07-24 14:32:45.854405 sinr-1.2.0a0/LICENSE
+-rw-r--r--   0        0        0     5534 2023-07-24 14:32:45.854405 sinr-1.2.0a0/README.rst
+-rw-r--r--   0        0        0     2436 2023-07-24 14:32:45.854405 sinr-1.2.0a0/build.py
+-rw-r--r--   0        0        0     2038 2023-07-24 14:33:01.210423 sinr-1.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-07-24 14:33:01.226423 sinr-1.2.0a0/sinr/__init__.py
+-rw-r--r--   0        0        0    48483 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/graph_embeddings.py
+-rw-r--r--   0        0        0     1039 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/how_to_install.md
+-rw-r--r--   0        0        0      315 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/logger.py
+-rw-r--r--   0        0        0     4333 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/nfm.py
+-rw-r--r--   0        0        0     1161 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/strategy_loader.py
+-rw-r--r--   0        0        0       88 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/cooccurrence.py
+-rw-r--r--   0        0        0     9181 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/cooccurrence_cython.pyx
+-rw-r--r--   0        0        0     7346 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/evaluate.py
+-rw-r--r--   0        0        0    17185 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/exception_for_similarity.txt
+-rw-r--r--   0        0        0     4494 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/exceptions_for_categorization.txt
+-rw-r--r--   0        0        0    19605 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/exceptions_for_evaluation.txt
+-rw-r--r--   0        0        0     4808 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/pmi.py
+-rw-r--r--   0        0        0     9492 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/text/preprocess.py
+-rw-r--r--   0        0        0     1927 2023-07-24 14:32:45.882406 sinr-1.2.0a0/sinr/viz.py
+-rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 sinr-1.2.0a0/PKG-INFO
```

### Comparing `sinr-1.1.1/LICENSE` & `sinr-1.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/README.rst` & `sinr-1.2.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/build.py` & `sinr-1.2.0a0/build.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/pyproject.toml` & `sinr-1.2.0a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "numpy~=1.24.2",
   "wheel"
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sinr"
-version = "1.1.1"
+version = "v1.2.0-alpha"
 description = "Build word and graph embeddings based on community detection in graphs."
 authors = ["Thibault Prouteau <thibault.prouteau@univ-lemans.fr>", "Nicolas Dugue <nicolas.dugue@univ-lemans.fr>", " Simon Guillot <simon.guillot@univ-lemans.fr>", "Anthony Perez"]
 license = "CeCILL 2.1"
 homepage = "https://sinr-embeddings.github.io/sinr/_build/html/index.html"
 repository = "https://github.com/SINr-Embeddings/sinr"
 keywords = ["node embedding", "word embedding", "embedding", "graph embedding", "louvain", "community"]
 classifiers = [
@@ -48,26 +48,35 @@
 pandas = "<=1.3.5"
 tabulate = "^0.9.0"
 leidenalg = "^0.9.1"
 igraph = "^0.10.4"
 matplotlib = "^3.7.0"
 spacy = "^3.5.0"
 
+[tool.poetry.extras]
+docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon", "sphinx-tabs"]
+
 
 [tool.poetry.group.dev.dependencies]
 nltk = "^3.8.1"
 networkx = "<2.7"
 cython = "^0.29.21"
 karateclub = "^1.3.3"
 pyment = "^0.3.3"
 xgboost = "^1.7.3"
 torch = "^1.13.1"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 sphinx-tabs = "^3.4.1"
+plotly = "^5.13.1"
+
+
 
 
+[tool.poetry.group.exp.dependencies]
+openpyxl = "^3.1.2"
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = false
 
+[tool.poetry_bumpversion.file."sinr/__init__.py"]
```

### Comparing `sinr-1.1.1/sinr/graph_embeddings.py` & `sinr-1.2.0a0/sinr/graph_embeddings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import pickle as pk
 
-from networkit import Graph, components, community, setNumberOfThreads, Partition
-from numpy import argpartition, argsort, asarray, where, nonzero
+from networkit import Graph, components, community, setNumberOfThreads, getCurrentNumberOfThreads, getMaxNumberOfThreads, Partition
+from numpy import argpartition, argsort, asarray, where, nonzero, concatenate, repeat, mean, nanmax
 from sklearn.neighbors import NearestNeighbors
 from scipy import spatial
+from scipy.sparse import csr_matrix
+import sklearn.preprocessing as skp
+from tqdm.auto import tqdm
+from functools import partialmethod
+from math import ceil
+import time
+import os
 
 from . import strategy_loader
 from .logger import logger
 from .nfm import get_nfm_embeddings
+import sinr.text.evaluate as ev
 
 
 class SINr(object):
     """Object that can be used to extract word or graph embeddings using the SINr approach.
     This object cannot then be used to inspect the resulting vectors. Instead, using the ModelBuilder class, a SINrVectors object should be created that will allow to use the resulting vectors.
     
     ...
@@ -19,58 +27,59 @@
 
     Attributes
     ----------
     Attributes should not be read
     """
 
     @classmethod
-    def load_from_cooc_pkl(cls, cooc_matrix_path, n_jobs=1):
+    def load_from_cooc_pkl(cls, cooc_matrix_path, n_jobs=-1):
         """Build a sinr object from a co-occurrence matrix stored as a pickle : useful to deal with textual data.
         Co-occurrence matrices should for instance be generated using sinr.text.cooccurrence
 
         :param cooc_matrix_path: Path to the cooccurrence matrix generated using sinr.text.cooccurrence : the file should be a pickle
         :type cooc_matrix_path: string
-        :param n_jobs: Number of jobs that should be used The default is 1.
+        :param n_jobs: Number of jobs that should be used The default is -1.
         :type n_jobs: int, optional
 
         
         """
         logger.info("Building Graph.")
 
         word_to_idx, matrix = strategy_loader.load_pkl_text(cooc_matrix_path)
         graph = get_graph_from_matrix(matrix)
         out_of_LgCC = get_lgcc(graph)
         logger.info("Finished building graph.")
         return cls(graph, out_of_LgCC, word_to_idx)
 
     @classmethod
-    def load_from_adjacency_matrix(cls, matrix_object, n_jobs=1):
+    def load_from_adjacency_matrix(cls, matrix_object, labels=None, n_jobs=-1):
         """Build a sinr object from an adjacency matrix as a sparse one (csr)
 
         :param matrix_object: Matrix describing the graph.
         :type matrix_object: csr_matrix
-        :param n_jobs: Number of jobs that should be used The default is 1.
+        :param labels:  (Default value = None)
+        :param n_jobs: Number of jobs that should be used The default is -1.
         :type n_jobs: int, optional
 
         
         """
         logger.info("Building Graph.")
-        word_to_idx, matrix = strategy_loader.load_adj_mat(matrix_object)
+        word_to_idx, matrix = strategy_loader.load_adj_mat(matrix_object, labels)
         graph = get_graph_from_matrix(matrix)
         out_of_LgCC = get_lgcc(graph)
         logger.info("Finished building graph.")
         return cls(graph, out_of_LgCC, word_to_idx)
 
     @classmethod
-    def load_from_graph(cls, graph, n_jobs=1):
+    def load_from_graph(cls, graph, n_jobs=-1):
         """Build a sinr object from a networkit graph object
 
         :param graph: Networkit graph object.
         :type graph: networkit
-        :param n_jobs: Number of jobs that should be used The default is 1.
+        :param n_jobs: Number of jobs that should be used The default is -1.
         :type n_jobs: int, optional
 
         
         """
         word_to_idx = dict()
         idx = 0
         for u in graph.iterNodes():
@@ -84,35 +93,36 @@
         """Runs the training of the embedding, i.e. community detection + vectors extraction
 
         :param algo: Community detection algorithm. The default, None allorws to run a Louvain algorithm
         :type algo: networkit.algo.community, optional
 
         
         """
-        if algo is None:
-            algo = community.PLM(self.cooc_graph, refine=False, gamma=1, turbo=True, recurse=False)
         self.communities = self.detect_communities(self.cooc_graph, algo=algo)
         self.extract_embeddings(communities=self.communities)
 
-    def detect_communities(self, gamma=100, algo=None, inspect=True):
+    def detect_communities(self, gamma=1, algo=None, inspect=True, par="balanced"):
         """Runs community detection on the graph
 
-        :param gamma: For Louvain algorithm which is the default algorithm (ignore this parameter if param algo is used), allows to control the size of the communities. The greater it is, the smaller the communities. The default is 100.
+        :param gamma: For Louvain algorithm which is the default algorithm (ignore this parameter if param algo is used), allows to control the size of the communities. The greater it is, the smaller the communities. The default is 1.
         :type gamma: int, optional
         :param algo: Community detection algorithm. The default, None allorws to run a Louvain algorithm
         :type algo: networkit.algo.community, optional
         :param inspect: Whether or not one wants to get insight about the communities extracted. The default is True.
         :type inspect: boolean, optional
+        :param par: Parallelisation strategy for networkit community detection (Louvain), see https://networkit.github.io/dev-docs/python_api/community.html#networkit.community.PLM for more details, "none randomized" allows randomness in Louvain in single thread mode. To force determinism pass the "none" parallelisation strategy. The default is balanced.
 
         
         """
         logger.info("Detecting communities.")
         print(f"Gamma for louvain : {gamma}")
+        if getMaxNumberOfThreads() == 1 and par!="none randomized":
+            logger.warning(f"""The current number of threads is set to {getMaxNumberOfThreads()} with parallelization strategy {par}. Nodes will not be randomized in Louvain. Consider using more threads by resetting the setNumberOfThreads parameter of networkit or use the 'none randomized' parallelization strategy.""")
         if algo is None:
-            algo = community.PLM(self.cooc_graph, refine=False, gamma=gamma, turbo=True, recurse=False)
+            algo = community.PLM(self.cooc_graph, refine=False, gamma=gamma, turbo=True, recurse=False, par=par)
         communities = community.detectCommunities(self.cooc_graph, algo=algo, inspect=inspect)
         communities.compact(useTurbo=True)  # Consecutive communities from 0 to number of communities - 1
         self.communities = communities
         logger.info("Finished detecting communities.")
         return communities
 
     def size_of_voc(self):
@@ -166,43 +176,48 @@
         np, nr, nfm = get_nfm_embeddings(self.cooc_graph, self.communities.getVector(), self.n_jobs)
         self.np = np
         self.nr = nr
         self.nfm = nfm
         logger.info("NFM successfully applied.")
         logger.info("Finished extracting embeddings.")
 
-    def __init__(self, graph, lgcc, wrd_to_idx, n_jobs=1):
+    def __init__(self, graph, lgcc, wrd_to_idx, n_jobs=-1):
         """Should not be used ! Some factory methods below starting with "load_" should be used instead.
 
         Parameters
         ----------
         graph : networkit graph
         lgcc : networkit graph
             the largest connected component of graph
         wrd_to_idx : dict
             A matching between a vocabulary and ids. Useful for text. Otherwise, the vocabulary and the ids are the same
         n_jobs : int, optional
-            Number of jobs that should be runned. The default is 1
+            Number of jobs that should be runned. The default is -1, all available threads
 
         Returns
         -------
         None.
 
         """
         self.nfm = None
         self.nr = None
         self.np = None
         self.communities = None
         self.n_jobs = n_jobs
-        setNumberOfThreads(n_jobs)
         self.wrd_to_idx = wrd_to_idx
         self.idx_to_wrd = _flip_keys_values(self.wrd_to_idx)
         self.cooc_graph = graph
         self.out_of_LgCC = lgcc
 
+        assert type(n_jobs) == int, "n_jobs must be of type int"
+        assert n_jobs == -1 or n_jobs>0, "Value for n_jobs must be -1 or greater than 0"
+
+        if n_jobs > 0:
+            setNumberOfThreads(n_jobs)
+
         self.wd_before, self.wd_after = None, None
 
     def get_out_of_LgCC_coms(self, communities):
         """Get communities that are not in the Largest Connected Component (LgCC).
 
         :param communities: Partition object of the communities as obtained by calling a Networkit community detection algorithm
         :type communities: Partition
@@ -312,26 +327,26 @@
 
 
     Attributes
     ----------
     Attributes should not be read
     """
 
-    def __init__(self, sinr, name, n_jobs=1, n_neighbors=31):
+    def __init__(self, sinr, name, n_jobs=-1, n_neighbors=31):
         """
         Creating a ModelBuilder object to build a `SINrVectors`.
 
         Parameters
         ----------
         sinr : SINr
             A SINr object with extracted vectors
         name : string
             Name of the model
         n_jobs : int, optional
-            DESCRIPTION. The default is 1.
+            DESCRIPTION. The default is -1, all the available threads.
         n_neighbors : int, optional
             Number of neighbors to use for similarity. The default is 31.
 
         """
         self.sinr = sinr
         self.model = SINrVectors(name, n_jobs, n_neighbors)
 
@@ -551,20 +566,20 @@
 class SINrVectors(object):
     """After training word or graph embeddings using SINr object, use the ModelBuilder object to build `SINrVectors`.
     `SINrVectors` is the object to manipulate the model, explore the embedding space and its interpretability
 
     """
     labels: bool
 
-    def __init__(self, name, n_jobs=1, n_neighbors=20):
+    def __init__(self, name, n_jobs=-1, n_neighbors=20):
         """
         Initializing `SINr` vectors objets
         :param name: name of the model, useful to save it
         :type name: str
-        :param n_jobs: number of jobs to use (k-nearest neighbors to obtain most similar words or nodes)
+        :param n_jobs: number of jobs to use (k-nearest neighbors to obtain most similar words or nodes), defaluts to -1
         :type n_jobs: int
         :param n_neighbors: number of neighbors to consider when querying the most similar words or nodes
         :type n_neighbors: int
         """
         self.G = None
         self.communities_sets = None
         self.community_membership = None
@@ -713,14 +728,233 @@
         nb_coms = max(self.community_membership)
         self.communities_sets = []
         for i in range(nb_coms + 1):
             self.communities_sets.append(set())
         for idx, com in enumerate(self.community_membership):
             self.communities_sets[com].add(idx)
 
+    def sparsify(self, k):
+
+        """Sparsify the vectors keeping activated the top k dimensions
+        
+        :param k: int
+        
+        """
+    
+        data = list()
+        rows = list()
+        cols = list()
+    
+        m_shape = self.vectors.get_shape()
+    
+        if not self.vectors.has_sorted_indices:
+            self.vectors.sort_indices()
+    
+        for i_row in range(m_shape[0]):  
+    
+            if(i_row == 0):
+                # datas/indices of the first line
+                data_row = self.vectors.data[ 0 : self.vectors.indptr[1] - self.vectors.indptr[0]]
+                indices_row = self.vectors.indices[ 0 : self.vectors.indptr[1] - self.vectors.indptr[0]]
+            else :
+                # datas/indices of a line : data/indices[indptr[line] - indptr[0] : indptr[next_line] - indptr[0]]
+                data_row = self.vectors.data[self.vectors.indptr[i_row] - self.vectors.indptr[0] : 
+                                            self.vectors.indptr[i_row + 1] - self.vectors.indptr[0]]
+                indices_row = self.vectors.indices[self.vectors.indptr[i_row] - self.vectors.indptr[0] : 
+                                                    self.vectors.indptr[i_row + 1] - self.vectors.indptr[0]]
+                
+            # datas are sorted if the number of activated dimensions is more than k
+            # we save the top k dimensions 
+            # if there is less than k datas for the line, we keep all the datas
+            if(k < len(data_row)):
+                ind_sort = argsort(data_row)
+                
+                data = concatenate((data_row[ind_sort[len(ind_sort)-k :]], data))
+                rows = concatenate((repeat(i_row,k), rows))
+                cols = concatenate((indices_row[ind_sort[len(ind_sort)-k :]],cols))
+    
+            else:
+                data = concatenate((data_row, data))
+                rows = concatenate((repeat(i_row,len(data_row)), rows))
+                cols = concatenate((indices_row,cols))
+                
+        new_vec = csr_matrix((data, (rows, cols)), shape=m_shape)
+        
+        self.set_vectors(new_vec)
+
+    def binarize(self):
+
+        """Binarize the vectors
+        
+        """
+        
+        self.set_vectors(skp.binarize(self.vectors))
+        
+    def dim_nnz_count(self, dim):
+        """ Count the number of non zero values in a dimension.
+        :param dim: index of the dimension
+        :type dim: int
+        
+        :return: the number of non zero values in the dimension
+        :rtype: int
+        """
+        
+        d = self.vectors.getcol(dim)
+        return d.nnz
+        
+    def remove_communities_dim_nnz(self, threshold_min = None, threshold_max = None):
+        """Remove dimensions (communities) which are the less activated and those which are the most activated.
+        
+        :param threshold_min: minimal number of non zero values to have for a dimension to be kept
+        :type threshold_min: int
+        :param threshold_max: maximal number of non zero values to have for a dimension to be kept
+        :type threshold_max: int
+        
+        """
+        
+        if threshold_min != None or threshold_max != None:
+            dims = self.get_number_of_dimensions()
+            
+            ind_min = list()
+            ind_max = list()
+
+            for dim in tqdm(range(dims)):
+                if threshold_min != None:
+                    if self.dim_nnz_count(dim) < threshold_min:
+                        ind_min.append(dim)
+                if threshold_max != None:
+                    if self.dim_nnz_count(dim) > threshold_max:
+                        ind_max.append(dim)
+
+            # Remove dimensions from the matrix of embeddings
+            self.set_vectors(self.vectors[:,list(set(range(self.vectors.shape[1]))-set(ind_min + ind_max))])
+
+            # Remove communities from communities sets
+            for i in tqdm(sorted(ind_max + ind_min, reverse = True)):
+                self.communities_sets.pop(i)
+
+            # Update the communities members
+            self.community_membership = set()
+
+            for c in self.communities_sets:
+                self.community_membership = self.community_membership.union(c)
+
+            self.community_membership = sorted(list(self.community_membership))
+    
+    def dim_nnz_thresholds(self, step = 100, diff_tol = 0.005):
+        """Give the minimal and the maximal number of non zero values to have for a dimension to be kept and not lower the model's similarity. Taking into account the datasets MEN, WS353, SCWS and SimLex-999.
+        
+        :param step: step to search thresholds (default value : 100)
+        :param: diff_tol: difference of similarity tolerated with the low threshold (default value : 0.005)
+        
+        :return: thresholds (low, high)
+        :rtype: tuple of int
+        
+        """
+        
+        # Disable tqdm to clear output
+        tqdm.__init__ = partialmethod(tqdm.__init__, disable=True)
+        
+        # Copy of the sinrvectors to remove dimensions
+        name = self.name
+        name_tmp = 'vec_ref_' + str(round(time.time()*1000))
+        self.name = name_tmp
+        self.save()
+        self.name = name
+        
+        # Maximum of non zero values in dimensions
+        nnz_count = list()
+
+        for d in range(self.get_number_of_dimensions()):
+            nnz_count.append(self.dim_nnz_count(d))
+
+        max_nnz = max(nnz_count)
+        
+        print(f'Maximum of non zero values in dimensions : {max_nnz}')
+
+        # Mean similarity of vectors with all dimensions (MEN, WS353, SCWS, SimLex-999)
+        simlex999 = ev.fetch_SimLex(which='999')
+        men = ev.fetch_data_MEN()
+        ws353 = ev.fetch_data_WS353()
+        scws = ev.fetch_data_SCWS()
+
+        sim_all_dim = list()
+        sim_all_dim.append(ev.eval_similarity(self, simlex999, print_missing=False))
+        sim_all_dim.append(ev.eval_similarity(self, men, print_missing=False))
+        sim_all_dim.append(ev.eval_similarity(self, ws353, print_missing=False))
+        sim_all_dim.append(ev.eval_similarity(self, scws, print_missing=False))
+
+        sim_mean_all_dim = mean(sim_all_dim)
+        
+        print(f'Mean similarity of the model with all dimensions (MEN, WS353, SCWS, SimLex-999) : {sim_mean_all_dim}\n')
+
+        # Low threshold for the number of nnz per dimension
+        # Taking the maximal threshold (multiple of step) 
+        # for which the similarity is greater than the similarity - 0.01 of the vectors with all dimensions
+
+        sim = sim_mean_all_dim
+        seuil = 0
+
+        while(sim > sim_mean_all_dim - diff_tol and seuil + step <= max_nnz and sim != float('nan')):
+            seuil += step
+
+            vec_seuil = SINrVectors(name_tmp)
+            vec_seuil.load()
+            vec_seuil.remove_communities_dim_nnz(threshold_min = seuil)
+
+            sim_vec_seuil = list()
+
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, simlex999, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, men, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, ws353, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, scws, print_missing=False))
+            
+            sim = mean(sim_vec_seuil)
+            
+            print(str(seuil) + ' : ' + str(round(sim, 3)) + ' ', end='')
+
+        print('\n')
+        min_threshold = seuil - step
+        
+        print(f'Low threshold : {min_threshold}\n')
+
+        # High threshold for the number of nnz per dimension
+        # Taking the threshold (multiple of 10) for which the similarity is maximal
+
+        vec_seuil = SINrVectors(name_tmp)
+        vec_seuil.load()
+
+        sim = list()
+        seuils = [x for x in range(ceil(max_nnz / 1000) * 1000, 0, -step)]
+
+        for s in seuils:
+            vec_seuil.remove_communities_dim_nnz(threshold_max = s)
+
+            sim_vec_seuil = list()
+
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, simlex999, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, men, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, ws353, print_missing=False))
+            sim_vec_seuil.append(ev.eval_similarity(vec_seuil, scws, print_missing=False))
+            
+            sim.append(mean(sim_vec_seuil))
+            print(str(s) + ' : ' + str(round(mean(sim_vec_seuil), 3)) + ' ', end='')
+
+        print('\n')
+        max_threshold = seuils[sim.index(nanmax(sim))]
+        
+        print(f'High threshold : {max_threshold}\nSimilarity with high threshold : {nanmax(sim)}\n')
+        
+        tqdm.__init__ = partialmethod(tqdm.__init__, disable=False)
+        
+        # Delete the copy file
+        os.remove(name_tmp + '.pk')
+
+        return min_threshold, max_threshold
+    
     def get_community_membership(self, obj):
         """Get the community index of a node or label.
 
         :param obj: an integer of the node or of its label
         :type obj: int or str
         :returns: the community of a specific object
 
@@ -751,16 +985,16 @@
         :type obj: int or str
         :returns: the index of the object
 
         """
         if type(obj) is int:
             return obj
         index = self.vocab.index(obj) if self.labels else obj
-        return index
-
+        return index   
+        
     def most_similar(self, obj):
         """Get the most similar objects of the one passed as a parameter using the cosine of their vectors.
 
         :param obj: the object for which to fetch the nearest neighbors
         :type obj: int or str
 
         """
@@ -912,15 +1146,15 @@
 
         """
         if self.communities_sets is None:
             raise NoInterpretabilityException
         index = self._get_index(obj)
         highest_dims = self._get_topk(index, topk_dim, row=True)
         vector = self._get_vector(index, row=True)
-        highest_dims = [self.get_dimension_descriptors_idx(idx, topk_val).with_value(vector[idx]).get_dict() for idx in
+        highest_dims = [self.get_dimension_descriptors_idx(idx, topk_val).with_value().get_dict() for idx in
                         highest_dims]
         return highest_dims
 
     # Using top words to describe dimensions
     def get_dimension_stereotypes(self, obj, topk=5):
         """Get the words with the highest values on dimension obj.
 
@@ -968,15 +1202,15 @@
 
         """
         # get index of the word considered
         index = self._get_index(obj)
         # get the topk dimensions for this word
         highest_dims = self._get_topk(index, topk_dim, row=True)
         vector = self._get_vector(index, row=True)
-        highest_dims = [self.get_dimension_stereotypes_idx(idx, topk_val).with_value(vector[idx]).get_dict() for idx in
+        highest_dims = [self.get_dimension_stereotypes_idx(idx, topk_val).with_value().get_dict() for idx in
                         highest_dims]
         return highest_dims
 
     def get_obj_stereotypes_and_descriptors(self, obj, topk_dim=5, topk_val=3):
         """Get the stereotypes and descriptors for obj.
 
         :param obj: object for which to fetch stereotypes and descriptors
@@ -1041,8 +1275,8 @@
 
         """
         data={}
         for item in self.vocab :
             data[item]=self.get_my_vector(item)
         f = open(self.name + "_light.pk", 'wb')
         pk.dump(data,f)
-        f.close()
+        f.close()
```

### Comparing `sinr-1.1.1/sinr/how_to_install.md` & `sinr-1.2.0a0/sinr/how_to_install.md`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/nfm.py` & `sinr-1.2.0a0/sinr/nfm.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/strategy_loader.py` & `sinr-1.2.0a0/sinr/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/text/cooccurrence.py` & `sinr-1.2.0a0/sinr/text/cooccurrence.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/text/cooccurrence_cython.pyx` & `sinr-1.2.0a0/sinr/text/cooccurrence_cython.pyx`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/text/pmi.py` & `sinr-1.2.0a0/sinr/text/pmi.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/sinr/text/preprocess.py` & `sinr-1.2.0a0/sinr/text/preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -133,43 +133,52 @@
                                          str(token.is_digit),
                                          str(token.like_num)])
                     corpus_opened.write(f'{content}\n')  # Write the token info
                 corpus_opened.write("</s>\n")
         corpus_opened.close()
         logger.info(f"VRT-style file written in {self.corpus_output.absolute()}")
 
-
-def extract_text(corpus_path, lemmatize=True, stop_words=False, lower_words=True, number=False, punct=False,
-                 exclude_pos=[],
-                 en=True, min_freq=50, alpha=True, exclude_en=[], min_length_word=3):
+def extract_text(corpus_path, exceptions_path=None, lemmatize=True, stop_words=False, lower_words=True, number=False, punct=False, exclude_pos=[], en="chunking", min_freq=50, alpha=True, exclude_en=[], min_length_word=3):
     """Extracts the text from a VRT corpus file.
 
     :param corpus_path: str
     :param lemmatize: bool (Default value = True)
     :param stop_words: bool (Default value = False)
     :param lower: bool
     :param number: bool (Default value = False)
     :param punct: bool (Default value = False)
     :param exclude_pos: list (Default value = [])
-    :param en: bool (Default value = True)
+    :param en: str ("chunking", "tagging", "deleting") (Default value = "chunking")
     :param min_freq: int (Default value = 50)
     :param alpha: bool (Default value = True)
     :param exclude_en: list (Default value = [])
     :param lower_words:  (Default value = True)
     :param min_length_word:  (Default value = 3)
     :returns: text (list(list(str))): A list of sentences containing words
 
     """
     corpus_file = open_corpus(corpus_path)
     text = corpus_file.read().splitlines()
     out = []
     pattern = re.compile(r"<text[^<>]*\"\>{1}")
     stop_words, number, punct, alpha = str(stop_words), str(number), str(punct), str(alpha)
     sentence = []
-
+    
+    if en != "chunking" and en != "tagging" and en != "deleting" :
+        logger.info(f"No correct option for en was provided: {en} is not valid. en option was thus set to chunking")
+        en = "chunking"
+        
+    if exceptions_path != None :
+        exceptions_file = open_corpus(exceptions_path)
+        exceptions = exceptions_file.read().splitlines()
+        if lower_words:
+            exceptions = [w.lower() for w in exceptions]
+    else : 
+        exceptions = []
+        
     for line in tqdm(text, total=len(text)):
         if line.startswith("<s>"):
             sentence = []
         elif line.startswith("</s>"):
             if len(sentence) > 2:
                 out.append(sentence)
         elif len(pattern.findall(line)) > 0:
@@ -177,59 +186,50 @@
         else:
             listline = line.split("\t")
             if len(listline) == 10:
                 for i in listline:
                     if bool(re.match('^\t\t', str(i))):
                         continue
                 token, lemma, pos, ent_iob, ent_type, is_punct, is_stop, is_alpha, is_digit, like_num = line.split("\t")
-                if lemmatize:
-                    if stop_words == is_stop and is_punct == punct and is_digit == number and like_num == number and not pos in exclude_pos and not ent_type in exclude_en and (
-                            alpha == is_alpha or ent_type != "None"):
+                if lower_words:
+                    token_ = token.lower()
+                    lemma_ = lemma.lower()
+                else:
+                    token_ = token
+                    lemma_ = lemma
+                if not lemmatize:
+                    lemma_ = token_
+                if token_ in exceptions : 
+                    sentence.append(token_)
+                else :
+                    if stop_words == is_stop and is_punct == punct and is_digit == number and like_num == number and not pos in exclude_pos and not ent_type in exclude_en and (alpha == is_alpha or ent_type != "None"):
                         if exclude_en and ent_iob != "None":
                             pass
                         else:
-                            if lower_words:
-                                if ent_type != "None" and len(lemma) > 1:
-                                    sentence.append(token)  # sentence.append(lemma.lower())
-                                    # print(lemma)
-                                elif len(lemma) > min_length_word:
-                                    sentence.append(lemma.lower())
-                            else:
-                                if ent_type != "None":
-                                    sentence.append(token)
-                                elif len(lemma) > min_length_word:
-                                    sentence.append(lemma)
+                            if ent_type != "None" and len(lemma_) > 1:
+                                if en == "chunking" :
+                                    sentence.append(token_)
+                                elif en == "tagging" :
+                                    sentence.append(ent_type)  
+                                elif en == "deleting" :
+                                    pass
+                            elif len(lemma) > min_length_word:
+                                sentence.append(lemma_)
                     else:
                         pass
-                else:
-                    if stop_words == is_stop and is_punct == punct and is_digit == number and alpha == is_alpha and like_num == number and not pos in exclude_pos and not ent_type in exclude_en:
-                        if exclude_en and ent_iob != "None":
-                            pass
-                        else:
-                            if lower_words:
-                                if ent_type != "None" and len(token) > 1:
-                                    sentence.append(token)  # (token)
-                                elif len(token) > min_length_word:
-                                    sentence.append(token.lower())
-                            else:
-                                if ent_type != "None":
-                                    sentence.append(token)  # (token)
-                                elif len(lemma) > min_length_word:
-                                    sentence.append(token)
             else:
                 continue
     if min_freq > 1:
         counts = Counter([word for sent in out for word in sent])
         accepted_tokens = {word for word, count in counts.items() if count >= min_freq}
         out = [[word for word in sent if word in accepted_tokens] for sent in out]
         # line = corpus.readline().rstrip()
         # x+=1
     return out
-
-
+        
 def open_corpus(corpus_path):
     """
 
     :param corpus_path: 
 
     """
     if isinstance(corpus_path, str):
```

### Comparing `sinr-1.1.1/sinr/viz.py` & `sinr-1.2.0a0/sinr/viz.py`

 * *Files identical despite different names*

### Comparing `sinr-1.1.1/PKG-INFO` & `sinr-1.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinr
-Version: 1.1.1
+Version: 1.2.0a0
 Summary: Build word and graph embeddings based on community detection in graphs.
 Home-page: https://sinr-embeddings.github.io/sinr/_build/html/index.html
 License: CeCILL 2.1
 Keywords: node embedding,word embedding,embedding,graph embedding,louvain,community
 Author: Thibault Prouteau
 Author-email: thibault.prouteau@univ-lemans.fr
 Requires-Python: >=3.8,<4.0
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
 Requires-Dist: igraph (>=0.10.4,<0.11.0)
 Requires-Dist: ipykernel (>=6.21.1,<7.0.0)
 Requires-Dist: joblib (>=1.1.1)
 Requires-Dist: leidenalg (>=0.9.1,<0.10.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: networkit (==9.1.1)
 Requires-Dist: numpy (>=1.21.0)
```

