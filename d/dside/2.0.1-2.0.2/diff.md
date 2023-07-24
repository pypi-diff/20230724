# Comparing `tmp/dside-2.0.1.tar.gz` & `tmp/dside-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dside-2.0.1.tar", last modified: Wed Feb 22 00:50:53 2023, max compression
+gzip compressed data, was "dside-2.0.2.tar", last modified: Mon Jul 24 14:09:41 2023, max compression
```

## Comparing `dside-2.0.1.tar` & `dside-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 00:50:53.760182 dside-2.0.1/
--rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     2611 2023-02-22 00:50:53.758182 dside-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2004 2023-01-09 13:10:13.000000 dside-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-22 00:50:53.760182 dside-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-02-22 00:50:02.000000 dside-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 00:50:53.702999 dside-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-22 00:50:53.731005 dside-2.0.1/src/dside/
--rw-rw-rw-   0        0        0    62011 2023-02-22 00:49:13.000000 dside-2.0.1/src/dside/DSI.py
--rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.0.1/src/dside/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 00:50:53.756181 dside-2.0.1/src/dside.egg-info/
--rw-rw-rw-   0        0        0     2611 2023-02-22 00:50:53.000000 dside-2.0.1/src/dside.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-02-22 00:50:53.000000 dside-2.0.1/src/dside.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 00:50:53.000000 dside-2.0.1/src/dside.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-22 00:50:53.000000 dside-2.0.1/src/dside.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-22 00:50:53.000000 dside-2.0.1/src/dside.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.605594 dside-2.0.2/
+-rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2653 2023-07-24 14:09:41.604599 dside-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2023-03-11 12:37:11.000000 dside-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:09:41.605594 dside-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-07-24 14:04:37.000000 dside-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.582662 dside-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.588640 dside-2.0.2/src/dside/
+-rw-rw-rw-   0        0        0    62364 2023-07-24 13:59:31.000000 dside-2.0.2/src/dside/DSI.py
+-rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.0.2/src/dside/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.603602 dside-2.0.2/src/dside.egg-info/
+-rw-rw-rw-   0        0        0     2653 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/top_level.txt
```

### Comparing `dside-2.0.1/LICENSE` & `dside-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dside-2.0.1/PKG-INFO` & `dside-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.0.1
+Version: 2.0.2
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
@@ -21,21 +21,21 @@
 [![PyPI](https://img.shields.io/pypi/v/dside.svg)](https://pypi.org/project/dside)
 [![Downloads](https://pepy.tech/badge/dside)](https://pepy.tech/project/dside)
 
 Design space identification tool for plotting and analysing design spaces (2D and 3D). Constraints with respect to key performance indicators (KPIs) are used to categorize the samples. Concave hulls (alpha shape) are used to identify design space (DSp) and quantify the size of the space. Given nominal operating point (NOP), an acceptable operating region (AOR) can be quantified to find the maximum multivariate allowable disturbance that the process can still handle while satisfying all constraints (multivariate proven acceptable range - MPAR).
 
 
 ## Installation
-Currently, dside requires pandas, numpy, matplotlib, and shapely. dside can be installed with the following commands.
+Currently, dside requires pandas, numpy, and matplotlib. dside can be installed with the following commands.
 ```bash
 pip install dside
 ```
 
 ## Quick Overview
-Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges).
+Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges). Identification of multi-region spaces is possible.
 
 ```
 import dside
 # 1. Create instance of ds with data from DataFrame df
 ds = dside.DSI(df)
 # 2. Screen the points using the constraints (dictionary)
 ds.screen(constraints)
```

### Comparing `dside-2.0.1/README.md` & `dside-2.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 [![PyPI](https://img.shields.io/pypi/v/dside.svg)](https://pypi.org/project/dside)
 [![Downloads](https://pepy.tech/badge/dside)](https://pepy.tech/project/dside)
 
 Design space identification tool for plotting and analysing design spaces (2D and 3D). Constraints with respect to key performance indicators (KPIs) are used to categorize the samples. Concave hulls (alpha shape) are used to identify design space (DSp) and quantify the size of the space. Given nominal operating point (NOP), an acceptable operating region (AOR) can be quantified to find the maximum multivariate allowable disturbance that the process can still handle while satisfying all constraints (multivariate proven acceptable range - MPAR).
 
 
 ## Installation
-Currently, dside requires pandas, numpy, matplotlib, and shapely. dside can be installed with the following commands.
+Currently, dside requires pandas, numpy, and matplotlib. dside can be installed with the following commands.
 ```bash
 pip install dside
 ```
 
 ## Quick Overview
-Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges).
+Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges). Identification of multi-region spaces is possible.
 
 ```
 import dside
 # 1. Create instance of ds with data from DataFrame df
 ds = dside.DSI(df)
 # 2. Screen the points using the constraints (dictionary)
 ds.screen(constraints)
```

### Comparing `dside-2.0.1/setup.py` & `dside-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 short_description = 'Design space identification tool for plotting and analysing design'+\
     ' spaces (2D and 3D).'
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name = 'dside',
@@ -26,9 +26,9 @@
     packages = find_packages(where = 'src'), # List of all python modules to be installed
     package_dir = {'': 'src'},
     python_requires='>=3.9',                 # Minimum version requirement of the package
     py_modules=['dside'],                    # Name of the python package
     install_requires=['numpy',
                       'matplotlib',
                       'pandas',
-                      'shapely']              # Install other dependencies if any
+                     ]              # Install other dependencies if any
 )
```

### Comparing `dside-2.0.1/src/dside/DSI.py` & `dside-2.0.2/src/dside/DSI.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,19 +107,20 @@
         self.default_opt = {
             # ----- Saving Options ----- #
             'save_flag': False, # If True, then figure will be saved
             'save_name': 'test.jpg', # save file name including path
             'save_dpi': 480, # save dpi
             
             # ----- Labels ----- #
-            'xlabel': 'x',       # x axis label
-            'ylabel': 'y',       # y axis label
-            'zlabel': 'z',       # z axis label
-            'cmap': 'inferno80', # Matplotlib colour map
-            'hmv': 'None',       # heat map variable name
+            'xlabel': 'x',          # x axis label
+            'ylabel': 'y',          # y axis label
+            'zlabel': 'z',          # z axis label
+            'labelpad': [8, 8, 8],  # Label padding
+            'cmap': 'inferno80',    # Matplotlib colour map
+            'hmv': 'None',          # heat map variable name
             'hmvlabel': 'hmvlabel: heat map var label', # heat map variable label
             
             # ----- Hidden Elements ----- #
             'hidehmv': False, # If True, no heat map will be plotted
             'hidesat': False, # If True, no satisfied variables will be plotted
             'hidevio': False, # If True, no violated variables will be plotted
             'hidedsp': False, # If True, hides the surface/boundary
@@ -307,15 +308,20 @@
         if self.opt['bw']:
             self.opt.update(self.bw_template)
         self.opt.update(opt)
         
         # ---------------------------- External definitions ---------------------------- #
         sat = self.sat
         vio = self.vio
-        opt = self.opt    
+        opt = self.opt
+        labelpad = opt['labelpad']
+        if type(labelpad) == int:
+            labelpad = [labelpad]
+        if len(labelpad) == 1:
+            labelpad *= 3
         plt.rcParams.update({'font.size': opt['font_size']})
         
         # ----------------------------- Heat map Variable ----------------------------- #
         hmv_R = {'name': opt['hmv'], 'mean': '-', 'max': '-', 'max_sample': '-', \
             'min': '-',  'min_sample': '-'}
         if opt['hmv'] != 'None':
             if opt['hidesat']:
@@ -415,20 +421,20 @@
             shp = self.shp
             if dim == 2:
                 for i in range(len(shp['reg_bounds_val'])):
                     if i == 0:
                         plt.plot(*zip(*shp['reg_bounds_val'][i]),\
                             linewidth = opt['dspwidth'], linestyle = opt['dspstyle'],\
                             color = opt['dspcolor'], label = opt['dsplabel'],\
-                            zorder = opt['dspzorder'])
+                            zorder = opt['dspzorder'], solid_capstyle = 'round')
                     else:
                         plt.plot(*zip(*shp['reg_bounds_val'][i]),\
                             linewidth = opt['dspwidth'], linestyle = opt['dspstyle'],\
                             color = opt['dspcolor'],\
-                            zorder = opt['dspzorder'])
+                            zorder = opt['dspzorder'], solid_capstyle = 'round')
 
             if dim == 3:
                 for i in range(len(shp['reg_bounds'])):
                     if i == 0:
                         surf = ax.plot_trisurf(*zip(*shp['P']), triangles = shp['reg_bounds'][i], \
                             color = opt['dspcolor'],\
                             alpha = opt['dspalpha'], label = opt['dsplabel'],\
@@ -464,18 +470,18 @@
                 ax.set_ylim([vmin[1] - limfactor*vrange[1],\
                     vmax[1] + limfactor*vrange[1]])
                 ax.set_zlim([vmin[2] - limfactor*vrange[2],\
                     vmax[2] + limfactor*vrange[2]])
         
         
         # Labels
-        plt.xlabel(opt['xlabel'])
-        plt.ylabel(opt['ylabel'])
+        plt.xlabel(opt['xlabel'], labelpad = labelpad[0])
+        plt.ylabel(opt['ylabel'], labelpad = labelpad[1])
         if dim == 3:
-            ax.set_zlabel(opt['zlabel'])
+            ax.set_zlabel(opt['zlabel'], labelpad = labelpad[3])
             ax.view_init(elev = opt['elev'], azim = opt['azim'])
         if (opt['hmv'] == 'None') or (opt['hidehmv'] == True):
             plt.legend(loc = opt['legloc'],\
                 framealpha = opt['framealpha']).set_zorder(opt['legendzorder'])
         
         # Saving
         plt.tight_layout()
```

### Comparing `dside-2.0.1/src/dside.egg-info/PKG-INFO` & `dside-2.0.2/src/dside.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.0.1
+Version: 2.0.2
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
@@ -21,21 +21,21 @@
 [![PyPI](https://img.shields.io/pypi/v/dside.svg)](https://pypi.org/project/dside)
 [![Downloads](https://pepy.tech/badge/dside)](https://pepy.tech/project/dside)
 
 Design space identification tool for plotting and analysing design spaces (2D and 3D). Constraints with respect to key performance indicators (KPIs) are used to categorize the samples. Concave hulls (alpha shape) are used to identify design space (DSp) and quantify the size of the space. Given nominal operating point (NOP), an acceptable operating region (AOR) can be quantified to find the maximum multivariate allowable disturbance that the process can still handle while satisfying all constraints (multivariate proven acceptable range - MPAR).
 
 
 ## Installation
-Currently, dside requires pandas, numpy, matplotlib, and shapely. dside can be installed with the following commands.
+Currently, dside requires pandas, numpy, and matplotlib. dside can be installed with the following commands.
 ```bash
 pip install dside
 ```
 
 ## Quick Overview
-Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges).
+Use this tool to visualize 2D and 3D design spaces, obtain mathematical representations of the design space boundary in the form of alpha shapes, calculate the size of the design space, and investigate nominal operating points in terms of performance and flexibility (acceptable ranges). Identification of multi-region spaces is possible.
 
 ```
 import dside
 # 1. Create instance of ds with data from DataFrame df
 ds = dside.DSI(df)
 # 2. Screen the points using the constraints (dictionary)
 ds.screen(constraints)
```

