# Comparing `tmp/pydantic_numpy-2.2.2.tar.gz` & `tmp/pydantic_numpy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-2.2.2.tar", max compression
+gzip compressed data, was "pydantic_numpy-3.0.0.tar", max compression
```

## Comparing `pydantic_numpy-2.2.2.tar` & `pydantic_numpy-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,20 @@
--rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-2.2.2/LICENSE
--rw-r--r--   0        0        0     2055 2023-04-23 14:42:01.570137 pydantic_numpy-2.2.2/README.md
--rw-r--r--   0        0        0      215 2023-04-23 14:42:01.571137 pydantic_numpy-2.2.2/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0     2580 2023-04-29 07:57:37.210284 pydantic_numpy-2.2.2/pydantic_numpy/dtype.py
--rw-r--r--   0        0        0     5236 2023-07-18 10:02:41.536876 pydantic_numpy-2.2.2/pydantic_numpy/model.py
--rw-r--r--   0        0        0     3153 2023-03-17 05:45:48.795212 pydantic_numpy-2.2.2/pydantic_numpy/ndarray.py
--rw-r--r--   0        0        0     1023 2023-07-18 10:05:20.705498 pydantic_numpy-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 pydantic_numpy-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1967 2023-07-24 07:26:03.954095 pydantic_numpy-3.0.0/README.md
+-rw-r--r--   0        0        0      189 2023-07-24 08:00:18.252802 pydantic_numpy-3.0.0/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 08:09:14.284263 pydantic_numpy-3.0.0/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0     5666 2023-07-24 11:20:43.842009 pydantic_numpy-3.0.0/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0     2005 2023-07-24 11:04:27.972235 pydantic_numpy-3.0.0/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0     7428 2023-07-24 12:17:49.594506 pydantic_numpy-3.0.0/pydantic_numpy/model.py
+-rw-r--r--   0        0        0        0 2023-07-24 08:00:18.249803 pydantic_numpy-3.0.0/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-24 08:19:57.319153 pydantic_numpy-3.0.0/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     2285 2023-07-24 08:19:57.259153 pydantic_numpy-3.0.0/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     2284 2023-07-24 08:19:57.293153 pydantic_numpy-3.0.0/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     2036 2023-07-24 08:19:57.247153 pydantic_numpy-3.0.0/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2023-07-23 11:42:56.554729 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/__init__.py
+-rw-r--r--   0        0        0     2860 2023-07-24 08:35:12.890564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/i_dimensional.py
+-rw-r--r--   0        0        0     2860 2023-07-24 08:35:12.883564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/ii_dimensional.py
+-rw-r--r--   0        0        0     2859 2023-07-24 08:36:13.362365 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/iii_dimensional.py
+-rw-r--r--   0        0        0     2578 2023-07-24 08:35:12.875564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/n_dimensional.py
+-rw-r--r--   0        0        0      571 2023-07-24 12:11:47.665552 pydantic_numpy-3.0.0/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1171 2023-07-24 12:41:09.789859 pydantic_numpy-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 pydantic_numpy-3.0.0/PKG-INFO
```

### Comparing `pydantic_numpy-2.2.2/LICENSE` & `pydantic_numpy-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-2.2.2/README.md` & `pydantic_numpy-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Install
 ```shell
 pip install pydantic-numpy
 ```
 
 ## Usage
 
-For more examples see [test_ndarray.py](./tests/test_ndarray.py)
+For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
 import pydantic_numpy.dtype as pnd
 from pydantic_numpy import NDArray, NDArrayFp32, NumpyModel
 
 
 class MyPydanticNumpyModel(NumpyModel):
@@ -38,17 +38,14 @@
 `NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model.
 
 ### Data type (dtype) support!
 
 This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
 
 ## Considerations
+You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only support Pydantic V1 and will not work with V2.
 
-The `NDArray` class from `pydantic-numpy` is daughter of `np.ndarray`. IDEs and linters might complain that you are passing an incorrect `type` to a model. The only solution is to merge these change into `numpy`.
-
-You can also use the `typings` in `pydantic.validate_arguments`.
-
-You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support.
+### Licensing notice
+As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
 ## History
-
-The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
+The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

### Comparing `pydantic_numpy-2.2.2/pydantic_numpy/model.py` & `pydantic_numpy-3.0.0/pydantic_numpy/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 import pickle as pickle_pkg
 from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    Iterable,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
+from typing import Any, Callable, ClassVar, Iterable, Optional, Type
 
 import compress_pickle
 import numpy as np
-from pydantic import BaseModel, DirectoryPath, FilePath, validate_arguments
+import numpy.typing as npt
+from pydantic import BaseModel, DirectoryPath, FilePath, validate_call
 from ruamel.yaml import YAML
 
+from pydantic_numpy.util import np_general_all_close
+
 yaml = YAML()
 
 
 class NumpyModel(BaseModel):
     _dump_compression: ClassVar[str] = "lz4"
     _dump_numpy_savez_file_name: ClassVar[str] = "arrays.npz"
     _dump_non_array_file_stem: ClassVar[str] = "object_info"
 
     _directory_suffix: ClassVar[str] = ".pdnp"
 
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, NumpyModel):
+            # When comparing instances of generic types for equality, as long as all field values are equal,
+            # only require their generic origin types to be equal, rather than exact type equality.
+            # This prevents headaches like MyGeneric(x=1) != MyGeneric[Any](x=1).
+            self_type = self.__pydantic_generic_metadata__["origin"] or self.__class__
+            other_type = other.__pydantic_generic_metadata__["origin"] or other.__class__
+
+            self_ndarray_field_to_array, self_other_field_to_value = self._dump_numpy_split_dict()
+            other_ndarray_field_to_array, other_other_field_to_value = other._dump_numpy_split_dict()
+
+            return (
+                self_type == other_type
+                and self_other_field_to_value == other_other_field_to_value
+                and self.__pydantic_private__ == other.__pydantic_private__
+                and self.__pydantic_extra__ == other.__pydantic_extra__
+                and _compare_np_array_dicts(self_ndarray_field_to_array, other_ndarray_field_to_array)
+            )
+        elif isinstance(other, BaseModel):
+            return super().__eq__(other)
+        else:
+            return NotImplemented  # delegate to the other item in the comparison
+
     @classmethod
-    @validate_arguments
+    @validate_call
     def model_directory_path(cls, output_directory: DirectoryPath, object_id: str) -> DirectoryPath:
         return output_directory / f"{object_id}.{cls.__name__}{cls._directory_suffix}"
 
+    @validate_call
     def dump(
         self, output_directory: Path, object_id: str, compress: bool = True, pickle: bool = False
     ) -> DirectoryPath:
-        assert not self.__config__.arbitrary_types_allowed or (
-            self.__config__.arbitrary_types_allowed and pickle
+        assert "arbitrary_types_allowed" not in self.model_config or (
+            self.model_config["arbitrary_types_allowed"] and pickle
         ), "Arbitrary types are only supported in pickle mode"
 
         dump_directory_path = self.model_directory_path(output_directory, object_id)
         dump_directory_path.mkdir(parents=True, exist_ok=True)
 
         ndarray_field_to_array, other_field_to_value = self._dump_numpy_split_dict()
 
@@ -65,20 +81,21 @@
             else:
                 with open(dump_directory_path / self._dump_non_array_yaml_name, "w") as out_yaml:
                     yaml.dump(other_field_to_value, out_yaml)
 
         return dump_directory_path
 
     @classmethod
+    @validate_call
     def load(
         cls,
         output_directory: DirectoryPath,
         object_id: str,
         pre_load_modifier: Optional[Callable[[dict[str, Any]], dict[str, Any]]] = None,
-    ) -> "NumpyModelVar":
+    ):
         object_directory_path = cls.model_directory_path(output_directory, object_id)
 
         npz_file = np.load(object_directory_path / cls._dump_numpy_savez_file_name)
 
         other_path: FilePath
         if (other_path := object_directory_path / cls._dump_compressed_pickle_file_name).exists():
             other_field_to_value = compress_pickle.load(other_path)
@@ -93,17 +110,19 @@
 
         field_to_value = {**npz_file, **other_field_to_value}
         if pre_load_modifier:
             field_to_value = pre_load_modifier(field_to_value)
 
         return cls(**field_to_value)
 
-    def _dump_numpy_split_dict(self) -> Tuple[Dict, Dict]:
-        ndarray_field_to_array, other_field_to_value = {}, {}
-        for k, v in self.dict(exclude_unset=True).items():
+    def _dump_numpy_split_dict(self) -> tuple[dict, dict]:
+        ndarray_field_to_array = {}
+        other_field_to_value = {}
+
+        for k, v in self.model_dump(exclude_unset=True).items():
             if isinstance(v, np.ndarray):
                 ndarray_field_to_array[k] = v
             else:
                 other_field_to_value[k] = v
 
         return ndarray_field_to_array, other_field_to_value
 
@@ -119,30 +138,61 @@
 
     @classmethod
     @property
     def _dump_non_array_yaml_name(cls) -> str:
         return f"{cls._dump_non_array_file_stem}.yaml"
 
 
-NumpyModelVar = TypeVar("NumpyModelVar", bound=NumpyModel)
-NumpyModel.update_forward_refs(NumpyModelVar=NumpyModelVar)
-
-
 NumpyModelCLS = Type[NumpyModel]
 
 
 def model_agnostic_load(
     output_directory: DirectoryPath,
     object_id: str,
     models: Iterable[NumpyModelCLS],
     not_found_error: bool = False,
     **load_kwargs,
-) -> Union[NumpyModelVar, None]:
+) -> Optional[NumpyModel]:
     for model in models:
         if model.model_directory_path(output_directory, object_id).exists():
             return model.load(output_directory, object_id, **load_kwargs)
+
     if not_found_error:
         raise FileNotFoundError(
             f"Could not find NumpyModel with {object_id} in {output_directory}."
             f"Tried from following classes:\n{', '.join(model.__name__ for model in models)}"
         )
+
     return None
+
+
+def _compare_np_array_dicts(
+    dict_a: dict[str, npt.NDArray], dict_b: dict[str, npt.NDArray], rtol: float = 1e-05, atol: float = 1e-08
+) -> bool:
+    """
+    Compare two dictionaries containing numpy arrays as values.
+
+    Parameters:
+    dict_a, dict_b: dictionaries to compare. They should have same keys.
+    rtol, atol: relative and absolute tolerances for np.isclose()
+
+    Returns:
+    Boolean value for each key, True if corresponding arrays are close, else False.
+    """
+
+    keys1 = frozenset(dict_a.keys())
+    keys2 = frozenset(dict_b.keys())
+
+    if keys1 != keys2:
+        raise ValueError("Dictionaries have different keys")
+
+    for key in keys1:
+        arr_a = dict_a[key]
+        arr_b = dict_b[key]
+
+        if arr_a.shape != arr_b.shape:
+            raise ValueError(f"Arrays for key '{key}' have different shapes")
+
+        if not np_general_all_close(arr_a, arr_b):
+            return False
+
+    return True
```

### Comparing `pydantic_numpy-2.2.2/pyproject.toml` & `pydantic_numpy-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "2.2.2"
-description = "Seamlessly integrate numpy arrays into pydantic models"
-authors = ["Can H. Tartanoglu <canhtart@gmail.com>", "Christoph Heindl"]
-license = "MIT"
-
+version = "3.0.0"
+description = "Pydantic Model integration of the NumPy array"
+authors = ["Can H. Tartanoglu", "Christoph Heindl"]
+maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
-repository = "https://github.com/caniko/pydantic-numpy"
+homepage = "https://github.com/caniko/pydantic-numpy"
+license = "BSD-4"
 
 keywords = ["pydantic", "numpy", "typing"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent"
 ]
@@ -19,28 +19,31 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 compress-pickle = { version = "*", extras = ["lz4"] }
 ruamel-yaml = "^0.17.21"
 
 numpy = "*"
-pydantic = "^1.10.0"
+pydantic = "^2.0"
+coverage = "^7.2.7"
 
-[tool.poetry.dev-dependencies]
-pytest = "*"
-black = "*"
-isort = "*"
-pre-commit = "*"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+parameterized = "^0.9.0"
+hypothesis = "^6.82.0"
+setuptools = "^68.0.0"
+pytest-xdist = "^3.3.1"
 
 [tool.black]
 line-length = 120
 target-version = ["py311"]
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 120
+ignore-init-module-imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_numpy-2.2.2/PKG-INFO` & `pydantic_numpy-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 2.2.2
-Summary: Seamlessly integrate numpy arrays into pydantic models
+Version: 3.0.0
+Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
-License: MIT
+License: BSD-4
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
-Author-email: canhtart@gmail.com
+Maintainer: Can H. Tartanoglu
+Maintainer-email: python@rotas.mozmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: compress-pickle[lz4]
+Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: numpy
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
-Project-URL: Repository, https://github.com/caniko/pydantic-numpy
 Description-Content-Type: text/markdown
 
 # pydantic-numpy
 
 Integrate NumPy into Pydantic, and provide tooling! `NumpyModel` make it possible to dump and load `np.ndarray` within model fields!
 
 ### Install
 ```shell
 pip install pydantic-numpy
 ```
 
 ## Usage
 
-For more examples see [test_ndarray.py](./tests/test_ndarray.py)
+For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
 import pydantic_numpy.dtype as pnd
 from pydantic_numpy import NDArray, NDArrayFp32, NumpyModel
 
 
 class MyPydanticNumpyModel(NumpyModel):
@@ -63,18 +64,14 @@
 `NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model.
 
 ### Data type (dtype) support!
 
 This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
 
 ## Considerations
+You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only support Pydantic V1 and will not work with V2.
 
-The `NDArray` class from `pydantic-numpy` is daughter of `np.ndarray`. IDEs and linters might complain that you are passing an incorrect `type` to a model. The only solution is to merge these change into `numpy`.
-
-You can also use the `typings` in `pydantic.validate_arguments`.
-
-You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support.
+### Licensing notice
+As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
 ## History
-
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
-
```

