# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.3.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.3.tar", last modified: Fri Jul 21 11:44:07 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.4.tar", last modified: Mon Jul 24 14:55:46 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.3.tar` & `EnsembleParticleSwarmOptimization-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-21 11:44:07.093069 EnsembleParticleSwarmOptimization-0.1.3/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-21 11:44:07.093069 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-21 11:44:07.000000 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-21 11:44:07.000000 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-21 11:44:07.000000 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-21 11:44:07.000000 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-21 11:44:07.000000 EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-21 11:44:07.093069 EnsembleParticleSwarmOptimization-0.1.3/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-21 11:44:07.093069 EnsembleParticleSwarmOptimization-0.1.3/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30395 2023-07-21 11:35:34.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-21 11:33:30.000000 EnsembleParticleSwarmOptimization-0.1.3/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.3/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-21 11:44:07.093069 EnsembleParticleSwarmOptimization-0.1.3/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-21 11:33:36.000000 EnsembleParticleSwarmOptimization-0.1.3/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30609 2023-07-24 14:53:44.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-24 14:55:17.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-24 14:55:23.000000 EnsembleParticleSwarmOptimization-0.1.4/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.4/PySO/Clustering_Swarms.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.4/PySO/HierarchicalSwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.4/PySO/MWE_Swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,16 @@
             assert (  len(Periodic)==self.Ndim  and  all(np.isin(Periodic, [0,1]))  )
             self.Periodic = list(Periodic)
 
         self.PeriodicParamRanges = np.array([
                                             np.inf if self.Periodic[i]==0 else np.ptp(b)
                                         for i, b in enumerate(self.Model.bounds)])
 
+	# Param indexes where periodicity happens
+        self.Periodic_params = np.where(self.Periodic == 1)[0]
 
         self.BoundsArray = np.array(self.Model.bounds)
 
         #     NOTE: ptp by default positive
 
 
         if Velocity_clipping_or_rescale == 'Clip':
@@ -337,15 +339,15 @@
 
 
     def EnforceBoundaries(self):
         """
         Boundary conditions on the edge of the search region
         """
         # Periodic BCs
-        self.Points = self.BoundsArray[:,0] + np.mod(self.Points-self.BoundsArray[:,0],self.PeriodicParamRanges)
+        self.Points[:,self.Periodic_params] = self.BoundsArray[self.Periodic_params,0] + np.mod(self.Points[:,self.Periodic_params]-self.BoundsArray[self.Periodic_params,0],self.PeriodicParamRanges[self.Periodic_params])
 
         # Hard edges
         clipped_points = np.clip(self.Points, a_min=self.BoundsArray[:,0], a_max=self.BoundsArray[:,1])
 
         # Reflective boundary velocities
         # This does mess with the MH MCMC part of the velocity rule, so proposals near prior boundary in the case MH_fraction=1.0 will be affected
         velocity_reflection_indices = np.where(clipped_points != self.Points)
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.4/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.4/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.3/setup.py` & `EnsembleParticleSwarmOptimization-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.3",
+    version="0.1.4",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

