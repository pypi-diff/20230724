# Comparing `tmp/PySolidState-0.1.4.tar.gz` & `tmp/PySolidState-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.1.4.tar", last modified: Mon Jul 24 01:49:36 2023, max compression
+gzip compressed data, was "PySolidState-0.1.5.tar", last modified: Mon Jul 24 02:32:42 2023, max compression
```

## Comparing `PySolidState-0.1.4.tar` & `PySolidState-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.353169 PySolidState-0.1.4/
--rw-rw-rw-   0        0        0     6968 2023-07-24 01:49:36.351174 PySolidState-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.279169 PySolidState-0.1.4/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.345167 PySolidState-0.1.4/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.4/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0    33211 2023-07-23 22:11:15.000000 PySolidState-0.1.4/PySolidState/crystal_structure/cell.py
--rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.4/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    17396 2023-07-24 01:46:55.000000 PySolidState-0.1.4/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.4/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-24 01:49:36.320187 PySolidState-0.1.4/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     6968 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-24 01:49:35.000000 PySolidState-0.1.4/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 01:49:36.354176 PySolidState-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-07-24 01:49:30.000000 PySolidState-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.571556 PySolidState-0.1.5/
+-rw-rw-rw-   0        0        0     6968 2023-07-24 02:32:42.569568 PySolidState-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.435561 PySolidState-0.1.5/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.565558 PySolidState-0.1.5/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0    33207 2023-07-24 02:31:55.000000 PySolidState-0.1.5/PySolidState/crystal_structure/cell.py
+-rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.5/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    17396 2023-07-24 02:15:17.000000 PySolidState-0.1.5/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.5/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.510560 PySolidState-0.1.5/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     6968 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-24 02:32:42.000000 PySolidState-0.1.5/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 02:32:42.572557 PySolidState-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-07-24 02:31:59.000000 PySolidState-0.1.5/setup.py
```

### Comparing `PySolidState-0.1.4/PKG-INFO` & `PySolidState-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.4
+Version: 0.1.5
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
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.4 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.5 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
 Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
 GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.5/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.5/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/cell.py` & `PySolidState-0.1.5/PySolidState/crystal_structure/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
                 for points in points_list:
                     # Obtener las coordenadas X, Y, Z de los puntos
                     x_points, y_points, z_points = points[:,
                                                           0], points[:, 1], points[:, 2]
 
                     # Calcular el punto central del hexágono
-                    central_point = np.mean(points, axes=0)
+                    central_point = np.mean(points, axis=0)
 
                     # Crear una lista de triángulos conectando el punto central con los puntos adyacentes
                     triangles = [[i, (i+1) % len(points), len(points)]
                                  for i in range(len(points))]
 
                     # Agregar el punto central al final de las listas de coordenadas
                     x_points = np.append(x_points, central_point[0])
@@ -700,9 +700,7 @@
             center_y = ydescent + height / 2
             radius = min(width, height) / 2 * self.radius
             circle = mpatches.Circle((center_x, center_y), radius, facecolor=orig_handle.get_facecolor(),
                                     edgecolor=orig_handle.get_edgecolor(), linewidth=orig_handle.get_linewidth())
             self.update_prop(circle, orig_handle, legend)
             circle.set_transform(trans)
             return [circle]
-
-
```

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.5/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.5/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.1.5/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.1.5/PySolidState.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.1.4
+Version: 0.1.5
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
-Metadata-Version: 2.1 Name: PySolidState Version: 0.1.4 Summary: PySolidState
+Metadata-Version: 2.1 Name: PySolidState Version: 0.1.5 Summary: PySolidState
 is a library developed to facilitate the study of solid-state materials,
 ranging from crystal structures to tight-binding models. It provides a set of
 tools and functionalities that enable researchers and students to analyze and
 simulate various aspects of the solid-state physics. Home-page: https://
 github.com/miguelta281/PySolidState Author: Jose Miguel Tarazona, Yerimi Gamboa
 Caballero Author-email: miguelta281@gmail.com, jeremi0112@gmail.com License:
 GNU General Public License v3.0 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySolidState-0.1.4/PySolidState.egg-info/SOURCES.txt` & `PySolidState-0.1.5/PySolidState.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/README.md` & `PySolidState-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.4/setup.py` & `PySolidState-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.1.4",
+    version="0.1.5",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero",
     author_email="miguelta281@gmail.com, jeremi0112@gmail.com",
     license="GNU General Public License v3.0",
```

