# Comparing `tmp/inscar-3.0.3.tar.gz` & `tmp/inscar-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscar-3.0.3.tar", max compression
+gzip compressed data, was "inscar-3.0.4.tar", max compression
```

## Comparing `inscar-3.0.3.tar` & `inscar-3.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1088 2022-05-27 11:03:24.790545 inscar-3.0.3/LICENSE.rst
--rw-r--r--   0        0        0     4542 2022-05-27 11:03:24.790545 inscar-3.0.3/README.rst
--rw-r--r--   0        0        0      964 2022-05-27 11:03:38.678639 inscar-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      347 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/__init__.py
--rw-r--r--   0        0        0     5912 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/config.py
--rw-r--r--   0        0        0     3142 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/experimental/extra_vdfs.py
--rw-r--r--   0        0        0     7861 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/integrand_functions.py
--rw-r--r--   0        0        0     3977 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/numba_integration.py
--rw-r--r--   0        0        0     8996 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/spectrum_calculation.py
--rw-r--r--   0        0        0     3036 2022-05-27 11:03:24.850546 inscar-3.0.3/src/inscar/vdfs.py
--rw-r--r--   0        0        0     5624 2022-05-27 11:03:40.502143 inscar-3.0.3/setup.py
--rw-r--r--   0        0        0     5326 2022-05-27 11:03:40.502682 inscar-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-24 14:42:00.402468 inscar-3.0.4/LICENSE.rst
+-rw-r--r--   0        0        0     4894 2023-07-24 14:42:00.402468 inscar-3.0.4/README.rst
+-rw-r--r--   0        0        0     1102 2023-07-24 14:42:27.126456 inscar-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-07-24 14:42:00.474468 inscar-3.0.4/src/inscar/__init__.py
+-rw-r--r--   0        0        0     6807 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/config.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/experimental/__init__.py
+-rw-r--r--   0        0        0     3667 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/experimental/extra_vdfs.py
+-rw-r--r--   0        0        0     8803 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/integrand_functions.py
+-rw-r--r--   0        0        0     5217 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/numba_integration.py
+-rw-r--r--   0        0        0     9231 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/spectrum_calculation.py
+-rw-r--r--   0        0        0     3285 2023-07-24 14:42:00.478468 inscar-3.0.4/src/inscar/vdfs.py
+-rw-r--r--   0        0        0     5689 1970-01-01 00:00:00.000000 inscar-3.0.4/PKG-INFO
```

### Comparing `inscar-3.0.3/LICENSE.rst` & `inscar-3.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `inscar-3.0.3/README.rst` & `inscar-3.0.4/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -65,38 +65,38 @@
 Please see the `Modules Reference <Modules_>`_ for details.
 
 Physical environment
 ^^^^^^^^^^^^^^^^^^^^
 
 The plasma parameters that are supported natively by the program are
 
-* Radar frequency [Hz]
+* Radar frequency ``[Hz]``
 
-  * This will also set the radar wave number (= -4pi(radar frequency)/(speed of light))
+  * This will also set the radar wave number ``(= -4pi(radar frequency)/(speed of light))``
 
-* Magnetic field strength [T]
-* Aspect angle [1]
-* Electron temperature [K]
-* Ion temperature [K]
-* Electron collision frequency [Hz]
-* Ion collision frequency [Hz]
-* Electron mass in atomic mass units [u]
-* Ion mass in atomic mass units [u]
-* Electron number density [m^(-3)]
-* Ion number density [m^(-3)]
-* Kappa value for the kappa velocity distribution function
+* Magnetic field strength ``[T]``
+* Aspect angle ``[1]``
+* Electron temperature ``[K]``
+* Ion temperature ``[K]``
+* Electron collision frequency ``[Hz]``
+* Ion collision frequency ``[Hz]``
+* Electron mass in atomic mass units ``[u]``
+* Ion mass in atomic mass units ``[u]``
+* Electron number density ``[m^(-3)]``
+* Ion number density ``[m^(-3)]``
+* Kappa value for the kappa velocity distribution function ``[1]``
 
 Custom simulation set-ups can be made by inheriting from the different classes. Say you
 want a ``Particle`` class that also carries information about the temperature of a
 collection of super thermal electrons as well as some height information. You then
 inherit from ``Particle`` and decorate it with the ``@attr.s`` object:
 
 .. code:: python
 
-   @attr.s
+    @attr.s
     class RealDataParticle(isr.Particle):
         """Create a particle object with extra attributes."""
 
         superthermal_temperature: float = attr.ib(
             default=90000,
             validator=is_positive,
             on_setattr=attr.setters.validate,
@@ -111,15 +111,23 @@
 The program support different methods of calculating the spectrum, based on how you
 assume the particles to be distributed. This includes a Maxwellian distribution
 (``IntMaxwell`` class) and a kappa distribution (``IntKappa`` class), in addition to any
 arbitrary isotropic distribution (``IntLong`` class) which can take any ``Vdf`` as
 particle velocity distribution (default is ``VdfMaxwell``). An example showing how a new
 ``Vdf`` class can be made is given in assets_ (``VdfRealData``).
 
+Aside
+^^^^^
+
+This program was developed during my master thesis. For a more detailed explanation of
+the mathematical derivations and an analysis of the numerical precision of the program,
+please refer to the thesis found at `munin.uit.no`_.
+
 .. _Hagfors (1961): https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/JZ066i006p01699
 .. _Mace (2003): https://aip.scitation.org/doi/pdf/10.1063/1.1570828
+.. _munin.uit.no: https://hdl.handle.net/10037/19542
 .. _PyPI: https://pypi.org/
 .. _pip: https://pip.pypa.io/
 .. _assets: https://github.com/engeir/inscar/tree/main/assets
 .. github-only
 .. _Contributor Guide: CONTRIBUTING.rst
 .. _Modules: https://inscar.readthedocs.io/en/latest/modules.html
```

### Comparing `inscar-3.0.3/src/inscar/experimental/extra_vdfs.py` & `inscar-3.0.4/src/inscar/vdfs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,119 @@
-"""Extra, experimental velocity distribution functions."""
+"""Velocity distribution function to be used by the integrand class ``a_vdf``.
+
+One of the integrands available for use in the Gordeyev integral.
+"""
+
+from abc import ABC, abstractmethod
 
 import numpy as np
 import scipy.constants as const
-import scipy.integrate as si
 import scipy.special as sps
 
-import inscar as isr
+from inscar import config
+
+
+class Vdf(ABC):
+    """Base class for a VDF object.
+
+    Parameters
+    ----------
+    ABC:
+        Abstract base class that all Vdf objects inherit from
+    """
+
+    @abstractmethod
+    def normalize(self) -> None:
+        """Calculate the normalization for the VDF."""
+
+    @abstractmethod
+    def f_0(self) -> np.ndarray:
+        """Return the values along the velocity axis of a VDF.
+
+        Returns
+        -------
+        np.ndarray
+            1D array with the VDF values at the sampled points
+        """
 
 
-class VdfKappa2(isr.Vdf):
-    """Create an object that make kappa vol. 2 distribution functions.
+class VdfMaxwell(Vdf):
+    """Create an object that make Maxwellian distribution functions.
 
-    Kappa VDF used in dispersion relation paper by Ziebell, Gaelzer and Simoes
-    (2017). Defined by Leubner (2002) (sec 3.2).
+    Parameters
+    ----------
+    VDF: ABC
+        Abstract base class to make VDF objects
     """
 
-    def __init__(self, params: isr.Parameters, particle: isr.Particle):
+    def __init__(self, params: config.Parameters, particle: config.Particle):
         """Initialize VDF parameters.
 
         Parameters
         ----------
         params : Parameters
             `Parameters` object with the parameters of the simulation.
         particle : Particle
             `Particle` object with the parameters of the particle.
         """
         self.params = params
         self.particle = particle
         self.normalize()
 
     def normalize(self) -> None:
-        self.v_th = np.sqrt(self.particle.temperature * const.k / self.particle.mass)
         self.A = (
-            (np.pi * self.particle.kappa * self.v_th**2) ** (-3 / 2)
-            * sps.gamma(self.particle.kappa)
-            / sps.gamma(self.particle.kappa - 3 / 2)
-        )
+            2 * np.pi * self.particle.temperature * const.k / self.particle.mass
+        ) ** (-3 / 2)
 
     def f_0(self) -> np.ndarray:
-        return self.A * (
-            1
-            + self.particle.velocity_axis**2 / (self.particle.kappa * self.v_th**2)
-        ) ** (-self.particle.kappa)
+        return self.A * np.exp(
+            -self.particle.velocity_axis**2
+            / (2 * self.particle.temperature * const.k / self.particle.mass)
+        )
 
 
-class VdfGaussShell(isr.Vdf):
-    """Create an object that make Gauss shell distribution functions.
+class VdfKappa(Vdf):
+    """Create an object that make kappa distribution functions.
 
-    This implementation need more testing and refining.
+    Notes
+    -----
+    Kappa VDF used in Gordeyev paper by Mace [1]_.
+
+    References
+    ----------
+    .. [1] R. L. Mace, "A Gordeyev integral for electrostatic waves in a magnetized
+       plasma with a kappa velocity distribution," Physics of plasmas, vol. 10, no. 6,
+       pp. 2101-2193, 2003.
     """
 
-    def __init__(self, params: isr.Parameters, particle: isr.Particle):
+    def __init__(self, params: config.Parameters, particle: config.Particle):
         """Initialize VDF parameters.
 
         Parameters
         ----------
         params : Parameters
             `Parameters` object with the parameters of the simulation.
         particle : Particle
             `Particle` object with the parameters of the particle.
         """
         self.params = params
         self.particle = particle
-        temp_superthermal = getattr(self.particle, "temperature_superthermal", 90000)
-        self.vth = np.sqrt(self.particle.temperature * const.k / self.particle.mass)
-        self.r = (temp_superthermal * const.k / self.particle.mass) ** 0.5
-        self.steep = 5
-        self.f_M = isr.VdfMaxwell(self.params, self.particle)
         self.normalize()
 
     def normalize(self) -> None:
-        func = np.exp(
-            -self.steep
-            * (abs(self.particle.velocity_axis) - self.r) ** 2
-            / (2 * self.particle.temperature * const.k / self.particle.mass)
+        self.theta_2 = (
+            2
+            * ((self.particle.kappa - 3 / 2) / self.particle.kappa)
+            * self.particle.temperature
+            * const.k
+            / self.particle.mass
         )
-        f = func * self.particle.velocity_axis**2 * 4 * np.pi
-        self.A = 1 / si.simps(f, self.particle.velocity_axis)
-        ev = 0.5 * const.m_e * self.r**2 / const.eV
-        print(f"Gauss shell at E = {round(ev, 2)} eV")
-
-    def f_0(self) -> np.ndarray:
-        func = (
-            self.A
-            * np.exp(
-                -self.steep
-                * (abs(self.particle.velocity_axis) - self.r) ** 2
-                / (2 * self.particle.temperature * const.k / self.particle.mass)
-            )
-            + 1e4 * self.f_M.f_0()
+        self.A = (
+            (np.pi * self.particle.kappa * self.theta_2) ** (-3 / 2)
+            * sps.gamma(self.particle.kappa + 1)
+            / sps.gamma(self.particle.kappa - 1 / 2)
         )
 
-        return func / (1e4 + 1)
+    def f_0(self) -> np.ndarray:
+        return self.A * (
+            1 + self.particle.velocity_axis**2 / (self.particle.kappa * self.theta_2)
+        ) ** (-self.particle.kappa - 1)
```

### Comparing `inscar-3.0.3/src/inscar/integrand_functions.py` & `inscar-3.0.4/src/inscar/integrand_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,23 @@
     def integrand(self) -> np.ndarray:
         """Return the `np.ndarray` that is used as the integrand."""
 
 
 class IntKappa(Integrand):
     """Implementation of the integrand of the Gordeyev integral.
 
-    This implementation is for the kappa distribution described by Mace (2003).
+    Notes
+    -----
+    This implementation is for the kappa distribution described by Mace [1]_.
+
+    References
+    ----------
+    .. [1] R. L. Mace, "A Gordeyev integral for electrostatic waves in a magnetized
+       plasma with a kappa velocity distribution," Physics of plasmas, vol. 10, no. 6,
+       pp. 2101-2193, 2003.
     """
 
     @property
     def the_type(self) -> str:
         return "kappa"
 
     def __init__(self) -> None:
@@ -100,16 +108,27 @@
             * np.exp(-y * self.particle.collision_frequency)
         )
 
 
 class IntMaxwell(Integrand):
     """Implementation of the integrand of the Gordeyev integral.
 
+    Notes
+    -----
     This implementation is for the integral for the Maxwellian distribution from e.g.
-    Hagfors (1961) or Mace (2003).
+    Hagfors [1]_ or Mace [2]_.
+
+    References
+    ----------
+    .. [1] T. Hagfors, "Density Fluctuations in a Plasma in a Magnetic Field, with
+       Applications to the Ionosphere," Journal of Geophysical Research, vol. 66, no.
+       9, pp. 1699-1712, 1961.
+    .. [2] R. L. Mace, "A Gordeyev integral for electrostatic waves in a magnetized
+       plasma with a kappa velocity distribution," Physics of plasmas, vol. 10, no. 6,
+       pp. 2101-2193, 2003.
     """
 
     @property
     def the_type(self) -> str:
         return "maxwell"
 
     def __init__(self) -> None:
@@ -146,16 +165,24 @@
             / self.particle.mass
         )
 
 
 class IntLong(Integrand):
     """Implementation of the integrand of the Gordeyev integral.
 
+    Notes
+    -----
     This implementation is for the integral for the isotropic distribution from Mace
-    (2003).
+    [1]_.
+
+    References
+    ----------
+    .. [1] R. L. Mace, "A Gordeyev integral for electrostatic waves in a magnetized
+       plasma with a kappa velocity distribution," Physics of plasmas, vol. 10, no. 6,
+       pp. 2101-2193, 2003.
     """
 
     @property
     def the_type(self) -> str:
         return "a_vdf"
 
     def __init__(self) -> None:
```

### Comparing `inscar-3.0.3/src/inscar/spectrum_calculation.py` & `inscar-3.0.4/src/inscar/spectrum_calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,59 +23,59 @@
 
     def set_params(self, params: config.Parameters) -> None:
         """Set the plasma parameters.
 
         Parameters
         ----------
         params: Parameters
-            An instance of the `Parameters` class.
+            An instance of the ``Parameters`` class.
         """
         self.params = params
 
     def set_ion(self, ion: config.Particle) -> None:
         """Set the ion particles to use.
 
         Parameters
         ----------
         ion: Particle
-            An instance of the `Particle` class, representing ions.
+            An instance of the ``Particle`` class, representing ions.
         """
         self.ion = ion
 
     def set_electron(self, electron: config.Particle) -> None:
         """Set the electron particles to use.
 
         Parameters
         ----------
         electron: Particle
-            An instance of the `Particle` class, representing electrons.
+            An instance of the ``Particle`` class, representing electrons.
         """
         self.electron = electron
 
     def set_ion_integration_function(
         self, function: integrand_functions.Integrand
     ) -> None:
         """Set the ion integration method to use.
 
         Parameters
         ----------
         function: Integrand
-            An object of type `Integrand`, representing the ions.
+            An object of type ``Integrand``, representing the ions.
         """
         self.ion_integration_function = function
 
     def set_electron_integration_function(
         self, function: integrand_functions.Integrand
     ) -> None:
         """Set the electron integration method to use.
 
         Parameters
         ----------
         function: Integrand
-            An object of type `Integrand`, representing the electrons.
+            An object of type ``Integrand``, representing the electrons.
         """
         self.electron_integration_function = function
 
     def calculate_spectrum(self) -> Tuple[np.ndarray, np.ndarray]:
         """Calculate a spectrum based on the given parameters and calculation methods.
 
         Returns
@@ -97,15 +97,16 @@
             raise ValueError("No electron particle set. Use set_electron().")
         if not hasattr(self, "ion_integration_function"):
             raise ValueError(
                 "No ion integration function set. Use set_ion_integration_function()."
             )
         if not hasattr(self, "electron_integration_function"):
             raise ValueError(
-                "No electron integration function set. Use set_electron_integration_function()."
+                "No electron integration function set. "
+                + "Use set_electron_integration_function()."
             )
 
         fi = self._calulate_f(self.ion, self.ion_integration_function)
         fe = self._calulate_f(self.electron, self.electron_integration_function)
 
         xp_i = self._susceptibility(self.ion, self.ion_integration_function)
         xp_e = self._susceptibility(self.electron, self.electron_integration_function)
@@ -122,21 +123,27 @@
                 / denominator
             )
         return self.params.linear_frequency, spectrum
 
     def set_calculate_f_function(
         self, f_func: Callable[[config.Particle, integrand_functions.Integrand], float]
     ) -> None:
-        """Set what function to use to calculate the F function.
+        """Set what function to use to calculate the :math:`F` function.
+
+        See also
+        --------
+        inscar.numba_integration.integrate
 
         Parameters
         ----------
         f_func: Callable[[Particle, Integrand], float]
             A function that take a particle and an integrand function as input, and that
-            calculates the F function based on these, returning a numpy array.
+            calculates the :math:`F` function based on these, returning a numpy array.
+            By default, the ``integrate`` function from the ``numba_integration`` module
+            is used.
         """
         self._calulate_f = f_func
 
     def _calulate_f_function(
         self, particle: config.Particle, int_func: integrand_functions.Integrand
     ) -> np.ndarray:
         int_func.initialize(self.params, particle)
```

### Comparing `inscar-3.0.3/src/inscar/vdfs.py` & `inscar-3.0.4/src/inscar/experimental/extra_vdfs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,106 @@
-"""Velocity distribution function to be used by the integrand class `a_vdf`.
-
-One of the integrands available for use in the Gordeyev integral.
-"""
-
-from abc import ABC, abstractmethod
+"""Extra, experimental velocity distribution functions."""
 
 import numpy as np
 import scipy.constants as const
+import scipy.integrate as si
 import scipy.special as sps
 
-from inscar import config
-
-
-class Vdf(ABC):
-    """Base class for a VDF object.
-
-    Parameters
-    ----------
-    ABC:
-        Abstract base class that all Vdf objects inherit from
-    """
-
-    @abstractmethod
-    def normalize(self) -> None:
-        """Calculate the normalization for the VDF."""
-
-    @abstractmethod
-    def f_0(self) -> np.ndarray:
-        """Return the values along the velocity axis of a VDF.
+import inscar as isr
 
-        Returns
-        -------
-        np.ndarray
-            1D array with the VDF values at the sampled points
-        """
 
+class VdfKappa2(isr.Vdf):
+    """Create an object that make kappa vol. 2 distribution functions.
 
-class VdfMaxwell(Vdf):
-    """Create an object that make Maxwellian distribution functions.
+    Notes
+    -----
+    Kappa VDF used in dispersion relation paper by Ziebell, Gaelzer and Simões
+    [1]_. Defined by Leubner [2]_.
 
-    Parameters
+    References
     ----------
-    VDF: ABC
-        Abstract base class to make VDF objects
+    .. [1] L. Ziebell, R. Gaelzer, & F. Simões, "Dispersion relation for electrostatic
+       waves in plasmas with isotropic and anisotropic Kappa distributions for electrons
+       and ions," Journal of Plasma Physics, vol. 83, no. 5, pp. 905830503, 2017.
+       doi:10.1017/S0022377817000733
+    .. [2] M. P. Leubner, "A nonextensive entropy approach to Kappa-distributions,"
+       Astrophysics and Space Science, vol. 282, no. 3, pp. 573-579, 2002.
+       doi:10.1029/2000JA000425
     """
 
-    def __init__(self, params: config.Parameters, particle: config.Particle):
+    def __init__(self, params: isr.Parameters, particle: isr.Particle):
         """Initialize VDF parameters.
 
         Parameters
         ----------
         params : Parameters
             `Parameters` object with the parameters of the simulation.
         particle : Particle
             `Particle` object with the parameters of the particle.
         """
         self.params = params
         self.particle = particle
         self.normalize()
 
     def normalize(self) -> None:
+        self.v_th = np.sqrt(self.particle.temperature * const.k / self.particle.mass)
         self.A = (
-            2 * np.pi * self.particle.temperature * const.k / self.particle.mass
-        ) ** (-3 / 2)
-
-    def f_0(self) -> np.ndarray:
-        return self.A * np.exp(
-            -self.particle.velocity_axis**2
-            / (2 * self.particle.temperature * const.k / self.particle.mass)
+            (np.pi * self.particle.kappa * self.v_th**2) ** (-3 / 2)
+            * sps.gamma(self.particle.kappa)
+            / sps.gamma(self.particle.kappa - 3 / 2)
         )
 
+    def f_0(self) -> np.ndarray:
+        return self.A * (
+            1
+            + self.particle.velocity_axis**2 / (self.particle.kappa * self.v_th**2)
+        ) ** (-self.particle.kappa)
 
-class VdfKappa(Vdf):
-    """Create an object that make kappa distribution functions.
 
-    Kappa VDF used in Gordeyev paper by Mace (2003).
+class VdfGaussShell(isr.Vdf):
+    """Create an object that make Gauss shell distribution functions.
 
+    This implementation need more testing and refining.
     """
 
-    def __init__(self, params: config.Parameters, particle: config.Particle):
+    def __init__(self, params: isr.Parameters, particle: isr.Particle):
         """Initialize VDF parameters.
 
         Parameters
         ----------
         params : Parameters
             `Parameters` object with the parameters of the simulation.
         particle : Particle
             `Particle` object with the parameters of the particle.
         """
         self.params = params
         self.particle = particle
+        temp_superthermal = getattr(self.particle, "temperature_superthermal", 90000)
+        self.vth = np.sqrt(self.particle.temperature * const.k / self.particle.mass)
+        self.r = (temp_superthermal * const.k / self.particle.mass) ** 0.5
+        self.steep = 5
+        self.f_M = isr.VdfMaxwell(self.params, self.particle)
         self.normalize()
 
     def normalize(self) -> None:
-        self.theta_2 = (
-            2
-            * ((self.particle.kappa - 3 / 2) / self.particle.kappa)
-            * self.particle.temperature
-            * const.k
-            / self.particle.mass
-        )
-        self.A = (
-            (np.pi * self.particle.kappa * self.theta_2) ** (-3 / 2)
-            * sps.gamma(self.particle.kappa + 1)
-            / sps.gamma(self.particle.kappa - 1 / 2)
+        func = np.exp(
+            -self.steep
+            * (abs(self.particle.velocity_axis) - self.r) ** 2
+            / (2 * self.particle.temperature * const.k / self.particle.mass)
         )
+        f = func * self.particle.velocity_axis**2 * 4 * np.pi
+        self.A = 1 / si.simps(f, self.particle.velocity_axis)
+        ev = 0.5 * const.m_e * self.r**2 / const.eV
+        print(f"Gauss shell at E = {round(ev, 2)} eV")
 
     def f_0(self) -> np.ndarray:
-        return self.A * (
-            1 + self.particle.velocity_axis**2 / (self.particle.kappa * self.theta_2)
-        ) ** (-self.particle.kappa - 1)
+        func = (
+            self.A
+            * np.exp(
+                -self.steep
+                * (abs(self.particle.velocity_axis) - self.r) ** 2
+                / (2 * self.particle.temperature * const.k / self.particle.mass)
+            )
+            + 1e4 * self.f_M.f_0()
+        )
+
+        return func / (1e4 + 1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inscar-3.0.3/setup.py` & `inscar-3.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: inscar
+Version: 3.0.4
+Summary: Calculate an incoherent scatter spectrum with arbitrary isotropic electron velocity distributions and radar pointing at oblique angles to the magnetic field
+Author: engeir
+Author-email: eirroleng@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: attrs (>=21.4,<23.0)
+Requires-Dist: importlib-metadata (>=4.11.4,<7.0.0)
+Requires-Dist: numba (>=0.55.1,<0.57.0)
+Requires-Dist: numpy (>=1.20.2,<2.0.0)
+Requires-Dist: scipy (>=1.6.2,<2.0.0)
+Project-URL: Documentation, https://inscar.readthedocs.io
+Description-Content-Type: text/x-rst
+
+inscar
+======
+
+    INcoherent SCAtter Radar spectrum
+
+|PyPI| |PyPI Downloads| |Status| |Python Version| |License| |Read the Docs| |Tests|
+|Codecov| |DOI| |pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/inscar.svg
+   :target: https://pypi.org/project/inscar/
+   :alt: PyPI
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/inscar.svg
+   :target: https://pypi.org/project/inscar/
+   :alt: PyPI Downloads
+.. |Status| image:: https://img.shields.io/pypi/status/inscar.svg
+   :target: https://pypi.org/project/inscar/
+   :alt: Status
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/inscar
+   :target: https://pypi.org/project/inscar
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/inscar/latest.svg?label=Read%20the%20Docs
+   :target: https://inscar.readthedocs.io/
+   :alt: Read the documentation at https://ncdump-rich.readthedocs.io/
+.. |Tests| image:: https://github.com/engeir/inscar/workflows/Tests/badge.svg
+   :target: https://github.com/engeir/inscar/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/engeir/inscar/branch/master/graph/badge.svg?token=P8S18UILSB
+   :target: https://codecov.io/gh/engeir/inscar
+   :alt: Codecov
+.. |DOI| image:: https://zenodo.org/badge/233043566.svg
+   :target: https://zenodo.org/badge/latestdoi/233043566
+   :alt: pre-commit
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+.. |CodeQL| image:: https://github.com/engeir/inscar/workflows/CodeQL/badge.svg
+   :alt: CodeQL
+
+.. image:: ./img/normal_is_spectra.png
+
+Info
+----
+
+Calculates an incoherent scatter radar spectrum based on the theory presented in
+`Hagfors (1961)`_ and `Mace (2003)`_.
+
+Installing
+----------
+
+You can install *inscar* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install inscar
+
+Usage
+-----
+
+Please see the `Modules Reference <Modules_>`_ for details.
+
+Physical environment
+^^^^^^^^^^^^^^^^^^^^
+
+The plasma parameters that are supported natively by the program are
+
+* Radar frequency ``[Hz]``
+
+  * This will also set the radar wave number ``(= -4pi(radar frequency)/(speed of light))``
+
+* Magnetic field strength ``[T]``
+* Aspect angle ``[1]``
+* Electron temperature ``[K]``
+* Ion temperature ``[K]``
+* Electron collision frequency ``[Hz]``
+* Ion collision frequency ``[Hz]``
+* Electron mass in atomic mass units ``[u]``
+* Ion mass in atomic mass units ``[u]``
+* Electron number density ``[m^(-3)]``
+* Ion number density ``[m^(-3)]``
+* Kappa value for the kappa velocity distribution function ``[1]``
+
+Custom simulation set-ups can be made by inheriting from the different classes. Say you
+want a ``Particle`` class that also carries information about the temperature of a
+collection of super thermal electrons as well as some height information. You then
+inherit from ``Particle`` and decorate it with the ``@attr.s`` object:
+
+.. code:: python
+
+    @attr.s
+    class RealDataParticle(isr.Particle):
+        """Create a particle object with extra attributes."""
+
+        superthermal_temperature: float = attr.ib(
+            default=90000,
+            validator=is_positive,
+            on_setattr=attr.setters.validate,
+        )
+        z: int = attr.ib(default=300)
+
+For more examples, see the assets_ directory.
+
+Calculation method
+^^^^^^^^^^^^^^^^^^
+
+The program support different methods of calculating the spectrum, based on how you
+assume the particles to be distributed. This includes a Maxwellian distribution
+(``IntMaxwell`` class) and a kappa distribution (``IntKappa`` class), in addition to any
+arbitrary isotropic distribution (``IntLong`` class) which can take any ``Vdf`` as
+particle velocity distribution (default is ``VdfMaxwell``). An example showing how a new
+``Vdf`` class can be made is given in assets_ (``VdfRealData``).
+
+Aside
+^^^^^
+
+This program was developed during my master thesis. For a more detailed explanation of
+the mathematical derivations and an analysis of the numerical precision of the program,
+please refer to the thesis found at `munin.uit.no`_.
+
+.. _Hagfors (1961): https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/JZ066i006p01699
+.. _Mace (2003): https://aip.scitation.org/doi/pdf/10.1063/1.1570828
+.. _munin.uit.no: https://hdl.handle.net/10037/19542
+.. _PyPI: https://pypi.org/
+.. _pip: https://pip.pypa.io/
+.. _assets: https://github.com/engeir/inscar/tree/main/assets
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
+.. _Modules: https://inscar.readthedocs.io/en/latest/modules.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['inscar', 'inscar.experimental']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=21.4.0,<22.0.0',
- 'importlib-metadata>=4.11.4,<5.0.0',
- 'matplotlib>=3.4.1,<4.0.0',
- 'numba>=0.55.1,<0.56.0',
- 'numpy>=1.20.2,<2.0.0',
- 'scipy>=1.6.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'inscar',
-    'version': '3.0.3',
-    'description': 'Calculate an incoherent scatter spectrum with arbitrary isotropic electron velocity distributions and radar pointing at oblique angles to the magnetic field',
-    'long_description': 'inscar\n======\n\n    INcoherent SCAtter Radar spectrum\n\n|PyPI| |PyPI Downloads| |Status| |Python Version| |License| |Read the Docs| |Tests|\n|Codecov| |DOI| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/inscar.svg\n   :target: https://pypi.org/project/inscar/\n   :alt: PyPI\n.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/inscar.svg\n   :target: https://pypi.org/project/inscar/\n   :alt: PyPI Downloads\n.. |Status| image:: https://img.shields.io/pypi/status/inscar.svg\n   :target: https://pypi.org/project/inscar/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/inscar\n   :target: https://pypi.org/project/inscar\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/inscar/latest.svg?label=Read%20the%20Docs\n   :target: https://inscar.readthedocs.io/\n   :alt: Read the documentation at https://ncdump-rich.readthedocs.io/\n.. |Tests| image:: https://github.com/engeir/inscar/workflows/Tests/badge.svg\n   :target: https://github.com/engeir/inscar/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/engeir/inscar/branch/master/graph/badge.svg?token=P8S18UILSB\n   :target: https://codecov.io/gh/engeir/inscar\n   :alt: Codecov\n.. |DOI| image:: https://zenodo.org/badge/233043566.svg\n   :target: https://zenodo.org/badge/latestdoi/233043566\n   :alt: pre-commit\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n.. |CodeQL| image:: https://github.com/engeir/inscar/workflows/CodeQL/badge.svg\n   :alt: CodeQL\n\n.. image:: ./img/normal_is_spectra.png\n\nInfo\n----\n\nCalculates an incoherent scatter radar spectrum based on the theory presented in\n`Hagfors (1961)`_ and `Mace (2003)`_.\n\nInstalling\n----------\n\nYou can install *inscar* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install inscar\n\nUsage\n-----\n\nPlease see the `Modules Reference <Modules_>`_ for details.\n\nPhysical environment\n^^^^^^^^^^^^^^^^^^^^\n\nThe plasma parameters that are supported natively by the program are\n\n* Radar frequency [Hz]\n\n  * This will also set the radar wave number (= -4pi(radar frequency)/(speed of light))\n\n* Magnetic field strength [T]\n* Aspect angle [1]\n* Electron temperature [K]\n* Ion temperature [K]\n* Electron collision frequency [Hz]\n* Ion collision frequency [Hz]\n* Electron mass in atomic mass units [u]\n* Ion mass in atomic mass units [u]\n* Electron number density [m^(-3)]\n* Ion number density [m^(-3)]\n* Kappa value for the kappa velocity distribution function\n\nCustom simulation set-ups can be made by inheriting from the different classes. Say you\nwant a ``Particle`` class that also carries information about the temperature of a\ncollection of super thermal electrons as well as some height information. You then\ninherit from ``Particle`` and decorate it with the ``@attr.s`` object:\n\n.. code:: python\n\n   @attr.s\n    class RealDataParticle(isr.Particle):\n        """Create a particle object with extra attributes."""\n\n        superthermal_temperature: float = attr.ib(\n            default=90000,\n            validator=is_positive,\n            on_setattr=attr.setters.validate,\n        )\n        z: int = attr.ib(default=300)\n\nFor more examples, see the assets_ directory.\n\nCalculation method\n^^^^^^^^^^^^^^^^^^\n\nThe program support different methods of calculating the spectrum, based on how you\nassume the particles to be distributed. This includes a Maxwellian distribution\n(``IntMaxwell`` class) and a kappa distribution (``IntKappa`` class), in addition to any\narbitrary isotropic distribution (``IntLong`` class) which can take any ``Vdf`` as\nparticle velocity distribution (default is ``VdfMaxwell``). An example showing how a new\n``Vdf`` class can be made is given in assets_ (``VdfRealData``).\n\n.. _Hagfors (1961): https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/JZ066i006p01699\n.. _Mace (2003): https://aip.scitation.org/doi/pdf/10.1063/1.1570828\n.. _PyPI: https://pypi.org/\n.. _pip: https://pip.pypa.io/\n.. _assets: https://github.com/engeir/inscar/tree/main/assets\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Modules: https://inscar.readthedocs.io/en/latest/modules.html\n',
-    'author': 'engeir',
-    'author_email': 'eirroleng@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

