# Comparing `tmp/sc-3D-1.0.2.tar.gz` & `tmp/sc-3D-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-3D-1.0.2.tar", last modified: Tue Jul 18 12:30:12 2023, max compression
+gzip compressed data, was "sc-3D-1.1.0.tar", last modified: Mon Jul 24 07:48:28 2023, max compression
```

## Comparing `sc-3D-1.0.2.tar` & `sc-3D-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 12:30:12.424887 sc-3D-1.0.2/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-1.0.2/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-18 12:30:12.424945 sc-3D-1.0.2/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     6683 2023-07-18 08:43:48.000000 sc-3D-1.0.2/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-1.0.2/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1562 2023-07-18 12:30:12.425699 sc-3D-1.0.2/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 12:30:12.422699 sc-3D-1.0.2/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 12:30:12.423731 sc-3D-1.0.2/src/sc3D/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       93 2023-07-18 12:29:28.000000 sc-3D-1.0.2/src/sc3D/__init__.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 12:30:12.424091 sc-3D-1.0.2/src/sc3D/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-1.0.2/src/sc3D/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-1.0.2/src/sc3D/_tests/test_sc3D.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    95033 2023-07-18 09:51:59.000000 sc-3D-1.0.2/src/sc3D/sc3D.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11169 2023-07-18 08:42:42.000000 sc-3D-1.0.2/src/sc3D/transformations.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 12:30:12.424784 sc-3D-1.0.2/src/sc_3D.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-18 12:30:12.000000 sc-3D-1.0.2/src/sc_3D.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      329 2023-07-18 12:30:12.000000 sc-3D-1.0.2/src/sc_3D.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-18 12:30:12.000000 sc-3D-1.0.2/src/sc_3D.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       92 2023-07-18 12:30:12.000000 sc-3D-1.0.2/src/sc_3D.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-07-18 12:30:12.000000 sc-3D-1.0.2/src/sc_3D.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:28.637823 sc-3D-1.1.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-1.1.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-24 07:48:28.637893 sc-3D-1.1.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     6683 2023-07-18 08:43:48.000000 sc-3D-1.1.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-1.1.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1562 2023-07-24 07:48:28.638207 sc-3D-1.1.0/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:28.635274 sc-3D-1.1.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:28.636578 sc-3D-1.1.0/src/sc3D/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       93 2023-07-24 07:46:38.000000 sc-3D-1.1.0/src/sc3D/__init__.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:28.636829 sc-3D-1.1.0/src/sc3D/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-1.1.0/src/sc3D/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-1.1.0/src/sc3D/_tests/test_sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)   100024 2023-07-24 07:43:05.000000 sc-3D-1.1.0/src/sc3D/sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11169 2023-07-18 08:42:42.000000 sc-3D-1.1.0/src/sc3D/transformations.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:28.637718 sc-3D-1.1.0/src/sc_3D.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-24 07:48:28.000000 sc-3D-1.1.0/src/sc_3D.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      329 2023-07-24 07:48:28.000000 sc-3D-1.1.0/src/sc_3D.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-24 07:48:28.000000 sc-3D-1.1.0/src/sc_3D.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       92 2023-07-24 07:48:28.000000 sc-3D-1.1.0/src/sc_3D.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-07-24 07:48:28.000000 sc-3D-1.1.0/src/sc_3D.egg-info/top_level.txt
```

### Comparing `sc-3D-1.0.2/LICENSE` & `sc-3D-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.2/PKG-INFO` & `sc-3D-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-3D
-Version: 1.0.2
+Version: 1.1.0
 Summary: Array alignment and 3D differential expression for 3D sc omics
 Home-page: https://github.com/GuignardLab/sc3D
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/sc3D/issues
 Project-URL: Documentation, https://github.com/GuignardLab/sc3D#README.md
```

### Comparing `sc-3D-1.0.2/README.md` & `sc-3D-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.2/pyproject.toml` & `sc-3D-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.2/setup.cfg` & `sc-3D-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sc-3D
-version = 1.0.2
+version = 1.1.0
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 url = https://github.com/GuignardLab/sc3D
 license = MIT
 description = Array alignment and 3D differential expression for 3D sc omics
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `sc-3D-1.0.2/src/sc3D/_tests/test_sc3D.py` & `sc-3D-1.1.0/src/sc3D/_tests/test_sc3D.py`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.2/src/sc3D/sc3D.py` & `sc-3D-1.1.0/src/sc3D/sc3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from scipy.spatial.distance import cdist
 from scipy.optimize import linear_sum_assignment
 from scipy.interpolate import InterpolatedUnivariateSpline, interp1d
 from scipy.stats import zscore, linregress
 from seaborn import scatterplot
 import json
 from pathlib import Path
+from time import time
 
 import anndata
 from sc3D.transformations import transformations as tr
 
 
 class Embryo:
     """
@@ -475,31 +476,28 @@
                     if self.tissue[c] == tissue
                 ]
             )
             positions_cs1 = np.array(
                 [
                     self.final.get(c, self.registered_pos[c])
                     for c in cells_cs1
-                    if self.tissue[c] == tissue
                 ]
             )
             if refine:
                 positions_cs2 = np.array(
                     [
                         self.pos_reg_aff[c]
                         for c in cells_cs2
-                        if self.tissue[c] == tissue
                     ]
                 )
             else:
                 positions_cs2 = np.array(
                     [
                         self.registered_pos[c]
                         for c in cells_cs2
-                        if self.tissue[c] == tissue
                     ]
                 )
             if len(positions_cs1) > 0 and len(positions_cs2) > 0:
                 distance = cdist(positions_cs1, positions_cs2)
                 copy_d = distance.copy()
                 if isinstance(th_d, bool):
                     th_d_tissue = np.max(distance) / 2
@@ -512,15 +510,16 @@
                 try:
                     pairing = linear_sum_assignment(distance)
                     pos_ref += list(positions_cs1[pairing[0]])
                     pos_flo += list(positions_cs2[pairing[1]])
                     self.pairing.update(
                         zip(cells_cs1[pairing[0]], cells_cs2[pairing[1]])
                     )
-                except Exception:
+                except Exception as e:
+                    print("re-doing linear sum assignment :(")
                     pairing = linear_sum_assignment(copy_d)
                     pos_ref_tmp = positions_cs1[pairing[0]]
                     pos_flo_tmp = positions_cs2[pairing[1]]
                     distance_paired = np.linalg.norm(
                         np.array(pos_ref_tmp) - np.array(pos_flo_tmp), axis=1
                     ).reshape(-1, 1)
                     to_keep = (distance_paired < th_d_tissue).reshape(-1)
@@ -533,15 +532,15 @@
                             cells_cs1[pairing[0][to_keep]],
                             cells_cs2[pairing[1][to_keep]],
                         )
                     )
         return pos_ref, pos_flo
 
     def register_cs(
-        self, cs1, cs2, refine=False, rigid=False, final=False, th_d=None
+        self, cs1, cs2, refine=False, rigid=False, final=False, th_d=None, timing=False
     ):
         """
         Registers the puck `cs2` onto the puck `cs1`.
 
         Args:
             cs1 (int): id of the first puck
             cs2 (int): id of the second puck
@@ -556,27 +555,41 @@
             th_d (bool | float): threshold above which a pairing is discarded.
                 If th_d is a boolean, then the threshold is the median of the
                 distribution of all the distances. If th_d is a float the value
                 given is used as a threshold.
                 Usually used as a float.
 
         """
+        if timing:
+            start = time()
+            if not hasattr(self, "timing"):
+                self.timing = {}
+            current_cs_timing = self.timing.setdefault((cs1, cs2), {})
         if self.registered_pos is None:
             self.register_with_tissues()
+            if timing:
+                current_cs_timing["register_with_tissues"] = time() - start
+                start = time()
         if (self.final is None) and final:
             self.final = {
                 c: self.centered_pos[c]
                 for c in self.cells_from_cover_slip[cs1]
             }
         pos_ref, pos_flo = self.build_pairing(
             cs1, cs2, rebuild=False, refine=refine, th_d=th_d
         )
+        if timing:
+            current_cs_timing["build_pairing"] = time() - start
+            start = time()
         M = self.register(
             np.array(pos_ref), np.array(pos_flo), apply=False, rigid=rigid
         )
+        if timing:
+            current_cs_timing["register"] = time() - start
+            start = time()
         cells_cs2 = self.cells_from_cover_slip[cs2]
         if refine:
             positions_cs2 = np.array([self.pos_reg_aff[c] for c in cells_cs2])
         else:
             positions_cs2 = np.array(
                 [self.registered_pos[c] for c in cells_cs2]
             )
@@ -584,14 +597,17 @@
             positions_cs2, ((0, 0), (0, 1)), "constant", constant_values=1
         ).T
         new_pos = np.dot(M, pos)[:2].T
         new_pos = pos[:2].T
         self.pos_reg_aff.update(zip(cells_cs2, new_pos))
         if final:
             self.final.update(zip(cells_cs2, new_pos))
+        if timing:
+            current_cs_timing["apply"] = time() - start
+            start = time()
         return M
 
     @staticmethod
     def build_gabriel_graph(node_ids, pos, data_struct="adj-dict", dist=False):
         """
         Build the gabriel graph of a set of nodes with
         associtated positions.
@@ -710,14 +726,110 @@
         tmp_raw = self.anndata.raw.to_adata()
         tmp_raw.X = product_sparse.toarray()
         if inplace:
             self.anndata.raw = tmp_raw
         else:
             return tmp_raw
 
+    def downsample(self, spacing=10, pos_id="pos_3D"):
+        """
+        Downsample the sample slice by slice on a grid defined by `spacing`.
+        For example, downsampling with a spacing of 10
+        will create new slices with a distance between beads of 10 units.
+        The expression of the new "beads" will be the average of the expression
+        of the beads within a radius `spacing/2` from the coordinate of the new bead.
+        The tissue assigned to the new bead is the tissue that is the most present within
+        the orginal beads in the radius `spacing/2`.
+        The function returns a anndata object (`out`) that can then be saved with the
+        anndata `write` function: out.write("path_to_file.h5ad").
+
+        Args:
+            spacing (int): the spacing between the x and y coordinates in the new grid
+            pos_id (str | dict): the position dictionary to take into account
+
+        Returns:
+            (anndata): the resampled anndata dataset with the following `.obs`:
+                - "nb_cells": The number of cells from the original dataset
+                              collected for the "bead"
+                - `self.pos_reg_id`: the new 3D position of the "bead"
+                - `self.tissue_id`: the tissue/cluster of the "bead"
+                - `self.array_id`: the array/puck of the "bead"
+        """
+        from itertools import product
+
+        first = True
+        mapping_from_removed = np.arange(max(self.all_cells) + 1)
+        mapping_from_removed[sorted(self.all_cells)] = np.arange(
+            len(self.all_cells)
+        )
+        if isinstance(pos_id, str):
+            pos_vals = self.__getattribute__(pos_id)
+        else:
+            pos_vals = pos_id
+        for s, s_cells in self.cells_from_cover_slip.items():
+            cells = [c for c in s_cells]
+            pos = np.array([pos_vals[c][:2] for c in s_cells])
+            min_x, min_y = np.min(pos, axis=0)
+            max_x, max_y = np.max(pos, axis=0)
+            x_coords = np.linspace(
+                min_x, max_x, int((max_x - min_x) // spacing)
+            )
+            y_coords = np.linspace(
+                min_y, max_y, int((max_y - min_y) // spacing)
+            )
+            coordinates = np.array(list(product(x_coords, y_coords)))
+            z = self.pos_3D[list(s_cells)[0]][-1] / 4
+            kdtree = KDTree(pos)
+            mapping = kdtree.query_ball_point(coordinates, spacing / 2)
+            final_positions = np.array(
+                [
+                    list(coordinates[i]) + [z]
+                    for i, v in enumerate(mapping)
+                    if 0 < len(v)
+                ]
+            )
+            final_expr = np.array(
+                [
+                    np.mean(
+                        self.anndata.raw[
+                            mapping_from_removed[[cells[vi] for vi in v]]
+                        ].X.A,
+                        axis=0,
+                    )
+                    for v in mapping
+                    if 0 < len(v)
+                ]
+            )
+            nb_cells = np.array([len(v) for v in mapping if 0 < len(v)])
+            tissue = [
+                np.unique(
+                    [self.tissue[cells[vi]] for vi in v], return_counts=True
+                )
+                for v in mapping
+                if 0 < len(v)
+            ]
+            tissue = np.array(
+                [self.corres_tissue[v[0][np.argmax(v[1])]] for v in tissue]
+            )
+            if first:
+                out = anndata.AnnData(final_expr, var=self.anndata.raw.var)
+                out.obs["nb_cells"] = nb_cells
+                out.obsm[self.pos_reg_id] = final_positions
+                out.obs[self.tissue_id] = tissue
+                out.obs[self.array_id] = s
+                first = False
+            else:
+                out_new = anndata.AnnData(final_expr, var=self.anndata.raw.var)
+                out_new.obs["nb_cells"] = nb_cells
+                out_new.obsm[self.pos_reg_id] = final_positions
+                out_new.obs[self.tissue_id] = tissue
+                out_new.obs[self.array_id] = s
+                out = anndata.concat([out, out_new])
+        return out
+
     def plot_coverslip(
         self,
         cs,
         pos="pos",
         ax=None,
         tissues_to_plot=None,
         legend=False,
@@ -792,19 +904,29 @@
                     * 3,
                 )
                 for t in tissues
             ]
         scatter = ax.scatter(*positions.T, c=color, **scatter_args)
         if legend:
             from matplotlib import colormaps
+
             cmap = colormaps[scatter_args["cmap"]]
-            mapping = lambda v: (v - scatter_args["vmin"]) / (scatter_args["vmax"] - scatter_args["vmin"])
+            mapping = lambda v: (v - scatter_args["vmin"]) / (
+                scatter_args["vmax"] - scatter_args["vmin"]
+            )
             for t in np.unique(tissues):
-                ax.plot([], [], linestyle="", marker=scatter_args["marker"], color=cmap(mapping(t)), label=self.corres_tissue.get(t, t))
-            ax.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+                ax.plot(
+                    [],
+                    [],
+                    linestyle="",
+                    marker=scatter_args["marker"],
+                    color=cmap(mapping(t)),
+                    label=self.corres_tissue.get(t, t),
+                )
+            ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
         if not pre_existing_ax:
             ax.set_aspect("equal")
             fig.tight_layout()
         if show:
             plt.show()
         return fig, ax
 
@@ -942,16 +1064,14 @@
         if cs is not None:
             cs_to_treat = cs
         else:
             cs_to_treat = self.all_cover_slips
         if self.z_pos is None or set(self.z_pos) != set(self.all_cells):
             self.set_zpos()
         if timing:
-            from time import time
-
             start = current_time = time()
             times = []
         self.trsfs = {}
         if isinstance(method, str) and method.lower() == "paste":
             try:
                 import paste as pst
             except:
@@ -1075,15 +1195,15 @@
 
         else:
             self.GG_cs = {}
             self.KDT_cs = {}
             for i, cs1 in enumerate(cs_to_treat[:-1]):
                 cs2 = cs_to_treat[i + 1]
                 self.trsfs[cs2] = self.register_cs(
-                    cs1, cs2, rigid=rigid, final=True, th_d=th_d
+                    cs1, cs2, rigid=rigid, final=True, th_d=th_d, timing=timing
                 )
                 if timing:
                     times.append([cs1, cs2, time() - current_time])
                     current_time = time()
 
             if timing:
                 times.append([-1, -1, time() - start])
@@ -2332,16 +2452,18 @@
         self.full_GG = None
         self.gene_expr_th = None
         self.whole_tissue_nb_N = None
         self.diff_expressed_3D = {}
         self.tissues_diff_expre_processed = None
         self.umap_id = umap_id
         self.array_id = array_id
+        self.tissue_id = tissue_id
         self.pos_id = pos_id
         self.__diff_expr_processed = {}
+        self.pos_reg_id = pos_reg_id
 
         if Path(data_path).suffix in [".h5ad", ".h5", ".csv"] or (
             0 < len(sample_list)
             and Path(sample_list[0]).suffix in [".h5ad", ".h5", ".csv"]
         ):
             self.read_anndata(
                 data_path,
```

### Comparing `sc-3D-1.0.2/src/sc3D/transformations.py` & `sc-3D-1.1.0/src/sc3D/transformations.py`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.2/src/sc_3D.egg-info/PKG-INFO` & `sc-3D-1.1.0/src/sc_3D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-3D
-Version: 1.0.2
+Version: 1.1.0
 Summary: Array alignment and 3D differential expression for 3D sc omics
 Home-page: https://github.com/GuignardLab/sc3D
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/sc3D/issues
 Project-URL: Documentation, https://github.com/GuignardLab/sc3D#README.md
```

