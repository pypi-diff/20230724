# Comparing `tmp/auto-pr-1.0.2.tar.gz` & `tmp/auto_pr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-pr-1.0.2.tar", max compression
+gzip compressed data, was "auto_pr-1.0.3.tar", max compression
```

## Comparing `auto-pr-1.0.2.tar` & `auto_pr-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2021-08-26 11:04:40.759990 auto-pr-1.0.2/LICENSE
--rw-r--r--   0        0        0     4455 2021-08-26 11:04:40.759990 auto-pr-1.0.2/README.md
--rw-r--r--   0        0        0     9033 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/__init__.py
--rw-r--r--   0        0        0       63 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/__main__.py
--rw-r--r--   0        0        0     1571 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/config.py
--rw-r--r--   0        0        0     2139 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/database.py
--rw-r--r--   0        0        0     5176 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/github.py
--rw-r--r--   0        0        0     9068 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/repo.py
--rw-r--r--   0        0        0      451 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/util.py
--rw-r--r--   0        0        0     3368 2021-08-26 11:04:40.759990 auto-pr-1.0.2/autopr/workdir.py
--rw-r--r--   0        0        0      792 2021-08-26 11:04:40.759990 auto-pr-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5433 2021-08-26 11:05:15.131256 auto-pr-1.0.2/setup.py
--rw-r--r--   0        0        0     5219 2021-08-26 11:05:15.131787 auto-pr-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 12:21:10.647512 auto_pr-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4455 2023-07-24 12:21:10.647512 auto_pr-1.0.3/README.md
+-rw-r--r--   0        0        0     9033 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/__main__.py
+-rw-r--r--   0        0        0     1571 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/config.py
+-rw-r--r--   0        0        0     2139 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/database.py
+-rw-r--r--   0        0        0     5176 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/github.py
+-rw-r--r--   0        0        0     9068 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/repo.py
+-rw-r--r--   0        0        0      451 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/util.py
+-rw-r--r--   0        0        0     3368 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/workdir.py
+-rw-r--r--   0        0        0      792 2023-07-24 12:21:10.647512 auto_pr-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 auto_pr-1.0.3/setup.py
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 auto_pr-1.0.3/PKG-INFO
```

### Comparing `auto-pr-1.0.2/LICENSE` & `auto_pr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/README.md` & `auto_pr-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/__init__.py` & `auto_pr-1.0.3/autopr/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/config.py` & `auto_pr-1.0.3/autopr/config.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/database.py` & `auto_pr-1.0.3/autopr/database.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/github.py` & `auto_pr-1.0.3/autopr/github.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/repo.py` & `auto_pr-1.0.3/autopr/repo.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/autopr/workdir.py` & `auto_pr-1.0.3/autopr/workdir.py`

 * *Files identical despite different names*

### Comparing `auto-pr-1.0.2/pyproject.toml` & `auto_pr-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-pr"
-version = "1.0.2"
+version = "1.0.3"
 description = "Perform bulk updates across repositories"
 license = "Apache-2.0"
 
 authors = ["GetYourGuide GmbH"]
 
 readme = "README.md"
 repository = "https://github.com/getyourguide/auto-pr"
@@ -18,15 +18,15 @@
 auto-pr = "autopr:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 marshmallow = "3.13.0"
 marshmallow-dataclass = "8.5.3"
 click = "8.0.1"
-PyYAML = "5.4.1"
+PyYAML = "6.0.1"
 PyGithub = "1.55"
 single-source = "0.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-socket = "*"
 setuptools = "*"
```

### Comparing `auto-pr-1.0.2/setup.py` & `auto_pr-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 ['autopr']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyGithub==1.55',
- 'PyYAML==5.4.1',
+ 'PyYAML==6.0.1',
  'click==8.0.1',
  'marshmallow-dataclass==8.5.3',
  'marshmallow==3.13.0',
  'single-source==0.2.0']
 
 entry_points = \
 {'console_scripts': ['auto-pr = autopr:main']}
 
 setup_kwargs = {
     'name': 'auto-pr',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Perform bulk updates across repositories',
     'long_description': '<img width="128" src="https://github.com/getyourguide/auto-pr/raw/master/img/logo.svg" alt="auto-pr logo" />\n\n![CI](https://github.com/getyourguide/auto-pr/workflows/CI/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=getyourguide/auto-pr&amp;utm_campaign=Badge_Grade)\n[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&utm_medium=referral&utm_content=getyourguide/auto-pr&utm_campaign=Badge_Coverage)\n[![PyPI version](https://badge.fury.io/py/auto-pr.svg)](https://badge.fury.io/py/auto-pr)\n![PyPI downloads](https://img.shields.io/pypi/dm/auto-pr)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# auto-pr\n\nA command line tool to perform bulk updates across multiple GitHub repositories.\n\n## How to install\n\nWith [pipx](https://pipxproject.github.io/pipx/) (recommended):\n\n```bash\npipx install auto-pr\n```\nWith pip:\n\n```bash\npip install auto-pr\n```\n\n## Usage\n\n[![Usage](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)\n\n### Init\n\nFirst initialise the project directory by running the `init` command within an empty directory.\n\n```bash\nauto-pr init --api-key=<github_token> --ssh-key-file=<path-to-ssh-key>\n```\n\nWhere `<github_token>` is a GitHub [personal access token](https://github.com/settings/tokens) which has `repo` and `user:user:email` scope.\n\nNext modify the generated `config.yaml` file with your desired configurations.\n\n```yaml\ncredentials:\n  api_key: <github_token>\n  ssh_key_file: /path/to/ssh/key/to/push/.ssh/id_rsa\npr:\n  body: >\n    Body of the PR that will be generated\n\n    Can be multi-line :)\n  branch: auto-pr # The branch name to use when making changes\n  message: Replace default pipelines with modules # Commit message\n  title: \'My awesome change\' # Title of the PR\nrepositories: # Rules that define what repos to update\n  - mode: add\n    match_owner: <org/user>\nupdate_command:\n  - touch\n  - my-file\n```\n\n### Repositories\n\nYou can define the list of repositories to pull and build into the database to update using a list of rules.\n\n-   `mode` - either `add` or `remove` - used to either match or negate\n-   `public` (optional) - pull only public or private, leave out for both\n-   `archived` (optional) -  archived or non-archived, leave out for both\n-   `match_owner` (optional) - the owner or user to pull\n-   `match_name` (optional) - a list of regular expressions to match against to pull\n\nThe flags of the filter rules are optional not specifying will run the command on all repositories that the token has access too.\n\n### Update Command\n\nThis is the list containing the command to be executed along with the arguments passed to it. It will be executed from\nthe root of each repository that is processed.\n\nIf an error occurs during the execution it will be displayed in the output but will not halt the execution.\n\nSee [example commands](docs/examples.md#commands)\n\n### Pull\n\nAfter you have configured the project you can now pull the repositories down that match your rules.\n\n```bash\nauto-pr pull\n```\n\nThis will generate a `db.json` file within your workdir containing a list of mapped repositories and their state.\n\nThis command can be run multiple times, if there are new matching repositories found they will be merged into the existing database.\n\n### Test\n\nOnce the `pull` command has finished setting up the work directory you can now run test to check what the changes that will be made by the script will yield.\n\n### Run\n\nWhen you\'re confident with the changes output from the `test` command you can finally execute `run`.\n\n```bash\nauto-pr run\n```\n\nThis will perform the changes to a branch on the locally cloned repository and push the branch upstream with the information you provided within `config.yaml`.\n\nSee `--help` for more information about other commands and their  usage.\n\n## Security\n\nFor sensitive security matters please contact [security@getyourguide.com](mailto:security@getyourguide.com).\n\n## Legal\n\nCopyright 2021 GetYourGuide GmbH.\n\nauto-pr is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for the full text.\n',
     'author': 'GetYourGuide GmbH',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/getyourguide/auto-pr',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `auto-pr-1.0.2/PKG-INFO` & `auto_pr-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: auto-pr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Perform bulk updates across repositories
 Home-page: https://github.com/getyourguide/auto-pr
 License: Apache-2.0
 Author: GetYourGuide GmbH
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.55)
-Requires-Dist: PyYAML (==5.4.1)
+Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: click (==8.0.1)
 Requires-Dist: marshmallow (==3.13.0)
 Requires-Dist: marshmallow-dataclass (==8.5.3)
 Requires-Dist: single-source (==0.2.0)
 Project-URL: Repository, https://github.com/getyourguide/auto-pr
 Description-Content-Type: text/markdown
```

