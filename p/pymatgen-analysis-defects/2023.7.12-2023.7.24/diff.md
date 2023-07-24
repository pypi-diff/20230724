# Comparing `tmp/pymatgen-analysis-defects-2023.7.12.tar.gz` & `tmp/pymatgen-analysis-defects-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.7.12.tar", last modified: Thu Jul 13 00:14:31 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.7.24.tar", last modified: Mon Jul 24 21:13:17 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.7.12.tar` & `pymatgen-analysis-defects-2023.7.24.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.613632 pymatgen-analysis-defects-2023.7.12/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.613632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.621632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.621632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.735245 pymatgen-analysis-defects-2023.7.24/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.735245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28842 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39802 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.7.12/LICENSE` & `pymatgen-analysis-defects-2023.7.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/PKG-INFO` & `pymatgen-analysis-defects-2023.7.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.7.12
+Version: 2023.7.24
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.7.12/README.rst` & `pymatgen-analysis-defects-2023.7.24/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 import numpy as np
 from monty.json import MSONable
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core import Element, PeriodicSite, Species, Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.symmetry.structure import SymmetrizedStructure
-from pyrho.utils import get_plane_spacing
 
 from pymatgen.analysis.defects.supercells import get_sc_fromstruct
 
+from .utils import get_plane_spacing
+
 # TODO Possible redesign idea: ``DefectSite`` class defined with a defect object.
 # This makes some of the accounting logic a bit harder since we will probably
 # just have one concrete ``Defect`` class so you can write custom multiplicity functions
 # but it makes the implementation of defect complexes trivial.
 # i.e. each defect will be defined by a structure and a collection of ``DefectSite``s
 
 __author__ = "Jimmy-Xuan Shen"
@@ -410,15 +411,15 @@
         rm_oxi = self.structure[self.defect_site_index].specie.oxi_state
         sub_states = self.site.specie.common_oxidation_states
         if len(sub_states) == 0:
             raise ValueError(
                 f"No common oxidation states found for {self.site.specie}."
                 "Please specify the oxidation state manually."
             )
-        sub_oxi = sub_states[0]
+        sub_oxi = min(sub_states, key=lambda x: abs(x - rm_oxi))
         return sub_oxi - rm_oxi
 
     def __repr__(self) -> str:
         """Representation of a substitutional defect."""
         rm_species = get_element(self.defect_site.specie)
         sub_species = get_element(self.site.specie)
         return (
```

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             shape (n_sites, n_soap_features)
     """
     adaptor = AseAtomsAdaptor()
     species_ = [str(el) for el in struct.composition.elements]
     dummy_structure = struct.copy()
     for el in species_:
         dummy_structure.replace_species({str(el): DUMMY_SPECIES})
-    soap_desc = SOAP(species=[DUMMY_SPECIES], rcut=5, nmax=8, lmax=6, periodic=True)
+    soap_desc = SOAP(species=[DUMMY_SPECIES], r_cut=5, n_max=8, l_max=6, periodic=True)
     vecs = soap_desc.create(adaptor.get_atoms(dummy_structure))
     return vecs
 
 
 def get_site_vecs(struct: Structure):
     """Get the SiteVec representation of each site in the structure."""
     vecs = get_soap_vec(struct)
```

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1039,7 +1039,45 @@
             sgroups = list(_group_docs_by_structure(list(g), sm, get_structure))
             if len(sgroups) <= 1:
                 for group in sgroups:
                     yield h, group
             else:
                 for itr, group in enumerate(sgroups):
                     yield f"{h}:{itr}", group
+
+
+def get_plane_spacing(lattice: npt.NDArray) -> list[float]:
+    """Get the cartesian spacing between periodic planes of a unit cell.
+    Copied from materialsproject/pyrho
+
+    >>> get_plane_spacing([[1,0,0], [1,1,0], [0,0,2]])
+    [0.7653..., 1.042..., 2.0]
+
+    Args:
+    lattice:
+        List of lattice vectors in cartesian coordinates
+
+    Returns:
+    List[float]:
+        List where the k-th element is is the spacing of planes generated by all
+        lattice vectors EXCEPT the k-th one
+
+    """
+    # get all pairwise projections i must be smaller than j
+    ndim = len(lattice)
+    idx_pairs = [*itertools.combinations(range(ndim), 2)]
+    latt_len = [np.linalg.norm(lattice[i]) for i in range(ndim)]
+    pproj = {
+        (i, j): np.dot(lattice[i], lattice[j]) / latt_len[i] / latt_len[j]
+        for i, j in idx_pairs
+    }
+    # get the spacing in each direction:
+    spacing = []
+    for idir in range(ndim):
+        idir_proj = [
+            np.array(lattice[j]) * pproj[tuple(sorted([idir, j]))]  # type: ignore
+            for j in range(ndim)
+            if j != idir
+        ]
+        v_perp_subspace = lattice[idir] - sum(idir_proj)
+        spacing.append(np.linalg.norm(v_perp_subspace))
+    return spacing
```

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.7.12
+Version: 2023.7.24
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/pyproject.toml` & `pymatgen-analysis-defects-2023.7.24/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,40 +11,40 @@
   "Programming Language :: Python :: 3.10",
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Science/Research",
   "Operating System :: OS Independent",
   "Topic :: Other/Nonlisted Topic",
   "Topic :: Scientific/Engineering",
 ]
-dependencies = ["pymatgen>=2023.5.8", "scikit-image>=0.19.3", "mp-pyrho>=0.3.0", "numpy<=1.23.5"]
+dependencies = [
+  "pymatgen>=2023.5.8",
+  "scikit-image>=0.19.3",
+  "numpy"
+]
 description = "Pymatgen extension for defects analysis"
 dynamic = ["version"]
 keywords = ["high-throughput", "automated", "dft", "defects"]
 license = { text = "modified BSD" }
 name = "pymatgen-analysis-defects"
 readme = "README.rst"
 requires-python = '>=3.8'
 
 [project.optional-dependencies]
-finder = ["dscribe>=1.2.1"]
+finder = ["dscribe>=2.0.0"]
 dev = ["pre-commit>=2.12.1"]
 docs = [
   "jupyter-book>=0.13.1",
 ]
 pydefect = ["pydefect>=0.6.2"]
 
 strict = [
-  "pymatgen>=2023.5.8",
-  "dscribe==1.2.2",
-  "scikit-image==0.20.0",
-  "pytest==7.2.2",
-  "pytest-cov==4.0.0",
-  "pre-commit==3.3.3",
-  "mp-pyrho==0.3.0",
-  "numpy==1.23.5"
+  "pymatgen==2023.7.20",
+  "dscribe==2.0.0",
+  "scikit-image==0.21.0",
+  "numpy==1.24.4",
 ]
 
 tests = ["pytest==7.2.2", "pytest-cov==4.0.0"]
 
 [tool.setuptools.dynamic]
 readme = { file = ["README.rst"] }
```

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_core.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_finder.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_generators.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.12/tests/test_utils.py` & `pymatgen-analysis-defects-2023.7.24/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pymatgen.analysis.defects.utils import (
     ChargeInsertionAnalyzer,
     TopographyAnalyzer,
     cluster_nodes,
     get_avg_chg,
     get_local_extrema,
     get_localized_states,
+    get_plane_spacing,
     group_docs,
 )
 
 
 def test_get_local_extrema(gan_struct):
     data = np.ones((48, 48, 48))
     chgcar = Chgcar(poscar=gan_struct, data={"total": data})
@@ -154,7 +155,12 @@
     g_names = []
     for name, group in sgroups:
         defect_names = ",".join([x.name for x in group])
         g_names.append(name)
         res.append(defect_names)
     assert "|".join(sorted(res)) == "N_i|N_i,N_i|v_Ga,v_Ga|v_N,v_N"
     assert "|".join(sorted(g_names)) == "N_i:0|N_i:1|v_Ga|v_N"
+
+
+def test_plane_spacing(gan_struct):
+    lattice = gan_struct.lattice.matrix
+    assert np.allclose(get_plane_spacing(lattice), [2.785, 2.785, 5.239], atol=0.001)
```

