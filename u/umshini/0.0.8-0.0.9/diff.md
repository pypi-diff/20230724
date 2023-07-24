# Comparing `tmp/umshini-0.0.8.tar.gz` & `tmp/umshini-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umshini-0.0.8.tar", last modified: Fri Jul 14 21:42:11 2023, max compression
+gzip compressed data, was "umshini-0.0.9.tar", last modified: Mon Jul 24 16:55:41 2023, max compression
```

## Comparing `umshini-0.0.8.tar` & `umshini-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-07-14 21:42:08.000000 umshini-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-07-14 21:42:11.271493 umshini-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-14 21:42:08.000000 umshini-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-14 21:42:08.000000 umshini-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:42:11.271493 umshini-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 21:42:08.000000 umshini-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.267492 umshini-0.0.8/umshini/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/envs/envs_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/example_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/tournament_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/socket_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/test_compression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:41.951682 umshini-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-07-24 16:55:33.000000 umshini-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42918 2023-07-24 16:55:41.951682 umshini-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-24 16:55:33.000000 umshini-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-24 16:55:33.000000 umshini-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:55:41.951682 umshini-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 16:55:33.000000 umshini-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:41.947682 umshini-0.0.9/umshini/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:41.951682 umshini-0.0.9/umshini/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/envs/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/example_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/tournament_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:41.951682 umshini-0.0.9/umshini/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/utils/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/utils/socket_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 16:55:33.000000 umshini-0.0.9/umshini/utils/test_compression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:55:41.951682 umshini-0.0.9/umshini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42918 2023-07-24 16:55:41.000000 umshini-0.0.9/umshini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 16:55:41.000000 umshini-0.0.9/umshini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:55:41.000000 umshini-0.0.9/umshini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 16:55:41.000000 umshini-0.0.9/umshini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:55:41.000000 umshini-0.0.9/umshini.egg-info/top_level.txt
```

### Comparing `umshini-0.0.8/LICENSE` & `umshini-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/PKG-INFO` & `umshini-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.8
+Version: 0.0.9
 Summary: Umshini client for playing in MARL tournaments
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -663,23 +663,24 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
-Project-URL: Homepage, https://github.com/umshini/umshini
+Project-URL: Repository, https://github.com/Umshini/Umshini-Server/
+Project-URL: Bug Report, https://github.com/Umshini/Umshini-Server/issues
 Keywords: Reinforcement Learning,game,RL,AI,gym
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: classic
 Provides-Extra: llm
 Provides-Extra: all
 License-File: LICENSE
 
 # Umshini-Client
```

### Comparing `umshini-0.0.8/README.md` & `umshini-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/pyproject.toml` & `umshini-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,28 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["Reinforcement Learning", "game", "RL", "AI", "gym"]
-requires-python = ">=3.7,<3.10"
+requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.19.0",
     "Cython>=0.29.21",
     "pettingzoo>=1.23.1" ,
-    "supersuit>=3.8.1",
     "halo",
     "colorama",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 classic = ["pettingzoo[classic]>=1.23.1"]
-llm = ["chatarena[umshini]>=0.1.12.6"]
+llm = ["chatarena[umshini]>=0.1.12.7"]
 all = ["pettingzoo[classic]>=1.23.1", "chatarena[umshini]>=0.1.12.7"]
 
 [tool.setuptools.dynamic]
 version = {attr = "umshini.__version__"}
 
 [project.urls]
-Homepage = "https://github.com/umshini/umshini"
+Repository = "https://github.com/Umshini/Umshini-Server/"
+"Bug Report" = "https://github.com/Umshini/Umshini-Server/issues"
```

### Comparing `umshini-0.0.8/umshini/envs/envs_list.py` & `umshini-0.0.9/umshini/envs/envs_list.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/umshini/example_client.py` & `umshini-0.0.9/umshini/example_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             quit()
         current_round = 1
         while env is not None:
             term = False
             trunc = False
             timestep = 0
             rew = info = None
-            obs = env.reset()
+            obs, info = env.reset()
             while not (term or trunc):
                 if timestep % 100 == 0 and self.debug:
                     print(f"{self.botname}: Timestep {timestep}\n")
                 time.sleep(self.latency / 1000)  # Used to simulate network latency
                 action_surprise = self.policy(
                     obs, rew, term, trunc, info
                 )  # receive action and surprise from user
```

### Comparing `umshini-0.0.8/umshini/learner.py` & `umshini-0.0.9/umshini/learner.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/umshini/tournament_client.py` & `umshini-0.0.9/umshini/tournament_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 # Send JSON through socket
 def send_json(sock, data):
     return sock.sendall(json.dumps(data).encode("utf-8"))
 
 
 # Receive JSON from socket
-def recv_json(sock, timeout=30):
+def recv_json(sock, timeout=60):
     sock.settimeout(timeout)
     data = sock.recv(2**30)  # Arbitrarily large buffer
-    sock.settimeout(30)
+    sock.settimeout(60)
     return data
 
 
 class NetworkEnv(gym.Env):
     def __init__(self, env_id, seed, game_ip, game_port, username, token, verbose=0):
         self.verbose = verbose
         if self.verbose > 0:
@@ -102,19 +102,20 @@
             info["_terminated"] = True
             self.spinner.succeed()
             return self.obs, rew, term, trunc, info
 
         # Unpack observation
         obs = decompress(observation_data["data"][self.agent])
         self.obs = obs
+        info = decompress(observation_data["info"][self.agent])
+        self.info = info
 
         # TODO: Decide what information a live tournament agent should have access to.
         # Probably observation, info, term or trunc, though term or trunc are obvious from the message type
         rew = 0
-        info = {}
         term = False
         trunc = False
         self.steps += 1
         self.spinner.text = f"Playing game (step: {self.steps})"
         return obs, rew, term, trunc, info
 
     def render(self, mode="human"):
@@ -141,16 +142,18 @@
                 print("No data received")
         if observation_data["type"] != "observation":
             # Game is done
             return self.obs
 
         # Unpack observation
         obs = decompress(observation_data["data"][self.agent])
+        info = decompress(observation_data["info"][self.agent])
         self.obs = obs
-        return self.obs
+        self.info = info
+        return self.obs, self.info
 
     def close(self):
         self.env.close()
         self.game_connection.close()
 
 
 # Local environment used to test if agent works before connecting to network env
@@ -336,14 +339,17 @@
         # Receive game server info from matchmaker
         spinner = Halo(
             text="Creating your game", text_color="cyan", color="green", spinner="dots"
         )
         spinner.start()
         try:
             sdata = recv_json(self.main_connection)
+            while sdata.get("queued") is True:
+                print("Waiting for game...")
+                sdata = recv_json(self.main_connection)
         except TimeoutError as err:
             print("Failed to receive game info from server", flush=True)
             raise err
         spinner.succeed()
 
         # Create network env with game server info
         env = NetworkEnv(
```

### Comparing `umshini-0.0.8/umshini/utils/compress.py` & `umshini-0.0.9/umshini/utils/compress.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/umshini/utils/socket_wrap.py` & `umshini-0.0.9/umshini/utils/socket_wrap.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.8/umshini.egg-info/PKG-INFO` & `umshini-0.0.9/umshini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.8
+Version: 0.0.9
 Summary: Umshini client for playing in MARL tournaments
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -663,23 +663,24 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
-Project-URL: Homepage, https://github.com/umshini/umshini
+Project-URL: Repository, https://github.com/Umshini/Umshini-Server/
+Project-URL: Bug Report, https://github.com/Umshini/Umshini-Server/issues
 Keywords: Reinforcement Learning,game,RL,AI,gym
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: classic
 Provides-Extra: llm
 Provides-Extra: all
 License-File: LICENSE
 
 # Umshini-Client
```

