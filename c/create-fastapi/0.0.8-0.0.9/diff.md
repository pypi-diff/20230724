# Comparing `tmp/create_fastapi-0.0.8.tar.gz` & `tmp/create_fastapi-0.0.9.tar.gz`

## Comparing `create_fastapi-0.0.8.tar` & `create_fastapi-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/cli.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/ICommand.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/__init__.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/command_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/impl/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/impl/clone_git.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/impl/dependency_installer.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/commands/impl/dir_creator.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/helpers/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/cfa/helpers/logger.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/LICENSE
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/README.md
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 create_fastapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/cli.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/ICommand.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/command_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/impl/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/impl/dependency_installer.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/impl/dir_creator.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/commands/impl/git_clone.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/helpers/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/cfa/helpers/logger.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/README.md
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    16638 2020-02-02 00:00:00.000000 create_fastapi-0.0.9/PKG-INFO
```

### Comparing `create_fastapi-0.0.8/cfa/commands/command_builder.py` & `create_fastapi-0.0.9/cfa/commands/command_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 from cfa.commands.ICommand import ICommand
-from cfa.commands.impl.clone_git import GitClone
+from cfa.commands.impl.git_clone import GitClone
 from cfa.commands.impl.dependency_installer import DependencyInstaller
 from cfa.commands.impl.dir_creator import DirCreator
 
 
 class CommandBuilder:
     def __init__(self):
         self.commands: List[ICommand] = []
```

### Comparing `create_fastapi-0.0.8/cfa/commands/impl/clone_git.py` & `create_fastapi-0.0.9/cfa/commands/impl/git_clone.py`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.8/cfa/commands/impl/dependency_installer.py` & `create_fastapi-0.0.9/cfa/commands/impl/dependency_installer.py`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.8/.gitignore` & `create_fastapi-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.8/LICENSE` & `create_fastapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.8/pyproject.toml` & `create_fastapi-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "create-fastapi"
 description = "create-fastapi-app"
 readme = "README.md"
-version = "0.0.8"
+version = "0.0.9"
 
 authors = [{ name = "Shahar Luftig", email = "shaharluftig@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
 keywords = [
     "backend",
```

### Comparing `create_fastapi-0.0.8/PKG-INFO` & `create_fastapi-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: create-fastapi-app
 Project-URL: Homepage, https://github.com/shaharluftig/create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -220,8 +220,89 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: gitpython~=3.1.32
 Requires-Dist: typer~=0.9.0
 Requires-Dist: virtualenv~=20.24.1
 Description-Content-Type: text/markdown
 
-# create-fastapi-app
+# Create FastAPI App
+
+Create FastAPI App is a command-line tool that allows you to quickly set up a new FastAPI project with a predefined
+directory structure and configurations. Inspired by `create-react-app` for React projects, this tool aims to simplify
+the initial setup process and get you up and running with FastAPI in no time.
+
+## Table of Contents
+
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Project Structure](#project-structure)
+- [Contributing](#contributing)
+- [License](#license)
+
+## Features
+
+- **Rapid Setup**: Create a new FastAPI project effortlessly without worrying about the initial project structure and
+  configurations.
+- **Ready-to-Code**: Start coding your FastAPI application right away without spending time on boilerplate code.
+
+## Prerequisites
+
+Before using Create FastAPI App, you need to have the following tools installed on your system:
+
+- Python (3.6 or higher)
+- Pip (Python package manager)
+
+## Installation
+
+You can install Create FastAPI App using `pipx`. Open your terminal or command prompt and run the following command:
+* `pipx install create-fastapi`
+
+## Usage
+
+To create a new FastAPI project, use the `create-fastapi-app` command followed by the desired project name:
+`my-fastapi-app`
+
+```bash
+create-fastapi-app my-fastapi-app
+```
+
+By default, this will create a new FastAPI project in a directory named `my-fastapi-app`
+
+Once the project is created, navigate to the project directory and start the development server:
+
+- `cd my-fastapi-app`
+- `python main.py`
+
+## Project structure
+
+- `app`: This directory contains the main application code.
+    - `main.py`: Defines the main FastAPI application, including routes and endpoints.
+    - `models`: Directory for data models and Pydantic schemas.
+    - `routes`: Directory for organizing different API routes.
+    - `utils`: Directory for utility functions and modules.
+
+- `tests`: Contains test files to verify the application's functionality.
+
+- `.env`: Environment variables file to store sensitive or configuration-specific data.
+
+- `.gitignore`: Specifies the files and directories to be ignored by version control (e.g., `.env`, `__pycache__/`,
+  etc.).
+
+- `requirements.txt`: Lists the project dependencies needed to run the FastAPI application.
+### Testing
+* `pytest .`
+
+### Linting
+* `ruff .`
+
+## Contributing
+
+Contributions are welcome! If you find any issues with the tool or want to suggest enhancements, please create a GitHub
+issue or submit a pull request.
+
+## License
+
+Create FastAPI App is open-source software licensed under the [MIT License](https://opensource.org/licenses/MIT).
+
+---
```

