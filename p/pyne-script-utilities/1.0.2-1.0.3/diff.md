# Comparing `tmp/pyne_script_utilities-1.0.2.tar.gz` & `tmp/pyne_script_utilities-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyne_script_utilities-1.0.2.tar", last modified: Sun Jul 23 09:30:38 2023, max compression
+gzip compressed data, was "pyne_script_utilities-1.0.3.tar", last modified: Mon Jul 24 17:46:30 2023, max compression
```

## Comparing `pyne_script_utilities-1.0.2.tar` & `pyne_script_utilities-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/
--rw-r--r--   0 krijn     (1000) krijn     (1000)    35148 2023-07-06 09:11:48.000000 pyne_script_utilities-1.0.2/LICENSE
--rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/PKG-INFO
--rw-r--r--   0 krijn     (1000) krijn     (1000)      613 2023-07-19 19:47:36.000000 pyne_script_utilities-1.0.2/README.md
--rw-r--r--   0 krijn     (1000) krijn     (1000)      727 2023-07-23 09:27:44.000000 pyne_script_utilities-1.0.2/pyproject.toml
--rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/setup.cfg
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/src/
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/src/pyne_script/
--rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-22 13:56:07.000000 pyne_script_utilities-1.0.2/src/pyne_script/__init__.py
--rw-r--r--   0 krijn     (1000) krijn     (1000)    20703 2023-07-23 09:27:11.000000 pyne_script_utilities-1.0.2/src/pyne_script/series.py
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-23 09:30:38.159611 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/
--rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-23 09:30:38.000000 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/PKG-INFO
--rw-r--r--   0 krijn     (1000) krijn     (1000)      330 2023-07-23 09:30:38.000000 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)        1 2023-07-23 09:30:38.000000 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)        6 2023-07-23 09:30:38.000000 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/requires.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)       12 2023-07-23 09:30:38.000000 pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)    35148 2023-07-06 09:11:48.000000 pyne_script_utilities-1.0.3/LICENSE
+-rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/PKG-INFO
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      613 2023-07-19 19:47:36.000000 pyne_script_utilities-1.0.3/README.md
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      727 2023-07-24 17:44:52.000000 pyne_script_utilities-1.0.3/pyproject.toml
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/setup.cfg
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/src/
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/src/pyne_script/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-22 13:56:07.000000 pyne_script_utilities-1.0.3/src/pyne_script/__init__.py
+-rw-r--r--   0 krijn     (1000) krijn     (1000)    22728 2023-07-24 17:34:09.000000 pyne_script_utilities-1.0.3/src/pyne_script/series.py
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 17:46:30.642702 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 17:46:30.000000 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      330 2023-07-24 17:46:30.000000 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)        1 2023-07-24 17:46:30.000000 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)        6 2023-07-24 17:46:30.000000 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/requires.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       12 2023-07-24 17:46:30.000000 pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/top_level.txt
```

### Comparing `pyne_script_utilities-1.0.2/LICENSE` & `pyne_script_utilities-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyne_script_utilities-1.0.2/PKG-INFO` & `pyne_script_utilities-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyne_script_utilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A set of utility sub-modules that allow for code structure similar to pinescript in python
 Author: 80sVectorz
 Project-URL: Homepage, https://github.com/80sVectorz/pyne_script
 Project-URL: Bug Tracker, https://github.com/80sVectorz/pyne_script/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

### Comparing `pyne_script_utilities-1.0.2/README.md` & `pyne_script_utilities-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyne_script_utilities-1.0.2/pyproject.toml` & `pyne_script_utilities-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["pyne_script*"]
 namespaces = false
 
 [project]
 name = "pyne_script_utilities"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="80sVectorz"},
 ]
 description = "A set of utility sub-modules that allow for code structure similar to pinescript in python"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["numpy"]
```

### Comparing `pyne_script_utilities-1.0.2/src/pyne_script/series.py` & `pyne_script_utilities-1.0.3/src/pyne_script/series.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 class SeriesHeadObject:
     value: float | int
     key: str | int
     track_history_mode: int
     window_size: int | None
     values: np.ndarray | None
     history: list[int | float] | None
+    head_position: list[int]
 
     def __init__(
         self,
         value: float | int,
         key: str | int,
         track_history_mode: int,
+        head_position: list[int],
         window_size: int | None = 200,
         values: np.ndarray | None = None,
         history: None | list[int | float] = None,
     ) -> None:
         self.value = value
         self.key = key
         self.track_history_mode = track_history_mode
         self.window_size = window_size
         self.values = values
         self.history = history
+        self.head_position = head_position
 
     def __setitem__(self, *_) -> None:
         raise SeriesCannotMutateHistory()
 
     def index(self, i: int, error: bool = False) -> tuple[int, bool, bool]:
         overflow_window = False
         overflow_full = False
@@ -67,42 +70,62 @@
                     if self.track_history_mode == 1:
                         values = self.history
                     if self.track_history_mode in [0, 2] and not overflow_window:
                         values = self.values
                     else:
                         values = self.history
 
-                    out.append(values[-index])  # type: ignore
+                    out.append(values[:-1][-index])  # type: ignore
                     break
                 case slice():
                     values = None
-                    for slice_index in [index.start, index.stop]:
+                    indices = {}
+                    for index_type, slice_index in {
+                        "start": index.start,
+                        "stop": index.stop,
+                    }.items():
+                        if slice_index == None:
+                            indices[index_type] = slice_index
+                            if self.track_history_mode in [1, 2]:
+                                values = self.history
+                            elif self.track_history_mode == 0:
+                                values = self.values[
+                                    -min(self.window_size, self.head_position[0]) :
+                                ]
+                                if self.window_size == self.head_position[0] + 1:
+                                    values = self.values
+                            continue
                         index_checked = self.index(slice_index, error=True)
                         overflow_window = index_checked[1]
                         if self.track_history_mode == 1:
                             values = self.history
                         if (
                             values != self.history
                             and self.track_history_mode in [0, 2]
                             and not overflow_window
                         ):
-                            values = self.values
+                            values = self.values[
+                                -min(self.window_size, self.head_position[0]) :
+                            ]
+                            if self.window_size == self.head_position[0] + 1:
+                                values = self.values
                         else:
                             values = self.history
+                        indices[index_type] = -slice_index
 
                     if index.step:
                         try:
                             out.append(
-                                values[-index.start : -index.stop : index.step]  # type: ignore
+                                values[indices["start"] : indices["stop"] : index.step]  # type: ignore
                             )
                         except:
                             raise SeriesIndexError(self.key)
                     else:
                         try:
-                            out.append(values[-index.start : -index.stop])  # type: ignore
+                            out.append(values[indices["start"] : indices["stop"]])  # type: ignore
                         except:
                             raise SeriesIndexError(self.key)
 
                     break
                 case _:
                     raise InvalidSeriesIndex(self.key)
 
@@ -113,100 +136,112 @@
 
 class SeriesHeadObjectFloat(float, SeriesHeadObject):
     def __new__(
         cls,
         val: float,
         key: str | int,
         track_history_mode: int,
+        head_position: list[int],
         window_size: int | None = 200,
         values: np.ndarray | None = None,
         history: None | list[int | float] = None,
     ) -> float:
         i = float.__new__(SeriesHeadObjectFloat, val)
         i.values = values
         i.key = key
         i.track_history_mode = track_history_mode
+        i.head_position = head_position
         i.window_size = window_size
         i.values = values
         i.history = history
         return i
 
     def __init__(
         self,
         val: float,
         key: str | int,
         track_history_mode: int,
+        head_position: list[int],
         window_size: int | None = 200,
         values: np.ndarray | None = None,
         history: None | list[int | float] = None,
     ) -> None:
         self.val = val
         self.key = key
         self.track_history_mode = track_history_mode
+        self.head_position = head_position
         self.window_size = window_size
         self.values = values
         self.history = history
-        super().__init__(val, key, track_history_mode, window_size, values, history)
+        super().__init__(
+            val, key, track_history_mode, head_position, window_size, values, history
+        )
 
     def __str__(self):
         return self.value.__str__()
 
     def __repr__(self):
         return self.__str__()
 
 
 class SeriesHeadObjectInteger(int, SeriesHeadObject):
     def __new__(
         cls,
         val: int,
         key: str | int,
         track_history_mode: int,
+        head_position: list[int],
         window_size: int | None = 200,
         values: np.ndarray | None = None,
         history: None | list[int | float] = None,
     ) -> int:
         i = int.__new__(SeriesHeadObjectInteger, val)
         i.values = values
         i.key = key
         i.track_history_mode = track_history_mode
+        i.head_position = head_position
         i.window_size = window_size
         i.values = values
         i.history = history
         return i
 
     def __init__(
         self,
         val: int,
         key: str | int,
         track_history_mode: int,
+        head_position: list[int],
         window_size: int | None = 200,
         values: np.ndarray | None = None,
         history: None | list[int | float] = None,
     ) -> None:
         self.val = val
         self.key = key
         self.track_history_mode = track_history_mode
+        self.head_position = head_position
         self.window_size = window_size
         self.values = values
         self.history = history
-        super().__init__(val, key, track_history_mode, window_size, values, history)
+        super().__init__(
+            val, key, track_history_mode, head_position, window_size, values, history
+        )
 
     def __str__(self):
         return self.value.__str__()
 
     def __repr__(self):
         return self.__str__()
 
 
 class Series:
     keys: set
     key_mappings: dict[str | int, int]
     values: dict[type, np.ndarray | None]
     heads: dict[type, np.ndarray | None]
-    head_positions: int
+    head_positions: list[int]
     window_size: int
     heads_assigned: set[int | str]
     series_types: dict[str | int, type]
 
     track_history_mode: int
     history: dict[str | int, list[int | float]] | None
 
@@ -235,14 +270,15 @@
         - (default:200) window_size: The size of the rolling window when using track_history_modes 0 or 2.
 
         - (default: int:int64 float:float128) dtypes: dtypes for np arrays of different source types.
         """
         self.keys = set()
         self.key_mappings = {}
         self.series_types = {}
+        self.head_positions = [0]
         self.values = {}
         self.heads = {}
         self.track_history_mode = track_history_mode
         self.window_size = window_size
 
         if self.track_history_mode not in [0, 1, 2]:
             pass
@@ -284,29 +320,29 @@
                     )
                 else:
                     self.heads[float] = np.zeros(
                         len(key_value_pairs.values()), dtype=dtypes[float]
                     )
 
                 self.heads_assigned = set(key_value_pairs.keys())
-                self.head_positions = length_ticker - 1
+                self.head_positions[0] = length_ticker - 1
+
+                self.heads[series_type][self.key_mappings[key]] = copy.copy(
+                    key_value_pairs[key][-1]
+                )
 
                 if self.track_history_mode in [1, 2]:  # use unbounded history tracking
                     self.history = {}
                     for key in self.key_mappings.keys():
                         self.history[key] = []
                         if length_ticker != 1:
                             self.history[key] += copy.deepcopy(
                                 key_value_pairs[key][:-1]
                             )
 
-                        self.heads[series_type][self.key_mappings[key]] = copy.copy(
-                            key_value_pairs[key][-1]
-                        )
-
                 if self.track_history_mode in [
                     0,
                     2,
                 ]:  # use bounded rolling window tracking
                     if series_type == int:
                         self.values[int] = np.zeros(
                             (len(key_value_pairs.values()), window_size),
@@ -315,18 +351,25 @@
                     else:
                         self.values[float] = np.zeros(
                             (len(key_value_pairs.values()), window_size),
                             dtype=dtypes[float],
                         )
 
                     if length_ticker > 2:
-                        self.values[series_type][ #type: ignore
-                            i, -min([window_size, length_ticker - 2]) :
-                        ] = np.array(key_value_pairs[key])[
-                            -min([window_size, length_ticker - 1]) : -1]  # type: ignore
+                        B = np.pad(
+                            np.array(
+                                key_value_pairs[key][
+                                    -min(window_size + 1, length_ticker) : -1
+                                ]
+                            ),
+                            (max(window_size - (length_ticker - 1), 0), 0),
+                            "constant",
+                            constant_values=(0),
+                        )
+                        self.values[series_type][i] += B  # type: ignore
 
         if initial_update:
             self.update()
 
     def index(
         self, i: int, error: bool = False, key: str | None = None
     ) -> tuple[int, bool, bool]:
@@ -358,16 +401,16 @@
                 unassigned_heads.append(key)
             else:
                 self.heads_assigned.remove(key)
 
         if not all_assigned:
             raise PrematureSeriesUpdate(unassigned_heads)
 
-        index = self.index(self.head_positions + 1)
-        self.head_positions = index[0]
+        index = self.index(self.head_positions[0] + 1)
+        self.head_positions[0] = index[0]
         if self.track_history_mode in [0, 2]:
             if self.track_history_mode in [0, 2]:
                 if int in self.values.keys():
                     self.values[int] = np.roll(self.values[int], (0, -1))  # type: ignore
                     self.values[int][:, -1] = self.heads[int]  # type: ignore
                 if float in self.values.keys():
                     self.values[float] = np.roll(self.values[float], (0, -1))  # type: ignore
@@ -381,79 +424,83 @@
         self, key: int | str
     ) -> SeriesHeadObjectFloat | SeriesHeadObjectInteger:
         if isinstance(key, list | tuple):
             raise InvalidSeriesIndex()
 
         if isinstance(key, str | int):
             if key in self.keys:
-                if self.head_positions > 0:
+                if self.head_positions[0] > 0:
                     values = None
                     history = None
                     if self.track_history_mode in [0, 2]:
-                        values = self.values[self.series_types[key]][self.key_mappings[key]][:-1]  # type: ignore
+                        values = self.values[self.series_types[key]][self.key_mappings[key]]  # type: ignore
                     if self.track_history_mode in [1, 2]:
-                        history = self.history[key][:-1]  # type: ignore
+                        history = self.history[key]  # type: ignore
                     if self.series_types[key] == int:
                         return SeriesHeadObjectInteger(
                             val=int(self.heads[int][self.key_mappings[key]]),
                             key=key,
                             track_history_mode=self.track_history_mode,
+                            head_position=self.head_positions,
                             window_size=self.window_size,
                             values=values,
                             history=history,
                         )
                     else:
                         return SeriesHeadObjectFloat(
                             self.heads[float][self.key_mappings[key]],
                             key=key,
                             track_history_mode=self.track_history_mode,
+                            head_position=self.head_positions,
                             window_size=self.window_size,
                             values=values,
                             history=history,
                         )
                 else:
                     raise UnAssignedHead(key)
             else:
                 raise NonExistentHead(key, "get")
         else:
             raise InvalidSeriesIndex()
 
     def __getattribute__(self, __name: str) -> Any:
         keys = None
         try:
-            keys = object.__getattribute__(self,"keys")
+            keys = object.__getattribute__(self, "keys")
         except:
             pass
         if keys and __name in keys:
             return self.__getitem__(__name)
-        return object.__getattribute__(self,__name)
+        return object.__getattribute__(self, __name)
 
     def __setitem__(self, key: str | int, value: int | float) -> None:
         if isinstance(key, list | tuple):
             raise InvalidSeriesIndex
 
         if isinstance(key, str | int):
             if key in self.keys:
-                self.heads[self.series_types[key]][self.key_mappings[key]] = self.series_types[key](value)
+                self.heads[self.series_types[key]][
+                    self.key_mappings[key]
+                ] = self.series_types[key](value)
                 self.heads_assigned.add(key)
             else:
                 raise NonExistentHead(key, "set")
         else:
             raise InvalidSeriesIndex()
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         keys = None
         try:
-            keys = object.__getattribute__(self,"keys")
+            keys = object.__getattribute__(self, "keys")
         except:
             pass
         if keys and __name in keys:
-            self.__setitem__(__name,__value)
+            self.__setitem__(__name, __value)
             return
-        object.__setattr__(self,__name,__value)
+        object.__setattr__(self, __name, __value)
 
 
 class PyneSeriesException(Exception):
     """The base class for any pyne script series related exceptions."""
 
     def __init__(self, *args) -> None:
         self.args = args
@@ -555,14 +602,15 @@
 class SeriesInvalidKeyValuePairs_Format(PyneSeriesException):
     """When Series init reveives invalid key value pairs with invalid key types"""
 
     def __str__(self) -> str:
         msg = """Series init recieved invalid key value pairs: Invalid format. Dictionary of string or int keys and equal length numeric list value pairs excpected."""
         return msg
 
+
 class SeriesInvalidKeyValuePairs_Duplicate(PyneSeriesException):
     """When Series init reveives key value pairs with duplicate keys
 
     Args:
     0. Key
     """
```

### Comparing `pyne_script_utilities-1.0.2/src/pyne_script_utilities.egg-info/PKG-INFO` & `pyne_script_utilities-1.0.3/src/pyne_script_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyne-script-utilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A set of utility sub-modules that allow for code structure similar to pinescript in python
 Author: 80sVectorz
 Project-URL: Homepage, https://github.com/80sVectorz/pyne_script
 Project-URL: Bug Tracker, https://github.com/80sVectorz/pyne_script/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

