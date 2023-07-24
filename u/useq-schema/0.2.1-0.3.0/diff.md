# Comparing `tmp/useq_schema-0.2.1.tar.gz` & `tmp/useq_schema-0.3.0.tar.gz`

## Comparing `useq_schema-0.2.1.tar` & `useq_schema-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 useq_schema-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.2.1/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/images/favicon.ico
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/axes.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/event.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/__init__.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_base_model.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_channel.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_grid.py
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_mda_event.py
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_position.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_time.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_utils.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/py.typed
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_grid.py
--rw-r--r--   0        0        0    23284 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_position_sequence.py
--rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_serialization.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/fixtures/mda.json
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.2.1/LICENSE
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.2.1/README.md
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 useq_schema-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.0/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_actions.py
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_base_model.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_channel.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_grid.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_position.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_time.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_utils.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/py.typed
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_grid.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_misc.py
+-rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_position_sequence.py
+-rw-r--r--   0        0        0    10261 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_serialization.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.3.0/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 useq_schema-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.3.0/PKG-INFO
```

### Comparing `useq_schema-0.2.1/.pre-commit-config.yaml` & `useq_schema-0.3.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,45 +3,45 @@
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.1.1
+    rev: v2.3.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: pretty-format-json
         args: ["--autofix"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.275
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-PyYAML
-          - pydantic
+          - pydantic<2.0.0
         files: "^src/"
```

### Comparing `useq_schema-0.2.1/mkdocs.yml` & `useq_schema-0.3.0/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   - pymmcore-plus: /pymmcore-plus/
   - useq-schema:
       - index.md
       - Schema:
         - schema/sequence.md
         - schema/event.md
         - schema/axes.md
+        - schema/hardware_autofocus.md
       - api.md
   - pymmcore-widgets: /pymmcore-widgets/
 
 theme:
   name: "material"
   features:
     - content.tabs.link
```

### Comparing `useq_schema-0.2.1/setup.py` & `useq_schema-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/.github/workflows/test_and_deploy.yml` & `useq_schema-0.3.0/.github/workflows/test_and_deploy.yml`

 * *Files 15% similar despite different names*

```diff
@@ -67,20 +67,48 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e pymmcore-plus-from-github[testing]
           pip install -e .[test]
 
       - name: Install Micro-Manager
-        run: python -m pymmcore_plus.install
+        run: mmcore install
 
       - name: Test
         run: pytest -v --color=yes
         working-directory: pymmcore-plus-from-github
 
+  test_pymmcore_widgets:
+    name: Test pymmcore-widgets
+    runs-on: macos-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/checkout@v3
+        with:
+          repository: pymmcore-plus/pymmcore-widgets
+          path: pymmcore-widgets-from-github
+
+      - name: Set up Python 3.10
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -e pymmcore-widgets-from-github[test,image,pyqt6]
+          pip install -e .[test]
+
+      - name: Install Micro-Manager
+        run: mmcore install
+
+      - name: Test
+        run: pytest -v --color=yes -W ignore
+        working-directory: pymmcore-widgets-from-github
+
 
   deploy:
     needs: test
     runs-on: ubuntu-latest
     if: ${{ github.repository == 'pymmcore-plus/useq-schema' && contains(github.ref, 'tags') }}
     steps:
       - uses: actions/checkout@v3
```

### Comparing `useq_schema-0.2.1/docs/api.md` & `useq_schema-0.3.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/docs/index.md` & `useq_schema-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/docs/images/favicon.ico` & `useq_schema-0.3.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/docs/schema/axes.md` & `useq_schema-0.3.0/docs/schema/axes.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,14 @@
         members: []
 ::: useq.TIntervalDuration
     options:
         members: []
 ::: useq.MultiPhaseTimePlan
     options:
         members: []
-::: useq.NoT
-    options:
-        members: []
 
 ## Z Plans
 
 Ways to describe a z-stack acquisition sequence.
 
 ::: useq.ZTopBottom
     options:
@@ -51,26 +48,19 @@
         members: []
 ::: useq.ZRangeAround
     options:
         members: []
 ::: useq.ZRelativePositions
     options:
         members: []
-::: useq.NoZ
-    options:
-        members: []
 
 ## Grid Plans
 
 Ways to describe a grid acquisition sequence.
 
 ::: useq.GridRelative
     options:
         members: []
 
 ::: useq.GridFromEdges
     options:
         members: []
-
-::: useq.NoGrid
-    options:
-        members: []
```

### Comparing `useq_schema-0.2.1/docs/stylesheets/extra.css` & `useq_schema-0.3.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/src/useq/_base_model.py` & `useq_schema-0.3.0/src/useq/_base_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,25 @@
     Type,
     TypeVar,
     Union,
 )
 
 from pydantic import BaseModel, root_validator
 from pydantic.error_wrappers import ErrorWrapper, ValidationError
-from pydantic.types import StrBytes
 from pydantic.utils import ROOT_KEY
 
 if TYPE_CHECKING:
+    from pydantic.types import StrBytes
+
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
 
 
 __all__ = ["UseqModel", "FrozenModel"]
 
+_T = TypeVar("_T", bound="FrozenModel")
 _Y = TypeVar("_Y", bound="UseqModel")
 
 
 class FrozenModel(BaseModel):
     class Config:
         allow_population_by_field_name = True
         extra = "allow"
@@ -44,14 +46,28 @@
             warnings.warn(
                 f"{name} got unknown keyword arguments: {extra_kwargs}", stacklevel=2
             )
             for k in extra_kwargs:
                 values.pop(k)
         return values
 
+    def replace(self: _T, **kwargs: Any) -> _T:
+        """Return a new instance replacing specified kwargs with new values.
+
+        This model is immutable, so this method is useful for creating a new
+        sequence with only a few fields changed.  The uid of the new sequence will
+        be different from the original.
+
+        The difference between this and `self.copy(update={...})` is that this method
+        will perform validation and casting on the new values, whereas `copy` assumes
+        that all objects are valid and will not perform any validation or casting.
+        """
+        state = self.dict(exclude={"uid"})
+        return type(self)(**{**state, **kwargs})
+
 
 class UseqModel(FrozenModel):
     def __repr_args__(self) -> ReprArgs:
         return [
             (k, val)
             for k, val in super().__repr_args__()
             if k in self.__fields__
```

### Comparing `useq_schema-0.2.1/src/useq/_channel.py` & `useq_schema-0.3.0/src/useq/_channel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Generator, Optional
 
-from pydantic.types import PositiveFloat, PositiveInt
+from pydantic import Field
 
-from ._base_model import FrozenModel
+from useq import _mda_event
+from useq._base_model import FrozenModel
 
 
 class Channel(FrozenModel):
     """Define an acquisition channel.
 
     Attributes
     ----------
     config : str
         Name of the configuration to use for this channel, (e.g. `"488nm"`, `"DAPI"`,
         `"FITC"`).
     group : str
         Optional name of the group to which this channel belongs. By default,
         `"Channel"`.
-    exposure : PositiveFloat | None
-        Exposure time in seconds. If not provided, implies use current exposure time.
-        By default, `None`.
+    exposure : float | None
+        Exposure time in seconds. Must be positive.  If not provided, implies use
+        current exposure time. By default, `None`.
     do_stack : bool
         If `True`, instructs engine to include this channel in any Z stacks being
         acquired. By default, `True`.
     z_offset : float
         Relative Z offset from current position, in microns. By default, `0`.
-    acquire_every : PositiveInt
+    acquire_every : int
         Acquire every Nth frame (if acquiring a time series). By default, `1`.
     camera: str | None
         Name of the camera to use for this channel. If not provided, implies use
         current camera. By default, `None`.
     """
 
     config: str
     group: str = "Channel"
-    exposure: Optional[PositiveFloat] = None
+    exposure: Optional[float] = Field(None, gt=0.0)
     do_stack: bool = True
     z_offset: float = 0.0
-    acquire_every: PositiveInt = 1  # acquire every n frames
+    acquire_every: int = Field(default=1, gt=0)  # acquire every n frames
     camera: Optional[str] = None
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable, None, None]:
         yield cls.validate
 
     @classmethod
@@ -50,7 +51,10 @@
         if isinstance(value, Channel):
             return value
         if isinstance(value, str):
             return Channel(config=value)
         if isinstance(value, dict):
             return Channel(**value)
         raise TypeError(f"invalid Channel argument: {value!r}")
+
+    def to_event_channel(self) -> _mda_event.Channel:
+        return _mda_event.Channel(config=self.config, group=self.group)
```

### Comparing `useq_schema-0.2.1/src/useq/_grid.py` & `useq_schema-0.3.0/src/useq/_grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,17 +240,8 @@
 
     def _offset_y(self, dy: float) -> float:
         return (
             ((self.rows - 1) * dy) / 2 if self.relative_to == RelativeTo.center else 0.0
         )
 
 
-class NoGrid(_GridPlan):
-    """Don't acquire a grid."""
-
-    def iter_grid_positions(
-        self, fov_width: float, fov_height: float
-    ) -> Iterator[GridPosition]:
-        return iter([])
-
-
-AnyGridPlan = Union[GridFromEdges, GridRelative, NoGrid]
+AnyGridPlan = Union[GridFromEdges, GridRelative]
```

### Comparing `useq_schema-0.2.1/src/useq/_mda_event.py` & `useq_schema-0.3.0/src/useq/_mda_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
+import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     NamedTuple,
     NoReturn,
     Optional,
     Sequence,
     Tuple,
 )
 
 from pydantic import Field, validator
-from pydantic.types import PositiveFloat
 
-from ._base_model import UseqModel
-from ._utils import ReadOnlyDict
+from useq._actions import AcquireImage, Action
+from useq._base_model import UseqModel
+from useq._utils import ReadOnlyDict
 
 if TYPE_CHECKING:
-    from ._mda_sequence import MDASequence
+    from useq._mda_sequence import MDASequence
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
 
 
 class Channel(UseqModel):
     """Channel in a MDA event.
 
@@ -36,14 +37,19 @@
         Optional name of the group to which this channel belongs. By default,
         `"Channel"`.
     """
 
     config: str
     group: str = "Channel"
 
+    def __eq__(self, _value: object) -> bool:
+        if isinstance(_value, str):
+            return self.config == _value
+        return super().__eq__(_value)
+
 
 class PropertyTuple(NamedTuple):
     """Three-tuple capturing a device, property, and value.
 
     Attributes
     ----------
     device_name : str
@@ -76,15 +82,15 @@
         to index.  For example: `{'t': 4, 'c': 0, 'z': 5},`
     channel : Channel | None
         Channel to use for this event. If `None`, implies use current channel.
         By default, `None`.  `Channel` is a simple pydantic object with two attributes:
         `config` and `group`.  `config` is the name of the configuration to use for this
         channel, (e.g. `"488nm"`, `"DAPI"`, `"FITC"`).  `group` is the name of the group
         to which this channel belongs. By default, `"Channel"`.
-    exposure : PositiveFloat | None
+    exposure : float | None
         Exposure time in seconds. If not provided, implies use current exposure time.
         By default, `None`.
     min_start_time : float | None
         Minimum start time of this event, in seconds.  If provided, the engine will
         pause until this time has elapsed (relative to the start of the sequence)
         before starting this event. By default, `None`.
     pos_name : str | None
@@ -94,46 +100,61 @@
         default, `None`.
     y_pos : float | None
         Y position in microns. If not provided, implies use current position. By
         default, `None`.
     z_pos : float | None
         Z position in microns. If not provided, implies use current position. By
         default, `None`.
+    sequence : MDASequence | None
+        A reference to the [`useq.MDASequence`][] this event belongs to. This is a
+        read-only attribute. By default, `None`.
     properties : Sequence[PropertyTuple] | None
         List of [`useq.PropertyTuple`][] to set before starting this event. Where each
         item in the list is a 3-member named tuple of `(device_name, property_name,
         property_value)`.  This is inspired by micro-manager's Device Adapter API, but
         could be used to set arbitrary properties in any backend that supports the
         concept of devices that have properties with values. By default, `None`.
-    sequence : MDASequence | None
-        A reference to the [`useq.MDASequence`][] this event belongs to. This is a
-        read-only attribute. By default, `None`.
-    global_index : int
-        The global index of this event in the sequence. For example, in an
-        `MDASequence` with 2 channels and 5 time points, the global index of each
-        event will be an integer from 0 to 9.  By default, `0`.
     metadata : dict
         Optional metadata to be associated with this event.
+    action : Action
+        The action to perform for this event.  By default, [`useq.AcquireImage`][].
+        Example of another action is [`useq.HardwareAutofocus`][] which could be used
+        to perform a hardware autofocus.
+    keep_shutter_open : bool
+        If True, the illumination shutter should be left open after the event has
+        been executed, otherwise it should be closed. By default, `False`."
+        This is useful when the sequence of events being executed use the same
+        illumination scheme (such as a z-stack in a single channel), and closing and
+        opening the shutter between events would be slow.
     """
 
     index: ReadOnlyDict[str, int] = Field(default_factory=ReadOnlyDict)
     channel: Optional[Channel] = None
-    exposure: Optional[PositiveFloat] = None
+    exposure: Optional[float] = Field(default=None, gt=0.0)
     min_start_time: Optional[float] = None  # time in sec
     pos_name: Optional[str] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     z_pos: Optional[float] = None
-    properties: Optional[List[PropertyTuple]] = None
     sequence: Optional[MDASequence] = Field(default=None, repr=False)
-    global_index: int = Field(default=0, repr=False)
+    properties: Optional[List[PropertyTuple]] = None
     metadata: Dict[str, Any] = Field(default_factory=dict)
+    action: Action = Field(default_factory=AcquireImage)
+    keep_shutter_open: bool = False
 
     # action
     # keep shutter open between channels/steps
+    @property
+    def global_index(self) -> int:
+        warnings.warn(
+            "global_index is no longer functional.  Use `enumerate()` "
+            "on an iterable of events instead.",
+            stacklevel=2,
+        )
+        return 0
 
     @validator("index", pre=True)
     def validate_index(cls, v: dict) -> ReadOnlyDict[str, int]:
         return ReadOnlyDict(v)
 
     def __repr_args__(self) -> ReprArgs:
         d = self.__dict__.copy()
```

### Comparing `useq_schema-0.2.1/src/useq/_mda_sequence.py` & `useq_schema-0.3.0/src/useq/_mda_sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 from __future__ import annotations
 
 from itertools import product
-from typing import (
-    Any,
-    Dict,
-    Iterator,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-    cast,
-    no_type_check,
-)
+from typing import Any, Dict, Iterator, Optional, Sequence, Tuple, cast
 from uuid import UUID, uuid4
 from warnings import warn
 
 import numpy as np
 from pydantic import Field, PrivateAttr, root_validator, validator
+from typing_extensions import TypedDict
 
-from . import _mda_event
-from ._base_model import UseqModel
-from ._channel import Channel
-from ._grid import AnyGridPlan, GridPosition, NoGrid
-from ._mda_event import MDAEvent
-from ._position import Position
-from ._time import AnyTimePlan, NoT
-from ._z import AnyZPlan, NoZ
+from useq._base_model import UseqModel
+from useq._channel import Channel  # noqa: TCH001
+from useq._grid import AnyGridPlan, GridPosition  # noqa: TCH001
+from useq._hardware_autofocus import AnyAutofocusPlan, AxesBasedAF
+from useq._mda_event import Channel as EventChannel
+from useq._mda_event import MDAEvent
+from useq._position import Position
+from useq._time import AnyTimePlan  # noqa: TCH001
+from useq._z import AnyZPlan  # noqa: TCH001
 
 TIME = "t"
 CHANNEL = "c"
 POSITION = "p"
 Z = "z"
 GRID = "g"
 INDICES = (TIME, POSITION, GRID, CHANNEL, Z)
@@ -52,29 +44,31 @@
         A dictionary of user metadata to be stored with the sequence.
     axis_order : str
         The order of the axes in the sequence. Must be a permutation of `"tpgcz"`. The
         default is `"tpgcz"`.
     stage_positions : tuple[Position, ...]
         The stage positions to visit. (each with `x`, `y`, `z`, `name`, and `sequence`,
         all of which are optional).
-    grid_plan : GridFromEdges, GridRelative, NoGrid
-        The grid plan to follow. One of `GridFromEdges`, `GridRelative` or `NoGrid`.
+    grid_plan : GridFromEdges | GridRelative | None
+        The grid plan to follow. One of `GridFromEdges`, `GridRelative` or `None`.
     channels : tuple[Channel, ...]
         The channels to acquire. see `Channel`.
     time_plan : MultiPhaseTimePlan | TIntervalDuration | TIntervalLoops \
-        | TDurationLoops | NoT
+        | TDurationLoops | None
         The time plan to follow. One of `TIntervalDuration`, `TIntervalLoops`,
-        `TDurationLoops`, `MultiPhaseTimePlan`, or `NoT`
+        `TDurationLoops`, `MultiPhaseTimePlan`, or `None`
     z_plan : ZTopBottom | ZRangeAround | ZAboveBelow | ZRelativePositions | \
-        ZAbsolutePositions | NoZ
+        ZAbsolutePositions | None
         The z plan to follow. One of `ZTopBottom`, `ZRangeAround`, `ZAboveBelow`,
-        `ZRelativePositions`, `ZAbsolutePositions`, or `NoZ`.
+        `ZRelativePositions`, `ZAbsolutePositions`, or `None`.
     uid : UUID
         A read-only unique identifier (uuid version 4) for the sequence. This will be
         generated, do not set.
+    autofocus_plan : AxesBasedAF | None
+        The hardware autofocus plan to follow. One of `AxesBasedAF` or `None`.
 
     Examples
     --------
     >>> from useq import MDASequence, Position, Channel, TIntervalDuration
     >>> seq = MDASequence(
     ...     time_plan={"interval": 0.1, "loops": 2},
     ...     stage_positions=[(1, 1, 1)],
@@ -106,18 +100,19 @@
       range: 3.0
       step: 1.0
     """
 
     metadata: Dict[str, Any] = Field(default_factory=dict)
     axis_order: str = "".join(INDICES)
     stage_positions: Tuple[Position, ...] = Field(default_factory=tuple)
-    grid_plan: AnyGridPlan = Field(default_factory=NoGrid)
+    grid_plan: Optional[AnyGridPlan] = None
     channels: Tuple[Channel, ...] = Field(default_factory=tuple)
-    time_plan: AnyTimePlan = Field(default_factory=NoT)
-    z_plan: AnyZPlan = Field(default_factory=NoZ)
+    time_plan: Optional[AnyTimePlan] = None
+    z_plan: Optional[AnyZPlan] = None
+    autofocus_plan: Optional[AnyAutofocusPlan] = None
 
     _uid: UUID = PrivateAttr(default_factory=uuid4)
     _length: Optional[int] = PrivateAttr(default=None)
     _fov_size: Tuple[float, float] = PrivateAttr(default=(1, 1))
 
     @property
     def uid(self) -> UUID:
@@ -127,47 +122,24 @@
     def set_fov_size(self, fov_size: Tuple[float, float]) -> None:
         """Set the field of view size.
 
         This is used to calculate the number of positions in a grid plan.
         """
         self._fov_size = fov_size
 
-    @no_type_check
-    def replace(
-        self,
-        metadata: Dict[str, Any] = Undefined,
-        axis_order: str = Undefined,
-        stage_positions: Tuple[Position, ...] = Undefined,
-        grid_plan: AnyGridPlan = Undefined,
-        channels: Tuple[Channel, ...] = Undefined,
-        time_plan: AnyTimePlan = Undefined,
-        z_plan: AnyZPlan = Undefined,
-    ) -> MDASequence:
-        """Return a new `MDAsequence` replacing specified kwargs with new values.
-
-        MDASequences are immutable, so this method is useful for creating a new
-        sequence with only a few fields changed.  The uid of the new sequence will
-        be different from the original.
-        """
-        kwargs = {
-            k: v for k, v in locals().items() if v is not Undefined and k != "self"
-        }
-        state = self.dict(exclude={"uid"})
-        return type(self)(**{**state, **kwargs})
-
     def __hash__(self) -> int:
         return hash(self.uid)
 
     @validator("z_plan", pre=True)
-    def validate_zplan(cls, v: Any) -> Union[dict, NoZ]:
-        return v or NoZ()
+    def validate_zplan(cls, v: Any) -> Optional[dict]:
+        return v or None
 
     @validator("time_plan", pre=True)
-    def validate_time_plan(cls, v: Any) -> Union[dict, NoT]:
-        return {"phases": v} if isinstance(v, (tuple, list)) else v or NoT()
+    def validate_time_plan(cls, v: Any) -> Optional[dict]:
+        return {"phases": v} if isinstance(v, (tuple, list)) else v or None
 
     @validator("stage_positions", pre=True)
     def validate_positions(cls, v: Any) -> Any:
         if isinstance(v, np.ndarray):
             if v.ndim == 1:
                 return [v]
             elif v.ndim == 2:
@@ -194,14 +166,15 @@
         if "axis_order" in values:
             values["axis_order"] = cls._check_order(
                 values["axis_order"],
                 z_plan=values.get("z_plan"),
                 stage_positions=values.get("stage_positions", ()),
                 channels=values.get("channels", ()),
                 grid_plan=values.get("grid_plan"),
+                autofocus_plan=values.get("autofocus_plan"),
             )
         return values
 
     def __eq__(self, other: Any) -> bool:
         """Return `True` if two `MDASequences` are equal (uid is excluded)."""
         if isinstance(other, MDASequence):
             return bool(self.dict(exclude={"uid"}) == other.dict(exclude={"uid"}))
@@ -211,14 +184,15 @@
     @staticmethod
     def _check_order(
         order: str,
         z_plan: Optional[AnyZPlan] = None,
         stage_positions: Sequence[Position] = (),
         channels: Sequence[Channel] = (),
         grid_plan: Optional[AnyGridPlan] = None,
+        autofocus_plan: Optional[AnyAutofocusPlan] = None,
     ) -> str:
         if (
             Z in order
             and POSITION in order
             and order.index(Z) < order.index(POSITION)
             and z_plan
             and any(p.sequence.z_plan for p in stage_positions if p.sequence)
@@ -239,16 +213,15 @@
                 "{TIME!r} in the acquisition order: may not yield intended results.",
                 stacklevel=2,
             )
 
         if (
             GRID in order
             and POSITION in order
-            and grid_plan is not None
-            and not isinstance(grid_plan, NoGrid)
+            and grid_plan
             and not grid_plan.is_relative
             and len(stage_positions) > 1
         ):
             sub_position_grid_plans = [
                 p for p in stage_positions if p.sequence and p.sequence.grid_plan
             ]
             if len(stage_positions) - len(sub_position_grid_plans) > 1:
@@ -262,14 +235,23 @@
             and stage_positions
             and any(p.sequence.stage_positions for p in stage_positions if p.sequence)
         ):
             raise ValueError(
                 "Currently, a Position sequence cannot have multiple stage positions!"
             )
 
+        # Cannot use autofocus plan with absolute z_plan
+        if Z in order and z_plan and not z_plan.is_relative:
+            err = "Absolute Z positions cannot be used with autofocus plan."
+            if isinstance(autofocus_plan, AxesBasedAF):
+                raise ValueError(err)
+            for p in stage_positions:
+                if p.sequence is not None and p.sequence.autofocus_plan:
+                    raise ValueError(err)
+
         return order
 
     def __str__(self) -> str:
         shape = [
             f"n{k.lower()}: {len(list(self.iter_axis(k)))}" for k in self.axis_order
         ]
         return "Multi-Dimensional Acquisition ▶ " + ", ".join(shape)
@@ -299,23 +281,27 @@
         """Single letter string of axes used in this sequence, e.g. `ztc`."""
         return "".join(k for k in self.axis_order if self.sizes[k])
 
     def iter_axis(
         self, axis: str
     ) -> Iterator[Position | Channel | float | GridPosition]:
         """Iterate over the events of a given axis."""
-        yield from {
+        plan = {
             TIME: self.time_plan,
             POSITION: self.stage_positions,
             Z: self.z_plan,
             CHANNEL: self.channels,
-            GRID: self.grid_plan.iter_grid_positions(
-                self._fov_size[0], self._fov_size[1]
+            GRID: (
+                self.grid_plan.iter_grid_positions(self._fov_size[0], self._fov_size[1])
+                if self.grid_plan
+                else ()
             ),
         }[axis]
+        if plan:
+            yield from plan
 
     def __iter__(self) -> Iterator[MDAEvent]:  # type: ignore [override]
         """Same as `iter_events`. Supports `for event in sequence: ...` syntax."""
         yield from self.iter_events()
 
     class _SkipFrame(Exception):
         pass
@@ -329,229 +315,286 @@
         Yields
         ------
         MDAEvent
             Each event in the MDA sequence.
         """
         return iter_sequence(self)
 
-    def _combine_z(
-        self,
-        z_pos: float,
-        z_ind: int,
-        channel: Optional[Channel],
-        position: Optional[Position],
-    ) -> float:
-        if channel:
-            # only acquire on the middle plane:
-            if not channel.do_stack and z_ind != len(self.z_plan) // 2:
-                raise self._SkipFrame()
-            if channel.z_offset is not None:
-                z_pos += channel.z_offset
-        if self.z_plan.is_relative:
-            # TODO: either disallow without position z, or add concept of "current"
-            z_pos += getattr(position, Z, None) or 0
-        return z_pos
-
     def to_pycromanager(self) -> list[dict]:
         """Convenience to convert this sequence to a list of pycro-manager events.
 
         See: <https://pycro-manager.readthedocs.io/en/latest/apis.html>
         """
         return [event.to_pycromanager() for event in self]
 
 
 MDAEvent.update_forward_refs(MDASequence=MDASequence)
 Position.update_forward_refs(MDASequence=MDASequence)
 
 
-def iter_sequence(sequence: MDASequence) -> Iterator[MDAEvent]:
+class MDAEventDict(TypedDict, total=False):
+    index: dict[str, int]
+    channel: EventChannel | None
+    exposure: float | None
+    min_start_time: float | None
+    pos_name: str | None
+    x_pos: float | None
+    y_pos: float | None
+    z_pos: float | None
+    sequence: MDASequence | None
+    properties: list[tuple] | None
+    metadata: dict
+
+
+class PositionDict(TypedDict, total=False):
+    x_pos: float
+    y_pos: float
+    z_pos: float
+
+
+def iter_sequence(
+    sequence: MDASequence,
+    *,
+    base_event_kwargs: MDAEventDict | None = None,
+    event_kwarg_overrides: MDAEventDict | None = None,
+    position_offsets: PositionDict | None = None,
+) -> Iterator[MDAEvent]:
     """Iterate over all events in the MDA sequence.'.
 
     !!! note
         This method will usually be used via [`useq.MDASequence.iter_events`][], or by
         simply iterating over the sequence.
 
     This does the job of iterating over all the frames in the MDA sequence,
     handling the logic of merging all z plans in channels and stage positions
     defined in the plans for each axis.
 
     The is the most "logic heavy" part of `useq-schema` (the rest of which is
     almost entirely declarative).  This iterator is useful for consuming `MDASequence`
     objects in a python runtime, but it isn't considered a "core" part of the schema.
 
+    Parameters
+    ----------
+    sequence : MDASequence
+        The sequence to iterate over.
+    base_event_kwargs : MDAEventDict | None
+        A dictionary of "global" kwargs to begin with when building the kwargs passed
+        to each MDAEvent.  These will be overriden by event-specific kwargs (e.g. if
+        the event specifies a channel, it will be used instead of the
+        `base_event_kwargs`.)
+    event_kwarg_overrides : MDAEventDict | None
+        A dictionary of kwargs that will be applied to all events. Unlike
+        `base_event_kwargs`, these kwargs take precedence over any event-specific
+        kwargs.
+    position_offsets : PositionDict | None
+        A dictionary of offsets to apply to each position. This can be used to shift
+        all positions in a sub-sequence.  Keys must be one of `x_pos`, `y_pos`, or
+        `z_pos` and values should be floats.s
+
     Yields
     ------
     MDAEvent
         Each event in the MDA sequence.
     """
-    global_index = 0
     order = sequence.used_axes
-
-    event_iterator = (enumerate(sequence.iter_axis(ax)) for ax in order)
-    for item in product(*event_iterator):
+    axis_iterators = (enumerate(sequence.iter_axis(ax)) for ax in order)
+    for item in product(*axis_iterators):
         if not item:  # the case with no events
             continue  # pragma: no cover
 
-        _ev = dict(zip(order, item))
-        index = {k: _ev[k][0] for k in INDICES if k in _ev}
-
-        position = cast(
-            "Position | None", _ev[POSITION][1] if POSITION in _ev else None
-        )
-        channel = cast("Channel | None", _ev[CHANNEL][1] if CHANNEL in _ev else None)
-        time = cast("int | None", _ev[TIME][1] if TIME in _ev else None)
-        grid = cast("GridPosition | None", _ev[GRID][1] if GRID in _ev else None)
+        # get axes objects for this event
+        index, time, position, grid, channel, z_pos = _parse_axes(zip(order, item))
 
-        # skip channels
-        if channel and TIME in index and index[TIME] % channel.acquire_every:
+        # skip if necessary
+        if _should_skip(position, channel, index, sequence.z_plan):
             continue
-        # skip if also in position.sequence
-        if position and position.sequence:
-            if (
-                # if a position specifies channels, then the *global* channel index
-                # is no longer relevant... so we skip all but the first "global" channel
-                CHANNEL in index
-                and index[CHANNEL] != 0
-                # UNLESS the position specifies any other plan.
-                # NOTE: if we ever add more plans, they will need to be explicitly added
-                # https://github.com/pymmcore-plus/useq-schema/pull/85
-                and not any(
-                    (
-                        position.sequence.grid_plan,
-                        position.sequence.z_plan,
-                        position.sequence.time_plan,
-                    )
-                )
-            ):
-                continue
-            if Z in index and index[Z] != 0 and position.sequence.z_plan:
-                continue
-            if GRID in index and index[GRID] != 0 and position.sequence.grid_plan:
-                continue
 
-        _channel = (
-            _mda_event.Channel(config=channel.config, group=channel.group)
-            if channel
-            else None
-        )
-
-        _exposure = getattr(channel, "exposure", None)
-
-        pos_name = getattr(position, "name", None)
-
-        try:
-            z_pos = (
-                sequence._combine_z(_ev[Z][1], index[Z], channel, position)
-                if Z in _ev
-                else position.z
-                if position
-                else None
-            )
-        except sequence._SkipFrame:
-            continue
+        # build kwargs that will be passed to this MDAEvent
+        event_kwargs = base_event_kwargs or MDAEventDict(sequence=sequence)
+        # the .update() here lets us build on top of the base_event.index if present
+        event_kwargs.setdefault("index", {}).update(index)
+        # determine x, y, z positions
+        event_kwargs.update(_xyzpos(position, channel, sequence.z_plan, grid, z_pos))
 
-        if grid:
-            x_pos: Optional[float] = grid.x
-            y_pos: Optional[float] = grid.y
-            if grid.is_relative:
-                px = getattr(position, "x", 0) or 0
-                py = getattr(position, "y", 0) or 0
-                x_pos = x_pos + px if x_pos is not None else None
-                y_pos = y_pos + py if y_pos is not None else None
-        else:
-            x_pos = getattr(position, "x", None)
-            y_pos = getattr(position, "y", None)
-
-        if position and position.sequence:
-            for sub_event in iter_sequence(position.sequence):
-                # we're going to create a modified sub-event, inheriting some of the
-                # values from the parent event, and shifting the position of the
-                # event to account for global position offsets (or override if the
-                # sub-event has an absolute XYZ position plan.)
-                update_kwargs = dict(
-                    global_index=global_index,
-                    index={**index, **sub_event.index},
-                    sequence=sequence,
-                    pos_name=position.name or pos_name,
-                    **_maybe_shifted_positions(
-                        sub_event=sub_event,
-                        position=position,
-                        z_pos=z_pos,
-                        x_pos=x_pos,
-                        y_pos=y_pos,
-                    ),
+        if position and position.name:
+            event_kwargs["pos_name"] = position.name
+        if channel:
+            event_kwargs["channel"] = channel.to_event_channel()
+            if channel.exposure is not None:
+                event_kwargs["exposure"] = channel.exposure
+        if time is not None:
+            event_kwargs["min_start_time"] = time
+
+        # apply any overrides
+        if event_kwarg_overrides:
+            event_kwargs.update(event_kwarg_overrides)
+
+        # shift positions if position_offsets have been provided
+        # (usually from sub-sequences)
+        if position_offsets:
+            for k, v in position_offsets.items():
+                if event_kwargs[k] is not None:  # type: ignore[literal-required]
+                    event_kwargs[k] += v  # type: ignore[literal-required]
+
+        # grab global autofocus plan (may be overridden by position-specific plan below)
+        autofocus_plan = sequence.autofocus_plan
+
+        # if a position has been declared with a sub-sequence, we recurse into it
+        if position:
+            if position.sequence:
+                # determine any relative position shifts or global overrides
+                _pos, _offsets = _position_offsets(position, event_kwargs)
+                # build overrides for this position
+                pos_overrides = MDAEventDict(sequence=sequence, **_pos)  # type: ignore
+                if position.name:
+                    pos_overrides["pos_name"] = position.name
+
+                sub_seq = position.sequence
+                # if the sub-sequence doe not have an autofocus plan, we override it
+                # with the parent sequence's autofocus plan
+                if not sub_seq.autofocus_plan:
+                    sub_seq = sub_seq.copy(update={"autofocus_plan": autofocus_plan})
+
+                # recurse into the sub-sequence
+                yield from iter_sequence(
+                    sub_seq,
+                    base_event_kwargs=event_kwargs.copy(),
+                    event_kwarg_overrides=pos_overrides,
+                    position_offsets=_offsets,
                 )
-
-                # time, exposure, and channel are inherited from the parent event
-                # if they are not present on the sub-event.
-                for val, name in [
-                    (time, "min_start_time"),
-                    (_exposure, "exposure"),
-                    (_channel, "channel"),
-                ]:
-                    subval = getattr(sub_event, name)
-                    update_kwargs[name] = subval if subval is not None else val
-
-                yield sub_event.copy(update=update_kwargs)
-                global_index += 1
-
-            continue
-
-        yield MDAEvent(
-            index=index,
-            min_start_time=time,
-            pos_name=pos_name,
-            x_pos=x_pos,
-            y_pos=y_pos,
-            z_pos=z_pos,
-            exposure=_exposure,
-            channel=_channel,
-            sequence=sequence,
-            global_index=global_index,
-        )
-        global_index += 1
-
-
-def _maybe_shifted_positions(
-    sub_event: MDAEvent,  # the event we just created in the position sequence
-    position: Position,  # the position we are iterating
-    z_pos: float | None,  # global z position
-    x_pos: float | None,  # global x position
-    y_pos: float | None,  # global y position
-) -> dict:
-    kwargs = {}
-    # this function should only be called inside the sub-iteration loop
-    # so we can assume that position.sequence is not None
+                continue
+            # note that position.sequence may be Falsey even if not None, for example
+            # if all it has is an autofocus plan.  In that case, we don't recurse.
+            # and we don't hit the continue statement, but we can use the autofocus plan
+            elif position.sequence is not None and position.sequence.autofocus_plan:
+                autofocus_plan = position.sequence.autofocus_plan
+
+        event = MDAEvent(**event_kwargs)
+        if autofocus_plan:
+            af_event = autofocus_plan.event(event)
+            if af_event:
+                yield af_event
+        yield event
+
+
+def _position_offsets(
+    position: Position, event_kwargs: MDAEventDict
+) -> tuple[MDAEventDict, PositionDict]:
+    """Determine shifts and position overrides for position subsequences."""
     pos_seq = cast("MDASequence", position.sequence)
-
-    # if the position sequence has no z_plan, then we can use the global z_pos
-    # elif the position has a relative z_plan, then we need to shift the sub_event
+    overrides = MDAEventDict()
+    offsets = PositionDict()
     if not pos_seq.z_plan:
-        kwargs["z_pos"] = z_pos
+        # if this position has no z_plan, we use the z_pos from the parent
+        overrides["z_pos"] = event_kwargs.get("z_pos")
     elif pos_seq.z_plan.is_relative:
-        kwargs["z_pos"] = _shift_axis("z", position.z, sub_event)
+        # otherwise apply z-shifts if this position has a relative z_plan
+        offsets["z_pos"] = position.z or 0.0
 
-    # if the position sequence has no grid_plane, then we can use the global z_pos
-    # elif the position has a relative grid_plan, then we need to shift the sub_event
     if not pos_seq.grid_plan:
-        kwargs["x_pos"] = x_pos
-        kwargs["y_pos"] = y_pos
+        # if this position has no grid plan, we use the x_pos and y_pos from the parent
+        overrides["x_pos"] = event_kwargs.get("x_pos")
+        overrides["y_pos"] = event_kwargs.get("y_pos")
     elif pos_seq.grid_plan.is_relative:
-        kwargs["x_pos"] = _shift_axis("x", position.x, sub_event)
-        kwargs["y_pos"] = _shift_axis("y", position.y, sub_event)
-    return kwargs
+        # otherwise apply x/y shifts if this position has a relative grid plan
+        offsets["x_pos"] = position.x or 0.0
+        offsets["y_pos"] = position.y or 0.0
+    return overrides, offsets
+
+
+def _parse_axes(
+    event: zip[tuple[str, Any]],
+) -> tuple[
+    dict[str, int],
+    float | None,  # time
+    Position | None,
+    GridPosition | None,
+    Channel | None,
+    float | None,  # z
+]:
+    """Parse an individual event from the product of axis iterators.
+
+    Returns typed objects for each axis, and the index of the event.
+    """
+    _ev = dict(event)
+    index = {ax: _ev[ax][0] for ax in INDICES if ax in _ev}
+    axes = (_ev[ax][1] if ax in _ev else None for ax in INDICES)
+    return (index, *axes)  # type: ignore[return-value]
 
 
-def _shift_axis(axis: str, new_val: float | None, event: MDAEvent) -> float | None:
-    """Return a new value for the axis, accounting for the sub_event's position.
+def _should_skip(
+    position: Position | None,
+    channel: Channel | None,
+    index: dict[str, int],
+    z_plan: AnyZPlan | None,
+) -> bool:
+    """Return True if this event should be skipped."""
+    if channel:
+        # skip channels
+        if TIME in index and index[TIME] % channel.acquire_every:
+            return True
 
-    If both new_val and the corresponding axis position for the sub_event are None,
-    return None, otherwise return the sum of the two.
-    """
-    sub_pos = getattr(event, f"{axis}_pos")
-    return (
-        None
-        if new_val is None and sub_pos is None
-        else (new_val or 0) + sub_pos
-        if sub_pos is not None
-        else new_val
+        # only acquire on the middle plane:
+        if not channel.do_stack and z_plan and index[Z] != len(z_plan) // 2:
+            return True
+
+    if not position or not position.sequence:
+        return False
+
+    # NOTE: if we ever add more plans, they will need to be explicitly added
+    # https://github.com/pymmcore-plus/useq-schema/pull/85
+
+    # get if sub-sequence has any plan
+    plans = any(
+        (
+            position.sequence.grid_plan,
+            position.sequence.z_plan,
+            position.sequence.time_plan,
+        )
     )
+    # overwriting the *global* channel index since it is no longer relevant.
+    # if channel IS SPECIFIED in the position.sequence WITH any plan,
+    # we skip otherwise the channel will be acquired twice. Same happens if
+    # the channel IS NOT SPECIFIED but ANY plan is.
+    if (
+        CHANNEL in index
+        and index[CHANNEL] != 0
+        and ((position.sequence.channels and plans) or not plans)
+    ):
+        return True
+    if Z in index and index[Z] != 0 and position.sequence.z_plan:
+        return True
+    if GRID in index and index[GRID] != 0 and position.sequence.grid_plan:
+        return True
+    return False
+
+
+def _xyzpos(
+    position: Position | None,
+    channel: Channel | None,
+    z_plan: AnyZPlan | None,
+    grid: GridPosition | None = None,
+    z_pos: float | None = None,
+) -> MDAEventDict:
+    if z_pos is not None:
+        # combine z_pos with z_offset
+        if channel and channel.z_offset is not None:
+            z_pos += channel.z_offset
+        if z_plan and z_plan.is_relative:
+            # TODO: either disallow without position z, or add concept of "current"
+            z_pos += getattr(position, Z, None) or 0
+    elif position:
+        z_pos = position.z
+
+    if grid:
+        x_pos: Optional[float] = grid.x
+        y_pos: Optional[float] = grid.y
+        if grid.is_relative:
+            px = getattr(position, "x", 0) or 0
+            py = getattr(position, "y", 0) or 0
+            x_pos = x_pos + px if x_pos is not None else None
+            y_pos = y_pos + py if y_pos is not None else None
+    else:
+        x_pos = getattr(position, "x", None)
+        y_pos = getattr(position, "y", None)
+
+    return {"x_pos": x_pos, "y_pos": y_pos, "z_pos": z_pos}
```

### Comparing `useq_schema-0.2.1/src/useq/_position.py` & `useq_schema-0.3.0/src/useq/_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Generator, Optional
 
 import numpy as np
 
-from ._base_model import FrozenModel
+from useq._base_model import FrozenModel
 
 if TYPE_CHECKING:
     from useq import MDASequence
 
 
 class Position(FrozenModel):
     """Define a position in 3D space.
```

### Comparing `useq_schema-0.2.1/src/useq/_time.py` & `useq_schema-0.3.0/src/useq/_time.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import Any, Callable, Generator, Iterator, Sequence, Union
 
+from pydantic import Field
 from pydantic.datetime_parse import parse_duration
-from pydantic.types import PositiveInt
 
-from ._base_model import FrozenModel
+from useq._base_model import FrozenModel
 
 
 class timedelta(datetime.timedelta):
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate
 
@@ -30,52 +30,49 @@
 
     def deltas(self) -> Iterator[datetime.timedelta]:
         current = timedelta(0)
         for _ in range(self.loops):  # type: ignore  # TODO
             yield current
             current += self.interval  # type: ignore  # TODO
 
-    def __bool__(self) -> bool:
-        return len(self) > 0
-
 
 class TIntervalLoops(TimePlan):
     """Define temporal sequence using interval and number of loops.
 
     Attributes
     ----------
     interval : str | timedelta
         Time between frames.
-    loops : PositiveInt
+    loops : int
         Number of frames.
     prioritize_duration : bool
         If `True`, instructs engine to prioritize duration over number of frames in case
         of conflict. By default, `False`.
     """
 
     interval: timedelta
-    loops: PositiveInt
+    loops: int = Field(..., gt=0)
 
 
 class TDurationLoops(TimePlan):
     """Define temporal sequence using duration and number of loops.
 
     Attributes
     ----------
     duration : str | timedelta
         Total duration of sequence.
-    loops : PositiveInt
+    loops : int
         Number of frames.
     prioritize_duration : bool
         If `True`, instructs engine to prioritize duration over number of frames in case
         of conflict. By default, `False`.
     """
 
     duration: timedelta
-    loops: PositiveInt
+    loops: int = Field(..., gt=0)
 
     @property
     def interval(self) -> datetime.timedelta:
         # -1 makes it so that the last loop will *occur* at duration, not *finish*
         return self.duration / (self.loops - 1)
 
 
@@ -98,30 +95,23 @@
     prioritize_duration: bool = True
 
     @property
     def loops(self) -> int:
         return self.duration // self.interval + 1
 
 
-class NoT(TimePlan):
-    """Don't acquire a time sequence."""
-
-    def deltas(self) -> Iterator[datetime.timedelta]:
-        yield from ()
-
-
-SinglePhaseTimePlan = Union[TIntervalDuration, TIntervalLoops, TDurationLoops, NoT]
+SinglePhaseTimePlan = Union[TIntervalDuration, TIntervalLoops, TDurationLoops]
 
 
 class MultiPhaseTimePlan(TimePlan):
     """Time sequence composed of multiple phases.
 
     Attributes
     ----------
-    phases : Sequence[TIntervalDuration | TIntervalLoops | TDurationLoops | NoT]
+    phases : Sequence[TIntervalDuration | TIntervalLoops | TDurationLoops]
         Sequence of time plans.
     """
 
     phases: Sequence[SinglePhaseTimePlan]
 
     def deltas(self) -> Iterator[datetime.timedelta]:
         accum = datetime.timedelta(0)
```

### Comparing `useq_schema-0.2.1/src/useq/_utils.py` & `useq_schema-0.3.0/src/useq/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Iterable, Iterator, Mapping, Tuple, TypeVar, Union
 
+from pydantic import validator
+
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 
 class ReadOnlyDict(Mapping[KT, VT]):
     def __init__(
         self, data: Union[Mapping[KT, VT], Iterable[Tuple[KT, VT]]] = ()
@@ -17,7 +19,12 @@
         return len(self._data)
 
     def __iter__(self) -> Iterator[KT]:
         return iter(self._data)
 
     def __repr__(self) -> str:
         return repr(self._data)
+
+
+def list_cast(field: str) -> classmethod:
+    v = validator(field, pre=True, allow_reuse=True, check_fields=False)
+    return v(list)
```

### Comparing `useq_schema-0.2.1/src/useq/_z.py` & `useq_schema-0.3.0/src/useq/_z.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterator, List, Sequence, Union
 
 import numpy as np
 
-from ._base_model import FrozenModel
+from useq._base_model import FrozenModel
+from useq._utils import list_cast
 
 
 class ZPlan(FrozenModel):
     go_up: bool
 
     def __iter__(self) -> Iterator[float]:  # type: ignore
         positions = self.positions()
@@ -119,14 +120,16 @@
         If `True` (the default), visits points in the order provided, otherwise in
         reverse.
     """
 
     relative: List[float]
     go_up: bool = True
 
+    _normrel = list_cast("relative")
+
     def positions(self) -> Sequence[float]:
         return self.relative
 
 
 class ZAbsolutePositions(ZPlan):
     """Define Z as a list of absolute positions.
 
@@ -138,32 +141,22 @@
         If `True` (the default), visits points in the order provided, otherwise in
         reverse.
     """
 
     absolute: List[float]
     go_up: bool = True
 
+    _normabs = list_cast("absolute")
+
     def positions(self) -> Sequence[float]:
         return self.absolute
 
     @property
     def is_relative(self) -> bool:
         return False
 
 
-class NoZ(ZPlan):
-    """Don't acquire Z."""
-
-    go_up: bool = True
-
-    def positions(self) -> Sequence[float]:
-        return []
-
-    def __bool__(self) -> bool:
-        return False
-
-
 # order matters... this is the order in which pydantic will try to coerce input.
 # should go from most specific to least specific
 AnyZPlan = Union[
-    ZTopBottom, ZAboveBelow, ZRangeAround, ZAbsolutePositions, ZRelativePositions, NoZ
+    ZTopBottom, ZAboveBelow, ZRangeAround, ZAbsolutePositions, ZRelativePositions
 ]
```

### Comparing `useq_schema-0.2.1/tests/conftest.py` & `useq_schema-0.3.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,8 +28,13 @@
         ],
         time_plan=[
             {"interval": 3, "loops": 3},
             {"duration": {"minutes": 40}, "interval": 10},
         ],
         z_plan={"range": 1.0, "step": 0.5},
         grid_plan={"rows": 2, "columns": 1},
+        autofocus_plan={
+            "autofocus_device_name": "Z",
+            "autofocus_motor_offset": 50,
+            "axes": ("c",),
+        },
     )
```

### Comparing `useq_schema-0.2.1/tests/test_grid.py` & `useq_schema-0.3.0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/tests/test_sequence.py` & `useq_schema-0.3.0/tests/test_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 from useq import (
     Channel,
     GridFromEdges,
     GridRelative,
     MDAEvent,
     MDASequence,
-    NoGrid,
-    NoT,
-    NoZ,
     Position,
     TDurationLoops,
     TIntervalDuration,
     TIntervalLoops,
     ZAboveBelow,
     ZAbsolutePositions,
     ZRangeAround,
@@ -28,22 +25,20 @@
 _T = List[Tuple[Any, Sequence[float]]]
 
 z_as_class: _T = [
     (ZAboveBelow(above=8, below=4, step=2), [-4, -2, 0, 2, 4, 6, 8]),
     (ZAbsolutePositions(absolute=[0, 0.5, 5]), [0, 0.5, 5]),
     (ZRelativePositions(relative=[0, 0.5, 5]), [0, 0.5, 5]),
     (ZRangeAround(range=8, step=1), [-4, -3, -2, -1, 0, 1, 2, 3, 4]),
-    (NoZ(), []),
 ]
 z_as_dict: _T = [
     ({"above": 8, "below": 4, "step": 2}, [-4, -2, 0, 2, 4, 6, 8]),
     ({"range": 8, "step": 1}, [-4, -3, -2, -1, 0, 1, 2, 3, 4]),
     ({"absolute": [0, 0.5, 5]}, [0, 0.5, 5]),
     ({"relative": [0, 0.5, 5]}, [0, 0.5, 5]),
-    (None, []),
 ]
 z_inputs = z_as_class + z_as_dict
 
 t_as_class: _T = [
     # frame every second for 4 seconds
     (TIntervalDuration(interval=1, duration=4), [0, 1, 2, 3, 4]),
     # 5 frames spanning 8 seconds
@@ -56,25 +51,23 @@
             TIntervalDuration(interval=1, duration=4),
         ],
         [0, 0.25, 0.5, 0.75, 1, 2, 3, 4, 5],
     ),
 ]
 
 t_as_dict: _T = [
-    (None, []),
     ({"interval": 0.5, "duration": 2}, [0, 0.5, 1, 1.5, 2]),
     ({"loops": 5, "duration": 8}, [0, 2, 4, 6, 8]),
     ({"loops": 5, "interval": 0.25}, [0, 0.25, 0.5, 0.75, 1]),
     (
         [{"loops": 5, "interval": 0.25}, {"interval": 1, "duration": 4}],
         [0, 0.25, 0.50, 0.75, 1, 2, 3, 4, 5],
     ),
     ({"loops": 5, "duration": {"milliseconds": 8}}, [0, 0.002, 0.004, 0.006, 0.008]),
     ({"loops": 5, "duration": {"seconds": 8}}, [0, 2, 4, 6, 8]),
-    (NoT(), []),
 ]
 t_inputs = t_as_class + t_as_dict
 
 g_as_dict = [
     (
         {"overlap": 10.0, "rows": 1, "columns": 2, "relative_to": "center"},
         [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.center],
@@ -83,27 +76,25 @@
         {"overlap": 10.0, "rows": 1, "columns": 2, "relative_to": "top_left"},
         [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.top_left],
     ),
     (
         {"overlap": 10.0, "top": 0.0, "left": 0.0, "bottom": 2.0, "right": 2.0},
         [(10.0, 10.0), OrderMode.row_wise_snake, 0.0, 0.0, 2.0, 2.0],
     ),
-    ({}, [(0.0, 0.0), OrderMode.row_wise_snake]),
 ]
 
 g_as_class = [
     (
         GridRelative(overlap=10.0, rows=1, columns=2, relative_to="center"),
         [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.center],
     ),
     (
         GridFromEdges(overlap=10.0, top=0.0, left=0, bottom=2, right=2),
         [(10.0, 10.0), OrderMode.row_wise_snake, 0.0, 0.0, 2.0, 2.0],
     ),
-    (NoGrid(), [(0.0, 0.0), OrderMode.row_wise_snake]),
 ]
 g_inputs = g_as_class + g_as_dict
 
 
 all_orders = ["".join(i) for i in itertools.permutations("tpgcz")]
 
 c_inputs = [
@@ -321,7 +312,12 @@
 def test_mda_warns_extra() -> None:
     with pytest.warns(UserWarning, match="got unknown keyword arguments"):
         seq = MDASequence(random_key="random_value")
     assert not hasattr(seq, "random_key")
 
     with pytest.warns(UserWarning, match="got unknown keyword arguments"):
         Position(random_key="random_value")
+
+
+def test_skip_channel_do_stack_no_zplan():
+    mda = MDASequence(channels=[{"config": "DAPI", "do_stack": False}])
+    assert len(list(mda)) == 1
```

### Comparing `useq_schema-0.2.1/tests/fixtures/mda.json` & `useq_schema-0.3.0/tests/fixtures/mda.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8744140625%*

 * *Differences: {"'autofocus_plan'": "OrderedDict([('autofocus_device_name', 'Z'), ('autofocus_motor_offset', "*

 * *                     "50.0), ('axes', ['c'])])",*

 * * "'stage_positions'": "{1: {'sequence': {'time_plan': None, 'autofocus_plan': None}}}"}*

```diff
@@ -1,8 +1,15 @@
 {
+    "autofocus_plan": {
+        "autofocus_device_name": "Z",
+        "autofocus_motor_offset": 50.0,
+        "axes": [
+            "c"
+        ]
+    },
     "axis_order": "tpgcz",
     "channels": [
         {
             "acquire_every": 1,
             "camera": null,
             "config": "Cy5",
             "do_stack": true,
@@ -49,31 +56,30 @@
             "x": 10.0,
             "y": 20.0,
             "z": null
         },
         {
             "name": "test_name",
             "sequence": {
+                "autofocus_plan": null,
                 "axis_order": "tpgcz",
                 "channels": [],
                 "grid_plan": {
                     "columns": 3,
                     "mode": "row_wise_snake",
                     "overlap": [
                         0.0,
                         0.0
                     ],
                     "relative_to": "center",
                     "rows": 2
                 },
                 "metadata": {},
                 "stage_positions": [],
-                "time_plan": {
-                    "prioritize_duration": false
-                },
+                "time_plan": null,
                 "z_plan": {
                     "above": 10.0,
                     "below": 0.0,
                     "go_up": true,
                     "step": 1.0
                 }
             },
```

### Comparing `useq_schema-0.2.1/.gitignore` & `useq_schema-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/LICENSE` & `useq_schema-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/README.md` & `useq_schema-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.1/pyproject.toml` & `useq_schema-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -55,49 +55,54 @@
 [tool.hatch.version]
 source = "vcs"
 
 # https://hatch.pypa.io/latest/config/build/#file-selection
 [tool.hatch.build.targets.wheel]
 packages = ["src/useq"]
 
-# https://github.com/charliermarsh/ruff
+# https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 line-length = 88
 target-version = "py37"
 src = ["src", "tests"]
 select = [
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I",    # isort
     "UP",   # pyupgrade
     "S",    # bandit
     "C4",   # comprehensions
     "B",    # bugbear
     "A001", # Variable shadowing a python builtin
+    "TCH",  # flake8-type-checking
+    "TID",  # flake8-tidy-imports
     "RUF",  # ruff-specific rules
+    "PERF", # performance
 ]
 ignore = [
-    "D100", # Missing docstring in public module
-    "D104", # Missing docstring in public package
-    "D107", # Missing docstring in __init__
-    "D203", # 1 blank line required before class docstring
-    "D212", # Multi-line docstring summary should start at the first line
-    "D213", # Multi-line docstring summary should start at the second line
-    "D401", # Imperative mood
-    "D413", # Missing blank line after last section
-    "D416", # Section name should end with a colon
+    "D100",  # Missing docstring in public module
+    "D104",  # Missing docstring in public package
+    "D107",  # Missing docstring in __init__
+    "D203",  # 1 blank line required before class docstring
+    "D212",  # Multi-line docstring summary should start at the first line
+    "D213",  # Multi-line docstring summary should start at the second line
+    "D401",  # Imperative mood
+    "D413",  # Missing blank line after last section
+    "D416",  # Section name should end with a colon
+    "UP006",
+    "UP007",
 ]
 
-[tool.ruff.pyupgrade]
-# Preserve types, even if a file imports `from __future__ import annotations`.
-keep-runtime-typing = true
-
 [tool.ruff.per-file-ignores]
-"tests/*.py" = ["D", "S101"]
+"tests/*.py" = ["D", "S101", "E501"]
+
+[tool.ruff.flake8-tidy-imports]
+# Disallow all relative imports.
+ban-relative-imports = "all"
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = ["error"]
```

### Comparing `useq_schema-0.2.1/PKG-INFO` & `useq_schema-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.2.1
+Version: 0.3.0
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
```

