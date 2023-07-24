# Comparing `tmp/slack-logger-python-0.1.1.tar.gz` & `tmp/slack-logger-python-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-logger-python-0.1.1.tar", last modified: Sun Jul 23 01:00:13 2023, max compression
+gzip compressed data, was "slack-logger-python-0.2.8.tar", last modified: Mon Jul 24 15:20:20 2023, max compression
```

## Comparing `slack-logger-python-0.1.1.tar` & `slack-logger-python-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.627708 slack-logger-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.623708 slack-logger-python-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.623708 slack-logger-python-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.github/workflows/tagging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.623708 slack-logger-python-0.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-23 01:00:13.627708 slack-logger-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 01:00:13.627708 slack-logger-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.623708 slack-logger-python-0.1.1/slack_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/slack_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/slack_logger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.627708 slack-logger-python-0.1.1/slack_logger_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-23 01:00:13.000000 slack-logger-python-0.1.1/slack_logger_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-23 01:00:13.000000 slack-logger-python-0.1.1/slack_logger_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 01:00:13.000000 slack-logger-python-0.1.1/slack_logger_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 01:00:13.000000 slack-logger-python-0.1.1/slack_logger_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-23 01:00:13.000000 slack-logger-python-0.1.1/slack_logger_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:13.627708 slack-logger-python-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-23 01:00:03.000000 slack-logger-python-0.1.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.576969 slack-logger-python-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/tagging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 15:20:09.000000 slack-logger-python-0.2.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/slack_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/slack_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/slack_logger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/slack_logger_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/tests/test_basic.py
```

### Comparing `slack-logger-python-0.1.1/.github/workflows/deploy.yml` & `slack-logger-python-0.2.8/.github/workflows/deploy.yml`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     tags: [ v* ]
   pull_request:
     types: [ opened, synchronize ]
   workflow_dispatch:
 
 
 permissions:
-  contents: read
+  contents: write
   id-token: write
 
 env:
   REGISTRY: ghcr.io
   REPOSITORY: ${{ github.repository }} # <owner/repo>
   MODULE_NAME: slack_logger
   VERSION: ${{ github.ref_type == 'tag' && github.ref_name || github.event.pull_request.head.sha || github.sha  }}
@@ -67,14 +67,49 @@
           set -o pipefail
           mypy ${{env.MODULE_NAME}} tests
 
       - name: pytest | Run Tests
         run: |
           pytest
 
+      - name: Gather Badge Data
+        if: github.ref_name == 'main' && github.event_name == 'push'
+        run: |
+          coverage run -m pytest -s
+          coverage report -m
+
+      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9 # pin@v3
+        if: always() && github.ref_name == 'main' && github.event_name == 'push'
+        with:
+          ref: assets
+          path: assets
+
+      - name: Create Badge Directory
+        if: github.ref_name == 'main' && github.event_name == 'push'
+        run: mkdir -p assets/badges
+
+      - name: Create Coverage Badge
+        if: github.ref_name == 'main' && github.event_name == 'push'
+        uses: tj-actions/coverage-badge-py@782bdaaa8b2e37612e6b6fac5e559e5544e6eef2 # pin@v2
+        with:
+          output: assets/badges/coverage.svg
+
+      - name: Commit Badge
+        if: github.ref_name == 'main' && github.event_name == 'push'
+        run: |
+          cd assets
+          if [[ -n "$(git status --porcelain)" ]]; then
+            git config --local user.email "action@github.com"
+            git config --local user.name "GitHub Action"
+            git add badges/coverage.svg
+            git commit -m "Update coverage badge"
+            git push
+          fi
+
+
   deploy:
     name: "Deploy"
     runs-on: ubuntu-latest
     timeout-minutes: 15
     if: github.ref_type == 'tag'
     environment: 'prod'
     needs:
@@ -91,12 +126,16 @@
         with:
           python-version: "3.10"
           cache: "pip"
 
       - name: pip | Install Dependencies
         run: pip install build
 
+      - name: Get Version
+        run: |
+          echo "${VERSION:1}" > VERSION
+
       - name: Build
         run: python -m build
 
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@f8c70e705ffc13c3b4d1221169b84f12a75d6ca8 # pin@release/v1
```

### Comparing `slack-logger-python-0.1.1/.github/workflows/format.yml` & `slack-logger-python-0.2.8/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.1.1/.github/workflows/tagging.yml` & `slack-logger-python-0.2.8/.github/workflows/tagging.yml`

 * *Files 9% similar despite different names*

```diff
@@ -4,45 +4,48 @@
   schedule:
     - cron: '0 0 * * *' # Everyday at midnight
   pull_request:
     types: [ closed ]
 
 permissions:
   id-token: write
-  contents: read
+  contents: write
 
 jobs:
   tagging:
     name: "Version Tag"
     if: github.event.action != 'closed' || (github.event.pull_request.merged && contains(github.event.pull_request.labels.*.name, 'bump-version-after-merge'))
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9 # pin@v3
-        with:
-          ref: ${{ github.event.pull_request.head.sha }}
-
       - name: Generate github token
         id: generate-token
         uses: tibdex/github-app-token@b62528385c34dbc9f38e5f4225ac829252d1ea92 # pin@v1
         with:
           app_id: ${{ secrets.GH_APP_ID }}
           private_key: ${{ secrets.GH_PRIVATE_KEY }}
 
+      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9 # pin@v3
+        with:
+          ref: ${{ github.event.pull_request.head.sha }}
+          token: ${{ steps.generate-token.outputs.token }}
+
       - name: Bump version and push tag
         id: tagging
         uses: mathieudutour/github-tag-action@fcfbdceb3093f6d85a3b194740f8c6cec632f4e2 # pin@v6.1
         with:
           github_token: ${{ steps.generate-token.outputs.token }}
           release_branches: 'main'
-          default_bump: false
+          default_bump: ${{ github.event_name == 'workflow_dispatch' && 'patch' || false}}
+
+      - name: Update version file
+        if: steps.tagging.outputs.new_version && steps.tagging.outputs.new_version != 'undefined'
+        run: echo "${{ steps.tagging.outputs.new_version }}" > VERSION
 
       - name: Create a GitHub release
         uses: ncipollo/release-action@a2e71bdd4e7dab70ca26a852f29600c98b33153e # pin@v1
         if: steps.tagging.outputs.new_version && steps.tagging.outputs.new_version != 'undefined'
         with:
           tag: ${{ steps.tagging.outputs.new_tag }}
           name: Release ${{ steps.tagging.outputs.new_tag }}
           body: ${{ steps.tagging.outputs.changelog }}
+          token: ${{ steps.generate-token.outputs.token }}
 
-      - name: Update version file
-        if: steps.tagging.outputs.new_version && steps.tagging.outputs.new_version != 'undefined'
-        run: echo "${{ steps.tagging.outputs.new_version }}" > VERSION
```

### Comparing `slack-logger-python-0.1.1/.gitignore` & `slack-logger-python-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.1.1/LICENSE` & `slack-logger-python-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.1.1/PKG-INFO` & `slack-logger-python-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.1.1
+Version: 0.2.8
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Slack Python Logging
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+![coverage](/../assets/badges/coverage.svg)
 
 Slack logger implementing the python logging interface to be used with the standard logging tools in python.
 
 A handler and a formatter is provided, currently working with a webhook url only.
 
 Messages are fully customizable using slacks block layout, see [Creating rich message layouts](https://api.slack.com/messaging/composing/layouts) and [Reference: Layout blocks](https://api.slack.com/reference/block-kit/blocks).
```

### Comparing `slack-logger-python-0.1.1/README.md` & `slack-logger-python-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Slack Python Logging
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+![coverage](/../assets/badges/coverage.svg)
 
 Slack logger implementing the python logging interface to be used with the standard logging tools in python.
 
 A handler and a formatter is provided, currently working with a webhook url only.
 
 Messages are fully customizable using slacks block layout, see [Creating rich message layouts](https://api.slack.com/messaging/composing/layouts) and [Reference: Layout blocks](https://api.slack.com/reference/block-kit/blocks).
```

### Comparing `slack-logger-python-0.1.1/pyproject.toml` & `slack-logger-python-0.2.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -128,7 +128,12 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra --capture=tee-sys"
 log_cli = true
 testpaths = [
     "tests",
 ]
+
+[tool.coverage.run]
+source = [
+    "slack_logger"
+]
```

### Comparing `slack-logger-python-0.1.1/shell.nix` & `slack-logger-python-0.2.8/shell.nix`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.1.1/slack_logger/__init__.py` & `slack-logger-python-0.2.8/slack_logger/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import json
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from logging import LogRecord
-from typing import Any, Dict, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Union
 
 from attrs import define
 from slack_sdk.models.attachments import Attachment
-from slack_sdk.models.blocks import Block, DividerBlock, HeaderBlock, SectionBlock
+from slack_sdk.models.blocks import Block, ContextBlock, DividerBlock, HeaderBlock, SectionBlock
 from slack_sdk.models.blocks.basic_components import MarkdownTextObject, PlainTextObject
 from slack_sdk.webhook.async_client import AsyncWebhookClient
 from slack_sdk.webhook.webhook_response import WebhookResponse
 
 log = logging.getLogger("slack_logger")
 log.setLevel(logging.DEBUG)
 
@@ -29,24 +29,70 @@
 }
 
 
 @define
 class Configuration:
     service: Optional[str] = None
     environment: Optional[str] = None
+    context: List[str] = []
     emojis: Dict[int, str] = DEFAULT_EMOJIS
     extra_fields: Dict[str, str] = {}
 
 
 @define
 class MessageDesign(ABC):
     @abstractmethod
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         pass
 
+    def get_env(self, config: Configuration, record: LogRecord) -> Optional[str]:
+        dynamic_env: Optional[str] = getattr(record, "environment", None)
+        if dynamic_env is not None:
+            return dynamic_env
+        if config.environment is not None:
+            return config.environment
+        return None
+
+    def get_service(self, config: Configuration, record: LogRecord) -> Optional[str]:
+        dynamic_service: Optional[str] = getattr(record, "service", None)
+        if dynamic_service is not None:
+            return dynamic_service
+        if config.service is not None:
+            return config.service
+        return None
+
+    def construct_header(
+        self, record: LogRecord, config: Configuration, icon: Optional[str], level: str
+    ) -> HeaderBlock:
+        service: Optional[str] = self.get_service(config=config, record=record)
+        header_msg: str
+        if icon is not None:
+            header_msg = f"{icon} "
+        header_msg += level
+        if config.service is not None:
+            header_msg += f" | {service}"
+        else:
+            header_msg += f" | {record.name}"
+
+        return HeaderBlock(text=PlainTextObject(text=header_msg))
+
+    def construct_context(
+        self, config: Configuration, env: Optional[str], service: Optional[str]
+    ) -> Optional[ContextBlock]:
+        if config.context != []:
+            context_msg = ", ".join(config.context)
+            return ContextBlock(elements=[MarkdownTextObject(text=context_msg)])
+        elif env is not None and service is not None:
+            return ContextBlock(elements=[MarkdownTextObject(text=f":point_right: {env}, {service}")])
+        elif env is None:
+            return ContextBlock(elements=[MarkdownTextObject(text=f":point_right: {env}")])
+        elif service is None:
+            return ContextBlock(elements=[MarkdownTextObject(text=f":point_right: {service}")])
+        return None
+
     def format(self, record: LogRecord) -> str:
         maybe_blocks: Sequence[Optional[Block]] = self.format_blocks(record=record)
         blocks: Sequence[Block] = [b for b in maybe_blocks if b is not None]
         str_blocks: str = json.dumps(list(map(lambda block: block.to_dict(), blocks)))
         log.debug(f"str_blocks: {str_blocks}")
         return str_blocks
 
@@ -62,19 +108,15 @@
     config: Configuration
 
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         level = record.levelname
         message = record.getMessage()
         icon = self.config.emojis.get(record.levelno)
 
-        header: HeaderBlock
-        if icon is not None:
-            header = HeaderBlock(text=PlainTextObject(text=f"{icon} {level} | {self.config.service}"))
-        else:
-            header = HeaderBlock(text=PlainTextObject(text=f"{level} | {self.config.service}"))
+        header: HeaderBlock = self.construct_header(record=record, config=self.config, icon=icon, level=level)
 
         body = SectionBlock(text=MarkdownTextObject(text=message))
         default_blocks: Sequence[Block] = [
             header,
             body,
         ]
 
@@ -86,39 +128,36 @@
     config: Configuration
 
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         level = record.levelname
         message = record.getMessage()
         icon = self.config.emojis.get(record.levelno)
 
-        dynamic_extra_fields = getattr(record, "extra_fields", {})
-        all_extra_fields = {**self.config.extra_fields, **dynamic_extra_fields}
-
-        header: HeaderBlock
-        if icon is not None:
-            header = HeaderBlock(text=PlainTextObject(text=f"{icon} {level} | {self.config.service}"))
-        else:
-            header = HeaderBlock(text=PlainTextObject(text=f"{level} | {self.config.service}"))
+        env: Optional[str] = self.get_env(config=self.config, record=record)
+        service: Optional[str] = self.get_service(config=self.config, record=record)
 
+        header: HeaderBlock = self.construct_header(record=record, config=self.config, icon=icon, level=level)
+        context: Optional[ContextBlock] = self.construct_context(config=self.config, env=env, service=service)
         body = SectionBlock(text=MarkdownTextObject(text=message))
 
         error: Optional[SectionBlock] = None
         if record.exc_info is not None:
             error = SectionBlock(text=MarkdownTextObject(text=f"```{record.exc_text}```"))
 
-        fields = SectionBlock(
-            fields=[
-                MarkdownTextObject(text=f"*Environment*\n{self.config.environment}"),
-                MarkdownTextObject(text=f"*Service*\n{self.config.service}"),
-            ]
-            + [MarkdownTextObject(text=f"*{key}*\n{value}") for key, value in all_extra_fields.items()]
-        )
+        dynamic_extra_fields = getattr(record, "extra_fields", {})
+        all_extra_fields = {**self.config.extra_fields, **dynamic_extra_fields}
+        fields: Optional[SectionBlock] = None
+        if all_extra_fields != {}:
+            fields = SectionBlock(
+                fields=[MarkdownTextObject(text=f"*{key}*\n{value}") for key, value in all_extra_fields.items()]
+            )
 
         maybe_blocks: Sequence[Optional[Block]] = [
             header,
+            context,
             DividerBlock(),
             body,
             error,
             DividerBlock(),
             fields,
         ]
 
@@ -143,21 +182,18 @@
         return cls(design=MinimalDesign(config), config=config)
 
     @classmethod
     def default(cls, config: Configuration) -> "SlackFormatter":
         return cls(design=RichDesign(config), config=config)
 
     def format(self, record: LogRecord) -> str:
+        super().format(record)
         return self.design.format(record)
 
 
-# show = True:  log the values in the configuration
-# show = False: hide the values in the configuration
-# Injection filter
-# https://docs.python.org/3/howto/logging-cookbook.html#using-filters-to-impart-contextual-information
 class FilterType(Enum):
     AnyWhitelist = "AnyWhitelist"
     AllWhitelist = "AllWhitelist"
     AnyBlacklist = "AnyBlacklist"
     AllBlacklist = "AllBlacklist"
 
 
@@ -215,17 +251,14 @@
             service=log_filters.get("service", None),
             environment=log_filters.get("environment", None),
             extra_fields=log_filters.get("extra_fields", {}),
         )
         return self.filterConfig(serviceConfig=rconfig, record=record)
 
 
-# class ConfigFilter(SlackFilter):
-
-
 @define
 class DummyClient(AsyncWebhookClient):
     url: str = ""
 
     async def send(
         self,
         *,
@@ -248,15 +281,15 @@
                 assert isinstance(block, Block)
                 res.append(block.to_dict())
             t = json.dumps({"blocks": res})
         else:
             t = json.dumps({"text": str(text)})
 
         log.info(t)
-        return WebhookResponse(url="", status_code=200, body=t, headers={})
+        return WebhookResponse(url="", status_code=200, body="ok", headers={})
 
 
 class SlackHandler(logging.Handler):
     client: AsyncWebhookClient
 
     def __init__(self, client: AsyncWebhookClient):
         super(SlackHandler, self).__init__()
@@ -269,42 +302,34 @@
         )
 
     @classmethod
     def dummy(cls) -> "SlackHandler":
         return cls(client=DummyClient())
 
     async def send_text_via_webhook(self, text: str) -> str:
-        log.debug(text)
-        response = await self.client.send(text=text)  # type: ignore
+        response = await self.client.send(text=text)
         assert response.status_code == 200
-        # assert response.body == "ok"
+        assert response.body == "ok"
         return str(response.body)
 
     async def send_blocks_via_webhook(self, blocks: str) -> str:
-        # parsed_blocks = json.loads(blocks)
         block_seq = Block.parse_all(json.loads(blocks))
         response = await self.client.send(blocks=block_seq)
         assert response.status_code == 200
-        # assert response.body == "ok"
+        assert response.body == "ok"
         return str(response.body)
 
     def emit(self, record: LogRecord) -> None:
         try:
+            formatted_message = self.format(record)
             if isinstance(self.formatter, SlackFormatter):
-                formatted_message = self.format(record)
-                log.debug(f"formatted_message: {formatted_message}")
                 asyncio.run(self.send_blocks_via_webhook(blocks=formatted_message))
             else:
-                formatted_message = self.format(record)
-                log.debug(f"formatted_message: {formatted_message}")
                 asyncio.run(self.send_text_via_webhook(text=formatted_message))
 
-            # log.debug(f"format: {format}")
-            # asyncio.run(self.send_message_via_webhook(message=formatted_message))
-            # asyncio.run(self.send_blocks_via_webhook(blocks=formatted_message))
         except Exception:
             self.handleError(record)
 
     def handle(self, record: LogRecord) -> bool:
         # This pre-filters the messages with the Slack Filters
         if isinstance(self.formatter, SlackFormatter) and self.formatter.config is not None:
             format_config: Configuration = self.formatter.config
```

### Comparing `slack-logger-python-0.1.1/slack_logger_python.egg-info/PKG-INFO` & `slack-logger-python-0.2.8/slack_logger_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.1.1
+Version: 0.2.8
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Slack Python Logging
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+![coverage](/../assets/badges/coverage.svg)
 
 Slack logger implementing the python logging interface to be used with the standard logging tools in python.
 
 A handler and a formatter is provided, currently working with a webhook url only.
 
 Messages are fully customizable using slacks block layout, see [Creating rich message layouts](https://api.slack.com/messaging/composing/layouts) and [Reference: Layout blocks](https://api.slack.com/reference/block-kit/blocks).
```

### Comparing `slack-logger-python-0.1.1/slack_logger_python.egg-info/SOURCES.txt` & `slack-logger-python-0.2.8/slack_logger_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.1.1/tests/test_basic.py` & `slack-logger-python-0.2.8/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 
 import pytest
 
 from slack_logger import DEFAULT_EMOJIS, Configuration, FilterType, SlackFilter, SlackFormatter, SlackHandler
 
 logger = logging.getLogger("LocalTest")
 
-# Log to console as well
-stream_handler = logging.StreamHandler()
-stream_handler.setFormatter(logging.Formatter("%(asctime)s %(name)s|%(levelname)s: %(message)s"))
-logger.addHandler(stream_handler)
-
 # Setup test handler
 slack_handler = SlackHandler.dummy()
 slack_handler.setLevel(logging.WARN)
 logger.addHandler(slack_handler)
 
 
 # Check if only correct level is logged
@@ -165,16 +160,14 @@
 
     # Cleanup
     slack_handler.removeFilter(slackFilter10)
     assert len(slack_handler.filters) == 0
 
 
 DEFAULT_ADDITIONAL_FIELDS: Dict[str, Dict[str, str]] = {
-    "env": {"text": "*Environment*\ntest", "type": "mrkdwn"},
-    "service": {"text": "*Service*\ntestrunner", "type": "mrkdwn"},
     "foo": {"text": "*foo*\nbar", "type": "mrkdwn"},
     "raven": {"text": "*raven*\ncaw", "type": "mrkdwn"},
 }
 
 
 def default_msg(
     log_msg: str, levelno: int, additional_fields_dict: Dict[str, Dict[str, str]] = DEFAULT_ADDITIONAL_FIELDS
@@ -182,14 +175,15 @@
     additional_fields: List[Dict[str, str]] = list(additional_fields_dict.values())
     emoji = DEFAULT_EMOJIS.get(levelno)
     level_name = logging._levelToName.get(levelno)
     return json.dumps(
         {
             "blocks": [
                 {"text": {"text": f"{emoji} {level_name} | testrunner", "type": "plain_text"}, "type": "header"},
+                {"elements": [{"text": ":point_right: test, testrunner", "type": "mrkdwn"}], "type": "context"},
                 {"type": "divider"},
                 {
                     "text": {"text": log_msg, "type": "mrkdwn"},
                     "type": "section",
                 },
                 {"type": "divider"},
                 {
@@ -285,27 +279,27 @@
         slack_handler.setFormatter(None)
         caplog.clear()
 
         log_msg = "Error!"
         with pytest.raises(ZeroDivisionError):
             exception_logging(log_msg)
 
-        blocks_prefix = '{"blocks": [{"text": {"text": ":x: ERROR | testrunner", "type": "plain_text"}, "type": "header"}, {"type": "divider"}, {"text": {"text": "Error!", "type": "mrkdwn"}, "type": "section"}, {"text": {"text": "```Traceback (most recent call last):'
+        blocks_prefix = '{"blocks": [{"text": {"text": ":x: ERROR | testrunner", "type": "plain_text"}, "type": "header"}, {"elements": [{"text": ":point_right: test, testrunner", "type": "mrkdwn"}], "type": "context"}, {"type": "divider"}, {"text": {"text": "Error!", "type": "mrkdwn"}, "type": "section"}, {"text": {"text": "```Traceback (most recent call last):'
 
         assert any(map(lambda m: blocks_prefix in m, caplog.messages))
 
     def test_auto_exception_logging(self, caplog) -> None:  # type: ignore
         slack_handler.setFormatter(None)
         caplog.clear()
 
         log_msg = "Exception!"
         with pytest.raises(Exception):
             auto_exception_logging(log_msg)
 
-        blocks_prefix = '{"blocks": [{"text": {"text": ":x: ERROR | testrunner", "type": "plain_text"}, "type": "header"}, {"type": "divider"}, {"text": {"text": "Exception!", "type": "mrkdwn"}, "type": "section"}, {"text": {"text": "```Traceback (most recent call last):'
+        blocks_prefix = '{"blocks": [{"text": {"text": ":x: ERROR | testrunner", "type": "plain_text"}, "type": "header"}, {"elements": [{"text": ":point_right: test, testrunner", "type": "mrkdwn"}], "type": "context"}, {"type": "divider"}, {"text": {"text": "Exception!", "type": "mrkdwn"}, "type": "section"}, {"text": {"text": "```Traceback (most recent call last):'
 
         assert any(map(lambda m: blocks_prefix in m, caplog.messages))
 
     def test_filters(self, caplog) -> None:  # type: ignore
         slack_handler.setFormatter(None)
         caplog.clear()
```

