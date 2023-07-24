# Comparing `tmp/dside-2.0.2.tar.gz` & `tmp/dside-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dside-2.0.2.tar", last modified: Mon Jul 24 14:09:41 2023, max compression
+gzip compressed data, was "dside-2.0.3.tar", last modified: Mon Jul 24 14:26:25 2023, max compression
```

## Comparing `dside-2.0.2.tar` & `dside-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.605594 dside-2.0.2/
--rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     2653 2023-07-24 14:09:41.604599 dside-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2023-03-11 12:37:11.000000 dside-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 14:09:41.605594 dside-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-07-24 14:04:37.000000 dside-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.582662 dside-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.588640 dside-2.0.2/src/dside/
--rw-rw-rw-   0        0        0    62364 2023-07-24 13:59:31.000000 dside-2.0.2/src/dside/DSI.py
--rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.0.2/src/dside/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:09:41.603602 dside-2.0.2/src/dside.egg-info/
--rw-rw-rw-   0        0        0     2653 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 14:09:41.000000 dside-2.0.2/src/dside.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 14:26:25.429600 dside-2.0.3/
+-rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2653 2023-07-24 14:26:25.428605 dside-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2023-03-11 12:37:11.000000 dside-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:26:25.429600 dside-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-07-24 14:25:30.000000 dside-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:26:25.396688 dside-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 14:26:25.406661 dside-2.0.3/src/dside/
+-rw-rw-rw-   0        0        0    62438 2023-07-24 14:24:59.000000 dside-2.0.3/src/dside/DSI.py
+-rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.0.3/src/dside/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:26:25.427605 dside-2.0.3/src/dside.egg-info/
+-rw-rw-rw-   0        0        0     2653 2023-07-24 14:26:25.000000 dside-2.0.3/src/dside.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-24 14:26:25.000000 dside-2.0.3/src/dside.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:26:25.000000 dside-2.0.3/src/dside.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-24 14:26:25.000000 dside-2.0.3/src/dside.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 14:26:25.000000 dside-2.0.3/src/dside.egg-info/top_level.txt
```

### Comparing `dside-2.0.2/LICENSE` & `dside-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dside-2.0.2/PKG-INFO` & `dside-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.0.2
+Version: 2.0.3
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dside-2.0.2/README.md` & `dside-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dside-2.0.2/setup.py` & `dside-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 short_description = 'Design space identification tool for plotting and analysing design'+\
     ' spaces (2D and 3D).'
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name = 'dside',
```

### Comparing `dside-2.0.2/src/dside/DSI.py` & `dside-2.0.3/src/dside/DSI.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,18 @@
             self.opt.update(self.bw_template)
         self.opt.update(opt)
         
         # ---------------------------- External definitions ---------------------------- #
         sat = self.sat
         vio = self.vio
         opt = self.opt
-        labelpad = opt['labelpad']
+        try:
+            labelpad = opt['labelpad']
+        except KeyError:
+            labelpad = [8]*3
         if type(labelpad) == int:
             labelpad = [labelpad]
         if len(labelpad) == 1:
             labelpad *= 3
         plt.rcParams.update({'font.size': opt['font_size']})
         
         # ----------------------------- Heat map Variable ----------------------------- #
@@ -473,15 +476,15 @@
                     vmax[2] + limfactor*vrange[2]])
         
         
         # Labels
         plt.xlabel(opt['xlabel'], labelpad = labelpad[0])
         plt.ylabel(opt['ylabel'], labelpad = labelpad[1])
         if dim == 3:
-            ax.set_zlabel(opt['zlabel'], labelpad = labelpad[3])
+            ax.set_zlabel(opt['zlabel'], labelpad = labelpad[2])
             ax.view_init(elev = opt['elev'], azim = opt['azim'])
         if (opt['hmv'] == 'None') or (opt['hidehmv'] == True):
             plt.legend(loc = opt['legloc'],\
                 framealpha = opt['framealpha']).set_zorder(opt['legendzorder'])
         
         # Saving
         plt.tight_layout()
```

### Comparing `dside-2.0.2/src/dside.egg-info/PKG-INFO` & `dside-2.0.3/src/dside.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.0.2
+Version: 2.0.3
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

