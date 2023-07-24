# Comparing `tmp/gymnasium_connect_four-1.0.2.tar.gz` & `tmp/gymnasium_connect_four-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.0.2.tar", last modified: Sun Jul 23 18:00:41 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.1.0.tar", last modified: Mon Jul 24 10:54:51 2023, max compression
```

## Comparing `gymnasium_connect_four-1.0.2.tar` & `gymnasium_connect_four-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 18:00:41.304881 gymnasium_connect_four-1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-23 18:00:41.303879 gymnasium_connect_four-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3334 2023-07-23 17:37:53.000000 gymnasium_connect_four-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 18:00:41.282882 gymnasium_connect_four-1.0.2/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9016 2023-07-23 18:00:27.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-23 15:35:19.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 18:00:41.293880 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4199 2023-07-23 16:48:20.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     3643 2023-07-23 16:48:25.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      295 2023-07-23 16:46:25.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1489 2023-07-23 16:46:28.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     1896 2023-07-23 16:48:02.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      602 2023-07-23 16:51:40.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0     4068 2023-07-23 17:21:33.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/MinMaxPlayer.py
--rw-rw-rw-   0        0        0      482 2023-07-23 16:51:55.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      393 2023-07-23 15:52:13.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0     2559 2023-07-23 16:48:37.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     3949 2023-07-23 16:49:03.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      442 2023-07-23 17:21:40.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 18:00:41.296882 gymnasium_connect_four-1.0.2/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3380 2023-07-23 17:21:26.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.0.2/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 18:00:41.302879 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-23 18:00:41.000000 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-07-23 18:00:41.000000 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 18:00:41.000000 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-23 18:00:41.000000 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-23 18:00:41.000000 gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 18:00:41.304881 gymnasium_connect_four-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-23 18:00:32.000000 gymnasium_connect_four-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.993398 gymnasium_connect_four-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-07-24 10:54:51.993398 gymnasium_connect_four-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9722 2023-07-24 10:16:33.000000 gymnasium_connect_four-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.962147 gymnasium_connect_four-1.1.0/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9016 2023-07-23 18:00:27.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 15:35:19.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.977772 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4253 2023-07-24 06:32:12.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     3693 2023-07-24 09:48:05.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      338 2023-07-24 06:32:47.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1543 2023-07-24 06:32:40.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 06:32:30.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0     4118 2023-07-24 06:02:34.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/MinMaxPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-24 06:02:41.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0     2609 2023-07-24 06:32:25.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     3999 2023-07-24 06:32:20.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      442 2023-07-23 17:21:40.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.977772 gymnasium_connect_four-1.1.0/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4914 2023-07-24 10:14:31.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.1.0/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.993398 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-24 10:54:51.000000 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1028 2023-07-24 10:54:51.000000 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:54:51.000000 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-24 10:54:51.000000 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-24 10:54:51.000000 gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:54:51.993398 gymnasium_connect_four-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-24 10:14:40.000000 gymnasium_connect_four-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:54:51.993398 gymnasium_connect_four-1.1.0/test/
+-rw-rw-rw-   0        0        0     2373 2023-07-23 20:26:41.000000 gymnasium_connect_four-1.1.0/test/test_easy_mini_grid_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.0.2/LICENSE` & `gymnasium_connect_four-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from .Player import Player
 
 class AdultPlayer(Player):
     
     def __init__(self, _=""):
         pass
-
+    
     def play(self, observation):
         moves_to_avoid = []
 
         # Check for a winning move for the player
         for move in range(7):
             if observation[0, move] == 0:
                 new_board = self.apply_move(observation, move, 1)
@@ -52,14 +52,17 @@
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
         return np.random.choice(valid_moves)
 
     def getName(self):
         return "AdultPlayer"
 
+    def getElo(self):
+        return 1712
+    
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,8 +87,11 @@
                 if (board[i:i+4, j:j+4].diagonal() == player).all():
                     return True
                 if (board[i:i+4, j:j+4][::-1].diagonal() == player).all():
                     return True
         return False
 
     def getName(self):
-        return "AdultSmarterPlayer"
+        return "AdultSmarterPlayer"
+    
+    def getElo(self):
+        return 1767
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,18 @@
                 if self.check_win(new_board, 1):
                     return move
 
         return np.random.choice(range(7))
 
     def getName(self):
         return "ChildPlayer"
-
+    
+    def getElo(self):
+        return 1208
+    
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         # Play a random move
         valid_moves = [c for c in range(7) if observation[0, c] == 0]
         return np.random.choice(valid_moves)
 
     def getName(self):
         return "ChildSmarterPlayer"
 
+    def getElo(self):
+        return 1525
+    
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,11 @@
                 print("Please enter an integer.")
         return move
 
     def getName(self):
         return "ConsolePlayer"
 
     def isDeterministic(self):
-        return False
+        return False
+    
+    def getElo(self):
+        return None
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/MinMaxPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/MinMaxPlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
             best_move = np.random.choice(valid_moves)
 
         return best_move
 
     def getName(self):
         return f"MinimaxPlayer depth {self.depth}"
 
+    def getElo(self):
+        return None
+    
     def isDeterministic(self):
         return False
 
     def minimax(self, board, depth, maximizing_player):
         if depth == 0 or self.is_terminal_node(board):
             evaluation = self.evaluate_board(board)
             return evaluation, []
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
         return np.random.choice(valid_moves)
 
     def getName(self):
         return "TeenagerPlayer"
 
+    def getElo(self):
+        return 1604
+    
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.0.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.1.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
         return np.random.choice(valid_moves)
 
     def getName(self):
         return "TeenagerSmarterPlayer"
 
+    def getElo(self):
+        return 1611
+    
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.0.2/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.1.0/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 connect_four_gymnasium/players/__init__.py
 connect_four_gymnasium/tools/EloLeaderboard.py
 connect_four_gymnasium/tools/__init__.py
 gymnasium_connect_four.egg-info/PKG-INFO
 gymnasium_connect_four.egg-info/SOURCES.txt
 gymnasium_connect_four.egg-info/dependency_links.txt
 gymnasium_connect_four.egg-info/requires.txt
-gymnasium_connect_four.egg-info/top_level.txt
+gymnasium_connect_four.egg-info/top_level.txt
+test/test_easy_mini_grid_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.0.2/setup.py` & `gymnasium_connect_four-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.0.2',
+    version='1.1.0',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

