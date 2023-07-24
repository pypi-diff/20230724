# Comparing `tmp/amunpy-0.9.8.tar.gz` & `tmp/amunpy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amunpy-0.9.8.tar", last modified: Fri Oct 14 15:38:39 2022, max compression
+gzip compressed data, was "amunpy-0.9.9.tar", last modified: Sun Oct 23 18:57:37 2022, max compression
```

## Comparing `amunpy-0.9.8.tar` & `amunpy-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-14 15:38:39.604740 amunpy-0.9.8/
--rw-r--r--   0 grzegorz  (1000) users      (100)    35149 2021-03-18 14:19:25.000000 amunpy-0.9.8/LICENSE
--rw-r--r--   0 grzegorz  (1000) users      (100)      655 2022-10-14 15:38:39.604740 amunpy-0.9.8/PKG-INFO
--rw-r--r--   0 grzegorz  (1000) users      (100)       90 2021-03-18 14:19:25.000000 amunpy-0.9.8/README.md
--rw-r--r--   0 grzegorz  (1000) users      (100)      104 2021-03-18 14:19:25.000000 amunpy-0.9.8/pyproject.toml
--rw-r--r--   0 grzegorz  (1000) users      (100)       38 2022-10-14 15:38:39.604740 amunpy-0.9.8/setup.cfg
--rw-r--r--   0 grzegorz  (1000) users      (100)      967 2022-10-14 15:36:25.000000 amunpy-0.9.8/setup.py
-drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-14 15:38:39.601739 amunpy-0.9.8/src/
-drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-14 15:38:39.603739 amunpy-0.9.8/src/amunpy/
--rw-r--r--   0 grzegorz  (1000) users      (100)      713 2022-10-14 15:36:38.000000 amunpy-0.9.8/src/amunpy/__init__.py
--rw-r--r--   0 grzegorz  (1000) users      (100)    56098 2022-10-14 15:33:34.000000 amunpy-0.9.8/src/amunpy/amun.py
--rw-r--r--   0 grzegorz  (1000) users      (100)     6289 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/amunh5.py
--rw-r--r--   0 grzegorz  (1000) users      (100)    34503 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/amunh5_deprecated.py
--rw-r--r--   0 grzegorz  (1000) users      (100)    12717 2022-07-14 20:34:51.000000 amunpy-0.9.8/src/amunpy/amunxml.py
--rw-r--r--   0 grzegorz  (1000) users      (100)     3451 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/integrals.py
--rw-r--r--   0 grzegorz  (1000) users      (100)     5320 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/interpolation.py
--rw-r--r--   0 grzegorz  (1000) users      (100)     8028 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/octree.py
--rw-r--r--   0 grzegorz  (1000) users      (100)     7636 2022-02-09 22:48:03.000000 amunpy-0.9.8/src/amunpy/vtkio.py
-drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-14 15:38:39.604740 amunpy-0.9.8/src/amunpy.egg-info/
--rw-r--r--   0 grzegorz  (1000) users      (100)      655 2022-10-14 15:38:39.000000 amunpy-0.9.8/src/amunpy.egg-info/PKG-INFO
--rw-r--r--   0 grzegorz  (1000) users      (100)      420 2022-10-14 15:38:39.000000 amunpy-0.9.8/src/amunpy.egg-info/SOURCES.txt
--rw-r--r--   0 grzegorz  (1000) users      (100)        1 2022-10-14 15:38:39.000000 amunpy-0.9.8/src/amunpy.egg-info/dependency_links.txt
--rw-r--r--   0 grzegorz  (1000) users      (100)       55 2022-10-14 15:38:39.000000 amunpy-0.9.8/src/amunpy.egg-info/requires.txt
--rw-r--r--   0 grzegorz  (1000) users      (100)        7 2022-10-14 15:38:39.000000 amunpy-0.9.8/src/amunpy.egg-info/top_level.txt
+drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-23 18:57:37.882599 amunpy-0.9.9/
+-rw-r--r--   0 grzegorz  (1000) users      (100)    35149 2022-10-15 19:28:32.000000 amunpy-0.9.9/LICENSE
+-rw-r--r--   0 grzegorz  (1000) users      (100)      655 2022-10-23 18:57:37.882599 amunpy-0.9.9/PKG-INFO
+-rw-r--r--   0 grzegorz  (1000) users      (100)       90 2022-10-15 19:28:32.000000 amunpy-0.9.9/README.md
+-rw-r--r--   0 grzegorz  (1000) users      (100)      104 2022-10-15 19:28:32.000000 amunpy-0.9.9/pyproject.toml
+-rw-r--r--   0 grzegorz  (1000) users      (100)       38 2022-10-23 18:57:37.882599 amunpy-0.9.9/setup.cfg
+-rw-r--r--   0 grzegorz  (1000) users      (100)      967 2022-10-23 18:55:57.000000 amunpy-0.9.9/setup.py
+drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-23 18:57:37.879599 amunpy-0.9.9/src/
+drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-23 18:57:37.881599 amunpy-0.9.9/src/amunpy/
+-rw-r--r--   0 grzegorz  (1000) users      (100)      713 2022-10-23 18:56:06.000000 amunpy-0.9.9/src/amunpy/__init__.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)    55620 2022-10-23 18:54:55.000000 amunpy-0.9.9/src/amunpy/amun.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)     6289 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/amunh5.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)    34503 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/amunh5_deprecated.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)    12717 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/amunxml.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)     3451 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/integrals.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)     5320 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/interpolation.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)     8028 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/octree.py
+-rw-r--r--   0 grzegorz  (1000) users      (100)     7636 2022-10-15 19:28:32.000000 amunpy-0.9.9/src/amunpy/vtkio.py
+drwxr-xr-x   0 grzegorz  (1000) users      (100)        0 2022-10-23 18:57:37.882599 amunpy-0.9.9/src/amunpy.egg-info/
+-rw-r--r--   0 grzegorz  (1000) users      (100)      655 2022-10-23 18:57:37.000000 amunpy-0.9.9/src/amunpy.egg-info/PKG-INFO
+-rw-r--r--   0 grzegorz  (1000) users      (100)      420 2022-10-23 18:57:37.000000 amunpy-0.9.9/src/amunpy.egg-info/SOURCES.txt
+-rw-r--r--   0 grzegorz  (1000) users      (100)        1 2022-10-23 18:57:37.000000 amunpy-0.9.9/src/amunpy.egg-info/dependency_links.txt
+-rw-r--r--   0 grzegorz  (1000) users      (100)       55 2022-10-23 18:57:37.000000 amunpy-0.9.9/src/amunpy.egg-info/requires.txt
+-rw-r--r--   0 grzegorz  (1000) users      (100)        7 2022-10-23 18:57:37.000000 amunpy-0.9.9/src/amunpy.egg-info/top_level.txt
```

### Comparing `amunpy-0.9.8/LICENSE` & `amunpy-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/PKG-INFO` & `amunpy-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amunpy
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Interface for the AMUN code's snapshots
 Home-page: https://www.amuncode.org/
 Author: Grzegorz Kowal
 Author-email: grzegorz@amuncode.org
 Project-URL: Bug Tracker, https://bitbucket.org/amunteam/amun-code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `amunpy-0.9.8/setup.py` & `amunpy-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="amunpy",
-    version="0.9.8",
+    version="0.9.9",
     author="Grzegorz Kowal",
     author_email="grzegorz@amuncode.org",
     description="Python Interface for the AMUN code's snapshots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.amuncode.org/",
     project_urls={
```

### Comparing `amunpy-0.9.8/src/amunpy/__init__.py` & `amunpy-0.9.9/src/amunpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 from .vtkio import *
 
 __all__ = [ 'AmunXML', 'AmunH5', 'WriteVTK', \
         'amun_attribute', 'amun_coordinate', 'amun_dataset', 'amun_dataset_vtk', 'amun_integrals' ]
 
 __author__ = "Grzegorz Kowal"
 __copyright__ = "Copyright 2018-2022 Grzegorz Kowal <grzegorz@amuncode.org>"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __maintainer__ = "Grzegorz Kowal"
 __email__ = "grzegorz@amuncode.org"
```

### Comparing `amunpy-0.9.8/src/amunpy/amun.py` & `amunpy-0.9.9/src/amunpy/amun.py`

 * *Files 9% similar despite different names*

```diff
@@ -312,152 +312,147 @@
             dset += tmp**2
             dset *= 0.5
         elif dataset == 'elex':
             by = self.__read_binary_data__('magy', chunk_number)
             bz = self.__read_binary_data__('magz', chunk_number)
             vy = self.__read_binary_data__('vely', chunk_number)
             vz = self.__read_binary_data__('velz', chunk_number)
-            dset = vy * bz - vz * by
+            dset = vz * by - vy * bz
             if self.attributes['resistivity'] > 0:
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(bz, -1, axis=iy) - numpy.roll(bz,  1, axis=iy))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(by,  1, axis=1) - numpy.roll(by, -1, axis=1))
-                    tmp += (numpy.roll(bz, -1, axis=2) - numpy.roll(bz,  1, axis=2))
-                else:
-                    tmp  = (numpy.roll(bz, -1, axis=1) - numpy.roll(bz,  1, axis=1))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(by,  1, axis=iz) - numpy.roll(by, -1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dset -= 0.5 * self.attributes['resistivity'] * tmp
+                dset += (self.attributes['resistivity'] / 2) * tmp
         elif dataset == 'eley':
             bx = self.__read_binary_data__('magx', chunk_number)
             bz = self.__read_binary_data__('magz', chunk_number)
             vx = self.__read_binary_data__('velx', chunk_number)
             vz = self.__read_binary_data__('velz', chunk_number)
-            dset = vz * bx - vx * bz
+            dset = vx * bz - vz * bx
             if self.attributes['resistivity'] > 0:
+                ix = self.attributes['ndims']
+                tmp  = (numpy.roll(bz,  1, axis=ix) - numpy.roll(bz, -1, axis=ix))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(bx, -1, axis=1) - numpy.roll(bx,  1, axis=1))
-                    tmp += (numpy.roll(bz,  1, axis=3) - numpy.roll(bz, -1, axis=3))
-                else:
-                    tmp  = (numpy.roll(bz,  1, axis=2) - numpy.roll(bz, -1, axis=2))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(bx, -1, axis=iz) - numpy.roll(bx,  1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dset -= 0.5 * self.attributes['resistivity'] * tmp
+                dset += (self.attributes['resistivity'] / 2) * tmp
         elif dataset == 'elez':
             bx = self.__read_binary_data__('magx', chunk_number)
             by = self.__read_binary_data__('magy', chunk_number)
             vx = self.__read_binary_data__('velx', chunk_number)
             vy = self.__read_binary_data__('vely', chunk_number)
-            dset = vx * by - vy * bx
+            dset = vy * bx - vx * by
             if self.attributes['resistivity'] > 0:
-                if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(bx,  1, axis=2) - numpy.roll(bx, -1, axis=2))
-                    tmp += (numpy.roll(by, -1, axis=3) - numpy.roll(by,  1, axis=3))
-                else:
-                    tmp  = (numpy.roll(bx,  1, axis=1) - numpy.roll(bx, -1, axis=1))
-                    tmp += (numpy.roll(by, -1, axis=2) - numpy.roll(by,  1, axis=2))
+                ix = self.attributes['ndims']
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(by, -1, axis=ix) - numpy.roll(by,  1, axis=ix))
+                tmp += (numpy.roll(bx,  1, axis=iy) - numpy.roll(bx, -1, axis=iy))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dset -= 0.5 * self.attributes['resistivity'] * tmp
+                dset += (self.attributes['resistivity'] / 2) * tmp
         elif dataset == 'elec':
             b1 = self.__read_binary_data__('magy', chunk_number)
             b2 = self.__read_binary_data__('magz', chunk_number)
             v1 = self.__read_binary_data__('vely', chunk_number)
             v2 = self.__read_binary_data__('velz', chunk_number)
-            dtmp = v1 * b2 - v2 * b1
+            dtmp = v2 * b1 - v1 * b2
             if self.attributes['resistivity'] > 0:
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(b2, -1, axis=iy) - numpy.roll(b2,  1, axis=iy))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1,  1, axis=1) - numpy.roll(b1, -1, axis=1))
-                    tmp += (numpy.roll(b2, -1, axis=2) - numpy.roll(b2,  1, axis=2))
-                else:
-                    tmp  = (numpy.roll(b2, -1, axis=1) - numpy.roll(b2,  1, axis=1))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(b1,  1, axis=iz) - numpy.roll(b1, -1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dtmp -= 0.5 * self.attributes['resistivity'] * tmp
+                dtmp += (self.attributes['resistivity'] / 2) * tmp
             dset  = dtmp**2
 
             b1 = self.__read_binary_data__('magx', chunk_number)
             v1 = self.__read_binary_data__('velx', chunk_number)
-            dtmp = v2 * b1 - v1 * b2
+            dtmp = v1 * b2 - v2 * b1
             if self.attributes['resistivity'] > 0:
+                ix = self.attributes['ndims']
+                tmp  = (numpy.roll(b2,  1, axis=ix) - numpy.roll(b2, -1, axis=ix))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1, -1, axis=1) - numpy.roll(b1,  1, axis=1))
-                    tmp += (numpy.roll(b2,  1, axis=3) - numpy.roll(b2, -1, axis=3))
-                else:
-                    tmp  = (numpy.roll(b2,  1, axis=2) - numpy.roll(b2, -1, axis=2))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(b1, -1, axis=iz) - numpy.roll(b1,  1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dtmp -= 0.5 * self.attributes['resistivity'] * tmp
+                dtmp += (self.attributes['resistivity'] / 2) * tmp
             dset += dtmp**2
 
             b2 = self.__read_binary_data__('magy', chunk_number)
             v2 = self.__read_binary_data__('vely', chunk_number)
-            dtmp = v1 * b2 - v2 * b1
+            dtmp = v2 * b1 - v1 * b2
             if self.attributes['resistivity'] > 0:
-                if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1,  1, axis=2) - numpy.roll(b1, -1, axis=2))
-                    tmp += (numpy.roll(b2, -1, axis=3) - numpy.roll(b2,  1, axis=3))
-                else:
-                    tmp  = (numpy.roll(b1,  1, axis=1) - numpy.roll(b1, -1, axis=1))
-                    tmp += (numpy.roll(b2, -1, axis=2) - numpy.roll(b2,  1, axis=2))
+                ix = self.attributes['ndims']
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(b2, -1, axis=ix) - numpy.roll(b2,  1, axis=ix))
+                tmp += (numpy.roll(b1,  1, axis=iy) - numpy.roll(b1, -1, axis=iy))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                dtmp -= 0.5 * self.attributes['resistivity'] * tmp
+                dtmp += (self.attributes['resistivity'] / 2) * tmp
+
             dset += dtmp**2
-            dset = numpy.sqrt(dset)
+            dset  = numpy.sqrt(dset)
         elif dataset == 'evec':
             b1 = self.__read_binary_data__('magy', chunk_number)
             b2 = self.__read_binary_data__('magz', chunk_number)
             v1 = self.__read_binary_data__('vely', chunk_number)
             v2 = self.__read_binary_data__('velz', chunk_number)
-            wx = v1 * b2 - v2 * b1
+            wx = v2 * b1 - v1 * b2
             if self.attributes['resistivity'] > 0:
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(b2, -1, axis=iy) - numpy.roll(b2,  1, axis=iy))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1,  1, axis=1) - numpy.roll(b1, -1, axis=1))
-                    tmp += (numpy.roll(b2, -1, axis=2) - numpy.roll(b2,  1, axis=2))
-                else:
-                    tmp  = (numpy.roll(b2, -1, axis=1) - numpy.roll(b2,  1, axis=1))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(b1,  1, axis=iz) - numpy.roll(b1, -1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                wx -= 0.5 * self.attributes['resistivity'] * tmp
+                wx += (self.attributes['resistivity'] / 2) * tmp
 
             b1 = self.__read_binary_data__('magx', chunk_number)
             v1 = self.__read_binary_data__('velx', chunk_number)
-            wy = v2 * b1 - v1 * b2
+            wy = v1 * b2 - v2 * b1
             if self.attributes['resistivity'] > 0:
+                ix = self.attributes['ndims']
+                tmp  = (numpy.roll(b2,  1, axis=ix) - numpy.roll(b2, -1, axis=ix))
                 if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1, -1, axis=1) - numpy.roll(b1,  1, axis=1))
-                    tmp += (numpy.roll(b2,  1, axis=3) - numpy.roll(b2, -1, axis=3))
-                else:
-                    tmp  = (numpy.roll(b2,  1, axis=2) - numpy.roll(b2, -1, axis=2))
+                    iz = self.attributes['ndims'] - 2
+                    tmp += (numpy.roll(b1, -1, axis=iz) - numpy.roll(b1,  1, axis=iz))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                wy -= 0.5 * self.attributes['resistivity'] * tmp
+                wy += (self.attributes['resistivity'] / 2) * tmp
 
             b2 = self.__read_binary_data__('magy', chunk_number)
             v2 = self.__read_binary_data__('vely', chunk_number)
             wz = v1 * b2 - v2 * b1
             if self.attributes['resistivity'] > 0:
-                if self.attributes['ndims'] == 3:
-                    tmp  = (numpy.roll(b1,  1, axis=2) - numpy.roll(b1, -1, axis=2))
-                    tmp += (numpy.roll(b2, -1, axis=3) - numpy.roll(b2,  1, axis=3))
-                else:
-                    tmp  = (numpy.roll(b1,  1, axis=1) - numpy.roll(b1, -1, axis=1))
-                    tmp += (numpy.roll(b2, -1, axis=2) - numpy.roll(b2,  1, axis=2))
+                ix = self.attributes['ndims']
+                iy = self.attributes['ndims'] - 1
+                tmp  = (numpy.roll(b2, -1, axis=ix) - numpy.roll(b2,  1, axis=ix))
+                tmp += (numpy.roll(b1,  1, axis=iy) - numpy.roll(b1, -1, axis=iy))
 
                 for p in range(self.chunks[chunk_number]['dblocks']):
                     tmp[p,...] /= self.cell_size[self.chunks[chunk_number]['levels'][p]]
-                wz -= 0.5 * self.attributes['resistivity'] * tmp
+                wz += (self.attributes['resistivity'] / 2) * tmp
 
             dset = [wx, wy, wz]
         elif dataset == 'eint':
             dset = self.__read_binary_data__('pres', chunk_number)
             dset *= 1.0 / (self.attributes('adiabatic_index') - 1)
         elif dataset == 'temp':
             dset = self.__read_binary_data__('pres', chunk_number) / self.__read_binary_data__('dens', chunk_number)
```

### Comparing `amunpy-0.9.8/src/amunpy/amunh5.py` & `amunpy-0.9.9/src/amunpy/amunh5.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/amunh5_deprecated.py` & `amunpy-0.9.9/src/amunpy/amunh5_deprecated.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/amunxml.py` & `amunpy-0.9.9/src/amunpy/amunxml.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/integrals.py` & `amunpy-0.9.9/src/amunpy/integrals.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/interpolation.py` & `amunpy-0.9.9/src/amunpy/interpolation.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/octree.py` & `amunpy-0.9.9/src/amunpy/octree.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy/vtkio.py` & `amunpy-0.9.9/src/amunpy/vtkio.py`

 * *Files identical despite different names*

### Comparing `amunpy-0.9.8/src/amunpy.egg-info/PKG-INFO` & `amunpy-0.9.9/src/amunpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amunpy
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Interface for the AMUN code's snapshots
 Home-page: https://www.amuncode.org/
 Author: Grzegorz Kowal
 Author-email: grzegorz@amuncode.org
 Project-URL: Bug Tracker, https://bitbucket.org/amunteam/amun-code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

