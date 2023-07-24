# Comparing `tmp/github_actions_cli-1.0.0b2.tar.gz` & `tmp/github_actions_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_actions_cli-1.0.0b2.tar", max compression
+gzip compressed data, was "github_actions_cli-1.0.1.tar", max compression
```

## Comparing `github_actions_cli-1.0.0b2.tar` & `github_actions_cli-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1500 2023-07-22 16:14:30.465697 github_actions_cli-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     2016 2023-07-22 16:30:30.348267 github_actions_cli-1.0.0b2/README.md
--rw-r--r--   0        0        0        0 2023-07-22 19:45:14.822523 github_actions_cli-1.0.0b2/gha_cli/__init__.py
--rwxr-xr-x   0        0        0     5413 2023-07-22 19:40:09.586657 github_actions_cli-1.0.0b2/gha_cli/cli.py
--rw-r--r--   0        0        0     1513 2023-07-22 19:54:41.913866 github_actions_cli-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 github_actions_cli-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-07-24 14:05:26.171784 github_actions_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3113 2023-07-24 14:05:26.171784 github_actions_cli-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 14:05:26.171784 github_actions_cli-1.0.1/gha_cli/__init__.py
+-rwxr-xr-x   0        0        0     8638 2023-07-24 14:05:26.171784 github_actions_cli-1.0.1/gha_cli/cli.py
+-rw-r--r--   0        0        0     1538 2023-07-24 14:05:26.171784 github_actions_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 github_actions_cli-1.0.1/PKG-INFO
```

### Comparing `github_actions_cli-1.0.0b2/LICENSE` & `github_actions_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `github_actions_cli-1.0.0b2/README.md` & `github_actions_cli-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,109 @@
 GitHub Actions CLI
 ====================
 
 The purpose of this tool is to work with your GitHub Actions workflows in your repositories.
 It is complementary to the GitHub CLI.
 
-So far, three main flows are supported:
+# Basic usage
 
-# List all workflows path and name in a specified repository.
+Run `github-actions-cli` within a directory which has a clone of a GitHub repository.
+The tool will list the GitHub actions workflows, the actions they use, the current versions they use, and the latest
+versions of the actions.
+
+```text
+./.github/workflows/test.yml:
+	actions/checkout                  v3 ==> v3.5.3
+	release-drafter/release-drafter    v5 ==> v5.24.0
+	actions/setup-python              v4 ==> v4.7.0
+./.github/workflows/publish.yml:
+	pypa/gh-action-pypi-publish    release/v1 ==> v1.8.8
+	actions/checkout                  v3 ==> v3.5.3
+	actions/setup-python              v4 ==> v4.7.0
+```
+
+# Supported use cases
+
+```text
+Usage: github-actions-cli [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -repo TEXT           Repository to analyze, can be a local directory or a
+                       {OWNER}/{REPO} format  [default: .]
+  --github-token TEXT  GitHub token to use, by default will use GITHUB_TOKEN
+                       environment variable
+  --help               Show this message and exit.
+
+Commands:
+  list-actions    List actions in a workflow
+  list-workflows  List workflows in repository
+  update-actions  Show actions required updates in repository workflows
+```
+
+## `update-actions` List all actions that are out of date in a repository (Default)
+
+List the latest versions of actions used in a repository workflows
+and potentially update the workflow files.
+
+For example, running `github-actions-cli` without any parameters will look for workflows in the
+current directory (`.`), check whether there are updates required for the actions in the workflows
+it finds.
+
+Another example, running on a remote repository, `github-actions-cli -repo cunla/fakeredis update-actions -u`,
+will look for the latest versions of the actions used in the repository cunla/fakeredis, and because of the `-u`
+flag, it will create a commit updating the workflows to the latest.
+
+> Note:
+> Having `GITHUB_TOKEN` with permissions to make commits on the repository
+> is required in order to write to repository.
+
+Parameters:
+
+```text
+Usage: cli.py update-actions [OPTIONS]
+
+  Show actions required updates in repository workflows
+
+Options:
+  -u, --update      Do not update, list only
+  -commit-msg TEXT  Commit msg, only relevant when remote repo
+```
+
+## `list-workflows` List all workflows path and name in a specified repository.
 
 Example:
 
 ```shell
-python ghautils.py cunla/fakeredis list-workflows
+github-actions-cli -repo cunla/fakeredis list-workflows
 ```
+
 will return:
 
 ```text
-.github/workflows/publish.yml:Upload Python Package
-.github/workflows/test.yml:Unit tests
-dynamic/github-code-scanning/codeql:CodeQL
-dynamic/pages/pages-build-deployment:pages-build-deployment
+.github/workflows/publish.yml
+.github/workflows/test.yml
 ```
 
-# List all actions `uses` in a workflow
+## `list-actions` List all actions `uses` in a workflow
 
 Given a repo and a workflow path, return all actions in the workflow.
 
 Example:
+
 ```shell
-python ghautils.py cunla/fakeredis list-actions .github/workflows/publish.yml
+github-actions-cli -repo cunla/fakeredis list-actions .github/workflows/test.yml
 ```
 
 Result
+
 ```text
-pypa/gh-action-pypi-publish@release/v1
 actions/checkout@v3
+./.github/actions/test-coverage
+release-drafter/release-drafter@v5
 actions/setup-python@v4
 ```
 
-# Update all actions in a repository workflow(s)
-Show the latest versions of actions used in a repository workflow.
+# Installation
 
-Example:
 ```shell
-python ghautils.py cunla/fakeredis update
+pip install github-actions-cli
 ```
-Result:
-```text
-.github/workflows/publish.yml
-  actions/setup-python @ v4     ==> v4.7.0
-  pypa/gh-action-pypi-publish @ release/v1      ==> v1.8.8
-  actions/checkout @ v3         ==> v3.5.3
-.github/workflows/test.yml
-  actions/setup-python @ v4     ==> v4.7.0
-  release-drafter/release-drafter @ v5  ==> v5.24.0
-  actions/checkout @ v3         ==> v3.5.3
-```
-
-# Help messages
-
-```text
-usage: ghautils.py [-h] [--github-token GITHUB_TOKEN] repo {list-workflows,list-actions,update} ...
-
-positional arguments:
-  repo                  Repository to analyze
-  {list-workflows,list-actions,update}
-    list-workflows      List github workflows
-    list-actions        List actions in a workflow
-    update              Update actions in github workflows
-
-options:
-  -h, --help            show this help message and exit
-  --github-token GITHUB_TOKEN
-                        GitHub token to use, by default will use GITHUB_TOKEN environment variable
-```
```

### Comparing `github_actions_cli-1.0.0b2/pyproject.toml` & `github_actions_cli-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-github-actions-cli = "gha_cli.cli:run"
+github-actions-cli = "gha_cli.cli:cli"
 
 [tool.poetry]
 name = "github-actions-cli"
-version = "1.0.0b2"
+version = "1.0.1"
 description = "GitHub Actions CLI - allows updating workflows, etc."
 readme = "README.md"
 keywords = ["GitHub Actions", "CLI"]
 packages = [
     { include = "gha_cli" },
 ]
 
@@ -40,21 +40,23 @@
 "Bug Tracker" = "https://github.com/dsoftwareinc/github-actions-cli/issues"
 "Funding" = "https://github.com/sponsors/cunla"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pygithub = "^1.59"
 pyyaml = "^6.0"
+click = "^8.1"
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.5"
 Flake8-pyproject = "^1.2"
 
 [tool.flake8]
 max-line-length = 119
 exclude = [
     ".git",
     ".github",
     "__pycache__",
     "dist",
     "venv",
+    ".venv"
 ]
```

