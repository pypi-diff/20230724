# Comparing `tmp/cece-0.0.2.tar.gz` & `tmp/cece-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cece-0.0.2.tar", last modified: Sun Jul 23 14:33:58 2023, max compression
+gzip compressed data, was "cece-0.0.3.tar", last modified: Mon Jul 24 12:47:45 2023, max compression
```

## Comparing `cece-0.0.2.tar` & `cece-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 14:33:58.241673 cece-0.0.2/
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     1076 2023-07-23 11:31:40.000000 cece-0.0.2/LICENCE
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     9813 2023-07-23 14:33:58.241403 cece-0.0.2/PKG-INFO
-drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 14:33:58.236425 cece-0.0.2/app/
-drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 14:33:58.238906 cece-0.0.2/app/cece/
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 12:34:58.000000 cece-0.0.2/app/cece/__init__.py
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     4416 2023-07-23 12:53:48.000000 cece-0.0.2/app/cece/queries.py
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     4911 2023-07-23 14:28:22.000000 cece-0.0.2/app/cece/refine.py
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      775 2023-07-23 14:26:59.000000 cece-0.0.2/app/cece/wordnet.py
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     5347 2023-07-23 14:28:23.000000 cece-0.0.2/app/cece/xDataset.py
-drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 14:33:58.240927 cece-0.0.2/app/cece.egg-info/
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     9813 2023-07-23 14:33:58.000000 cece-0.0.2/app/cece.egg-info/PKG-INFO
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      276 2023-07-23 14:33:58.000000 cece-0.0.2/app/cece.egg-info/SOURCES.txt
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        1 2023-07-23 14:33:58.000000 cece-0.0.2/app/cece.egg-info/dependency_links.txt
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)       61 2023-07-23 14:33:58.000000 cece-0.0.2/app/cece.egg-info/requires.txt
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        5 2023-07-23 14:33:58.000000 cece-0.0.2/app/cece.egg-info/top_level.txt
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)       38 2023-07-23 14:33:58.241759 cece-0.0.2/setup.cfg
--rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      839 2023-07-23 14:29:07.000000 cece-0.0.2/setup.py
+drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-24 12:47:45.611350 cece-0.0.3/
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)    13056 2023-07-24 12:47:45.611101 cece-0.0.3/PKG-INFO
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     9962 2023-07-24 12:02:35.000000 cece-0.0.3/README.md
+drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-24 12:47:45.607057 cece-0.0.3/app/
+drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-24 12:47:45.609257 cece-0.0.3/app/cece/
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-23 12:34:58.000000 cece-0.0.3/app/cece/__init__.py
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     4416 2023-07-23 12:53:48.000000 cece-0.0.3/app/cece/queries.py
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     4911 2023-07-23 14:28:22.000000 cece-0.0.3/app/cece/refine.py
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      775 2023-07-23 14:26:59.000000 cece-0.0.3/app/cece/wordnet.py
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)     6938 2023-07-23 18:57:29.000000 cece-0.0.3/app/cece/xDataset.py
+drwxr-xr-x   0 giorgosfilandrianos   (501) staff       (20)        0 2023-07-24 12:47:45.610677 cece-0.0.3/app/cece.egg-info/
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)    13056 2023-07-24 12:47:45.000000 cece-0.0.3/app/cece.egg-info/PKG-INFO
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      278 2023-07-24 12:47:45.000000 cece-0.0.3/app/cece.egg-info/SOURCES.txt
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        1 2023-07-24 12:47:45.000000 cece-0.0.3/app/cece.egg-info/dependency_links.txt
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)       48 2023-07-24 12:47:45.000000 cece-0.0.3/app/cece.egg-info/requires.txt
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)        5 2023-07-24 12:47:45.000000 cece-0.0.3/app/cece.egg-info/top_level.txt
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)       38 2023-07-24 12:47:45.611437 cece-0.0.3/setup.cfg
+-rw-r--r--   0 giorgosfilandrianos   (501) staff       (20)      824 2023-07-24 12:47:42.000000 cece-0.0.3/setup.py
```

### Comparing `cece-0.0.2/PKG-INFO` & `cece-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,159 @@
 Metadata-Version: 2.1
 Name: cece
-Version: 0.0.2
-Summary: Semantic Edits as Counterfctual Explanations
+Version: 0.0.3
+Summary: Conceptual Edits as Counterfactual Explanations
 Home-page: UNKNOWN
 Author: Giorgos Filandrianos
 Author-email: georgefilandr@gmail.com
 License: MIT
-Description: # Choose Your Data Wisely
+Description: # Conceptual Edits as Counterfactual Explanations (CECE)
         
-        This repository contains code for our paper, [Choose your Data Wisely: A Framework for Semantic Counterfactuals
+        ![png](https://github.com/geofila/Semantic-Counterfactuals/blob/main/app/images/logo.png?raw=true)
+        
+        **CECE: a powerful Python library for generating semantic counterfactual explanations for any machine learning algorithm.**
+        
+        <a target="_blank" href="https://colab.research.google.com/github/geofila/Semantic-Counterfactuals/blob/main/app/cece/playground.ipynb">
+          <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+        </a>
+        
+        More information about the framework and the algorithm that the library uses can be found in the paper: [Choose your Data Wisely: A Framework for Semantic Counterfactuals
         ](https://arxiv.org/pdf/2305.17667.pdf).
         
         ## Citation
         ```bibtex
         @article{dervakos2023choose,
           title={Choose your Data Wisely: A Framework for Semantic Counterfactuals},
           author={Dervakos, Edmund and Thomas, Konstantinos and Filandrianos, Giorgos and Stamou, Giorgos},
           journal={arXiv preprint arXiv:2305.17667},
           year={2023}
         }
         ```
         
+        # How to install the library
+        ```python
+        # Install cece
+        pip install cece
+        ```
+        
+        **- or -**
+        
+        ```python
+        git clone https://github.com/geofila/Semantic-Counterfactuals.git
+        cd Semantic-Counterfactuals
+        git install .
+        ```
+        
+        # How to use the library
         
+        ## Use Case 1: Calculate the semantic distance between 2 queries
         
-        ## Use Case 1: Calculate GED between 2 objects
         
-        ``` python
+        ```python
         from cece.queries import *
         from cece.refine import *
         
         
         q1 = Query(np.array([set(["car", "vehicle"]), set(["tree"])]))
         q2 = Query(np.array([set(["car"]), set(["tree"]), set(["person"])]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         
         print (r)
         ```
         
-        
             Remains the same: {'tree'}
             -------------------------------------
             Tranform {'car'} from {'vehicle'} -> set()
             Add: {'person'}
             --------------------------------------
             (2, {'additions': [{'person'}], 'removals': [], 'transf': [({'car', 'vehicle'}, {'car'})]})
-            [{'car', 'vehicle'} {'tree'}]
-            {}
         
-        ``` python
+        
+        
+        ```python
         from cece.wordnet import *
         
         q1 = Query(np.array([set(connect_term_to_wordnet("car")),
                              set(connect_term_to_wordnet("man")),]))
         
         q2 = Query(np.array([set(connect_term_to_wordnet("woman")),
                              set(connect_term_to_wordnet("truck"),)]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
             -------------------------------------
-            Tranform {'object.n.01', 'entity.n.01', 'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'physical_entity.n.01', 'conveyance.n.03', 'artifact.n.01', 'whole.n.02', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'} from {'car.n.01'} -> {'truck.n.01'}
-            Tranform {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'organism.n.01', 'adult.n.01'} from {'man.n.01'} -> {'woman.n.01'}
+            Tranform {'motor_vehicle.n.01', 'artifact.n.01', 'instrumentality.n.03', 'whole.n.02', 'object.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'physical_entity.n.01', 'entity.n.01'} from {'car.n.01'} -> {'truck.n.01'}
+            Tranform {'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'} from {'man.n.01'} -> {'woman.n.01'}
             --------------------------------------
             Cost:  4
         
-        ``` python
+        
+        
+        ```python
         
         q1 = Query(np.array([connect_term_to_wordnet("tree"),
                              connect_term_to_wordnet("man"),]))
         
         q2 = Query(np.array([connect_term_to_wordnet("man"),
                              connect_term_to_wordnet("truck"),]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
         
         ### or even simpler
         
         
-        ``` python
+        ```python
         q1 = Query(np.array(connect_list_to_wordnet(["tree", "man"])))
         q2 = Query(np.array(connect_list_to_wordnet(["man", "truck"])))
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
         
-        ## Or even simpler {#or-even-simpler}
+        ### or even simpler
+        
         
-        ``` python
+        ```python
         from cece.xDataset import createMSQ
         
         q1 = createMSQ(["tree", "man"], connect_to_wordnet = True)
         q2 = createMSQ(["man", "truck"], connect_to_wordnet = True)
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
-        ## Use Case 2: Use it for a Datatset {#-use-case-2-use-it-for-a-datatset}
         
-        ``` python
+        ## Use Case 2: Use it for a Datatset
+        
+        
+        ```python
         from cece.xDataset import *
         
         
         # initialize an instance of the Dataset
         ds = xDataset(dataset = [["tree", "man"],
                                  ["man", "truck"],
                                  ["kitchen", "oven", "refrigerator"], 
@@ -136,54 +163,70 @@
                       labels = ["outdoor", "outdoor", "indoor", "indoor", "indoor"],
                       connect_to_wordnet = True)
         
         
         ds.retrieve(ds.dataset[1])
         ```
         
-        ``` python
+        
+        
+        
+            {1: 0, 0: 14, 4: 28, 3: 29, 2: 36}
+        
+        
+        
+        
+        ```python
         for idx, cost in ds.retrieve(ds.dataset[1]).items():
             print (f"Cost: {cost} for '{ds.labels[idx]}' with id: {idx}")
         ```
         
             Cost: 0 for 'outdoor' with id: 1
             Cost: 14 for 'outdoor' with id: 0
             Cost: 28 for 'indoor' with id: 4
             Cost: 29 for 'indoor' with id: 3
             Cost: 36 for 'indoor' with id: 2
         
-        ``` python
+        
+        
+        ```python
         results = ds.retrieve([ "car", "woman"])
         
         for idx, cost in results.items():
             print (f"Cost: {cost} for '{ds.labels[idx]}' with id: {idx}")
         ```
         
             Cost: 4 for 'outdoor' with id: 1
             Cost: 16 for 'outdoor' with id: 0
             Cost: 27 for 'indoor' with id: 3
             Cost: 28 for 'indoor' with id: 4
             Cost: 36 for 'indoor' with id: 2
         
         
-        ### Explain Method - Get a Semantic Counterfatual
+        ## Explain Method - Get a Semantic Counterfatual
+        
         
-        ``` python
+        ```python
         results = ds.explain([ "car", "woman"], "outdoor")
         
         print (f"Cost: {results[1]} for '{ds.labels[results[0]]}' with id: {results[0]}")
         ```
         
             Cost: 27 for 'indoor' with id: 3
         
-        ``` python
+        
+        
+        ```python
         from cece.xDataset import *
         ds.find_edits(["car", "man"], ["woman", "truck"])
         ```
         
+        
+        
+        
             (4,
              {'additions': [],
               'removals': [],
               'transf': [({'artifact.n.01',
                  'car.n.01',
                  'conveyance.n.03',
                  'entity.n.01',
@@ -222,14 +265,80 @@
                  'object.n.01',
                  'organism.n.01',
                  'person.n.01',
                  'physical_entity.n.01',
                  'whole.n.02',
                  'woman.n.01'})]})
         
+        
+        
+        ## Global Explanations 
+        
+        
+        ```python
+        from cece.xDataset import *
+        
+        # initialize an instance of the Dataset
+        ds = xDataset(dataset = [["tree", "man"],
+                                 ["man", "truck"],
+                                 ["kitchen", "oven", "refrigerator", "man"], 
+                                 ["bed", "blanket", "woman"],
+                                 ["sofa", "pillow", "man"],],
+        
+                      labels = ["outdoor", "outdoor", "indoor", "indoor", "indoor"],
+                      connect_to_wordnet = True)
+        
+        ds.global_explanation([["tree", "man", "car"], ["man", "truck", "car"]], ["outdoor", "outdoor"])
+        ```
+        
+        
+        
+        
+            {'motor_vehicle.n.01': -3,
+             'conveyance.n.03': -3,
+             'wheeled_vehicle.n.01': -3,
+             'vehicle.n.01': -3,
+             'self-propelled_vehicle.n.01': -3,
+             'padding.n.01': 2,
+             'cushion.n.03': 2,
+             'pillow.n.01': 2,
+             'car.n.01': -2,
+             'sofa.n.01': 2,
+             'furnishing.n.02': 2,
+             'seat.n.03': 2,
+             'furniture.n.01': 2,
+             'living_thing.n.01': -1,
+             'organism.n.01': -1,
+             'vascular_plant.n.01': -1,
+             'tree.n.01': -1,
+             'woody_plant.n.01': -1,
+             'plant.n.02': -1,
+             'artifact.n.01': 1,
+             'truck.n.01': -1,
+             'instrumentality.n.03': -1}
+        
+        
+        
+        
+        ```python
+        # plot the global explanation in abar plot
+        import matplotlib.pyplot as plt
+        
+        explanations = ds.global_explanation([["tree", "man", "car"], ["man", "truck", "car"]], ["outdoor", "outdoor"])
+        
+        plt.bar(explanations.keys(), explanations.values())
+        plt.xticks(rotation=90)
+        plt.show()
+        ```
+        
+        
+            
+        ![png](https://github.com/geofila/Semantic-Counterfactuals/blob/main/app/images/global_explanations_example.png?raw=true)
+            
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cece-0.0.2/app/cece/queries.py` & `cece-0.0.3/app/cece/queries.py`

 * *Files identical despite different names*

### Comparing `cece-0.0.2/app/cece/refine.py` & `cece-0.0.3/app/cece/refine.py`

 * *Files identical despite different names*

### Comparing `cece-0.0.2/app/cece/wordnet.py` & `cece-0.0.3/app/cece/wordnet.py`

 * *Files identical despite different names*

### Comparing `cece-0.0.2/app/cece/xDataset.py` & `cece-0.0.3/app/cece/xDataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -108,28 +108,61 @@
         if not isinstance(q2, Query):
             q2 = createMSQ(q2, self.connect_to_wordnet)
 
         return refine (q1, q2, obj_distance = obj_distance, addition_cost = addition_cost, removal_cost = removal_cost, verbose = verbose, return_edits = True)
 
 
 
-    # def global_explanation(self, queries, labels, obj_distance = None, addition_cost = None, removal_cost = None):
-    #     if self.labels is None:
-    #         raise ValueError("The dataset is not labeled")
+    def global_explanation(self, queries, labels, obj_distance = None, addition_cost = None, removal_cost = None):
         
-    #     # we are going to calculate the global explanation
-    #     # for each label we are going to find the closest instance
-    #     # and then we are going to find the edits between the query and the closest instance
-    #     if len(set(labels)) > 1: 
-    #         print ("Warning: the dataset contains more than 1 label!")
-
-    #     global_explanation = {}
+        if self.labels is None:
+            raise ValueError("The dataset is not labeled")
         
+        # we are going to calculate the global explanation
+        # for each label we are going to find the closest instance
+        # and then we are going to find the edits between the query and the closest instance
+        if len(set(labels)) > 1: 
+            print ("Warning: the dataset contains more than 1 label!")
+
+        global_explanation = {}
+
+        for query, label in zip(queries, labels):
+            resp = self.explain(query, label, obj_distance = obj_distance, addition_cost = addition_cost, removal_cost = removal_cost)
+            if resp is None:
+                continue 
+            
+            _, edits = self.find_edits(query, self.dataset[resp[0]], obj_distance = obj_distance, addition_cost = addition_cost, removal_cost = removal_cost)
         
-    
+            for obj in edits["additions"]:
+                for concept in obj:
+                    if concept not in global_explanation:
+                        global_explanation[concept] = 0
+                    global_explanation[concept] += 1
+
+            for obj in edits["removals"]:
+                for concept in obj:
+                    if concept not in global_explanation:
+                        global_explanation[concept] = 0
+                    global_explanation[concept] -= 1
+
+            for obj1, obj2 in edits["transf"]:
+                for concept in obj1 - obj2:
+                    if concept not in global_explanation:
+                        global_explanation[concept] = 0
+                    global_explanation[concept] -= 1
+                
+                for concept in obj2 - obj1:
+                    if concept not in global_explanation:
+                        global_explanation[concept] = 0
+                    global_explanation[concept] += 1
+
+        # sort based on the abs value of the explanation
+        global_explanation = {k: v for k, v in sorted(global_explanation.items(), key=lambda item: abs(item[1]), reverse = True)}
+        return global_explanation
+
 
 
     def __repr__(self):
         return f"xDataset with {len(self.dataset)} instances"
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `cece-0.0.2/app/cece.egg-info/PKG-INFO` & `cece-0.0.3/app/cece.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,159 @@
 Metadata-Version: 2.1
 Name: cece
-Version: 0.0.2
-Summary: Semantic Edits as Counterfctual Explanations
+Version: 0.0.3
+Summary: Conceptual Edits as Counterfactual Explanations
 Home-page: UNKNOWN
 Author: Giorgos Filandrianos
 Author-email: georgefilandr@gmail.com
 License: MIT
-Description: # Choose Your Data Wisely
+Description: # Conceptual Edits as Counterfactual Explanations (CECE)
         
-        This repository contains code for our paper, [Choose your Data Wisely: A Framework for Semantic Counterfactuals
+        ![png](https://github.com/geofila/Semantic-Counterfactuals/blob/main/app/images/logo.png?raw=true)
+        
+        **CECE: a powerful Python library for generating semantic counterfactual explanations for any machine learning algorithm.**
+        
+        <a target="_blank" href="https://colab.research.google.com/github/geofila/Semantic-Counterfactuals/blob/main/app/cece/playground.ipynb">
+          <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+        </a>
+        
+        More information about the framework and the algorithm that the library uses can be found in the paper: [Choose your Data Wisely: A Framework for Semantic Counterfactuals
         ](https://arxiv.org/pdf/2305.17667.pdf).
         
         ## Citation
         ```bibtex
         @article{dervakos2023choose,
           title={Choose your Data Wisely: A Framework for Semantic Counterfactuals},
           author={Dervakos, Edmund and Thomas, Konstantinos and Filandrianos, Giorgos and Stamou, Giorgos},
           journal={arXiv preprint arXiv:2305.17667},
           year={2023}
         }
         ```
         
+        # How to install the library
+        ```python
+        # Install cece
+        pip install cece
+        ```
+        
+        **- or -**
+        
+        ```python
+        git clone https://github.com/geofila/Semantic-Counterfactuals.git
+        cd Semantic-Counterfactuals
+        git install .
+        ```
+        
+        # How to use the library
         
+        ## Use Case 1: Calculate the semantic distance between 2 queries
         
-        ## Use Case 1: Calculate GED between 2 objects
         
-        ``` python
+        ```python
         from cece.queries import *
         from cece.refine import *
         
         
         q1 = Query(np.array([set(["car", "vehicle"]), set(["tree"])]))
         q2 = Query(np.array([set(["car"]), set(["tree"]), set(["person"])]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         
         print (r)
         ```
         
-        
             Remains the same: {'tree'}
             -------------------------------------
             Tranform {'car'} from {'vehicle'} -> set()
             Add: {'person'}
             --------------------------------------
             (2, {'additions': [{'person'}], 'removals': [], 'transf': [({'car', 'vehicle'}, {'car'})]})
-            [{'car', 'vehicle'} {'tree'}]
-            {}
         
-        ``` python
+        
+        
+        ```python
         from cece.wordnet import *
         
         q1 = Query(np.array([set(connect_term_to_wordnet("car")),
                              set(connect_term_to_wordnet("man")),]))
         
         q2 = Query(np.array([set(connect_term_to_wordnet("woman")),
                              set(connect_term_to_wordnet("truck"),)]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
             -------------------------------------
-            Tranform {'object.n.01', 'entity.n.01', 'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'physical_entity.n.01', 'conveyance.n.03', 'artifact.n.01', 'whole.n.02', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'} from {'car.n.01'} -> {'truck.n.01'}
-            Tranform {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'organism.n.01', 'adult.n.01'} from {'man.n.01'} -> {'woman.n.01'}
+            Tranform {'motor_vehicle.n.01', 'artifact.n.01', 'instrumentality.n.03', 'whole.n.02', 'object.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'physical_entity.n.01', 'entity.n.01'} from {'car.n.01'} -> {'truck.n.01'}
+            Tranform {'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'} from {'man.n.01'} -> {'woman.n.01'}
             --------------------------------------
             Cost:  4
         
-        ``` python
+        
+        
+        ```python
         
         q1 = Query(np.array([connect_term_to_wordnet("tree"),
                              connect_term_to_wordnet("man"),]))
         
         q2 = Query(np.array([connect_term_to_wordnet("man"),
                              connect_term_to_wordnet("truck"),]))
         
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
         
         ### or even simpler
         
         
-        ``` python
+        ```python
         q1 = Query(np.array(connect_list_to_wordnet(["tree", "man"])))
         q2 = Query(np.array(connect_list_to_wordnet(["man", "truck"])))
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
         
-        ## Or even simpler {#or-even-simpler}
+        ### or even simpler
+        
         
-        ``` python
+        ```python
         from cece.xDataset import createMSQ
         
         q1 = createMSQ(["tree", "man"], connect_to_wordnet = True)
         q2 = createMSQ(["man", "truck"], connect_to_wordnet = True)
         r = refine (q1, q2,verbose= True, return_edits = True)
         print ("Cost: ", r[0])
         ```
         
-            Remains the same: {'object.n.01', 'entity.n.01', 'living_thing.n.01', 'person.n.01', 'physical_entity.n.01', 'whole.n.02', 'man.n.01', 'organism.n.01', 'adult.n.01'}
+            Remains the same: {'man.n.01', 'living_thing.n.01', 'adult.n.01', 'whole.n.02', 'organism.n.01', 'person.n.01', 'object.n.01', 'physical_entity.n.01', 'entity.n.01'}
             -------------------------------------
-            Tranform {'whole.n.02', 'physical_entity.n.01', 'object.n.01', 'entity.n.01'} from {'living_thing.n.01', 'woody_plant.n.01', 'vascular_plant.n.01', 'plant.n.02', 'organism.n.01', 'tree.n.01'} -> {'motor_vehicle.n.01', 'vehicle.n.01', 'instrumentality.n.03', 'conveyance.n.03', 'truck.n.01', 'artifact.n.01', 'self-propelled_vehicle.n.01', 'wheeled_vehicle.n.01'}
+            Tranform {'entity.n.01', 'whole.n.02', 'physical_entity.n.01', 'object.n.01'} from {'living_thing.n.01', 'organism.n.01', 'vascular_plant.n.01', 'tree.n.01', 'woody_plant.n.01', 'plant.n.02'} -> {'motor_vehicle.n.01', 'instrumentality.n.03', 'truck.n.01', 'conveyance.n.03', 'wheeled_vehicle.n.01', 'vehicle.n.01', 'self-propelled_vehicle.n.01', 'artifact.n.01'}
             --------------------------------------
             Cost:  14
         
-        ## Use Case 2: Use it for a Datatset {#-use-case-2-use-it-for-a-datatset}
         
-        ``` python
+        ## Use Case 2: Use it for a Datatset
+        
+        
+        ```python
         from cece.xDataset import *
         
         
         # initialize an instance of the Dataset
         ds = xDataset(dataset = [["tree", "man"],
                                  ["man", "truck"],
                                  ["kitchen", "oven", "refrigerator"], 
@@ -136,54 +163,70 @@
                       labels = ["outdoor", "outdoor", "indoor", "indoor", "indoor"],
                       connect_to_wordnet = True)
         
         
         ds.retrieve(ds.dataset[1])
         ```
         
-        ``` python
+        
+        
+        
+            {1: 0, 0: 14, 4: 28, 3: 29, 2: 36}
+        
+        
+        
+        
+        ```python
         for idx, cost in ds.retrieve(ds.dataset[1]).items():
             print (f"Cost: {cost} for '{ds.labels[idx]}' with id: {idx}")
         ```
         
             Cost: 0 for 'outdoor' with id: 1
             Cost: 14 for 'outdoor' with id: 0
             Cost: 28 for 'indoor' with id: 4
             Cost: 29 for 'indoor' with id: 3
             Cost: 36 for 'indoor' with id: 2
         
-        ``` python
+        
+        
+        ```python
         results = ds.retrieve([ "car", "woman"])
         
         for idx, cost in results.items():
             print (f"Cost: {cost} for '{ds.labels[idx]}' with id: {idx}")
         ```
         
             Cost: 4 for 'outdoor' with id: 1
             Cost: 16 for 'outdoor' with id: 0
             Cost: 27 for 'indoor' with id: 3
             Cost: 28 for 'indoor' with id: 4
             Cost: 36 for 'indoor' with id: 2
         
         
-        ### Explain Method - Get a Semantic Counterfatual
+        ## Explain Method - Get a Semantic Counterfatual
+        
         
-        ``` python
+        ```python
         results = ds.explain([ "car", "woman"], "outdoor")
         
         print (f"Cost: {results[1]} for '{ds.labels[results[0]]}' with id: {results[0]}")
         ```
         
             Cost: 27 for 'indoor' with id: 3
         
-        ``` python
+        
+        
+        ```python
         from cece.xDataset import *
         ds.find_edits(["car", "man"], ["woman", "truck"])
         ```
         
+        
+        
+        
             (4,
              {'additions': [],
               'removals': [],
               'transf': [({'artifact.n.01',
                  'car.n.01',
                  'conveyance.n.03',
                  'entity.n.01',
@@ -222,14 +265,80 @@
                  'object.n.01',
                  'organism.n.01',
                  'person.n.01',
                  'physical_entity.n.01',
                  'whole.n.02',
                  'woman.n.01'})]})
         
+        
+        
+        ## Global Explanations 
+        
+        
+        ```python
+        from cece.xDataset import *
+        
+        # initialize an instance of the Dataset
+        ds = xDataset(dataset = [["tree", "man"],
+                                 ["man", "truck"],
+                                 ["kitchen", "oven", "refrigerator", "man"], 
+                                 ["bed", "blanket", "woman"],
+                                 ["sofa", "pillow", "man"],],
+        
+                      labels = ["outdoor", "outdoor", "indoor", "indoor", "indoor"],
+                      connect_to_wordnet = True)
+        
+        ds.global_explanation([["tree", "man", "car"], ["man", "truck", "car"]], ["outdoor", "outdoor"])
+        ```
+        
+        
+        
+        
+            {'motor_vehicle.n.01': -3,
+             'conveyance.n.03': -3,
+             'wheeled_vehicle.n.01': -3,
+             'vehicle.n.01': -3,
+             'self-propelled_vehicle.n.01': -3,
+             'padding.n.01': 2,
+             'cushion.n.03': 2,
+             'pillow.n.01': 2,
+             'car.n.01': -2,
+             'sofa.n.01': 2,
+             'furnishing.n.02': 2,
+             'seat.n.03': 2,
+             'furniture.n.01': 2,
+             'living_thing.n.01': -1,
+             'organism.n.01': -1,
+             'vascular_plant.n.01': -1,
+             'tree.n.01': -1,
+             'woody_plant.n.01': -1,
+             'plant.n.02': -1,
+             'artifact.n.01': 1,
+             'truck.n.01': -1,
+             'instrumentality.n.03': -1}
+        
+        
+        
+        
+        ```python
+        # plot the global explanation in abar plot
+        import matplotlib.pyplot as plt
+        
+        explanations = ds.global_explanation([["tree", "man", "car"], ["man", "truck", "car"]], ["outdoor", "outdoor"])
+        
+        plt.bar(explanations.keys(), explanations.values())
+        plt.xticks(rotation=90)
+        plt.show()
+        ```
+        
+        
+            
+        ![png](https://github.com/geofila/Semantic-Counterfactuals/blob/main/app/images/global_explanations_example.png?raw=true)
+            
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cece-0.0.2/setup.py` & `cece-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="cece",
-    version="0.0.02",
-    description="Semantic Edits as Counterfctual Explanations",
+    version="0.0.03",
+    description="Conceptual Edits as Counterfactual Explanations",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Giorgos Filandrianos",
     author_email="georgefilandr@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=["bson >= 0.5.10", "numpy >= 1.20.1", "networkx >= 2.5"],
+    install_requires=["numpy >= 1.20.1", "networkx >= 2.5"],
     extras_require={
         "dev": ["twine>=4.0.2"],
     },
     python_requires=">=3.8.8",
 )
```

