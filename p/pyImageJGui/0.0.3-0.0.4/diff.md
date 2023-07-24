# Comparing `tmp/pyImageJGui-0.0.3.tar.gz` & `tmp/pyimagejgui-0.0.4.tar.gz`

## Comparing `pyImageJGui-0.0.3.tar` & `pyimagejgui-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,33 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/init.bat
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/init.sh
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/angle.svg
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/circle.svg
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/clear.svg
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/elliptical.svg
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/file.svg
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/freehand.svg
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/hand.svg
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/line.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/magnifier.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/polygon.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/rectangle.svg
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/icon/rotate.svg
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/style/__init__.py
--rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/style/main.qss
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/style/qssloader.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/AngleRoi.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/CircleRoi.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/EllipseRoi.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/LineRoi.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/RectangleRoi.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/constant.py
--rw-r--r--   0        0        0    14383 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/imageView.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui/ui/main_ui.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui.egg-info/PKG-INFO
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/src/pyImageJGui.egg-info/top_level.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/README.md
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pyimagejgui-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/init.bat
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/init.sh
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/angle.svg
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/circle.svg
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/clear.svg
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/elliptical.svg
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/file.svg
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/freehand.svg
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/hand.svg
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/line.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/magnifier.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/polygon.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/rectangle.svg
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/icon/rotate.svg
+-rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/style/main.qss
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/style/qssloader.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/AngleRoi.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/CircleRoi.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/EllipseRoi.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/LineRoi.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/RectangleRoi.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/constant.py
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/imageView.py
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/src/pyImageJGui/ui/main_ui.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/README.md
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pyimagejgui-0.0.4/PKG-INFO
```

### Comparing `pyimagejgui-0.0.3/main.py` & `pyimagejgui-0.0.4/main.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/.github/workflows/python-publish.yml` & `pyimagejgui-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/angle.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/angle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/circle.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/circle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/clear.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/clear.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/elliptical.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/elliptical.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/file.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/file.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/freehand.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/freehand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/hand.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/hand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/magnifier.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/magnifier.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/polygon.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/polygon.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/icon/rotate.svg` & `pyimagejgui-0.0.4/src/pyImageJGui/icon/rotate.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/style/main.qss` & `pyimagejgui-0.0.4/src/pyImageJGui/style/main.qss`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/AngleRoi.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/AngleRoi.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @Software : PyCharm
 """
 from typing import Union
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
-from src.pyImageJGui.ui.LineRoi import LineRoi
+from LineRoi import LineRoi
 from shapely import geometry
 
 
 class AngleRoi():
     def __init__(self, scale_factor):
         self.line1 = LineRoi(scale_factor)
         self.line2 = LineRoi(scale_factor)
```

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/CircleRoi.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/CircleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/EllipseRoi.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/EllipseRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/LineRoi.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/LineRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/RectangleRoi.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/RectangleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/imageView.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/imageView.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 @File: imageView.py
 @Software : PyCharm
 """
 import math
 from PySide6.QtWidgets import *
 from PySide6.QtGui import *
 from PySide6.QtCore import *
-from src.pyImageJGui.ui.constant import ROI
-from src.pyImageJGui.ui.RectangleRoi import RectangleRoi
-from src.pyImageJGui.ui.CircleRoi import CircleRoi
-from src.pyImageJGui.ui.LineRoi import LineRoi
-from src.pyImageJGui.ui.AngleRoi import AngleRoi
-from src.pyImageJGui.ui.EllipseRoi import EllipseRoi
+from constant import ROI
+from RectangleRoi import RectangleRoi
+from CircleRoi import CircleRoi
+from LineRoi import LineRoi
+from AngleRoi import AngleRoi
+from EllipseRoi import EllipseRoi
 
 
 class ImageViewer(QGraphicsView):
 
     def __init__(self, cursor: QLineEdit, roi: ROI, parent: QWidget):
         super().__init__()
         self.cursor = cursor
```

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui/ui/main_ui.py` & `pyimagejgui-0.0.4/src/pyImageJGui/ui/main_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 @Software : PyCharm
 """
 import os
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 from PySide6.QtCore import *
 import cv2 as cv
-from src.pyImageJGui.ui.imageView import ImageViewer
-from src.pyImageJGui.ui.constant import ROI
+from imageView import ImageViewer
+from constant import ROI
 
 path = os.path.dirname(os.path.dirname(__file__))
 
 
 class ImageWidget(QWidget):
     def __init__(self, parent=None):
         QWidget.__init__(self, parent)
```

### Comparing `pyimagejgui-0.0.3/src/pyImageJGui.egg-info/PKG-INFO` & `pyimagejgui-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: pyImageJGui
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python for ImageJ GUI
-Author-email: sdb <sdb20200101@gmail.com>
 Project-URL: homepage, https://github.com/aghb123/pyImageJGui
-Keywords: imagej,GUI,PySide6
-Platform: any
+Author-email: sdb <sdb20200101@gmail.com>
+License-File: LICENSE
+Keywords: GUI,PySide6,imagej
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
+Requires-Dist: pyside6
+Requires-Dist: shapely
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-# pyImageJGui
+# pyImageJGui
```

### Comparing `pyimagejgui-0.0.3/LICENSE` & `pyimagejgui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.3/pyproject.toml` & `pyimagejgui-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyImageJGui"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python for ImageJ GUI"
 authors = [{name = "sdb", email = "sdb20200101@gmail.com"}]
 readme = "README.md"
 keywords = ["imagej", "GUI", "PySide6"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

