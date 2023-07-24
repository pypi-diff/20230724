# Comparing `tmp/lmo-0.7.0.tar.gz` & `tmp/lmo-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.7.0.tar", max compression
+gzip compressed data, was "lmo-0.8.0.tar", max compression
```

## Comparing `lmo-0.7.0.tar` & `lmo-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.7.0/LICENSE
--rw-r--r--   0        0        0     3865 2023-07-16 04:39:16.565156 lmo-0.7.0/README.md
--rw-r--r--   0        0        0      752 2023-07-16 21:07:04.201216 lmo-0.7.0/lmo/__init__.py
--rw-r--r--   0        0        0    21555 2023-07-17 20:38:35.304271 lmo-0.7.0/lmo/_lm.py
--rw-r--r--   0        0        0    11915 2023-07-16 20:56:43.798563 lmo-0.7.0/lmo/_lm_co.py
--rw-r--r--   0        0        0      160 2023-07-16 20:51:40.539410 lmo-0.7.0/lmo/_meta.py
--rw-r--r--   0        0        0     5093 2023-07-16 20:51:26.919089 lmo-0.7.0/lmo/_pwm.py
--rw-r--r--   0        0        0     4841 2023-07-16 20:46:14.547721 lmo-0.7.0/lmo/_utils.py
--rw-r--r--   0        0        0     2278 2023-07-16 20:43:58.184505 lmo-0.7.0/lmo/diagnostic.py
--rw-r--r--   0        0        0    10940 2023-07-16 20:42:19.250171 lmo-0.7.0/lmo/linalg.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.7.0/lmo/py.typed
--rw-r--r--   0        0        0    10513 2023-07-16 20:22:06.045490 lmo-0.7.0/lmo/theoretical.py
--rw-r--r--   0        0        0     1682 2023-07-16 19:21:00.902603 lmo-0.7.0/lmo/typing.py
--rw-r--r--   0        0        0     3825 2023-07-17 21:24:40.836795 lmo-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 lmo-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3865 2023-07-16 04:39:16.565156 lmo-0.8.0/README.md
+-rw-r--r--   0        0        0      846 2023-07-23 21:29:19.935256 lmo-0.8.0/lmo/__init__.py
+-rw-r--r--   0        0        0    30179 2023-07-24 01:54:40.094431 lmo-0.8.0/lmo/_lm.py
+-rw-r--r--   0        0        0    12599 2023-07-23 20:30:37.618885 lmo-0.8.0/lmo/_lm_co.py
+-rw-r--r--   0        0        0      160 2023-07-16 20:51:40.539410 lmo-0.8.0/lmo/_meta.py
+-rw-r--r--   0        0        0     5515 2023-07-23 21:31:59.599266 lmo-0.8.0/lmo/_utils.py
+-rw-r--r--   0        0        0     2249 2023-07-23 17:52:22.126379 lmo-0.8.0/lmo/diagnostic.py
+-rw-r--r--   0        0        0    13577 2023-07-24 02:05:07.788837 lmo-0.8.0/lmo/linalg.py
+-rw-r--r--   0        0        0     3425 2023-07-24 01:48:14.041262 lmo-0.8.0/lmo/ostats.py
+-rw-r--r--   0        0        0     5125 2023-07-23 17:06:07.374009 lmo-0.8.0/lmo/pwm_beta.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.8.0/lmo/py.typed
+-rw-r--r--   0        0        0    15588 2023-07-23 22:10:00.392413 lmo-0.8.0/lmo/theoretical.py
+-rw-r--r--   0        0        0     2185 2023-07-23 18:57:56.454838 lmo-0.8.0/lmo/typing.py
+-rw-r--r--   0        0        0     3825 2023-07-24 01:58:24.855716 lmo-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 lmo-0.8.0/PKG-INFO
```

### Comparing `lmo-0.7.0/LICENSE` & `lmo-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.7.0/README.md` & `lmo-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.7.0/lmo/__init__.py` & `lmo-0.8.0/lmo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,25 @@
     '__version__',
 
     'l_weights',
     'l_moment',
     'l_moment_cov',
     'l_ratio',
     'l_ratio_se',
+    'l_stats',
+    'l_stats_se',
     'l_loc',
     'l_scale',
     'l_variation',
     'l_skew',
     'l_kurtosis',
 
     'l_comoment',
     'l_coratio',
+    'l_costats',
     'l_coloc',
     'l_coscale',
     'l_corr',
     'l_coskew',
     'l_cokurtosis',
 )
 
@@ -29,22 +32,25 @@
     l_loc,
     l_moment,
     l_moment_cov,
     l_ratio,
     l_ratio_se,
     l_scale,
     l_skew,
+    l_stats,
+    l_stats_se,
     l_variation,
     l_weights,
 )
 from ._lm_co import (
     l_cokurtosis,
     l_coloc,
     l_comoment,
     l_coratio,
     l_corr,
     l_coscale,
     l_coskew,
+    l_costats,
 )
 from ._meta import get_version as _get_version
 
 __version__: _Final[str] = _get_version()
```

### Comparing `lmo-0.7.0/lmo/_lm.py` & `lmo-0.8.0/lmo/_lm.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,44 +2,54 @@
 
 __all__ = (
     'l_weights',
     'l_moment',
     'l_moment_cov',
     'l_ratio',
     'l_ratio_se',
+    'l_stats',
+    'l_stats_se',
     'l_loc',
     'l_scale',
     'l_variation',
     'l_skew',
     'l_kurtosis',
 )
 
-from typing import Any, Final, TypeVar, cast
+import sys
+from typing import Any, Final, TypeVar, cast, overload
 
 import numpy as np
 import numpy.typing as npt
 
-from ._pwm import b_moment_cov, b_weights
-from ._utils import clean_order, ensure_axis_at, ordered
-from .linalg import sandwich, sh_legendre, trim_matrix
-from .typing import AnyInt, IntVector, SortKind
+from . import ostats
+from ._utils import clean_order, ensure_axis_at, moments_to_ratio, ordered
+from .linalg import ir_pascal, sandwich, sh_legendre, trim_matrix
+from .pwm_beta import cov, weights
+from .typing import AnyInt, IntVector, LMomentOptions, SortKind
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Unpack
+else:
+    from typing import Unpack
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 # Low-level weight methods
 
 _L_WEIGHTS_CACHE: Final[
     dict[
-        tuple[int, int, int],  # (n, t_1, t_2)
+        tuple[int, int | float, int | float],  # (n, t_1, t_2)
         npt.NDArray[np.floating[Any]],
     ]
 ] = {}
 
-def _l0_weights(
+
+def _l0_weights_pwm(
     r: int,
     n: int,
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
 ) -> npt.NDArray[T]:
     r"""
     Efficiently calculates the projection matrix $P = [p_{k, i}]_{r \times n}$
@@ -58,37 +68,98 @@
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
     """
     p_r = np.empty((r, n), dtype)
 
     if r > 0:
-        np.matmul(sh_legendre(r), b_weights(r, n, dtype), out=p_r)
+        np.matmul(sh_legendre(r), weights(r, n, dtype), out=p_r)
 
     return p_r
 
 
-def l_weights(
+def _l_weights_pwm(
     r: int,
     n: int,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[int, int],
     dtype: np.dtype[T] | type[T] = np.float_,
+) -> npt.NDArray[T]:
+    if sum(trim) == 0:
+        return _l0_weights_pwm(r, n, dtype)
+
+    p_r = np.empty((r, n), dtype)
+
+    if r == 0:
+        return p_r
+
+    # the k-th TL-(t_1, t_2) weights are a linear combination of L-weights
+    # with orders k, ..., k + t_1 + t_2
+
+    np.matmul(
+        trim_matrix(r, trim),
+        _l0_weights_pwm(r + sum(trim), n),
+        out=p_r,
+    )
+
+    # remove numerical noise from the trimmings, and correct for potential
+    # shifts in means
+    t1, t2 = trim
+    p_r[:, :t1] = p_r[:, n - t2:] = 0
+    p_r[1:, t1:n - t2] -= p_r[1:, t1:n - t2].mean(1, keepdims=True)
+
+    return p_r
+
+
+def _l_weights_ostat(
+    r: int,
+    N: int,  # noqa: N803
+    /,
+    trim: tuple[float, float],
+    dtype: np.dtype[T] | type[T] = np.float_,
+) -> npt.NDArray[T]:
+    s, t = trim
+
+    assert 0 < r + s + t <= N, (r, N, trim)
+    assert r >= 1, r
+    assert s >= 0 and t >= 0, trim
+
+    c = ir_pascal(r)
+    jnj = np.arange(N, dtype=dtype)
+    jnj /= (N - jnj)
+
+    out = np.zeros((r, N), dtype=dtype)
+    for n in range(r):
+        w0 = ostats.weights(s, s + t + n + 1, N)
+        out[n] = c[n, 0] * w0
+        for k in range(1, n + 1):
+            # order statistic recurrence relation
+            w0 = np.roll(w0, 1) * jnj * ((t + n - k + 1) / (s + k))
+            out[n] += c[n, k] * w0
+    return out
+
+
+def l_weights(
+    r: int,
+    n: int,
+    /,
+    trim: tuple[float, float] = (0, 0),
     *,
     cache: bool = False,
-) -> npt.NDArray[T]:
+) -> npt.NDArray[np.float_]:
     r"""
     Projection matrix of the first $r$ (T)L-moments for $n$ samples.
 
-    The matrix is a linear combination of the Power Weighted Moment
-    (PWM) weight matrix (the sample estimator of $beta_{r_1}$), and the
-    shifted Legendre polynomials.
-
-    If `trim != (0, 1)`, a linearized (and corrected) adaptation of the
-    recurrence relations from *Hosking (2007)* are applied, as well.
+    For integer trim is the matrix is a linear combination of the Power
+    Weighted Moment (PWM) weights (the sample estimator of $beta_{r_1}$), and
+    the shifted Legendre polynomials.
+
+    If the trimmings are nonzero and integers, a linearized (and corrected)
+    adaptation of the recurrence relations from *Hosking (2007)* are applied,
+    as well.
 
     $$
     (2k + t_1 + t_2 - 1) \lambda^{(t_1, t_2)}_k
         = (k + t_1 + t_2) \lambda^{(t_1 - 1, t_2)}_k
         + \frac{1}{k} (k + 1) (k + t_2) \lambda^{(t_1 - 1, t_2)}_{k+1}
     $$
 
@@ -98,14 +169,19 @@
     (2k + t_1 + t_2 - 1) \lambda^{(t_1, t_2)}_k
         = (k + t_1 + t_2) \lambda^{(t_1, t_2 - 1)}_k
         - \frac{1}{k} (k + 1) (k + t_1) \lambda^{(t_1, t_2 - 1)}_{k+1}
     $$
 
     for $t_2 > 0$.
 
+    If the trim values are floats instead, the weights are calculated directly
+    from the (generalized) order statistics. At the time of writing (07-2023),
+    these "generalized trimmed L-moments" have not been discussed in the
+    literature or the R-packages. It's probably a good idea to publish this...
+
     TLDR:
         This matrix (linearly) transforms $x_{i:n}$ (i.e. the sorted
         observation vector(s) of size $n$), into (an unbiased estimate of) the
         *generalized trimmed L-moments*, with orders $\le r$.
 
     Returns:
         P_r: 2-D array of shape `(r, n)`.
@@ -119,71 +195,171 @@
         >>> _ @ [-1, 0, 1 / 2, 3 / 2]
         array([0.25      , 0.66666667, 0.        ])
 
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
     """
+    if r == 0:
+        return np.empty((r, n))
+
+    match trim:
+        case s, t if s < 0 or t < 0:
+            msg = f'trim orders must be >=0, got {trim}'
+            raise ValueError(msg)
+        case s, t:
+            pass
+        case _:  # type: ignore [reportUneccessaryComparison]
+            msg = (
+                f'trim must be a tuple with two non-negative ints or floats, '
+                f'got {trim!r}'
+            )
+            raise TypeError(msg)
+
+    # manual cache lookup, only if cache=False (for testability)
+    # e.g. `functools.cache` would be inefficient for e.g. r=3 with cached r=4
     cache_key = n, *trim
     if (
-        cache_key in _L_WEIGHTS_CACHE
-        and (p_r := _L_WEIGHTS_CACHE[cache_key]).shape[0] <= r
+        cache
+        and cache_key in _L_WEIGHTS_CACHE
+        and (w := _L_WEIGHTS_CACHE[cache_key]).shape[0] <= r
     ):
-        if p_r.dtype is not np.dtype(dtype):
-            p_r = p_r.view(dtype)
-        if p_r.shape[0] < r:
-            p_r = p_r[:r]
+        if w.shape[0] < r:
+            w = w[:r]
 
         # ignore if r is larger that what's cached
-        if p_r.shape[0] == r:
-            assert p_r.shape == (r, n)
-            return cast(npt.NDArray[T], p_r)
+        if w.shape[0] == r:
+            assert w.shape == (r, n)
+            return w
+
+    if isinstance(s, int | np.integer) and isinstance(t, int | np.integer):
+        w = _l_weights_pwm(r, n, trim=(int(s), int(t)))
+    else:
+        w = _l_weights_ostat(r, n, trim=(float(s), float(t)))
 
+    if cache:
+        # memoize
+        _L_WEIGHTS_CACHE[cache_key] = w
 
-    if sum(trim) == 0:
-        return _l0_weights(r, n, dtype)
+    return w
 
-    p_r = np.empty((r, n), dtype)
 
-    if r == 0:
-        return p_r
 
-    # the k-th TL-(t_1, t_2) weights are a linear combination of L-weights
-    # with orders k, ..., k + t_1 + t_2
+# Summary statistics
 
-    np.matmul(
-        trim_matrix(r, trim),
-        _l0_weights(r + sum(trim), n),
-        out=p_r,
-    )
 
-    # remove numerical noise from the trimmings, and correct for potential
-    # shifts in means
-    t1, t2 = trim
-    p_r[:, :t1] = p_r[:, n - t2:] = 0
-    p_r[1:, t1:n - t2] -= p_r[1:, t1:n - t2].mean(1, keepdims=True)
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: None = ...,
+    dtype: type[np.float_] = ...,
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> np.float_:
+    ...
 
-    if cache:
-        # memoize, and mark as readonly to avoid corruping the cache
-        p_r.setflags(write=False)
-        _L_WEIGHTS_CACHE[cache_key] = p_r
 
-    return p_r
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: None = ...,
+    dtype: np.dtype[T] | type[T],
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> T:
+    ...
 
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int,
+    dtype: type[np.float_] = ...,
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> np.float_ | npt.NDArray[np.float_]:
+    ...
+
+
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int,
+    dtype: np.dtype[T] | type[T],
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> T | npt.NDArray[T]:
+    ...
+
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: type[np.float_],
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> npt.NDArray[np.float_]:
+    ...
+
+
+@overload
+def l_moment(
+    a: npt.ArrayLike,
+    r: IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: np.dtype[T] | type[T],
+    fweights: IntVector | None = ...,
+    aweights: npt.ArrayLike | None = ...,
+    sort: SortKind | None = ...,
+    cache: bool = ...,
+) -> npt.NDArray[T]:
+    ...
 
-# Summary statistics
 
 def l_moment(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    *,
+
     fweights: IntVector | None = None,
     aweights: npt.ArrayLike | None = None,
     sort: SortKind | None = 'stable',
     cache: bool = False,
 ) -> T | npt.NDArray[T]:
     r"""
     Estimates the generalized trimmed L-moment $\lambda^{(t_1, t_2)}_r$ from
@@ -195,34 +371,32 @@
             Array containing numbers whose L-moments is desired.
             If `a` is not an array, a conversion is attempted.
 
         r:
             The L-moment order(s), non-negative integer or array.
 
         trim:
-            Left- and right-trim orders $(t_1, t_2)$, non-negative integers
-            that are bound by $t_1 + t_2 < n - r$.
+            Left- and right-trim orders $(t_1, t_2)$, non-negative ints or
+            floats that are bound by $t_1 + t_2 < n - r$.
 
             Some special cases include:
 
-            - $(0, 0)$: The original **L**-moment, introduced by Hosking (1990).
-                Useful for fitting the e.g. log-normal and generalized extreme
-                value (GEV) distributions.
+            - $(0, 0)$: The original **L**-moment, introduced by Hosking
+                in 1990.
             - $(0, m)$: **LL**-moment (**L**inear combination of **L**owest
-                order statistics), instroduced by Bayazit & Onoz (2002).
+                order statistics), instroduced by Bayazit & Onoz in 2002.
                 Assigns more weight to smaller observations.
             - $(s, 0)$: **LH**-moment (**L**inear combination of **H**igher
-                order statistics), by Wang (1997).
+                order statistics), as described by Wang in 1997.
                 Assigns more weight to larger observations.
             - $(t, t)$: **TL**-moment (**T**rimmed L-moment) $\\lambda_r^t$,
-                with symmetric trimming. First introduced by
-                Elamir & Seheult (2003).
-                Generally more robust than L-moments.
-                Useful for fitting heavy-tailed distributions, such as the
-                Cauchy distribution.
+                with symmetric trimming. First introduced by Elamir & Seheult
+                in 2003, and refined by Hosking in 2007. Generally more robust
+                than L-moments. Useful for fitting pathological distributions,
+                such as the Cauchy distribution.
 
         axis:
             Axis along wich to calculate the moments. If `None` (default),
             all samples in the array will be used.
 
         dtype:
             Floating type to use in computing the L-moments. Default is
@@ -257,20 +431,28 @@
         l:
             The L-moment(s) of the input This is a scalar iff a is 1-d and
             r is a scalar. Otherwise, this is an array with
             `np.ndim(r) + np.ndim(a) - 1` dimensions and shape like
             `(*np.shape(r), *(d for d in np.shape(a) if d != axis))`.
 
     Examples:
+        Calculate the L-location and L-scale from student-T(2) samples, for
+        different (symmetric) trim-lengths.
+
         >>> import lmo, numpy as np
-        >>> x = np.random.default_rng(12345).standard_normal(20)
-        >>> lmo.l_moment(x, [1, 2, 3, 4])
-        array([0.00106117, 0.65354263, 0.01436636, 0.04280225])
-        >>> lmo.l_moment(x, [1, 2, 3, 4], trim=(1, 1))
-        array([-0.0133052 ,  0.36644423, -0.00823471, -0.01034343])
+        >>> x = np.random.default_rng(12345).standard_t(2, 99)
+        >>> lmo.l_moment(x, [1, 2], trim=(0, 0))
+        array([-0.01412282,  0.94063132])
+        >>> lmo.l_moment(x, [1, 2], trim=(1/2, 1/2))
+        array([-0.02158858,  0.57977201])
+        >>> lmo.l_moment(x, [1, 2], trim=(1, 1))
+        array([-0.0124483 ,  0.40120115])
+
+        The theoretical L-locations are all 0, and the the L-scale are
+        `1.1107`, `0.6002` and `0.4165`, respectively.
 
     See Also:
         - [L-moment - Wikipedia](https://wikipedia.org/wiki/L-moment)
         - [`scipy.stats.moment`][scipy.stats.moment]
 
     References:
         - [J.R.M. Hosking (1990)](https://jstor.org/stable/2345653)
@@ -286,37 +468,36 @@
         fweights=fweights,
         aweights=aweights,
         sort=sort,
     )
     x_k = ensure_axis_at(x_k, axis, -1)
     n = x_k.shape[-1]
 
-    r_max = clean_order(np.max(np.asarray(r)))
+    _r = np.asarray(r)
+    r_max = clean_order(np.max(_r))
 
-    l_r = np.inner(l_weights(r_max, n, trim, dtype=dtype, cache=cache), x_k)
+    l_r = np.inner(l_weights(r_max, n, trim, cache=cache), x_k)
 
     # we like 0-based indexing; so if P_r starts at r=1, prepend all 1's
     # for r=0 (any zeroth moment is defined to be 1)
     l_r = np.r_[np.ones((1, *l_r.shape[1:]), dtype=l_r.dtype), l_r]
 
-    assert np.all(l_r[0] == 1)
-    assert len(l_r) == r_max + 1, (l_r.shape, r_max)
-
     # l[r] fails when r is e.g. a tuple (valid sequence).
-    return l_r.take(r, 0)
+    return cast(T | npt.NDArray[T], l_r.take(_r, 0))
 
 
 def l_moment_cov(
     a: npt.ArrayLike,
     r_max: AnyInt,
     /,
     trim: tuple[int, int] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> npt.NDArray[T]:
     """
     Non-parmateric auto-covariance matrix of the generalized trimmed
     L-moment point estimates with orders `r = 1, ..., r_max`.
 
     Returns:
         S_l: Variance-covariance matrix/tensor of shape `(r_max, r_max, ...)`
@@ -350,42 +531,164 @@
     References:
         - [E. Elamir & A. Seheult (2003) - Trimmed L-moments](
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [E. Elamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 
     """
+    if any(int(t) != t for t in trim):
+        msg = 'l_moment_cov does not support fractional trimming (yet)'
+        raise TypeError(msg)
+
     ks = int(r_max + sum(trim))
     if ks < r_max:
         msg = 'trimmings must be positive'
         raise ValueError(msg)
 
 
     # projection matrix: PWMs -> generalized trimmed L-moments
     p_l: npt.NDArray[np.floating[Any]]
     p_l = trim_matrix(int(r_max), trim=trim, dtype=dtype) @ sh_legendre(ks)
     # clean some numerical noise
     p_l = np.round(p_l, 12) + 0.
 
     # PWM covariance matrix
-    s_b = b_moment_cov(a, ks, axis=axis, dtype=dtype, **kwargs)
+    s_b = cov(a, ks, axis=axis, dtype=dtype, **kwargs)
 
     # tasty, eh?
     return sandwich(p_l, s_b, dtype=dtype)
 
 
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    s: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: None = ...,
+    dtype: type[np.float_] = ...,
+    **kwargs: Unpack[LMomentOptions],
+) -> np.float_:
+    ...
+
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    s: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: None = ...,
+    dtype: np.dtype[T] | type[T],
+    **kwargs: Unpack[LMomentOptions],
+) -> T:
+    ...
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    s: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int,
+    dtype: type[np.float_] = ...,
+    **kwargs: Unpack[LMomentOptions],
+) -> np.float_ | npt.NDArray[np.float_]:
+    ...
+
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt,
+    s: AnyInt,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int,
+    dtype: np.dtype[T] | type[T],
+    **kwargs: Unpack[LMomentOptions],
+) -> T | npt.NDArray[T]:
+    ...
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: IntVector,
+    s: AnyInt | IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: type[np.float_] = ...,
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[np.float_]:
+    ...
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: IntVector,
+    s: AnyInt | IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: np.dtype[T] | type[T],
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[T]:
+    ...
+
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt | IntVector,
+    s: IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: type[np.float_] = ...,
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[np.float_]:
+    ...
+
+
+@overload
+def l_ratio(
+    a: npt.ArrayLike,
+    r: AnyInt | IntVector,
+    s: IntVector,
+    /,
+    trim: tuple[float, float] = ...,
+    *,
+    axis: int | None = ...,
+    dtype: np.dtype[T] | type[T],
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[T]:
+    ...
+
+
 def l_ratio(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     s: AnyInt | IntVector,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     Estimates the generalized L-moment ratio:
 
     $$
     \tau^{(t_1, t_2)}_{rs} = \frac{
         \lambda^{(t_1, t_2)}_r
@@ -410,46 +713,30 @@
         array([1.53196368, 0.77549561, 0.4463163 , 0.29752178])
         >>> lmo.l_ratio(x, [1, 2, 3, 4], [0, 0, 2, 2], trim=(0, 1))
         array([0.75646807, 0.32203446, 0.23887609, 0.07917904])
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
     """  # noqa: D415
-    _r, _s = np.asarray(r), np.asarray(s)
-    rs = np.stack(np.broadcast_arrays(_r, _s))
-
-    l_rs = cast(
-        npt.NDArray[T],
-        l_moment(a, rs, trim, axis=axis, dtype=dtype, **kwargs),
-    )
-
-    r_eq_s = _r == _s
-    if r_eq_s.ndim < l_rs.ndim - 1:
-        r_eq_s = r_eq_s.reshape(
-            r_eq_s.shape + (1,) * (l_rs.ndim - r_eq_s.ndim - 1),
-        )
-
-    with np.errstate(divide='ignore'):
-        return np.where(
-            r_eq_s,
-            np.ones_like(l_rs[0]),
-            np.divide(l_rs[0], l_rs[1], where=~r_eq_s),
-        )[()]
+    rs = np.stack(np.broadcast_arrays(np.asarray(r), np.asarray(s)))
+    l_rs = l_moment(a, rs, trim, axis=axis, dtype=dtype, **kwargs)
 
+    return moments_to_ratio(rs, l_rs)
 
 
 def l_ratio_se(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     s: AnyInt | IntVector,
     /,
     trim: tuple[int, int] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> npt.NDArray[T]:
     """
     Non-parametric estimates of the Standard Error (SE) in the L-ratio
     estimates from [`lmo.l_ratio`][lmo.l_ratio].
 
     Examples:
         Estimate the values and errors of the TL-loc, scale, skew and kurtosis
@@ -478,19 +765,19 @@
 
     """
     _r, _s = np.broadcast_arrays(np.asarray(r), np.asarray(s))
     _rs = np.stack((_r, _s))
     r_max: AnyInt = np.amax(np.r_[_r, _s].ravel())
 
     # L-moments
-    l_rs = cast(npt.NDArray[T], l_moment(a, _rs, trim, axis, dtype, **kwargs))
+    l_rs = l_moment(a, _rs, trim, axis=axis, dtype=dtype, **kwargs)
     l_r, l_s = l_rs[0], l_rs[1]
 
     # L-moment auto-covariance matrix
-    k_l = l_moment_cov(a, r_max, trim, axis, dtype, **kwargs)
+    k_l = l_moment_cov(a, r_max, trim, axis=axis, dtype=dtype, **kwargs)
     # prepend the "zeroth" moment, with has 0 (co)variance
     k_l = np.pad(k_l, (1, 0), constant_values=0)
 
     s_rr = k_l[_r, _r]  # Var[l_r]
     s_ss = k_l[_s, _s]  # Var[l_r]
     s_rs = k_l[_r, _s]  # Cov[l_r, l_s]
 
@@ -505,56 +792,127 @@
         _s_tt = np.where(_s == 0, s_rr, _s_tt)
         # Var[l_r / l_0] == Var[l_r / 1] == Var[l_r]
         s_tt = np.where(_r == _s, 0, _s_tt)
 
     return np.sqrt(s_tt)
 
 
-def l_loc(
+def l_stats(
+    a: npt.ArrayLike,
+    /,
+    trim: tuple[float, float] = (0, 0),
+    *,
+    axis: int | None = None,
+    dtype: np.dtype[T] | type[T] = np.float_,
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[T]:
+    """
+    Calculates the L-loc(ation), L-scale, L-skew(ness) and L-kurtosis.
+
+    Equivalent to `lmo.l_ratio(a, [1, 2, 3, 4], [0, 0, 2, 2], *, **)`.
+
+    Examples:
+        >>> import lmo, scipy.stats
+        >>> x = scipy.stats.gumbel_r.rvs(size=99, random_state=12345)
+        >>> lmo.l_stats(x)
+        array([0.79014773, 0.68346357, 0.12207413, 0.12829047])
+
+        The theoretical L-stats of the standard Gumbel distribution are
+        `[0.577, 0.693, 0.170, 0.150]`.
+
+    See Also:
+        - [`lmo.l_stats_se`][lmo.l_stats_se]
+        - [`lmo.l_ratio`][lmo.l_ratio]
+        - [`lmo.l_costats`][lmo.l_costats]
+    """
+    r, s = [1, 2, 3, 4], [0, 0, 2, 2]
+    return l_ratio(a, r, s, trim=trim, axis=axis, dtype=dtype, **kwargs)
+
+
+def l_stats_se(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
+    *,
+    axis: int | None = None,
+    dtype: np.dtype[T] | type[T] = np.float_,
+    **kwargs: Unpack[LMomentOptions],
+) -> npt.NDArray[T]:
+    """
+    Calculates the standard errors (SE's) of the [`L-stats`][lmo.l_stats].
+
+    Equivalent to `lmo.l_ratio_se(a, [1, 2, 3, 4], [0, 0, 2, 2], *, **)`.
+
+    Examples:
+        >>> import lmo, scipy.stats
+        >>> x = scipy.stats.gumbel_r.rvs(size=99, random_state=12345)
+        >>> lmo.l_stats(x)
+        array([0.79014773, 0.68346357, 0.12207413, 0.12829047])
+        >>> lmo.l_stats_se(x)
+        array([0.12305147, 0.05348839, 0.04472984, 0.03408495])
+
+        The theoretical L-stats of the standard Gumbel distribution are
+        `[0.577, 0.693, 0.170, 0.150]`. The corresponding relative z-scores
+        are `[-1.730, 0.181, 1.070, 0.648]`.
+
+    See Also:
+        - [`lmo.l_stats`][lmo.l_stats]
+        - [`lmo.l_ratio_se`][lmo.l_ratio_se]
+    """
+    r, s = [1, 2, 3, 4], [0, 0, 2, 2]
+    return l_ratio_se(a, r, s, trim=trim, axis=axis, dtype=dtype, **kwargs)
+
+
+def l_loc(
+    a: npt.ArrayLike,
+    /,
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     *L-location* (or *L-loc*): unbiased estimator of the first L-moment,
     $\lambda^{(t_1, t_2)}_1$.
 
     Alias for [`lmo.l_moment(a, 1, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.mean()
         -7.56485034...
-        >>> lmo.l_loc(x)
+        >>> lmo.l_loc(x)  # no trim; equivalent to the (arithmetic) mean
         -7.56485034...
-        >>> lmo.l_loc(x, trim=(1, 1))
+        >>> lmo.l_loc(x, trim=(1, 1))  # TL-location
         -0.15924180...
+        >>> lmo.l_loc(x, trim=(3/2, 3/2))  # Fractional trimming (only in Lmo)
+        -0.08845121...
+
 
     Notes:
         If `trim = (0, 0)` (default), the L-location is equivalent to the
         [arithmetic mean](https://wikipedia.org/wiki/Arithmetic_mean).
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
         - [`numpy.average`][numpy.average]
     """
-    return l_moment(a, 1, trim, axis, dtype, **kwargs)
+    return l_moment(a, 1, trim, axis=axis, dtype=dtype, **kwargs)
 
 
 def l_scale(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     *L-scale*: unbiased estimator of the second L-moment,
     $\lambda^{(t_1, t_2)}_2$.
 
     Alias for [`lmo.l_moment(a, 2, *, **)`][lmo.l_moment].
 
@@ -573,24 +931,25 @@
         [Gini mean difference (GMD)](
         https://wikipedia.org/wiki/Gini_mean_difference).
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
         - [`numpy.std`][numpy.std]
     """
-    return l_moment(a, 2, trim, axis, dtype, **kwargs)
+    return l_moment(a, 2, trim, axis=axis, dtype=dtype, **kwargs)
 
 
 def l_variation(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     The *coefficient of L-variation* (or *L-CV*) unbiased sample estimator:
 
     $$
     \tau^{(t_1, t_2)} = \frac{
         \lambda^{(t_1, t_2)}_2
@@ -618,24 +977,25 @@
 
     See Also:
         - [Gini coefficient - Wikipedia](
             https://wikipedia.org/wiki/Gini_coefficient)
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.variation.l_ratio`][scipy.stats.variation]
     """  # noqa: D415
-    return l_ratio(a, 2, 1, trim, axis, dtype, **kwargs)
+    return l_ratio(a, 2, 1, trim, axis=axis, dtype=dtype, **kwargs)
 
 
 def l_skew(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     Unbiased sample estimator of the *coefficient of L-skewness*, or *L-skew*
     for short:
 
     $$
     \tau^{(t_1, t_2)}_3
@@ -656,24 +1016,25 @@
         >>> lmo.l_skew(x, trim=(0, 1))
         0.27116139...
 
     See Also:
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.skew`][scipy.stats.skew]
     """  # noqa: D415
-    return l_ratio(a, 3, 2, trim, axis, dtype, **kwargs)
+    return l_ratio(a, 3, 2, trim, axis=axis, dtype=dtype, **kwargs)
 
 
 def l_kurtosis(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
+    trim: tuple[float, float] = (0, 0),
+    *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LMomentOptions],
 ) -> T | npt.NDArray[T]:
     r"""
     L-kurtosis coefficient; the 4th sample L-moment ratio.
 
     $$
     \tau^{(t_1, t_2)}_4
         = \frac{
@@ -698,8 +1059,8 @@
         $[-\frac{1}{4}, 1)$, and by the L-skewness $\\tau_3$ as
         $5 \tau_3^2 - 1 \le 4 \tau_4$.
 
     See Also:
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.kurtosis`][scipy.stats.kurtosis]
     """
-    return l_ratio(a, 4, 2, trim, axis, dtype, **kwargs)
+    return l_ratio(a, 4, 2, trim, axis=axis, dtype=dtype, **kwargs)
```

### Comparing `lmo-0.7.0/lmo/_lm_co.py` & `lmo-0.8.0/lmo/_lm_co.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 __all__ = (
     'l_comoment',
     'l_coratio',
+    'l_costats',
     'l_coloc',
     'l_coscale',
     'l_corr',
     'l_coskew',
     'l_cokurtosis',
 )
 
+import sys
 from typing import Any, TypeVar, cast
 
 import numpy as np
 from numpy import typing as npt
 
 from ._lm import l_weights
 from ._utils import clean_order, ordered
-from .typing import AnyInt, IntVector, SortKind
+from .typing import AnyInt, IntVector, LComomentOptions, SortKind
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Unpack
+else:
+    from typing import Unpack
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def l_comoment(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
-    dtype: np.dtype[T] | type[T] = np.float_,
+    trim: tuple[float, float] = (0, 0),
     *,
+    dtype: np.dtype[T] | type[T] = np.float_,
+    rowvar: bool = True,
     sort: SortKind | None = 'stable',
     cache: bool = False,
 ) -> npt.NDArray[T]:
     r"""
     Multivariate extension of [`lmo.l_moment`][lmo.l_moment].
 
     Estimates the L-comoment matrix:
@@ -65,16 +72,16 @@
             observation of all those variables. Also see `rowvar` below.
             If `a` is not an array, a conversion is attempted.
 
         r:
             The L-moment order(s), non-negative integer or array.
 
         trim:
-            Left- and right-trim orders $(t_1, t_2)$, non-negative integers
-            that are bound by $t_1 + t_2 < n - r$.
+            Left- and right-trim orders $(t_1, t_2)$, non-negative ints or
+            floats that are bound by $t_1 + t_2 < n - r$.
 
             Some special cases include:
 
             - $(0, 0)$: The original **L**-moment, introduced by Hosking (1990).
                 Useful for fitting the e.g. log-normal and generalized extreme
                 value (GEV) distributions.
             - $(0, m)$: **LL**-moment (**L**inear combination of **L**owest
@@ -144,15 +151,15 @@
     r_max = clean_order(cast(int, np.max(_r)))
     m, n = x.shape
 
     if not m:
         return np.empty((*np.shape(_r), 0, 0), dtype=dtype)
 
     # projection matrix of shape (r, n)
-    p_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
+    p_r = l_weights(r_max, n, trim, cache=cache)
 
     # L-comoment matrices for r = 0, ..., r_max
     l_ij = np.empty((r_max + 1, m, m), dtype=dtype)
 
     # the zeroth L-comoment is the delta function, so the L-comoment
     # matrix is the identity matrix
     l_ij[0] = np.eye(m, dtype=dtype)
@@ -167,18 +174,18 @@
 
 
 def l_coratio(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     s: AnyInt | IntVector,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     Estimate the generalized matrix of L-comoment ratio's.
 
     $$
     \tilde \Lambda_{rs}^{(t_1, t_2)} =
         \left[
@@ -188,28 +195,50 @@
     $$
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_ratio`][lmo.l_ratio]
     """
     rs = np.stack(np.broadcast_arrays(np.asarray(r), np.asarray(s)))
-    l_r, l_s = l_comoment(a, rs, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    l_r, l_s = l_comoment(a, rs, trim, dtype=dtype, **kwargs)
 
     l_s = np.diagonal(l_s, axis1=-2, axis2=-1)
 
     return l_r / np.expand_dims(l_s, -1)
 
 
+def l_costats(
+    a: npt.ArrayLike,
+    /,
+    trim: tuple[float, float] = (0, 0),
+    *,
+    dtype: np.dtype[T] | type[T] = np.float_,
+    **kwargs: Unpack[LComomentOptions],
+) -> npt.NDArray[T]:
+    """
+    Calculates the L-*co*scale, L-corr(elation), L-*co*skew(ness) and 
+    L-*co*kurtosis.
+
+    Equivalent to `lmo.l_coratio(a, [2, 2, 3, 4], [0, 2, 2, 2], *, **)`.
+
+    See Also:
+        - [`lmo.l_stats`][lmo.l_stats]
+        - [`lmo.l_coratio`][lmo.l_coratio]
+    """
+    r, s = [2, 2, 3, 4], [0, 2, 2, 2]
+    return l_coratio(a, r, s, trim=trim, dtype=dtype, **kwargs)
+
+
 def l_coloc(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     L-colocation matrix of 1st L-comoment estimates, $\Lambda^{(t_1, t_2)}_1$.
 
     Alias for [`lmo.l_comoment(a, 1, *, **)`][lmo.l_comoment].
 
     Notes:
@@ -241,24 +270,24 @@
 
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_loc`][lmo.l_loc]
         - [`numpy.mean`][numpy.mean]
     """
-    return l_comoment(a, 1, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    return l_comoment(a, 1, trim, dtype=dtype, **kwargs)
 
 
 def l_coscale(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     L-coscale matrix of 2nd L-comoment estimates, $\Lambda^{(t_1, t_2)}_2$.
 
     Alias for [`lmo.l_comoment(a, 2, *, **)`][lmo.l_comoment].
 
     Analogous to the (auto-) variance-covariance matrix, the L-coscale matrix
@@ -277,24 +306,24 @@
                [-0.37918065,  0.54440895]])
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_scale`][lmo.l_scale]
         - [`numpy.cov`][numpy.cov]
     """
-    return l_comoment(a, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    return l_comoment(a, 2, trim, dtype=dtype, **kwargs)
 
 
 def l_corr(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     Sample L-correlation coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_2$;
     the ratio of the L-coscale matrix over the L-scale **column**-vectors.
 
     Alias for [`lmo.l_coratio(a, 2, 2, *, **)`][lmo.l_coratio].
 
@@ -323,48 +352,48 @@
         array([[ 1.        , -0.66383285],
                [-0.66383285,  1.        ]])
 
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`numpy.corrcoef`][numpy.corrcoef]
     """
-    return l_coratio(a, 2, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    return l_coratio(a, 2, 2, trim, dtype=dtype, **kwargs)
 
 
 def l_coskew(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     Sample L-coskewness coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_3$.
 
     Alias for [`lmo.l_coratio(a, 3, 2, *, **)`][lmo.l_coratio].
 
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`lmo.l_skew`][lmo.l_skew]
     """
-    return l_coratio(a, 3, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    return l_coratio(a, 3, 2, trim, dtype=dtype, **kwargs)
 
 
 def l_cokurtosis(
     a: npt.ArrayLike,
     /,
-    trim: tuple[int, int] = (0, 0),
-    rowvar: bool = True,
+    trim: tuple[float, float] = (0, 0),
+    *,
     dtype: np.dtype[T] | type[T] = np.float_,
-    **kwargs: Any,
+    **kwargs: Unpack[LComomentOptions],
 ) -> npt.NDArray[T]:
     r"""
     Sample L-cokurtosis coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_4$.
 
     Alias for [`lmo.l_coratio(a, 4, 2, *, **)`][lmo.l_coratio].
 
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`lmo.l_kurtosis`][lmo.l_kurtosis]
     """
-    return l_coratio(a, 4, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    return l_coratio(a, 4, 2, trim, dtype=dtype, **kwargs)
```

### Comparing `lmo-0.7.0/lmo/_pwm.py` & `lmo-0.8.0/lmo/pwm_beta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Power-Weighted Moment (PWM) estimators.
+r"""
+Power-Weighted Moment (PWM) $\beta_k = M_{1,k,0}$.
 
 Primarily used as an intermediate step for L-moment estimation.
 """
-__all__ = 'b_weights', 'b_moment_cov'
+__all__ = 'weights', 'cov'
 
 from typing import Any, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 
 from ._utils import ordered
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
-def b_weights(
+def weights(
     r: int,
     n: int,
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
 ) -> npt.NDArray[T]:
     r"""
     Probability Weighted moment (PWM) projection matrix $B$ of the
@@ -33,15 +33,16 @@
         n: Sample count.
         dtype: Desired output floating data type.
 
     Returns:
         P_b: Upper-triangular projection matrix of shape `(r, n)`.
 
     Examples:
-        >>> b_weights(4, 5)
+        >>> from lmo import pwm_beta
+        >>> pwm_beta.weights(4, 5)
         array([[0.2       , 0.2       , 0.2       , 0.2       , 0.2       ],
                [0.        , 0.05      , 0.1       , 0.15      , 0.2       ],
                [0.        , 0.        , 0.03333333, 0.1       , 0.2       ],
                [0.        , 0.        , 0.        , 0.05      , 0.2       ]])
 
     """
     if not (0 <= r <= n):
@@ -59,15 +60,15 @@
     for k in range(1, r):
         w_r[k, k:] = w_r[k - 1, k:] * i1[:-k] / (n - k)
 
     # the + 0. eliminates negative zeros
     return cast(npt.NDArray[T], w_r / n + 0.)
 
 
-def b_moment_cov(
+def cov(
     a: npt.ArrayLike,
     r: int,
     /,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
@@ -96,15 +97,15 @@
     x = ordered(a, axis=axis, dtype=dtype, **kwargs)
 
     # ensure the samples are "in front" (along axis=0)
     if axis and x.ndim > 1:
         x = np.moveaxis(x, axis, 0)
 
     n = len(x)
-    p_k = b_weights(r, n, dtype=dtype)
+    p_k = weights(r, n, dtype=dtype)
 
     # beta pwm estimates
     b = p_k @ x if x.ndim == 1 else np.inner(p_k, x.T)
     assert b.shape == (r, *x.shape[1:])
 
     # the covariance matrix
     s_b = np.empty((r, *b.shape), dtype=dtype)
```

### Comparing `lmo-0.7.0/lmo/_utils.py` & `lmo-0.8.0/lmo/_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-__all__ = 'clean_order', 'ensure_axis_at', 'as_float_array', 'ordered'
+__all__ = (
+    'clean_order',
+    'ensure_axis_at',
+    'as_float_array',
+    'ordered',
+    'moments_to_ratio',
+)
 
 from typing import Any, SupportsIndex, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
 from .typing import IndexOrder, IntVector, SortKind
 
 T = TypeVar('T', bound=np.generic)
+FT = TypeVar('FT', bound=np.floating[Any])
 
 
 def clean_order(
     order: SupportsIndex,
     /,
     name: str = 'r',
     strict: bool = False,
@@ -153,7 +160,29 @@
     x_k = _sort_like(_x)
 
     if aweights is None:
         return x_k
 
     w_k = _sort_like(_clean_array(aweights))
     return _apply_aweights(x_k, w_k, axis=axis or 0)
+
+
+def moments_to_ratio(
+    rs: npt.NDArray[np.integer[Any]],
+    l_rs: npt.NDArray[FT],
+    /,
+) -> FT | npt.NDArray[FT]:
+    assert rs.shape == l_rs.shape, [rs.shape, l_rs.shape]
+    assert len(rs) == 2
+
+    r_eq_s = rs[0] == rs[1]
+    if r_eq_s.ndim < l_rs.ndim - 1:
+        r_eq_s = r_eq_s.reshape(
+            r_eq_s.shape + (1,) * (l_rs.ndim - r_eq_s.ndim - 1),
+        )
+
+    with np.errstate(divide='ignore', invalid='ignore'):
+        return np.where(
+            r_eq_s,
+            np.ones_like(l_rs[0]),
+            np.divide(l_rs[0], l_rs[1], where=~r_eq_s),
+        )[()]
```

### Comparing `lmo-0.7.0/lmo/diagnostic.py` & `lmo-0.8.0/lmo/diagnostic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Statistical test and tools."""
 
 __all__ = ('normaltest',)
 
-from typing import NamedTuple, cast
+from typing import NamedTuple
 
 import numpy as np
 import numpy.typing as npt
 
 from ._lm import l_ratio
 
 
@@ -14,14 +14,15 @@
     statistic: float | npt.NDArray[np.float_]
     pvalue: float | npt.NDArray[np.float_]
 
 
 def normaltest(
     a: npt.ArrayLike,
     /,
+    *,
     axis: int | None = None,
 ) -> NormaltestResult:
     r"""
     Test the null hypothesis that a sample comes from a normal distribution.
     Based on the Harri & Coble (2011) test, and includes Hosking's correction.
 
     Args:
@@ -54,15 +55,15 @@
     """
     x = np.asanyarray(a)
 
     # sample size
     n = x.size if axis is None else x.shape[axis]
 
     # L-skew and L-kurtosis
-    t3, t4 = cast(npt.NDArray[np.float_], l_ratio(a, [3, 4], [2, 2], axis=axis))
+    t3, t4 = l_ratio(a, [3, 4], [2, 2], axis=axis)
 
     # theoretical L-skew and L-kurtosis of the normal distribution (for all
     # loc/mu and scale/sigma)
     tau3, tau4 = 0.0, 30/np.pi * np.arctan(np.sqrt(2)) - 9
 
     z3 = (t3 - tau3) / np.sqrt(
         0.1866 / n
```

### Comparing `lmo-0.7.0/lmo/linalg.py` & `lmo-0.8.0/lmo/linalg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ruff: noqa: N803
 """Linear algebra and linearized orthogonal polynomials."""
 
 __all__ = (
     'sandwich',
+    'pascal',
+    'ir_pascal',
     'sh_legendre',
     'sh_jacobi',
     'succession_matrix',
     'trim_matrix',
 )
 
 import sys
@@ -19,15 +21,15 @@
     from typing_extensions import assert_never
 
 import numpy as np
 import numpy.typing as npt
 
 from .typing import AnyInt
 
-T = TypeVar('T', bound=np.number[Any])
+T = TypeVar('T', bound=np.integer[Any] | np.floating[Any])
 
 
 def sandwich(
     A: npt.NDArray[np.number[Any]],
     X: npt.NDArray[T | np.number[Any]],
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
@@ -48,15 +50,109 @@
         - https://wikipedia.org/wiki/Covariance_matrix
     """
     # if X is 1 - d, this is equivalent to: C @ S_b @ C.T
     spec = 'ui, ij..., vj -> uv...'
     return np.einsum(spec, A, X, A, dtype=dtype)  # pyright: ignore
 
 
-def sh_legendre(k : int, /, dtype: type[T] = np.int_) -> npt.NDArray[T]:
+def pascal(
+    k: int,
+    /,
+    dtype: np.dtype[T] | type[T] = np.int_,
+    *,
+    inv: bool = False,
+) -> npt.NDArray[T]:
+    r"""
+    Construct the lower-diagonal Pascal matrix $L_{k \times k$}$, or its matrix
+    inverse $L^{-1}$.
+
+    $$
+    \begin{align}
+    L_{ij} &= \binom{i}{j} \\
+    L^{-1}_{ij} &= (-1)^{i - j} L_{ij}
+    \end{align}
+    $$
+
+    Implemented using recursion, unlike the slow naive implementation from the
+    equivalent [`scipy.linalg.pascal`][scipy.linalg.pascal] and
+    [`scipy.linalg.invpascal`][scipy.linalg.invpascal] functions using
+    `kind='lower'`.
+    By using the binomial recurrence relation, assuming $0 < j < i$,
+    $\binom{i}{j} = \frac{i}{j} \binom{i-1}{j-1}$, the following recursive
+    definition is obtained:
+
+    $$
+    L_{ij} =
+    \begin{cases}
+        0 & \text{if } i < j \text{,} \\
+        1 & \text{if } i = j \vee j = 0 \text{, and} \\
+        (i \, L_{i-1,\, j-1}) / j & \text{otherwise.}
+    \end{cases}
+    $$
+
+    Examples:
+        >>> import numpy as np
+        >>> from lmo.linalg import pascal
+        >>> pascal(4)
+        array([[1, 0, 0, 0],
+               [1, 1, 0, 0],
+               [1, 2, 1, 0],
+               [1, 3, 3, 1]])
+        >>> pascal(4, inv=True)
+        array([[ 1,  0,  0,  0],
+               [-1,  1,  0,  0],
+               [ 1, -2,  1,  0],
+               [-1,  3, -3,  1]])
+        >>> np.rint(np.linalg.inv(pascal(4))).astype(np.int_)
+        array([[ 1,  0,  0,  0],
+               [-1,  1,  0,  0],
+               [ 1, -2,  1,  0],
+               [-1,  3, -3,  1]])
+
+        Now, let's compare with scipy:
+
+        >>> from scipy.linalg import invpascal
+        >>> invpascal(4, kind='lower')
+        array([[ 1,  0,  0,  0],
+               [-1,  1,  0,  0],
+               [ 1, -2,  1,  0],
+               [-1,  3, -3,  1]])
+    """
+    assert k >= 0
+    out = np.zeros((k, k), dtype=dtype)
+    if k == 0:
+        return out
+
+    out[:, 0] = 1
+    if inv:
+        # 1337 matrix inversion
+        out[1::2, 0] = -1
+
+    jj = np.arange(1, k, dtype=np.int_)
+    for i in range(1, k):
+        out[i, 1:i+1] = i * out[i - 1, :i] // jj[:i]
+
+    return out
+
+
+def ir_pascal(k: int, /) -> npt.NDArray[np.float_]:
+    r"""
+    Inverse regulatized lower-diagonal Pascal matrix,
+    $\bar{L}_{ij} = L^{-1}_ij / i$.
+
+    Used to linearly combine order statistics order statistics into L-moments.
+    """
+    return pascal(k, np.float_, inv=True) / np.arange(1, k + 1)[:, None]
+
+
+def sh_legendre(
+    k : int,
+    /,
+    dtype: np.dtype[T] | type[T] = np.int_,
+) -> npt.NDArray[T]:
     r"""
     Shifted Legendre polynomial coefficient matrix $\widetilde{P}$ of
     shape `(k, k)`.
 
     The $j$-th coefficient of the shifted Legendre polynomial of degree $k$ is
     at $(k, j)$:
 
@@ -89,27 +185,39 @@
     See Also:
         - https://wikipedia.org/wiki/Legendre_polynomials
         - https://wikipedia.org/wiki/Pascal_matrix
     """
     return sh_jacobi(k, 0, 0).astype(dtype)
 
 
-def _sh_jacobi_i(k: int, a: int, b: int, dtype: type[T]) -> npt.NDArray[T]:
+def _sh_jacobi_i(
+    k: int,
+    a: int,
+    b: int,
+    /,
+    dtype: np.dtype[T] | type[T],
+) -> npt.NDArray[T]:
     out = np.zeros((k, k), dtype=dtype)
     for r in range(k):
         for j in range(r + 1):
             out[r, j] = (
                 (-1) ** (r - j)
                 * comb(r + a + b + j, j)
                 * comb(r + b, r - j)
             )
     return out
 
 
-def _sh_jacobi_f(k: int, a: float, b: float, dtype: type[T]) -> npt.NDArray[T]:
+def _sh_jacobi_f(
+    k: int,
+    a: float,
+    b: float,
+    /,
+    dtype: np.dtype[T] | type[T],
+) -> npt.NDArray[T]:
     out = np.zeros((k, k), dtype=dtype)
 
     # semi dynamic programming
     lfact_j = np.array([lgamma(j + 1) for j in range(k)])
     lfact_jb = np.array([lgamma(j + b + 1) for j in range(k)])
     lfact_jab = np.array([lgamma(j + a + b + 1) for j in range(k * 2)])
 
@@ -129,15 +237,15 @@
 
 
 def sh_jacobi(
     k: AnyInt,
     a: T | int,
     b: T | int,
     /,
-    dtype: type[T] | None = None,
+    dtype: np.dtype[T] | type[T] | None = None,
 ) -> npt.NDArray[T | np.int_]:
     r"""
     Shifted Jacobi polynomial coefficient matrix $\widetilde{P}^{(a,b)}$ of
     shape `(k, k)`.
 
     The $j$-th coefficient of the shifted Jacobi polynomial of degree $k$ is
     at $(k, j)$:
```

### Comparing `lmo-0.7.0/pyproject.toml` & `lmo-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "lmo"
-version = "0.7.0"
+version = "0.8.0"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
```

### Comparing `lmo-0.7.0/PKG-INFO` & `lmo-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.7.0
+Version: 0.8.0
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

