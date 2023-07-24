# Comparing `tmp/jax-md-0.2.6.tar.gz` & `tmp/jax-md-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-md-0.2.6.tar", last modified: Mon Jul 24 14:35:23 2023, max compression
+gzip compressed data, was "jax-md-0.2.7.tar", last modified: Mon Jul 24 15:49:10 2023, max compression
```

## Comparing `jax-md-0.2.6.tar` & `jax-md-0.2.7.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 17:59:08.000000 jax-md-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      574 2023-07-20 17:59:08.000000 jax-md-0.2.6/LICENSE_SHORT
--rw-r--r--   0 root         (0) root         (0)    19228 2023-07-24 14:35:23.346403 jax-md-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18222 2023-07-20 17:59:08.000000 jax-md-0.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/_nn/
--rw-r--r--   0 root         (0) root         (0)      667 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19618 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/behler_parrinello.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/_nn/e3nn_layer.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/gnome.py
--rw-r--r--   0 root         (0) root         (0)    15885 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/_nn/nequip.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/colab_tools/
--rw-r--r--   0 root         (0) root         (0)      615 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/colab_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9876 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/colab_tools/renderer.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/dataclasses.py
--rw-r--r--   0 root         (0) root         (0)    23043 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/elasticity.py
--rw-r--r--   0 root         (0) root         (0)    77180 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/energy.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/io.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/minimize.py
--rw-r--r--   0 root         (0) root         (0)    10567 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/nn.py
--rw-r--r--   0 root         (0) root         (0)    41487 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/partition.py
--rw-r--r--   0 root         (0) root         (0)    25660 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/quantity.py
--rw-r--r--   0 root         (0) root         (0)    39882 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/rigid_body.py
--rw-r--r--   0 root         (0) root         (0)    47018 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/simulate.py
--rw-r--r--   0 root         (0) root         (0)    36532 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/smap.py
--rw-r--r--   0 root         (0) root         (0)    16456 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/space.py
--rw-r--r--   0 root         (0) root         (0)    11874 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/test_util.py
--rw-r--r--   0 root         (0) root         (0)    58774 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/tpu.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/units.py
--rw-r--r--   0 root         (0) root         (0)     2838 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19228 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      722 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-24 14:35:23.346403 jax-md-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2314 2023-07-24 14:33:31.000000 jax-md-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.262566 jax-md-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 17:59:08.000000 jax-md-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      574 2023-07-20 17:59:08.000000 jax-md-0.2.7/LICENSE_SHORT
+-rw-r--r--   0 root         (0) root         (0)    19237 2023-07-24 15:49:10.262566 jax-md-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18231 2023-07-24 15:48:34.000000 jax-md-0.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.258567 jax-md-0.2.7/jax_md/
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.262566 jax-md-0.2.7/jax_md/_energy/
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-24 15:48:34.000000 jax-md-0.2.7/jax_md/_energy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10415 2023-07-24 15:48:34.000000 jax-md-0.2.7/jax_md/_energy/electrostatics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.262566 jax-md-0.2.7/jax_md/_nn/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/_nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19618 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/_nn/behler_parrinello.py
+-rw-r--r--   0 root         (0) root         (0)    14909 2023-07-24 15:45:31.000000 jax-md-0.2.7/jax_md/_nn/e3nn_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/_nn/gnome.py
+-rw-r--r--   0 root         (0) root         (0)    15837 2023-07-24 15:45:31.000000 jax-md-0.2.7/jax_md/_nn/nequip.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/_nn/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.262566 jax-md-0.2.7/jax_md/colab_tools/
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/colab_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9876 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/colab_tools/renderer.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-24 14:39:35.000000 jax-md-0.2.7/jax_md/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)    23043 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/elasticity.py
+-rw-r--r--   0 root         (0) root         (0)    77695 2023-07-24 15:48:34.000000 jax-md-0.2.7/jax_md/energy.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/io.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/minimize.py
+-rw-r--r--   0 root         (0) root         (0)    10567 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/nn.py
+-rw-r--r--   0 root         (0) root         (0)    41468 2023-07-24 15:45:31.000000 jax-md-0.2.7/jax_md/partition.py
+-rw-r--r--   0 root         (0) root         (0)    25660 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/quantity.py
+-rw-r--r--   0 root         (0) root         (0)    39882 2023-07-24 14:39:35.000000 jax-md-0.2.7/jax_md/rigid_body.py
+-rw-r--r--   0 root         (0) root         (0)    47018 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/simulate.py
+-rw-r--r--   0 root         (0) root         (0)    36532 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/smap.py
+-rw-r--r--   0 root         (0) root         (0)    16456 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/space.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    58774 2023-07-24 14:39:35.000000 jax-md-0.2.7/jax_md/tpu.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/units.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-07-20 17:59:08.000000 jax-md-0.2.7/jax_md/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:49:10.262566 jax-md-0.2.7/jax_md.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19237 2023-07-24 15:49:10.000000 jax-md-0.2.7/jax_md.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-24 15:49:10.000000 jax-md-0.2.7/jax_md.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:49:10.000000 jax-md-0.2.7/jax_md.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 15:49:10.000000 jax-md-0.2.7/jax_md.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 15:49:10.000000 jax-md-0.2.7/jax_md.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-24 15:49:10.262566 jax-md-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-07-24 15:45:54.000000 jax-md-0.2.7/setup.py
```

### Comparing `jax-md-0.2.6/LICENSE` & `jax-md-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/LICENSE_SHORT` & `jax-md-0.2.7/LICENSE_SHORT`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/PKG-INFO` & `jax-md-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-md
-Version: 0.2.6
+Version: 0.2.7
 Summary: Differentiable, Hardware Accelerated, Molecular Dynamics
 Home-page: https://github.com/google/jax-md
 Download-URL: https://pypi.org/project/jax-md/
 Author: Google
 Author-email: jax-md-dev@google.com
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/google/jax-md
@@ -169,15 +169,15 @@
 Cell List Example:
 ```python
 from jax_md import partition
 
 cell_size = 5.0
 capacity = 10
 cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
-cell_list_data = cell_list_fn(R)
+cell_list_data = cell_list_fn.allocate(R)
 ```
 
 Neighbor List Example:
 ```python
 from jax_md import partition
 
 neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
```

### Comparing `jax-md-0.2.6/README.md` & `jax-md-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 Cell List Example:
 ```python
 from jax_md import partition
 
 cell_size = 5.0
 capacity = 10
 cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
-cell_list_data = cell_list_fn(R)
+cell_list_data = cell_list_fn.allocate(R)
 ```
 
 Neighbor List Example:
 ```python
 from jax_md import partition
 
 neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
```

### Comparing `jax-md-0.2.6/jax_md/__init__.py` & `jax-md-0.2.7/jax_md/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/_nn/__init__.py` & `jax-md-0.2.7/jax_md/_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/_nn/behler_parrinello.py` & `jax-md-0.2.7/jax_md/_nn/behler_parrinello.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/_nn/e3nn_layer.py` & `jax-md-0.2.7/jax_md/_nn/e3nn_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,97 +204,91 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
 from typing import Optional
 
+import e3nn_jax as e3nn
 from e3nn_jax import Irreps
 from e3nn_jax import IrrepsArray
-from e3nn_jax import FunctionalLinear
 from e3nn_jax.legacy import FunctionalFullyConnectedTensorProduct
+from e3nn_jax import FunctionalLinear 
+from e3nn_jax.utils import vmap
 
 import flax.linen as nn
 
 import jax
 import jax.numpy as jnp
 
 from jax.nn import initializers
 from jax import tree_util
 from jax import jit
-from jax import vmap
 from jax import tree_map
 
 import numpy as onp
 
-
-def naive_broadcast_decorator(func):
-  def wrapper(*args):
-      leading_shape = jnp.broadcast_shapes(*(arg.shape[:-1] for arg in args))
-      args = [arg.broadcast_to(leading_shape + (-1,)) for arg in args]
-      f = func
-      for _ in range(len(leading_shape)):
-          f = jax.vmap(f)
-      return f(*args)
-
-  return wrapper
-
-
 class FullyConnectedTensorProductE3nn(nn.Module):
   """Flax module of an equivariant Fully-Connected Tensor Product."""
   irreps_out: Irreps
   irreps_in1: Optional[Irreps] = None
   irreps_in2: Optional[Irreps] = None
 
   @nn.compact
-  def __call__(self, x1: IrrepsArray, x2: IrrepsArray) -> IrrepsArray:
-
+  def __call__(self, x1: IrrepsArray, x2: IrrepsArray, **kwargs) -> IrrepsArray:
     irreps_out = Irreps(self.irreps_out)
     irreps_in1 = Irreps(
         self.irreps_in1
         ) if self.irreps_in1 is not None else None
     irreps_in2 = Irreps(
         self.irreps_in2
         ) if self.irreps_in2 is not None else None
 
+    x1 = e3nn.as_irreps_array(x1)
+    x2 = e3nn.as_irreps_array(x2)
+
+    leading_shape = jnp.broadcast_shapes(x1.shape[:-1], x2.shape[:-1])
+    x1 = x1.broadcast_to(leading_shape + (-1,))
+    x2 = x2.broadcast_to(leading_shape + (-1,))
+
     if irreps_in1 is not None:
-      x1 = IrrepsArray(irreps_in1, x1)
+        x1 = x1.rechunk(irreps_in1)
     if irreps_in2 is not None:
-      x2 = IrrepsArray(irreps_in2, x2)
+        x2 = x2.rechunk(irreps_in2)
 
-    x1 = x1.remove_nones().simplify()
-    x2 = x2.remove_nones().simplify()
+    x1 = x1.remove_zero_chunks().simplify()
+    x2 = x2.remove_zero_chunks().simplify()
 
     tp = FunctionalFullyConnectedTensorProduct(
-        x1.irreps,
-        x2.irreps,
-        irreps_out.simplify()
-        )
+        x1.irreps, x2.irreps, irreps_out.simplify()
+    )
 
     ws = [
         self.param(
             (
                 f"w[{ins.i_in1},{ins.i_in2},{ins.i_out}] "
                 f"{tp.irreps_in1[ins.i_in1]},"
                 f"{tp.irreps_in2[ins.i_in2]},{tp.irreps_out[ins.i_out]}"
                 ),
             nn.initializers.normal(stddev=ins.weight_std),
             ins.path_shape
             )
         for ins in tp.instructions
     ]
 
-    f = naive_broadcast_decorator(lambda x1, x2: tp.left_right(ws, x1, x2))
+    f = lambda x1, x2: tp.left_right(ws, x1, x2, **kwargs)
+
+    for _ in range(len(leading_shape)):
+        f = e3nn.utils.vmap(f)
+
     output = f(x1, x2)
-    output = tree_map(lambda x: x.astype(x1.dtype), output)
     return output.rechunk(irreps_out)
 
 
 class Linear(nn.Module):
-  """Flax module of an equivariant Linear."""
   irreps_out: Irreps
   irreps_in: Optional[Irreps] = None
 
   @nn.compact
   def __call__(self, x: IrrepsArray) -> IrrepsArray:
     irreps_out = Irreps(self.irreps_out)
     irreps_in = Irreps(self.irreps_in) if self.irreps_in is not None else None
@@ -325,11 +319,9 @@
             )
         for ins in lin.instructions
         ]
 
     f = lambda x: lin(w, x)
     for _ in range(x.ndim - 1):
       f = vmap(f)
-    output = f(x)
-    output = tree_map(lambda y: y.astype(x.dtype), output)
-    return output
+    return f(x)
```

### Comparing `jax-md-0.2.6/jax_md/_nn/gnome.py` & `jax-md-0.2.7/jax_md/_nn/gnome.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/_nn/nequip.py` & `jax-md-0.2.7/jax_md/_nn/nequip.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 Irrep = e3nn.Irrep
 Array = util.Array
 FeaturizerFn = nn_util.FeaturizerFn
 
 
 get_nonlinearity_by_name = nn_util.get_nonlinearity_by_name
 partial = functools.partial
-
+tree_map = partial(jax.tree_map, is_leaf=lambda x: isinstance(x, e3nn.IrrepsArray))
 
 # Code
 
 
 def prod(xs):
   """From e3nn_jax/util/__init__.py."""
   return functools.reduce(operator.mul, xs, 1)
@@ -176,25 +176,23 @@
     # this can equivalently be seen as a matrix multiplication acting on
     # the node features where the weight matrix is indexed by the node
     # attributes (typically the chemical species), i.e. a linear transform
     # that is a function of the species of the central atom
     if self.use_sc:
       self_connection = FullyConnectedTensorProductE3nn(
           h_out_irreps,
-          # node_features.irreps,
-          # node_attributes.irreps
           )(node_features, node_attributes)
 
     h = node_features
 
     # first linear, stays in current h-space
     h = Linear(node_features.irreps)(h)
 
     # map node features onto edges for tp
-    edge_features = jax.tree_map(lambda x: x[edge_src], h)
+    edge_features = tree_map(lambda x: x[edge_src], h)
 
     # we gather the instructions for the tp as well as the tp output irreps
     mode = 'uvu'
     trainable = 'True'
     irreps_after_tp = []
     instructions = []
 
@@ -254,27 +252,25 @@
         )
 
     # the TP weights (v dimension) are given by the FC
     weight = fc(edge_embedded)
 
     # tp between node features that have been mapped onto edges and edge RSH
     # weighted by FC weight, we vmap over the dimension of the edges
-    edge_features = jax.vmap(tp.left_right)(weight, edge_features, edge_sh)
+    edge_features = e3nn.utils.vmap(tp.left_right)(weight, edge_features, edge_sh)
     # TODO: It's not great that e3nn_jax automatically upcasts internally,
     # but this would need to be fixed at the e3nn level.
-    edge_features = jax.tree_map(lambda x: x.astype(h.dtype), edge_features)
+    edge_features = tree_map(lambda x: x.astype(h.dtype), edge_features)
 
     # aggregate edges onto nodes after tp using e3nn-jax's index_add
     h_type = h.dtype
-    h = jax.tree_map(
-        lambda x: e3nn.index_add(edge_dst, x, out_dim=h.shape[0]),
-        edge_features
-        )
-    # TODO: Remove this once e3nn_jax doesn't upcast inputs.
-    h = jax.tree_map(lambda x: x.astype(h_type), h)
+
+    e = edge_features.remove_zero_chunks().simplify()
+    h = e3nn.index_add(edge_dst, e, out_dim=h.shape[0])
+    h = h.astype(h_type)
 
     # normalize by the average (not local) number of neighbors
     h = h / self.n_neighbors
 
     # second linear, now we create extra gate scalars by mapping to h-out
     h = Linear(h_out_irreps)(h)
 
@@ -294,15 +290,15 @@
         odd_act=get_nonlinearity_by_name(self.nonlinearities['o']),
         even_gate_act=get_nonlinearity_by_name(self.nonlinearities['e']),
         odd_gate_act=get_nonlinearity_by_name(self.nonlinearities['o'])
         )
 
     h = gate_fn(h)
     # TODO: Remove this once e3nn_jax doesn't upcast inputs.
-    h = jax.tree_map(lambda x: x.astype(h_type), h)
+    h = tree_map(lambda x: x.astype(h_type), h)
 
     return h
 
 
 class NequIPEnergyModel(nn.Module):
   """NequIP.
 
@@ -413,23 +409,23 @@
 
     # shift + scale atomic energies
     atomic_output = self.scale * atomic_output + self.shift
 
     # this aggregation follows jraph/_src/models.py
     n_graph = graph.n_node.shape[0]
     graph_idx = jnp.arange(n_graph)
-    sum_n_node = tree_util.tree_leaves(graph.nodes)[0].shape[0]
+    sum_n_node = tree_util.tree_leaves(graph.nodes, is_leaf=lambda x: isinstance(x, e3nn.IrrepsArray))[0].shape[0]
     node_gr_idx = jnp.repeat(
         graph_idx,
         graph.n_node,
         axis=0,
         total_repeat_length=sum_n_node
         )
 
-    global_output = tree_util.tree_map(
+    global_output = tree_map(
         lambda n: jraph.segment_sum(
             n,
             node_gr_idx,
             n_graph
             ), atomic_output)
 
     return global_output
```

### Comparing `jax-md-0.2.6/jax_md/_nn/util.py` & `jax-md-0.2.7/jax_md/_nn/util.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/colab_tools/__init__.py` & `jax-md-0.2.7/jax_md/colab_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/colab_tools/renderer.py` & `jax-md-0.2.7/jax_md/colab_tools/renderer.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/dataclasses.py` & `jax-md-0.2.7/jax_md/dataclasses.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/elasticity.py` & `jax-md-0.2.7/jax_md/elasticity.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/energy.py` & `jax-md-0.2.7/jax_md/energy.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,26 @@
 import haiku as hk
 from jax.scipy.special import erfc  # error function
 from jax_md import space, smap, partition, nn, quantity, interpolate, util
 
 from ml_collections import ConfigDict
 
 
+# Electrostatics
+
+
+from jax_md._energy.electrostatics import coulomb_direct_pair
+from jax_md._energy.electrostatics import coulomb_direct_neighbor_list
+from jax_md._energy.electrostatics import coulomb_recip_ewald
+from jax_md._energy.electrostatics import coulomb_recip_pme
+from jax_md._energy.electrostatics import coulomb_ewald_neighbor_list
+from jax_md._energy.electrostatics import coulomb
+from jax_md._energy.electrostatics import coulomb_neighbor_list
+
+
 # Define aliases different neural network primitives.
 bp = nn.behler_parrinello
 gnome = nn.gnome
 nequip = nn.nequip
 
 maybe_downcast = util.maybe_downcast
 
@@ -1014,20 +1026,20 @@
 
   Returns:
     Bond-order values between i and j atoms
   """
   drij = space.distance(dRij)
   drik = space.distance(dRik)
 
-  mask_ijk *= (1 - jnp.eye(mask_ijk.shape[-1]))[None, :, :]
+  mask_ijk *= (1 - jnp.eye(mask_ijk.shape[-1], dtype=dRij.dtype))[None, :, :]
 
   # compute g_ijk - angle penalty value
   costheta = quantity.cosine_angles(dRij)
   gijk = 1.0 + (c**2 / d**2) - (c**2 / (d**2 + (h - costheta)**2))
-
+  
   # compute exponential term - distance penalty value
   dr_diff = drij[:, None, :] - drik[:, :, None]
   dr_diff = jnp.where(mask_ijk, dr_diff, 0)
   explr3 = jnp.exp(lam3**m * dr_diff**m)
 
   # compute fC with dr_ik
   fC = _ters_cutoff(drik, R, D)
@@ -1142,15 +1154,17 @@
                           params['nTf'], params['mTf'])
   # define compute functions.
   def compute_fn(R, **kwargs):
     d = partial(displacement, **kwargs)
     dR = space.map_product(d)(R, R)
     dr = space.distance(dR)
     N = R.shape[0]
-    mask = jnp.where(1 - jnp.eye(N), dr < params['R'] + params['D'], 0)
+    mask = jnp.where(1 - jnp.eye(N), 
+                     dr < params['R'] + params['D'], 0)
+    mask = mask.astype(R.dtype)
     mask_ijk = mask[:, None, :] * mask[:, :, None]
     repulsive = util.safe_mask(mask, repulsive_fn, dr)
     attractive = attractive_fn(dR, dR, mask_ijk) * mask
     first_term = util.high_precision_sum(repulsive)
     second_term = util.high_precision_sum(attractive)
     return first_term + second_term
   return compute_fn
@@ -1310,31 +1324,31 @@
   l_tau = (l_ijk + tau_Z) ** 2
   term2 = ((1 - jnp.exp(-Q_Z * l_tau)) + (eta * Q_Z * l_tau))
 
   within_cutoff = (dr12 > 0) & (dr13 > 0) & (jnp.linalg.norm(dR12 - dR13) > 1e-5)
   return jnp.where(within_cutoff, lam * term1 * term2, 0)
 
 def edip(displacement: DisplacementFn,
-           u1: f64 = -0.165799,
-           u2: f64 = 32.557,
-           u3: f64 = 0.286198,
-           u4: f64 = 0.66,
-           rho: f64 = 1.2085196,
-           eta: f64 = 0.2523244,
-           Q_0: f64 = 312.1341346,
-           mu: f64 = 0.6966326,
-           beta: f64 = 0.0070975,
-           alpha: f64 = 3.1083847,
-           A: f64 = 7.9821730,
-           lam: f64 = 1.4533108,
-           B: f64 = 1.5075463,
-           gamma: f64 = 1.1247945,
-           sigma: f64 = 0.5774108,
-           c: f64 = 2.5609104,
-           cutoff: f64 = 3.1213820) -> Callable[[Array], Array]:
+         u1: f64 = -0.165799,
+         u2: f64 = 32.557,
+         u3: f64 = 0.286198,
+         u4: f64 = 0.66,
+         rho: f64 = 1.2085196,
+         eta: f64 = 0.2523244,
+         Q_0: f64 = 312.1341346,
+         mu: f64 = 0.6966326,
+         beta: f64 = 0.0070975,
+         alpha: f64 = 3.1083847,
+         A: f64 = 7.9821730,
+         lam: f64 = 1.4533108,
+         B: f64 = 1.5075463,
+         gamma: f64 = 1.1247945,
+         sigma: f64 = 0.5774108,
+         c: f64 = 2.5609104,
+         cutoff: f64 = 3.1213820) -> Callable[[Array], Array]:
     """
     Computes the the Environment-dependent interatomic potential (EDIP).
     The parameter values are for bulk Silicon [1,2]. The EDIP potential is a bond
     order potential which depends on the local coordination number of the atom.
 
     :param displacement: displacement function for the space.
     :param u1: parameter for the three-body bond order function tau(Z) (pure number)
@@ -1371,15 +1385,15 @@
 
     def compute_fn(R, **kwargs):
       _three_body_fn = vmap(vmap(vmap(three_body_fn, (None, 0, None)), (None, None, 0)))
       d = partial(displacement, **kwargs)
       dR = space.map_product(d)(R, R)
       dr = space.distance(dR)
       N = R.shape[0]
-      mask = (1 - jnp.eye(N)) * (dr < cutoff)
+      mask = (1 - jnp.eye(N, dtype=R.dtype)) * (dr < cutoff)
       first_term = util.high_precision_sum(two_body_fn(mask, dr))
       second_term = util.high_precision_sum(_three_body_fn(mask, dR, dR)) / 2.0
       return first_term + second_term
 
     return compute_fn
```

### Comparing `jax-md-0.2.6/jax_md/interpolate.py` & `jax-md-0.2.7/jax_md/interpolate.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/io.py` & `jax-md-0.2.7/jax_md/io.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/minimize.py` & `jax-md-0.2.7/jax_md/minimize.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/nn.py` & `jax-md-0.2.7/jax_md/nn.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/partition.py` & `jax-md-0.2.7/jax_md/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from operator import mul
 
 import numpy as onp
 
 from jax import lax
 from jax import ops
 from jax import jit, vmap, eval_shape
-from jax.abstract_arrays import ShapedArray
+from jax.core import ShapedArray
 from jax.interpreters import partial_eval as pe
 from jax import tree_map
 import jax.numpy as jnp
 
 from jax_md import space
 from jax_md import dataclasses
 from jax_md import util
@@ -290,15 +290,15 @@
     an explicit integer denoting the capacity. Note that an existing cell list
     can also be updated by calling `cell_list.update(position)`.
   """
 
   if util.is_array(box_size):
     box_size = onp.array(box_size)
     if len(box_size.shape) == 1:
-      box_size = jnp.reshape(box_size, (1, -1))
+      box_size = onp.reshape(box_size, (1, -1))
 
   if util.is_array(minimum_cell_size):
     minimum_cell_size = onp.array(minimum_cell_size)
 
   def cell_list_fn(position: Array,
                    capacity_overflow_update: Optional[
                        Tuple[int, bool, Callable[..., CellList]]] = None,
@@ -586,15 +586,15 @@
     return True
   if box.ndim == 2:
     return jnp.triu(box) == box
   return False
 
 
 @dataclasses.dataclass
-class NeighborList(object):
+class NeighborList:
   """A struct containing the state of a Neighbor List.
 
   Attributes:
     idx: For an N particle system this is an `[N, max_occupancy]` array of
       integers such that `idx[i, j]` is the j-th neighbor of particle i.
     reference_position: The positions of particles when the neighbor list was
       constructed. This is used to decide whether the neighbor list ought to be
```

### Comparing `jax-md-0.2.6/jax_md/quantity.py` & `jax-md-0.2.7/jax_md/quantity.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/rigid_body.py` & `jax-md-0.2.7/jax_md/rigid_body.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/simulate.py` & `jax-md-0.2.7/jax_md/simulate.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/smap.py` & `jax-md-0.2.7/jax_md/smap.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/space.py` & `jax-md-0.2.7/jax_md/space.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/test_util.py` & `jax-md-0.2.7/jax_md/test_util.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/tpu.py` & `jax-md-0.2.7/jax_md/tpu.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/units.py` & `jax-md-0.2.7/jax_md/units.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md/util.py` & `jax-md-0.2.7/jax_md/util.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.6/jax_md.egg-info/PKG-INFO` & `jax-md-0.2.7/jax_md.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-md
-Version: 0.2.6
+Version: 0.2.7
 Summary: Differentiable, Hardware Accelerated, Molecular Dynamics
 Home-page: https://github.com/google/jax-md
 Download-URL: https://pypi.org/project/jax-md/
 Author: Google
 Author-email: jax-md-dev@google.com
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/google/jax-md
@@ -169,15 +169,15 @@
 Cell List Example:
 ```python
 from jax_md import partition
 
 cell_size = 5.0
 capacity = 10
 cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
-cell_list_data = cell_list_fn(R)
+cell_list_data = cell_list_fn.allocate(R)
 ```
 
 Neighbor List Example:
 ```python
 from jax_md import partition
 
 neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
```

### Comparing `jax-md-0.2.6/jax_md.egg-info/SOURCES.txt` & `jax-md-0.2.7/jax_md.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 jax_md/units.py
 jax_md/util.py
 jax_md.egg-info/PKG-INFO
 jax_md.egg-info/SOURCES.txt
 jax_md.egg-info/dependency_links.txt
 jax_md.egg-info/requires.txt
 jax_md.egg-info/top_level.txt
+jax_md/_energy/__init__.py
+jax_md/_energy/electrostatics.py
 jax_md/_nn/__init__.py
 jax_md/_nn/behler_parrinello.py
 jax_md/_nn/e3nn_layer.py
 jax_md/_nn/gnome.py
 jax_md/_nn/nequip.py
 jax_md/_nn/util.py
 jax_md/colab_tools/__init__.py
```

### Comparing `jax-md-0.2.6/setup.py` & `jax-md-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'e3nn-jax',
     'dm-haiku',
     'optax',
 ]
 
 setuptools.setup(
     name='jax-md',
-    version='0.2.6',
+    version='0.2.7',
     license='Apache 2.0',
     author='Google',
     author_email='jax-md-dev@google.com',
     install_requires=INSTALL_REQUIRES,
     url='https://github.com/google/jax-md',
     packages=setuptools.find_packages(),
     download_url = "https://pypi.org/project/jax-md/",
```

