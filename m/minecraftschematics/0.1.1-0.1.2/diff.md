# Comparing `tmp/minecraftschematics-0.1.1.tar.gz` & `tmp/minecraftschematics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraftschematics-0.1.1.tar", last modified: Sat Jul 22 20:13:08 2023, max compression
+gzip compressed data, was "minecraftschematics-0.1.2.tar", last modified: Mon Jul 24 13:58:43 2023, max compression
```

## Comparing `minecraftschematics-0.1.1.tar` & `minecraftschematics-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/
--rw-r--r--   0 gwern     (1000) gwern     (1000)     3121 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/PKG-INFO
--rw-r--r--   0 gwern     (1000) gwern     (1000)     2807 2023-07-22 20:11:56.000000 minecraftschematics-0.1.1/README.md
-drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/minecraftschematics/
--rw-r--r--   0 gwern     (1000) gwern     (1000)       93 2023-07-22 19:57:12.000000 minecraftschematics-0.1.1/minecraftschematics/__init__.py
--rw-r--r--   0 gwern     (1000) gwern     (1000)     9603 2023-07-22 19:57:39.000000 minecraftschematics-0.1.1/minecraftschematics/schematic.py
--rw-r--r--   0 gwern     (1000) gwern     (1000)     3285 2023-07-22 19:57:52.000000 minecraftschematics-0.1.1/minecraftschematics/utils.py
-drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/minecraftschematics.egg-info/
--rw-r--r--   0 gwern     (1000) gwern     (1000)     3121 2023-07-22 20:13:08.000000 minecraftschematics-0.1.1/minecraftschematics.egg-info/PKG-INFO
--rw-r--r--   0 gwern     (1000) gwern     (1000)      350 2023-07-22 20:13:08.000000 minecraftschematics-0.1.1/minecraftschematics.egg-info/SOURCES.txt
--rw-r--r--   0 gwern     (1000) gwern     (1000)        1 2023-07-22 20:13:08.000000 minecraftschematics-0.1.1/minecraftschematics.egg-info/dependency_links.txt
--rw-r--r--   0 gwern     (1000) gwern     (1000)       13 2023-07-22 20:13:08.000000 minecraftschematics-0.1.1/minecraftschematics.egg-info/requires.txt
--rw-r--r--   0 gwern     (1000) gwern     (1000)       20 2023-07-22 20:13:08.000000 minecraftschematics-0.1.1/minecraftschematics.egg-info/top_level.txt
--rw-r--r--   0 gwern     (1000) gwern     (1000)       38 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/setup.cfg
--rw-r--r--   0 gwern     (1000) gwern     (1000)      803 2023-07-22 20:12:07.000000 minecraftschematics-0.1.1/setup.py
-drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-22 20:13:08.739423 minecraftschematics-0.1.1/tests/
--rw-r--r--   0 gwern     (1000) gwern     (1000)     2756 2023-07-22 19:55:08.000000 minecraftschematics-0.1.1/tests/test_schematic.py
+drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-24 13:58:43.024472 minecraftschematics-0.1.2/
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     3145 2023-07-24 13:58:43.024472 minecraftschematics-0.1.2/PKG-INFO
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     2831 2023-07-24 13:58:22.000000 minecraftschematics-0.1.2/README.md
+drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-24 13:58:43.021139 minecraftschematics-0.1.2/minecraftschematics/
+-rw-r--r--   0 gwern     (1000) gwern     (1000)       93 2023-07-22 19:57:12.000000 minecraftschematics-0.1.2/minecraftschematics/__init__.py
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     9104 2023-07-24 13:27:53.000000 minecraftschematics-0.1.2/minecraftschematics/schematic.py
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     3285 2023-07-22 19:57:52.000000 minecraftschematics-0.1.2/minecraftschematics/utils.py
+drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-24 13:58:43.021139 minecraftschematics-0.1.2/minecraftschematics.egg-info/
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     3145 2023-07-24 13:58:42.000000 minecraftschematics-0.1.2/minecraftschematics.egg-info/PKG-INFO
+-rw-r--r--   0 gwern     (1000) gwern     (1000)      350 2023-07-24 13:58:42.000000 minecraftschematics-0.1.2/minecraftschematics.egg-info/SOURCES.txt
+-rw-r--r--   0 gwern     (1000) gwern     (1000)        1 2023-07-24 13:58:42.000000 minecraftschematics-0.1.2/minecraftschematics.egg-info/dependency_links.txt
+-rw-r--r--   0 gwern     (1000) gwern     (1000)       13 2023-07-24 13:58:42.000000 minecraftschematics-0.1.2/minecraftschematics.egg-info/requires.txt
+-rw-r--r--   0 gwern     (1000) gwern     (1000)       20 2023-07-24 13:58:42.000000 minecraftschematics-0.1.2/minecraftschematics.egg-info/top_level.txt
+-rw-r--r--   0 gwern     (1000) gwern     (1000)       38 2023-07-24 13:58:43.024472 minecraftschematics-0.1.2/setup.cfg
+-rw-r--r--   0 gwern     (1000) gwern     (1000)      803 2023-07-24 13:00:18.000000 minecraftschematics-0.1.2/setup.py
+drwxr-xr-x   0 gwern     (1000) gwern     (1000)        0 2023-07-24 13:58:43.021139 minecraftschematics-0.1.2/tests/
+-rw-r--r--   0 gwern     (1000) gwern     (1000)     2750 2023-07-24 12:51:16.000000 minecraftschematics-0.1.2/tests/test_schematic.py
```

### Comparing `minecraftschematics-0.1.1/PKG-INFO` & `minecraftschematics-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraftschematics
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for working with Minecraft Schematics in Python with numpy
 Author: Gabriel Werneck Paiva
 Author-email: gwerneckpaiva@gmail.com
 License: MIT
 Keywords: python,minecraft,schematic,numpy,nbtlib
 Description-Content-Type: text/markdown
 
@@ -19,32 +19,32 @@
 - Load Minecraft schematic files (.schematic) and read their contents.
 - Access schematic size and dimensions (width, height, length).
 - Get block data as a 3D numpy array representing the blocks in the schematic.
 - Access individual blocks' information, including type and properties.
 
 ## Installation
 
-To install PySchematic, you can use pip:
+To install Minecraft Schematics, you can use pip:
 
 ```bash
-pip install pyschematic
+pip install minecraftschematics
 ```
 
 ## Usage
 
 Here's a quick guide on how to use the `minecraftschematics` library:
 
 ### Schematic Class
 
 The `Schematic` class is the main class of the library. It is used to load schematic files with the `load` method and access the schematic's data.
 
 ```python
 from minecraftschematics import Schematic
 
-schematic = Schematic().load('path/to/your/schematic_file.schematic')
+schematic = Schematic.load('path/to/your/schematic_file.schematic')
 
 print(schematic.size)     # Output: (3, 4, 5)
 print(schematic.width)    # Output: 3
 print(schematic.height)   # Output: 4
 print(schematic.length)   # Output: 5
 
 # Get block data as a 3D numpy array
@@ -75,15 +75,15 @@
 
 - Python 3.10+
 - numpy
 - nbtlib
 
 ## Contributing
 
-If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/pyschematic).
+If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/minecraft-schematics).
 
 ## License
 
 This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
 
 ---
 *This project is based on the Minecraft Schematic format version 2.*
```

### Comparing `minecraftschematics-0.1.1/README.md` & `minecraftschematics-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 - Load Minecraft schematic files (.schematic) and read their contents.
 - Access schematic size and dimensions (width, height, length).
 - Get block data as a 3D numpy array representing the blocks in the schematic.
 - Access individual blocks' information, including type and properties.
 
 ## Installation
 
-To install PySchematic, you can use pip:
+To install Minecraft Schematics, you can use pip:
 
 ```bash
-pip install pyschematic
+pip install minecraftschematics
 ```
 
 ## Usage
 
 Here's a quick guide on how to use the `minecraftschematics` library:
 
 ### Schematic Class
 
 The `Schematic` class is the main class of the library. It is used to load schematic files with the `load` method and access the schematic's data.
 
 ```python
 from minecraftschematics import Schematic
 
-schematic = Schematic().load('path/to/your/schematic_file.schematic')
+schematic = Schematic.load('path/to/your/schematic_file.schematic')
 
 print(schematic.size)     # Output: (3, 4, 5)
 print(schematic.width)    # Output: 3
 print(schematic.height)   # Output: 4
 print(schematic.length)   # Output: 5
 
 # Get block data as a 3D numpy array
@@ -65,15 +65,15 @@
 
 - Python 3.10+
 - numpy
 - nbtlib
 
 ## Contributing
 
-If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/pyschematic).
+If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/minecraft-schematics).
 
 ## License
 
 This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
 
 ---
 *This project is based on the Minecraft Schematic format version 2.*
```

### Comparing `minecraftschematics-0.1.1/minecraftschematics/schematic.py` & `minecraftschematics-0.1.2/minecraftschematics/schematic.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,51 +55,53 @@
 
 
 class Schematic():
     def __init__(self):
         """Representation of a Minecraft schematic."""
         self.raw = None
 
-    def load(self, path: str, force=False):
+    @staticmethod
+    def load(path: str, force=False):
         """Load the schematic from a file.
 
         Args:
             path (str): The path to the schematic file.
             force (bool, optional): Force loading the schematic even if it is an incompatible version. Defaults to False. (Not recommended as it may cause unintended errors.)
 
         Returns:
-            Schematic: The current instance of the Schematic class.
+            Schematic: An instance of the Schematic class.
 
         Raises:
             FileNotFoundError: If the file does not exist.
             nbt.lib.MalformedFileError: If the file cannot be loaded due to a parsing error.
             Exception: If the schematic is an incompatible version and force is False.
         """
         try:
-            self.raw = nbt.load(path)
+            s = Schematic()
+            s.raw = nbt.load(path)
             if (not force):
-                match self.raw['Version']:
+                match s.raw.get('Version'):
                     case None:
                         raise Exception(
                             "Version not found. This is likely due to an old version of the schematic format which this library does not support. Check out https://github.com/cbs228/nbtschematic for a library that supports version 1.")
                     case 1:
                         raise Exception(
                             "Version 1 is not supported as it is an old version of the schematic format. Check out https://github.com/cbs228/nbtschematic for a library that supports version 1.")
                     case 2:
                         pass
                     case _:
                         raise Exception(
-                            f"This library does not fully support the version {self.raw['Version']} of the schematic format. Use force=True to force loading the schematic. This may cause unintended errors.")
+                            f"This library does not fully support the version {s.raw.get('Version')} of the schematic format. Use force=True to force loading the schematic. This may cause unintended errors.")
 
         except FileNotFoundError as e:
             raise FileNotFoundError(f"File not found: {path}") from e
         except nbt.lib.MalformedFileError as e:
             raise nbt.lib.MalformedFileError(
                 f"Error loading schematic: {path}") from e
-        return self
+        return s
 
     @property
     def size(self) -> Tuple[np.short, np.short, np.short]:
         """Tuple: The size of the schematic in (width, height, length)."""
         return self.width, self.height, self.length
 
     @property
@@ -119,22 +121,17 @@
 
     @property
     def blocks(self) -> np.ndarray:
         """np.ndarray: A 3D numpy array representing the blocks in the schematic."""
         # create list with length of last index
         block_data = np.array(self.raw['BlockData'])
         blocks = np.array([None] * len(block_data))
-        palette_inversed = np.array([(Block(blockdata), self.raw['Palette'][blockdata])
-                                     for blockdata in self.raw['Palette']])
 
-        for block, id_in_schematic in palette_inversed:
-            # get positions of all blocks with id_in_schematic in block_data
-            positions = np.where(block_data == id_in_schematic)
-            # set all blocks at positions to block
-            blocks[positions] = block
+        for position, id_in_schematic in enumerate(block_data):
+            blocks[position] = self.palette[id_in_schematic]
 
         # reshape blocks to 3D array
         blocks = blocks.reshape(self.width, self.height, self.length)
 
         for block_entity in self.block_entities:
             blocks[block_entity['Pos'][2], block_entity['Pos'][1],
                    block_entity['Pos'][0]].add_block_entity(block_entity)
@@ -158,20 +155,14 @@
         for blockdata in self.raw['Palette']:
             result[self.raw['Palette'][blockdata]] = Block(blockdata)
 
         return result
 
     @property
     def palette_max(self) -> np.int8:
-
-        # If the palette max is not set, we can infer it from the length of the palette
-        return self.raw['PaletteMax'] or len(self.palette)
-
-    @property
-    def palette_max(self) -> np.int8:
         """The maximum index value for the block palette in the schematic.
 
         This value represents the highest ID of a block in the schematic or the number of unique blocks in the schematic's block palette.
 
         Returns:
             np.int8: The maximum index value for the block palette in the schematic.
         """
```

### Comparing `minecraftschematics-0.1.1/minecraftschematics/utils.py` & `minecraftschematics-0.1.2/minecraftschematics/utils.py`

 * *Files identical despite different names*

### Comparing `minecraftschematics-0.1.1/minecraftschematics.egg-info/PKG-INFO` & `minecraftschematics-0.1.2/minecraftschematics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraftschematics
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for working with Minecraft Schematics in Python with numpy
 Author: Gabriel Werneck Paiva
 Author-email: gwerneckpaiva@gmail.com
 License: MIT
 Keywords: python,minecraft,schematic,numpy,nbtlib
 Description-Content-Type: text/markdown
 
@@ -19,32 +19,32 @@
 - Load Minecraft schematic files (.schematic) and read their contents.
 - Access schematic size and dimensions (width, height, length).
 - Get block data as a 3D numpy array representing the blocks in the schematic.
 - Access individual blocks' information, including type and properties.
 
 ## Installation
 
-To install PySchematic, you can use pip:
+To install Minecraft Schematics, you can use pip:
 
 ```bash
-pip install pyschematic
+pip install minecraftschematics
 ```
 
 ## Usage
 
 Here's a quick guide on how to use the `minecraftschematics` library:
 
 ### Schematic Class
 
 The `Schematic` class is the main class of the library. It is used to load schematic files with the `load` method and access the schematic's data.
 
 ```python
 from minecraftschematics import Schematic
 
-schematic = Schematic().load('path/to/your/schematic_file.schematic')
+schematic = Schematic.load('path/to/your/schematic_file.schematic')
 
 print(schematic.size)     # Output: (3, 4, 5)
 print(schematic.width)    # Output: 3
 print(schematic.height)   # Output: 4
 print(schematic.length)   # Output: 5
 
 # Get block data as a 3D numpy array
@@ -75,15 +75,15 @@
 
 - Python 3.10+
 - numpy
 - nbtlib
 
 ## Contributing
 
-If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/pyschematic).
+If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/gwerneckpaiva/minecraft-schematics).
 
 ## License
 
 This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
 
 ---
 *This project is based on the Minecraft Schematic format version 2.*
```

### Comparing `minecraftschematics-0.1.1/setup.py` & `minecraftschematics-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "minecraftschematics"
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 DESCRIPTION = "A library for working with Minecraft Schematics in Python with numpy"
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
     name=NAME,
```

### Comparing `minecraftschematics-0.1.1/tests/test_schematic.py` & `minecraftschematics-0.1.2/tests/test_schematic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tests/test_minecraft_schematic.py
 
 from os import path
 import json
 import nbtlib as nbt
 import numpy as np
 
-from pyschematic import Block, Schematic
+from minecraftschematics import Block, Schematic
 
 # Test data
 all_blocks = 'newblocks.schem'
 all_blocks_directory = path.join(
     path.dirname(__file__), "schematics", all_blocks)
 
 house = 'house.schem'
@@ -46,51 +46,51 @@
     block = Block(block_data)
     assert block.raw_properties == "east=none,north=side,power=0,south=side,west=none"
 
 # Schematic class tests
 
 
 def test_schematic_load():
-    schematic = Schematic().load(all_blocks_directory)
+    schematic = Schematic.load(all_blocks_directory)
     assert isinstance(schematic.raw, nbt.Compound)
 
 
 def test_schematic_blocks_shape():
-    schematic = Schematic().load(all_blocks_directory)
+    schematic = Schematic.load(all_blocks_directory)
     schematicnbt = nbt.load(all_blocks_directory)
     expected_width = schematicnbt["Width"]
     expected_height = schematicnbt["Height"]
     expected_length = schematicnbt["Length"]
 
     blocks = schematic.blocks
     assert blocks.shape == (expected_width, expected_height, expected_length)
 
 
 def test_schematic_blocks():
-    schematic = Schematic().load(all_blocks_directory)
+    schematic = Schematic.load(all_blocks_directory)
     print(schematic.blocks)
     assert schematic.blocks[0, 0, 0] == Block("minecraft:packed_ice")
 
 
 def test_offset():
-    schematic = Schematic().load(house_directory)
+    schematic = Schematic.load(house_directory)
     assert schematic.offset == (-6, 36, 24)
 
 
 def test_worldedit_offset():
     schematic = Schematic().load(house_directory)
     assert schematic.worldedit_offset == (-10, -1, 8)
 
 
 def test_palette():
-    schematic = Schematic().load(house_directory)
+    schematic = Schematic.load(house_directory)
     assert schematic.palette[0] == Block("minecraft:water[level=0]")
 
 
 def test_palette_max():
-    schematic = Schematic().load(house_directory)
+    schematic = Schematic.load(house_directory)
     assert schematic.palette_max == 69
 
 
 def test_block_entities():
-    schematic = Schematic().load(block_entities_directory)
+    schematic = Schematic.load(block_entities_directory)
     assert json.loads(schematic.block_entities[0]['front_text']['messages'][1])['text'] == 'Hello world'
```

