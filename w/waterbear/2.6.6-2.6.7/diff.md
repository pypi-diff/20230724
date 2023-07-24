# Comparing `tmp/waterbear-2.6.6-py3-none-any.whl.zip` & `tmp/waterbear-2.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9492 bytes, number of entries: 8
+Zip file size: 9849 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       54 b- defN 19-Jun-12 01:22 waterbear/__init__.py
--rw-r--r--  2.0 unx     7086 b- defN 19-Dec-11 15:21 waterbear/test_waterbear.py
--rw-r--r--  2.0 unx     7162 b- defN 20-Sep-14 13:48 waterbear/waterbear.py
--rw-r--r--  2.0 unx     1523 b- defN 20-Sep-14 13:49 waterbear-2.6.6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     9741 b- defN 20-Sep-14 13:49 waterbear-2.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Sep-14 13:49 waterbear-2.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 20-Sep-14 13:49 waterbear-2.6.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      638 b- defN 20-Sep-14 13:49 waterbear-2.6.6.dist-info/RECORD
-8 files, 26306 bytes uncompressed, 8378 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     7141 b- defN 23-Jul-23 05:52 waterbear/test_waterbear.py
+-rw-r--r--  2.0 unx     7981 b- defN 23-Jul-23 16:41 waterbear/waterbear.py
+-rw-r--r--  2.0 unx     1523 b- defN 23-Jul-24 03:22 waterbear-2.6.7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     9766 b- defN 23-Jul-24 03:22 waterbear-2.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 03:22 waterbear-2.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-24 03:22 waterbear-2.6.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      638 b- defN 23-Jul-24 03:22 waterbear-2.6.7.dist-info/RECORD
+8 files, 27205 bytes uncompressed, 8735 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: waterbear/test_waterbear.py
 Comment: 
 
 Filename: waterbear/waterbear.py
 Comment: 
 
-Filename: waterbear-2.6.6.dist-info/LICENSE.md
+Filename: waterbear-2.6.7.dist-info/LICENSE.md
 Comment: 
 
-Filename: waterbear-2.6.6.dist-info/METADATA
+Filename: waterbear-2.6.7.dist-info/METADATA
 Comment: 
 
-Filename: waterbear-2.6.6.dist-info/WHEEL
+Filename: waterbear-2.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: waterbear-2.6.6.dist-info/top_level.txt
+Filename: waterbear-2.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: waterbear-2.6.6.dist-info/RECORD
+Filename: waterbear-2.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## waterbear/test_waterbear.py

```diff
@@ -60,14 +60,15 @@
     bear.not_idempotent.append('ha')
     assert bear.not_idempotent == [], 'calling attribute does NOT add new values in idempotent mode.'
 
 
 def test_dict_methods():
     bear = Bear(a=10, b=100)
     assert str(bear) == "{'a': 10, 'b': 100}"
+    assert str(bear.__dict__) == "{'a': 10, 'b': 100}"
     assert dir(bear) == ['a', 'b']
 
 
 def test_dict_comparison():
     bear = Bear()
     assert not {}, 'empty dictionary are treated as False value.'
     assert not bear, 'bear should be treated as False value too!'
```

## waterbear/waterbear.py

```diff
@@ -1,19 +1,29 @@
 import logging
 
 from copy import deepcopy
 
 
-class Bear():
+class Bear:
+    """
+    Bear automatically injects the key value pairs into the class at construction.
+
+    Note: Bear does NOT automatically inject attributes of the current name space
+        into the dictionary. This ia  good thing. To use the object as a namespace,
+        use params-proto's ParamsProto or PrefixProto instead.
+
+    - Ge
+    """
     def __init_subclass__(cls, **kwargs):
         # intercept the kwargs in the init_subclass call
         super().__init_subclass__()
 
     def __init__(self, **d):
-        """Features:
+        """
+        Features:
 
         0. Take in a list of keyword arguments in constructor, and assign them as attributes
         1. Correctly handles `dir` command, so shows correct auto-completion in editors.
         2. Correctly handles `vars` command, and returns a dictionary version of self.
 
         default: if d['new_key'] is queried, the default value is inserted into the dictionary.
 
@@ -43,16 +53,28 @@
             del d['__idempotent_get']
         else:
             self.__idempotent_get = False  # the default value of idempotent_get is False.
         # keep the input as a reference. Destructuring breaks this reference.
         self.__d = d
 
     def __getattribute__(self, item):
-        # Note: Because we make a `__d` call, we need to filter for recursion.
-        # Note: Always check the dictionary first.
+        """
+        Waterbear get attribute method. Deligate to system default if
+        the attribute is not found in the local dictionary.
+
+        Child classes need to escape things like static methods, properties etc.
+        in the Bear constructor, so that they are not returned as is.
+
+        1. First try to detect if method is private
+        2. then tries to retrieve it from the local dict
+        3. If that fails, try using super method again.
+
+        note-1: Because we make a `__d` call, we need to filter for recursion.
+        note-2: Always check the dictionary first.
+        """
         if item.startswith("__") or item.startswith("_Bear"):
             return super(Bear, self).__getattribute__(item)
         try:
             value = self.__d[item]
             if type(value) == dict and self.__is_recursive:
                 bear = Bear()
                 bear.__d = value
```

## Comparing `waterbear-2.6.6.dist-info/LICENSE.md` & `waterbear-2.6.7.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `waterbear-2.6.6.dist-info/METADATA` & `waterbear-2.6.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: waterbear
-Version: 2.6.6
+Version: 2.6.7
 Summary: A utility that makes it easy to use dot notation with python dictionaries
 Home-page: https://github.com/episodeyang/waterbear
 Author: Ge Yang
 Author-email: yangge1987@gmail.com
 License: UNKNOWN
 Keywords: waterbear,dict,dot-notation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.md
 
 .. figure:: https://github.com/episodeyang/waterbear/blob/master/figures/waterbear_resized.jpg?raw=true
    :width: 355px
    :height: 266px
    :scale: 50%
    :alt: waterbear_is_a_bear
```

## Comparing `waterbear-2.6.6.dist-info/RECORD` & `waterbear-2.6.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 waterbear/__init__.py,sha256=Umz9q3qHqT9Fk0KpcBajRH3CkXQB5CWe96tS-AHAgI0,54
-waterbear/test_waterbear.py,sha256=LKwQ_EtPsuUKt9A1lEzcxh1DptPx7XDQa3EDMwxL87c,7086
-waterbear/waterbear.py,sha256=F172Y7PhbtqQW-sTaWPebKnNgo3r03-R7V7QnIMybIo,7162
-waterbear-2.6.6.dist-info/LICENSE.md,sha256=ilFqTGUJLufdVP1pgSIcGlf0pmEbfyXoiqNoCQT86ds,1523
-waterbear-2.6.6.dist-info/METADATA,sha256=xUArUWCdUzrVu90L3stQbrFZlW9WFIOjznbH3aS23c4,9741
-waterbear-2.6.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-waterbear-2.6.6.dist-info/top_level.txt,sha256=OFQUE5VwvsetMVfuro3ourO6Ek8Z_ucEFX7EHyizeBM,10
-waterbear-2.6.6.dist-info/RECORD,,
+waterbear/test_waterbear.py,sha256=9AulvfLB1VNNoe8cM-IjuLEdX_3b25FmrwAy0PMnUSw,7141
+waterbear/waterbear.py,sha256=XZUSwFpK9-W9utBFUsEljPwHfnm60EzpxvHW2cPWWcw,7981
+waterbear-2.6.7.dist-info/LICENSE.md,sha256=ilFqTGUJLufdVP1pgSIcGlf0pmEbfyXoiqNoCQT86ds,1523
+waterbear-2.6.7.dist-info/METADATA,sha256=tk8u-2duiaWRjveV3OvZAKGFW9qQG9F97iGZYwx9Ml8,9766
+waterbear-2.6.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+waterbear-2.6.7.dist-info/top_level.txt,sha256=OFQUE5VwvsetMVfuro3ourO6Ek8Z_ucEFX7EHyizeBM,10
+waterbear-2.6.7.dist-info/RECORD,,
```

