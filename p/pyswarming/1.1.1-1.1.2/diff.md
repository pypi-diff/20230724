# Comparing `tmp/pyswarming-1.1.1.tar.gz` & `tmp/pyswarming-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/macbookpro/Documents/GitHub/pyswarming/dist/.tmp-cg596bkg/pyswarming-1.1.1.tar", last modified: Fri Jul 21 18:15:11 2023, max compression
+gzip compressed data, was "/Users/macbookpro/Documents/GitHub/pyswarming/dist/.tmp-fqy6wnqa/pyswarming-1.1.2.tar", last modified: Mon Jul 24 11:52:09 2023, max compression
```

## Comparing `pyswarming-1.1.1.tar` & `pyswarming-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)     1529 2023-04-24 23:27:31.000000 pyswarming-1.1.1/LICENSE.md
--rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-21 18:15:11.000000 pyswarming-1.1.1/PKG-INFO
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    12824 2023-07-21 18:04:39.000000 pyswarming-1.1.1/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)      899 2023-07-21 17:48:11.000000 pyswarming-1.1.1/pyswarming/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)    14252 2023-03-29 00:19:04.000000 pyswarming-1.1.1/pyswarming/auto_differentiation.py
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    25881 2023-07-20 18:25:06.000000 pyswarming-1.1.1/pyswarming/behaviors.py
--rw-r--r--   0 macbookpro   (501) staff       (20)    12629 2023-07-21 14:37:10.000000 pyswarming-1.1.1/pyswarming/swarm.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)      372 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      106 2023-07-21 18:15:11.000000 pyswarming-1.1.1/setup.cfg
--rwxr-xr-x   0 macbookpro   (501) staff       (20)     1146 2023-07-21 17:48:02.000000 pyswarming-1.1.1/setup.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/tests/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-29 00:19:04.000000 pyswarming-1.1.1/tests/__init__.py
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    28166 2023-07-20 18:54:34.000000 pyswarming-1.1.1/tests/test_behaviors.py
--rwxr-xr-x   0 macbookpro   (501) staff       (20)     1391 2023-07-20 20:23:44.000000 pyswarming-1.1.1/tests/test_swarm.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-24 11:52:09.000000 pyswarming-1.1.2/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1529 2023-04-24 23:27:31.000000 pyswarming-1.1.2/LICENSE.md
+-rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-24 11:52:09.000000 pyswarming-1.1.2/PKG-INFO
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    12824 2023-07-24 11:51:05.000000 pyswarming-1.1.2/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)      994 2023-07-24 11:51:11.000000 pyswarming-1.1.2/pyswarming/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    14252 2023-03-29 00:19:04.000000 pyswarming-1.1.2/pyswarming/auto_differentiation.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    25881 2023-07-20 18:25:06.000000 pyswarming-1.1.2/pyswarming/behaviors.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    11003 2023-07-24 01:50:32.000000 pyswarming-1.1.2/pyswarming/swarm.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)      372 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-24 11:52:09.000000 pyswarming-1.1.2/pyswarming.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      106 2023-07-24 11:52:09.000000 pyswarming-1.1.2/setup.cfg
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1146 2023-07-24 11:51:09.000000 pyswarming-1.1.2/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-24 11:52:09.000000 pyswarming-1.1.2/tests/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-29 00:19:04.000000 pyswarming-1.1.2/tests/__init__.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    28166 2023-07-20 18:54:34.000000 pyswarming-1.1.2/tests/test_behaviors.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1793 2023-07-24 01:15:03.000000 pyswarming-1.1.2/tests/test_swarm.py
```

### Comparing `pyswarming-1.1.1/LICENSE.md` & `pyswarming-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.1/PKG-INFO` & `pyswarming-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswarming
-Version: 1.1.1
+Version: 1.1.2
 Summary: A research toolkit for Swarm Robotics
 Home-page: https://github.com/mrsonandrade/pyswarming
 Author: Emerson Martins de Andrade
 Author-email: mrson@oceanica.ufrj.br
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.1-blue)
+![version](https://img.shields.io/badge/version-1.1.2-blue)
 [![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
```

### Comparing `pyswarming-1.1.1/README.md` & `pyswarming-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.1-blue)
+![version](https://img.shields.io/badge/version-1.1.2-blue)
 [![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
```

### Comparing `pyswarming-1.1.1/pyswarming/auto_differentiation.py` & `pyswarming-1.1.2/pyswarming/auto_differentiation.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.1/pyswarming/behaviors.py` & `pyswarming-1.1.2/pyswarming/behaviors.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.1/pyswarming/swarm.py` & `pyswarming-1.1.2/pyswarming/swarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,43 +69,14 @@
         - 'gaussian' : the creation is based in an gaussian distribution.
 
     plot_limits : list
         list containing the plot limits (matplotlib).
 
     behaviors : list
         list containing the behaviors to be simulated.
-
-    Example 1
-    --------
-    >>> import pyswarming.swarm as ps
-    >>> my_swarm = ps.Swarm(n = 10, # number of robots
-                            linear_speed = 0.5, # linear speed of each robot
-                            dT = 1.0, # sampling time
-                            deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
-                            deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
-                            distribution_type =  'uniform', # type of distribution used to deploy the robots
-                            plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                            behaviors = ['collective_navigation']) # list of behaviors
-    >>> my_swarm.behaviors_dict['r_out']['collective_navigation']['alpha'] = 2.0  # setting the strength of the repulsion
-    >>> my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = [-40, -40, 0] # setting the target position [x, y, z]
-    >>> my_swarm.simulate()
-
-    Example 2
-    --------
-    >>> import pyswarming.swarm as ps
-    >>> my_swarm = ps.Swarm(n = 10, # number of robots
-                            linear_speed = 0.5, # linear speed of each robot
-                            dT = 1.0, # sampling time
-                            deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
-                            deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
-                            distribution_type =  'uniform', # type of distribution used to deploy the robots
-                            plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                            behaviors = ['target','aggregation']) # list of behaviors
-    >>> my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target position [x, y, z]
-    >>> my_swarm.simulate()
     """
 
     def __init__(self, n,
                  linear_speed = 0.5,
                  dT = 1.0,
                  deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]],
                  deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*np.pi]],
@@ -240,16 +211,30 @@
 
         self.pose = np.concatenate((r, theta), axis=1)
 
     def simulate(self,
                  frames = 720,
                  interval = 1,
                  blit = False,
-                 repeat = False):
+                 repeat = False,
+                 mode = 'pltshow'):
 
         # First set up the figure and the axis
         if self.dimensions == 2:
             self.fig, self.ax = plt.subplots()
 
-        anim = animation.FuncAnimation(self.fig, self._animate, frames=frames, interval=interval, blit=blit, repeat=repeat)
+        if mode == 'pltshow':
+            anim = animation.FuncAnimation(self.fig, self._animate, frames=frames, interval=interval, blit=blit, repeat=repeat)
+            plt.show()
+
+        elif mode == 'anim':
+            import warnings
+            warnings.filterwarnings("ignore")
+            anim = animation.FuncAnimation(self.fig, self._animate, frames=frames, interval=interval, blit=blit, repeat=repeat)
+            return anim
+        
+        elif mode == 'simulate':
+            for time_i in range(frames):
+                self._animate(time_i)
+            return self.pose
 
-        plt.show()
+
```

### Comparing `pyswarming-1.1.1/pyswarming.egg-info/PKG-INFO` & `pyswarming-1.1.2/pyswarming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswarming
-Version: 1.1.1
+Version: 1.1.2
 Summary: A research toolkit for Swarm Robotics
 Home-page: https://github.com/mrsonandrade/pyswarming
 Author: Emerson Martins de Andrade
 Author-email: mrson@oceanica.ufrj.br
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.1-blue)
+![version](https://img.shields.io/badge/version-1.1.2-blue)
 [![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
```

### Comparing `pyswarming-1.1.1/setup.py` & `pyswarming-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 INSTALL_REQUIRES = [
     "numpy",
     "matplotlib",
 ]
 
 setuptools.setup(
     name="pyswarming",
-    version="1.1.1",
+    version="1.1.2",
     author="Emerson Martins de Andrade",
     author_email="mrson@oceanica.ufrj.br",
     description="A research toolkit for Swarm Robotics",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mrsonandrade/pyswarming",
     packages=setuptools.find_packages(),
```

### Comparing `pyswarming-1.1.1/tests/test_behaviors.py` & `pyswarming-1.1.2/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.1/tests/test_swarm.py` & `pyswarming-1.1.2/tests/test_swarm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import pyswarming.swarm as ps
 
 import numpy as np
 
 def test_swarm():
-    #@pytest.fixture(scope='function')
-    my_swarm = ps.Swarm(n = 10, # number of robots
+    my_swarm = ps.Swarm(n = 3, # number of robots
                         linear_speed = 0.5, # linear speed of each robot
                         dT = 1.0, # sampling time
-                        deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                        deployment_point_limits = [[0.0, 0.0, 0.0], [0.1, 0.1, 0.1]], # lower and upper limits for the position deployment
                         deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
                         distribution_type =  'uniform', # type of distribution used to deploy the robots
                         plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
                         behaviors = ['target','aggregation']) # list of behaviors
     my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target position [x, y, z]
     
     assert type(my_swarm.pose) == np.ndarray # type
-    assert my_swarm.pose.shape == (10, 6) # shape
+    assert my_swarm.pose.shape == (3, 6) # shape
     assert (my_swarm.pose[:,:3] >= 0.0).all() # coordinates
-    assert (my_swarm.pose[:,:3] <= 5.0).all() # coordinates
+    assert (my_swarm.pose[:,:3] <= 0.1).all() # coordinates
     assert (my_swarm.pose[:,3:] >= 0.0).all() # orientations
     assert (my_swarm.pose[:,3:] <= 2*3.1415).all() # orientations
     assert my_swarm.behaviors == ['target','aggregation'] # behaviors
+    pose_expected = np.array([[-40.28693728, -39.83492534,   0.        ,   0.        , 0.        ,  -2.36183599],
+                               [-40.07904417, -39.7754317 ,   0.        ,   0.        , 0.        ,  -2.35999654],
+                               [-39.87972043, -39.69159204,   0.        ,   0.        , 0.        ,  -2.35855876]])
+    assert np.isclose(my_swarm.simulate(mode='simulate'), pose_expected, atol=1e-0).all() == True
```

