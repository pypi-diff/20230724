# Comparing `tmp/struvolpy-1.0.2.tar.gz` & `tmp/struvolpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struvolpy-1.0.2.tar", last modified: Thu Jul 20 11:46:48 2023, max compression
+gzip compressed data, was "struvolpy-1.0.3.tar", last modified: Mon Jul 24 14:47:11 2023, max compression
```

## Comparing `struvolpy-1.0.2.tar` & `struvolpy-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/
--rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-19 13:31:13.000000 struvolpy-1.0.2/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-20 11:46:48.192202 struvolpy-1.0.2/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 13:31:13.000000 struvolpy-1.0.2/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      958 2023-07-20 11:46:48.192202 struvolpy-1.0.2/setup.cfg
--rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-19 13:31:13.000000 struvolpy-1.0.2/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.188202 struvolpy-1.0.2/struvolpy/
--rw-rw-r--   0 luc       (1000) luc       (1000)    20325 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/Structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)    22154 2023-07-20 11:13:06.000000 struvolpy-1.0.2/struvolpy/Volume.py
--rw-rw-r--   0 luc       (1000) luc       (1000)       83 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/struvolpy/wrappers/
--rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/wrappers/__init__.py
--rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/wrappers/wrappers.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.188202 struvolpy-1.0.2/struvolpy.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/top_level.txt
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/tests/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-19 13:31:13.000000 struvolpy-1.0.2/tests/test_structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-19 13:31:13.000000 struvolpy-1.0.2/tests/test_volume.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-18 08:40:59.000000 struvolpy-1.0.3/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:47:11.577516 struvolpy-1.0.3/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 08:46:27.000000 struvolpy-1.0.3/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      982 2023-07-24 14:47:11.581516 struvolpy-1.0.3/setup.cfg
+-rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-18 08:40:59.000000 struvolpy-1.0.3/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    20296 2023-07-21 12:37:23.000000 struvolpy-1.0.3/struvolpy/Structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)    22113 2023-07-23 21:32:39.000000 struvolpy-1.0.3/struvolpy/Volume.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)      132 2023-07-21 12:37:23.000000 struvolpy-1.0.3/struvolpy/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy/wrappers/
+-rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-18 14:24:41.000000 struvolpy-1.0.3/struvolpy/wrappers/__init__.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-18 15:44:06.000000 struvolpy-1.0.3/struvolpy/wrappers/wrappers.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/struvolpy.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-24 14:47:11.000000 struvolpy-1.0.3/struvolpy.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 14:47:11.577516 struvolpy-1.0.3/tests/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-18 15:14:19.000000 struvolpy-1.0.3/tests/test_structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-23 21:33:33.000000 struvolpy-1.0.3/tests/test_volume.py
```

### Comparing `struvolpy-1.0.2/LICENSE` & `struvolpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.2/PKG-INFO` & `struvolpy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.2/README.md` & `struvolpy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.2/setup.cfg` & `struvolpy-1.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = struvolpy
-version = 1.0.2
+version = 1.0.3
 author = Luc Elliott
 author_email = hllelli2@liverpool.ac.uk
 description = "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 long_description = file: ./README.md
 long_description_content_type = text/markdown
 Home-page = https://github.com/hllelli2/struvolpy/
 license = "GPLv3"
@@ -35,12 +35,15 @@
 	.gitattributes
 	.pytest_cache
 	.git
 	.vscode
 	.history
 	*.egg
 	*.egg-info
+	docs
+	site
+	mkdocs.yml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `struvolpy-1.0.2/struvolpy/Structure.py` & `struvolpy-1.0.3/struvolpy/Structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
             gemmi_structure.setup_entities()
 
             if not hetatm:
                 try:
                     gemmi_structure.remove_ligands_and_waters()
                 except RuntimeError as e:
                     logger.info("Removed ligands and waters failed, continuing")
-                    print(e)
                     pass
             if not water:
                 gemmi_structure.remove_waters()
 
             gemmi_structure.remove_empty_chains()
             # TODO: Test what would happen if there are nameless chains
             # name nameless chains
```

### Comparing `struvolpy-1.0.2/struvolpy/Volume.py` & `struvolpy-1.0.3/struvolpy/Volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,14 @@
             volume.header.mz * voxelspacing,
         )
 
         return cls(volume)
 
     @classmethod
     def from_TEMPy_map(cls, tempy_map, filename_output="VolumeFromTempy.mrc"):
-        print(type(tempy_map))
         grid = tempy_map.fullMap
 
         voxelspacing = tempy_map.apix[0]
         origin = tempy_map.origin
         return cls.from_data(grid, voxelspacing, origin, filename_output)
 
     def __init__(self, volume_parser) -> None:
@@ -237,15 +236,15 @@
             volume_parser (VolumeParser): The VolumeParser object.
         """
 
         self.__filename = volume_parser.filename
         self.__header = volume_parser.header
         vx = vy = vz = volume_parser.voxel_spacing
         self.__voxel_size = vx, vy, vz
-        self.__origin = volume_parser.origin()
+        self.__origin = tuple(volume_parser.origin().item())
         self.__grid = volume_parser.grid()
         self.__nstart = volume_parser.nstart()
         self.__simulated = False
         self.__resolution = -1.0
         self.__tempy_map = None
         self.__threshold = -1.0
 
@@ -356,39 +355,39 @@
     def origin(self) -> tuple:
         """
         Gets the origin of the Volume object.
 
         Returns:
             tuple: The origin.
         """
-        return self.__origin.item()
+        return self.__origin
 
     @origin.setter
     def origin(self, origin) -> None:
         """
         Sets the origin of the Volume object.
 
         Args:
             origin (list): The origin as a list of 3 floats or integers.
         """
         if len(origin) != 3:
             raise TypeError("origin must be a list of 3 floats or integers")
         # ox, oy, oz = origin
-        self.__origin = np.array(origin)
+        self.__origin = tuple(origin)
 
     @property
     def start(self) -> np.ndarray:
         """
         Gets the start of the Volume object.
 
         Returns:
             np.ndarray: The start.
         """
 
-        return np.array([o / self.voxelspacing for o in self.__origin.item()])
+        return np.array([o / self.voxelspacing for o in self.__origin])
 
     @start.setter
     def start(self, start: Sequence) -> None:
         """
         Sets the start of the Volume object.
 
         Args:
@@ -631,15 +630,15 @@
 
         Returns:
             None
         """
 
         self.__tempy_map = Map(
             self.__grid,
-            self.__origin.item(),
+            self.__origin,
             self.__voxel_size,
             self.__filename,
             MapParser.parseCcpemHeader(self.__header),
         )
 
     def duplicate(self) -> "Volume":
         """
```

### Comparing `struvolpy-1.0.2/struvolpy/wrappers/wrappers.py` & `struvolpy-1.0.3/struvolpy/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.2/struvolpy.egg-info/PKG-INFO` & `struvolpy-1.0.3/struvolpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.2/tests/test_structure.py` & `struvolpy-1.0.3/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.2/tests/test_volume.py` & `struvolpy-1.0.3/tests/test_volume.py`

 * *Files identical despite different names*

