# Comparing `tmp/precisenumbers-0.0.3.tar.gz` & `tmp/precisenumbers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precisenumbers-0.0.3.tar", last modified: Sun Jan 22 20:25:38 2023, max compression
+gzip compressed data, was "precisenumbers-0.0.4.tar", last modified: Mon Jul 24 21:30:24 2023, max compression
```

## Comparing `precisenumbers-0.0.3.tar` & `precisenumbers-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-01-22 20:25:38.880908 precisenumbers-0.0.3/
--rw-r--r--   0 jessicamoore   (501) staff       (20)     1066 2022-12-03 15:40:32.000000 precisenumbers-0.0.3/LICENSE
--rw-r--r--   0 jessicamoore   (501) staff       (20)      244 2023-01-22 20:25:38.880789 precisenumbers-0.0.3/PKG-INFO
--rw-r--r--   0 jessicamoore   (501) staff       (20)     1868 2022-12-19 21:35:25.000000 precisenumbers-0.0.3/README.rst
-drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-01-22 20:25:38.879761 precisenumbers-0.0.3/precisenumbers/
--rw-r--r--   0 jessicamoore   (501) staff       (20)     5382 2023-01-22 20:18:52.000000 precisenumbers-0.0.3/precisenumbers/__init__.py
--rw-r--r--   0 jessicamoore   (501) staff       (20)     1961 2023-01-22 20:18:52.000000 precisenumbers-0.0.3/precisenumbers/coordinates.py
-drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-01-22 20:25:38.880185 precisenumbers-0.0.3/precisenumbers.egg-info/
--rw-r--r--   0 jessicamoore   (501) staff       (20)      244 2023-01-22 20:25:38.000000 precisenumbers-0.0.3/precisenumbers.egg-info/PKG-INFO
--rw-r--r--   0 jessicamoore   (501) staff       (20)      309 2023-01-22 20:25:38.000000 precisenumbers-0.0.3/precisenumbers.egg-info/SOURCES.txt
--rw-r--r--   0 jessicamoore   (501) staff       (20)        1 2023-01-22 20:25:38.000000 precisenumbers-0.0.3/precisenumbers.egg-info/dependency_links.txt
--rw-r--r--   0 jessicamoore   (501) staff       (20)       21 2023-01-22 20:25:38.000000 precisenumbers-0.0.3/precisenumbers.egg-info/top_level.txt
--rw-r--r--   0 jessicamoore   (501) staff       (20)       38 2023-01-22 20:25:38.880947 precisenumbers-0.0.3/setup.cfg
--rw-r--r--   0 jessicamoore   (501) staff       (20)      327 2023-01-22 20:22:07.000000 precisenumbers-0.0.3/setup.py
-drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-01-22 20:25:38.880622 precisenumbers-0.0.3/tests/
--rw-r--r--   0 jessicamoore   (501) staff       (20)        0 2022-12-03 15:40:32.000000 precisenumbers-0.0.3/tests/__init__.py
--rw-r--r--   0 jessicamoore   (501) staff       (20)     3711 2023-01-15 18:28:24.000000 precisenumbers-0.0.3/tests/test_coordinates.py
--rw-r--r--   0 jessicamoore   (501) staff       (20)     4308 2023-01-22 20:18:52.000000 precisenumbers-0.0.3/tests/test_precisenumbers.py
+drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-07-24 21:30:24.072140 precisenumbers-0.0.4/
+-rw-r--r--   0 jessicamoore   (501) staff       (20)     1066 2023-04-05 00:55:59.000000 precisenumbers-0.0.4/LICENSE
+-rw-r--r--   0 jessicamoore   (501) staff       (20)      199 2023-07-24 21:30:24.072028 precisenumbers-0.0.4/PKG-INFO
+-rw-r--r--   0 jessicamoore   (501) staff       (20)     1868 2023-04-05 00:55:59.000000 precisenumbers-0.0.4/README.rst
+drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-07-24 21:30:24.071233 precisenumbers-0.0.4/precisenumbers/
+-rw-r--r--   0 jessicamoore   (501) staff       (20)     6136 2023-07-24 21:27:09.000000 precisenumbers-0.0.4/precisenumbers/__init__.py
+drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-07-24 21:30:24.071696 precisenumbers-0.0.4/precisenumbers.egg-info/
+-rw-r--r--   0 jessicamoore   (501) staff       (20)      199 2023-07-24 21:30:24.000000 precisenumbers-0.0.4/precisenumbers.egg-info/PKG-INFO
+-rw-r--r--   0 jessicamoore   (501) staff       (20)      253 2023-07-24 21:30:24.000000 precisenumbers-0.0.4/precisenumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 jessicamoore   (501) staff       (20)        1 2023-07-24 21:30:24.000000 precisenumbers-0.0.4/precisenumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 jessicamoore   (501) staff       (20)       21 2023-07-24 21:30:24.000000 precisenumbers-0.0.4/precisenumbers.egg-info/top_level.txt
+-rw-r--r--   0 jessicamoore   (501) staff       (20)       38 2023-07-24 21:30:24.072177 precisenumbers-0.0.4/setup.cfg
+-rw-r--r--   0 jessicamoore   (501) staff       (20)      327 2023-07-24 21:27:05.000000 precisenumbers-0.0.4/setup.py
+drwxr-xr-x   0 jessicamoore   (501) staff       (20)        0 2023-07-24 21:30:24.071881 precisenumbers-0.0.4/tests/
+-rw-r--r--   0 jessicamoore   (501) staff       (20)        0 2023-04-05 00:55:59.000000 precisenumbers-0.0.4/tests/__init__.py
+-rw-r--r--   0 jessicamoore   (501) staff       (20)     4814 2023-07-24 21:23:23.000000 precisenumbers-0.0.4/tests/test_precisenumbers.py
```

### Comparing `precisenumbers-0.0.3/LICENSE` & `precisenumbers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `precisenumbers-0.0.3/README.rst` & `precisenumbers-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `precisenumbers-0.0.3/precisenumbers/__init__.py` & `precisenumbers-0.0.4/precisenumbers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 import logging
 import math
 from typing import Optional, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
+def _float_to_str(f: float) -> str:
+    float_string = str(f)
+    if 'e' not in float_string:  # detect scientific notation
+        return float_string
+
+    digits, exp = float_string.split('e')
+    digits = digits.replace('.', '').replace('-', '')
+    exp = int(exp)
+    zero_padding = '0' * (abs(exp) - 1)  # minus 1 for decimal point in the sci notation
+    sign = '-' if f < 0 else ''
+    if exp > 0:
+        return '{}{}{}'.format(sign, digits, zero_padding)
+
+    return '{}0.{}{}'.format(sign, zero_padding, digits)
+
+
 def parse_number(number: Union[float, int, str]) -> Tuple[int, int, int, int]:
     """Segment a number into the boolean negative indicator (which will be used to create
     the multiplier), integer, fractional, and precision
 
     Args:
         number: the number to be parsed
             e.g., '-85.1420'
@@ -27,15 +43,15 @@
         raise NotImplementedError('number must be float, int, or str')
 
     negative = math.copysign(1, float(number)) < 0
 
     if isinstance(number, int):
         return negative, abs(number), 0, 0
 
-    number = str(number)
+    number = _float_to_str(number)
 
     if '.' in number:
         integer_str, fractional_str = number.split('.')
         return (
             negative,
             abs(int(integer_str)),
             int(fractional_str),
@@ -68,15 +84,16 @@
 
         # Handle optional precision kwarg
         if precision is None or precision == inferred_precision:
             self.fractional, self.precision = inferred_fractional, inferred_precision
         else:
             if precision < inferred_precision:
                 logger.warning(
-                    f'inferred precision value is {inferred_precision}; using specified precision value of {precision}, '
+                    f'inferred precision value is {inferred_precision}; using specified '
+                    + f'precision value of {precision}, '
                     + 'which may result in data loss'
                 )
             self.fractional = self._change_power_of_ten(
                 inferred_fractional, inferred_precision, precision
             )
 
             self.precision = precision
@@ -132,17 +149,26 @@
         return False
 
     def __float__(self) -> float:
         """Provides the float representation of the PreciseNumber"""
         return self.multiplier * (self.integer + self.fractional / 10**self.precision)
 
     def __repr__(self) -> str:
-        return f'PreciseNumber(multiplier={self.multiplier}, integer={self.integer}, fractional={self.fractional}, precision={self.precision})'
+        m = f'multiplier={self.multiplier}'
+        i = f'integer={self.integer}'
+        f = f'fractional={self.fractional}'
+        p = f'precision={self.precision}'
+
+        return f'PreciseNumber({m}, {i}, {f}, {p})'
 
     def __str__(self) -> str:
         """Provides the string representation of the PreciseNumber"""
         negative_indicator = '-' if self.multiplier == -1 else ''
+        num_zeros = self.precision - len(str(self.fractional))
 
         if self.precision == 0:
             return negative_indicator + str(self.integer)
 
-        return f'{negative_indicator}{self.integer}.{"0" * (self.precision - len(str(self.fractional))) + str(self.fractional)}'
+        before_decimal = f'{negative_indicator}{self.integer}'
+        after_decimal = f'{"0" * num_zeros + str(self.fractional)}'
+
+        return f'{before_decimal}.{after_decimal}'
```

### Comparing `precisenumbers-0.0.3/tests/test_precisenumbers.py` & `precisenumbers-0.0.4/tests/test_precisenumbers.py`

 * *Files 11% similar despite different names*

```diff
@@ -155,7 +155,19 @@
 def test_precisenumber_repr():
     assert precisenumbers.PreciseNumber(1.0, precision=5).__repr__() == 'PreciseNumber(multiplier=1, integer=1, fractional=0, precision=5)'
 
 
 def test_parse_number():
     with pytest.raises(NotImplementedError):
         precisenumbers.parse_number([1, 2])
+
+
+def test_float_to_str():
+    assert precisenumbers._float_to_str(1.0) == '1.0'
+    assert precisenumbers._float_to_str(1) == '1'
+    assert precisenumbers._float_to_str(1e-07) == '0.0000001'
+    assert precisenumbers._float_to_str(1e+16) == '1000000000000000'
+
+    assert precisenumbers._float_to_str(-1.0) == '-1.0'
+    assert precisenumbers._float_to_str(-1) == '-1'
+    assert precisenumbers._float_to_str(-1e-07) == '-0.0000001'
+    assert precisenumbers._float_to_str(-1e+16) == '-1000000000000000'
```

