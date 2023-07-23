# Comparing `tmp/PySolidState-0.1.2.tar.gz` & `tmp/PySolidState-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.1.2.tar", last modified: Tue Jul 18 20:35:02 2023, max compression
+gzip compressed data, was "PySolidState-0.1.3.tar", last modified: Sun Jul 23 22:16:02 2023, max compression
```

## Comparing `PySolidState-0.1.2.tar` & `PySolidState-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:35:02.029773 PySolidState-0.1.2/
--rw-rw-rw-   0        0        0     6955 2023-07-18 20:35:02.025774 PySolidState-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 20:35:01.950770 PySolidState-0.1.2/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:35:02.021773 PySolidState-0.1.2/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7632 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7052 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16788 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-18 20:35:01.995776 PySolidState-0.1.2/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     6955 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6056 2023-07-18 20:34:24.000000 PySolidState-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 20:35:02.029773 PySolidState-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1380 2023-07-18 20:34:51.000000 PySolidState-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.805662 PySolidState-0.1.3/
+-rw-rw-rw-   0        0        0     6968 2023-07-23 22:16:02.804660 PySolidState-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.735659 PySolidState-0.1.3/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.800658 PySolidState-0.1.3/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.3/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0    33211 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/cell.py
+-rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    17359 2023-07-23 22:11:15.000000 PySolidState-0.1.3/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.3/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-23 22:16:02.778659 PySolidState-0.1.3/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     6968 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-23 22:16:02.000000 PySolidState-0.1.3/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-23 22:16:02.806661 PySolidState-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-07-23 22:15:38.000000 PySolidState-0.1.3/setup.py
```

### Comparing `PySolidState-0.1.2/PKG-INFO` & `PySolidState-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.2
+Version: 0.1.3
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
-Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
-Author-email: makesens19@gmail.com
+Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero
+Author-email: miguelta281@gmail.com, jeremi0112@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 <h1 align="center"> <a href="https://imgur.com/L01ipPl"><img src="https://i.imgur.com/L01ipPl.png" title="source: imgur.com" /></a>
   
@@ -104,8 +104,7 @@
 base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
 
 # Se crea la estructura cristalina o cristal uniendo la red y la base ya creadas
 crs = CrystalStructure(lattice=lattice, base=base, dimension='3D')
 #Se crea la figura de la red cristalina o cristal Na+Cl- (Cloruro de Sodio)
 crs.plot()
 ```
-
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.2 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.3 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
-Caballero, Felipe Author-email: makesens19@gmail.com License: GNU General
-Public License v3.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
+GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown
       ****** [https://i.imgur.com/L01ipPl.png]PySolidState (PySS) ******
 >PySS es una biblioteca desarrollada como una herramienta de apoyo para el
 estudio introductorio del estado sÃÂ³lido y los conceptos bÃÂ¡sicos de los
 materiales. Su enfoque principal es proporcionar apoyo visual y funcionalidades
 que permitan asentar los conceptos fundamentales en esta ÃÂ¡rea de estudio,
 desde estructuras cristalinas hasta modelos de enlace fuerte. Con un conjunto
 de herramientas y funcionalidades, PySolidState permite a investigadores y
```

### Comparing `PySolidState-0.1.2/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.3/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.2/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.3/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.2/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.3/PySolidState/crystal_structure/crystalStructure.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,14 +68,21 @@
             if self.dimension == '2D':
                 fig = plt.figure()
 
                 ax = fig.add_subplot(111, aspect='equal')
                 # Scatter plot of the points
                 ax.scatter(self.lattice.points[:, 0],
                         self.lattice.points[:, 1], color='black', s=1)
+
+                ax.quiver(0, 0, self.lattice.vectors[0][0], self.lattice.vectors[0][1],  angles='xy', scale_units='xy', scale=1, color='black')
+                ax.quiver(0, 0, self.lattice.vectors[1][0], self.lattice.vectors[1][1],  angles='xy', scale_units='xy', scale=1, color='black')
+
+                # Show the names of the vectors
+                ax.text(self.lattice.vectors[0][0] + 0.3, self.lattice.vectors[0][1], r"$\vec{a_1}$", fontsize=12, color='black', ha='center', va='center')
+                ax.text(self.lattice.vectors[1][0], self.lattice.vectors[1][1] + 0.3, r"$\vec{a_2}$", fontsize=12, color='black', ha='center', va='center')
                 
                 handles, labels = ax.get_legend_handles_labels()
                 unique_atom_names = set(labels)
 
                 for atom in self.base.atoms:
                     atom_name = atom[0].name
                     circle = patches.Circle((atom[1][0], atom[1][1]), radius=atom[0].size, facecolor=atom[0].color, edgecolor=atom[0].color, alpha=0.5, label=atom_name)
@@ -102,21 +109,31 @@
 
                 mlab.figure(bgcolor=(1, 1, 1))
 
                 unique_atom_names = []
                 count = 0
                 for atom in atoms:
                     self._plot_sphere(atom[1][0],atom[1][1],atom[1][2], r=atom[0].size, color_name= atom[0].color )
+                    # Mostraar los nombres de los atomos
                     if atom[0].name not in unique_atom_names:
                         unique_atom_names.append(atom[0].name)
                         self._plot_sphere(3,3.5,3.5-count, r=atom[0].size, color_name= atom[0].color )
                         mlab.text3d(3,3.5+atom[0].size,3.5-atom[0].size -count, atom[0].name, color=(0, 0, 0), scale=0.2)
 
                         count += 2* atom[0].size
 
+                # Mostar los vectores base
+                for vector in self.lattice.vectors:
+                    mlab.quiver3d(0, 0, 0, vector[0], vector[1], vector[2], color=(0, 0, 0), scale_factor=1)
+                    
+                mlab.text3d( self.lattice.vectors[0][0], self.lattice.vectors[0][1], self.lattice.vectors[0][2], 'a1', color=(0, 0, 0), scale=0.2)
+                mlab.text3d( self.lattice.vectors[1][0], self.lattice.vectors[1][1], self.lattice.vectors[1][2], 'a2', color=(0, 0, 0), scale=0.2)
+                mlab.text3d( self.lattice.vectors[2][0], self.lattice.vectors[2][1], self.lattice.vectors[2][2], 'a3', color=(0, 0, 0), scale=0.2)
+
+
                 mlab.show()
 
 
         elif (plot_lattice == True) and (plot_base == False):
             self.lattice.plot()
         elif (plot_lattice==False) and (plot_base == True):
             self.base.plot()
```

### Comparing `PySolidState-0.1.2/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.3/PySolidState/crystal_structure/lattice.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mpl_toolkits.mplot3d import Axes3D
 import json
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 import pkg_resources
 
 
 class Lattice:
-    def __init__(self, system: str = None, structure_type: str = None, magnitude: tuple = None, angles: tuple = None, dimension: str = '2D'):
+    def __init__(self, system: str = None, structure_type: str = None, magnitude: tuple = None, angles: tuple = None,dimension: str = '2D', size:int = 1):
 
         """
         Constructor of the Lattice class that represents a crystalline lattice in a three-dimensional system.
 
         Parameters:
 
         system (str): The predefined system to be used. If provided, the magnitude and angles parameters will be ignored.
@@ -21,40 +21,49 @@
         dimension (str): Dimension of the lattice. By default, it is '2D'.
 
         Note: Either 'system' or 'magnitude' and 'angles' must be provided.
 
         """
         
         self.dimension = dimension
-        self.__system = system
-        self.__structure_type = structure_type
+        self.system = system
+        self.structure_type = structure_type
+        self.__size =  size
+
+        # Limitar el tamaño a 3
+        if self.__size > 3:
+            self.__size = 3
+
+        # Garantiza que el menor tamaño seaa 1
+        elif self.__size < 1:
+            self.__size = 1
 
         # Verificar si se van a utilizar sistemas predefinidos
         if system is not None:
             file_path = pkg_resources.resource_filename('PySolidState', 'crystal_structure/lattices.json')
 
             # Leer el archivo
             with open(file_path) as file:
                 lattices = json.load(file)
             
-            self.magnitude = lattices[self.dimension][self.__system]['magnitude']
-            self.angles = lattices[self.dimension][self.__system]['angles']
+            self.magnitude = lattices[self.dimension][self.system]['magnitude']
+            self.angles = lattices[self.dimension][self.system]['angles']
             if dimension == '2D':
-                self.__angles_radian = tuple(np.math.radians(degree) for degree in (90,90,lattices[self.dimension][self.__system]['angles'][2]))
+                self.__angles_radian = tuple(np.math.radians(degree) for degree in (90,90,lattices[self.dimension][self.system]['angles'][2]))
             else:
-                self.__angles_radian = tuple(np.math.radians(degree) for degree in lattices[self.dimension][self.__system]['angles'])
+                self.__angles_radian = tuple(np.math.radians(degree) for degree in lattices[self.dimension][self.system]['angles'])
         # Evaluate if magnitudes and angles have been defined.
         elif (magnitude is not None) and (angles is not None):
             self.magnitude = magnitude
             self.angles = angles
             if dimension == '2D':
                 angles = (90,90,angles[2])
             self.__angles_radian = tuple(
                 np.math.radians(degree) for degree in angles)
-            self.__system = self._get_system() # Assign a system based on the angles and magnitudes.
+            self.system = self._get_system() # Assign a system based on the angles and magnitudes.
             
         else:
             raise ValueError("You must provide either 'system' or 'magnitude' and 'angles'")
 
         self.points = self._create_points()
 
         # Base vectors
@@ -243,44 +252,48 @@
 
         # Generate the range of values for each axis
         if self.dimension == '2D':
             v1_range = np.arange(-5, 5)
             v2_range = np.arange(-5, 5)
             v3_range = np.arange(0, 1)
         else:
-            v1_range = np.arange(-1, 3)
-            v2_range = np.arange(-1, 3)
-            v3_range = np.arange(-1, 3)
-
-        # Create the meshgrid of points
+            if self.__size == 1:
+                v1_range = np.arange(1- self.__size,1 + self.__size)
+                v2_range = np.arange(1- self.__size,1 + self.__size)
+                v3_range = np.arange(1- self.__size,1 + self.__size)
+            else:
+                v1_range = np.arange(1- self.__size,0 + self.__size)
+                v2_range = np.arange(1- self.__size,0 + self.__size)
+                v3_range = np.arange(1- self.__size,0 + self.__size)
+            # Create the meshgrid of points
         v1, v2, v3 = np.meshgrid(v1_range, v2_range, v3_range)
 
         # Combine the points into a single array
         points_v = np.vstack([v1.ravel(), v2.ravel(), v3.ravel()]).T
 
 
         file_path = pkg_resources.resource_filename('PySolidState', 'crystal_structure/lattices.json')
 
         # Leer el archivo
         with open(file_path) as file:
             lattices = json.load(file)
 
-        if (self.__structure_type is not None):
-            if (self.__structure_type in lattices[self.dimension][self.__system]['structure_type']):
-                if self.__structure_type == 'centered':
+        if (self.structure_type is not None):
+            if (self.structure_type in lattices[self.dimension][self.system]['structure_type']):
+                if self.structure_type == 'centered':
                     v1_centered, v2_centered, v3_centered = np.meshgrid(v1_range + 0.5, v2_range + 0.5, v3_range)
                     points_centered = np.vstack([v1_centered.ravel(), v2_centered.ravel(), v3_centered.ravel()]).T
                     points_v = np.concatenate((points_v, points_centered), axis=0)
                 
-                elif self.__structure_type == 'body_centered':
+                elif self.structure_type == 'body_centered':
                     v1_centered, v2_centered, v3_centered = np.meshgrid(v1_range + 0.5, v2_range + 0.5, v3_range + 0.5)
                     points_centered = np.vstack([v1_centered.ravel(), v2_centered.ravel(), v3_centered.ravel()]).T
                     points_v = np.concatenate((points_v, points_centered), axis=0)
 
-                elif self.__structure_type == 'face_centered':
+                elif self.structure_type == 'face_centered':
                     # Face 1
                     v1_c1, v2_c1, v3_c1 = np.meshgrid(v1_range + 0.5, v2_range + 0.5, v3_range)
                     points_c1 = np.vstack([v1_c1.ravel(), v2_c1.ravel(), v3_c1.ravel()]).T
                     points_v = np.concatenate((points_v, points_c1), axis=0)
 
                     # Face 2
                     v1_c2, v2_c2, v3_c2 = np.meshgrid(v1_range + 0.5, v2_range, v3_range + 0.5)
@@ -289,15 +302,15 @@
 
                     # Face 3
                     v1_c3, v2_c3, v3_c3 = np.meshgrid(v1_range, v2_range + 0.5, v3_range + 0.5)
                     points_c3 = np.vstack([v1_c3.ravel(), v2_c3.ravel(), v3_c3.ravel()]).T
                     points_v = np.concatenate((points_v, points_c3), axis=0)
 
                     
-                elif self.__structure_type == 'base_centered':
+                elif self.structure_type == 'base_centered':
                     v1_centered, v2_centered, v3_centered = np.meshgrid(v1_range + 0.5, v2_range + 0.5, v3_range)
                     points_centered = np.vstack([v1_centered.ravel(), v2_centered.ravel(), v3_centered.ravel()]).T
                     points_v = np.concatenate((points_v, points_centered), axis=0)
 
             else:
                 raise ValueError('The structure_type does not correspond to this system')
```

### Comparing `PySolidState-0.1.2/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.1.3/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.2/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.1.3/PySolidState.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.2
+Version: 0.1.3
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
-Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
-Author-email: makesens19@gmail.com
+Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero
+Author-email: miguelta281@gmail.com, jeremi0112@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 <h1 align="center"> <a href="https://imgur.com/L01ipPl"><img src="https://i.imgur.com/L01ipPl.png" title="source: imgur.com" /></a>
   
@@ -104,8 +104,7 @@
 base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
 
 # Se crea la estructura cristalina o cristal uniendo la red y la base ya creadas
 crs = CrystalStructure(lattice=lattice, base=base, dimension='3D')
 #Se crea la figura de la red cristalina o cristal Na+Cl- (Cloruro de Sodio)
 crs.plot()
 ```
-
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.2 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.3 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
-Caballero, Felipe Author-email: makesens19@gmail.com License: GNU General
-Public License v3.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
+GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown
       ****** [https://i.imgur.com/L01ipPl.png]PySolidState (PySS) ******
 >PySS es una biblioteca desarrollada como una herramienta de apoyo para el
 estudio introductorio del estado sÃÂ³lido y los conceptos bÃÂ¡sicos de los
 materiales. Su enfoque principal es proporcionar apoyo visual y funcionalidades
 que permitan asentar los conceptos fundamentales en esta ÃÂ¡rea de estudio,
 desde estructuras cristalinas hasta modelos de enlace fuerte. Con un conjunto
 de herramientas y funcionalidades, PySolidState permite a investigadores y
```

### Comparing `PySolidState-0.1.2/README.md` & `PySolidState-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,98 @@
-<h1 align="center"> <a href="https://imgur.com/L01ipPl"><img src="https://i.imgur.com/L01ipPl.png" title="source: imgur.com" /></a>
-  
-<h1 align="center"> PySolidState (PySS) </h1>
-
->PySS es una biblioteca desarrollada como una herramienta de apoyo para el estudio introductorio del estado sólido y los conceptos básicos de los materiales. Su enfoque principal es proporcionar apoyo visual y funcionalidades que permitan asentar los conceptos fundamentales en esta área de estudio, desde estructuras cristalinas hasta modelos de enlace fuerte. Con un conjunto de herramientas y funcionalidades, PySolidState permite a investigadores y estudiantes analizar y simular varios aspectos de la física del estado sólido. Además, esta biblioteca se combina con notas de curso sobre estado sólido, lo que la convierte en un recurso bastante completo para el aprendizaje de la materia a nivel universitario. Gracias a su enfoque en la visualización y el apoyo práctico, PySolidState se convierte en una valiosa herramienta que, junto con las notas de curso, ofrece una base sólida para comprender los principios y fundamentos del estado sólido.
-
-**Deployment**
-
-![PyPI](https://img.shields.io/pypi/v/PySolidState)
-
-## Recursos
-- Documentación
-- Notas del curso de estado solido
-
-## Instalación
-Se recomienda utilizar pip para la instalación. Asegúrese de que la última versión esté instalada, ya que PySS se actualiza con frecuencia:
-
->Nota: Es importante antes de instalar la libreria PySolidState haber ejecutado la consola en modo administrador si se trabajara con jupyter notebook.
-
-ejecute los siguientes comando para la instalación:
-```python
-   pip install PySolidState    # Instalacion normal
-   pip install --upgrade PySolidState  # o actualizar si es necesario
-```
-**Dependencias Requeridas:**
-- Python 3.9+
-- matplotlib >=3.7.1
-- numpy>=1.24.3
-- mayavi>=4.7.2
-- scikit-spatial>=7.0.0
-
-## Uso
-### Crear Red (Create Lattice):
-Uno de los conceptos mas basico y fundamental en el estado solido es el de red, siendo las unicas posibles en formar estructuras cistalinas las redes de Bravais; para crea una de estas tenemos dos formas de hacerlo:
-
-**1)** Construyendo la red a partir de los parámetros ***System*** (nombre de una de las redes de Brabais),  ***structure_type*** (Si la red tiene centrada en las caras, centrada en el cuerpo o centrada en las bases) y ***dimension*** (dimensión en la cual se creara la red 2D o 3D). A continuación se muestra un ejemplo de uso:
-```python
-from PySolidState.crystal_structure.lattice import Lattice  # Importamos el modulo estructura cristalina de la libreria junto al metodo lattices
-
-lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D') # Se crea la red
-lattice.plot()  # Se grafica la red
-```
-**2)** Construyendo la red a partir de los parámetros ***magnitude*** (tupla con la norma de cada uno de los vectores de la red a1, a2 y a3),  ***angles*** (tupla con los angulos que describen los vectores de la red (Gama, Alfa, Beta)) y ***dimension*** (dimensión en la cual se creara la red 2D o 3D). A continuación se muestra un ejemplo de uso:
-```python
-from PySolidState.crystal_structure.lattice import Lattice  # Importamos el modulo estructura cristalina de la libreria junto al metodo lattices
-
-lattice = Lattice(magnitude=(1,1,1),angles=(90,90,90), dimension='3D') # Se crea la red
-lattice.plot()  # Se grafica la red
-```
-### Crear base (Create base):
-El otro concepto más básico es el de base, siendo esta base el conjunto de átomos que se acomodan en cada punto de red para formar la estructura cristalina. A continuación se muestra un ejemplo de como crear esta base de átomos:
-
-```python
-# Se importan los módulos Lattice, Atom, Base
-from PySolidState.crystal_structure.lattice import Lattice
-from PySolidState.crystal_structure.atom import Atom
-from PySolidState.crystal_structure.base import Base
-
-#Se crean los átomos que harán parte de la base de átomos
-atom2 = Atom(name='Na+', size= 0.2, color= 'orangered')
-atom1 = Atom(name='Cl-', size= 0.3, color= 'springgreen')
-
-#Se crea la red a la cual se acomodaran
-lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D')
-
-# Se crea la base de átomos
-base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
-
-#Se grafica la base de atomos en un punto de red
-base.plot()
-```
-Como notamos en el ejemplo la clase Base se inicializa pasándole los vectores de la red, una lista que contiene listas de los átomos creados, con su vector posición en la base a formar y la dimensión en la que se describirá.
-
-### Crear estructurá cristalina
-Con los dos conceptos previamente mostrados podemos formar lo que se conoce como estructura cristalina o cristal, siendo esta estructura la unión de una red de Bravais con una base de átomos, para ello a continuación se muestra un ejemplo de como construirla:
-
-```python
-# Se importan los modulos Lattice, Atom, Base y CristalStruture.
-%matplotlib widget
-from PySolidState.crystal_structure.lattice import Lattice
-from PySolidState.crystal_structure.atom import Atom
-from PySolidState.crystal_structure.base import Base
-from PySolidState.crystal_structure.crystalStructure import CrystalStructure
-
-#Se crean los átomos que harán parte de la base de átomos.
-atom2 = Atom(name='Na+', size= 0.2, color= 'orangered')
-atom1 = Atom(name='Cl-', size= 0.3, color= 'springgreen')
-
-#Se crea la red de Bravais en la cual se acomodara la base de atomos.
-lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D')
-# Se crea la base de átomos
-base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
-
-# Se crea la estructura cristalina o cristal uniendo la red y la base ya creadas
-crs = CrystalStructure(lattice=lattice, base=base, dimension='3D')
-#Se crea la figura de la red cristalina o cristal Na+Cl- (Cloruro de Sodio)
-crs.plot()
-```
-
+<h1 align="center"> <a href="https://imgur.com/L01ipPl"><img src="https://i.imgur.com/L01ipPl.png" title="source: imgur.com" /></a>
+  
+<h1 align="center"> PySolidState (PySS) </h1>
+
+>PySS es una biblioteca desarrollada como una herramienta de apoyo para el estudio introductorio del estado sólido y los conceptos básicos de los materiales. Su enfoque principal es proporcionar apoyo visual y funcionalidades que permitan asentar los conceptos fundamentales en esta área de estudio, desde estructuras cristalinas hasta modelos de enlace fuerte. Con un conjunto de herramientas y funcionalidades, PySolidState permite a investigadores y estudiantes analizar y simular varios aspectos de la física del estado sólido. Además, esta biblioteca se combina con notas de curso sobre estado sólido, lo que la convierte en un recurso bastante completo para el aprendizaje de la materia a nivel universitario. Gracias a su enfoque en la visualización y el apoyo práctico, PySolidState se convierte en una valiosa herramienta que, junto con las notas de curso, ofrece una base sólida para comprender los principios y fundamentos del estado sólido.
+
+**Deployment**
+
+![PyPI](https://img.shields.io/pypi/v/PySolidState)
+
+## Recursos
+- Documentación
+- Notas del curso de estado solido
+
+## Instalación
+Se recomienda utilizar pip para la instalación. Asegúrese de que la última versión esté instalada, ya que PySS se actualiza con frecuencia:
+
+>Nota: Es importante antes de instalar la libreria PySolidState haber ejecutado la consola en modo administrador si se trabajara con jupyter notebook.
+
+ejecute los siguientes comando para la instalación:
+```python
+   pip install PySolidState    # Instalacion normal
+   pip install --upgrade PySolidState  # o actualizar si es necesario
+```
+**Dependencias Requeridas:**
+- Python 3.9+
+- matplotlib >=3.7.1
+- numpy>=1.24.3
+- mayavi>=4.7.2
+- scikit-spatial>=7.0.0
+
+## Uso
+### Crear Red (Create Lattice):
+Uno de los conceptos mas basico y fundamental en el estado solido es el de red, siendo las unicas posibles en formar estructuras cistalinas las redes de Bravais; para crea una de estas tenemos dos formas de hacerlo:
+
+**1)** Construyendo la red a partir de los parámetros ***System*** (nombre de una de las redes de Brabais),  ***structure_type*** (Si la red tiene centrada en las caras, centrada en el cuerpo o centrada en las bases) y ***dimension*** (dimensión en la cual se creara la red 2D o 3D). A continuación se muestra un ejemplo de uso:
+```python
+from PySolidState.crystal_structure.lattice import Lattice  # Importamos el modulo estructura cristalina de la libreria junto al metodo lattices
+
+lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D') # Se crea la red
+lattice.plot()  # Se grafica la red
+```
+**2)** Construyendo la red a partir de los parámetros ***magnitude*** (tupla con la norma de cada uno de los vectores de la red a1, a2 y a3),  ***angles*** (tupla con los angulos que describen los vectores de la red (Gama, Alfa, Beta)) y ***dimension*** (dimensión en la cual se creara la red 2D o 3D). A continuación se muestra un ejemplo de uso:
+```python
+from PySolidState.crystal_structure.lattice import Lattice  # Importamos el modulo estructura cristalina de la libreria junto al metodo lattices
+
+lattice = Lattice(magnitude=(1,1,1),angles=(90,90,90), dimension='3D') # Se crea la red
+lattice.plot()  # Se grafica la red
+```
+### Crear base (Create base):
+El otro concepto más básico es el de base, siendo esta base el conjunto de átomos que se acomodan en cada punto de red para formar la estructura cristalina. A continuación se muestra un ejemplo de como crear esta base de átomos:
+
+```python
+# Se importan los módulos Lattice, Atom, Base
+from PySolidState.crystal_structure.lattice import Lattice
+from PySolidState.crystal_structure.atom import Atom
+from PySolidState.crystal_structure.base import Base
+
+#Se crean los átomos que harán parte de la base de átomos
+atom2 = Atom(name='Na+', size= 0.2, color= 'orangered')
+atom1 = Atom(name='Cl-', size= 0.3, color= 'springgreen')
+
+#Se crea la red a la cual se acomodaran
+lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D')
+
+# Se crea la base de átomos
+base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
+
+#Se grafica la base de atomos en un punto de red
+base.plot()
+```
+Como notamos en el ejemplo la clase Base se inicializa pasándole los vectores de la red, una lista que contiene listas de los átomos creados, con su vector posición en la base a formar y la dimensión en la que se describirá.
+
+### Crear estructurá cristalina
+Con los dos conceptos previamente mostrados podemos formar lo que se conoce como estructura cristalina o cristal, siendo esta estructura la unión de una red de Bravais con una base de átomos, para ello a continuación se muestra un ejemplo de como construirla:
+
+```python
+# Se importan los modulos Lattice, Atom, Base y CristalStruture.
+%matplotlib widget
+from PySolidState.crystal_structure.lattice import Lattice
+from PySolidState.crystal_structure.atom import Atom
+from PySolidState.crystal_structure.base import Base
+from PySolidState.crystal_structure.crystalStructure import CrystalStructure
+
+#Se crean los átomos que harán parte de la base de átomos.
+atom2 = Atom(name='Na+', size= 0.2, color= 'orangered')
+atom1 = Atom(name='Cl-', size= 0.3, color= 'springgreen')
+
+#Se crea la red de Bravais en la cual se acomodara la base de atomos.
+lattice = Lattice(system='cubic',structure_type='face_centered', dimension='3D')
+# Se crea la base de átomos
+base = Base(lattice_vectors= lattice.vectors, atoms=[[atom1, [0,0,0]],[atom2, [0.5,0,0]],[atom2, [0,0.5,0]],[atom2, [0,0,0.5]]], dimension='3D')
+
+# Se crea la estructura cristalina o cristal uniendo la red y la base ya creadas
+crs = CrystalStructure(lattice=lattice, base=base, dimension='3D')
+#Se crea la figura de la red cristalina o cristal Na+Cl- (Cloruro de Sodio)
+crs.plot()
+```
```

### Comparing `PySolidState-0.1.2/setup.py` & `PySolidState-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.1.2",
+    version="0.1.3",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
-    author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
-    author_email="makesens19@gmail.com",
+    author="Jose Miguel Tarazona, Yerimi Gamboa Caballero",
+    author_email="miguelta281@gmail.com, jeremi0112@gmail.com",
     license="GNU General Public License v3.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     package_data={
     'PySolidState': ['crystal_structure/lattices.json'],
     },
     packages=["PySolidState", "PySolidState.crystal_structure"],
     include_package_data=True,
     data_files=[('data', ['PySolidState/crystal_structure/lattices.json'])],
 
-    install_requires=["numpy", "matplotlib","mayavi","ipympl"]
+    install_requires=["numpy", "matplotlib","mayavi","ipympl","scipy"]
 )
```

