# Comparing `tmp/PySolidState-0.1.3.tar.gz` & `tmp/PySolidState-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.1.3.tar", last modified: Sun Jul 23 22:16:02 2023, max compression
+gzip compressed data, was "PySolidState-0.1.4.tar", last modified: Mon Jul 24 01:49:36 2023, max compression
```

## Comparing `PySolidState-0.1.3.tar` & `PySolidState-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.805662 PySolidState-0.1.3/
--rw-rw-rw-   0        0        0     6968 2023-07-23 22:16:02.804660 PySolidState-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.735659 PySolidState-0.1.3/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.800658 PySolidState-0.1.3/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0    33211 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/cell.py
--rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    17359 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.3/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.778659 PySolidState-0.1.3/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     6968 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 22:16:02.806661 PySolidState-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-07-23 22:15:38.000000 PySolidState-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.353169 PySolidState-0.1.4/
+-rw-rw-rw-   0        0        0     6968 2023-07-24 01:49:36.351174 PySolidState-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.279169 PySolidState-0.1.4/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.345167 PySolidState-0.1.4/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0    33211 2023-07-23 22:11:15.000000 PySolidState-0.1.4/PySolidState/crystal_structure/cell.py
+-rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.4/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    17396 2023-07-24 01:46:55.000000 PySolidState-0.1.4/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.4/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.320187 PySolidState-0.1.4/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     6968 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:49:36.354176 PySolidState-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-07-24 01:49:30.000000 PySolidState-0.1.4/setup.py
```

### Comparing `PySolidState-0.1.3/PKG-INFO` & `PySolidState-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.3
+Version: 0.1.4
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero
 Author-email: miguelta281@gmail.com, jeremi0112@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.3 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.4 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
 Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
 GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.4/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.4/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/cell.py` & `PySolidState-0.1.4/PySolidState/crystal_structure/cell.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.4/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.4/PySolidState/crystal_structure/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,21 +195,22 @@
             else:
                 raise ValueError("Invalid magnitudes and angles provided for a 2D crystal lattice.")
             return system
 
         elif self.dimension == '3D':
             # Check for different magnitudes and non-90-degree angles in all three directions
             if (self.magnitude[0] != self.magnitude[1]) and (self.magnitude[0] != self.magnitude[2]) and \
-                    (self.magnitude[1] != self.magnitude[2]) and (self.angles[0] != 90) and (self.angles[1] != 90) and \
-                    (self.angles[2] != 90):
+                    (self.magnitude[1] != self.magnitude[2]) and (self.angles[0] != self.angles[1]) and (self.angles[1] != self.angles[2]) and \
+                    (self.angles[2] != self.angles[0]):
                 system = 'triclinic'
+
             # Check for different magnitudes and a 90-degree angle in two directions, and a 120-degree angle in the third direction
             elif (self.magnitude[0] != self.magnitude[1]) and (self.magnitude[0] != self.magnitude[2]) and \
-                    (self.magnitude[1] != self.magnitude[2]) and (self.angles[0] == 90) and (self.angles[1] == 90) and \
-                    (self.angles[2] == 120):
+                    (self.magnitude[1] != self.magnitude[2]) and (self.angles[0] == 90) and (self.angles[1] != 90) and \
+                    (self.angles[2] == 90):
                 system = 'monoclinic'
             # Check for different magnitudes and a 90-degree angle in all three directions
             elif (self.magnitude[0] != self.magnitude[1]) and (self.magnitude[0] != self.magnitude[2]) and \
                     (self.magnitude[1] != self.magnitude[2]) and (self.angles[0] == 90) and (self.angles[1] == 90) and \
                     (self.angles[2] == 90):
                 system = 'orthorhombic'
             # Check for equal magnitudes in two directions and a 90-degree angle in all three directions
```

### Comparing `PySolidState-0.1.3/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.1.4/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.1.4/PySolidState.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.3
+Version: 0.1.4
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero
 Author-email: miguelta281@gmail.com, jeremi0112@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.3 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.4 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
 Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
 GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySolidState-0.1.3/PySolidState.egg-info/SOURCES.txt` & `PySolidState-0.1.4/PySolidState.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/README.md` & `PySolidState-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.3/setup.py` & `PySolidState-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.1.3",
+    version="0.1.4",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero",
     author_email="miguelta281@gmail.com, jeremi0112@gmail.com",
     license="GNU General Public License v3.0",
```

