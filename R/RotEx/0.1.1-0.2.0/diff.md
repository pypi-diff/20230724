# Comparing `tmp/RotEx-0.1.1.tar.gz` & `tmp/RotEx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RotEx-0.1.1.tar", last modified: Wed Jul  5 08:46:58 2023, max compression
+gzip compressed data, was "RotEx-0.2.0.tar", last modified: Mon Jul 24 10:47:23 2023, max compression
```

## Comparing `RotEx-0.1.1.tar` & `RotEx-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:58.703032 RotEx-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 08:46:42.000000 RotEx-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-05 08:46:58.703032 RotEx-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-05 08:46:42.000000 RotEx-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:58.703032 RotEx-0.1.1/RotEx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.000000 RotEx-0.1.1/RotEx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-05 08:46:42.000000 RotEx-0.1.1/RotEx/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-05 08:46:42.000000 RotEx-0.1.1/RotEx/rotate_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-07-05 08:46:42.000000 RotEx-0.1.1/RotEx/rotex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-05 08:46:42.000000 RotEx-0.1.1/RotEx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:58.703032 RotEx-0.1.1/RotEx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-05 08:46:58.000000 RotEx-0.1.1/RotEx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 08:46:58.000000 RotEx-0.1.1/RotEx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:46:58.000000 RotEx-0.1.1/RotEx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 08:46:58.000000 RotEx-0.1.1/RotEx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 08:46:58.000000 RotEx-0.1.1/RotEx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 08:46:58.703032 RotEx-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 08:46:42.000000 RotEx-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:58.703032 RotEx-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-05 08:46:42.000000 RotEx-0.1.1/tests/test_attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-05 08:46:42.000000 RotEx-0.1.1/tests/test_rotate_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-05 08:46:42.000000 RotEx-0.1.1/tests/test_rotex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:47:23.488562 RotEx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 10:47:07.000000 RotEx-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-24 10:47:23.488562 RotEx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 10:47:07.000000 RotEx-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:47:23.488562 RotEx-0.2.0/RotEx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:47:07.000000 RotEx-0.2.0/RotEx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-24 10:47:07.000000 RotEx-0.2.0/RotEx/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 10:47:07.000000 RotEx-0.2.0/RotEx/rotate_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-24 10:47:07.000000 RotEx-0.2.0/RotEx/rotex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-24 10:47:07.000000 RotEx-0.2.0/RotEx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:47:23.488562 RotEx-0.2.0/RotEx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-24 10:47:23.000000 RotEx-0.2.0/RotEx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 10:47:23.000000 RotEx-0.2.0/RotEx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:47:23.000000 RotEx-0.2.0/RotEx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 10:47:23.000000 RotEx-0.2.0/RotEx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 10:47:23.000000 RotEx-0.2.0/RotEx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:47:23.488562 RotEx-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 10:47:07.000000 RotEx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:47:23.488562 RotEx-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-07-24 10:47:07.000000 RotEx-0.2.0/tests/test_attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-24 10:47:07.000000 RotEx-0.2.0/tests/test_rotate_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-24 10:47:07.000000 RotEx-0.2.0/tests/test_rotex.py
```

### Comparing `RotEx-0.1.1/LICENSE` & `RotEx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RotEx-0.1.1/PKG-INFO` & `RotEx-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RotEx
-Version: 0.1.1
+Version: 0.2.0
 Summary: RotEx is a set of python helper functions to apply 3D rotation, especially Euler Angles, based on scipy.spatial.transform.Rotation
 Home-page: https://github.com/dinglezhang/RotEx
 Author: dingle
 Author-email: zhangdingh_2004@hotmail.com
 Keywords: euler-angles,attitude,rotation,3d-rotation,rotation-extension,rotation-help
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `RotEx-0.1.1/README.md` & `RotEx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `RotEx-0.1.1/RotEx/attitude.py` & `RotEx-0.2.0/RotEx/attitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from scipy.spatial.transform import Rotation
 
 from . import utils
 from . import rotex
 
 logger = utils.get_logger()
```

### Comparing `RotEx-0.1.1/RotEx/rotate_vectors.py` & `RotEx-0.2.0/RotEx/rotate_vectors.py`

 * *Files identical despite different names*

### Comparing `RotEx-0.1.1/RotEx/rotex.py` & `RotEx-0.2.0/RotEx/rotex.py`

 * *Files 26% similar despite different names*

```diff
@@ -240,32 +240,128 @@
   logger.info('rotvec in new frame: %s' % rotvec_in_new_frame)
 
   rot_in_new_frame = Rotation.from_rotvec(rotvec_in_new_frame)
 
   return rot_in_new_frame
 
 '''
+Calculate rotation angular displacement.
+
+Args:
+  rot: the rotation
+  is_degree: True is degree and False is radian for output augular velocity
+Return:
+  [0]: rotation angular vector
+  [1]: rotation angular scalar
+'''
+def calc_angular_displacement(rot, is_degree):
+  rotvec = rot.as_rotvec()
+  logger.info('rotvec: %s' % rotvec)
+
+  angular_vector = rotvec
+  angular_scalar = np.linalg.norm(angular_vector)
+  logger.info('rotation angular vector(rad): %s' % angular_vector)
+  logger.info('rotation angular scalar(rad): %s' % angular_scalar)
+  if is_degree:
+    angular_vector = np.rad2deg(angular_vector)
+    angular_scalar = np.rad2deg(angular_scalar)
+    logger.info('rotation angular vector(deg): %s' % angular_vector)
+    logger.info('rotation angular scalar(deg): %s' % angular_scalar)
+
+  return angular_vector, angular_scalar
+
+'''
 Calculate angular velocity by rotation and delta time.
 
 Args:
   rot: the rotation
   delta_time: time cost for the rotation
   is_degree: True is degree and False is radian for output augular velocity
 Return:
   [0]: angular velocity, which is a vecotr
   [1]: angular rate, which is a scalar
 '''
 def calc_angular_velocity(rot, delta_time, is_degree):
-  rotvec = rot.as_rotvec()
-  logger.info('rotvec: %s' % rotvec)
+  (angular_vector, angular_scalar) = calc_angular_displacement(rot, is_degree)
 
-  angular_velocity = rotvec / delta_time
-  angular_rate = np.linalg.norm(angular_velocity)
-  logger.info('angular velocity(rad): %s' % angular_velocity)
-  logger.info('angular rate(rad): %s' % angular_rate)
-  if is_degree:
-    angular_velocity = np.rad2deg(angular_velocity)
-    angular_rate = np.rad2deg(angular_rate)
-    logger.info('angular velocity(deg): %s' % angular_velocity)
-    logger.info('angular rate(deg): %s' % angular_rate)
+  angular_velocity = angular_vector / delta_time
+  angular_rate = angular_scalar / delta_time
+  angular_unit = utils.get_angular_unit(is_degree)
+  logger.info('angular velocity(%s): %s' % (angular_unit, angular_velocity))
+  logger.info('angular rate(%s): %s' % (angular_unit, angular_rate))
 
   return angular_velocity, angular_rate
+
+'''
+Calculate angular acceleration by two angular velocities and delta time.
+[ToDo] So far it is just to get difference between two angular velocities and divide by delta time, temporarily.
+       Need to find a good way to decribe rot with changing angular velocity, then to calculate the angular acceleration.
+
+Args:
+  angular_velocity_1, angular_velocity_2: two angular velocities from 1 to 2
+  delta_time: time cost for the change of angular_velocity
+Return:
+  [0]: angular acceleration vector
+  [1]: angular acceleration scalar
+  whether accelerationis degree or not dependends on the input
+'''
+def calc_angular_acceleration(angular_velocity_1, angular_velocity_2, delta_time):
+  angular_acceleration_vector = (angular_velocity_2 - angular_velocity_1) / delta_time
+  angular_acceleration_scalar = np.linalg.norm(angular_acceleration_vector)
+
+  return angular_acceleration_vector, angular_acceleration_scalar
+
+'''
+Calculate linear displacement for vectors by rotation.
+
+Args:
+  rot: the rotation
+  vectors: vectors to be rotated
+Return:
+  [0]: linear displacement vectors
+  [1]: linear displacement scalars
+'''
+def calc_linear_displacement(rot, vectors):
+  angular_vector = calc_angular_displacement(rot, False)[0]
+
+  linear_displacement_vectors = np.cross(angular_vector, vectors)
+  linear_displacement_scalars = np.linalg.norm(linear_displacement_vectors, axis = 1)
+
+  return linear_displacement_vectors, linear_displacement_scalars
+
+'''
+Calculate linear velocity for vectors by rotation and delta time.
+
+Args:
+  rot: the rotation
+  vectors: vectors to be rotated
+  delta_time: time cost for the rotation
+Return:
+  [0]: linear velocities, which are vectors
+  [1]: linear rates, which are scalars
+'''
+def calc_linear_velocity(rot, vectors, delta_time):
+  angular_velocity = calc_angular_velocity(rot, delta_time, False)[0]
+
+  linear_velocities = np.cross(angular_velocity, vectors)
+  linear_rates = np.linalg.norm(linear_velocities, axis = 1)
+
+  return linear_velocities, linear_rates
+
+'''
+Calculate centripetal acceleration for vectors by rotation and delta time.
+
+Args:
+  rot: the rotation
+  vectors: vectors to be rotated
+  delta_time: time cost for the rotation
+Return:
+  [0]: centripetal acceleration vectors
+  [1]: centripetal acceleration scalars
+'''
+def calc_centripetal_acceleration(rot, vectors, delta_time):
+  angular_velocity = calc_angular_velocity(rot, delta_time, False)[0]
+
+  centripetal_acceleration_vectors = np.cross(angular_velocity, np.cross(angular_velocity, vectors))
+  centripetal_acceleration_scalars = np.linalg.norm(centripetal_acceleration_vectors, axis = 1)
+
+  return centripetal_acceleration_vectors, centripetal_acceleration_scalars
```

### Comparing `RotEx-0.1.1/RotEx/utils.py` & `RotEx-0.2.0/RotEx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ROTATION_SEQUENCES_EXTRINSIC = [element.lower() for element in ROTATION_SEQUENCES_INTRINSIC]
 
 logger = logging.getLogger()
 logger.setLevel('INFO')
 #logger.setLevel('WARNING')
 
 handler = logging.StreamHandler()
-fmtr = logging.Formatter(fmt="[%(asctime)s][%(filename)s:%(lineno)d][%(funcName)s()][%(levelname)s]: %(message)s")
+fmtr = logging.Formatter(fmt = "[%(asctime)s][%(filename)s:%(lineno)d][%(funcName)s()][%(levelname)s]: %(message)s")
 handler.setFormatter(fmtr)
 logger.addHandler(handler)
 
 def get_logger():
   return logger
 
 def get_angular_unit(is_degree):
```

### Comparing `RotEx-0.1.1/RotEx.egg-info/PKG-INFO` & `RotEx-0.2.0/RotEx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RotEx
-Version: 0.1.1
+Version: 0.2.0
 Summary: RotEx is a set of python helper functions to apply 3D rotation, especially Euler Angles, based on scipy.spatial.transform.Rotation
 Home-page: https://github.com/dinglezhang/RotEx
 Author: dingle
 Author-email: zhangdingh_2004@hotmail.com
 Keywords: euler-angles,attitude,rotation,3d-rotation,rotation-extension,rotation-help
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `RotEx-0.1.1/setup.py` & `RotEx-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from codecs import open
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
-    name="RotEx",
-    version="0.1.1",
-    author="dingle",
-    author_email="zhangdingh_2004@hotmail.com",
-    description="RotEx is a set of python helper functions to apply 3D rotation, especially Euler Angles, based on scipy.spatial.transform.Rotation",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/dinglezhang/RotEx",
+    name = "RotEx",
+    version = "0.2.0",
+    author = "dingle",
+    author_email = "zhangdingh_2004@hotmail.com",
+    description = "RotEx is a set of python helper functions to apply 3D rotation, especially Euler Angles, based on scipy.spatial.transform.Rotation",
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
+    url = "https://github.com/dinglezhang/RotEx",
 
-    include_package_data=True,
-    install_requires=['scipy'],
-    extras_require={"dev": ['pytest']},
-    packages=find_packages(exclude=["tests*"]),
+    include_package_data = True,
+    install_requires = ['scipy'],
+    extras_require = {"dev": ['pytest']},
+    packages = find_packages(exclude = ["tests*"]),
 
-    keywords=["euler-angles", "attitude", "rotation", "3d-rotation", "rotation-extension", "rotation-help"],
-    classifiers=[
+    keywords = ["euler-angles", "attitude", "rotation", "3d-rotation", "rotation-extension", "rotation-help"],
+    classifiers = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License"
     ]
 )
```

### Comparing `RotEx-0.1.1/tests/test_attitude.py` & `RotEx-0.2.0/tests/test_attitude.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,37 +6,52 @@
 
 from RotEx import utils
 from RotEx import rotex
 from RotEx import attitude
 
 from . import test_rotate_vectors
 
-@pytest.mark.parametrize('rfu_d_in_enu_frame, expected_rfu_d_in_enu_frame',
-                        [(np.array([-45, 0, 0]), np.array([45, 0, 0])),
-                         (np.array([0, 45, 0]), np.array([0, 45, 0])),
-                         (np.array([0, 0, 45]), np.array([0, 0, 45])),
-                         (np.array([-90, 45, 90]), np.array([90, 45, 90]))])
-def test_change_frame_enu_2_ned(rfu_d_in_enu_frame, expected_rfu_d_in_enu_frame):
+att_in_frame_1 = \
+  [np.array([-45, 0, 0]),
+   np.array([0, 45, 0]),
+   np.array([0, 0, 45]),
+   np.array([-90, 45, 90])]
+
+att_in_frame_2 = \
+  [np.array([45, 0, 0]),
+   np.array([0, 45, 0]),
+   np.array([0, 0, 45]),
+   np.array([90, 45, 90])]
+
+heading_samples = \
+  [np.array([-1, 1, math.sqrt(2)]),
+   np.array([-1, 2, 3]),
+   np.array([-1, 2, 0.5])]
+
+slope_angle_samples = [0, 15, 45, -30]
+
+att_d_smaples = \
+  [np.array([10, -1, 4]),
+   np.array([11, -2, 5]),
+   np.array([12, -3, 6])]
+
+rot_seq_samples = ['ZYX', 'zyx']
+
+@pytest.mark.parametrize('rfu_d_in_enu_frame, rfu_d_in_enu_frame_expected', [(a, b) for a, b in zip(att_in_frame_1, att_in_frame_2)])
+def test_change_frame_enu_2_ned(rfu_d_in_enu_frame, rfu_d_in_enu_frame_expected):
   (rot_in_ned_frame, frd_d_in_ned_frame) = attitude.change_frame_enu_2_ned(rfu_d_in_enu_frame, True)
-  assert_allclose(frd_d_in_ned_frame, expected_rfu_d_in_enu_frame, atol=1e-8)
+  assert_allclose(frd_d_in_ned_frame, rfu_d_in_enu_frame_expected, atol = 1e-8)
 
-@pytest.mark.parametrize('frd_d_in_ned_frame, expected_frd_d_in_ned_frame',
-                        [(np.array([45, 0, 0]), np.array([-45, 0, 0])),
-                         (np.array([0, 45, 0]), np.array([0, 45, 0])),
-                         (np.array([0, 0, 45]), np.array([0, 0, 45])),
-                         (np.array([90, 45, 90]), np.array([-90, 45, 90]))])
-def test_change_frame_ned_2_enu(frd_d_in_ned_frame, expected_frd_d_in_ned_frame):
+@pytest.mark.parametrize('frd_d_in_ned_frame, frd_d_in_ned_frame_expected', [(a, b) for a, b in zip(att_in_frame_2, att_in_frame_1)])
+def test_change_frame_ned_2_enu(frd_d_in_ned_frame, frd_d_in_ned_frame_expected):
   (rot_in_enu_frame, rfu_d_in_enu_frame) = attitude.change_frame_ned_2_enu(frd_d_in_ned_frame, True)
-  assert_allclose(rfu_d_in_enu_frame, expected_frd_d_in_ned_frame)
+  assert_allclose(rfu_d_in_enu_frame, frd_d_in_ned_frame_expected, atol = 1e-8)
 
-@pytest.mark.parametrize('heading_as_rfu',
-                        [np.array([-1, 1, math.sqrt(2)]),
-                         np.array([-1, 2, 3]),
-                         np.array([-1, 2, 0.5])])
-@pytest.mark.parametrize('right_slope_angle_d', [0, 15, 45, -30])
+@pytest.mark.parametrize('heading_as_rfu', heading_samples)
+@pytest.mark.parametrize('right_slope_angle_d', slope_angle_samples)
 def test_from_heading_in_enu_frame(heading_as_rfu, right_slope_angle_d):
   is_possible = rotex._analyze_vector_and_angle_against_xy_plane(heading_as_rfu, np.deg2rad(right_slope_angle_d))[0]
 
   if not is_possible:
     with pytest.raises(ValueError,  match='It is impossible to rotate to the vector'):
       attitude.from_heading_in_enu_frame(heading_as_rfu, right_slope_angle_d, True)
   else:
@@ -49,21 +64,18 @@
                                                  heading_end_expected, False)
 
     # test on right slope angle by right direction
     right_start = np.array([1, 0, 0])
     right_end = rot.apply(right_start)
     right_slope_angle_result = utils.calc_angle_between_vector_and_xy_plane(right_end, True)
 
-    assert_allclose(right_slope_angle_result, right_slope_angle_d, atol=1e-8)
+    assert_allclose(right_slope_angle_result, right_slope_angle_d, atol = 1e-8)
 
-@pytest.mark.parametrize('heading_as_frd',
-                        [np.array([-1, 1, math.sqrt(2)]),
-                         np.array([-1, 2, 3]),
-                         np.array([-1, 2, 0.5])])
-@pytest.mark.parametrize('right_slope_angle_d', [0, 15, 45, -30])
+@pytest.mark.parametrize('heading_as_frd', heading_samples)
+@pytest.mark.parametrize('right_slope_angle_d', slope_angle_samples)
 def test_from_heading_in_ned_frame(heading_as_frd, right_slope_angle_d):
   is_possible = rotex._analyze_vector_and_angle_against_xy_plane(heading_as_frd, np.deg2rad(right_slope_angle_d))[0]
 
   if not is_possible:
     with pytest.raises(ValueError,  match='It is impossible to rotate to the vector'):
       attitude.from_heading_in_ned_frame(heading_as_frd, right_slope_angle_d, True)
   else:
@@ -76,19 +88,19 @@
                                                  heading_end_expected, False)
 
     # test on right slope angle by right direction
     right_start = np.array([0, 1, 0])
     right_end = rot.apply(right_start)
     right_slope_angle_result = -utils.calc_angle_between_vector_and_xy_plane(right_end, True)
 
-    assert_allclose(right_slope_angle_result, right_slope_angle_d, atol=1e-8)
+    assert_allclose(right_slope_angle_result, right_slope_angle_d, atol = 1e-8)
 
-@pytest.mark.parametrize('att_d_1', [np.array([10, 1, 4])])
-@pytest.mark.parametrize('att_d_2', [np.array([11, 2, 5])])
-@pytest.mark.parametrize('rot_seq', ['ZYX', 'zyx'])
+@pytest.mark.parametrize('att_d_1', att_d_smaples)
+@pytest.mark.parametrize('att_d_2', att_d_smaples)
+@pytest.mark.parametrize('rot_seq', rot_seq_samples)
 @pytest.mark.parametrize('in_world_frame', [True, False])
 def test_get_delta_att(att_d_1, att_d_2, rot_seq, in_world_frame, vector_samples):
   rot1 = Rotation.from_euler(rot_seq, att_d_1, True)
   rot2 = Rotation.from_euler(rot_seq, att_d_2, True)
 
   if in_world_frame:
     vectors_by_rot1 = rot1.apply(vector_samples)
@@ -97,19 +109,19 @@
     vectors_by_rot1 = vector_samples # they are original coordinates in rot1 frame
     vectors_by_rot2 = rot2.apply(vector_samples)
     vectors_by_rot2 = rot1.inv().apply(vectors_by_rot2)
 
   (delta_rot, delta_euler_d) = attitude.get_delta_att(att_d_1, att_d_2, rot_seq, True, in_world_frame)
   vectors_by_delta_rot = delta_rot.apply(vectors_by_rot1)
 
-  assert_allclose(vectors_by_rot2, vectors_by_delta_rot)
+  assert_allclose(vectors_by_rot2, vectors_by_delta_rot, atol = 1e-8)
 
-@pytest.mark.parametrize('att_d_1', [np.array([10, 1, 4]), np.array([11, 2, 5])])
+@pytest.mark.parametrize('att_d_1', att_d_smaples)
 @pytest.mark.parametrize('factor', [1.1, 1.2])
-@pytest.mark.parametrize('rot_seq', ['ZYX', 'zyx'])
+@pytest.mark.parametrize('rot_seq', rot_seq_samples)
 def test_linear_delta_att(att_d_1, factor, rot_seq):
   # calculate att_d_2 from att_d_1 and factor (linear change on rotvec)
   rot1 = Rotation.from_euler(rot_seq, att_d_1, True)
   rotvec1 = rot1.as_rotvec()
   rotvec2 = rotvec1 * factor
   rot2 = Rotation.from_rotvec(rotvec2)
   att_d_2 = rot2.as_euler(rot_seq, True)
@@ -120,23 +132,31 @@
   # calcaulate delta_att_linear by a special way for linear rotvec change
   delta_rotvec_linear = rotvec2 - rotvec1
   delta_rot_linear = Rotation.from_rotvec(delta_rotvec_linear)
   delta_euler_d_linear = delta_rot_linear.as_euler(rot_seq, True)
 
   assert_allclose(delta_euler_d, delta_euler_d_linear)
 
-@pytest.mark.parametrize('att_d_1', [np.array([10, 1, 4])])
-@pytest.mark.parametrize('att_d_2', [np.array([11, 2, 5])])
-@pytest.mark.parametrize('rot_seq', ['ZYX', 'zyx'])
+@pytest.mark.parametrize('att_d_0', att_d_smaples)
+@pytest.mark.parametrize('att_d_1', att_d_smaples)
+@pytest.mark.parametrize('att_d_2', att_d_smaples)
+@pytest.mark.parametrize('rot_seq', rot_seq_samples)
 @pytest.mark.parametrize('delta_time', [2, 3])
-def test_calc_angular_velocity(att_d_1, att_d_2, rot_seq, delta_time):
-  angular_velocity = attitude.calc_angular_velocity(att_d_1, att_d_2, rot_seq, True, delta_time, False)[0]
+def test_calc_angular_velocity_acceleration(att_d_0, att_d_1, att_d_2, rot_seq, delta_time):
+  angular_velocity_1 = attitude.calc_angular_velocity(att_d_0, att_d_1, rot_seq, True, delta_time, False)[0]
+  angular_velocity_2 = attitude.calc_angular_velocity(att_d_1, att_d_2, rot_seq, True, delta_time, False)[0]
+  angular_acceleration = rotex.calc_angular_acceleration(angular_velocity_2, angular_velocity_1, delta_time)[0]
 
-  times = [0, delta_time]
-  angles = [att_d_1, att_d_2]
+  times = [0, delta_time, delta_time * 2]
+  angles = [att_d_0, att_d_1, att_d_2]
   rotations = Rotation.from_euler(rot_seq, angles, True)
-
   spline = RotationSpline(times, rotations)
-  angular_velocity_spline = spline(times, 1)[1]
+
+  times = [0, delta_time * 2]
+  angular_velocity_spline = spline(times, 1)
   angular_velocity_spline = np.rad2deg(angular_velocity_spline)
+  angular_acceleration_spline = spline(times, 2)
+  angular_acceleration_spline = np.rad2deg(angular_acceleration_spline)
 
-  assert_allclose(angular_velocity, angular_velocity_spline)
+  assert_allclose(angular_velocity_1, angular_velocity_spline[0], atol = 1e-8)
+  assert_allclose(angular_velocity_2, angular_velocity_spline[1], atol = 1e-8)
+  assert_allclose(angular_acceleration, (angular_acceleration_spline[0] + angular_acceleration_spline[1])/2, atol = 1e-6)
```

### Comparing `RotEx-0.1.1/tests/test_rotate_vectors.py` & `RotEx-0.2.0/tests/test_rotate_vectors.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,34 +39,27 @@
                                   [0, 0, 1],
                                   [0, 1, 0],
                                   [-1, 0, 0],
                                   [-1, 1, 1]
                                 ]), True)])
 def test_rotate_vectors_once(vectors, euler_d, rot_seq, vectors_rotated_expected, on_frame):
   vectors_rotated = rotate_vectors.rotate_vectors_by_euler(vectors, euler_d, rot_seq, True, 1, on_frame)
-  assert_allclose(vectors_rotated, vectors_rotated_expected, atol=1e-8)
+  assert_allclose(vectors_rotated, vectors_rotated_expected, atol = 1e-8)
 
-@pytest.mark.parametrize('vectors',
-                        [np.array([
-                                  [1, 0, 0],
-                                  [0, 1, 0],
-                                  [0, 0, 1],
-                                  [1, 1, 1]
-                                ])])
 @pytest.mark.parametrize('euler_d', [np.array([3, 3, 3])])
 @pytest.mark.parametrize('rot_seq', ['ZYX', 'zyx'])
 @pytest.mark.parametrize('times', [3, 4, 5])
 @pytest.mark.parametrize('on_frame', [True, False])
-def test_rotate_vectors_multple_times(vectors, euler_d, rot_seq, times, on_frame):
-  vectors_rotated_one_by_one = vectors
+def test_rotate_vectors_multple_times(vector_samples, euler_d, rot_seq, times, on_frame):
+  vectors_rotated_one_by_one = vector_samples
   for i in range(1, times + 1):
     vectors_rotated_one_by_one = rotate_vectors.rotate_vectors_by_euler(vectors_rotated_one_by_one, euler_d, rot_seq, True, 1, on_frame)
 
-  vectors_rotated_composed = rotate_vectors.rotate_vectors_by_euler(vectors, euler_d, rot_seq, True, times, on_frame)
+  vectors_rotated_composed = rotate_vectors.rotate_vectors_by_euler(vector_samples, euler_d, rot_seq, True, times, on_frame)
 
   assert_allclose(vectors_rotated_one_by_one, vectors_rotated_composed)
 
   euler_d = euler_d * times
-  vectors_rotated_multiply_angles = rotate_vectors.rotate_vectors_by_euler(vectors, euler_d, rot_seq, True, 1, on_frame)
+  vectors_rotated_multiply_angles = rotate_vectors.rotate_vectors_by_euler(vector_samples, euler_d, rot_seq, True, 1, on_frame)
 
   # [ToDo] it maybe SAME if rotation on only one axis
   assert not np.allclose(vectors_rotated_one_by_one, vectors_rotated_multiply_angles)
```

