# Comparing `tmp/halig-0.3.2.tar.gz` & `tmp/halig-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.3.2.tar", last modified: Wed May 17 17:01:10 2023, max compression
+gzip compressed data, was "halig-0.4.0.tar", last modified: Mon Jul 24 17:53:27 2023, max compression
```

## Comparing `halig-0.3.2.tar` & `halig-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.3.2/LICENSE
--rw-r--r--   0        0        0     1633 2023-05-13 08:52:41.111337 halig-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.2/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-05-17 17:00:35.079571 halig-0.3.2/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.2/halig/commands/__init__.py
--rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/base.py
--rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.3.2/halig/commands/edit.py
--rw-r--r--   0        0        0     1397 2023-05-17 09:18:35.363381 halig-0.3.2/halig/commands/import_unencrypted.py
--rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/notebooks.py
--rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/show.py
--rw-r--r--   0        0        0     1418 2023-05-09 18:17:46.623174 halig-0.3.2/halig/encryption.py
--rw-r--r--   0        0        0     1573 2023-05-13 10:06:04.121116 halig-0.3.2/halig/literals.py
--rw-r--r--   0        0        0     3757 2023-05-14 19:00:10.001739 halig-0.3.2/halig/main.py
--rw-r--r--   0        0        0     3420 2023-05-13 10:13:03.572546 halig-0.3.2/halig/settings.py
--rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.3.2/halig/utils.py
--rw-r--r--   0        0        0     2717 2023-05-17 17:01:10.991488 halig-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.3.2/tests/commands/__init__.py
--rw-r--r--   0        0        0     2279 2023-05-14 18:42:09.595033 halig-0.3.2/tests/commands/conftest.py
--rw-r--r--   0        0        0     1168 2023-05-09 17:58:32.738050 halig-0.3.2/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1423 2023-05-17 16:53:27.712608 halig-0.3.2/tests/commands/test_import.py
--rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.3.2/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.3.2/tests/commands/test_show.py
--rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.3.2/tests/test_encryption.py
--rw-r--r--   0        0        0     1320 2023-05-13 09:11:29.085662 halig-0.3.2/tests/test_settings.py
--rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.3.2/tests/test_utils.py
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 halig-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-06-19 16:50:30.000000 halig-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1635 2023-06-19 16:50:30.000000 halig-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.0/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 17:53:11.853227 halig-0.4.0/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.0/halig/commands/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-24 17:42:38.529912 halig-0.4.0/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-06-19 16:50:47.000000 halig-0.4.0/halig/commands/edit.py
+-rw-r--r--   0        0        0     1397 2023-06-19 16:50:47.000000 halig-0.4.0/halig/commands/import_unencrypted.py
+-rw-r--r--   0        0        0     1128 2023-07-22 12:38:35.359342 halig-0.4.0/halig/commands/notebooks.py
+-rw-r--r--   0        0        0      622 2023-07-24 17:42:09.847162 halig-0.4.0/halig/commands/reencrypt.py
+-rw-r--r--   0        0        0     3911 2023-07-24 17:51:38.933140 halig-0.4.0/halig/commands/search.py
+-rw-r--r--   0        0        0     1199 2023-06-19 16:50:47.000000 halig-0.4.0/halig/commands/show.py
+-rw-r--r--   0        0        0     1468 2023-07-24 17:49:45.965214 halig-0.4.0/halig/encryption.py
+-rw-r--r--   0        0        0     2213 2023-07-24 17:51:37.854150 halig-0.4.0/halig/literals.py
+-rw-r--r--   0        0        0     4358 2023-07-24 17:52:16.472798 halig-0.4.0/halig/main.py
+-rw-r--r--   0        0        0     3615 2023-07-22 11:29:23.649835 halig-0.4.0/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-06-19 16:50:47.000000 halig-0.4.0/halig/utils.py
+-rw-r--r--   0        0        0     2786 2023-07-24 17:53:27.877064 halig-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/__init__.py
+-rw-r--r--   0        0        0     2279 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1168 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1423 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/test_import.py
+-rw-r--r--   0        0        0     1563 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0      426 2023-07-24 17:50:25.691829 halig-0.4.0/tests/commands/test_reencrypt.py
+-rw-r--r--   0        0        0     1141 2023-06-19 16:50:47.000000 halig-0.4.0/tests/commands/test_show.py
+-rw-r--r--   0        0        0     2831 2023-07-23 15:39:00.934986 halig-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2276 2023-06-19 16:50:47.000000 halig-0.4.0/tests/test_encryption.py
+-rw-r--r--   0        0        0     1320 2023-07-22 11:21:54.274911 halig-0.4.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1482 2023-06-19 16:50:47.000000 halig-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 halig-0.4.0/PKG-INFO
```

### Comparing `halig-0.3.2/LICENSE` & `halig-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/README.md` & `halig-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Features
 
 - Simple notebooks management with paths autocompletion
 - Passphrase-less, fully-encrypted notes, compatible with existing SSH keys 
 - No external `age` binary needed
 - Almost all `age` advantages, like having multiple keys for encryption and decryption
-- Remote (HTTP) public keys import: e.g: github.com/<username>.keys
+- Remote (HTTP) public keys import: e.g: github.com/\<username\>.keys
 
 ## Install
 
 ```shell
 pipx install halig # or pip
 ```
```

### Comparing `halig-0.3.2/halig/commands/edit.py` & `halig-0.4.0/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/halig/commands/import_unencrypted.py` & `halig-0.4.0/halig/commands/import_unencrypted.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/halig/commands/notebooks.py` & `halig-0.4.0/halig/commands/notebooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         q: deque[tuple[Path, Tree, int | float]] = deque([(root_path, tree, 0)])
         while q:
             current_folder_path, current_tree_node, depth = q.popleft()
             if depth >= self.max_depth:
                 break
             for item in sorted(current_folder_path.iterdir()):
                 if item.is_dir():
-                    item_tree_node = current_tree_node.add(item.name)
-                    q.append((item, item_tree_node, depth + 1))
+                    if item.name != ".git":
+                        item_tree_node = current_tree_node.add(item.name)
+                        q.append((item, item_tree_node, depth + 1))
                 else:
                     current_tree_node.add(item.name)
         return tree
 
     def run(self):
         print(self.build_tree(self.settings.notebooks_root_path))  # pragma: no cover
```

### Comparing `halig-0.3.2/halig/commands/show.py` & `halig-0.4.0/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/halig/encryption.py` & `halig-0.4.0/halig/encryption.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 
     def encrypt(self, data: str | bytes) -> bytes:
         if isinstance(data, str):
             data = data.encode()
         return rage_encrypt(data, self.recipients)  # type: ignore[no-any-return]
 
     def decrypt(self, data: bytes) -> bytes:
+        if not len(data):
+            return data
         return rage_decrypt(data, self.identities)  # type: ignore[no-any-return]
```

### Comparing `halig-0.3.2/halig/literals.py` & `halig-0.4.0/halig/literals.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 # COMMANDS
 COMMANDS_NOTEBOOKS_HELP = "List all notebooks and notes, tree-style"
 COMMANDS_EDIT_HELP = "Edit or add a note into a notebook"
 COMMANDS_SHOW_HELP = "Show a note's contents"
 COMMANDS_VERSION = "Show halig's version"
 COMMANDS_IMPORT_HELP = "Encrypt existing unencrypted files"
+COMMANDS_SEARCH_HELP = """Perform a full-text search against all your notes,
+which are indexed into a SQLite FTS5 database located at `~/.cache/halig/halig.db`
+"""
+COMMANDS_REENCRYPT_HELP = """Reencrypt all available notes. This operation is useful
+when new public keys have been added to the config file and you want the notes
+to be seen by the new pairing private keys"""
 
 # OPTIONS
 OPTION_CONFIG_HELP = "Configuration file. Must be YAML and schema compatible"
 OPTION_LEVEL_HELP = (
     "Tree max recursion level; negative numbers indicate a value of infinity"
 )
 OPTION_UNLINK_HELP = """Setting this will remove the original markdown files;
 only the newly encrypted .age files will be preserved. Backup your data first
 """
+OPTION_INDEX_HELP = """Index the SQLite database with your notes contents. The first
+time you perform a search, this flag should be set. Afterwards, you should only index
+when new notes have been added or older ones have been changed, since it's a slow
+operation"""
 # ARGUMENTS
 ARGUMENT_EDIT_NOTE_HELP = """A valid, settings-relative path.
 Be aware that valid can also mean implicit notes, that is, pointing to a
 current-day note just by its notebook name. For example, if today is
 2023-04-04 and you have a notebook containing a 2023-04-04.age note,
 simply pointing to the notebook's name, e.g. `halig edit notebook` will
 edit the 2023-04-04.age note. Also keep in mind that the note may or may
```

### Comparing `halig-0.3.2/halig/main.py` & `halig-0.4.0/halig/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from typer import Argument, Option, Typer
 
 from halig import literals
 from halig.__version__ import __version__
 from halig.commands.edit import EditCommand
 from halig.commands.import_unencrypted import ImportCommand
 from halig.commands.notebooks import NotebooksCommand
+from halig.commands.reencrypt import ReencryptCommand
+from halig.commands.search import SearchCommand
 from halig.commands.show import ShowCommand
 from halig.settings import load_from_file
 from halig.utils import capture
 
 app = Typer(pretty_exceptions_enable=False, pretty_exceptions_show_locals=False)
 
 config_option = Option(None, "--config", "-c", help=literals.OPTION_CONFIG_HELP)
@@ -110,14 +112,37 @@
             )
             if should_unlink in ["N", "n"]:
                 command.unlink = False
 
         command.run()
 
 
+@app.command(help=literals.COMMANDS_SEARCH_HELP)
+def search(
+    term: str,
+    index: bool = Option(False, help=literals.OPTION_INDEX_HELP),  # noqa: B008
+):
+    settings = load_from_file()
+    command = SearchCommand(
+        term=term,
+        index=index,
+        settings=settings,
+    )
+    command.run()
+
+
+@app.command(help=literals.COMMANDS_REENCRYPT_HELP)
+def reencrypt():
+    settings = load_from_file()
+    command = ReencryptCommand(
+        settings=settings,
+    )
+    command.run()
+
+
 @app.command(help=literals.COMMANDS_VERSION)
 @capture
 def version():
     print(__version__)
 
 
 if __name__ == "__main__":
```

### Comparing `halig-0.3.2/halig/settings.py` & `halig-0.4.0/halig/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from pathlib import Path
 from typing import Any
 
 import httpx
 import httpx_cache
 import platformdirs
 import yaml
-from pydantic import BaseSettings, DirectoryPath, FilePath, HttpUrl, validator
+from pydantic import DirectoryPath, Field, FilePath, HttpUrl, field_validator
+from pydantic_core import Url
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class Settings(BaseSettings):
     """Settings model. It mainly stores paths that are interesting to the project.
      All the path-attributes described below have a validity check upon instantiation,
      meaning that they should exist and be readable and/or writable
 
@@ -21,35 +23,41 @@
             Defaults to `[~/.ssh/id_ed25519]`
         recipient_paths (list[FilePath|HttpUrl]): a list *valid* paths of public keys,
             which usually is understood as a public key. Defaults to
             `[~/.ssh/id_ed25519.pub]`
     """
 
     notebooks_root_path: DirectoryPath
-    identity_paths: list[FilePath] = [Path("~/.ssh/id_ed25519").expanduser()]
-    recipient_paths: list[FilePath | HttpUrl] = [
-        Path("~/.ssh/id_ed25519.pub").expanduser(),
-    ]
-
-    @validator("identity_paths", "recipient_paths", pre=True)
-    def validate_paths(cls, v: Any):  # noqa: N805
+    identity_paths: list[FilePath] = Field(
+        default=[Path("~/.ssh/id_ed25519").expanduser()],
+    )
+    recipient_paths: list[FilePath | HttpUrl] = Field(
+        default=[
+            Path("~/.ssh/id_ed25519.pub").expanduser(),
+        ],
+    )
+
+    @field_validator("identity_paths", "recipient_paths", mode="before")
+    @classmethod
+    def validate_paths(cls, v: Any):
         if not isinstance(v, list):
             v = [v]
         new_v = []
         for path in v:
             new_path = path
             if isinstance(path, str) and not path.startswith("http"):
                 new_path = Path(path)
             new_v.append(
                 new_path.expanduser() if isinstance(new_path, Path) else new_path,
             )
         return new_v
 
-    @validator("notebooks_root_path", pre=True)
-    def validate_notebooks_path(cls, v: Any):  # noqa: N805
+    @field_validator("notebooks_root_path", mode="before")
+    @classmethod
+    def validate_notebooks_path(cls, v: Any):
         if isinstance(v, str):
             return Path(v).expanduser()
         if isinstance(v, Path):
             return v.expanduser()
         return v
 
     def load_private_keys(self) -> set[str]:
@@ -58,28 +66,27 @@
             with path.open("r") as f:
                 keys.add(f.read())
         return keys
 
     def load_public_keys(self) -> set[str]:
         keys = set()
         for path in self.recipient_paths:
-            if isinstance(path, HttpUrl):
+            if isinstance(path, Url):
                 with httpx_cache.Client(cache=httpx_cache.FileCache()) as client:
                     response = client.get(str(path))
                 if response.status_code == httpx.codes.OK:
                     for line in response.content.decode().split("\n"):
                         if line:
                             keys.add(line)
             elif isinstance(path, Path):
                 with path.open("r") as f:
                     keys.add(f.read())
         return keys
 
-    class Config:
-        env_prefix = "halig_"
+    model_config = SettingsConfigDict(env_prefix="halig_")
 
 
 @lru_cache
 def load_from_file(file_path: Path | None = None) -> Settings:
     if file_path is None:
         halig_config_home = platformdirs.user_config_path("halig", ensure_exists=True)
         file_path = halig_config_home / "halig.yml"
```

### Comparing `halig-0.3.2/halig/utils.py` & `halig-0.4.0/halig/utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/pyproject.toml` & `halig-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 authors = [
     { name = "cătălin", email = "185504a9@duck.com" },
 ]
 requires-python = ">=3.10"
 dependencies = [
     "typer<1.0.0,>=0.6.1",
     "rich>=13.3.3",
-    "pydantic>=1.10.7",
+    "pydantic>=2.0.3",
     "pyyaml>=6.0",
-    "pyrage>=1.0.3",
+    "pyrage>=1.1.1",
     "pendulum>=2.1.2",
     "httpx>=0.24.0",
     "platformdirs>=3.5.1",
     "httpx-cache>=0.9.0",
+    "pydantic-settings>=2.0.2",
 ]
 name = "halig"
 dynamic = []
 description = "age-encrypted, file-based, note-taking CLI app"
 readme = "README.md"
 keywords = [
     "cli",
@@ -34,15 +35,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.3.2"
+version = "0.4.0"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
@@ -71,14 +72,17 @@
     "mypy>=1.1.1",
     "types-PyYAML>=6.0.12.9",
 ]
 docs = [
     "mkdocs-material>=9.1.5",
     "mkdocstrings[python]>=0.20.0",
 ]
+dev = [
+    "bump-pydantic>=0.6.0",
+]
 
 [tool.pdm.version]
 source = "file"
 path = "halig/__version__.py"
 
 [tool.pdm.build]
 excludes = [
```

### Comparing `halig-0.3.2/tests/commands/conftest.py` & `halig-0.4.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/commands/test_edit.py` & `halig-0.4.0/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/commands/test_import.py` & `halig-0.4.0/tests/commands/test_import.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/commands/test_notebooks.py` & `halig-0.4.0/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/commands/test_show.py` & `halig-0.4.0/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/conftest.py` & `halig-0.4.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 @pytest.fixture()
 def settings_file_path(halig_path: Path, notebooks_path: Path) -> Path:
     yaml_file = halig_path / "halig.yml"
     yaml_file.touch()
     s = Settings(notebooks_root_path=notebooks_path)
     # `.dict()` doesn't serialize some fields that yaml doesn't understand
-    serialized = json.loads(s.json())
+    serialized = json.loads(s.model_dump_json())
     with yaml_file.open("w") as f:
         yaml.safe_dump(serialized, f)
     return yaml_file
 
 
 @pytest.fixture()
 def empty_file_path(halig_path: Path) -> Path:
```

### Comparing `halig-0.3.2/tests/test_encryption.py` & `halig-0.4.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/tests/test_settings.py` & `halig-0.4.0/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def test_settings_from_env(settings: Settings, notebooks_root_path_envvar):
     from_env_settings = Settings()  # type: ignore[call-arg]
     assert from_env_settings.notebooks_root_path == settings.notebooks_root_path
 
 
 def test_settings_from_non_existing_file_raises_value_error():
-    with pytest.raises(ValueError, match="field required"):
+    with pytest.raises(ValueError, match="Field required"):
         Settings()  # type: ignore[call-arg]
 
 
 def test_load_from_file(notebooks_path: Path, settings_file_path: Path):
     settings = load_from_file(settings_file_path)
     assert settings.notebooks_root_path == notebooks_path
```

### Comparing `halig-0.3.2/tests/test_utils.py` & `halig-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.2/PKG-INFO` & `halig-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.3.2
+Version: 0.4.0
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -18,21 +18,22 @@
 Project-URL: Homepage, https://git.roboces.dev/catalin/halig
 Project-URL: Repository, https://git.roboces.dev/catalin/halig
 Project-URL: Documentation, https://git.roboces.dev/catalin/halig
 Project-URL: Changelog, https://git.roboces.dev/catalin/halig
 Requires-Python: >=3.10
 Requires-Dist: typer<1.0.0,>=0.6.1
 Requires-Dist: rich>=13.3.3
-Requires-Dist: pydantic>=1.10.7
+Requires-Dist: pydantic>=2.0.3
 Requires-Dist: pyyaml>=6.0
-Requires-Dist: pyrage>=1.0.3
+Requires-Dist: pyrage>=1.1.1
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: platformdirs>=3.5.1
 Requires-Dist: httpx-cache>=0.9.0
+Requires-Dist: pydantic-settings>=2.0.2
 Requires-Dist: pytest>=7.2.2; extra == "testing"
 Requires-Dist: pytest-cov>=4.0.0; extra == "testing"
 Requires-Dist: pyfakefs>=5.1.0; extra == "testing"
 Requires-Dist: pytest-clarity>=1.0.1; extra == "testing"
 Requires-Dist: pytest-reportlog>=0.2.1; extra == "testing"
 Requires-Dist: pytest-duration-insights>=0.1.1; extra == "testing"
 Requires-Dist: pytest-pretty>=1.1.1; extra == "testing"
@@ -41,17 +42,19 @@
 Requires-Dist: black>=23.3.0; extra == "linting"
 Requires-Dist: ruff>=0.0.260; extra == "linting"
 Requires-Dist: pyright>=1.1.301; extra == "linting"
 Requires-Dist: mypy>=1.1.1; extra == "linting"
 Requires-Dist: types-PyYAML>=6.0.12.9; extra == "linting"
 Requires-Dist: mkdocs-material>=9.1.5; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.20.0; extra == "docs"
+Requires-Dist: bump-pydantic>=0.6.0; extra == "dev"
 Provides-Extra: testing
 Provides-Extra: linting
 Provides-Extra: docs
+Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # halig
 
 ![PyPI](https://img.shields.io/pypi/v/halig?logo=python)
 ![PyPI - License](https://img.shields.io/pypi/l/halig)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/halig)
@@ -66,15 +69,15 @@
 
 ## Features
 
 - Simple notebooks management with paths autocompletion
 - Passphrase-less, fully-encrypted notes, compatible with existing SSH keys 
 - No external `age` binary needed
 - Almost all `age` advantages, like having multiple keys for encryption and decryption
-- Remote (HTTP) public keys import: e.g: github.com/<username>.keys
+- Remote (HTTP) public keys import: e.g: github.com/\<username\>.keys
 
 ## Install
 
 ```shell
 pipx install halig # or pip
 ```
```

