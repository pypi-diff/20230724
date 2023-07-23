# Comparing `tmp/dreifus-0.0.9.tar.gz` & `tmp/dreifus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-3h5abee6/dreifus-0.0.9.tar", last modified: Fri Jun 16 11:10:03 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-ewb7znmi/dreifus-0.1.1.tar", last modified: Thu Jul 20 13:46:11 2023, max compression
```

## Comparing `dreifus-0.0.9.tar` & `dreifus-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:03.166873 dreifus-0.0.9/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-16 11:10:03.152836 dreifus-0.0.9/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.9/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-16 11:09:14.000000 dreifus-0.0.9/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-16 11:10:03.168617 dreifus-0.0.9/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.9/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:01.839337 dreifus-0.0.9/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.185717 dreifus-0.0.9/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.9/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.9/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6338 2023-06-16 11:08:44.000000 dreifus-0.0.9/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1550 2023-06-06 21:52:50.000000 dreifus-0.0.9/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.676022 dreifus-0.0.9/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.0.9/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.9/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.9/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.9/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17626 2023-06-06 18:45:27.000000 dreifus-0.0.9/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.9/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.0.9/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.9/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      952 2023-06-06 21:55:22.000000 dreifus-0.0.9/src/dreifus/render.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.9/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.772160 dreifus-0.0.9/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.9/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.9/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.961296 dreifus-0.0.9/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.9/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.9/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.9/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.9/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.342316 dreifus-0.0.9/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      922 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:03.121955 dreifus-0.0.9/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.9/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.0.9/test/test_camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.9/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.9/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.9/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:11.000000 dreifus-0.1.1/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2517 2023-07-20 13:46:11.000000 dreifus-0.1.1/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2062 2023-07-20 13:45:18.000000 dreifus-0.1.1/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-07-20 13:45:31.000000 dreifus-0.1.1/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-07-20 13:46:11.000000 dreifus-0.1.1/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.1.1/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:10.000000 dreifus-0.1.1/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:10.000000 dreifus-0.1.1/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.1.1/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.1.1/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6338 2023-06-16 11:08:44.000000 dreifus-0.1.1/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1550 2023-06-06 21:52:50.000000 dreifus-0.1.1/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:11.000000 dreifus-0.1.1/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.1.1/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6062 2023-07-16 13:27:08.000000 dreifus-0.1.1/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.1.1/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.1.1/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17874 2023-07-16 09:56:02.000000 dreifus-0.1.1/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.1.1/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.1.1/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12113 2023-07-19 15:21:54.000000 dreifus-0.1.1/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3094 2023-07-19 10:37:58.000000 dreifus-0.1.1/src/dreifus/render.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.1.1/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:11.000000 dreifus-0.1.1/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.1.1/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.1.1/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:11.000000 dreifus-0.1.1/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.1.1/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.1.1/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.1.1/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.1.1/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:10.000000 dreifus-0.1.1/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2517 2023-07-20 13:46:09.000000 dreifus-0.1.1/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      922 2023-07-20 13:46:10.000000 dreifus-0.1.1/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-20 13:46:09.000000 dreifus-0.1.1/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-07-20 13:46:09.000000 dreifus-0.1.1/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-07-20 13:46:09.000000 dreifus-0.1.1/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-20 13:46:11.000000 dreifus-0.1.1/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.1.1/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.1.1/test/test_camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.1.1/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.1.1/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.1.1/test/test_vector.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dreifus-0.0.9/pyproject.toml` & `dreifus-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.9"
+version = "0.1.1"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
```

### Comparing `dreifus-0.0.9/src/dreifus/camera.py` & `dreifus-0.1.1/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/camera_bundle.py` & `dreifus-0.1.1/src/dreifus/camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/graphics.py` & `dreifus-0.1.1/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.1.1/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     def cy(self) -> float:
         return self[1, 2].item()
 
     @property
     def s(self) -> float:
         return self[0, 1].item()
 
-    def rescale(self, scale_factor: float, scale_factor_y: Optional[float] = None) -> 'Intrinsics':
+    def rescale(self,
+                scale_factor: float,
+                scale_factor_y: Optional[float] = None,
+                inplace: bool = True) -> 'Intrinsics':
         """
         When images that correspond to this intrinsics matrix are resized, the intrinsics should also be re-scaled
         to account for the image size change.
         This is because the intrinsics effectively just scales
         from the canonical screen space ([-1, 1]^2 with the image center in [0, 0])
         to the image screen space ([0, h] x [0, w] with the image center in [cx, cy]).
         Note: this is an inplace operation.
@@ -78,21 +81,26 @@
         Returns
         -------
             The re-scaled intrinsics matrix
         """
         scale_factor_x = scale_factor
         scale_factor_y = scale_factor if scale_factor_y is None else scale_factor_y
 
-        self[0, 0] *= scale_factor_x  # fx
-        self[1, 1] *= scale_factor_y  # fy
-        self[0, 2] *= scale_factor_x  # cx
-        self[1, 2] *= scale_factor_y  # cy
+        if inplace:
+            intrinsics = self
+        else:
+            intrinsics = self.copy()
+
+        intrinsics[0, 0] *= scale_factor_x  # fx
+        intrinsics[1, 1] *= scale_factor_y  # fy
+        intrinsics[0, 2] *= scale_factor_x  # cx
+        intrinsics[1, 2] *= scale_factor_y  # cy
         # TODO: What about s?
 
-        return self
+        return intrinsics
 
     def crop(self,
              crop_left: int = 0,
              crop_top: int = 0) -> 'Intrinsics':
         """
         When images that correspond to this intrinsics matrix are cropped, the intrinsics should also be adjusted
         to account for the image size change.
```

### Comparing `dreifus-0.0.9/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.1.1/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/matrix/pose_base.py` & `dreifus-0.1.1/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.1.1/src/dreifus/matrix/pose_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     def get_quaternion(self) -> Vec4:
         return Vec4(R.from_matrix(self.get_rotation_matrix()).as_quat())
 
     def get_translation(self) -> Vec3:
         # assert self.pose_type == PoseType.CAM_2_WORLD, "camera position only makes sense for CAM_2_WORLD poses"
         return Vec3(self[:3, 3])
 
-    def set_translation(self, x: Vec3TypeX, y: Optional[FloatType] = None, z: Optional[FloatType] = None):
+    def set_translation(self, x: Optional[Vec3TypeX] = None, y: Optional[FloatType] = None, z: Optional[FloatType] = None):
         x, y, z = unpack_3d_params(x, y, z)
         if x is not None:
             self[0, 3] = x
         if y is not None:
             self[1, 3] = y
         if z is not None:
             self[2, 3] = z
@@ -241,14 +241,15 @@
         pose[:, :] = axis_switcher @ pose
 
         return pose
 
     def change_camera_coordinate_convention(self,
                                             new_camera_coordinate_convention: CameraCoordinateConvention,
                                             inplace: bool = True) -> 'Pose':
+        # TODO: Make this work for WORLD_2_CAM poses as well
         assert self.pose_type == PoseType.CAM_2_WORLD, "Camera coordinate conventions can only be changed on CAM_2_WORLD matrices"
 
         current_ccc = self.camera_coordinate_convention
 
         if inplace:
             pose = self
         else:
@@ -263,21 +264,26 @@
         if current_ccc.z_direction != new_camera_coordinate_convention.z_direction:
             pose.negate_orientation_axis(2)
 
         pose.camera_coordinate_convention = new_camera_coordinate_convention
 
         return pose
 
-    def change_pose_type(self, new_pose_type: PoseType) -> 'Pose':
+    def change_pose_type(self,
+                         new_pose_type: PoseType,
+                         inplace: bool = True) -> 'Pose':
         assert self.pose_type in {PoseType.CAM_2_WORLD, PoseType.WORLD_2_CAM}, \
             "start pose must be either cam2world or world2cam"
         assert new_pose_type in {PoseType.CAM_2_WORLD, PoseType.WORLD_2_CAM}, \
             "target pose type must be either cam2world or world2cam"
 
-        pose = self.copy()
+        if inplace:
+            pose = self
+        else:
+            pose = self.copy()
 
         if pose.pose_type != new_pose_type:
             pose = pose.invert()
 
         return pose
 
     def get_look_direction(self) -> 'Vec3':
@@ -350,16 +356,16 @@
 
         assert self.pose_type in {PoseType.CAM_2_WORLD, PoseType.WORLD_2_CAM}, \
             "start pose must be either cam2world or world2cam"
         assert other.pose_type in {PoseType.CAM_2_WORLD, PoseType.WORLD_2_CAM}, \
             "target pose must be either cam2world or world2cam"
 
         # TODO: Continue
-        source_cam2world = self.change_pose_type(PoseType.CAM_2_WORLD)
-        target_cam2world = other.change_pose_type(PoseType.CAM_2_WORLD)
+        source_cam2world = self.change_pose_type(PoseType.CAM_2_WORLD, inplace=False)
+        target_cam2world = other.change_pose_type(PoseType.CAM_2_WORLD, inplace=False)
 
         rigid_transformation = target_cam2world @ source_cam2world.invert()
         assert rigid_transformation.pose_type == PoseType.CAM_2_CAM
 
         return rigid_transformation
 
     def __rmatmul__(self, other):
```

### Comparing `dreifus-0.0.9/src/dreifus/matrix/pose_torch.py` & `dreifus-0.1.1/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.1.1/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/pyvista.py` & `dreifus-0.1.1/src/dreifus/pyvista.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional, Union, Tuple
 
 import numpy as np
 import pyvista as pv
 
-
 # TODO: Points is not a float type. This can cause issues when transforming or applying filters.
 #  Casting to ``np.float32``. Disable this by passing ``force_float=False``
+import vtk
+
 from dreifus.camera import PoseType, CameraCoordinateConvention
 from dreifus.matrix import Pose, Intrinsics
 from dreifus.vector import Vec3, Vec4
 from pyvista import examples
 
 
 def add_coordinate_axes(p: pv.Plotter,
@@ -130,15 +131,14 @@
                        img_h: Optional[float] = None,
                        image: Optional[np.ndarray] = None,
                        color='lightgray',
                        size: float = 0.3,
                        label: Optional[Union[str, int]] = None,
                        line_width: float = 1,
                        look_vector_length: float = 0):
-
     if pose.pose_type == PoseType.WORLD_2_CAM:
         pose = pose.invert()
 
     pose = pose.change_camera_coordinate_convention(CameraCoordinateConvention.OPEN_CV, inplace=False)
 
     assert pose.pose_type == PoseType.CAM_2_WORLD
     assert pose.camera_coordinate_convention == CameraCoordinateConvention.OPEN_CV
@@ -242,7 +242,84 @@
         # up_direction *= -1
     focal_point = cam_to_world.get_translation() + look_direction
 
     p.camera_set = True
     p.camera_position = cam_to_world.get_translation().tolist()
     p.camera.focal_point = focal_point
     p.camera.up = up_direction  # TODO: Do we need to negate here? OpenCV coordinate y goes down
+
+
+def render_from_camera(p: pv.Plotter,
+                       pose: Pose,
+                       intrinsics: Intrinsics) -> np.ndarray:
+    """
+    Render the given scene from the specified camera.
+    The image size will be the size of the pyvista window.
+    The pyvista plotter should be initialized like this:
+    ```
+    p = pv.Plotter(off_screen=True, window_size=[IMG_W, IMG_H])
+    ```
+
+    Parameters
+    ----------
+        p: the pyvista scene to render
+        pose: extrinsics camera pose
+        intrinsics: camera intrinsics
+
+    Returns
+    -------
+        A numpy array [IMG_H, IMG_W, 4] containing the rendered scene. The background is transparent and a mask can
+        be obtained from the alpha channel
+    """
+
+    pose = pose.change_pose_type(PoseType.CAM_2_WORLD, inplace=False)
+    pose = pose.change_camera_coordinate_convention(CameraCoordinateConvention.OPEN_CV, inplace=False)
+    pose = pose.change_pose_type(PoseType.WORLD_2_CAM, inplace=False)
+
+    w = p.window_size[0]
+    h = p.window_size[1]
+
+    # ----------------------------------------------------------
+    # Intrinsics
+    # ----------------------------------------------------------
+    cx = intrinsics.cx
+    cy = intrinsics.cy
+    fx = intrinsics.fx
+    fy = intrinsics.fy
+
+    # convert the principal point to window center (normalized coordinate system) and set it
+    wcx = -2 * (cx - float(w) / 2) / w
+    wcy = 2 * (cy - float(h) / 2) / h
+    p.camera.SetWindowCenter(wcx, wcy)
+
+    # convert the focal length to view angle and set it
+    view_angle = 180 / np.pi * (2.0 * np.arctan2(h / 2.0, fx))
+    p.camera.SetViewAngle(view_angle)
+
+    # ----------------------------------------------------------
+    # Extrinsics
+    # ----------------------------------------------------------
+
+    # apply the transform to scene objects
+    vtk_pose = vtk.vtkMatrix4x4()
+    for i in range(pose.shape[0]):
+        for j in range(pose.shape[1]):
+            vtk_pose.SetElement(i, j, pose[i, j])
+
+    p.camera.SetModelTransformMatrix(vtk_pose)
+
+    # the camera can stay at the origin because we are transforming the scene objects
+    p.camera.SetPosition(0, 0, 0)
+
+    # look in the +Z direction of the camera coordinate system
+    p.camera.SetFocalPoint(0, 0, 1)
+
+    # the camera Y axis points down
+    p.camera.SetViewUp(0, -1, 0)
+
+    # ensure the relevant range of depths are rendered
+    p.renderer.ResetCameraClippingRange()
+
+    p.render()  # Important, otherwise view isn't updated when render_from_camera() is called multiple times
+    img = np.asarray(p.screenshot(transparent_background=True))
+
+    return img
```

### Comparing `dreifus-0.0.9/src/dreifus/trajectory.py` & `dreifus-0.1.1/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/vector/vector_base.py` & `dreifus-0.1.1/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/vector/vector_numpy.py` & `dreifus-0.1.1/src/dreifus/vector/vector_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus/vector/vector_torch.py` & `dreifus-0.1.1/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.1.1/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/test/test_camera.py` & `dreifus-0.1.1/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/test/test_camera_bundle.py` & `dreifus-0.1.1/test/test_camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/test/test_intrinsics.py` & `dreifus-0.1.1/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/test/test_pose.py` & `dreifus-0.1.1/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.9/test/test_vector.py` & `dreifus-0.1.1/test/test_vector.py`

 * *Files identical despite different names*

