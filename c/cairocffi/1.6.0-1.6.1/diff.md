# Comparing `tmp/cairocffi-1.6.0.tar.gz` & `tmp/cairocffi-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cairocffi-1.6.0.tar", last modified: Mon Jun 12 08:13:48 2023, max compression
+gzip compressed data, was "cairocffi-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cairocffi-1.6.0.tar` & `cairocffi-1.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1534 2020-10-29 21:18:23.141438 cairocffi-1.6.0/LICENSE
--rw-r--r--   0        0        0       22 2023-03-25 08:13:29.041670 cairocffi-1.6.0/MANIFEST.in
--rw-r--r--   0        0        0     8872 2023-06-12 08:09:43.992397 cairocffi-1.6.0/NEWS.rst
--rw-r--r--   0        0        0     1612 2023-03-25 08:13:29.048670 cairocffi-1.6.0/README.rst
--rw-r--r--   0        0        0     4023 2023-06-12 08:00:06.780849 cairocffi-1.6.0/cairocffi/__init__.py
--rw-r--r--   0        0        0    55889 2023-03-25 08:13:29.050670 cairocffi-1.6.0/cairocffi/constants.py
--rw-r--r--   0        0        0    84791 2022-10-03 08:01:47.993857 cairocffi-1.6.0/cairocffi/context.py
--rw-r--r--   0        0        0     3571 2023-06-12 07:59:33.181255 cairocffi-1.6.0/cairocffi/ffi.py
--rw-r--r--   0        0        0    19493 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/fonts.py
--rw-r--r--   0        0        0     8064 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/matrix.py
--rw-r--r--   0        0        0    12978 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/patterns.py
--rw-r--r--   0        0        0     7256 2023-06-12 07:59:33.181255 cairocffi-1.6.0/cairocffi/pixbuf.py
--rw-r--r--   0        0        0    57999 2023-03-25 08:13:29.052671 cairocffi-1.6.0/cairocffi/surfaces.py
--rw-r--r--   0        0        0    46873 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_cairo.py
--rw-r--r--   0        0        0      405 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_numpy.py
--rw-r--r--   0        0        0     2398 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_pixbuf.py
--rw-r--r--   0        0        0     6338 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_xcb.py
--rw-r--r--   0        0        0     2023 2023-04-14 22:15:06.224429 cairocffi-1.6.0/cairocffi/xcb.py
--rw-r--r--   0        0        0    21215 2020-10-29 21:18:23.143438 cairocffi-1.6.0/docs/api.rst
--rw-r--r--   0        0        0     4335 2020-10-29 21:18:23.143438 cairocffi-1.6.0/docs/cffi_api.rst
--rw-r--r--   0        0        0       54 2023-03-11 07:55:03.041563 cairocffi-1.6.0/docs/changelog.rst
--rw-r--r--   0        0        0      555 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/conf.py
--rw-r--r--   0        0        0      139 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/index.rst
--rw-r--r--   0        0        0     5446 2021-10-04 10:06:33.130910 cairocffi-1.6.0/docs/overview.rst
--rw-r--r--   0        0        0     1234 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/pixbuf.rst
--rw-r--r--   0        0        0      273 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/xcb.rst
--rw-r--r--   0        0        0     1936 2023-06-12 07:59:33.182255 cairocffi-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      777 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/cairo_coverage.py
--rw-r--r--   0        0        0     1390 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/cairocffi_to_pycairo.py
--rw-r--r--   0        0        0      756 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/compare_pycairo.py
--rw-r--r--   0        0        0     3001 2023-03-25 08:13:29.052671 cairocffi-1.6.0/utils/mkconstants.py
--rw-r--r--   0        0        0     1853 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/pango_example.py
--rw-r--r--   0        0        0     1056 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/pycairo_to_cairocffi.py
--rw-r--r--   0        0        0      999 2023-03-11 07:55:03.041563 cairocffi-1.6.0/utils/tests.py
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 cairocffi-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1534 2020-10-29 21:18:23.141438 cairocffi-1.6.1/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-25 08:13:29.041670 cairocffi-1.6.1/MANIFEST.in
+-rw-r--r--   0        0        0     8998 2023-07-24 08:29:41.938151 cairocffi-1.6.1/NEWS.rst
+-rw-r--r--   0        0        0     1624 2023-06-12 13:34:52.103553 cairocffi-1.6.1/README.rst
+-rw-r--r--   0        0        0     4023 2023-07-24 08:26:28.109928 cairocffi-1.6.1/cairocffi/__init__.py
+-rw-r--r--   0        0        0    55889 2023-03-25 08:13:29.050670 cairocffi-1.6.1/cairocffi/constants.py
+-rw-r--r--   0        0        0    84444 2023-06-12 13:31:26.008613 cairocffi-1.6.1/cairocffi/context.py
+-rw-r--r--   0        0        0     3231 2023-07-23 08:08:07.669624 cairocffi-1.6.1/cairocffi/ffi.py
+-rw-r--r--   0        0        0    19496 2023-06-12 13:31:20.781538 cairocffi-1.6.1/cairocffi/fonts.py
+-rw-r--r--   0        0        0     8025 2023-06-12 11:29:31.080552 cairocffi-1.6.1/cairocffi/matrix.py
+-rw-r--r--   0        0        0    12969 2023-06-12 13:29:55.499320 cairocffi-1.6.1/cairocffi/patterns.py
+-rw-r--r--   0        0        0     7244 2023-06-12 13:31:03.919298 cairocffi-1.6.1/cairocffi/pixbuf.py
+-rw-r--r--   0        0        0    57784 2023-06-12 13:31:09.782381 cairocffi-1.6.1/cairocffi/surfaces.py
+-rw-r--r--   0        0        0    46867 2023-06-12 13:37:13.806570 cairocffi-1.6.1/cairocffi/test_cairo.py
+-rw-r--r--   0        0        0      405 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_numpy.py
+-rw-r--r--   0        0        0     2398 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_pixbuf.py
+-rw-r--r--   0        0        0     6338 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_xcb.py
+-rw-r--r--   0        0        0     2011 2023-06-12 10:21:04.001054 cairocffi-1.6.1/cairocffi/xcb.py
+-rw-r--r--   0        0        0    21443 2023-06-12 11:34:13.698751 cairocffi-1.6.1/docs/api.rst
+-rw-r--r--   0        0        0     4313 2023-06-12 13:29:47.039199 cairocffi-1.6.1/docs/cffi_api.rst
+-rw-r--r--   0        0        0       54 2023-03-11 07:55:03.041563 cairocffi-1.6.1/docs/changelog.rst
+-rw-r--r--   0        0        0     2792 2023-07-13 15:47:16.814348 cairocffi-1.6.1/docs/conf.py
+-rw-r--r--   0        0        0      169 2023-06-12 10:49:57.878672 cairocffi-1.6.1/docs/index.rst
+-rw-r--r--   0        0        0     5440 2023-06-12 13:32:34.458590 cairocffi-1.6.1/docs/overview.rst
+-rw-r--r--   0        0        0     1234 2020-10-29 21:18:23.144438 cairocffi-1.6.1/docs/pixbuf.rst
+-rw-r--r--   0        0        0      273 2020-10-29 21:18:23.144438 cairocffi-1.6.1/docs/xcb.rst
+-rw-r--r--   0        0        0     1881 2023-07-23 08:09:25.495449 cairocffi-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      777 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/cairo_coverage.py
+-rw-r--r--   0        0        0     1390 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/cairocffi_to_pycairo.py
+-rw-r--r--   0        0        0      756 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/compare_pycairo.py
+-rw-r--r--   0        0        0     3001 2023-03-25 08:13:29.052671 cairocffi-1.6.1/utils/mkconstants.py
+-rw-r--r--   0        0        0     1853 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/pango_example.py
+-rw-r--r--   0        0        0     1056 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/pycairo_to_cairocffi.py
+-rw-r--r--   0        0        0      999 2023-03-11 07:55:03.041563 cairocffi-1.6.1/utils/tests.py
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 cairocffi-1.6.1/PKG-INFO
```

### Comparing `cairocffi-1.6.0/LICENSE` & `cairocffi-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/NEWS.rst` & `cairocffi-1.6.1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 cairocffi changelog
 -------------------
 
 
+Version 1.6.1
+.............
+
+Released on 2023-07-24
+
+* `#217 <https://github.com/Kozea/cairocffi/issues/217>`_:
+  Repair installation with PyInstaller
+
+
 Version 1.6.0
 .............
 
 Released on 2023-06-12
 
 **This version uses a new CFFI mode that may break your program.**
 
@@ -253,28 +262,28 @@
 Version 0.5.1
 .............
 
 Released on 2013-07-16.
 
 Fix `#15 <https://github.com/SimonSapin/cairocffi/pull/15>`_:
 Work around `CFFI bug #92 <https://bitbucket.org/cffi/cffi/issue/92/>`_
-that caused memory leaks when file-like :obj:`target` objects
+that caused memory leaks when file-like ``target`` objects
 are passed to :meth:`Surface.write_to_png`, :class:`PDFSurface`,
 :class:`PSSurface` and :class:`SVGSurface`.
 
 
 Version 0.5
 ...........
 
 Released on 2013-06-20.
 
 Change :func:`~cairocffi.pixbuf.decode_to_image_surface`
 to raise a specific :exc:`~cairocffi.pixbuf.ImageLoadingError` exception
-instead of a generic :exc:`~exceptions.ValueError`.
-This new exception type inherits from :exc:`~exceptions.ValueError`.
+instead of a generic :exc:`ValueError`.
+This new exception type inherits from :exc:`ValueError`.
 
 
 Version 0.4.3
 .............
 
 Released on 2013-05-27.
```

### Comparing `cairocffi-1.6.0/README.rst` & `cairocffi-1.6.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 .. _CFFI: https://cffi.readthedocs.org/
 .. _Pycairo: https://pycairo.readthedocs.io/
 .. _cairo: http://cairographics.org/
 .. _GDK-PixBuf: https://gitlab.gnome.org/GNOME/gdk-pixbuf
 
 * Free software: BSD license
 * For Python 3.7+, tested on CPython and PyPy
-* Documentation: https://cairocffi.readthedocs.io
-* Changelog: https://cairocffi.readthedocs.io/en/stable/changelog.html
+* Documentation: https://doc.courtbouillon.org/cairocffi/
+* Changelog: https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 * Code, issues, tests: https://github.com/Kozea/cairocffi
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
 * API partially compatible with Pycairo.
 * Works with any version of cairo.
```

### Comparing `cairocffi-1.6.0/cairocffi/__init__.py` & `cairocffi-1.6.1/cairocffi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import sys
 from ctypes.util import find_library
 
 from . import constants
 from .ffi import ffi
 
-VERSION = __version__ = '1.6.0'
+VERSION = __version__ = '1.6.1'
 # supported version of cairo, used to be pycairo version too:
 version = '1.17.2'
 version_info = (1, 17, 2)
 
 
 def dlopen(ffi, library_names, filenames):
     """Try various names for the same library, for different platforms."""
```

### Comparing `cairocffi-1.6.0/cairocffi/constants.py` & `cairocffi-1.6.1/cairocffi/constants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/cairocffi/context.py` & `cairocffi-1.6.1/cairocffi/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self._check_status()
 
     def _check_status(self):
         _check_status(cairo.cairo_status(self._pointer))
 
     @classmethod
     def _from_pointer(cls, pointer, incref):
-        """Wrap an existing :c:type:`cairo_t *` cdata pointer.
+        """Wrap an existing ``cairo_t *`` cdata pointer.
 
         :type incref: bool
         :param incref:
             Whether increase the :ref:`reference count <refcounting>` now.
         :return:
             A new :class:`Context` instance.
 
@@ -202,15 +202,15 @@
         as opaque within the group,  (so that they occlude each other),
         and then blend the result with translucence onto the destination.
 
         Groups can be nested arbitrarily deep
         by making balanced calls to :meth:`push_group` / :meth:`pop_group`.
         Each call pushes / pops the new target group onto / from a stack.
 
-        The :meth:`group` method calls :meth:`save`
+        The :meth:`push_group` method calls :meth:`save`
         so that any changes to the graphics state
         will not be visible outside the group,
         (the pop_group methods call :meth:`restore`).
 
         By default the intermediate group will have
         a content type of :obj:`COLOR_ALPHA <CONTENT_COLOR_ALPHA>`.
         Other content types can be chosen for the group
@@ -237,15 +237,15 @@
         known as a group.
         The redirection lasts until the group is completed
         by a call to :meth:`pop_group` or :meth:`pop_group_to_source`.
         These calls provide the result of any drawing
         to the group as a pattern,
         (either as an explicit object, or set as the source pattern).
 
-        The group will have a content type of :obj:`content`.
+        The group will have a content type of ``content``.
         The ability to control this content  type
         is the only distinction between this method and :meth:`push_group`
         which you should see for a more detailed description
         of group rendering.
 
         :param content: A :ref:`CONTENT` string.
 
@@ -338,19 +338,19 @@
         cairo.cairo_set_source_rgb(self._pointer, red, green, blue)
         self._check_status()
 
     def set_source_surface(self, surface, x=0, y=0):
         """This is a convenience method for creating a pattern from surface
         and setting it as the source in this context with :meth:`set_source`.
 
-        The :obj:`x` and :obj:`y` parameters give the user-space coordinate
+        The ``x`` and ``y`` parameters give the user-space coordinate
         at which the surface origin should appear.
         (The surface origin is its upper-left corner
         before any transformation has been applied.)
-        The :obj:`x` and :obj:`y` parameters are negated
+        The ``x`` and ``y`` parameters are negated
         and then set as translation values in the pattern matrix.
 
         Other than the initial translation pattern matrix, as described above,
         all other pattern attributes, (such as its extend mode),
         are set to the default values as in :class:`SurfacePattern`.
         The resulting pattern can be queried with :meth:`get_source`
         so that these attributes can be modified if desired,
@@ -364,15 +364,15 @@
         :type y: float
 
         """
         cairo.cairo_set_source_surface(self._pointer, surface._pointer, x, y)
         self._check_status()
 
     def set_source(self, source):
-        """Sets the source pattern within this context to :obj:`source`.
+        """Sets the source pattern within this context to ``source``.
         This pattern will then be used for any subsequent drawing operation
         until a new source pattern is set.
 
         .. note::
 
             The pattern's transformation matrix will be locked
             to the user space in effect at the time of :meth:`set_source`.
@@ -429,29 +429,29 @@
         return cairo.cairo_get_antialias(self._pointer)
 
     def set_dash(self, dashes, offset=0):
         """Sets the dash pattern to be used by :meth:`stroke`.
         A dash pattern is specified by dashes, a list of positive values.
         Each value provides the length of alternate "on" and "off"
         portions of the stroke.
-        :obj:`offset` specifies an offset into the pattern
+        ``offset`` specifies an offset into the pattern
         at which the stroke begins.
 
         Each "on" segment will have caps applied
         as if the segment were a separate sub-path.
         In particular, it is valid to use an "on" length of 0
         with :obj:`LINE_CAP_ROUND` or :obj:`LINE_CAP_SQUARE`
         in order to distributed dots or squares along a path.
 
         Note: The length values are in user-space units
         as evaluated at the time of stroking.
         This is not necessarily the same as the user space
         at the time of :meth:`set_dash`.
 
-        If :obj:`dashes` is empty dashing is disabled.
+        If ``dashes`` is empty dashing is disabled.
         If it is of length 1 a symmetric pattern is assumed
         with alternating on and off portions of the size specified
         by the single value.
 
         :param dashes:
             A list of floats specifying alternate lengths
             of on and off stroke portions.
@@ -470,15 +470,15 @@
         self._check_status()
 
     def get_dash(self):
         """Return the current dash pattern.
 
         :returns:
             A ``(dashes, offset)`` tuple of a list and a float.
-            :obj:`dashes` is a list of floats,
+            ``dashes`` is a list of floats,
             empty if no dashing is in effect.
 
         """
         dashes = ffi.new('double[]', cairo.cairo_get_dash_count(self._pointer))
         offset = ffi.new('double *')
         cairo.cairo_get_dash(self._pointer, dashes, offset)
         self._check_status()
@@ -508,15 +508,15 @@
         """Return the current :ref:`FILL_RULE` string."""
         return cairo.cairo_get_fill_rule(self._pointer)
 
     def set_line_cap(self, line_cap):
         """Set the current :ref:`LINE_CAP` within the cairo context.
         As with the other stroke parameters,
         the current line cap style is examined by
-        :meth:`stroke`, :meth:`stroke_extents`, and :meth:`stroke_to_path`,
+        :meth:`stroke` and :meth:`stroke_extents`,
         but does not have any effect during path construction.
 
         The default line cap is :obj:`BUTT <LINE_CAP_BUTT>`.
 
         :param line_cap: A :ref:`LINE_CAP` string.
 
         """
@@ -527,15 +527,15 @@
         """Return the current :ref:`LINE_CAP` string."""
         return cairo.cairo_get_line_cap(self._pointer)
 
     def set_line_join(self, line_join):
         """Set the current :ref:`LINE_JOIN` within the cairo context.
         As with the other stroke parameters,
         the current line cap style is examined by
-        :meth:`stroke`, :meth:`stroke_extents`, and :meth:`stroke_to_path`,
+        :meth:`stroke` and :meth:`stroke_extents`,
         but does not have any effect during path construction.
 
         The default line cap is :obj:`MITER <LINE_JOIN_MITER>`.
 
         :param line_join: A :ref:`LINE_JOIN` string.
 
         """
@@ -564,15 +564,15 @@
             between a call to :meth:`set_line_width`
             and the stroking operation,
             then one can just pass user-space values to :meth:`set_line_width`
             and ignore this note.
 
         As with the other stroke parameters,
         the current line cap style is examined by
-        :meth:`stroke`, :meth:`stroke_extents`, and :meth:`stroke_to_path`,
+        :meth:`stroke` and :meth:`stroke_extents`,
         but does not have any effect during path construction.
 
         The default line width value is 2.0.
 
         :type width: float
         :param width: The new line width.
 
@@ -593,15 +593,15 @@
         whether the lines should be joined with a bevel instead of a miter.
         Cairo divides the length of the miter by the line width.
         If the result is greater than the miter limit,
         the style is converted to a bevel.
 
         As with the other stroke parameters,
         the current line cap style is examined by
-        :meth:`stroke`, :meth:`stroke_extents`, and :meth:`stroke_to_path`,
+        :meth:`stroke` and :meth:`stroke_extents`,
         but does not have any effect during path construction.
 
         The default miter limit value is 10.0,
         which will convert joins with interior angles less than 11 degrees
         to bevels instead of miters.
         For reference,
         a miter limit of 2.0 makes the miter cutoff at 60 degrees,
@@ -683,19 +683,19 @@
         """
         cairo.cairo_translate(self._pointer, tx, ty)
         self._check_status()
 
     def scale(self, sx, sy=None):
         """Modifies the current transformation matrix (CTM)
         by scaling the X and Y user-space axes
-        by :obj:`sx` and :obj:`sy` respectively.
+        by ``sx`` and ``sy`` respectively.
         The scaling of the axes takes place after
         any existing transformation of user space.
 
-        If :obj:`sy` is omitted, it is the same as :obj:`sx`
+        If ``sy`` is omitted, it is the same as ``sx``
         so that scaling preserves aspect ratios.
 
         :param sx: Scale factor in the X direction.
         :param sy: Scale factor in the Y direction.
         :type sx: float
         :type sy: float
 
@@ -703,15 +703,15 @@
         if sy is None:
             sy = sx
         cairo.cairo_scale(self._pointer, sx, sy)
         self._check_status()
 
     def rotate(self, radians):
         """Modifies the current transformation matrix (CTM)
-        by rotating the user-space axes by angle :obj:`radians`.
+        by rotating the user-space axes by angle ``radians``.
         The rotation of the axes takes places
         after any existing transformation of user space.
 
         :type radians: float
         :param radians:
             Angle of rotation, in radians.
             The direction of rotation is defined such that positive angles
@@ -722,29 +722,29 @@
 
         """
         cairo.cairo_rotate(self._pointer, radians)
         self._check_status()
 
     def transform(self, matrix):
         """Modifies the current transformation matrix (CTM)
-        by applying :obj:`matrix` as an additional transformation.
+        by applying ``matrix`` as an additional transformation.
         The new transformation of user space takes place
         after any existing transformation.
 
         :param matrix:
             A transformation :class:`Matrix`
             to be applied to the user-space axes.
 
         """
         cairo.cairo_transform(self._pointer, matrix._pointer)
         self._check_status()
 
     def set_matrix(self, matrix):
         """Modifies the current transformation matrix (CTM)
-        by setting it equal to :obj:`matrix`.
+        by setting it equal to ``matrix``.
 
         :param matrix:
             A transformation :class:`Matrix` from user space to device space.
 
         """
         cairo.cairo_set_matrix(self._pointer, matrix._pointer)
         self._check_status()
@@ -869,16 +869,15 @@
         :meth:`rel_move_to`,
         :meth:`rel_line_to`,
         :meth:`rel_curve_to`,
         :meth:`arc`,
         :meth:`arc_negative`,
         :meth:`rectangle`,
         :meth:`text_path`,
-        :meth:`glyph_path`,
-        :meth:`stroke_to_path`.
+        :meth:`glyph_path`.
 
         Some methods use and alter the current point
         but do not otherwise change current path:
         :meth:`show_text`,
         :meth:`show_glyphs`,
         :meth:`show_text_glyphs`.
 
@@ -1021,20 +1020,20 @@
         """
         cairo.cairo_rectangle(self._pointer, x, y, width, height)
         self._check_status()
 
     def arc(self, xc, yc, radius, angle1, angle2):
         """Adds a circular arc of the given radius to the current path.
         The arc is centered at ``(xc, yc)``,
-        begins at :obj:`angle1`
+        begins at ``angle1``
         and proceeds in the direction of increasing angles
-        to end at :obj:`angle2`.
-        If :obj:`angle2` is less than :obj:`angle1`
+        to end at ``angle2``.
+        If ``angle2`` is less than ``angle1``
         it will be progressively increased by ``2 * pi``
-        until it is greater than :obj:`angle1`.
+        until it is greater than ``angle1``.
 
         If there is a current point,
         an initial line segment will be added to the path
         to connect the current point to the beginning of the arc.
         If this initial line is undesired,
         it can be avoided by calling :meth:`new_sub_path`
         before calling :meth:`arc`.
@@ -1082,20 +1081,20 @@
         """
         cairo.cairo_arc(self._pointer, xc, yc, radius, angle1, angle2)
         self._check_status()
 
     def arc_negative(self, xc, yc, radius, angle1, angle2):
         """Adds a circular arc of the given radius to the current path.
         The arc is centered at ``(xc, yc)``,
-        begins at :obj:`angle1`
+        begins at ``angle1``
         and proceeds in the direction of decreasing angles
-        to end at :obj:`angle2`.
-        If :obj:`angle2` is greater than :obj:`angle1`
+        to end at ``angle2``.
+        If ``angle2`` is greater than ``angle1``
         it will be progressively decreased by ``2 * pi``
-        until it is greater than :obj:`angle1`.
+        until it is greater than ``angle1``.
 
         See :meth:`arc` for more details.
         This method differs only in
         the direction of the arc between the two angles.
 
         :param xc: X position of the center of the arc.
         :param yc: Y position of the center of the arc.
@@ -1284,15 +1283,15 @@
         """
         path = cairo.cairo_copy_path_flat(self._pointer)
         result = list(_iter_path(path))
         cairo.cairo_path_destroy(path)
         return result
 
     def append_path(self, path):
-        """Append :obj:`path` onto the current path.
+        """Append ``path`` onto the current path.
         The path may be either the return value from one of :meth:`copy_path`
         or :meth:`copy_path_flat` or it may be constructed manually.
 
         :param path:
             An iterable of tuples
             in the same format as returned by :meth:`copy_path`.
 
@@ -1354,39 +1353,39 @@
         self._check_status()
 
     def paint_with_alpha(self, alpha):
         """A drawing operator that paints the current source everywhere
         within the current clip region
         using a mask of constant alpha value alpha.
         The effect is similar to :meth:`paint`,
-        but the drawing is faded out using the :obj:`alpha` value.
+        but the drawing is faded out using the ``alpha`` value.
 
         :type alpha: float
         :param alpha: Alpha value, between 0 (transparent) and 1 (opaque).
 
         """
         cairo.cairo_paint_with_alpha(self._pointer, alpha)
         self._check_status()
 
     def mask(self, pattern):
         """A drawing operator that paints the current source
-        using the alpha channel of :obj:`pattern` as a mask.
-        (Opaque areas of :obj:`pattern` are painted with the source,
+        using the alpha channel of ``pattern`` as a mask.
+        (Opaque areas of ``pattern`` are painted with the source,
         transparent areas are not painted.)
 
         :param pattern: A :class:`Pattern` object.
 
         """
         cairo.cairo_mask(self._pointer, pattern._pointer)
         self._check_status()
 
     def mask_surface(self, surface, surface_x=0, surface_y=0):
         """A drawing operator that paints the current source
-        using the alpha channel of :obj:`surface` as a mask.
-        (Opaque areas of :obj:`surface` are painted with the source,
+        using the alpha channel of ``surface`` as a mask.
+        (Opaque areas of ``surface`` are painted with the source,
         transparent areas are not painted.)
 
         :param pattern: A :class:`Surface` object.
         :param surface_x: X coordinate at which to place the origin of surface.
         :param surface_y: Y coordinate at which to place the origin of surface.
         :type surface_x: float
         :type surface_y: float
@@ -1748,15 +1747,15 @@
 
         """
         cairo.cairo_select_font_face(
             self._pointer, _encode_string(family), slant, weight)
         self._check_status()
 
     def set_font_face(self, font_face):
-        """Replaces the current font face with :obj:`font_face`.
+        """Replaces the current font face with ``font_face``.
 
         :param font_face:
             A :class:`FontFace` object,
             or :obj:`None` to restore the default font.
 
         """
         font_face = font_face._pointer if font_face is not None else ffi.NULL
@@ -1771,15 +1770,15 @@
             wrapping an existing cairo object.
 
         """
         return FontFace._from_pointer(
             cairo.cairo_get_font_face(self._pointer), incref=True)
 
     def set_font_size(self, size):
-        """Sets the current font matrix to a scale by a factor of :obj:`size`,
+        """Sets the current font matrix to a scale by a factor of ``size``,
         replacing any font matrix previously set with :meth:`set_font_size`
         or :meth:`set_font_matrix`.
         This results in a font size of size user space units.
         (More precisely, this matrix will result in the font's
         em-square being a size by size square in user space.)
 
         If text is drawn without a call to :meth:`set_font_size`,
@@ -1790,15 +1789,15 @@
         :type size: float
 
         """
         cairo.cairo_set_font_size(self._pointer, size)
         self._check_status()
 
     def set_font_matrix(self, matrix):
-        """Sets the current font matrix to :obj:`matrix`.
+        """Sets the current font matrix to ``matrix``.
         The font matrix gives a transformation
         from the design space of the font
         (in this space, the em-square is 1 unit by 1 unit)
         to user space.
         Normally, a simple scale is used (see :meth:`set_font_size`),
         but a more complex font matrix can be used
         to shear the font or stretch it unequally along the two axes
@@ -1847,17 +1846,17 @@
         """
         font_options = FontOptions()
         cairo.cairo_get_font_options(self._pointer, font_options._pointer)
         return font_options
 
     def set_scaled_font(self, scaled_font):
         """Replaces the current font face, font matrix, and font options
-        with those of :obj:`scaled_font`.
+        with those of ``scaled_font``.
         Except for some translation, the current CTM of the context
-        should be the same as that of the :obj:`scaled_font`,
+        should be the same as that of the ``scaled_font``,
         which can be accessed using :meth:`ScaledFont.get_ctm`.
 
         :param scaled_font: A :class:`ScaledFont` object.
 
         """
         cairo.cairo_set_scaled_font(self._pointer, scaled_font._pointer)
         self._check_status()
@@ -1888,39 +1887,39 @@
         of the transformation matrix),
         but otherwise will remain unchanged.
 
         :returns:
             A ``(ascent, descent, height, max_x_advance, max_y_advance)``
             tuple of floats.
 
-        :obj:`ascent`
+        ``ascent``
             The distance that the font extends above the baseline.
             Note that this is not always exactly equal to
             the maximum of the extents of all the glyphs in the font,
             but rather is picked to express the font designer's intent
             as to how the font should align with elements above it.
-        :obj:`descent`
+        ``descent``
             The distance that the font extends below the baseline.
             This value is positive for typical fonts
             that include portions below the baseline.
             Note that this is not always exactly equal
             to the maximum of the extents of all the glyphs in the font,
             but rather is picked to express the font designer's intent
             as to how the font should align with elements below it.
-        :obj:`height`
+        ``height``
             The recommended vertical distance between baselines
             when setting consecutive lines of text with the font.
             This is greater than ``ascent + descent``
             by a quantity known as the line spacing or external leading.
             When space is at a premium, most fonts can be set
             with only a distance of ``ascent + descent`` between lines.
-        :obj:`max_x_advance`
+        ``max_x_advance``
             The maximum distance in the X direction
             that the origin is advanced for any glyph in the font.
-        :obj:`max_y_advance`
+        ``max_y_advance``
             The maximum distance in the Y direction
             that the origin is advanced for any glyph in the font.
             This will be zero for normal fonts used for horizontal writing.
             (The scripts of East Asia are sometimes written vertically.)
 
         """
         extents = ffi.new('cairo_font_extents_t *')
@@ -1938,20 +1937,20 @@
 
     def text_extents(self, text):
         """Returns the extents for a string of text.
 
         The extents describe a user-space rectangle
         that encloses the "inked" portion of the text,
         (as it would be drawn by :meth:`show_text`).
-        Additionally, the :obj:`x_advance` and :obj:`y_advance` values
+        Additionally, the ``x_advance`` and ``y_advance`` values
         indicate the amount by which the current point would be advanced
         by :meth:`show_text`.
 
         Note that whitespace characters do not directly contribute
-        to the size of the rectangle (:obj:`width` and :obj:`height`).
+        to the size of the rectangle (``width`` and ``height``).
         They do contribute indirectly by changing the position
         of non-whitespace characters.
         In particular, trailing whitespace characters are likely
         to not affect the size of the rectangle,
         though they will affect the x_advance and y_advance values.
 
         Because text extents are in user-space coordinates,
@@ -1966,36 +1965,36 @@
         but otherwise will remain unchanged.
 
         :param text: The text to measure, as an Unicode or UTF-8 string.
         :returns:
             A ``(x_bearing, y_bearing, width, height, x_advance, y_advance)``
             tuple of floats.
 
-        :obj:`x_bearing`
+        ``x_bearing``
             The horizontal distance
             from the origin to the leftmost part of the glyphs as drawn.
             Positive if the glyphs lie entirely to the right of the origin.
 
-        :obj:`y_bearing`
+        ``y_bearing``
             The vertical distance
             from the origin to the topmost part of the glyphs as drawn.
             Positive only if the glyphs lie completely below the origin;
             will usually be negative.
 
-        :obj:`width`
+        ``width``
             Width of the glyphs as drawn.
 
-        :obj:`height`
+        ``height``
             Height of the glyphs as drawn.
 
-        :obj:`x_advance`
+        ``x_advance``
             Distance to advance in the X direction
             after drawing these glyphs.
 
-        :obj:`y_advance`
+        ``y_advance``
             Distance to advance in the Y direction
             after drawing these glyphs.
             Will typically be zero except for vertical text layout
             as found in East-Asian languages.
 
         """
         extents = ffi.new('cairo_text_extents_t *')
@@ -2010,15 +2009,15 @@
 
     def glyph_extents(self, glyphs):
         """Returns the extents for a list of glyphs.
 
         The extents describe a user-space rectangle
         that encloses the "inked" portion of the glyphs,
         (as it would be drawn by :meth:`show_glyphs`).
-        Additionally, the :obj:`x_advance` and :obj:`y_advance` values
+        Additionally, the ``x_advance`` and ``y_advance`` values
         indicate the amount by which the current point would be advanced
         by :meth:`show_glyphs`.
 
         :param glyphs:
             A list of glyphs.
             See :meth:`show_text_glyphs` for the data structure.
         :returns:
@@ -2096,63 +2095,63 @@
         """This operation has rendering effects similar to :meth:`show_glyphs`
         but, if the target surface supports it
         (see :meth:`Surface.has_show_text_glyphs`),
         uses the provided text and cluster mapping
         to embed the text for the glyphs shown in the output.
         If the target does not support the extended attributes,
         this method acts like the basic :meth:`show_glyphs`
-        as if it had been passed :obj:`glyphs`.
+        as if it had been passed ``glyphs``.
 
-        The mapping between :obj:`text` and :obj:`glyphs`
+        The mapping between ``text`` and ``glyphs``
         is provided by an list of clusters.
         Each cluster covers a number of UTF-8 text bytes and glyphs,
         and neighboring clusters cover neighboring areas
-        of :obj:`text` and :obj:`glyphs`.
-        The clusters should collectively cover :obj:`text` and :obj:`glyphs`
+        of ``text`` and ``glyphs``.
+        The clusters should collectively cover ``text`` and ``glyphs``
         in entirety.
 
         :param text:
             The text to show, as an Unicode or UTF-8 string.
-            Because of how :obj:`clusters` work,
+            Because of how ``cluster`` work,
             using UTF-8 bytes might be more convenient.
         :param glyphs:
             A list of glyphs.
             Each glyph is a ``(glyph_id, x, y)`` tuple.
-            :obj:`glyph_id` is an opaque integer.
+            ``glyph_id`` is an opaque integer.
             Its exact interpretation depends on the font technology being used.
-            :obj:`x` and :obj:`y` are the float offsets
+            ``x`` and ``y`` are the float offsets
             in the X and Y direction
             between the origin used for drawing or measuring the string
             and the origin of this glyph.
             Note that the offsets are not cumulative.
             When drawing or measuring text,
             each glyph is individually positioned
             with respect to the overall origin.
         :param clusters:
             A list of clusters.
             A text cluster is a minimal mapping of some glyphs
             corresponding to some UTF-8 text,
             represented as a ``(num_bytes, num_glyphs)`` tuple of integers,
             the number of UTF-8 bytes and glyphs covered by the cluster.
             For a cluster to be valid,
-            both :obj:`num_bytes` and :obj:`num_glyphs` should be non-negative,
+            both ``num_bytes`` and ``num_glyphs`` should be non-negative,
             and at least one should be non-zero.
             Note that clusters with zero glyphs
             are not as well supported as normal clusters.
             For example, PDF rendering applications
             typically ignore those clusters when PDF text is being selected.
         :type cluster_flags: int
         :param cluster_flags:
             Flags (as a bit field) for the cluster mapping.
             The first cluster always covers bytes
-            from the beginning of :obj:`text`.
-            If :obj:`cluster_flags` does not have
+            from the beginning of ``text``.
+            If ``cluster_flags`` does not have
             the :obj:`TEXT_CLUSTER_FLAG_BACKWARD` flag set,
-            the first cluster also covers the beginning of :obj:`glyphs`,
-            otherwise it covers the end of the :obj:`glyphs` list
+            the first cluster also covers the beginning of ``glyphs``,
+            otherwise it covers the end of the ``glyphs`` list
             and following clusters move backward.
 
         """
         glyphs = ffi.new('cairo_glyph_t[]', glyphs)
         clusters = ffi.new('cairo_text_cluster_t[]', clusters)
         cairo.cairo_show_text_glyphs(
             self._pointer, _encode_string(text), -1,
```

### Comparing `cairocffi-1.6.0/cairocffi/ffi.py` & `cairocffi-1.6.1/cairocffi/ffi.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,17 @@
     Build the cffi bindings
 
     :copyright: Copyright 2013-2019 by Simon Sapin
     :license: BSD, see LICENSE for details.
 
 """
 
-from importlib.util import module_from_spec, spec_from_file_location
-from pathlib import Path
-
 from cffi import FFI
 
-# Path hack to import constants when this file is exec'd by setuptools
-constants_spec = spec_from_file_location(
-    'constants', Path(__file__).parent.joinpath('constants.py')
-)
-constants = module_from_spec(constants_spec)
-constants_spec.loader.exec_module(constants)
+from . import constants
 
 # Primary cffi definitions
 ffi = FFI()
 ffi.cdef(constants._CAIRO_HEADERS)
 
 # include xcffib cffi definitions for cairo xcb support
 try:
```

### Comparing `cairocffi-1.6.0/cairocffi/fonts.py` & `cairocffi-1.6.1/cairocffi/fonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self._check_status()
 
     def _check_status(self):
         _check_status(cairo.cairo_font_face_status(self._pointer))
 
     @staticmethod
     def _from_pointer(pointer, incref):
-        """Wrap an existing :c:type:`cairo_font_face_t *` cdata pointer.
+        """Wrap an existing ``cairo_font_face_t *`` cdata pointer.
 
         :type incref: bool
         :param incref:
             Whether increase the :ref:`reference count <refcounting>` now.
         :return:
             A new instance of :class:`FontFace` or one of its sub-classes,
             depending on the face’s type.
@@ -141,15 +141,15 @@
         self._check_status()
 
     def _check_status(self):
         _check_status(cairo.cairo_scaled_font_status(self._pointer))
 
     @staticmethod
     def _from_pointer(pointer, incref):
-        """Wrap an existing :c:type:`cairo_scaled_font_t *` cdata pointer.
+        """Wrap an existing ``cairo_scaled_font_t *`` cdata pointer.
 
         :type incref: bool
         :param incref:
             Whether increase the :ref:`reference count <refcounting>` now.
         :return: A new :class:`ScaledFont` instance.
 
         """
@@ -243,18 +243,18 @@
             extents.max_x_advance, extents.max_y_advance)
 
     def text_extents(self, text):
         """Returns the extents for a string of text.
 
         The extents describe a user-space rectangle
         that encloses the "inked" portion of the text,
-        (as it would be drawn by :meth:`show_text`).
-        Additionally, the :obj:`x_advance` and :obj:`y_advance` values
+        (as it would be drawn by :meth:`Context.show_text`).
+        Additionally, the ``x_advance`` and ``y_advance`` values
         indicate the amount by which the current point would be advanced
-        by :meth:`show_text`.
+        by :meth:`Context.show_text`.
 
         :param text: The text to measure, as an Unicode or UTF-8 string.
         :returns:
             A ``(x_bearing, y_bearing, width, height, x_advance, y_advance)``
             tuple of floats.
             See :meth:`Context.text_extents` for details.
 
@@ -269,18 +269,18 @@
             extents.x_advance, extents.y_advance)
 
     def glyph_extents(self, glyphs):
         """Returns the extents for a list of glyphs.
 
         The extents describe a user-space rectangle
         that encloses the "inked" portion of the glyphs,
-        (as it would be drawn by :meth:`show_glyphs`).
-        Additionally, the :obj:`x_advance` and :obj:`y_advance` values
+        (as it would be drawn by :meth:`Context.show_glyphs`).
+        Additionally, the ``x_advance`` and ``y_advance`` values
         indicate the amount by which the current point would be advanced
-        by :meth:`show_glyphs`.
+        by :meth:`Context.show_glyphs`.
 
         :param glyphs:
             A list of glyphs, as returned by :meth:`text_to_glyphs`.
             Each glyph is a ``(glyph_id, x, y)`` tuple
             of an integer and two floats.
         :returns:
             A ``(x_bearing, y_bearing, width, height, x_advance, y_advance)``
@@ -314,15 +314,15 @@
         :type with_clusters: bool
         :param x: X position to place first glyph.
         :param y: Y position to place first glyph.
         :param text: The text to convert, as an Unicode or UTF-8 string.
         :param with_clusters: Whether to compute the cluster mapping.
         :returns:
             A ``(glyphs, clusters, clusters_flags)`` tuple
-            if :obj:`with_clusters` is true, otherwise just :obj:`glyphs`.
+            if ``with_clusters`` is true, otherwise just ``glyphs``.
             See :meth:`Context.show_text_glyphs` for the data structure.
 
         .. note::
 
             This method is part of
             what the cairo designers call the "toy" text API.
             It is convenient for short demos and simple programs,
@@ -367,24 +367,24 @@
 
 
 class FontOptions(object):
     """An opaque object holding all options that are used when rendering fonts.
 
     Individual features of a :class:`FontOptions`
     can be set or accessed using method
-    named :meth:`set_FEATURE_NAME` and :meth:`get_FEATURE_NAME`,
+    named ``set_FEATURE_NAME`` and ``get_FEATURE_NAME``,
     like :meth:`set_antialias` and :meth:`get_antialias`.
 
     New features may be added to :class:`FontOptions` in the future.
     For this reason, ``==``, :meth:`copy`, :meth:`merge`, and :func:`hash`
     should be used to check for equality copy,, merge,
     or compute a hash value of :class:`FontOptions` objects.
 
     :param values:
-        Call the corresponding :meth:`set_FEATURE_NAME` methods
+        Call the corresponding ``set_FEATURE_NAME`` methods
         after creating a new :class:`FontOptions`::
 
             options = FontOptions()
             options.set_antialias(cairocffi.ANTIALIAS_BEST)
             assert FontOptions(antialias=cairocffi.ANTIALIAS_BEST) == options
 
     """
@@ -405,15 +405,15 @@
         """Return a new :class:`FontOptions` with the same values."""
         cls = type(self)
         other = object.__new__(cls)
         cls._init_pointer(other, cairo.cairo_font_options_copy(self._pointer))
         return other
 
     def merge(self, other):
-        """Merges non-default options from :obj:`other`,
+        """Merges non-default options from ``other``,
         replacing existing values.
         This operation can be thought of as somewhat similar
         to compositing other onto options
         with the operation of :obj:`OVER <OPERATOR_OVER>`.
 
         """
         cairo.cairo_font_options_merge(self._pointer, other._pointer)
@@ -517,17 +517,18 @@
     def get_variations(self):
         """Gets the OpenType font variations for the font options object.
 
         See :meth:`set_variations` for details about the
         string format.
 
         :return: the font variations for the font options object. The
-        returned string belongs to the ``options`` and must not be modified.
-        It is valid until either the font options object is destroyed or the
-        font variations in this object is modified with :meth:`set_variations`.
+          returned string belongs to the ``options`` and must not be modified.
+          It is valid until either the font options object is destroyed or the
+          font variations in this object is modified with
+          :meth:`set_variations`.
 
         *New in cairo 1.16.*
 
         *New in cairocffi 0.9.*
 
         """
         variations = cairo.cairo_font_options_get_variations(self._pointer)
```

### Comparing `cairocffi-1.6.0/cairocffi/matrix.py` & `cairocffi-1.6.1/cairocffi/matrix.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, xx=1, yx=0, xy=0, yy=1, x0=0, y0=0):
         self._pointer = ffi.new('cairo_matrix_t *')
         cairo.cairo_matrix_init(self._pointer, xx, yx, xy, yy, x0, y0)
 
     @classmethod
     def init_rotate(cls, radians):
         """Return a new :class:`Matrix` for a transformation
-        that rotates by :obj:`radians`.
+        that rotates by ``radians``.
 
         :type radians: float
         :param radians:
             Angle of rotation, in radians.
             The direction of rotation is defined such that
             positive angles rotate in the direction
             from the positive X axis toward the positive Y axis.
@@ -100,41 +100,41 @@
         cairo.cairo_matrix_multiply(
             res._pointer, self._pointer, other._pointer)
         return res
 
     __mul__ = multiply
 
     def translate(self, tx, ty):
-        """Applies a translation by :obj:`tx`, :obj:`ty`
+        """Applies a translation by ``tx``, ``ty``
         to the transformation in this matrix.
 
         The effect of the new transformation is to
-        first translate the coordinates by :obj:`tx` and :obj:`ty`,
+        first translate the coordinates by ``tx`` and ``ty``,
         then apply the original transformation to the coordinates.
 
         .. note::
             This changes the matrix in-place.
 
         :param tx: Amount to translate in the X direction.
         :param ty: Amount to translate in the Y direction.
         :type tx: float
         :type ty: float
 
         """
         cairo.cairo_matrix_translate(self._pointer, tx, ty)
 
     def scale(self, sx, sy=None):
-        """Applies scaling by :obj:`sx`, :obj:`sy`
+        """Applies scaling by ``sx``, ``sy``
         to the transformation in this matrix.
 
         The effect of the new transformation is to
-        first scale the coordinates by :obj:`sx` and :obj:`sy`,
+        first scale the coordinates by ``sx`` and ``sy``,
         then apply the original transformation to the coordinates.
 
-        If :obj:`sy` is omitted, it is the same as :obj:`sx`
+        If ``sy`` is omitted, it is the same as ``sx``
         so that scaling preserves aspect ratios.
 
         .. note::
             This changes the matrix in-place.
 
         :param sx: Scale factor in the X direction.
         :param sy: Scale factor in the Y direction.
@@ -143,19 +143,19 @@
 
         """
         if sy is None:
             sy = sx
         cairo.cairo_matrix_scale(self._pointer, sx, sy)
 
     def rotate(self, radians):
-        """Applies a rotation by :obj:`radians`
+        """Applies a rotation by ``radians``
         to the transformation in this matrix.
 
         The effect of the new transformation is to
-        first rotate the coordinates by :obj:`radians`,
+        first rotate the coordinates by ``radians``,
         then apply the original transformation to the coordinates.
 
         .. note::
             This changes the matrix in-place.
 
         :type radians: float
         :param radians:
```

### Comparing `cairocffi-1.6.0/cairocffi/patterns.py` & `cairocffi-1.6.1/cairocffi/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self._check_status()
 
     def _check_status(self):
         _check_status(cairo.cairo_pattern_status(self._pointer))
 
     @staticmethod
     def _from_pointer(pointer, incref):
-        """Wrap an existing :c:type:`cairo_pattern_t *` cdata pointer.
+        """Wrap an existing ``cairo_pattern_t *`` cdata pointer.
 
         :type incref: bool
         :param incref:
             Whether increase the :ref:`reference count <refcounting>` now.
         :return:
             A new instance of :class:`Pattern` or one of its sub-classes,
             depending on the pattern’s type.
@@ -105,15 +105,15 @@
         """Return the current filter string for this pattern.
         See :ref:`FILTER` for details on each filter.
 
         """
         return cairo.cairo_pattern_get_filter(self._pointer)
 
     def set_matrix(self, matrix):
-        """Sets the pattern’s transformation matrix to :obj:`matrix`.
+        """Sets the pattern’s transformation matrix to ``matrix``.
         This matrix is a transformation from user space to pattern space.
 
         When a pattern is first created
         it always has the identity matrix for its transformation matrix,
         which means that pattern space is initially identical to user space.
 
         **Important:**
```

### Comparing `cairocffi-1.6.0/cairocffi/pixbuf.py` & `cairocffi-1.6.1/cairocffi/pixbuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     The image data is probably corrupted.
 
     """
 
 
 def handle_g_error(error, return_value):
-    """Convert a :c:type:`GError**` to a Python :exception:`ImageLoadingError`,
+    """Convert a ``GError**`` to a Python :exception:`ImageLoadingError`,
     and raise it.
 
     """
     error = error[0]
     assert bool(return_value) == (error == ffi.NULL)
     if error != ffi.NULL:
         if error.message != ffi.NULL:
@@ -61,15 +61,15 @@
         else:  # pragma: no cover
             message = 'Pixbuf error'
         glib.g_error_free(error)
         raise ImageLoadingError(message)
 
 
 class Pixbuf(object):
-    """Wrap a :c:type:`GdkPixbuf` pointer and simulate methods."""
+    """Wrap a ``GdkPixbuf`` pointer and simulate methods."""
     def __init__(self, pointer):
         gobject.g_object_ref(pointer)
         self._pointer = ffi.gc(pointer, gobject.g_object_unref)
 
     def __getattr__(self, name):
         function = getattr(gdk_pixbuf, 'gdk_pixbuf_' + name)
         return partial(function, self._pointer)
```

### Comparing `cairocffi-1.6.0/cairocffi/surfaces.py` & `cairocffi-1.6.1/cairocffi/surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     depend upon the manner of its creation.
     If cairo creates the surface and backing storage for the user,
     it will be initially cleared;
     for example, :class:`ImageSurface` and :meth:`create_similar`.
     Alternatively, if the user passes in a reference
     to some backing storage and asks cairo to wrap that in a :class:`Surface`,
     then the contents are not modified;
-    for example, :class:`ImageSurface` with a :obj:`data` argument.
+    for example, :class:`ImageSurface` with a ``data`` argument.
 
     """
     def __init__(self, pointer, target_keep_alive=None):
         self._pointer = ffi.gc(
             pointer, _keepref(cairo, cairo.cairo_surface_destroy))
         self._check_status()
         if hasattr(target_keep_alive, '__array_interface__'):
@@ -167,15 +167,15 @@
             keep_alive.save()
 
     def _check_status(self):
         _check_status(cairo.cairo_surface_status(self._pointer))
 
     @staticmethod
     def _from_pointer(pointer, incref):
-        """Wrap an existing :c:type:`cairo_surface_t *` cdata pointer.
+        """Wrap an existing ``cairo_surface_t *`` cdata pointer.
 
         :type incref: bool
         :param incref:
             Whether increase the :ref:`reference count <refcounting>` now.
         :return:
             A new instance of :class:`Surface` or one of its sub-classes,
             depending on the surface’s type.
@@ -456,15 +456,15 @@
         """
         size = ffi.new('double[2]')
         cairo.cairo_surface_get_device_scale(self._pointer, size + 0, size + 1)
         return tuple(size)
 
     def set_mime_data(self, mime_type, data):
         """
-        Attach an image in the format :obj:`mime_type` to this surface.
+        Attach an image in the format ``mime_type`` to this surface.
 
         To remove the data from a surface,
         call this method with same mime type and :obj:`None` for data.
 
         The attached image (or filename) data can later
         be used by backends which support it
         (currently: PDF, PS, SVG and Win32 Printing surfaces)
@@ -487,18 +487,16 @@
 
         See corresponding backend surface docs
         for details about which MIME types it can handle.
         Caution: the associated MIME data will be discarded
         if you draw on the surface afterwards.
         Use this method with care.
 
-        :param mime_type: The MIME type of the image data.
-        :type mime_type: ASCII string
-        :param data: The image data to attach to the surface.
-        :type data: bytes
+        :param str mime_type: The MIME type of the image data.
+        :param bytes data: The image data to attach to the surface.
 
         *New in cairo 1.10.*
 
         """
         mime_type = ffi.new('char[]', mime_type.encode('utf8'))
         if data is None:
             _check_status(cairo.cairo_surface_set_mime_data(
@@ -513,16 +511,15 @@
                 *keep_alive.closure))
             keep_alive.save()  # Only on success
 
     def get_mime_data(self, mime_type):
         """Return mime data previously attached to surface
         using the specified mime type.
 
-        :param mime_type: The MIME type of the image data.
-        :type mime_type: ASCII string
+        :param str mime_type: The MIME type of the image data.
         :returns:
             A CFFI buffer object, or :obj:`None`
             if no data has been attached with the given mime type.
 
         *New in cairo 1.10.*
 
         """
@@ -531,18 +528,17 @@
         mime_type = ffi.new('char[]', mime_type.encode('utf8'))
         cairo.cairo_surface_get_mime_data(
             self._pointer, mime_type, buffer_address, buffer_length)
         return (ffi.buffer(buffer_address[0], buffer_length[0])
                 if buffer_address[0] != ffi.NULL else None)
 
     def supports_mime_type(self, mime_type):
-        """ Return whether surface supports :obj:`mime_type`.
+        """Return whether surface supports ``mime_type``.
 
-        :param mime_type: The MIME type of the image data.
-        :type mime_type: ASCII string
+        :param str mime_type: The MIME type of the image data.
 
         *New in cairo 1.12.*
 
         """
         mime_type = ffi.new('char[]', mime_type.encode('utf8'))
         return bool(cairo.cairo_surface_supports_mime_type(
             self._pointer, mime_type))
@@ -640,18 +636,18 @@
         self._check_status()
 
     def write_to_png(self, target=None):
         """Writes the contents of surface as a PNG image.
 
         :param target:
             A filename,
-            a binary mode file-like object with a :meth:`~file.write` method,
+            a binary mode :term:`file object` with a `write` method,
             or :obj:`None`.
         :returns:
-            If :obj:`target` is :obj:`None`,
+            If ``target`` is :obj:`None`,
             return the PNG contents as a byte string.
 
         """
         return_bytes = target is None
         if return_bytes:
             target = io.BytesIO()
         if hasattr(target, 'write'):
@@ -680,15 +676,15 @@
         if return_bytes:
             return target.getvalue()
 
 
 class ImageSurface(Surface):
     """Creates an image surface of the specified format and dimensions.
 
-    If :obj:`data` is not :obj:`None`
+    If ``data`` is not :obj:`None`
     its initial contents will be used as the initial image contents;
     you must explicitly clear the buffer,
     using, for example, :meth:`Context.rectangle` and :meth:`Context.fill`
     if you want it cleared.
 
     .. note::
 
@@ -707,15 +703,15 @@
         Buffer supplied in which to write contents,
         or :obj:`None` to create a new buffer.
     :param stride:
         The number of bytes between the start of rows
         in the buffer as allocated.
         This value should always be computed by :meth:`format_stride_for_width`
         before allocating the data buffer.
-        If omitted but :obj:`data` is given,
+        If omitted but ``data`` is given,
         :meth:`format_stride_for_width` is used.
     :type format: str
     :type width: int
     :type height: int
     :type stride: int
 
     """
@@ -768,15 +764,15 @@
 
     @classmethod
     def create_from_png(cls, source):
         """Decode a PNG file into a new image surface.
 
         :param source:
             A filename or
-            a binary mode file-like object with a :meth:`~file.read` method.
+            a binary mode :term:`file object` with a ``read`` method.
             If you already have a byte string in memory,
             use :class:`io.BytesIO`.
         :returns: A new :class:`ImageSurface` instance.
 
         """
         if hasattr(source, 'read'):
             read_func = _make_read_func(source)
@@ -789,16 +785,16 @@
         Surface.__init__(self, pointer)  # Skip ImageSurface.__init__
         return self
 
     def get_data(self):
         """Return the buffer pointing to the image’s pixel data,
         encoded according to the surface’s :ref:`FORMAT` string.
 
-        A call to :meth:`flush` is required before accessing the pixel data
-        to ensure that all pending drawing operations are finished.
+        A call to :meth:`~Surface.flush` is required before accessing the pixel
+        data to ensure that all pending drawing operations are finished.
         A call to :meth:`~Surface.mark_dirty` is required
         after the data is modified.
 
         :returns: A read-write CFFI buffer object.
 
         """
         return ffi.buffer(
@@ -827,15 +823,15 @@
 
         """
         return cairo.cairo_image_surface_get_stride(self._pointer)
 
 
 class PDFSurface(Surface):
     """Creates a PDF surface of the specified size in PostScript points
-    to be written to :obj:`target`.
+    to be written to ``target``.
 
     Note that the size of individual pages of the PDF output can vary.
     See :meth:`set_size`.
 
     The PDF surface backend recognizes the following MIME types
     for the data attached to a surface (see :meth:`~Surface.set_mime_data`)
     when it is used as a source pattern for drawing on this surface:
@@ -844,21 +840,21 @@
     If any of them is specified, the PDF backend emits an image
     with the content of MIME data
     (with the ``/DCTDecode`` or ``/JPXDecode`` filter, respectively)
     instead of a surface snapshot
     (with the ``/FlateDecode`` filter),
     which typically produces PDF with a smaller file size.
 
-    :obj:`target` can be :obj:`None` to specify no output.
+    ``target`` can be :obj:`None` to specify no output.
     This will generate a surface that may be queried and used as a source,
     without generating a temporary file.
 
     :param target:
         A filename,
-        a binary mode file-like object with a :meth:`~file.write` method,
+        a binary mode :term:`file object` with a ``write`` method,
         or :obj:`None`.
     :param width_in_points:
         Width of the surface, in points (1 point == 1/72.0 inch)
     :param height_in_points:
         Height of the surface, in points (1 point == 1/72.0 inch)
     :type width_in_points: float
     :type height_in_points: float
@@ -977,15 +973,15 @@
         *New in cairocffi 0.9.*
 
         """
         cairo.cairo_pdf_surface_set_thumbnail_size(
             self._pointer, width, height)
 
     def restrict_to_version(self, version):
-        """Restricts the generated PDF file to :obj:`version`.
+        """Restricts the generated PDF file to ``version``.
 
         See :meth:`get_versions` for a list of available version values
         that can be used here.
 
         This method should only be called
         before any drawing operations have been performed on the given surface.
         The simplest way to do this is to call this method
@@ -1028,34 +1024,34 @@
         if c_string == ffi.NULL:
             raise ValueError(version)
         return ffi.string(c_string).decode('ascii')
 
 
 class PSSurface(Surface):
     """Creates a PostScript surface of the specified size in PostScript points
-    to be written to :obj:`target`.
+    to be written to ``target``.
 
     Note that the size of individual pages of the PostScript output can vary.
     See :meth:`set_size`.
 
-    :obj:`target` can be :obj:`None` to specify no output.
+    ``target`` can be :obj:`None` to specify no output.
     This will generate a surface that may be queried and used as a source,
     without generating a temporary file.
 
     The PostScript surface backend recognizes the ``image/jpeg`` MIME type
     for the data attached to a surface (see :meth:`~Surface.set_mime_data`)
     when it is used as a source pattern for drawing on this surface.
     If it is specified, the PostScript backend emits an image
     with the content of MIME data (with the ``/DCTDecode`` filter)
     instead of a surface snapshot (with the ``/FlateDecode`` filter),
     which typically produces PostScript with a smaller file size.
 
     :param target:
         A filename,
-        a binary mode file-like object with a :meth:`~file.write` method,
+        a binary mode :term:`file object` with a ``write`` method,
         or :obj:`None`.
     :param width_in_points:
         Width of the surface, in points (1 point == 1/72.0 inch)
     :param height_in_points:
         Height of the surface, in points (1 point == 1/72.0 inch)
     :type width_in_points: float
     :type height_in_points: float
@@ -1176,15 +1172,15 @@
 
         """
         cairo.cairo_ps_surface_dsc_begin_page_setup(self._pointer)
         self._check_status()
 
     def set_eps(self, eps):
         """
-        If :obj:`eps` is True,
+        If ``eps`` is True,
         the PostScript surface will output Encapsulated PostScript.
 
         This method should only be called
         before any drawing operations have been performed on the current page.
         The simplest way to do this is to call this method
         immediately after creating the surface.
         An Encapsulated PostScript file should never contain
@@ -1221,15 +1217,15 @@
 
         """
         cairo.cairo_ps_surface_set_size(
             self._pointer, width_in_points, height_in_points)
         self._check_status()
 
     def restrict_to_level(self, level):
-        """Restricts the generated PostScript file to :obj:`level`.
+        """Restricts the generated PostScript file to ``level``.
 
         See :meth:`get_levels` for a list of available level values
         that can be used here.
 
         This method should only be called
         before any drawing operations have been performed on the given surface.
         The simplest way to do this is to call this method
@@ -1266,17 +1262,17 @@
         if c_string == ffi.NULL:
             raise ValueError(level)
         return ffi.string(c_string).decode('ascii')
 
 
 class SVGSurface(Surface):
     """Creates a SVG surface of the specified size in points
-    to be written to :obj:`target`.
+    to be written to ``target``.
 
-    :obj:`target` can be :obj:`None` to specify no output.
+    ``target`` can be :obj:`None` to specify no output.
     This will generate a surface that may be queried and used as a source,
     without generating a temporary file.
 
     The SVG surface backend recognizes the following MIME types
     for the data attached to a surface (see :meth:`~Surface.set_mime_data`)
     when it is used as a source pattern for drawing on this surface:
     ``image/png``,
@@ -1292,15 +1288,15 @@
 
     If ``text/x-uri`` is not present,
     but ``image/jpeg`` or ``image/png`` is specified,
     the corresponding data is Base64-encoded and emitted.
 
     :param target:
         A filename,
-        a binary mode file-like object with a :meth:`~file.write` method,
+        a binary mode :term:`file object` with a ``write`` method,
         or :obj:`None`.
     :param width_in_points:
         Width of the surface, in points (1 point == 1/72.0 inch)
     :param height_in_points:
         Height of the surface, in points (1 point == 1/72.0 inch)
     :type width_in_points: float
     :type height_in_points: float
@@ -1314,15 +1310,15 @@
         else:
             write_func = None
             pointer = cairo.cairo_svg_surface_create(
                 _encode_filename(target), width_in_points, height_in_points)
         Surface.__init__(self, pointer, target_keep_alive=write_func)
 
     def restrict_to_version(self, version):
-        """Restricts the generated SVG file to :obj:`version`.
+        """Restricts the generated SVG file to ``version``.
 
         See :meth:`get_versions` for a list of available version values
         that can be used here.
 
         This method should only be called
         before any drawing operations have been performed on the given surface.
         The simplest way to do this is to call this method
@@ -1364,15 +1360,15 @@
         self._check_status()
 
     def get_document_unit(self):
         """Get the unit of the SVG surface.
 
         If the surface passed as an argument is not a SVG surface, the function
         sets the error status to ``STATUS_SURFACE_TYPE_MISMATCH`` and
-        returns :ref:`SVG_UNIT_USER`.
+        returns :data:`SVG_UNIT_USER`.
 
         :return: The SVG unit of the SVG surface.
 
         *New in cairo 1.16.*
 
         *New in cairocffi 0.9.*
 
@@ -1411,15 +1407,15 @@
 class RecordingSurface(Surface):
     """A recording surface is a surface that records all drawing operations
     at the highest level of the surface backend interface,
     (that is, the level of paint, mask, stroke, fill, and show_text_glyphs).
     The recording surface can then be "replayed" against any target surface
     by using it as a source surface.
 
-    If you want to replay a surface so that the results in :obj:`target`
+    If you want to replay a surface so that the results in ``target``
     will be identical to the results that would have been obtained
     if the original operations applied to the recording surface
     had instead been applied to the target surface,
     you can use code like this::
 
         context = Context(target)
         context.set_source_surface(recording_surface, 0, 0)
@@ -1493,15 +1489,15 @@
     will be used as the size of the cairo surface. The resulting
     surface will always be of format CAIRO_FORMAT_RGB24; should
     you need another surface format, you will need to create one
     through cairo_win32_surface_create_with_dib().
 
     :param hdc :
         The DC to create a surface for,
-        as obtained from :func:`win32gui.CreateDC`.
+        as obtained from ``win32gui.CreateDC``.
         **Note**: this unsafely inteprets an integer as a pointer.
         Make sure it actually points to a valid DC!
     :type hdc: int
 
     *New in cairocffi 0.8*
 
     """
@@ -1521,15 +1517,15 @@
     The returned surface will be wrapped using the paginated surface
     to provide correct complex rendering behaviour;
     cairo_surface_show_page() and associated methods must be used
     for correct output.
 
     :param hdc:
         The DC to create a surface for,
-        as obtained from :func:`win32gui.CreateDC`.
+        as obtained from ``win32gui.CreateDC``.
         **Note**: this unsafely inteprets an integer as a pointer.
         Make sure it actually points to a valid DC!
     :type hdc: int
 
     *New in cairocffi 0.6*
 
     """
```

### Comparing `cairocffi-1.6.0/cairocffi/test_cairo.py` & `cairocffi-1.6.1/cairocffi/test_cairo.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,24 +294,24 @@
 def test_tag():
     file_obj = io.BytesIO()
     surface = PDFSurface(file_obj, 10, 10)
     context = Context(surface)
     context.tag_begin('Document')
     context.tag_begin(
         TAG_LINK,
-        attributes='rect=[1 2 4 5] uri=\'https://cairocffi.readthedocs.io/\'')
+        attributes='rect=[1 2 4 5] uri=\'https://www.courtbouillon.org/\'')
     context.set_source_rgba(1, 0, .5, 1)
     context.rectangle(2, 3, 4, 5)
     context.fill()
     context.tag_end(TAG_LINK)
     context.tag_end('Document')
     context.show_page()
     surface.finish()
     pdf = pikepdf.Pdf.open(file_obj)
-    assert '"/URI": "https://cairocffi.readthedocs.io/"' in str(pdf.objects)
+    assert '"/URI": "https://www.courtbouillon.org/"' in str(pdf.objects)
     assert '"/S": "/Document"' in str(pdf.objects)
 
 
 @pytest.mark.xfail(cairo_version() < 11504,
                    reason='Cairo version too low')
 def test_thumbnail_size():
     file_obj = io.BytesIO()
```

### Comparing `cairocffi-1.6.0/cairocffi/test_pixbuf.py` & `cairocffi-1.6.1/cairocffi/test_pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/cairocffi/test_xcb.py` & `cairocffi-1.6.1/cairocffi/test_xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/cairocffi/xcb.py` & `cairocffi-1.6.1/cairocffi/xcb.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     """The XCB surface is used to render cairo graphics to X Window System
     windows and pixmaps using the XCB library.
 
     Creates a cairo surface that targets the given drawable (pixmap or window).
 
     .. note::
 
-        This class works using objects and libraries in :mod:`xcffib`
+        This class works using objects and libraries in ``xcffib``.
 
-    :param conn: The :class:`xcffib.Connection` for an open XCB connection
+    :param conn: The ``xcffib.Connection`` for an open XCB connection
     :param drawable:
         An XID corresponding to an XCB drawable (a pixmap or a window)
-    :param visual: An :class:`xcffib.xproto.VISUALTYPE` object.
+    :param visual: An ``xcffib.xproto.VISUALTYPE`` object.
     :param width: integer
     :param height: integer
     """
     def __init__(self, conn, drawable, visual, width, height):
         c_visual = visualtype_to_c_struct(visual)
 
         p = cairo.cairo_xcb_surface_create(
```

### Comparing `cairocffi-1.6.0/docs/api.rst` & `cairocffi-1.6.1/docs/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Python API reference
 ####################
 
-.. module:: cairocffi
+.. currentmodule:: cairocffi
+
 
 Meta
 ====
 
 .. autofunction:: install_as_pycairo
 .. autofunction:: cairo_version
 .. autofunction:: cairo_version_string
@@ -13,78 +14,88 @@
 .. data:: Error
 
     An alias for :exc:`CairoError`, for compatibility with pycairo.
 
 
 Surfaces
 ========
-
 .. autoclass:: Surface
+    :members:
 
 ImageSurface
 ------------
 .. autoclass:: ImageSurface
+    :members:
 
 PDFSurface
 ----------
 .. autoclass:: PDFSurface
+    :members:
 
 PSSurface
 ---------
 .. autoclass:: PSSurface
+    :members:
 
 SVGSurface
 ----------
 .. autoclass:: SVGSurface
+    :members:
 
 RecordingSurface
 ----------------
 .. autoclass:: RecordingSurface
+    :members:
 
 Win32PrintingSurface
 --------------------
 .. autoclass:: Win32PrintingSurface
-
+    :members:
 
 Context
 =======
-
 .. autoclass:: Context
+    :members:
 
 
 Matrix
 ======
-
 .. autoclass:: Matrix
+    :members:
 
 
 Patterns
 ========
-
 .. autoclass:: Pattern()
+    :members:
 
 SolidPattern
 ------------
 .. autoclass:: SolidPattern
+    :members:
 
 SurfacePattern
 --------------
 .. autoclass:: SurfacePattern
+    :members:
 
 Gradient
 --------
 .. autoclass:: Gradient()
+    :members:
 
 LinearGradient
 ..............
 .. autoclass:: LinearGradient
+    :members:
 
 RadialGradient
 ..............
 .. autoclass:: RadialGradient
+    :members:
 
 
 .. _fonts:
 
 Fonts & text
 ============
 
@@ -112,47 +123,47 @@
 
     At the moment cairocffi only supports cairo’s "toy" font selection API.
     :class:`FontFace` objects of other types could be obtained
     eg. from :meth:`Context.get_font_face`,
     but they can not be instantiated directly.
 
 .. autoclass:: FontFace()
+    :members:
 
 ToyFontFace
 ...........
 .. autoclass:: ToyFontFace
+    :members:
 
 
 ScaledFont
 ----------
 .. autoclass:: ScaledFont
+    :members:
 
 FontOptions
 -----------
 .. autoclass:: FontOptions(**values)
+    :members:
 
 
-.. _enumerated values:
-
 Enumerated values
 =================
 
 Some parameters or return values in the cairo API
 only have a fixed, finite set of valid values.
 These are represented as *enumerated types* in C, and as integers in CFFI.
 Users are encouraged to use the constants defined here
-in the :mod:`cairocffi` module
+in the ``cairocffi`` module
 rather than literal integers.
 For example::
 
     surface = cairocffi.ImageSurface(cairocffi.FORMAT_ARGB32, 300, 400)
 
 
-.. _CONTENT:
-
 Content
 -------
 
 Used to describe the content that a :class:`Surface` will contain,
 whether color information, alpha information (translucence vs. opacity),
 or both.
```

### Comparing `cairocffi-1.6.0/docs/cffi_api.rst` & `cairocffi-1.6.1/docs/cffi_api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 
 
 Module-level objects
 --------------------
 
 .. data:: ffi
 
-    A :class:`cffi.FFI` instance with all of the cairo C API declared.
+    A :external:cffi:doc:`FFI <ref>` instance with all of the cairo C API
+    declared.
 
 .. data:: cairo
 
-    The libcairo library, pre-loaded with :meth:`ffi.dlopen`.
+    The libcairo library, pre-loaded with :external:cffi:ref:`ffi.dlopen() <dlopen>`.
     All cairo functions are accessible as attributes of this object::
 
         import cairocffi
         from cairocffi import cairo as cairo_c, SURFACE_TYPE_XLIB
 
         if cairo_c.cairo_surface_get_type(surface._pointer) == SURFACE_TYPE_XLIB:
             ...
@@ -52,62 +53,60 @@
 cairocffi’s Python wrapper will automatically decrease the reference count
 when they are garbage-collected.
 Therefore, care must be taken when creating a wrapper
 as to the reference count should be increased (for existing cairo objects)
 or not (for cairo objects that were just created with a refcount of 1.)
 
 
-.. _wrappers:
-
 Wrappers
 --------
 
 .. automethod:: Surface._from_pointer
 .. automethod:: Pattern._from_pointer
 .. automethod:: FontFace._from_pointer
 .. automethod:: ScaledFont._from_pointer
 .. automethod:: Context._from_pointer
 
 .. attribute:: Surface._pointer
 
-    The underlying :c:type:`cairo_surface_t *` cdata pointer.
+    The underlying ``cairo_surface_t *`` cdata pointer.
 
 .. attribute:: Pattern._pointer
 
-    The underlying :c:type:`cairo_pattern_t *` cdata pointer.
+    The underlying ``cairo_pattern_t *`` cdata pointer.
 
 .. attribute:: FontFace._pointer
 
-    The underlying :c:type:`cairo_font_face_t *` cdata pointer.
+    The underlying ``cairo_font_face_t *`` cdata pointer.
 
 .. attribute:: ScaledFont._pointer
 
-    The underlying :c:type:`cairo_scaled_font_t *` cdata pointer.
+    The underlying ``cairo_scaled_font_t *`` cdata pointer.
 
 .. attribute:: FontOptions._pointer
 
-    The underlying :c:type:`cairo_scaled_font_t *` cdata pointer.
+    The underlying ``cairo_scaled_font_t *`` cdata pointer.
 
 .. attribute:: Matrix._pointer
 
-    The underlying :c:type:`cairo_matrix_t *` cdata pointer.
+    The underlying ``cairo_matrix_t *`` cdata pointer.
 
 .. attribute:: Context._pointer
 
-    The underlying :c:type:`cairo_t *` cdata pointer.
+    The underlying ``cairo_t *`` cdata pointer.
 
 
 .. _converting_pycairo:
 
 Converting pycairo wrappers to cairocffi
 ----------------------------------------
 
 Some libraries such as PyGTK or PyGObject
 provide a pycairo :class:`~cairo.Context` object for you to draw on.
-It is possible to extract the underlying :c:type:`cairo_t *` pointer
+It is possible to extract the underlying ``cairo_t *`` pointer
 and create a cairocffi wrapper for the same cairo context.
 
 The follwing function does that with unsafe pointer manipulation.
 It only works on CPython.
 
 .. literalinclude:: ../utils/pycairo_to_cairocffi.py
```

### Comparing `cairocffi-1.6.0/docs/overview.rst` & `cairocffi-1.6.1/docs/overview.rst`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 cairo versions
 --------------
 
 Cairo, pycairo, and cairocffi each have version numbers. The same cairocffi
 version can be used with a variety of cairo versions. For example, the
 :meth:`Surface.set_mime_data` method is based on the
-:c:func:`cairo_surface_set_mime_data` C function, which is only available since
+``cairo_surface_set_mime_data`` C function, which is only available since
 cairo 1.10. You will get a runtime exception if you try to use it with an older
 cairo. You can however still use the rest of the API. There is no need for
 cairocffi’s versions to be tied to cairo’s versions.
 
 Use :func:`cairo_version` to test the version number for cairo::
 
     if cairocffi.cairo_version() > 11000:
```

### Comparing `cairocffi-1.6.0/docs/pixbuf.rst` & `cairocffi-1.6.1/docs/pixbuf.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/pyproject.toml` & `cairocffi-1.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,19 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Multimedia :: Graphics',
 ]
 dynamic = ['version']
 
-[tool.setuptools.dynamic]
-version = {attr = 'cairocffi.VERSION'}
-
 [project.urls]
-Documentation = 'https://cairocffi.readthedocs.io/'
+Documentation = 'https://doc.courtbouillon.org/cairocffi/'
 Code = 'https://github.com/Kozea/cairocffi/'
 Issues = 'https://github.com/Kozea/cairocffi/issues'
-Changelog = 'https://cairocffi.readthedocs.io/en/stable/changelog.html'
+Changelog = 'https://doc.courtbouillon.org/cairocffi/stable/changelog.html'
 Donation = 'https://opencollective.com/courtbouillon'
 
 [project.optional-dependencies]
 doc = ['sphinx', 'sphinx_rtd_theme']
 test = ['pytest', 'flake8', 'isort', 'numpy', 'pikepdf']
 xcb = ['xcffib >= 1.4.0']
```

### Comparing `cairocffi-1.6.0/utils/cairo_coverage.py` & `cairocffi-1.6.1/utils/cairo_coverage.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/cairocffi_to_pycairo.py` & `cairocffi-1.6.1/utils/cairocffi_to_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/compare_pycairo.py` & `cairocffi-1.6.1/utils/compare_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/mkconstants.py` & `cairocffi-1.6.1/utils/mkconstants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/pango_example.py` & `cairocffi-1.6.1/utils/pango_example.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/pycairo_to_cairocffi.py` & `cairocffi-1.6.1/utils/pycairo_to_cairocffi.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/utils/tests.py` & `cairocffi-1.6.1/utils/tests.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.0/PKG-INFO` & `cairocffi-1.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cairocffi
-Version: 1.6.0
+Version: 1.6.1
 Summary: cffi-based cairo bindings for Python
 Keywords: cairo,cffi,binding
 Author-email: Simon Sapin <contact@courtbouillon.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,17 @@
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: isort ; extra == "test"
 Requires-Dist: numpy ; extra == "test"
 Requires-Dist: pikepdf ; extra == "test"
 Requires-Dist: xcffib >= 1.4.0 ; extra == "xcb"
-Project-URL: Changelog, https://cairocffi.readthedocs.io/en/stable/changelog.html
+Project-URL: Changelog, https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 Project-URL: Code, https://github.com/Kozea/cairocffi/
-Project-URL: Documentation, https://cairocffi.readthedocs.io/
+Project-URL: Documentation, https://doc.courtbouillon.org/cairocffi/
 Project-URL: Donation, https://opencollective.com/courtbouillon
 Project-URL: Issues, https://github.com/Kozea/cairocffi/issues
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: xcb
 
 cairocffi is a `CFFI`_-based drop-in replacement for Pycairo_,
@@ -49,16 +49,16 @@
 .. _CFFI: https://cffi.readthedocs.org/
 .. _Pycairo: https://pycairo.readthedocs.io/
 .. _cairo: http://cairographics.org/
 .. _GDK-PixBuf: https://gitlab.gnome.org/GNOME/gdk-pixbuf
 
 * Free software: BSD license
 * For Python 3.7+, tested on CPython and PyPy
-* Documentation: https://cairocffi.readthedocs.io
-* Changelog: https://cairocffi.readthedocs.io/en/stable/changelog.html
+* Documentation: https://doc.courtbouillon.org/cairocffi/
+* Changelog: https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 * Code, issues, tests: https://github.com/Kozea/cairocffi
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
 * API partially compatible with Pycairo.
 * Works with any version of cairo.
```

