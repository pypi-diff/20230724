# Comparing `tmp/craft2d-0.1.4.tar.gz` & `tmp/craft2d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft2d-0.1.4.tar", max compression
+gzip compressed data, was "craft2d-0.1.5.tar", max compression
```

## Comparing `craft2d-0.1.4.tar` & `craft2d-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.4/craft2d/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.4/craft2d/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.4/craft2d/env/__init__.py
--rw-r--r--   0        0        0    14184 2023-07-24 07:21:32.317585 craft2d-0.1.4/craft2d/env/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.4/craft2d/render/__init__.py
--rw-r--r--   0        0        0    10299 2023-07-13 13:10:10.586272 craft2d-0.1.4/craft2d/render/render.py
--rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.4/craft2d/resources/agent/agent-down.png
--rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.4/craft2d/resources/agent/agent-left.png
--rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.4/craft2d/resources/agent/agent-right.png
--rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.4/craft2d/resources/agent/agent-up.png
--rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.4/craft2d/resources/farm/plant-large.png
--rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.4/craft2d/resources/farm/plant-medium.png
--rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.4/craft2d/resources/farm/plant-small.png
--rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.4/craft2d/resources/objects/bridge.png
--rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.4/craft2d/resources/objects/crafting-table.png
--rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.4/craft2d/resources/objects/gem.png
--rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.4/craft2d/resources/objects/grass.png
--rw-r--r--   0        0        0     3826 2023-07-13 13:05:51.408981 craft2d-0.1.4/craft2d/resources/objects/princess.png
--rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.4/craft2d/resources/objects/rope.png
--rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.4/craft2d/resources/objects/sticks.png
--rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.4/craft2d/resources/objects/stone.png
--rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.4/craft2d/resources/objects/tree.png
--rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.4/craft2d/resources/objects/weapon-advanced.png
--rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.4/craft2d/resources/objects/weapon-basic.png
--rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.4/craft2d/resources/objects/wood.png
--rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.4/craft2d/resources/terrain/grass.png
--rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.4/craft2d/resources/terrain/island.png
--rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.4/craft2d/resources/terrain/water.png
--rw-r--r--   0        0        0      538 2023-07-24 07:22:17.686794 craft2d-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.5/craft2d/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.5/craft2d/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.5/craft2d/env/__init__.py
+-rw-r--r--   0        0        0    16585 2023-07-24 17:56:17.165502 craft2d-0.1.5/craft2d/env/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.5/craft2d/render/__init__.py
+-rw-r--r--   0        0        0    10299 2023-07-13 13:10:10.586272 craft2d-0.1.5/craft2d/render/render.py
+-rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.5/craft2d/resources/agent/agent-down.png
+-rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.5/craft2d/resources/agent/agent-left.png
+-rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.5/craft2d/resources/agent/agent-right.png
+-rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.5/craft2d/resources/agent/agent-up.png
+-rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.5/craft2d/resources/farm/plant-large.png
+-rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.5/craft2d/resources/farm/plant-medium.png
+-rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.5/craft2d/resources/farm/plant-small.png
+-rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.5/craft2d/resources/objects/bridge.png
+-rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.5/craft2d/resources/objects/crafting-table.png
+-rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.5/craft2d/resources/objects/gem.png
+-rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.5/craft2d/resources/objects/grass.png
+-rw-r--r--   0        0        0     3826 2023-07-13 13:05:51.408981 craft2d-0.1.5/craft2d/resources/objects/princess.png
+-rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.5/craft2d/resources/objects/rope.png
+-rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.5/craft2d/resources/objects/sticks.png
+-rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.5/craft2d/resources/objects/stone.png
+-rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.5/craft2d/resources/objects/tree.png
+-rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.5/craft2d/resources/objects/weapon-advanced.png
+-rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.5/craft2d/resources/objects/weapon-basic.png
+-rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.5/craft2d/resources/objects/wood.png
+-rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.5/craft2d/resources/terrain/grass.png
+-rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.5/craft2d/resources/terrain/island.png
+-rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.5/craft2d/resources/terrain/water.png
+-rw-r--r--   0        0        0      538 2023-07-24 17:56:46.958253 craft2d-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.5/PKG-INFO
```

### Comparing `craft2d-0.1.4/craft2d/env/environment.py` & `craft2d-0.1.5/craft2d/env/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 RIGHT = 0
 LEFT = 1
 UP = 2
 DOWN = 3
 INTERACT = 4
 
-MAX_RESOURCE_COUNT = 3
+MAX_RESOURCE_COUNT = 10
 RESOURCE_COUNTS = {
-    "tree": 2,
-    "stone": 1,
-    "grass": 0,
+    "tree": 10,
+    "stone": 10,
+    "grass": 10,
     "gem": 0,
 }
 ENVIRONMENT_OBJECTS = (
     "tree",
     "stone",
     "grass",
     "crafting-table",
@@ -156,21 +156,25 @@
         else:
             self._update_agent_position(action)
             self._update_agent_direction(action)
 
         obs = self._create_observation()
         reward = 0
 
-        if self.task_object is not None:
+        # Reward = 1 when agent interacts with princess while holding task object
+        props = obs[-1]
+        if props == ("P",) and self.task_object is not None:
             task_obj_idx = PROPS.index(self.task_object)
 
-            if self.inventory[task_obj_idx] == self.task_object_count:
+            count = 1 if self.task_object_count == "M1" else 2
+
+            if self.inventory[task_obj_idx] == count:
                 reward = 1
-        done = reward == 1
 
+        done = reward == 1
         return obs, reward, done
 
     def render(self):
         if self.render_mode is None:
             assert self.spec is not None
             gym.logger.warn(
                 "You are calling render method without specifying any render mode. "
@@ -211,47 +215,104 @@
         else:
             task_collected = np.array([1])
 
         return (
             np.array([self.agent_position[0], self.agent_position[1]]).copy(),
             obs_grid.copy(),
             self.direction.copy(),
-            task_collected,
+            # task_collected,
             self.interaction_props,
         )
 
     def _sample_position(self):
         row = np.random.randint(2, self.n_rows - 1)
         col = np.random.randint(2, self.n_cols - 1)
         return row, col
 
     def _initialize_environment(self):
         used_positions = []
 
         for i, object_name in enumerate(ENVIRONMENT_OBJECTS):
-            # Skip water and bridge
             if object_name in ("water", "bridge"):
                 continue
 
-            # Determine how many of each object to place
             if object_name in RESOURCE_COUNTS:
                 count = RESOURCE_COUNTS[object_name]
             else:
                 count = 1
 
-            # Place required number of specified object
-            for _ in range(count):
-                row, col = self._sample_position()
-                while (row, col) in used_positions:
-                    row, col = self._sample_position()
-
-                # Add padding around object
-                for d_r, d_c in product(range(-1, 2), range(-1, 2)):
-                    used_positions.append((row + d_r, col + d_c))
-                self.grid[row, col, i] = 1
+            print(object_name)
+
+            center_row = np.random.randint(3, self.n_rows - 4)
+            center_col = np.random.randint(3, self.n_cols - 4)
+
+            if object_name == "tree":
+                center_row = 3
+                center_col = 8
+            elif object_name == "stone":
+                center_row = 8
+                center_col = 3
+            elif object_name == "grass":
+                center_row = 8
+                center_col = 8
+            elif object_name == "princess":
+                center_row = 0 + 2
+                center_col = 4 + 2
+            elif object_name == "crafting-table":
+                center_row = 2 + 2
+                center_col = 2 + 2
+
+            counter = 0
+
+            for d_r, d_c in product(range(-2, 2), range(-2, 2)):
+                if counter == count:
+                    break
+
+                if (center_row + d_r, center_col + d_c) in used_positions:
+                    continue
+
+                used_positions.append((center_row + d_r, center_col + d_c))
+                self.grid[center_row + d_r, center_col + d_c, i] = 1
+                counter += 1
+
+            # for _ in range(count):
+            #     row = center_row + np.random.randint(-2, 3)
+            #     col = center_col + np.random.randint(-2, 3)
+
+            #     while (row, col) in used_positions:
+            #         row = center_row + np.random.randint(-2, 3)
+            #         col = center_col + np.random.randint(-2, 3)
+
+            #     used_positions.append((row, col))
+
+            #     # for d_r, d_c in product(range(-1, 2), range(-1, 2)):
+            #     #     used_positions.append((row + d_r, col + d_c))
+            #     self.grid[row, col, i] = 1
+
+        # for i, object_name in enumerate(ENVIRONMENT_OBJECTS):
+        #     # Skip water and bridge
+        #     if object_name in ("water", "bridge"):
+        #         continue
+
+        #     # Determine how many of each object to place
+        #     if object_name in RESOURCE_COUNTS:
+        #         count = RESOURCE_COUNTS[object_name]
+        #     else:
+        #         count = 1
+
+        #     # Place required number of specified object
+        #     for _ in range(count):
+        #         row, col = self._sample_position()
+        #         while (row, col) in used_positions:
+        #             row, col = self._sample_position()
+
+        #         # Add padding around object
+        #         for d_r, d_c in product(range(-1, 2), range(-1, 2)):
+        #             used_positions.append((row + d_r, col + d_c))
+        #         self.grid[row, col, i] = 1
 
     def _initialize_island(self):
         # Get island position
         for r, c in product(range(self.n_rows), range(self.n_cols)):
             if self.grid[r, c, ENVIRONMENT_OBJECTS.index("gem")] == 1:
                 island_row = r
                 island_col = c
@@ -327,23 +388,28 @@
         object_name = ENVIRONMENT_OBJECTS[object_type]
 
         if object_name == "princess":
             if self.task_object is None:
                 self.task_object = np.random.choice(
                     (
                         "WD",
-                        "STN",
+                        # "STN",
                         # "GRS",
-                        "STKS",
+                        # "STKS",
                         # "RP",
-                        "W-BSC",
+                        # "W-BSC",
                         # "BRG",
                     )
                 )
-                self.task_object_count = np.random.choice(("M1",))
+                if self.task_object in ("WD", "STN"):
+                    count_options = ("M1",)
+                else:
+                    count_options = ("M1",)
+
+                self.task_object_count = np.random.choice(count_options)
                 self.interaction_props = (self.task_object, self.task_object_count)
             else:
                 self.interaction_props = ("P",)
         elif self.task_object is None:
             # Cannot interact before task specified
             return
```

### Comparing `craft2d-0.1.4/craft2d/render/render.py` & `craft2d-0.1.5/craft2d/render/render.py`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/agent/agent-down.png` & `craft2d-0.1.5/craft2d/resources/agent/agent-down.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/agent/agent-left.png` & `craft2d-0.1.5/craft2d/resources/agent/agent-left.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/agent/agent-right.png` & `craft2d-0.1.5/craft2d/resources/agent/agent-right.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/agent/agent-up.png` & `craft2d-0.1.5/craft2d/resources/agent/agent-up.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/farm/plant-large.png` & `craft2d-0.1.5/craft2d/resources/farm/plant-large.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/farm/plant-medium.png` & `craft2d-0.1.5/craft2d/resources/farm/plant-medium.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/farm/plant-small.png` & `craft2d-0.1.5/craft2d/resources/farm/plant-small.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/bridge.png` & `craft2d-0.1.5/craft2d/resources/objects/bridge.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/crafting-table.png` & `craft2d-0.1.5/craft2d/resources/objects/crafting-table.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/gem.png` & `craft2d-0.1.5/craft2d/resources/objects/gem.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/grass.png` & `craft2d-0.1.5/craft2d/resources/objects/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/princess.png` & `craft2d-0.1.5/craft2d/resources/objects/princess.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/rope.png` & `craft2d-0.1.5/craft2d/resources/objects/rope.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/sticks.png` & `craft2d-0.1.5/craft2d/resources/objects/sticks.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/stone.png` & `craft2d-0.1.5/craft2d/resources/objects/stone.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/tree.png` & `craft2d-0.1.5/craft2d/resources/objects/tree.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/weapon-advanced.png` & `craft2d-0.1.5/craft2d/resources/objects/weapon-advanced.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/weapon-basic.png` & `craft2d-0.1.5/craft2d/resources/objects/weapon-basic.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/objects/wood.png` & `craft2d-0.1.5/craft2d/resources/objects/wood.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/terrain/grass.png` & `craft2d-0.1.5/craft2d/resources/terrain/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/terrain/island.png` & `craft2d-0.1.5/craft2d/resources/terrain/island.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/craft2d/resources/terrain/water.png` & `craft2d-0.1.5/craft2d/resources/terrain/water.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.4/pyproject.toml` & `craft2d-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft2d"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Tristan Bester <tristanbester@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.25.1"
```

### Comparing `craft2d-0.1.4/PKG-INFO` & `craft2d-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft2d
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Tristan Bester
 Author-email: tristanbester@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

