# Comparing `tmp/processpiper-0.4.2.tar.gz` & `tmp/processpiper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.4.2.tar", last modified: Sun Jul 23 06:15:55 2023, max compression
+gzip compressed data, was "processpiper-0.4.3.tar", last modified: Mon Jul 24 09:27:53 2023, max compression
```

## Comparing `processpiper-0.4.2.tar` & `processpiper-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 06:15:55.737678 processpiper-0.4.2/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     6654 2023-07-23 06:15:55.737678 processpiper-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6099 2023-07-23 06:14:11.000000 processpiper-0.4.2/README.md
--rw-rw-rw-   0        0        0     1030 2023-07-23 06:14:11.000000 processpiper-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 06:15:55.737678 processpiper-0.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-23 06:15:55.703677 processpiper-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 06:15:55.725678 processpiper-0.4.2/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.4.2/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2372 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11722 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1881 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/constants.py
--rw-rw-rw-   0        0        0    12129 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.4.2/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     4359 2023-05-16 08:14:49.000000 processpiper-0.4.2/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     3291 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/helper.py
--rw-rw-rw-   0        0        0     9558 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    19270 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/layout.py
--rw-rw-rw-   0        0        0    46744 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     4946 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    21262 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    39089 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/shape.py
--rw-rw-rw-   0        0        0    11494 2023-06-23 09:06:58.000000 processpiper-0.4.2/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2263 2023-05-16 08:14:49.000000 processpiper-0.4.2/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-07-23 06:14:11.000000 processpiper-0.4.2/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-07-23 06:15:55.734678 processpiper-0.4.2/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6654 2023-07-23 06:15:55.000000 processpiper-0.4.2/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      762 2023-07-23 06:15:55.000000 processpiper-0.4.2/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 06:15:55.000000 processpiper-0.4.2/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-23 06:15:55.000000 processpiper-0.4.2/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-23 06:15:55.000000 processpiper-0.4.2/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 06:15:55.735676 processpiper-0.4.2/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.4.2/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.4.2/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:27:53.920087 processpiper-0.4.3/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     6654 2023-07-24 09:27:53.920087 processpiper-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6099 2023-07-23 06:14:11.000000 processpiper-0.4.3/README.md
+-rw-rw-rw-   0        0        0     1030 2023-07-23 06:14:11.000000 processpiper-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:27:53.920087 processpiper-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 09:27:53.881789 processpiper-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:27:53.901081 processpiper-0.4.3/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.4.3/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2372 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11722 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1881 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0    12129 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.4.3/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     4359 2023-05-16 08:14:49.000000 processpiper-0.4.3/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     3291 2023-07-23 06:14:11.000000 processpiper-0.4.3/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0     9558 2023-07-23 06:14:11.000000 processpiper-0.4.3/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    19885 2023-07-24 09:27:11.000000 processpiper-0.4.3/src/processpiper/layout.py
+-rw-rw-rw-   0        0        0    48358 2023-07-24 09:27:11.000000 processpiper-0.4.3/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     4946 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    21261 2023-07-24 09:27:11.000000 processpiper-0.4.3/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    39089 2023-07-23 06:14:11.000000 processpiper-0.4.3/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0    11494 2023-06-23 09:06:58.000000 processpiper-0.4.3/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2263 2023-05-16 08:14:49.000000 processpiper-0.4.3/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-07-24 09:27:11.000000 processpiper-0.4.3/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:27:53.917083 processpiper-0.4.3/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6654 2023-07-24 09:27:53.000000 processpiper-0.4.3/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      762 2023-07-24 09:27:53.000000 processpiper-0.4.3/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:27:53.000000 processpiper-0.4.3/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-24 09:27:53.000000 processpiper-0.4.3/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 09:27:53.000000 processpiper-0.4.3/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:27:53.919083 processpiper-0.4.3/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.4.3/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.4.3/src/tests/github_action_test.py
```

### Comparing `processpiper-0.4.2/LICENSE` & `processpiper-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/PKG-INFO` & `processpiper-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.4.2
+Version: 0.4.3
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: processpiper Version: 0.4.2 Summary: Processpiper.
+Metadata-Version: 2.1 Name: processpiper Version: 0.4.3 Summary: Processpiper.
 An open source python library to generate business process diagram using code.
 Author: CS Goh Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE ![release](https://img.shields.io/pypi/v/processpiper?style=plastic) !
```

### Comparing `processpiper-0.4.2/README.md` & `processpiper-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/pyproject.toml` & `processpiper-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/activity.py` & `processpiper-0.4.3/src/processpiper/activity.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/colourtheme.py` & `processpiper-0.4.3/src/processpiper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/constants.py` & `processpiper-0.4.3/src/processpiper/constants.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/event.py` & `processpiper-0.4.3/src/processpiper/event.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/footer.py` & `processpiper-0.4.3/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/gateway.py` & `processpiper-0.4.3/src/processpiper/gateway.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/helper.py` & `processpiper-0.4.3/src/processpiper/helper.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/lane.py` & `processpiper-0.4.3/src/processpiper/lane.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/layout.py` & `processpiper-0.4.3/src/processpiper/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,42 +82,46 @@
 
             if self.is_same_lane(previous_shape, current_shape):
                 # Same lane
 
                 if index == 0:
                     Helper.printc(
                         (
-                            "        ==>Same lane: ",
+                            "        ==>Same lane (row 0): ",
                             f"add_shape_to_lane [{current_shape.name}],",
                             f" {previous_shape_row_number=}",
                         ),
                         show_level="layout_grid",
                     )
                     self.add_shape_to_lane(
                         current_shape.lane_id, previous_shape_row_number, current_shape
                     )
-                else:
+                else:  ### Next row
                     Helper.printc(
-                        f"        ==>Same lane: add_shape_to_lane_rowcolumn [{current_shape.name}, {previous_shape_col_number + 1}]",
+                        f"        ==>Same lane (next row): add_shape_to_lane_rowcolumn [{current_shape.name}, {previous_shape_col_number}]",
                         show_level="layout_grid",
                     )
                     if self.is_column_empty(
                         current_shape.lane_id,
                         previous_shape_row_number,
-                        previous_shape_col_number + 1,
+                        previous_shape_col_number,
                     ):
                         Helper.printc("Is empty", 34, show_level="layout_grid")
                         self.add_shape_to_lane_rowcolumn(
                             current_shape.lane_id,
                             previous_shape_row_number,
-                            previous_shape_col_number + 1,
+                            previous_shape_col_number,
                             current_shape,
                         )
                     else:
                         Helper.printc("Not empty", 34, show_level="layout_grid")
+                        Helper.printc(
+                            f"Adding shape to {index + 1}, {previous_shape_col_number}",
+                            show_level="layout_grid",
+                        )
                         self.add_shape_to_lane_rowcolumn(
                             current_shape.lane_id,
                             index + 1,
                             # previous_shape_col_number + 1,
                             previous_shape_col_number,
                             current_shape,
                         )
@@ -219,15 +223,18 @@
             if col_number > len(self._grid[lane_id][row_number]):
                 for _ in range(col_number - len(self._grid[lane_id][row_number]) - 1):
                     self._grid[lane_id][row_number].append(None)
                 self._grid[lane_id][row_number].append(shape)
             elif col_number == 1:
                 self._grid[lane_id][row_number].append(shape)
             else:
-                self._grid[lane_id][row_number][col_number - 1] = shape
+                if self._grid[lane_id][row_number][col_number - 1] is None:
+                    self._grid[lane_id][row_number][col_number - 1] = shape
+                else:
+                    self._grid[lane_id][row_number].append(shape)
 
         Helper.printc(
             f"            ### {shape.name=}, {lane_id=}, {row_number=}, {col_number=}",
             36,
             show_level="layout_grid",
         )
 
@@ -261,14 +268,16 @@
     def is_column_empty(self, lane_id: str, row_number: int, col_number: int):
         # sourcery skip: use-any
         """Check if the column is empty"""
 
         row_number = f"row{row_number}"
         for row, col in self._grid[lane_id].items():
             if row == row_number and col[col_number - 1] is not None:
+                shape = col[col_number - 1]
+                Helper.printc(f"            ### {shape.name}", show_level="layout_grid")
                 return False
         return True
 
     def get_shape_lane_rowcolumn(self, shape: Shape):
         """Get the shape lane, row and column"""
         for lane_id, lane in self._grid.items():
             for row, col in lane.items():
@@ -278,14 +287,15 @@
                     return lane_id, row_number, col.index(shape) + 1
         return None, None, None
 
     def add_shape_to_lane(self, lane_id: str, row_number: int, current_shape: Shape):
         """Add the shape to the lane"""
         if lane_id is not None:
             col_number = self.get_next_column(lane_id, row_number)
+            # col_number = self.get_next_empty_column(lane_id, row_number)
             Helper.printc(
                 f"            ### {lane_id=}, {row_number=}, {col_number=}",
                 33,
                 show_level="layout_grid",
             )
             self.add_shape_to_lane_rowcolumn(
                 lane_id, row_number, col_number, current_shape
```

### Comparing `processpiper-0.4.2/src/processpiper/painter.py` & `processpiper-0.4.3/src/processpiper/painter.py`

 * *Files 2% similar despite different names*

```diff
@@ -707,15 +707,16 @@
         connector_line_colour: str = "",
     ):
         """Draw a right angle line between two points"""
         points, right_angle_points = self.get_connection_points(
             x1, y1, face_source, x2, y2, face_target
         )
         Helper.printc(
-            f"\t" * 2 + f"DRAW_RIGHT_ANGLE_LINE() {x1=}, {y1=}, {face_source=}, {x2=}, {y2=}, {face_target=}",
+            f"\t" * 2
+            + f"DRAW_RIGHT_ANGLE_LINE() {x1=}, {y1=}, {face_source=}, {x2=}, {y2=}, {face_target=}",
             show_level="draw_connection",
         )
 
         if connection_style == "dashed":
             self.draw_dashed_line(points, connector_line_width, connector_line_colour)
         else:
             self.__cr.line(
@@ -725,122 +726,162 @@
 
     def get_connection_points(self, x1, y1, face_source, x2, y2, face_target):
         """Get the points to draw a line between two elements"""
         tab_count = 3
         if x1 == x2 and y1 == y2:
             # Shapes are on top of each other / overlapping. NOTE: This should never happen
             Helper.printc(
-                 "\t" * tab_count + "Shapes are on top of each other / overlapping",
+                "\t" * tab_count + "Shapes are on top of each other / overlapping",
                 show_level="draw_connection",
             )
             Helper.printc(
-                f"\t" * tab_count + "A: right_angle_line: x1 == x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
+                f"\t" * tab_count
+                + "A: right_angle_line: x1 == x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
                 show_level="draw_connection",
             )
             points = [(x1, y1)]
             right_angle_point = points
 
         if x1 != x2 and y1 == y2:
             # Shapes are on the same horizontal line
             Helper.printc(
-                 "\t" * tab_count + "Shapes are on the same horizontal line",
+                "\t" * tab_count + "Shapes are on the same horizontal line",
                 show_level="draw_connection",
             )
             Helper.printc(
-                f"\t" * tab_count + "B: right_angle_line: x1 != x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
+                f"\t" * tab_count
+                + "B: right_angle_line: x1 != x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
                 show_level="draw_connection",
             )
             elbow_height = 40
             if face_source.find("top") != -1:
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y2 - elbow_height),
                     (x2, y2),
                 ]
                 right_angle_point = [(x1, y1 - elbow_height), (x2, y2 - elbow_height)]
             elif face_source.find("bottom") != -1:
-                points = [(x1, y1), (x1, y1 + elbow_height), (x2, y2 + elbow_height)]
-                right_angle_point = [(x1, y1 + elbow_height)]
+                # points = [(x1, y1), (x1, y1 + elbow_height), (x2, y2 + elbow_height)]
+                # right_angle_point = [(x1, y1 + elbow_height)]
+                if y2 <= y1:
+                    angle_height = 40
+                else:
+                    angle_height = y2 - y1 + 40
+
+                points = [
+                    (x1, y1),
+                    (x1, y1 + angle_height),
+                    (x2, y1 + angle_height),
+                    (x2, y2),
+                ]
+                right_angle_point = [
+                    (x1, y1 + angle_height),
+                    (x2, y1 + angle_height),
+                ]
             else:
                 points = [(x1, y1), (x2, y1)]
                 right_angle_point = [(x1, y1)]
 
         if x1 == x2 and y1 != y2:
             # Shapes are on the same vertical line
             Helper.printc(
-                 "\t" * tab_count + "Shapes are on the same vertical line",
+                "\t" * tab_count + "Shapes are on the same vertical line",
                 show_level="draw_connection",
             )
             Helper.printc(
-                f"\t" * tab_count + "C: right_angle_line: x1 == x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                f"\t" * tab_count
+                + "C: right_angle_line: x1 == x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
                 show_level="draw_connection",
             )
             points = [(x1, y1), (x1, y2)]
             right_angle_point = [(x1, y1)]
 
         if x1 != x2 and y1 != y2:
             # Shapes are on different horizontal and vertical lines
             # check if face1 string contained the word "right"
             Helper.printc(
-                "\t" * tab_count + "Shapes are on different horizontal and vertical lines",
+                "\t" * tab_count
+                + "Shapes are on different horizontal and vertical lines",
                 show_level="draw_connection",
             )
             if face_source.find("bottom") != -1:
                 if face_target.find("bottom") != -1:
                     Helper.printc(
-                         "\t" * tab_count + "D-bottom: both bottom",
+                        "\t" * tab_count + "D-bottom: both bottom",
                         show_level="draw_connection",
                     )
                     # if so, then the line should be drawn from the bottom side of the box
-                    angle_height = 40
+                    if y2 <= y1:
+                        angle_height = 50
+                    else:
+                        angle_height = y2 - y1 + 50
+
                     points = [
                         (x1, y1),
                         (x1, y1 + angle_height),
                         (x2, y1 + angle_height),
                         (x2, y2),
                     ]
                     right_angle_point = [
                         (x1, y1 + angle_height),
                         (x2, y1 + angle_height),
                     ]
-                else:
+                elif face_target.find("top") != -1:
                     Helper.printc(
-                         "\t" * tab_count + "D-bottom: source bottom",
+                        "\t" * tab_count + "D-bottom: source bottom, target top",
+                        show_level="draw_connection",
+                    )
+                    elbow_height = 40
+                    points = [
+                        (x1, y1),
+                        (x1, y1 + elbow_height),
+                        (x2, y1 + elbow_height),
+                        (x2, y2),
+                    ]
+                    right_angle_point = [
+                        (x1, y1 + elbow_height),
+                        (x2, y1 + elbow_height),
+                    ]
+                else:  ### target face is
+                    Helper.printc(
+                        "\t" * tab_count + "D-bottom: source bottom",
                         show_level="draw_connection",
                     )
                     # if so, then the line should be drawn from the bottom side of the box
                     points = [
                         (x1, y1),
                         (x1, y2),
                         (x2, y2),
                     ]
                     right_angle_point = [(x1, y2)]
             elif face_source.find("right") != -1:
                 Helper.printc(
-                    f"\t" * tab_count + "D-right: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    f"\t" * tab_count
+                    + "D-right: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
                     show_level="draw_connection",
                 )
                 if face_target.find("left") != -1:
-                    elbow_height = 40
+                    elbow_height = x2 - x1 - 40
                     points = [
                         (x1, y1),
                         (x1 + elbow_height, y1),
                         (x1 + elbow_height, y2),
                         (x2, y2),
                     ]
                     right_angle_point = [
                         (x1 + elbow_height, y1),
                         (x1 + elbow_height, y2),
                     ]
                 elif face_target.find("right") != -1:
                     elbow_height = 40
                     ### both faces are right
                     Helper.printc(
-                         "\t" * tab_count + "D-right-right (x1 < x2)",
+                        "\t" * tab_count + "D-right-right (x1 < x2)",
                         show_level="draw_connection",
                     )
                     points = [
                         (x1, y1),
                         (x2 + elbow_height, y1),
                         (x2 + elbow_height, y2),
                         (x2, y2),
@@ -848,28 +889,28 @@
                     right_angle_point = [
                         (x2 + elbow_height, y1),
                         (x2 + elbow_height, y2),
                     ]
                 elif face_target.find("top") != -1:
                     if y1 < y2:
                         Helper.printc(
-                             "\t" * 2 + "D-right-top (y1 < y2)",
+                            "\t" * 2 + "D-right-top (y1 < y2)",
                             show_level="draw_connection",
                         )
                         points = [
                             (x1, y1),
                             (x2, y1),
                             (x2, y2),
                         ]
                         right_angle_point = [
                             (x2, y1),
                         ]
                     else:
                         Helper.printc(
-                             "\t" * tab_count + "D-right-top (y1 >= y2)",
+                            "\t" * tab_count + "D-right-top (y1 >= y2)",
                             show_level="draw_connection",
                         )
                         vertical_elbow_height = 40
                         horizontal_elbow_height = 60
                         points = [
                             (x1, y1),
                             (x2 + horizontal_elbow_height, y1),
@@ -880,70 +921,75 @@
                         right_angle_point = [
                             (x2 + horizontal_elbow_height, y1),
                             (x2 + horizontal_elbow_height, y2 - vertical_elbow_height),
                             (x2, y2 - vertical_elbow_height),
                         ]
                 else:
                     Helper.printc(
-                         "\t" * tab_count + "D-right-bottom", show_level="draw_connection"
+                        "\t" * tab_count + "D-right-bottom",
+                        show_level="draw_connection",
                     )
                     points = [
                         (x1, y1),
                         (x2, y1),
                         (x2, y2),
                     ]
                     right_angle_point = [
                         (x2, y1),
                     ]
             elif face_source.find("top") != -1 and face_target.find("top") != -1:
                 Helper.printc(
-                    f"\t" * tab_count + "D-top: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    f"\t" * tab_count
+                    + "D-top: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
                     show_level="draw_connection",
                 )
                 # draw 1 right angle line
                 elbow_height = 40
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y1 - elbow_height),
                     (x2, y2),
                 ]
                 # right_angle_point = (x2, y2 - elbow_height)
                 right_angle_point = [(x1, y1 - elbow_height), (x2, y1 - elbow_height)]
             elif face_source.find("top") != -1 and face_target.find("bottom") != -1:
                 Helper.printc(
-                    f"\t" * tab_count + "D-top/bottom: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    f"\t" * tab_count
+                    + "D-top/bottom: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
                     show_level="draw_connection",
                 )
                 # draw 1 right angle line
                 elbow_height = 20
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y1 - elbow_height),
                     (x2, y2),
                 ]
                 # right_angle_point = (x2, y1 - elbow_height)
                 right_angle_point = [(x1, y1 - elbow_height), (x2, y1 - elbow_height)]
             else:
                 Helper.printc(
-                    f"\t" * tab_count + "D-else: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    f"\t" * tab_count
+                    + "D-else: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
                     show_level="draw_connection",
                 )
                 # if so, then the line should be drawn from the bottom side of the box
                 points = [(x1, y1), (x1, y2), (x2, y2)]
                 right_angle_point = [(x1, y2)]
                 # for point in points:
                 #     self.draw_circle(point[0], point[1], 4, "yellow")
 
         if x1 > x2:
             if y1 <= y2:
                 if abs(y1 - y2) == 10:
                     Helper.printc(
-                        f"\t" * tab_count + "E: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                        f"\t" * tab_count
+                        + "E: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
                         show_level="draw_connection",
                     )
                     elbow_height = 40
                     points = [
                         (x1, y1),
                         (x1, y1 - elbow_height),
                         (x2, y1 - elbow_height),
@@ -957,15 +1003,16 @@
                 if abs(y1 - y2) >= 100:
                     elbow_height = 40
                     if (
                         face_source.find("bottom") == -1
                         or face_target.find("right") == -1
                     ):
                         Helper.printc(
-                            f"\t" * tab_count + "F2: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                            f"\t" * tab_count
+                            + "F2: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
                             show_level="draw_connection",
                         )
                         points = [
                             (x1, y1),
                             (x1, y1 + elbow_height),
                             (x2, y1 + elbow_height),
                             (x2, y2),
@@ -973,26 +1020,28 @@
                         # right_angle_point = (x2, y1 - elbow_height)
                         right_angle_point = [
                             (x1, y1 - elbow_height),
                             (x2, y1 - elbow_height),
                         ]
                     else:
                         Helper.printc(
-                            f"\t" * tab_count + "F1: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                            f"\t" * tab_count
+                            + "F1: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
                             show_level="draw_connection",
                         )
                         points = [
                             (x1, y1),
                             (x1, y2),
                             (x2, y2),
                         ]
                         right_angle_point = [(x1, y2)]
             elif len(points) == 0:
                 Helper.printc(
-                    f"\t" * tab_count + "G: x1 > x2 and y1 > y2: {x1=}, {y1=}, {x2=}, {y2=}",
+                    f"\t" * tab_count
+                    + "G: x1 > x2 and y1 > y2: {x1=}, {y1=}, {x2=}, {y2=}",
                     show_level="draw_connection",
                 )
                 elbow_height = (y1 - y2) / 2
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y2 + elbow_height),
```

### Comparing `processpiper-0.4.2/src/processpiper/pool.py` & `processpiper-0.4.3/src/processpiper/pool.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/processmap.py` & `processpiper-0.4.3/src/processpiper/processmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     lane_max_width: int = field(init=False, default=0)
 
     def __post_init__(self):
         """Initialise the Process Map Class"""
 
         logging.basicConfig(
             # filename="processpiper.log",
-            level=logging.ERROR,
+            level=logging.INFO,
             format="%(asctime)s [%(levelname)s] : %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
         self.start_time = time.time()
         self.__painter = Painter(self.width, self.height)
         self.__set_colour_theme(self.colour_theme)
         self.__painter.set_background_colour(self.__painter.background_colour)
```

### Comparing `processpiper-0.4.2/src/processpiper/shape.py` & `processpiper-0.4.3/src/processpiper/shape.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/text2diagram.py` & `processpiper-0.4.3/src/processpiper/text2diagram.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/title.py` & `processpiper-0.4.3/src/processpiper/title.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/processpiper/version.py` & `processpiper-0.4.3/src/processpiper/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Version information for processpiper."""
-__version__ = "v0.4.2"
+__version__ = "v0.4.3"
```

### Comparing `processpiper-0.4.2/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.4.3/src/processpiper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.4.2
+Version: 0.4.3
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: processpiper Version: 0.4.2 Summary: Processpiper.
+Metadata-Version: 2.1 Name: processpiper Version: 0.4.3 Summary: Processpiper.
 An open source python library to generate business process diagram using code.
 Author: CS Goh Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE ![release](https://img.shields.io/pypi/v/processpiper?style=plastic) !
```

### Comparing `processpiper-0.4.2/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.4.3/src/processpiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.2/src/tests/github_action_test.py` & `processpiper-0.4.3/src/tests/github_action_test.py`

 * *Files identical despite different names*

