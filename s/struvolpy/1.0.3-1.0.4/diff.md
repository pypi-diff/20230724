# Comparing `tmp/struvolpy-1.0.3.tar.gz` & `tmp/struvolpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struvolpy-1.0.3.tar", last modified: Mon Jul 24 14:47:11 2023, max compression
+gzip compressed data, was "struvolpy-1.0.4.tar", last modified: Mon Jul 24 14:49:42 2023, max compression
```

## Comparing `struvolpy-1.0.3.tar` & `struvolpy-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/
--rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-18 08:40:59.000000 struvolpy-1.0.3/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:47:11.577516 struvolpy-1.0.3/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 08:46:27.000000 struvolpy-1.0.3/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      982 2023-07-24 14:47:11.581516 struvolpy-1.0.3/setup.cfg
--rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-18 08:40:59.000000 struvolpy-1.0.3/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy/
--rw-rw-r--   0 luc       (1000) luc       (1000)    20296 2023-07-21 12:37:23.000000 struvolpy-1.0.3/struvolpy/Structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)    22113 2023-07-23 21:32:39.000000 struvolpy-1.0.3/struvolpy/Volume.py
--rw-rw-r--   0 luc       (1000) luc       (1000)      132 2023-07-21 12:37:23.000000 struvolpy-1.0.3/struvolpy/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy/wrappers/
--rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-18 14:24:41.000000 struvolpy-1.0.3/struvolpy/wrappers/__init__.py
--rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-18 15:44:06.000000 struvolpy-1.0.3/struvolpy/wrappers/wrappers.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/top_level.txt
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/tests/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-18 15:14:19.000000 struvolpy-1.0.3/tests/test_structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-23 21:33:33.000000 struvolpy-1.0.3/tests/test_volume.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:49:42.126389 struvolpy-1.0.4/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-18 08:40:59.000000 struvolpy-1.0.4/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:49:42.126389 struvolpy-1.0.4/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 08:46:27.000000 struvolpy-1.0.4/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      982 2023-07-24 14:49:42.126389 struvolpy-1.0.4/setup.cfg
+-rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-18 08:40:59.000000 struvolpy-1.0.4/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:49:42.126389 struvolpy-1.0.4/struvolpy/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    20378 2023-07-24 14:49:07.000000 struvolpy-1.0.4/struvolpy/Structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)    22113 2023-07-23 21:32:39.000000 struvolpy-1.0.4/struvolpy/Volume.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)      132 2023-07-21 12:37:23.000000 struvolpy-1.0.4/struvolpy/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:49:42.126389 struvolpy-1.0.4/struvolpy/wrappers/
+-rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-18 14:24:41.000000 struvolpy-1.0.4/struvolpy/wrappers/__init__.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-18 15:44:06.000000 struvolpy-1.0.4/struvolpy/wrappers/wrappers.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:49:42.126389 struvolpy-1.0.4/struvolpy.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:49:42.000000 struvolpy-1.0.4/struvolpy.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-24 14:49:42.000000 struvolpy-1.0.4/struvolpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-24 14:49:42.000000 struvolpy-1.0.4/struvolpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-24 14:49:42.000000 struvolpy-1.0.4/struvolpy.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-24 14:49:42.000000 struvolpy-1.0.4/struvolpy.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:49:42.126389 struvolpy-1.0.4/tests/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-18 15:14:19.000000 struvolpy-1.0.4/tests/test_structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-23 21:33:33.000000 struvolpy-1.0.4/tests/test_volume.py
```

### Comparing `struvolpy-1.0.3/LICENSE` & `struvolpy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.3/PKG-INFO` & `struvolpy-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.3/README.md` & `struvolpy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.3/setup.cfg` & `struvolpy-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = struvolpy
-version = 1.0.3
+version = 1.0.4
 author = Luc Elliott
 author_email = hllelli2@liverpool.ac.uk
 description = "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 long_description = file: ./README.md
 long_description_content_type = text/markdown
 Home-page = https://github.com/hllelli2/struvolpy/
 license = "GPLv3"
```

### Comparing `struvolpy-1.0.3/struvolpy/Structure.py` & `struvolpy-1.0.4/struvolpy/Structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,51 +425,51 @@
         self.translate(-centreofmass)
         self.coor = np.dot(rotation_matrix, self.coor)
         rotated_centreofmass = np.dot(rotation_matrix, centreofmass)
         self.translate(rotated_centreofmass)
 
     # Structure comparisons
 
-    def overlap(self, structure, cdd_threshold=0.1, distance_threshold=0.5):
+    def overlap(
+        self, structure, distance_threshold=1, overlapping_points_threshold=0.05
+    ):
         """
-        Calculate the overlap between two structures.
+        Determines whether two structures overlap by checking if they have a minimum number of overlapping points.
 
         Args:
             structure (Structure): The structure to compare with.
-            cdd_threshold (float): The CDD threshold for overlap detection.
-            Default is 0.1.
-            distance_threshold (float): The distance threshold for overlap
-            detection. Default is 0.5.
+            distance_threshold (float): The maximum distance between two points for them to be considered overlapping.
+            overlapping_points_threshold (float): The minimum fraction of overlapping points required for the structures to be considered overlapping.
 
         Returns:
-            bool: True if the two structures overlap, False otherwise.
+            bool: True if the structures overlap, False otherwise.
 
         Raises:
-            None.
-
+            None
         """
-        # TODO: code along with copilot so need to double check things
+
         if self.__tree is None:
             self.__build_kdtree()
 
         coords2 = np.asarray(
-            [structure.coor[0], structure.coor[1], structure.coor[2]]
+            np.asarray([structure.coor[0], structure.coor[1], structure.coor[2]])
         ).T
 
-        cdd = np.sqrt(np.sum((self.__tree.query(coords2, k=1)[0] - cdd_threshold) ** 2))
+        min_overlap = (
+            min(len(self.__tree_coords), len(coords2)) * overlapping_points_threshold
+        )
+
+        num_intersecting_points = np.sum(
+            self.__tree.query(coords2, k=1)[0] < distance_threshold
+        )
 
-        if cdd < cdd_threshold:
-            return True
+        if num_intersecting_points < min_overlap:
+            return False
         else:
-            distances = self.__tree.query(coords2, k=1)[0]
-
-            if np.max(distances) < distance_threshold:
-                return True
-            else:
-                return False
+            return True
 
     def rmsd(self, structure):
         """
         Calculates the root-mean-square deviation (RMSD) between
         two structures.
 
         Args:
```

### Comparing `struvolpy-1.0.3/struvolpy/Volume.py` & `struvolpy-1.0.4/struvolpy/Volume.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.3/struvolpy/wrappers/wrappers.py` & `struvolpy-1.0.4/struvolpy/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.3/struvolpy.egg-info/PKG-INFO` & `struvolpy-1.0.4/struvolpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.3/tests/test_structure.py` & `struvolpy-1.0.4/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.3/tests/test_volume.py` & `struvolpy-1.0.4/tests/test_volume.py`

 * *Files identical despite different names*

