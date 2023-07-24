# Comparing `tmp/ccwriter-0.1.0.tar.gz` & `tmp/ccwriter-0.2.0.tar.gz`

## Comparing `ccwriter-0.1.0.tar` & `ccwriter-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.1.0/.python-version
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.1.0/requirements.lock
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ccwriter-0.1.0/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ccwriter-0.1.0/src/ccwriter/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.1.0/.gitignore
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ccwriter-0.1.0/README.md
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 ccwriter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 ccwriter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.python-version
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.0/requirements.lock
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ccwriter-0.2.0/src/ccwriter/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ccwriter-0.2.0/README.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 ccwriter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 ccwriter-0.2.0/PKG-INFO
```

### Comparing `ccwriter-0.1.0/.github/workflows/workflow.yaml` & `ccwriter-0.2.0/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `ccwriter-0.1.0/src/ccwriter/__init__.py` & `ccwriter-0.2.0/src/ccwriter/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,28 +2,37 @@
 
 https://www.cloudcompare.org/doc/wiki/index.php/BIN
 """
 
 from __future__ import annotations
 
 import io
+from enum import IntFlag
 from pathlib import Path
 from typing import IO, Union
 
 import numpy as np
 
 
+class CCFlags(IntFlag):
+    always_on = 1
+    colors = 2
+    normals = 4
+    scalar = 8
+    cloud_name = 16
+
+
 class CCWriter:
     """Write a CloudCompare BIN file."""
 
     def __init__(self, file: Union[str, Path, IO]) -> None:
         """
 
         Args:
-        file : str or Path or IO
+        file: str or Path or IO
             The file to write to.
         """
 
         self.cloud_counter = 0
         self.file = None
 
         if isinstance(file, (str, Path)):
@@ -84,36 +93,36 @@
         buffer = io.BytesIO()
         # Number of points
         buffer.write(count.to_bytes(4, "little"))
 
         combined_cloud = [cloud[:, 0], cloud[:, 1], cloud[:, 2]]
         dtypes = [("x", np.float32), ("y", np.float32), ("z", np.float32)]
 
-        flags = 1
+        flags = CCFlags.always_on
         if color is not None:
             if not isinstance(color, np.ndarray):
                 raise TypeError("Expected np.ndarray for 'colors'")
             if color.shape != (count, 3):
                 raise ValueError("Expected (count, 3) for 'colors'")
 
             combined_cloud.extend([color[:, 0], color[:, 1], color[:, 2]])
             dtypes.extend([("r", np.uint8), ("g", np.uint8), ("b", np.uint8)])
 
-            flags += 2
+            flags |= CCFlags.colors
         if normal is not None:
             if not isinstance(normal, np.ndarray):
                 raise TypeError("Expected np.ndarray for 'normals'")
 
             if normal.shape != (count, 3):
                 raise ValueError("Expected (count, 3) for 'normals'")
 
             combined_cloud.extend([normal[:, 0], normal[:, 1], normal[:, 2]])
             dtypes.extend([("nx", np.float32), ("ny", np.float32), ("nz", np.float32)])
 
-            flags += 4
+            flags |= CCFlags.normals
         if scalar is not None:
             if isinstance(scalar, int):
                 if scalar < 0 or cloud.ndim >= scalar:
                     raise ValueError("Expected scalar >= 0 and < cloud.ndim for 'scalar'")
                 scalar = cloud[:, scalar]
 
             if not isinstance(scalar, np.ndarray):
@@ -121,15 +130,15 @@
 
             if scalar.shape != (count,):
                 raise ValueError("Expected (count,) for 'scalar'")
 
             combined_cloud.append(scalar)
             dtypes.append(("scalar", np.float64))
 
-            flags += 8
+            flags |= CCFlags.scalar
         if name is not None:
             if not isinstance(name, str):
                 raise TypeError("Expected str for 'name'")
             flags += 16
 
         buffer.write(flags.to_bytes(1, "little"))
 
@@ -153,7 +162,54 @@
 
         self.file.seek(0)
         # Number of clouds
         self.file.write(self.cloud_counter.to_bytes(4, "little"))  # u32
 
         self.file.close()
         self.file = None
+
+
+class CCReader(dict):
+    def __init__(self, file: Union[str, Path, IO]) -> None:
+        """
+
+        Args:
+        file: str or Path or IO
+            The file to write to.
+        """
+
+        if isinstance(file, (str, Path)):
+            file = open(file, "rb")
+        elif not hasattr(file, "read") or not callable(file.read):
+            raise TypeError("Expected str, Path or IO for 'file'")
+
+        cloud_count = int.from_bytes(file.read(4), byteorder="little")  # cloud count
+
+        for idx in range(cloud_count):
+            number_of_points = int.from_bytes(file.read(4), byteorder="little")  # u32
+            flags = int.from_bytes(file.read(1), byteorder="little")  # u8
+
+            dtype = [("x", np.float32), ("y", np.float32), ("z", np.float32)]
+
+            if flags & CCFlags.colors:
+                dtype.extend([("r", np.uint8), ("g", np.uint8), ("b", np.uint8)])
+            if flags & CCFlags.normals:
+                dtype.extend([("nx", np.float32), ("ny", np.float32), ("nz", np.float32)])
+            if flags & CCFlags.scalar:
+                dtype.append(("scalar", np.float64))
+
+            name = None
+            if flags & CCFlags.cloud_name:
+                name = ""
+                while True:
+                    char = file.read(1)
+                    if char == b"\x00":
+                        break
+                    name += char.decode("ascii")
+
+            cloud = np.fromfile(file, dtype=dtype, count=number_of_points)
+
+            self[idx] = cloud
+            if name is not None:
+                self[name] = cloud
+
+        file.close()
```

### Comparing `ccwriter-0.1.0/README.md` & `ccwriter-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # CloudCompare bin writer
 
-Writer for the CloudCompare [BIN Format](https://www.cloudcompare.org/doc/wiki/index.php/BIN)
+Writer / Reader for the CloudCompare [BIN Format](https://www.cloudcompare.org/doc/wiki/index.php/BIN)
+
+## Installation
+
+```bash
+pip install ccwriter
+```
 
 ## Example
 
 ```python
 import numpy as np
 
-from ccwriter import CCWriter
+from ccwriter import CCReader, CCWriter
 
 amount = 10_000
 
 cloud = np.random.uniform(-100, 100, (amount, 3))
 color = np.random.uniform(-100, 100, (amount, 3))
 normal = np.random.uniform(-100, 100, (amount, 3))
 scaler = np.random.uniform(-100, 100, amount)
@@ -22,8 +28,18 @@
     cc.add_cloud(cloud, name="cloud")
     cc.add_cloud(cloud, name="cloud & color", color=color)
     cc.add_cloud(cloud, name="cloud & color & normal", color=color, normal=normal)
     cc.add_cloud(cloud, name="cloud & color & normal & scaler", color=color, normal=normal, scalar=scaler)
 
     cc.add_cloud(cloud_scaler, name="cloud_scaler & scaler_index", scalar=3)
 
+
+reader = CCReader("cloud.bin")
+
+print(reader[0].dtype)
+# (10000,) [('x', '<f4'), ('y', '<f4'), ('z', '<f4')]
+print(reader["cloud"].dtype)
+# (10000,) [('x', '<f4'), ('y', '<f4'), ('z', '<f4')]
+print(reader.keys())
+# dict_keys([0, 'cloud', 1, 'cloud & color', 2, 'cloud & color & normal', 3, 'cloud & color & normal & scaler', 4, 'cloud_scaler & scaler_index'])
+
 ```
```

### Comparing `ccwriter-0.1.0/pyproject.toml` & `ccwriter-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [project]
 name = "ccwriter"
-version = "0.1.0"
+version = "0.2.0"
 description = "Writer for CloudCompare .bin format"
 authors = [
     { name = "Marko Bausch", email = "60338487+mrkbac@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.22",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Framework :: Robot Framework :: Tool",
     "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.10",
-
+    "Programming Language :: Python :: 3.11",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
```

