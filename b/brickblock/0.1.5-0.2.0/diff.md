# Comparing `tmp/brickblock-0.1.5.tar.gz` & `tmp/brickblock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickblock-0.1.5.tar", max compression
+gzip compressed data, was "brickblock-0.2.0.tar", max compression
```

## Comparing `brickblock-0.1.5.tar` & `brickblock-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35823 2023-07-15 07:40:33.964780 brickblock-0.1.5/LICENSE
--rw-r--r--   0        0        0     1392 2023-07-19 21:31:24.895120 brickblock-0.1.5/README.md
--rw-r--r--   0        0        0       31 2023-07-15 12:28:30.690454 brickblock-0.1.5/brickblock/__init__.py
--rw-r--r--   0        0        0    22692 2023-07-20 19:38:04.861242 brickblock-0.1.5/brickblock/objects.py
--rw-r--r--   0        0        0    12781 2023-07-20 20:15:22.713412 brickblock-0.1.5/brickblock/space.py
--rw-r--r--   0        0        0      535 2023-07-20 20:29:40.582673 brickblock-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 brickblock-0.1.5/setup.py
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 brickblock-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-15 07:40:33.964780 brickblock-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1470 2023-07-24 19:18:19.551792 brickblock-0.2.0/README.md
+-rw-r--r--   0        0        0       31 2023-07-15 12:28:30.690454 brickblock-0.2.0/brickblock/__init__.py
+-rw-r--r--   0        0        0    22917 2023-07-21 09:08:13.965513 brickblock-0.2.0/brickblock/objects.py
+-rw-r--r--   0        0        0    19290 2023-07-24 18:54:24.796383 brickblock-0.2.0/brickblock/space.py
+-rw-r--r--   0        0        0      535 2023-07-24 19:12:15.039393 brickblock-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 brickblock-0.2.0/setup.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 brickblock-0.2.0/PKG-INFO
```

### Comparing `brickblock-0.1.5/LICENSE` & `brickblock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brickblock-0.1.5/README.md` & `brickblock-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.
 
 ## Core abstractions
 
 At the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
 
-There are objects used for composing visualisations in Brickblock, such as the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
+There are objects used for composing visualisations in Brickblock, such as the `Cube`. Objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths. They can also be mutated - and can be selected by name, base vector, or various IDs.
 
 Having these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
 
 ## Contributing
 
 Contributions are more than welcome! There is a very rough TODO in [todo.md](todo.md) that outlines both short- and long-term goals for the library. However, there are some rules:
```

### Comparing `brickblock-0.1.5/brickblock/objects.py` & `brickblock-0.2.0/brickblock/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         # not with 3D objects and the notion of left/right etc. You need to
         # transpose or flip the actual data (or the axes), and this is the
         # simplest way to achieve this. Of course, the flip-side is that now you
         # are saying the z-axis corresponds to height in Brickblock, which is
         # not ideal.
         # TODO: Have this as a transform for matplotlib and have your own
         # representation instead.
+        # The below basis vectors in that order actually define the transform
+        # you need. You could reshape the entire matrix in `render` and apply
+        # a single matmul to all the data, or just swap the columns.
         w, h, d = base_vector
         base_vector = np.array([w, d, h])
         self._width_basis_vector = np.array([1, 0, 0])
         self._height_basis_vector = np.array([0, 0, 1])
         self._depth_basis_vector = np.array([0, 1, 0])
 
         points = np.array(
```

### Comparing `brickblock-0.1.5/brickblock/space.py` & `brickblock-0.2.0/brickblock/space.py`

 * *Files 21% similar despite different names*

```diff
@@ -236,14 +236,162 @@
         if name is not None:
             if name in self.cuboid_names.keys():
                 raise Exception(
                     f"There already exists an object with name {name}."
                 )
             self.cuboid_names[name] = primitive_ids
 
+    # TODO: Decide how deletion should be implemented. Masking columns seem the
+    # most logical, but this could be an issue for memory consumption. On the
+    # other hand, 'actual deletion' would involve potentially expensive memory
+    # shuffling.
+    # Moreover, should you even be worrying about deletion? Masking is what you
+    # really want in virtually all cases. Deletion should actually be quite rare
+    # unless a user does something dumb or adds crazy numbers of objects.
+
+    def mutate_by_coordinate(self, coordinate: np.array, **kwargs) -> None:
+        """
+        Mutate the visual metadata of all objects - composite or primitive, with
+        base vectors equal to `coordinate` - with the named arguments in
+        `kwargs`.
+
+        Primitives that are part of composites are not included - that is, if
+        `coordinate` intersects with a composite on any point other than its
+        base vector, none of its primitives will be updated.
+
+        Note that the base vector is defined as the bottom-left-front-most point
+        of an object, primitive or composite.
+
+        # Args
+            coordinate: The coordinate which is compared to the base vector of
+                all objects in the space.
+            kwargs: Sequence of named arguments that contain updated visual
+                property values.
+        """
+        if coordinate.shape != (3,):
+            raise ValueError(
+                "Coordinates are three-dimensional, the input vector should be "
+                "3D."
+            )
+
+        # Map the coordinate to the correct representation.
+        # TODO: Decouple the user from a fixed basis.
+        w, h, d = coordinate
+        coordinate = np.array([w, d, h])
+
+        # First gather the IDs of primitive entries that match the coordinate.
+        matching_base_vectors = []
+        primitives_to_update = []
+        current_idx = 0
+
+        for idx in range(self.primitive_counter):
+            primitive = self.cuboid_coordinates[idx]
+            if np.array_equal(primitive[0, 0], coordinate):
+                matching_base_vectors.append(idx)
+
+        # Find all objects (primitive or composite) corresponding to those IDs.
+        for scene_id in sorted(self.cuboid_index.keys()):
+            for timestep_id in sorted(self.cuboid_index[scene_id].keys()):
+                primitive_ids = self.cuboid_index[scene_id][timestep_id]
+                # Because we gathered matching_base_vectors in order, and the
+                # bottom-left-front point of all objects is the first point, we
+                # can check just the first primitive_id of the list for both
+                # primitives and composites.
+
+                # Skip forward if you caught intermediate primitives.
+                while matching_base_vectors[current_idx] < primitive_ids[0]:
+                    current_idx += 1
+
+                if primitive_ids[0] == matching_base_vectors[current_idx]:
+                    primitives_to_update.extend(primitive_ids)
+                    current_idx += 1
+
+        self._mutate_by_primitive_ids(primitives_to_update, **kwargs)
+
+    def mutate_by_name(self, name: str, **kwargs) -> None:
+        """
+        Mutate the visual metadata of the object - composite or primitive, that
+        has its name equal to `name` - with the named arguments in `kwargs`.
+
+        # Args
+            name: The name of the object in the space to update.
+            kwargs: Sequence of named arguments that contain updated visual
+                property values.
+        """
+        if name not in self.cuboid_names.keys():
+            raise ValueError("The provided name does not exist in this space.")
+
+        primitive_ids = self.cuboid_names[name]
+
+        self._mutate_by_primitive_ids(primitive_ids, **kwargs)
+
+    def mutate_by_timestep(self, input_timestep: int, **kwargs) -> None:
+        """
+        Mutate the visual metadata of the object - composite or primitive, that
+        was created at timestep `input_timestep` - with the named arguments in
+        `kwargs`.
+
+        # Args
+            name: The name of the object in the space to update.
+            kwargs: Sequence of named arguments that contain updated visual
+                property values.
+        """
+        if (input_timestep < 0) or (input_timestep > self.time_step):
+            raise ValueError("The provided timestep is invalid in this space.")
+
+        for scene_id in sorted(self.cuboid_index.keys()):
+            for timestep_id in sorted(self.cuboid_index[scene_id].keys()):
+                if timestep_id == input_timestep:
+                    self._mutate_by_primitive_ids(
+                        self.cuboid_index[scene_id][timestep_id], **kwargs
+                    )
+                    break
+
+    def mutate_by_scene(self, input_scene: int, **kwargs) -> None:
+        """
+        Mutate the visual metadata of the object - composite or primitive, that
+        was created at timestep `input_timestep` - with the named arguments in
+        `kwargs`.
+
+        # Args
+            name: The name of the object in the space to update.
+            kwargs: Sequence of named arguments that contain updated visual
+                property values.
+        """
+        if (input_scene < 0) or (input_scene > self.scene_counter):
+            raise ValueError("The provided scene ID is invalid in this space.")
+
+        for scene_id in sorted(self.cuboid_index.keys()):
+            for timestep_id in sorted(self.cuboid_index[scene_id].keys()):
+                if scene_id == input_scene:
+                    self._mutate_by_primitive_ids(
+                        self.cuboid_index[scene_id][timestep_id], **kwargs
+                    )
+            break
+
+    def _mutate_by_primitive_ids(
+        self, primitive_ids: list[int], **kwargs
+    ) -> None:
+        """
+        Mutate the visual metadata of all primitives given by `primitive_ids`
+        with the named arguments in `kwargs`.
+
+        # Args
+            primitive_ids: The IDs of all the primitives in the space to update.
+            kwargs: Sequence of named arguments that contain updated visual
+                property values.
+        """
+        for key in kwargs.keys():
+            if key not in self.cuboid_visual_metadata.keys():
+                raise KeyError(
+                    "The provided key doesn't match any valid visual property."
+                )
+            for primitive_id in primitive_ids:
+                self.cuboid_visual_metadata[key][primitive_id] = kwargs[key]
+
     def snapshot(self) -> None:
         """
         Store the current state of the space as a scene, used for rendering.
 
         Note that valid scenes must have 1+ transforms - i.e. adding,
         deleting, or mutating an object, must be present in a scene.
         """
```

### Comparing `brickblock-0.1.5/pyproject.toml` & `brickblock-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brickblock"
-version = "0.1.5"
+version = "0.2.0"
 description = "A fun visualisation library for those that like boxes"
 authors = ["Daniel Soutar <danielsoutar144@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/danielsoutar/brickblock"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `brickblock-0.1.5/setup.py` & `brickblock-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.7.2,<4.0.0', 'numpy>=1.25.1,<2.0.0', 'pytest>=7.4.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'brickblock',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': 'A fun visualisation library for those that like boxes',
-    'long_description': "# Brickblock: A fun visualisation library for those that like boxes\n\nThis is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.\n\n## Core abstractions\n\nAt the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.\n\nThere are objects used for composing visualisations in Brickblock, such as the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.\n\nHaving these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.\n\n## Contributing\n\nContributions are more than welcome! There is a very rough TODO in [todo.md](todo.md) that outlines both short- and long-term goals for the library. However, there are some rules:\n\n* Always follow the [code of conduct](CODE_OF_CONDUCT.md)\n* All the tests should be passing with your change\n* Explain your change (PR template coming soon)\n* Add relevant tests and docstrings\n* Format your changes with `black`\n",
+    'long_description': "# Brickblock: A fun visualisation library for those that like boxes\n\nThis is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.\n\n## Core abstractions\n\nAt the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.\n\nThere are objects used for composing visualisations in Brickblock, such as the `Cube`. Objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths. They can also be mutated - and can be selected by name, base vector, or various IDs.\n\nHaving these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.\n\n## Contributing\n\nContributions are more than welcome! There is a very rough TODO in [todo.md](todo.md) that outlines both short- and long-term goals for the library. However, there are some rules:\n\n* Always follow the [code of conduct](CODE_OF_CONDUCT.md)\n* All the tests should be passing with your change\n* Explain your change (PR template coming soon)\n* Add relevant tests and docstrings\n* Format your changes with `black`\n",
     'author': 'Daniel Soutar',
     'author_email': 'danielsoutar144@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/danielsoutar/brickblock',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `brickblock-0.1.5/PKG-INFO` & `brickblock-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brickblock
-Version: 0.1.5
+Version: 0.2.0
 Summary: A fun visualisation library for those that like boxes
 Home-page: https://github.com/danielsoutar/brickblock
 Author: Daniel Soutar
 Author-email: danielsoutar144@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,15 @@
 
 This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.
 
 ## Core abstractions
 
 At the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
 
-There are objects used for composing visualisations in Brickblock, such as the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
+There are objects used for composing visualisations in Brickblock, such as the `Cube`. Objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths. They can also be mutated - and can be selected by name, base vector, or various IDs.
 
 Having these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
 
 ## Contributing
 
 Contributions are more than welcome! There is a very rough TODO in [todo.md](todo.md) that outlines both short- and long-term goals for the library. However, there are some rules:
```

