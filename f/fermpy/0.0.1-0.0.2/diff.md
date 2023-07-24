# Comparing `tmp/fermpy-0.0.1.tar.gz` & `tmp/fermpy-0.0.2.tar.gz`

## Comparing `fermpy-0.0.1.tar` & `fermpy-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/__init__.py
--rw-r--r--   0        0        0    21065 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/bases.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/hamiltonian_constructors.py
--rw-r--r--   0        0        0    24941 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/operator_representation.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/operator_sum.py
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 fermpy-0.0.1/src/fermpy/operators.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fermpy-0.0.1/LICENSE
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 fermpy-0.0.1/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fermpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fermpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    55462 2020-02-02 00:00:00.000000 fermpy-0.0.2/example.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/__init__.py
+-rw-r--r--   0        0        0    21065 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/bases.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/example.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/hamiltonian_constructors.py
+-rw-r--r--   0        0        0    26279 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/operator_representation.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/operator_sum.py
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 fermpy-0.0.2/src/fermpy/operators.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fermpy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fermpy-0.0.2/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fermpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 fermpy-0.0.2/PKG-INFO
```

### Comparing `fermpy-0.0.1/src/fermpy/bases.py` & `fermpy-0.0.2/src/fermpy/bases.py`

 * *Files identical despite different names*

### Comparing `fermpy-0.0.1/src/fermpy/operator_representation.py` & `fermpy-0.0.2/src/fermpy/operator_representation.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import numpy as np
 import scipy.sparse as sp
 import warnings
 from numpy.typing import ArrayLike
 from numbers import Number
 
-from operator_sum import OpSum, Term
-from bases import Basis
+from .operator_sum import OpSum, Term
+from .bases import Basis
 
 
 OP_TERM_ID = tuple[str, tuple[int, ...]] # (*str_name*, *sites*)
 OPR_TERM_ID = tuple[str, int, int, str, tuple[int, ...]] # (*basis.id*, *qn*, *str_name*, *sites*)
 
 
 class OpRep:
@@ -71,30 +71,35 @@
     
     def _build_mat_rep_sparse(self) -> dict[int, sp.csc_array]:
         mat_rep: dict[int, sp.csc_array] = {}
         dtype = np.complex128 if self.opsum.has_complex_term else np.float64
         for qn in self.qns_to_consider:
             # All coefficients of all terms are scalars.
             if not self.opsum.parameter_shape:
-                mat_rep_qn = sp.csc_array(2 * (self.basis.dims[qn], ), dtype=dtype)
-                for i, factored_term in enumerate(self.opsum.factored_terms):
+                is_first_term = True
+                for i, factored_term in enumerate(self.opsum.factored_terms, 1):
                     print('factorized term: ', i, f'/ {len(self.opsum.factored_terms)}')
                     if factored_term[0].is_zero:
                         continue
-                    mat_rep_qn_fac = sp.csc_array(2 * (self.basis.dims[qn], ), dtype=dtype)
-                    for term in factored_term:
+                    mat_rep_qn_fac = self._get_mat_rep_of_operator_from_term_single_QN(factored_term[0], qn).copy()
+                    for term in factored_term[1:]:
                         mat_rep_qn_fac += self._get_mat_rep_of_operator_from_term_single_QN(term, qn)
-                    mat_rep_qn += term.coeff * mat_rep_qn_fac
+                    mat_rep_qn_fac *= factored_term[0].coeff
+                    if is_first_term: # += operator is a bit slow with empty sparse arrays
+                        mat_rep_qn = mat_rep_qn_fac
+                        is_first_term = False
+                    else:
+                        mat_rep_qn += mat_rep_qn_fac
             
             # Some coefficients are numpy arrays; do broadcasting.
             else:
                 # Wrap scipy sparse arrays in numpy arrays to take care of broadcasting.
                 mat_rep_qn = np.full(shape=self.opsum.parameter_shape,
-                                      fill_value=sp.csc_array(2 * (self.basis.dims[qn], ), dtype=dtype),
-                                      dtype=object)
+                                     fill_value=sp.csc_array(2 * (self.basis.dims[qn], ), dtype=dtype),
+                                     dtype=object)
                 for factored_term in self.opsum.factored_terms:
                     if factored_term[0].is_zero:
                         continue
                     mat_rep_qn_fac = sp.csc_array(2 * (self.basis.dims[qn], ), dtype=dtype)
                     for term in factored_term:
                         mat_rep_qn_fac += self._get_mat_rep_of_operator_from_term_single_QN(term, qn)
                     if term.shape:
@@ -172,15 +177,16 @@
             return sp.linalg.eigsh(self.mat_rep[qn],
                                    k=k,
                                    return_eigenvectors=return_eigenvectors,
                                    which=which,
                                    tol=tol,
                                    **kwargs)
         
-        return np.linalg.eigh(self.mat_rep[qn]) if return_eigenvectors else np.linalg.eigvalsh(self.mat_rep[qn])
+        return np.linalg.eigh(self.mat_rep[qn]) if return_eigenvectors\
+            else np.linalg.eigvalsh(self.mat_rep[qn])
     
     def diagonalize_all_qns(self,
                             k: int | dict[int, int] = 6,
                             return_eigenvectors: bool = False,
                             which: str | dict[int, str] = 'SA',
                             tol: float | dict[int, float] = 0,
                             **kwargs)\
@@ -202,21 +208,15 @@
                                                k=k,
                                                return_eigenvectors=False,
                                                which=which,
                                                tol=tol,
                                                **kwargs)
                 for qn in self.mat_rep}
     
-def _parse_and_set_arg(kwargs_qns: dict[int, dict[str, ...]], arg, kw: str):
-    if isinstance(arg, dict):
-        kwargs_qns[kw] = arg
-    else:
-        pass
-    
-def operator_exp_val(op_rep: np.ndarray | sp.spmatrix | dict[int, np.ndarray | sp.spmatrix],
+def operator_exp_val(op_rep: OpRep | np.ndarray | sp.spmatrix | dict[int, np.ndarray | sp.spmatrix],
                      state_rep: np.ndarray | dict[int, np.ndarray],
                      axis: int | None = None,
                      prepend_dim_op_rep: bool = False,
                      append_dim_op_rep: bool = False,
                      op_rep_is_sparse: bool | None = None,
                      dtype: np.dtype | None = None,
                      weights: None | Number | ArrayLike = None)\
@@ -250,14 +250,23 @@
     # Example: op_rep.shape=(N, N) and
     #          state_rep.shape=(m1, m2, ..., m_{j-1}, N, m_j) with axis=-2 is valid.
     #          out.shape=(m1, m2, ..., m_j)
     
     # Example: op_rep.shape=(m1, m2, ..., N, N) and
     #          state_rep.shape=(N, ) with axis=0 or axis=-1 or axis=None is valid.
     #          out.shape=(m1, m2, ...)
+    if isinstance(op_rep, OpRep):
+        return operator_exp_val(op_rep=op_rep.mat_rep,
+                                state_rep=state_rep,
+                                axis=axis,
+                                prepend_dim_op_rep=prepend_dim_op_rep,
+                                append_dim_op_rep=append_dim_op_rep,
+                                op_rep_is_sparse=op_rep_is_sparse,
+                                dtype=dtype,
+                                weights=weights)
     if isinstance(op_rep, dict) or isinstance(state_rep, dict):
         assert isinstance(op_rep, dict) and isinstance(state_rep, dict)
         common_keys = set(op_rep).intersection(state_rep)
         return {qn: operator_exp_val(op_rep[qn], state_rep[qn], axis, 
                                      prepend_dim_op_rep, append_dim_op_rep,
                                      op_rep_is_sparse, dtype, weights)
                 for qn in common_keys}
@@ -400,26 +409,39 @@
     str_exp = _get_index_str(op_rep_exp_val_brc, axis=axis_eig)
     str_w = str_exp
     str_out = str_exp.replace("n", "")
     return np.einsum(f"{str_w}, {str_exp} -> {str_out}",
                      weights_brc, op_rep_exp_val_brc)
 
 
-def thermal_avg_of_op(op_rep: dict[int, np.ndarray | sp.spmatrix],
+def thermal_avg_of_op(op_rep: OpRep | dict[int, np.ndarray | sp.spmatrix],
                       eig_rep: dict[int, np.ndarray],
                       energies: dict[int, np.ndarray],
                       temp: float | np.ndarray,
                       degeneracies: dict[int, int],
                       axis_mat: int,
                       axis_eig: int,
                       energy_zero: float | np.ndarray | None = None,
                       prepend_dim_op_rep: bool = False,
                       append_dim_op_rep: bool = False,
                       op_rep_is_sparse: bool | None = None,
                       dtype: np.dtype | None = None) -> float | complex | np.ndarray:
+    if isinstance(op_rep, OpRep):
+        return thermal_avg_of_op(op_rep=op_rep.mat_rep,
+                                 eig_rep=eig_rep,
+                                 energies=energies,
+                                 temp=temp,
+                                 degeneracies=degeneracies,
+                                 axis_mat=axis_mat,
+                                 axis_eig=axis_eig,
+                                 energy_zero=energy_zero,
+                                 prepend_dim_op_rep=prepend_dim_op_rep,
+                                 append_dim_op_rep=append_dim_op_rep,
+                                 op_rep_is_sparse=op_rep_is_sparse,
+                                 dtype=dtype)
     assert (isinstance(op_rep, dict) and
             isinstance(eig_rep, dict) and
             isinstance(energies, dict) and
             isinstance(degeneracies, dict)), (type(op_rep), type(eig_rep), type(energies), type(degeneracies))
     common_keys = set(op_rep).intersection(eig_rep, energies, degeneracies)
     
     if (len(common_keys) != len(op_rep) or
```

### Comparing `fermpy-0.0.1/src/fermpy/operator_sum.py` & `fermpy-0.0.2/src/fermpy/operator_sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 from numpy.typing import ArrayLike
 from typing import Callable
 from collections.abc import MutableSequence
 from numbers import Number
 
-from operators import NAME_TO_OP, HC_DICT
+from .operators import NAME_TO_OP, HC_DICT
 
 
 STATE = tuple[int, ...]
 SITE = int | tuple[int, ...]
 OP = Callable[[STATE, SITE], None | tuple[STATE, int | float]]
 OP_FIXED = Callable[[STATE], None | tuple[STATE, int | float]]
 HAM_PAR = Number | ArrayLike
```

### Comparing `fermpy-0.0.1/src/fermpy/operators.py` & `fermpy-0.0.2/src/fermpy/operators.py`

 * *Files identical despite different names*

### Comparing `fermpy-0.0.1/LICENSE` & `fermpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fermpy-0.0.1/pyproject.toml` & `fermpy-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fermpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Emil Frost", email="emiljpfrost@gmail.com" },
 ]
 description = "Package for exactly solving low-dimensional fermionic Hamiltonians"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,9 +18,12 @@
 ]
 keywords = ["physics", "condensed matter", "fermion", "Hamiltonian", "exact diagonalization", "sparse"]
 dependencies = [
   "numpy>=1.20",
   "scipy>=1.10.0"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "package.__version__"}
+
 [project.urls]
 "Homepage" = "https://github.com/emilfrost/fermpy"
```

