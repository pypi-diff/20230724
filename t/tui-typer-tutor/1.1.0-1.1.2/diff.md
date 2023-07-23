# Comparing `tmp/tui_typer_tutor-1.1.0.tar.gz` & `tmp/tui_typer_tutor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_typer_tutor-1.1.0.tar", max compression
+gzip compressed data, was "tui_typer_tutor-1.1.2.tar", max compression
```

## Comparing `tui_typer_tutor-1.1.0.tar` & `tui_typer_tutor-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-06-24 01:02:07.591613 tui_typer_tutor-1.1.0/LICENSE
--rw-r--r--   0        0        0     2780 2023-07-07 09:55:11.938058 tui_typer_tutor-1.1.0/docs/README.md
--rw-r--r--   0        0        0     1527 2023-07-07 09:55:06.667130 tui_typer_tutor-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      335 2023-07-07 09:55:06.660826 tui_typer_tutor-1.1.0/tui_typer_tutor/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 09:58:56.713475 tui_typer_tutor-1.1.0/tui_typer_tutor/app/__init__.py
--rw-r--r--   0        0        0      659 2023-06-28 01:18:02.055916 tui_typer_tutor-1.1.0/tui_typer_tutor/app/ttt.py
--rw-r--r--   0        0        0       51 2023-06-26 01:07:36.370648 tui_typer_tutor-1.1.0/tui_typer_tutor/constants/__init__.py
--rw-r--r--   0        0        0     1250 2023-07-01 23:10:42.700299 tui_typer_tutor-1.1.0/tui_typer_tutor/constants/display_to_textual.py
--rw-r--r--   0        0        0        0 2023-06-25 00:11:43.547397 tui_typer_tutor-1.1.0/tui_typer_tutor/core/__init__.py
--rw-r--r--   0        0        0      554 2023-06-27 12:42:22.407622 tui_typer_tutor-1.1.0/tui_typer_tutor/core/config.py
--rw-r--r--   0        0        0     1824 2023-06-29 12:13:08.507232 tui_typer_tutor-1.1.0/tui_typer_tutor/core/metrics.py
--rw-r--r--   0        0        0       46 2023-06-25 23:10:12.527578 tui_typer_tutor-1.1.0/tui_typer_tutor/core/scrolled_labels.py
--rw-r--r--   0        0        0      537 2023-06-28 01:17:23.376603 tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.py
--rw-r--r--   0        0        0      322 2023-07-01 23:10:42.700361 tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.txt
--rw-r--r--   0        0        0     2010 2023-06-27 12:45:17.269183 tui_typer_tutor-1.1.0/tui_typer_tutor/core/typing.py
--rw-r--r--   0        0        0      844 2023-06-27 12:51:26.782478 tui_typer_tutor-1.1.0/tui_typer_tutor/core/uninstall.py
--rw-r--r--   0        0        0        0 2023-06-24 09:59:11.688594 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/__init__.py
--rw-r--r--   0        0        0     1135 2023-06-28 01:18:02.056168 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/help.py
--rw-r--r--   0        0        0     4455 2023-07-01 23:06:03.898939 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/main.py
--rw-r--r--   0        0        0     1082 2023-06-29 12:08:41.177093 tui_typer_tutor-1.1.0/tui_typer_tutor/scripts.py
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 tui_typer_tutor-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-24 01:02:07.591613 tui_typer_tutor-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2780 2023-07-23 22:49:06.221753 tui_typer_tutor-1.1.2/docs/README.md
+-rw-r--r--   0        0        0     1556 2023-07-23 22:49:01.951673 tui_typer_tutor-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1838 2023-07-23 22:49:01.945416 tui_typer_tutor-1.1.2/tui_typer_tutor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 09:58:56.713475 tui_typer_tutor-1.1.2/tui_typer_tutor/app/__init__.py
+-rw-r--r--   0        0        0      659 2023-06-28 01:18:02.055916 tui_typer_tutor-1.1.2/tui_typer_tutor/app/ttt.py
+-rw-r--r--   0        0        0       51 2023-06-26 01:07:36.370648 tui_typer_tutor-1.1.2/tui_typer_tutor/constants/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-01 23:10:42.700299 tui_typer_tutor-1.1.2/tui_typer_tutor/constants/display_to_textual.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:11:43.547397 tui_typer_tutor-1.1.2/tui_typer_tutor/core/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-23 22:47:53.049997 tui_typer_tutor-1.1.2/tui_typer_tutor/core/config.py
+-rw-r--r--   0        0        0     1824 2023-06-29 12:13:08.507232 tui_typer_tutor-1.1.2/tui_typer_tutor/core/metrics.py
+-rw-r--r--   0        0        0       46 2023-06-25 23:10:12.527578 tui_typer_tutor-1.1.2/tui_typer_tutor/core/scrolled_labels.py
+-rw-r--r--   0        0        0      537 2023-06-28 01:17:23.376603 tui_typer_tutor-1.1.2/tui_typer_tutor/core/seed_data.py
+-rw-r--r--   0        0        0      322 2023-07-01 23:10:42.700361 tui_typer_tutor-1.1.2/tui_typer_tutor/core/seed_data.txt
+-rw-r--r--   0        0        0     2017 2023-07-19 01:56:34.848253 tui_typer_tutor-1.1.2/tui_typer_tutor/core/typing.py
+-rw-r--r--   0        0        0      844 2023-06-27 12:51:26.782478 tui_typer_tutor-1.1.2/tui_typer_tutor/core/uninstall.py
+-rw-r--r--   0        0        0        0 2023-06-24 09:59:11.688594 tui_typer_tutor-1.1.2/tui_typer_tutor/screens/__init__.py
+-rw-r--r--   0        0        0     1135 2023-06-28 01:18:02.056168 tui_typer_tutor-1.1.2/tui_typer_tutor/screens/help.py
+-rw-r--r--   0        0        0     4455 2023-07-01 23:06:03.898939 tui_typer_tutor-1.1.2/tui_typer_tutor/screens/main.py
+-rw-r--r--   0        0        0     1082 2023-06-29 12:08:41.177093 tui_typer_tutor-1.1.2/tui_typer_tutor/scripts.py
+-rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 tui_typer_tutor-1.1.2/PKG-INFO
```

### Comparing `tui_typer_tutor-1.1.0/LICENSE` & `tui_typer_tutor-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/docs/README.md` & `tui_typer_tutor-1.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/pyproject.toml` & `tui_typer_tutor-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.1.0"
+version = "1.1.2"
 version_files = ["pyproject.toml:^version", "tui_typer_tutor/__init__.py:^__version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 1 - Planning",
   "License :: OSI Approved :: MIT License",
@@ -19,27 +19,28 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "tui_typer_tutor"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/tui-typer-tutor"
-version = "1.1.0"
+version = "1.1.2"
 
 [tool.poetry.dependencies]
 python = "^3.11.2"
 arguably = ">=1.2.5"
 bidict = ">=0.22.1"
-corallium = ">=0.2.2"
+corallium = ">=0.3.0"
 platformdirs = ">=3.8.0"
-pydantic = ">=1.10.9"
+pydantic = ">=2.0.3"
+pydantic-settings = ">=2.0.2"
 textual = ">=0.28.0"
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.2.6"}
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.5.0"}
 freezegun = ">=1.2.2"
 pytest-cache-assert = ">=3.0.8"
 
 [tool.poetry.scripts]
 ttt = "tui_typer_tutor.scripts:start"
 tui-typer-tutor = "tui_typer_tutor.scripts:start"
```

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/app/ttt.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/app/ttt.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/constants/display_to_textual.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/constants/display_to_textual.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/core/config.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/core/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """Config."""
 
 from functools import lru_cache
 from pathlib import Path
 
 from beartype import beartype
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 DEFAULT_SEED_FILE = Path(__file__).parent / 'seed_data.txt'
 """Default seed file if not specified."""
 
 
 class Config(BaseSettings):
     """Application config."""
 
     seed_file: Path = DEFAULT_SEED_FILE
-
-    class Config:
-        """Extended Configuration."""
-
-        env_prefix = 'TYPER_'
+    model_config = SettingsConfigDict(env_prefix='TYPER_')
 
 
 @lru_cache(maxsize=1)
 @beartype
 def get_config() -> Config:
     """Retrieve the application config."""
     return Config()
```

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/core/metrics.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/core/metrics.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/core/seed_data.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/core/typing.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/core/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         """Displayed text."""
         return DISPLAY_TO_TEXTUAL.inverse.get(self.textual) or UNKNOWN
 
 
 class TypedKey(ExpectedKey):
     """Typed Key."""
 
-    expected: ExpectedKey | None
+    expected: ExpectedKey | None = None
     """Store the expected key when typed and expected become out-of-sync."""
 
     @property
     def was_correct(self) -> bool:
         """If typed key matches expected."""
         return self.expected is not None and self.text == self.expected.text
```

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/core/uninstall.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/core/uninstall.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/screens/help.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/screens/help.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/screens/main.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/screens/main.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/tui_typer_tutor/scripts.py` & `tui_typer_tutor-1.1.2/tui_typer_tutor/scripts.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.1.0/PKG-INFO` & `tui_typer_tutor-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: tui-typer-tutor
-Version: 1.1.0
+Version: 1.1.2
 Summary: Uncomplicated terminal typing practice.
 Home-page: https://github.com/kyleking/tui-typer-tutor
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.11.2,<4.0.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arguably (>=1.2.5)
 Requires-Dist: bidict (>=0.22.1)
-Requires-Dist: corallium (>=0.2.2)
+Requires-Dist: corallium (>=0.3.0)
 Requires-Dist: platformdirs (>=3.8.0)
-Requires-Dist: pydantic (>=1.10.9)
+Requires-Dist: pydantic (>=2.0.3)
+Requires-Dist: pydantic-settings (>=2.0.2)
 Requires-Dist: textual (>=0.28.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/tui-typer-tutor/issues
 Project-URL: Changelog, https://github.com/kyleking/tui-typer-tutor/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://tui-typer-tutor.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/tui-typer-tutor
 Description-Content-Type: text/markdown
```

