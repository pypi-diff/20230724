# Comparing `tmp/godot_rl-0.5.0a0.tar.gz` & `tmp/godot_rl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edward/play/godot/godot_rl/tmp/godot_rl_agents/dist/.tmp-sg_t1odn/godot_rl-0.5.0a0.tar", last modified: Sat May  6 07:41:50 2023, max compression
+gzip compressed data, was "godot_rl-0.6.0.tar", last modified: Mon Jul 24 06:51:59 2023, max compression
```

## Comparing `godot_rl-0.5.0a0.tar` & `godot_rl-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/
--rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/LICENSE
--rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     6748 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/README.md
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.586258 godot_rl-0.5.0a0/godot_rl/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/__init__.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/core/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)    11885 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/godot_env.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3181 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/utils.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/custom_models/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3760 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/download_utils/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1191 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1746 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py
--rw-r--r--   0 edward    (1000) edward    (1000)      945 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3595 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/main.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1475 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     2855 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/stable_baselines_export.py
--rw-r--r--   0 edward    (1000) edward    (1000)     5668 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py
--rw-r--r--   0 edward    (1000) edward    (1000)     5566 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py
--rw-r--r--   0 edward    (1000) edward    (1000)     2349 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/stable_baselines_wrapper.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl.egg-info/
--rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     1047 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/dependency_links.txt
--rw-r--r--   0 edward    (1000) edward    (1000)      242 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/entry_points.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/not-zip-safe
--rw-r--r--   0 edward    (1000) edward    (1000)      534 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/requires.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        9 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/top_level.txt
--rw-r--r--   0 edward    (1000) edward    (1000)      887 2023-05-06 07:41:12.000000 godot_rl-0.5.0a0/pyproject.toml
--rw-r--r--   0 edward    (1000) edward    (1000)     1258 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/setup.cfg
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/tests/
--rw-r--r--   0 edward    (1000) edward    (1000)     1333 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py
--rw-r--r--   0 edward    (1000) edward    (1000)      421 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_call_method.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3358 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_godot_env.py
--rw-r--r--   0 edward    (1000) edward    (1000)      929 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_onnx_export.py
--rw-r--r--   0 edward    (1000) edward    (1000)      588 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_training.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1071 2023-04-09 18:36:52.000000 godot_rl-0.6.0/LICENSE
+-rw-rw-r--   0 edward    (1000) edward    (1000)     7829 2023-07-24 06:51:59.519665 godot_rl-0.6.0/PKG-INFO
+-rw-rw-r--   0 edward    (1000) edward    (1000)     6780 2023-07-18 20:01:12.000000 godot_rl-0.6.0/README.md
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/
+-rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-04-09 18:36:52.000000 godot_rl-0.6.0/godot_rl/__init__.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/core/
+-rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-04-09 18:36:52.000000 godot_rl-0.6.0/godot_rl/core/__init__.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)    13844 2023-07-23 12:31:39.000000 godot_rl-0.6.0/godot_rl/core/godot_env.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     4105 2023-07-23 12:31:39.000000 godot_rl-0.6.0/godot_rl/core/utils.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/custom_models/
+-rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-04-09 18:36:52.000000 godot_rl-0.6.0/godot_rl/custom_models/__init__.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     3760 2023-04-10 19:51:27.000000 godot_rl-0.6.0/godot_rl/custom_models/attention_model.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/download_utils/
+-rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-04-09 18:36:52.000000 godot_rl-0.6.0/godot_rl/download_utils/__init__.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1191 2023-04-10 19:52:13.000000 godot_rl-0.6.0/godot_rl/download_utils/download_examples.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1746 2023-04-10 19:52:13.000000 godot_rl-0.6.0/godot_rl/download_utils/download_godot_editor.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)      945 2023-04-10 19:52:13.000000 godot_rl-0.6.0/godot_rl/download_utils/from_hub.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     4014 2023-07-23 12:31:39.000000 godot_rl-0.6.0/godot_rl/main.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/wrappers/
+-rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-04-09 18:36:52.000000 godot_rl-0.6.0/godot_rl/wrappers/__init__.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1475 2023-04-10 19:52:13.000000 godot_rl-0.6.0/godot_rl/wrappers/clean_rl_wrapper.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl/wrappers/onnx/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-04-24 19:00:22.000000 godot_rl-0.6.0/godot_rl/wrappers/onnx/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     2855 2023-04-24 19:00:22.000000 godot_rl-0.6.0/godot_rl/wrappers/onnx/stable_baselines_export.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     5723 2023-07-18 20:01:12.000000 godot_rl-0.6.0/godot_rl/wrappers/ray_wrapper.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     6161 2023-07-23 12:31:39.000000 godot_rl-0.6.0/godot_rl/wrappers/sample_factory_wrapper.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     5454 2023-07-23 12:31:39.000000 godot_rl-0.6.0/godot_rl/wrappers/stable_baselines_wrapper.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/godot_rl.egg-info/
+-rw-rw-r--   0 edward    (1000) edward    (1000)     7829 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/PKG-INFO
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1076 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/SOURCES.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/dependency_links.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)      242 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/entry_points.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-04-09 18:41:13.000000 godot_rl-0.6.0/godot_rl.egg-info/not-zip-safe
+-rw-rw-r--   0 edward    (1000) edward    (1000)      421 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/requires.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        9 2023-07-24 06:51:59.000000 godot_rl-0.6.0/godot_rl.egg-info/top_level.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)      886 2023-07-24 06:51:39.000000 godot_rl-0.6.0/pyproject.toml
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1136 2023-07-24 06:51:59.519665 godot_rl-0.6.0/setup.cfg
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-24 06:51:59.519665 godot_rl-0.6.0/tests/
+-rw-r--r--   0 edward    (1000) edward    (1000)     1339 2023-07-23 12:31:39.000000 godot_rl-0.6.0/tests/test_action_space_preprocessor.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)      421 2023-04-09 18:36:52.000000 godot_rl-0.6.0/tests/test_call_method.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     3358 2023-04-09 18:36:52.000000 godot_rl-0.6.0/tests/test_godot_env.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      606 2023-07-23 12:31:39.000000 godot_rl-0.6.0/tests/test_sample_factory.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      929 2023-04-24 19:00:22.000000 godot_rl-0.6.0/tests/test_sb3_onnx_export.py
+-rw-rw-r--   0 edward    (1000) edward    (1000)     1032 2023-07-23 12:31:39.000000 godot_rl-0.6.0/tests/test_sb3_training.py
```

### Comparing `godot_rl-0.5.0a0/LICENSE` & `godot_rl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/PKG-INFO` & `godot_rl-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godot_rl
-Version: 0.5.0a0
+Version: 0.6.0
 Summary: A Deep Reinforcement Learning package for the Godot game engine
 Author: Edward Beeching
 Author-email: Edward Beeching <edbeeching@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
 Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
 Platform: unix
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
-Provides-Extra: sb3
 Provides-Extra: sf
 Provides-Extra: rllib
 Provides-Extra: clean-rl
 Provides-Extra: all
 License-File: LICENSE
 
 # Godot RL Agents
@@ -67,15 +66,15 @@
 gdrl.env_from_hub -r edbeeching/godot_rl_JumperHard 
 ```
 You may need to example run permissions on the game executable. `chmod +x examples/godot_rl_JumperHard/bin/JumperHard.x86_64`
 
 3. Train and visualize 
 
 ```bash
-gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --viz
+gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --experiment_name=Experiment_01 --viz
 ```
 
 ### In editor interactive training
 
 You can also train an agent in the Godot editor, without the need to export the game executable.
 
 1. Download the Godot 4 Game Engine from [https://godotengine.org/](https://godotengine.org/)
```

### Comparing `godot_rl-0.5.0a0/README.md` & `godot_rl-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 gdrl.env_from_hub -r edbeeching/godot_rl_JumperHard 
 ```
 You may need to example run permissions on the game executable. `chmod +x examples/godot_rl_JumperHard/bin/JumperHard.x86_64`
 
 3. Train and visualize 
 
 ```bash
-gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --viz
+gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --experiment_name=Experiment_01 --viz
 ```
 
 ### In editor interactive training
 
 You can also train an agent in the Godot editor, without the need to export the game executable.
 
 1. Download the Godot 4 Game Engine from [https://godotengine.org/](https://godotengine.org/)
```

### Comparing `godot_rl-0.5.0a0/godot_rl/core/godot_env.py` & `godot_rl-0.6.0/godot_rl/core/godot_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,50 @@
 import pathlib
 import socket
 import subprocess
 import time
 from sys import platform
 
 import numpy as np
-from gym import spaces
-
+from gymnasium import spaces
+from typing import Optional
 from godot_rl.core.utils import ActionSpaceProcessor, convert_macos_path
 
 
 class GodotEnv:
-    MAJOR_VERSION = "0"
-    MINOR_VERSION = "3"
-    DEFAULT_PORT = 11008
-    DEFAULT_TIMEOUT = 60
+    MAJOR_VERSION = "0" # Versioning for the environment
+    MINOR_VERSION = "4"
+    DEFAULT_PORT = 11008 # Default port for communication with Godot Game
+    DEFAULT_TIMEOUT = 60 # Default socket timeout TODO
 
     def __init__(
         self,
-        env_path=None,
-        port=11008,
-        show_window=False,
-        seed=0,
-        framerate=None,
-        action_repeat=None,
-        speedup=None,
-        convert_action_space=False,
+        env_path: str=None,
+        port: int=DEFAULT_PORT,
+        show_window: bool=False,
+        seed:int=0,
+        framerate:Optional[int]=None,
+        action_repeat:Optional[int]=None,
+        speedup:Optional[int]=None,
+        convert_action_space:bool=False,
     ):
+        """
+        Initialize a new instance of GodotEnv
+
+        Args:
+            env_path (str): path to the godot binary environment.
+            port (int): Port number for communication.
+            show_window (bool): flag to display Godot game window.
+            seed (int): seed to initialize the environment.
+            framerate (int): the framerate to run the Godot game at.
+            action_repeat (int): the number of frames to repeat an action for.
+            speedup (int): the factor to speedup game time by.
+            convert_action_space (bool): flag to convert action space.
+        """
 
-        if env_path is None:
-            port = GodotEnv.DEFAULT_PORT
         self.proc = None
         if env_path is not None and env_path != "debug":
             env_path = self._set_platform_suffix(env_path)
 
             self.check_platform(env_path)
             self._launch_env(env_path, port, show_window, framerate, seed, action_repeat, speedup)
         else:
@@ -49,25 +60,43 @@
         self._get_env_info()
         # sf2 requires a tuple action space
         self._tuple_action_space = spaces.Tuple([v for _, v in self._action_space.items()])
         self.action_space_processor = ActionSpaceProcessor(self._tuple_action_space, convert_action_space)
 
         atexit.register(self._close)
 
-    def _set_platform_suffix(self, env_path):
+    def _set_platform_suffix(self, env_path: str) -> str:
+        """
+        Set the platform suffix for the given environment path based on the platform.
+
+        Args:
+            env_path (str): The environment path.
+
+        Returns:
+            str: The environment path with the platform suffix.
+        """
         suffixes = {
             "linux": ".x86_64",
             "linux2": ".x86_64",
             "darwin": ".app",
             "win32": ".exe",
         }
         suffix = suffixes[platform]
         return str(pathlib.Path(env_path).with_suffix(suffix))
 
     def check_platform(self, filename: str):
+        """
+        Check the platform and assert the file type
+
+        Args:
+            filename (str): Path of the file to check.
+
+        Raises:
+            AssertionError: If the file type does not match with the platform or file does not exist.
+        """
         if platform == "linux" or platform == "linux2":
             # Linux
             assert (
                 pathlib.Path(filename).suffix == ".x86_64"
             ), f"Incorrect file suffix for filename {filename} suffix {pathlib.Path(filename).suffix }. Please provide a .x86_64 file"
         elif platform == "darwin":
             # OSX
@@ -81,15 +110,24 @@
             ), f"Incorrect file suffix for filename {filename} suffix {pathlib.Path(filename).suffix }. Please provide a .exe file"
         else:
             assert 0, f"unknown filetype {pathlib.Path(filename).suffix}"
 
         assert os.path.exists(filename)
 
     def from_numpy(self, action, order_ij=False):
-        # handles dict to tuple actions
+        """
+        Handles dict to tuple actions
+
+        Args:
+            action: The action to be converted.
+            order_ij (bool): Order flag.
+
+        Returns:
+            list: The converted action.
+        """
         result = []
 
         for i in range(self.num_envs):
             env_action = {}
 
             for j, k in enumerate(self._action_space.keys()):
                 if order_ij == True:
@@ -102,42 +140,87 @@
                 else:
                     env_action[k] = int(v)  # cannot serialize int32
 
             result.append(env_action)
         return result
 
     def step(self, action, order_ij=False):
+        """
+        Perform one step in the environment.
+
+        Args:
+            action: Action to be taken.
+            order_ij (bool): Order flag.
+
+        Returns:
+            tuple: Tuple containing observation, reward, done flag, termination flag, and info.
+        """
+        self.step_send(action, order_ij=order_ij)
+        return self.step_recv()
+        
+
+    def step_send(self, action, order_ij=False):
+        """
+        Send the action to the Godot environment.
+
+        Args:
+            action: Action to be sent.
+            order_ij (bool): Order flag.
+        """
         action = self.action_space_processor.to_original_dist(action)
         message = {
             "type": "action",
             "action": self.from_numpy(action, order_ij=order_ij),
         }
         self._send_as_json(message)
+    
+    def step_recv(self):
+        """
+        Receive the step response from the Godot environment.
+
+        Returns:
+            tuple: Tuple containing observation, reward, done flag, termination flag, and info.
+        """
         response = self._get_json_dict()
-
         response["obs"] = self._process_obs(response["obs"])
 
         return (
             response["obs"],
             response["reward"],
             np.array(response["done"]).tolist(),
             np.array(response["done"]).tolist(),  # TODO update API to term, trunc
             [{}] * len(response["done"]),
         )
+        
+        
 
     def _process_obs(self, response_obs: dict):
+        """
+        Process observation data.
 
+        Args:
+            response_obs (dict): The response observation to be processed.
+
+        Returns:
+            dict: The processed observation data.
+        """
         for k in response_obs[0].keys():
             if "2d" in k:
                 for sub in response_obs:
-                    sub[k] = self.decode_2d_obs_from_string(sub[k], self.observation_space[k].shape)
+                    sub[k] = self._decode_2d_obs_from_string(sub[k], self.observation_space[k].shape)
 
         return response_obs
 
     def reset(self, seed=None):
+        """
+        Reset the Godot environment.
+
+        Returns:
+            dict: The initial observation data.
+        """
         message = {
             "type": "reset",
         }
         self._send_as_json(message)
         response = self._get_json_dict()
         response["obs"] = self._process_obs(response["obs"])
         assert response["type"] == "reset"
@@ -163,14 +246,18 @@
         time.sleep(1.0)
         self.connection.close()
         try:
             atexit.unregister(self._close)
         except Exception as e:
             print("exception unregistering close method", e)
 
+    @property
+    def action_space(self):
+        return self.action_space_processor.action_space
+
     def _close(self):
         print("exit was not clean, using atexit to close env")
         self.close()
 
     def _launch_env(self, env_path, port, show_window, framerate, seed, action_repeat, speedup):
         # --fixed-fps {framerate}
         path = convert_macos_path(env_path) if platform == "darwin" else env_path
@@ -252,39 +339,25 @@
                     low=-1.0,
                     high=1.0,
                     shape=v["size"],
                     dtype=np.float32,
                 )
             elif v["space"] == "discrete":
                 observation_spaces[k] = spaces.Discrete(v["size"])
-            # elif v["space"] == "repeated": TODO: Add repeated spaces back when we have support and a good example
-            #     assert "max_length" in v
-            #     if v["subspace"] == "box":
-            #         subspace = observation_spaces[k] = spaces.Box(
-            #             low=-1.0,
-            #             high=1.0,
-            #             shape=v["size"],
-            #             dtype=np.float32,
-            #         )
-            #     elif v["subspace"] == "discrete":
-            #         subspace = spaces.Discrete(v["size"])
-            #     observation_spaces[k] = Repeated(subspace, v["max_length"])
             else:
                 print(f"observation space {v['space']} is not supported")
                 assert 0, f"observation space {v['space']} is not supported"
         self.observation_space = spaces.Dict(observation_spaces)
 
         self.num_envs = json_dict["n_agents"]
 
-    @property
-    def action_space(self):
-        return self.action_space_processor.action_space
+
 
     @staticmethod
-    def decode_2d_obs_from_string(
+    def _decode_2d_obs_from_string(
         hex_string,
         shape,
     ):
         return (
             np.frombuffer(bytes.fromhex(hex_string), dtype=np.float16)
             .reshape(shape)
             .astype(np.float32)[:, :, :]  # TODO remove the alpha channel
@@ -298,23 +371,21 @@
         data = self._get_data()
         return json.loads(data)
 
     def _get_obs(self):
         return self._get_data()
 
     def _clear_socket(self):
-
         self.connection.setblocking(False)
         try:
             while True:
                 data = self.connection.recv(4)
                 if not data:
                     break
         except BlockingIOError as e:
-            # print("BlockingIOError expection on clear")
             pass
         self.connection.setblocking(True)
 
     def _get_data(self):
         try:
             data = self.connection.recv(4)
             if not data:
```

### Comparing `godot_rl-0.5.0a0/godot_rl/core/utils.py` & `godot_rl-0.6.0/godot_rl/core/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import gym
-import numpy as np
+import importlib
 import re
 
+import gymnasium as gym
+import numpy as np
+
+
 
 def lod_to_dol(lod):
     return {k: [dic[k] for dic in lod] for k in lod[0]}
 
 
 def dol_to_lod(dol):
     return [dict(zip(dol, t)) for t in zip(*dol.values())]
@@ -36,34 +39,45 @@
 
         self._original_action_space = action_space
         self._convert = convert
 
         space_size = 0
 
         if convert:
+            use_multi_discrete_spaces = False
+            multi_discrete_spaces = np.array([])
             if isinstance(action_space, gym.spaces.Tuple):
 
-                for space in action_space.spaces:
-                    if isinstance(space, gym.spaces.Box):
-                        assert len(space.shape) == 1
-                        space_size += space.shape[0]
-                    elif isinstance(space, gym.spaces.Discrete):
-                        if space.n > 2:
-                            # for not only binary actions are supported, need to add support for the n>2 case
+                if all(isinstance(space, gym.spaces.Discrete) for space in action_space.spaces):
+                    use_multi_discrete_spaces = True
+                    for space in action_space.spaces:
+                        multi_discrete_spaces = np.append(multi_discrete_spaces, space.n)
+                else:
+                    for space in action_space.spaces:
+                        if isinstance(space, gym.spaces.Box):
+                            assert len(space.shape) == 1
+                            space_size += space.shape[0]
+                        elif isinstance(space, gym.spaces.Discrete):
+                            if space.n > 2:
+                                #for now only binary actions are supported if you mix different spaces
+                                # need to add support for the n>2 case
+                                raise NotImplementedError
+                            space_size += 1
+                        else:
                             raise NotImplementedError
-                        space_size += 1
-                    else:
-                        raise NotImplementedError
             elif isinstance(action_space, gym.spaces.Dict):
                 raise NotImplementedError
             else:
                 assert isinstance(space, [gym.spaces.Box, gym.spaces.Discrete])
                 return
 
-            self.converted_action_space = gym.spaces.Box(-1, 1, shape=[space_size])
+            if use_multi_discrete_spaces:
+                self.converted_action_space = gym.spaces.MultiDiscrete(multi_discrete_spaces)
+            else:
+                self.converted_action_space = gym.spaces.Box(-1, 1, shape=[space_size])
 
     @property
     def action_space(self):
         if not self._convert:
             return self._original_action_space
 
         return self.converted_action_space
@@ -88,7 +102,17 @@
                 original_action.append(discrete_actions)
                 counter += 1
 
             else:
                 raise NotImplementedError
 
         return original_action
+
+def can_import(module_name):
+    return not cant_import(module_name)
+
+def cant_import(module_name):
+    try:
+        importlib.import_module(module_name)
+        return False
+    except ImportError:
+        return True
```

### Comparing `godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py` & `godot_rl-0.6.0/godot_rl/custom_models/attention_model.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py` & `godot_rl-0.6.0/godot_rl/download_utils/download_examples.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py` & `godot_rl-0.6.0/godot_rl/download_utils/download_godot_editor.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py` & `godot_rl-0.6.0/godot_rl/download_utils/from_hub.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/main.py` & `godot_rl-0.6.0/godot_rl/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,61 +21,61 @@
 """
 
 import argparse
 
 try:
     from godot_rl.wrappers.ray_wrapper import rllib_training
 except ImportError as e:
-    print("Error: ", e)
     def rllib_training(args, extras):
         print("Import error when trying to use rllib. If you have not installed the package, try: pip install godot-rl[rllib]")
         print("Otherwise try fixing the error above.")
 
 
 try:
     from godot_rl.wrappers.stable_baselines_wrapper import stable_baselines_training
 except ImportError as e:
-    print("Error: ", e)
     def stable_baselines_training(args, extras):
         print(
             "Import error when trying to use sb3. If you have not installed the package, try: pip install godot-rl[sb3]"
         )
         print("Otherwise try fixing the error above.")
 
 try:
     from godot_rl.wrappers.sample_factory_wrapper import sample_factory_training, sample_factory_enjoy
 except ImportError as e:
-    print("Error: ", e)
     def sample_factory_training(args, extras):
         print(
             "Import error when trying to use sample-factory If you have not installed the package, try: pip install godot-rl[sf]"
         )
         print("Otherwise try fixing the error above.")
 
 
 def get_args():
     parser = argparse.ArgumentParser(allow_abbrev=False)
-    parser.add_argument(
-        "--trainer",
-        default="sb3",
-        choices=["sb3", "sf", "rllib"],
-        type=str,
-        help="framework to use (rllib or stable-baselines)",
-    )
+    parser.add_argument("--trainer", default="sb3", choices=["sb3", "sf", "rllib"], type=str, help="framework to use (rllib, sf, sb3)")
     parser.add_argument("--env_path", default=None, type=str, help="Godot binary to use")
-    parser.add_argument("--config_file", default="ppo_test.yaml", type=str, help="The yaml config file (used by rllib)")
+    parser.add_argument("--config_file", default="ppo_test.yaml", type=str, help="The yaml config file [only for rllib]")
     parser.add_argument("--restore", default=None, type=str, help="the location of a checkpoint to restore from")
     parser.add_argument("--eval", default=False, action="store_true", help="whether to eval the model")
     parser.add_argument("--speedup", default=1, type=int, help="whether to speed up the physics in the env")
     parser.add_argument("--export", default=False, action="store_true", help="wheter to export the model")
     parser.add_argument("--num_gpus", default=None, type=int, help="Number of GPUs to use [only for rllib]")
-    parser.add_argument("--experiment_name", default=None, type=str, help="The name of the experiment [only for rllib]")
+    parser.add_argument("--experiment_dir", default=None, type=str, help="The name of the the experiment directory, in which the tensorboard logs are getting stored")
+    parser.add_argument("--experiment_name", default="experiment", type=str, help="The name of the the experiment, which will be displayed in tensborboard")
     parser.add_argument("--viz", default=False, action="store_true", help="Whether to visualize one process")
+    
+    args, extras =  parser.parse_known_args()
+    if args.experiment_dir is None:
+        args.experiment_dir = f"logs/{args.trainer}"
+        
+    if args.trainer == "sf" and args.env_path is None:
+        print("WARNING: the sample-factory intergration is not designed to run in interactive mode, please export you game to use this trainer")
+        
 
-    return parser.parse_known_args()
+    return args, extras
 
 
 def main():
     args, extras = get_args()
     if args.trainer == "rllib":
         training_function = rllib_training
     elif args.trainer == "sb3":
```

### Comparing `godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py` & `godot_rl-0.6.0/godot_rl/wrappers/clean_rl_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/wrappers/onnx/stable_baselines_export.py` & `godot_rl-0.6.0/godot_rl/wrappers/onnx/stable_baselines_export.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py` & `godot_rl-0.6.0/godot_rl/wrappers/ray_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         name=run_name,
         config=exp["config"],
         stop=exp["stop"],
         verbose=3,
         checkpoint_freq=checkpoint_freq,
         checkpoint_at_end=not args.eval,
         restore=args.restore,
+        local_dir=args.experiment_dir or "logs/rllib",
         trial_name_creator=lambda trial: f"{args.experiment_name}" if args.experiment_name else f"{trial.trainable_name}_{trial.trial_id}"
     )
     if args.export:
         rllib_export(args.restore)
 
     ray.shutdown()
```

### Comparing `godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py` & `godot_rl-0.6.0/godot_rl/wrappers/sample_factory_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import argparse
-import sys
 from functools import partial
 import random
 import numpy as np
-from gym import spaces
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import register_env
 from sample_factory.train import run_rl
 from sample_factory.enjoy import enjoy
 
 from godot_rl.core.godot_env import GodotEnv
 from godot_rl.core.utils import lod_to_dol
+from gymnasium import Env
 
-
-class SampleFactoryEnvWrapperBatched(GodotEnv):
+class SampleFactoryEnvWrapperBatched(GodotEnv, Env):
     @property
     def unwrapped(self):
         return self
 
     @property
     def num_agents(self):
         return self.num_envs
 
-    def reset(self, seed=None):
+    def reset(self, seed=None, options=None):
         obs, info = super().reset(seed=seed)
         obs = lod_to_dol(obs)
         return {k: np.array(v) for k, v in obs.items()}, info
 
     def step(self, action):
         obs, reward, term, trunc, info = super().step(action, order_ij=False)
         obs = lod_to_dol(obs)
@@ -41,30 +39,28 @@
 
         return lod
 
     def render():
         return
 
 
-class SampleFactoryEnvWrapperNonBatched(GodotEnv):
+class SampleFactoryEnvWrapperNonBatched(GodotEnv, Env):
     @property
     def unwrapped(self):
         return self
 
     @property
     def num_agents(self):
         return self.num_envs
-
-    def reset(self, seed=None):
+    def reset(self, seed=None, options=None):
         obs, info = super().reset(seed=seed)
         return self.to_numpy(obs), info
 
     def step(self, action):
         obs, reward, term, trunc, info = super().step(action, order_ij=True)
-
         return self.to_numpy(obs), np.array(reward), np.array(term), np.array(trunc) * 0, info
 
     @staticmethod
     def to_numpy(lod):
 
         for d in lod:
             for k, v in d.items():
@@ -74,15 +70,15 @@
 
     def render():
         return
 
 
 def make_godot_env_func(env_path, full_env_name, cfg=None, env_config=None, render_mode=None, speedup=1, viz=False):
     seed = 0
-    port = 21008 + cfg.base_port
+    port = cfg.base_port
     print("BASE PORT ", cfg.base_port)
     show_window = False
     if env_config:
         port += 1 + env_config.env_id
         seed += 1 + env_config.env_id
         print("env id", env_config.env_id)
         if viz:  #
@@ -152,36 +148,51 @@
 
 
 def add_gdrl_env_args(_env, p: argparse.ArgumentParser, evaluation=False):
     if evaluation:
         # apparently env.render(mode="human") is not supported anymore and we need to specify the render mode in
         # the env actor
         p.add_argument("--render_mode", default="human", type=str, help="")
-    p.add_argument("--base_port", default=0, type=int, help="")
+    p.add_argument("--base_port", default=GodotEnv.DEFAULT_PORT, type=int, help="")
 
     p.add_argument(
         "--env_agents",
         default=2,
         type=int,
         help="Num agents in each envpool (if used)",
     )
+    p.add_argument(
+        "--experiment_dir",
+        default="logs/sf",
+        type=str,
+        help="The name of the experiment directory, in which the tensorboard logs are getting stored",
+    )
+    p.add_argument(
+        "--experiment_name",
+        default=None,
+        type=str,
+        help="The name of the experiment, which will be displayed in tensorboard",
+    )
 
 
 def parse_gdrl_args(argv=None, evaluation=False):
     parser, partial_cfg = parse_sf_args(argv=argv, evaluation=evaluation)
     add_gdrl_env_args(partial_cfg.env, parser, evaluation=evaluation)
     gdrl_override_defaults(partial_cfg.env, parser)
     final_cfg = parse_full_cfg(parser, argv)
+    args, _ = parser.parse_known_args(argv)
+    final_cfg.train_dir = args.experiment_dir or "logs/sf"
+    final_cfg.experiment = args.experiment_name or final_cfg.experiment
     return final_cfg
 
 
 def sample_factory_training(args, extras):
     register_gdrl_env(args)
     cfg = parse_gdrl_args(argv=extras, evaluation=args.eval)
-    cfg.base_port = random.randint(20000, 22000)
+    #cfg.base_port = random.randint(20000, 22000)
     status = run_rl(cfg)
     return status
 
 
 def sample_factory_enjoy(args, extras):
     register_gdrl_env(args)
     cfg = parse_gdrl_args(argv=extras, evaluation=args.eval)
```

### Comparing `godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO` & `godot_rl-0.6.0/godot_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godot-rl
-Version: 0.5.0a0
+Version: 0.6.0
 Summary: A Deep Reinforcement Learning package for the Godot game engine
 Author: Edward Beeching
 Author-email: Edward Beeching <edbeeching@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
 Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
 Platform: unix
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
-Provides-Extra: sb3
 Provides-Extra: sf
 Provides-Extra: rllib
 Provides-Extra: clean-rl
 Provides-Extra: all
 License-File: LICENSE
 
 # Godot RL Agents
@@ -67,15 +66,15 @@
 gdrl.env_from_hub -r edbeeching/godot_rl_JumperHard 
 ```
 You may need to example run permissions on the game executable. `chmod +x examples/godot_rl_JumperHard/bin/JumperHard.x86_64`
 
 3. Train and visualize 
 
 ```bash
-gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --viz
+gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --experiment_name=Experiment_01 --viz
 ```
 
 ### In editor interactive training
 
 You can also train an agent in the Godot editor, without the need to export the game executable.
 
 1. Download the Godot 4 Game Engine from [https://godotengine.org/](https://godotengine.org/)
```

### Comparing `godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt` & `godot_rl-0.6.0/godot_rl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 godot_rl/wrappers/__init__.py
 godot_rl/wrappers/clean_rl_wrapper.py
 godot_rl/wrappers/ray_wrapper.py
 godot_rl/wrappers/sample_factory_wrapper.py
 godot_rl/wrappers/stable_baselines_wrapper.py
 godot_rl/wrappers/onnx/__init__.py
 godot_rl/wrappers/onnx/stable_baselines_export.py
-tests/test_action_space_proprocessor.py
+tests/test_action_space_preprocessor.py
 tests/test_call_method.py
 tests/test_godot_env.py
+tests/test_sample_factory.py
 tests/test_sb3_onnx_export.py
 tests/test_sb3_training.py
```

### Comparing `godot_rl-0.5.0a0/pyproject.toml` & `godot_rl-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "godot_rl"
-version = "0.5.0a"
+version = "0.6.0"
 authors = [
   { name="Edward Beeching", email="edbeeching@gmail.com" },
 ]
 description = "A Deep Reinforcement Learning package for the Godot game engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `godot_rl-0.5.0a0/setup.cfg` & `godot_rl-0.6.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [options]
 packages = find:
 install_requires = 
 	numpy
 	tensorboard
 	wget
 	huggingface_hub>=0.10
-	gym==0.26.2
+	gymnasium
 	stable-baselines3
 	huggingface_sb3
 	onnx
 	onnxruntime
 python_requires = >=3.8
 zip_safe = no
 
@@ -37,35 +37,26 @@
 dev = 
 	pytest>=6.0
 	pytest-xdist
 	black[jupyter]~=22.0
 	flake8>=3.8.3
 	isort>=5.0.0
 	pyyaml>=5.3.1
-sb3 = 
-	gym==0.26.2
-	stable-baselines3
-	huggingface_sb3
 sf = 
 	sample-factory
-	gym==0.26.2
 rllib = 
 	numpy==1.23.5
 	ray==2.2.0
 	ray[rllib]
 	tensorflow_probability
 clean-rl = 
 	wandb
 all = 
 	numpy==1.23.5
-	gym==0.26.2
-	stable-baselines3
-	huggingface_sb3
 	sample-factory
-	
 	ray==2.2.0
 	ray[rllib]
 	tensorflow_probability
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py` & `godot_rl-0.6.0/tests/test_action_space_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from gym.spaces import Tuple, Dict, Box, Discrete
+from gymnasium.spaces import Tuple, Dict, Box, Discrete
 from godot_rl.core.godot_env import GodotEnv
 from godot_rl.core.utils import ActionSpaceProcessor
 
 @pytest.mark.parametrize("action_space", 
     [
         Tuple([Box(-1,1, shape=[7]), Box(-1,1, shape=[11])]),
         Tuple([Box(-1,1, shape=[7]), Discrete(2)]),
```

### Comparing `godot_rl-0.5.0a0/tests/test_godot_env.py` & `godot_rl-0.6.0/tests/test_godot_env.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0a0/tests/test_sb3_onnx_export.py` & `godot_rl-0.6.0/tests/test_sb3_onnx_export.py`

 * *Files identical despite different names*

