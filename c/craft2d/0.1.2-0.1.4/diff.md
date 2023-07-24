# Comparing `tmp/craft2d-0.1.2.tar.gz` & `tmp/craft2d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft2d-0.1.2.tar", max compression
+gzip compressed data, was "craft2d-0.1.4.tar", max compression
```

## Comparing `craft2d-0.1.2.tar` & `craft2d-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.2/craft2d/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.2/craft2d/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.2/craft2d/env/__init__.py
--rw-r--r--   0        0        0    12324 2023-07-12 16:06:09.446174 craft2d-0.1.2/craft2d/env/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.2/craft2d/render/__init__.py
--rw-r--r--   0        0        0    10024 2023-07-12 12:28:33.746399 craft2d-0.1.2/craft2d/render/render.py
--rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.2/craft2d/resources/agent/agent-down.png
--rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.2/craft2d/resources/agent/agent-left.png
--rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.2/craft2d/resources/agent/agent-right.png
--rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.2/craft2d/resources/agent/agent-up.png
--rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.2/craft2d/resources/farm/plant-large.png
--rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.2/craft2d/resources/farm/plant-medium.png
--rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.2/craft2d/resources/farm/plant-small.png
--rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.2/craft2d/resources/objects/bridge.png
--rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.2/craft2d/resources/objects/crafting-table.png
--rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.2/craft2d/resources/objects/gem.png
--rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.2/craft2d/resources/objects/grass.png
--rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.2/craft2d/resources/objects/rope.png
--rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.2/craft2d/resources/objects/sticks.png
--rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.2/craft2d/resources/objects/stone.png
--rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.2/craft2d/resources/objects/tree.png
--rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.2/craft2d/resources/objects/weapon-advanced.png
--rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.2/craft2d/resources/objects/weapon-basic.png
--rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.2/craft2d/resources/objects/wood.png
--rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.2/craft2d/resources/terrain/grass.png
--rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.2/craft2d/resources/terrain/island.png
--rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.2/craft2d/resources/terrain/water.png
--rw-r--r--   0        0        0      538 2023-07-12 16:07:54.910818 craft2d-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.4/craft2d/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.4/craft2d/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.4/craft2d/env/__init__.py
+-rw-r--r--   0        0        0    14184 2023-07-24 07:21:32.317585 craft2d-0.1.4/craft2d/env/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.4/craft2d/render/__init__.py
+-rw-r--r--   0        0        0    10299 2023-07-13 13:10:10.586272 craft2d-0.1.4/craft2d/render/render.py
+-rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.4/craft2d/resources/agent/agent-down.png
+-rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.4/craft2d/resources/agent/agent-left.png
+-rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.4/craft2d/resources/agent/agent-right.png
+-rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.4/craft2d/resources/agent/agent-up.png
+-rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.4/craft2d/resources/farm/plant-large.png
+-rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.4/craft2d/resources/farm/plant-medium.png
+-rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.4/craft2d/resources/farm/plant-small.png
+-rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.4/craft2d/resources/objects/bridge.png
+-rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.4/craft2d/resources/objects/crafting-table.png
+-rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.4/craft2d/resources/objects/gem.png
+-rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.4/craft2d/resources/objects/grass.png
+-rw-r--r--   0        0        0     3826 2023-07-13 13:05:51.408981 craft2d-0.1.4/craft2d/resources/objects/princess.png
+-rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.4/craft2d/resources/objects/rope.png
+-rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.4/craft2d/resources/objects/sticks.png
+-rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.4/craft2d/resources/objects/stone.png
+-rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.4/craft2d/resources/objects/tree.png
+-rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.4/craft2d/resources/objects/weapon-advanced.png
+-rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.4/craft2d/resources/objects/weapon-basic.png
+-rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.4/craft2d/resources/objects/wood.png
+-rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.4/craft2d/resources/terrain/grass.png
+-rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.4/craft2d/resources/terrain/island.png
+-rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.4/craft2d/resources/terrain/water.png
+-rw-r--r--   0        0        0      538 2023-07-24 07:22:17.686794 craft2d-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.4/PKG-INFO
```

### Comparing `craft2d-0.1.2/craft2d/env/environment.py` & `craft2d-0.1.4/craft2d/env/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 
 from craft2d.render.render import HumanRenderer
 
 RIGHT = 0
 LEFT = 1
 UP = 2
 DOWN = 3
-USE = 4
+INTERACT = 4
 
 MAX_RESOURCE_COUNT = 3
 RESOURCE_COUNTS = {
-    "tree": 4,
-    "stone": 2,
-    "grass": 2,
-    "gem": 1,
+    "tree": 2,
+    "stone": 1,
+    "grass": 0,
+    "gem": 0,
 }
 ENVIRONMENT_OBJECTS = (
     "tree",
     "stone",
     "grass",
     "crafting-table",
     "water",
     "gem",
     "bridge",
+    "princess",
 )
 INVENTORY_OBJECTS = (
     "wood",
     "stone",
     "grass",
     "sticks",
     "rope",
@@ -45,14 +46,23 @@
     "make-sticks": 3,
     "make-rope": 4,
     "make-bridge": 5,
     "make-basic-weapon": 6,
     "get-gem": 7,
     "make-advanced-weapon": 8,
 }
+PROPS = (
+    "WD",
+    "STN",
+    "GRS",
+    "STKS",
+    "RP",
+    "W-BSC",
+    "BRG",
+)
 
 
 class Craft2dEnv(gym.Env):
     def __init__(
         self,
         n_rows: int,
         n_cols: int,
@@ -98,24 +108,26 @@
                 env_objects=ENVIRONMENT_OBJECTS,
                 inv_objects=INVENTORY_OBJECTS,
                 fps=24,
             )
 
     def reset(
         self,
-        task: str = "get-wood",
         seed: int = None,
         options: dict[str, str] = None,
     ):
         super().reset(seed=seed)
-        # Set task
-        self.task = task
+        np.random.seed(seed)
         # Reset number of steps taken in environment
         self.n_steps = 0
 
+        # Reset task state
+        self.task_object = None
+        self.task_object_count = None
+
         # Object order specified in ENVIRONMENT_OBJECTS
         self.grid = np.zeros((self.n_rows, self.n_cols, self.n_env_objects))
         # Object order specified in INVENTORY_OBJECTS
         self.inventory = np.zeros((self.n_inv_objects,))
 
         # Initialize agent position and direction
         self.agent_position = (0, 0)
@@ -126,27 +138,37 @@
 
             # Add resources to environment
             self._initialize_environment()
             self.cached_grid = self.grid.copy()
         else:
             self.grid = self.cached_grid.copy()
 
-        # Setup island
-        self._initialize_island()
+        # # Setup island
+        # self._initialize_island()
+
+        self.interaction_props = ()
         return self._create_observation()
 
     def step(self, action: int):
-        if action == USE:
-            self._handle_use_action()
+        self.interaction_props = ()
+
+        if action == INTERACT:
+            self._handle_interact_action()
         else:
             self._update_agent_position(action)
             self._update_agent_direction(action)
 
         obs = self._create_observation()
-        reward = 1 if self.inventory[TASKS[self.task]] == 1 else 0
+        reward = 0
+
+        if self.task_object is not None:
+            task_obj_idx = PROPS.index(self.task_object)
+
+            if self.inventory[task_obj_idx] == self.task_object_count:
+                reward = 1
         done = reward == 1
 
         return obs, reward, done
 
     def render(self):
         if self.render_mode is None:
             assert self.spec is not None
@@ -163,41 +185,47 @@
                 inventory=self.inventory,
                 agent_position=self.agent_position,
                 direction=self.direction,
             )
 
     def _create_observation(self):
         # Fill observation with out of bounds
-        obs_grid = np.full((5, 5), fill_value=-1)
+        obs_grid = np.full((3, 3), fill_value=-1)
 
-        for d_r, d_c in product(range(-2, 3), range(-2, 3)):
+        for d_r, d_c in product(range(-1, 2), range(-1, 2)):
             n_r = self.agent_position[0] + d_r
             n_c = self.agent_position[1] + d_c
 
             # Test if out of bounds
             if (n_r >= self.n_rows or n_r < 0) or (n_c >= self.n_cols or n_c < 0):
                 continue
 
-            obs_grid[d_r + 2, d_c + 2] = np.argmax(self.grid[n_r, n_c])
+            if np.max(self.grid[n_r, n_c]) == 0:
+                # Empty cell
+                obs_grid[d_r + 1, d_c + 1] = 0
+            else:
+                # Object
+                obs_grid[d_r + 1, d_c + 1] = np.argmax(self.grid[n_r, n_c]) + 1
 
-        # return (
-        #     .copy(),
-        #     self.inventory.copy(),
-        #     self.direction.copy(),
-        # )
+        if self.task_object is None:
+            task_collected = np.array([0])
+        else:
+            task_collected = np.array([1])
 
         return (
             np.array([self.agent_position[0], self.agent_position[1]]).copy(),
-            self.inventory.copy(),
+            obs_grid.copy(),
             self.direction.copy(),
+            task_collected,
+            self.interaction_props,
         )
 
     def _sample_position(self):
-        row = np.random.randint(1, self.n_rows - 1)
-        col = np.random.randint(1, self.n_cols - 1)
+        row = np.random.randint(2, self.n_rows - 1)
+        col = np.random.randint(2, self.n_cols - 1)
         return row, col
 
     def _initialize_environment(self):
         used_positions = []
 
         for i, object_name in enumerate(ENVIRONMENT_OBJECTS):
             # Skip water and bridge
@@ -279,67 +307,97 @@
             self.direction[0] = 1
         elif action == LEFT:
             self.direction[1] = 1
         elif action == UP:
             self.direction[2] = 1
         elif action == DOWN:
             self.direction[3] = 1
-        elif action == USE:
+        elif action == INTERACT:
             self.direction = last_direction
 
-    def _handle_use_action(self):
+    def _handle_interact_action(self):
         # Cell in front of agent
         itr_row, itr_col = self._get_interaction_cell()
 
         # Test if cell is empty
         if np.max(self.grid[itr_row, itr_col]) == 0:
             return
 
         # Get object type
         object_type = np.argmax(self.grid[itr_row, itr_col])
         object_name = ENVIRONMENT_OBJECTS[object_type]
 
+        if object_name == "princess":
+            if self.task_object is None:
+                self.task_object = np.random.choice(
+                    (
+                        "WD",
+                        "STN",
+                        # "GRS",
+                        "STKS",
+                        # "RP",
+                        "W-BSC",
+                        # "BRG",
+                    )
+                )
+                self.task_object_count = np.random.choice(("M1",))
+                self.interaction_props = (self.task_object, self.task_object_count)
+            else:
+                self.interaction_props = ("P",)
+        elif self.task_object is None:
+            # Cannot interact before task specified
+            return
+
         # Collect resources from environment
         if object_name == "tree":
             self._collect_tree(itr_row, itr_col)
+            self.interaction_props = ("WD", "CL")
         elif object_name == "stone":
             self._collect_stone(itr_row, itr_col)
+            self.interaction_props = ("STN", "CL")
         elif object_name == "grass":
             self._collect_grass(itr_row, itr_col)
+            self.interaction_props = ("GRS", "CL")
         elif object_name == "gem":
             self._collect_gem(itr_row, itr_col)
+            self.interaction_props = ("GM", "CL")
         elif object_name == "water":
             self._handle_water_interaction(itr_row, itr_col)
         elif object_name == "crafting-table":
             self._handle_crafting_interaction()
 
     def _handle_crafting_interaction(self):
         if self.inventory[6] > 0 and self.inventory[7] > 0:
             # Advanced weapon
             self.inventory[8] += 1
             self.inventory[6] -= 1
             self.inventory[7] -= 1
+            self.interaction_props = ("W-ADV", "CL")
         if self.inventory[3] > 0 and self.inventory[1] >= 2:
             # Weapon
             self.inventory[6] += 1
             self.inventory[3] -= 1
             self.inventory[1] -= 2
+            self.interaction_props = ("W-BSC", "CL")
         elif self.inventory[3] > 0 and self.inventory[4] >= 1:
             # Bridge
             self.inventory[5] += 1
             self.inventory[3] -= 1
             self.inventory[4] -= 1
+            self.interaction_props = ("BRG", "CL")
         elif self.inventory[0] > 1:
             # Sticks
             self.inventory[0] -= 2
             self.inventory[3] += 1
+            self.interaction_props = ("STKS", "CL")
         elif self.inventory[2] > 1:
             # Rope
             self.inventory[2] -= 2
             self.inventory[4] += 1
+            self.interaction_props = ("RP", "CL")
 
     def _handle_water_interaction(self, itr_row, itr_col):
         # Place bridge on water if agent has bridge in inventory
         water_idx_env = ENVIRONMENT_OBJECTS.index("water")
         bridge_idx_env = ENVIRONMENT_OBJECTS.index("bridge")
         bridge_idx_inv = INVENTORY_OBJECTS.index("bridge")
```

### Comparing `craft2d-0.1.2/craft2d/render/render.py` & `craft2d-0.1.4/craft2d/render/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ROPE_IMG_PATH = "resources/objects/rope.png"
 BRIDGE_IMG_PATH = "resources/objects/bridge.png"
 WEAPON_BASIC_IMG_PATH = "resources/objects/weapon-basic.png"
 ISLAND_IMG_PATH = "resources/terrain/island.png"
 WATER_IMG_PATH = "resources/terrain/water.png"
 GEM_IMG_PATH = "resources/objects/gem.png"
 WEAPON_ADV_IMG_PATH = "resources/objects/weapon-advanced.png"
+PRINCESS_IMG_PATH = "resources/objects/princess.png"
 
 
 def get_file_path(file_name):
     spec = importlib.util.find_spec("craft2d")
     if spec is None:
         raise ImportError("Package 'craft2d' not found.")
 
@@ -51,16 +52,16 @@
         self.n_rows = n_rows
         self.n_cols = n_cols
         self.env_objects = env_objects
         self.inv_objects = inv_objects
         self.window_width = window_width
         self.window_height = window_height
         self.cell_size = (
-            self.window_width / (self.n_cols + 2),  # +2 for inventory
-            self.window_height / self.n_rows,
+            round(self.window_width / (self.n_cols + 2)),  # +2 for inventory
+            round(self.window_height / self.n_rows),
         )
 
         # Load assets
         self.background_image = self._load_image(get_file_path(BACKGROUND_IMG_PATH))
         self.player_images = self._load_images(PLAYER_IMGS_PATH)
         self.tree_image = self._load_image(get_file_path(TREE_IMG_PATH))
         self.wood_image = self._load_image(get_file_path(WOOD_IMG_PATH))
@@ -75,14 +76,15 @@
         self.weapon_basic_image = self._load_image(get_file_path(WEAPON_BASIC_IMG_PATH))
         self.island_image = self._load_image(get_file_path(ISLAND_IMG_PATH))
         self.water_image = self._load_image(get_file_path(WATER_IMG_PATH))
         self.gem_image = self._load_image(get_file_path(GEM_IMG_PATH))
         self.weapon_advanced_image = self._load_image(
             get_file_path(WEAPON_ADV_IMG_PATH)
         )
+        self.princess_image = self._load_image(get_file_path(PRINCESS_IMG_PATH))
 
         # Initialise pygame
         pygame.init()
         self.clock = pygame.time.Clock()
 
     def _render_background(self, grid):
         for r, c in product(range(self.n_rows), range(self.n_cols)):
@@ -117,59 +119,61 @@
                 self._render_cell(self.stone_image, r, c)
             elif object_name == "grass":
                 self._render_cell(self.grass_image, r, c)
             elif object_name == "crafting-table":
                 self._render_cell(self.crafting_table_image, r, c)
             elif object_name == "gem":
                 self._render_cell(self.gem_image, r, c)
+            elif object_name == "princess":
+                self._render_cell(self.princess_image, r, c)
 
     def _render_player(self, agent_position, direction):
         self._render_cell(
             image=self.player_images[np.argmax(direction)],
             row=agent_position[0],
             col=agent_position[1],
         )
 
     def _render_inventory(self, inventory):
         for idx, count in enumerate(inventory):
             object_name = self.inv_objects[idx]
 
             if object_name == "wood":
                 self._render_cell(image=self.wood_image, row=idx, col=self.n_cols)
-                self._render_text(text="Wood", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Wood", row=idx, col=self.n_cols, loc="top")
             elif object_name == "stone":
                 self._render_cell(image=self.stone_image, row=idx, col=self.n_cols)
-                self._render_text(text="Stone", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Stone", row=idx, col=self.n_cols, loc="top")
             elif object_name == "grass":
                 self._render_cell(image=self.grass_image, row=idx, col=self.n_cols)
-                self._render_text(text="Grass", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Grass", row=idx, col=self.n_cols, loc="top")
             elif object_name == "sticks":
                 self._render_cell(image=self.sticks_image, row=idx, col=self.n_cols)
-                self._render_text(text="Sticks", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Sticks", row=idx, col=self.n_cols, loc="top")
             elif object_name == "rope":
                 self._render_cell(image=self.rope_image, row=idx, col=self.n_cols)
-                self._render_text(text="Rope", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Rope", row=idx, col=self.n_cols, loc="top")
             elif object_name == "bridge":
                 self._render_cell(image=self.bridge_image, row=idx, col=self.n_cols)
-                self._render_text(text="Bridge", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Bridge", row=idx, col=self.n_cols, loc="top")
             elif object_name == "weapon-basic":
                 self._render_cell(
                     image=self.weapon_basic_image, row=idx, col=self.n_cols
                 )
-                self._render_text(text="Weapon", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Weapon", row=idx, col=self.n_cols, loc="top")
             elif object_name == "gem":
                 self._render_cell(image=self.gem_image, row=idx, col=self.n_cols)
-                self._render_text(text="Gem", row=idx, col=self.n_cols, loc="top")
+                # self._render_text(text="Gem", row=idx, col=self.n_cols, loc="top")
             elif object_name == "weapon-advanced":
                 self._render_cell(
                     image=self.weapon_advanced_image, row=idx, col=self.n_cols
                 )
-                self._render_text(
-                    text="Weapon (Adv)", row=idx, col=self.n_cols, loc="top"
-                )
+                # self._render_text(
+                #     text="Weapon (Adv)", row=idx, col=self.n_cols, loc="top"
+                # )
 
             self._render_text(
                 text="X " + str(int(count)), row=idx, col=self.n_cols + 1, size=20
             )
 
     def _render_text(self, text, row, col, size=20, loc="center"):
         font = pygame.font.Font(None, size)
```

### Comparing `craft2d-0.1.2/craft2d/resources/agent/agent-down.png` & `craft2d-0.1.4/craft2d/resources/agent/agent-down.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/agent/agent-left.png` & `craft2d-0.1.4/craft2d/resources/agent/agent-left.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/agent/agent-right.png` & `craft2d-0.1.4/craft2d/resources/agent/agent-right.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/agent/agent-up.png` & `craft2d-0.1.4/craft2d/resources/agent/agent-up.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/farm/plant-large.png` & `craft2d-0.1.4/craft2d/resources/farm/plant-large.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/farm/plant-medium.png` & `craft2d-0.1.4/craft2d/resources/farm/plant-medium.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/farm/plant-small.png` & `craft2d-0.1.4/craft2d/resources/farm/plant-small.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/bridge.png` & `craft2d-0.1.4/craft2d/resources/objects/bridge.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/crafting-table.png` & `craft2d-0.1.4/craft2d/resources/objects/crafting-table.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/gem.png` & `craft2d-0.1.4/craft2d/resources/objects/gem.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/grass.png` & `craft2d-0.1.4/craft2d/resources/objects/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/rope.png` & `craft2d-0.1.4/craft2d/resources/objects/rope.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/sticks.png` & `craft2d-0.1.4/craft2d/resources/objects/sticks.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/stone.png` & `craft2d-0.1.4/craft2d/resources/objects/stone.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/tree.png` & `craft2d-0.1.4/craft2d/resources/objects/tree.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/weapon-advanced.png` & `craft2d-0.1.4/craft2d/resources/objects/weapon-advanced.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/weapon-basic.png` & `craft2d-0.1.4/craft2d/resources/objects/weapon-basic.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/objects/wood.png` & `craft2d-0.1.4/craft2d/resources/objects/wood.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/terrain/grass.png` & `craft2d-0.1.4/craft2d/resources/terrain/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/terrain/island.png` & `craft2d-0.1.4/craft2d/resources/terrain/island.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/craft2d/resources/terrain/water.png` & `craft2d-0.1.4/craft2d/resources/terrain/water.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.2/pyproject.toml` & `craft2d-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft2d"
-version = "0.1.2"
+version = "0.1.4"
 description = ""
 authors = ["Tristan Bester <tristanbester@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.25.1"
```

### Comparing `craft2d-0.1.2/PKG-INFO` & `craft2d-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft2d
-Version: 0.1.2
+Version: 0.1.4
 Summary: 
 Author: Tristan Bester
 Author-email: tristanbester@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

