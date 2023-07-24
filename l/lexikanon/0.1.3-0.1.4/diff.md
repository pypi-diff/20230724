# Comparing `tmp/lexikanon-0.1.3.tar.gz` & `tmp/lexikanon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.1.3.tar", max compression
+gzip compressed data, was "lexikanon-0.1.4.tar", max compression
```

## Comparing `lexikanon-0.1.3.tar` & `lexikanon-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-26 10:16:01.950589 lexikanon-0.1.3/LICENSE
--rw-r--r--   0        0        0     3572 2023-04-26 10:16:01.950589 lexikanon-0.1.3/README.md
--rw-r--r--   0        0        0     2852 2023-04-26 10:16:28.279084 lexikanon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      890 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 10:16:28.223083 lexikanon-0.1.3/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      222 2023-04-26 10:16:28.223083 lexikanon-0.1.3/src/lexikanon/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/task/__init__.yaml
--rw-r--r--   0        0        0      195 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/py.typed
--rw-r--r--   0        0        0     4212 1970-01-01 00:00:00.000000 lexikanon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 07:39:52.669796 lexikanon-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2129 2023-07-24 07:39:52.669796 lexikanon-0.1.4/README.md
+-rw-r--r--   0        0        0     2881 2023-07-24 07:40:20.670040 lexikanon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      464 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 07:40:20.614040 lexikanon-0.1.4/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      195 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/py.typed
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 lexikanon-0.1.4/PKG-INFO
```

### Comparing `lexikanon-0.1.3/LICENSE` & `lexikanon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.3/pyproject.toml` & `lexikanon-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+click = "^8.1.3"
+hyfi = "^1.8.3"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
-black = "^23.1.0"
+black = ">=23.0.0,<=23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
@@ -70,30 +77,29 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/lexikanon/_version.py:__version__"
-version_pattern = 'src/lexikanon/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

