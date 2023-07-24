# Comparing `tmp/textology-0.0.6.tar.gz` & `tmp/textology-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.0.6.tar", last modified: Sun Jul 16 17:19:26 2023, max compression
+gzip compressed data, was "textology-0.2.0.tar", last modified: Mon Jul 24 01:21:10 2023, max compression
```

## Comparing `textology-0.0.6.tar` & `textology-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.205187 textology-0.0.6/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.0.6/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.0.6/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    15352 2023-07-16 17:19:26.205347 textology-0.0.6/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    13990 2023-07-16 17:16:06.000000 textology-0.0.6/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.0.6/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.0.6/requirements-full-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.0.6/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-16 17:19:26.206331 textology-0.0.6/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.0.6/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.193153 textology-0.0.6/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-16 17:16:06.000000 textology-0.0.6/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)    12177 2023-07-16 17:16:06.000000 textology-0.0.6/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2362 2023-07-08 19:46:35.000000 textology-0.0.6/textology/dash_compat.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.0.6/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.0.6/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.198110 textology-0.0.6/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      814 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     3944 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-04 19:31:50.000000 textology-0.0.6/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    23617 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.0.6/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.0.6/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    29250 2023-07-09 19:13:48.000000 textology-0.0.6/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.204811 textology-0.0.6/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     1165 2023-07-08 19:46:35.000000 textology-0.0.6/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1248 2023-07-15 18:59:20.000000 textology-0.0.6/textology/widgets/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-15 18:57:36.000000 textology-0.0.6/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2265 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.0.6/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_list_item_meta.py
--rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.0.6/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.195962 textology-0.0.6/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    15352 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     1050 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.960494 textology-0.2.0/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.2.0/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.2.0/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    15562 2023-07-24 01:21:10.960768 textology-0.2.0/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    14200 2023-07-24 01:09:35.000000 textology-0.2.0/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.2.0/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.2.0/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.2.0/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-24 01:21:10.962022 textology-0.2.0/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.2.0/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.938913 textology-0.2.0/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-24 01:09:35.000000 textology-0.2.0/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16797 2023-07-24 01:09:35.000000 textology-0.2.0/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6108 2023-07-24 01:09:35.000000 textology-0.2.0/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.2.0/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.2.0/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.948037 textology-0.2.0/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.2.0/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    31200 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5473 2023-07-24 01:09:35.000000 textology-0.2.0/textology/pages.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.2.0/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.2.0/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.2.0/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.959948 textology-0.2.0/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1204 2023-07-24 01:09:35.000000 textology-0.2.0/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1488 2023-07-24 01:09:35.000000 textology-0.2.0/textology/widgets/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-15 18:57:36.000000 textology-0.2.0/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2265 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.2.0/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.2.0/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.943831 textology-0.2.0/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    15562 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     1069 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/top_level.txt
```

### Comparing `textology-0.0.6/LICENSE` & `textology-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/PKG-INFO` & `textology-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.0.6
+Version: 0.2.0
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -132,61 +132,66 @@
 developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
 ```shell
 pip install textology[full-dev]
 ```
 
 ### Extended Applications
 
-Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
-extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
+Textology app classes, such as `ExtendedApp`, can replace any regular Textual App, and be used as is without any
+extensions turned on. Here is an example of the most commonly used application subclass, `ExtendedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
+
 ```python
-from textology.apps import ObservedApp
+from textology.apps import ExtendedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-app = ObservedApp(
+app = ExtendedApp(
     layout=Container(
         Button("Ping", id="ping-btn"),
         Button("Pong", id="pong-btn"),
         Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
+
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
 
+
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def pong(clicks):
     return Label(f"Pong pressed {clicks}")
 
+
 @app.when(
     Modified("sing-btn", "n_clicks"),
     Select("ping-btn", "n_clicks"),
     Select("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def song(song_clicks, ping_clicks, pong_clicks):
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
+
 app.run()
 ```
 
 - Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
@@ -194,23 +199,32 @@
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
 
+- Callbacks can also catch Exceptions from other callbacks:
+```python
+@app.when(
+    Raised(Exception),
+)
+def error_notification(error):
+    app.notify(f"An unknown error occurred: {error}", title="Error")
+```
+
 - <details>
   <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update
     from textology.widgets import Button, Container, Label
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Container(
             Button("Ping", id="ping-btn"),
             Button("Pong", id="pong-btn"),
             Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
@@ -246,15 +260,15 @@
     ```
 
 
 - <details>
   <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update, when
     from textology.widgets import Button, Container, Label
     
     
     class Page(Container):
         def compose(self):
             yield Button("Ping", id="ping-btn")
@@ -286,15 +300,15 @@
         )
         def song(self, event, ping_clicks, pong_clicks):
             if not ping_clicks or not pong_clicks:
                 return Label(f"Press Ping and Pong first to complete the song!")
             return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
     
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Page()
     )
     
     app.run()
     ```
 
 
@@ -418,14 +432,14 @@
 
 @pytest.mark.asyncio
 async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
-- Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
+- Ability to pass an App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
 
 View all options by running `pytest -h` and referring to `Custom options:` section.
```

### Comparing `textology-0.0.6/README.md` & `textology-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -97,61 +97,66 @@
 developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
 ```shell
 pip install textology[full-dev]
 ```
 
 ### Extended Applications
 
-Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
-extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
+Textology app classes, such as `ExtendedApp`, can replace any regular Textual App, and be used as is without any
+extensions turned on. Here is an example of the most commonly used application subclass, `ExtendedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
+
 ```python
-from textology.apps import ObservedApp
+from textology.apps import ExtendedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-app = ObservedApp(
+app = ExtendedApp(
     layout=Container(
         Button("Ping", id="ping-btn"),
         Button("Pong", id="pong-btn"),
         Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
+
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
 
+
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def pong(clicks):
     return Label(f"Pong pressed {clicks}")
 
+
 @app.when(
     Modified("sing-btn", "n_clicks"),
     Select("ping-btn", "n_clicks"),
     Select("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def song(song_clicks, ping_clicks, pong_clicks):
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
+
 app.run()
 ```
 
 - Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
@@ -159,23 +164,32 @@
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
 
+- Callbacks can also catch Exceptions from other callbacks:
+```python
+@app.when(
+    Raised(Exception),
+)
+def error_notification(error):
+    app.notify(f"An unknown error occurred: {error}", title="Error")
+```
+
 - <details>
   <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update
     from textology.widgets import Button, Container, Label
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Container(
             Button("Ping", id="ping-btn"),
             Button("Pong", id="pong-btn"),
             Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
@@ -211,15 +225,15 @@
     ```
 
 
 - <details>
   <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update, when
     from textology.widgets import Button, Container, Label
     
     
     class Page(Container):
         def compose(self):
             yield Button("Ping", id="ping-btn")
@@ -251,15 +265,15 @@
         )
         def song(self, event, ping_clicks, pong_clicks):
             if not ping_clicks or not pong_clicks:
                 return Label(f"Press Ping and Pong first to complete the song!")
             return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
     
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Page()
     )
     
     app.run()
     ```
 
 
@@ -383,12 +397,12 @@
 
 @pytest.mark.asyncio
 async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
-- Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
+- Ability to pass an App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
 
 View all options by running `pytest -h` and referring to `Custom options:` section.
```

### Comparing `textology-0.0.6/setup.cfg` & `textology-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/setup.py` & `textology-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/apps.py` & `textology-0.2.0/textology/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 """Custom textual Apps with textology extensions included."""
 
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from inspect import isawaitable
+from types import ModuleType
 from typing import Any
 from typing import Callable
 
 from textual import events
 from textual.app import App
 from textual.app import ComposeResult
 from textual.app import CSSPathType
-from textual.containers import Container
 from textual.css.query import NoMatches
 from textual.driver import Driver
 from textual.widget import Widget
 
+from .observers import Modified
 from .observers import ObserverManager
+from .observers import Select
+from .observers import Update
+from .pages import _GLOBAL_PAGE_MAP
+from .pages import Page
+from .pages import register_page
+from .router import Endpoint
+from .router import Request
+from .widgets import Container
+from .widgets import Label
 from .widgets import Location
+from .widgets import PageContainer
 
+_DEFAULT_CONTENT_ID = "content"
+_DEFAULT_URL_ID = "url"
 
-class WidgetApp(App):
+
+class LayoutApp(App):
     """Application with a single widget for the root layout."""
 
     def __init__(
         self,
         layout: Callable | Widget | None = None,
         driver_class: type[Driver] | None = None,
         css_path: CSSPathType | None = None,
@@ -46,161 +60,92 @@
             CssPathError: When the supplied CSS path(s) are an unexpected type.
         """
         super().__init__(
             driver_class=driver_class,
             css_path=css_path,
             watch_css=watch_css,
         )
-        self.layout = layout or self.default_layout
+        if not layout:
+            layout = Container(id=_DEFAULT_CONTENT_ID)
+        else:
+            layout = layout() if isinstance(layout, Callable) else layout
+        self.layout = layout
 
     def compose(self) -> ComposeResult:
         """Default compose with provided layout.
 
         Yields:
             Layout widget set on instantiation.
         """
-        yield self.layout if not isinstance(self.layout, Callable) else self.layout()
-
-    def default_layout(self) -> Widget:
-        """Default layout generator if a layout was not provided during initialization."""
-        return Container(id="content-window")
-
-
-class BrowserApp(WidgetApp):
-    """Application capable of routing user requests, and tracking browsing history."""
-
-    def __init__(
-        self,
-        layout: Callable | Widget | None = None,
-        driver_class: type[Driver] | None = None,
-        css_path: CSSPathType | None = None,
-        watch_css: bool = False,
-    ) -> None:
-        """Initialize an application with a browser history and router.
-
-        Args:
-            layout: Primary content widget, or function to create primary content widget.
-                Must contain Location widget.
-            driver_class: Driver class or `None` to auto-detect.
-                This will be used by some Textual tools.
-            css_path: Path to CSS or `None` to use the `CSS_PATH` class variable.
-                To load multiple CSS files, pass a list of strings or paths which will be loaded in order.
-            watch_css: Reload CSS if the files changed.
-                This is set automatically if you are using `textual run` with the `dev` switch.
-
-        Raises:
-            CssPathError: When the supplied CSS path(s) are an unexpected type.
-        """
-        if layout is None:
-            layout = Container(
-                Location(),
-                Container(id="content-window"),
-            )
-        elif isinstance(layout, Callable):
-            layout = layout()
-
-        if isinstance(layout, Location):
-            location = layout
-        else:
-            location = None
-            for node in layout.walk_children():
-                if isinstance(node, Location):
-                    location = node
-                    break
-        if not location:
-            raise ValueError("Layout must contain a Location object for routing requests")
-        super().__init__(
-            layout=layout,
-            driver_class=driver_class,
-            css_path=css_path,
-            watch_css=watch_css,
-        )
-        self.location = location
-
-    def back(self) -> int:
-        """Go back one URL in the browser history.
-
-        Returns:
-            The new index in the history.
-        """
-        return self.location.back()
-
-    def forward(self) -> int:
-        """Go forward one URL in the browser history.
-
-        Returns:
-            The new index in the history.
-        """
-        return self.location.forward()
-
-    def get(self, url: str) -> Any:
-        """Run a basic GET request against the browser.
-
-        URL and history in browser are be updated.
-
-        Args:
-            url: Path to request.
-
-        Returns:
-            The result of handling the request.
-        """
-        return self.location.get(url)
-
-    def reload(self) -> None:
-        """Reload the most recent URL in the browser history."""
-        self.location.reload()
-
-    def route(self, path: str, methods: list[str] = ("GET",)) -> Callable:
-        """Create a decorator that will register a path/method combination to a request callback on the browser.
+        yield self.layout
 
-        Args:
-            path: Resource location that the decorated function will be allowed to respond to.
-            methods: One or more methods that the decorated function will be allowed to respond to at the given path.
 
-        Returns:
-            A decorator that will register a function as capable of accepting requests to a specific path/method combo.
-        """
-        return self.location.route(path, methods=methods)
+class ExtendedApp(LayoutApp, ObserverManager):
+    """Textual application with multiple Textology extensions for automating UI updates.
 
+    Additional functionality:
+        - Automatic input/output callbacks for managing application state via ".when()" registration.
+        - URL based multi-page content via ".register_page()".
+        - URL routing for resource requests within the application via ".location.get()".
+        - URL history for navigating via ".back()", ".forward()", etc.
+    """
 
-class ObservedApp(WidgetApp, ObserverManager):
-    """Application capable of performing automatic input/output callbacks on reactive widget property updates."""
-
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         layout: Callable | Widget | None = None,
+        use_pages: bool = False,
+        pages: list[Page | ModuleType | str | Callable] | None = None,
         driver_class: type[Driver] | None = None,
         css_path: CSSPathType | None = None,
         watch_css: bool = False,
         logger: logging.Logger | None = None,
     ) -> None:
         """Initialize an application with tracking for input/output callbacks.
 
         Args:
             layout: Primary content widget, or function to create primary content widget.
+            use_pages: Whether to enable multi-page application support.
+                When enabled, this will include automatic URL routing callbacks via "widgets.Location".
+                Force enabled if "pages" are provided. Enabling without "pages" allows registering pages later.
+            pages: Initial pages to load into multi-page applications.
+                Refer to "register_page()" for options.
             driver_class: Driver class or `None` to auto-detect.
                 This will be used by some Textual tools.
             css_path: Path to CSS or `None` to use the `CSS_PATH` class variable.
                 To load multiple CSS files, pass a list of strings or paths which will be loaded in order.
             watch_css: Reload CSS if the files changed.
                 This is set automatically if you are using `textual run` with the `dev` switch.
             logger: Custom logger to send callback messages to.
 
         Raises:
             CssPathError: When the supplied CSS path(s) are an unexpected type.
         """
+        layout = layout or Container(
+            Location(id=_DEFAULT_URL_ID),
+            Container(id=_DEFAULT_CONTENT_ID) if not use_pages else PageContainer(id=_DEFAULT_CONTENT_ID),
+        )
         super().__init__(
             layout=layout,
             driver_class=driver_class,
             css_path=css_path,
             watch_css=watch_css,
         )
         # Manually set up observer manager mixin since App inheritance does not automatically trigger.
         ObserverManager.__init__(self, logger=logger or logging.root)
+        self.attach_to_observers(self)
+
         self._observer_message_handler_map = {}
+        self._location: Location | None = None
+        self._page_registry: dict[str, Page] = {}
+        self._use_pages = use_pages or bool(pages)
+
+        self.enable_pages()
+        if pages:
+            for page in pages:
+                self.register_page(page)
 
     def apply_update(
         self,
         observer_id: str,
         component: Widget,
         component_id: str,
         component_property: str,
@@ -216,21 +161,75 @@
                 component.mount_all(value)
         elif component_property == "screen":
             # Screen is a special property on applications, it cannot be directly applied. Manually add to stack.
             component.app.push_screen(value)
         else:
             super().apply_update(observer_id, component, component_id, component_property, value)
 
+    def back(self) -> int:
+        """Go back one URL in the history.
+
+        Returns:
+            The new index in the history.
+        """
+        return self.location.back()
+
+    def enable_pages(self) -> None:
+        """Set up multi-page application routing."""
+        if not self._use_pages:
+            return
+
+        location = self.location
+        if not location:
+            raise ValueError("Layout must contain a Location widget if pages are enabled")
+        if not location.id:
+            raise ValueError("Location widget must have an id if pages are enabled")
+
+        page_container = None
+        for node in self.layout.walk_children():
+            if isinstance(node, PageContainer):
+                page_container = node
+                break
+        if page_container is None:
+            raise ValueError("Layout must contain a PageContainer widget if pages are enabled")
+        if not page_container.id:
+            raise ValueError("PageContainer widget must have an id if pages are enabled")
+
+        # Finish final set up after all validations are performed to ensure page routing is supported.
+        self.when(
+            Modified(location.id, "pathname"),
+            Select(location.id, "search"),
+            Update(page_container.id, "children"),
+        )(self._page_router)
+        self.location.endpoint_not_found = Endpoint([], "", self._page_not_found)
+        for page in _GLOBAL_PAGE_MAP.values():
+            self.register_page(page)
+
+    def forward(self) -> int:
+        """Go forward one URL in the history.
+
+        Returns:
+            The new index in the history.
+        """
+        return self.location.forward()
+
     def get_component(self, component_id: str) -> Any:
         """Fina a component in the DOM."""
         try:
             return self.query_one(f"#{component_id}")
         except NoMatches:
             return None
 
+    @property
+    def location(self) -> Location | None:
+        """Find the application's primary Location widget for routing addresses."""
+        if self._location is None:
+            self._update_location()
+        return self._location
+
     async def _on_message(self, message: events.Message) -> None:
         """Process messages after sending to registered observers first."""
         control = message.control
         if control:
             controller_id = control.id
             if controller_id:
                 cls = message.__class__
@@ -262,15 +261,51 @@
                         self._observer_message_handler_map.setdefault(f"{widget_id}@{property_id}", []).append(
                             self._generate_callback(
                                 widget_id,
                                 property_id,
                                 observer,
                             )
                         )
-        self.attach_to_observers(self)
+
+    def _page_not_found(
+        self,
+        request: Request,
+    ) -> Label:
+        """Default handler for when a request is made to a page that is not available."""
+        self.logger.warning(f"Page not found {request.url.path}")
+        return Label("Page not found")
+
+    def page_registry(self) -> dict:
+        """Provide the combined page registry in use by this multi-page application."""
+        return self._page_registry
+
+    def _page_router(self, pathname: str, search: str) -> list[Widget]:
+        """Load the appropriate page based on the URL path and search options."""
+        self.logger.debug(f"Routing page content for: {pathname}")
+
+        # Simulate router "serve()" to allow error handling at the callback level instead of router/widget level.
+        request = Request(pathname if not search else f"{pathname}?{search}")
+        path = request.url.path
+        endpoint = self.location.endpoint(path, "GET")
+
+        # Create kwargs for the layout function based off of:
+        #   - App if requested, to avoid circular imports if needed.
+        #   - Original request object if requested by name, to allow full access to URL values.
+        #   - Inline path variables if path is a dynamic route.
+        #   - User search/query variables.
+        kwargs = {}
+        if "app" in endpoint.handler_vars:
+            kwargs["app"] = self
+        if "request" in endpoint.handler_vars:
+            kwargs["request"] = request
+        if not endpoint.route.static:
+            kwargs.update(**endpoint.route.match_groups(path))
+        kwargs.update(request.query)
+
+        return endpoint.handler(**kwargs)
 
     def _register_reactive_observers(self, widget: Widget) -> None:
         """Enable observers for a newly added widget and its reactive attributes if it has an ID."""
         # Do not watch any widgets or properties for changes that have not had an observer set up.
         widget_id = widget.id
         if not widget_id or (widget_id not in self._observer_map and widget_id not in self._observer_map_global):
             return
@@ -279,14 +314,73 @@
                 property_name not in self._observer_map[widget_id]
                 and property_name not in self._observer_map_global[widget_id]
             ):
                 continue
             for callback in self.generate_callbacks(widget_id, property_name):
                 self.watch(widget, property_name, callback, init=False)
 
+    def register_page(
+        self,
+        page: Page | ModuleType | str | Callable | None = None,
+        path: str | None = None,
+        redirect_from: str | list[str] | None = None,
+        layout: Callable | None = None,
+    ) -> None:
+        """Register a URL path to a layout in this multi-page application.
+
+        Args:
+            page: A module, or module path, where the remaining page's variables are defined.
+                e.g. If calling from within the module itself: "__name__"
+                e.g. If calling from another module: "mylib.home"
+            path: URL Path, with or without variables. e.g. "/", "/home", "/documents/{document_name}"
+                Inferred from the "module" or "layout" if not provided.
+                    e.g. "mylib.home" -> "/home"
+                    e.g. "layout_home_page" -> "/home_page"
+                Variables marked as {variable_name} in paths will be passed to "layout" as keyword arguments.
+            redirect_from: Paths that should redirect to this page's path. e.g. "/v1/home"
+            layout: Function to call to generate the widget(s) used in the page's layout.
+        """
+        if not self._use_pages:
+            raise ValueError("Pages are not enabled on this application")
+        page = register_page(
+            page=page,
+            path=path,
+            redirect_from=redirect_from,
+            layout=layout,
+            page_map=self._page_registry,
+        )
+        if page.path in ("/404", "/not_found", "/not_found_404"):
+            # This is a special page that is not directly routed; it is used on every invalid path request.
+            self.location.endpoint_not_found = Endpoint([], "", page.layout)
+        else:
+            self.route(page.path)(page.layout)
+
+    def reload(self) -> None:
+        """Reload the most recent URL in the history."""
+        self.location.reload()
+
+    def route(self, path: str, methods: list[str] = ("GET",)) -> Callable:
+        """Create a decorator that will register a path/method combination to a request callback.
+
+        Args:
+            path: Resource location that the decorated function will be allowed to respond to.
+            methods: One or more methods that the decorated function will be allowed to respond to at the given path.
+
+        Returns:
+            A decorator that will register a function as capable of accepting requests to a specific path/method combo.
+        """
+        return self.location.route(path, methods=methods)
+
+    def _update_location(self) -> None:
+        """Walk the layout tree to allow finding the application's Location widget at any point in the lifecycle."""
+        for node in self.layout.walk_children():
+            if isinstance(node, Location):
+                self._location = node
+                break
+
 
 def _post_mount_patch(self: Widget) -> None:
     """Called after the object has been mounted, regardless of mount event, to register observer support."""
     # Call the original function being patched to ensure the widget is fully set up before registering.
     _widget_post_mount(self)
     attach_to_observers = getattr(self.app, "attach_to_observers", None)
     if attach_to_observers:
```

### Comparing `textology-0.0.6/textology/history.py` & `textology-0.2.0/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/observers/__init__.py` & `textology-0.2.0/textology/observers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Utilities for routing component input/output requests via observation callbacks."""
 
 from ._dependencies import Dependency
 from ._dependencies import Modified
 from ._dependencies import NoUpdate
 from ._dependencies import Published
+from ._dependencies import Raised
 from ._dependencies import Select
 from ._dependencies import SupportsID
 from ._dependencies import Update
 from ._dependencies import flatten_dependencies
+from ._dependencies import no_update
 from ._exceptions import ObserverException
 from ._exceptions import PreventUpdate
 from ._exceptions import UnknownObserver
 from ._managers import WHEN_DECORATOR
 from ._managers import ObservedObject
 from ._managers import ObservedValue
 from ._managers import Observer
```

### Comparing `textology-0.0.6/textology/observers/_managers.py` & `textology-0.2.0/textology/observers/_managers.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,38 @@
 import traceback
 import weakref
 from collections import defaultdict
 from inspect import isawaitable
 from typing import Any
 from typing import Callable
 from typing import Coroutine
+from typing import Generator
 
 from textology.logging import NullLogger
 
 from ._dependencies import Dependency
+from ._dependencies import DependencyType
 from ._dependencies import Modified
 from ._dependencies import NoUpdate
 from ._dependencies import Published
+from ._dependencies import Raised
 from ._dependencies import Select
 from ._dependencies import Update
 from ._dependencies import flatten_dependencies
+from ._dependencies import no_update
+from ._dependencies import validate_dependencies
 from ._exceptions import PreventUpdate
 from ._exceptions import UnknownObserver
 
+UpdateResultType = dict[str, dict[str, Any]]
+
 # Type alias to represent function receiving 2 arguments (old value and new value) and returning nothing.
 ValueUpdateHandler = Callable[[Any, Any], Coroutine]
 
+_GLOBAL_OBSERVER_EXC_MAP: dict[type[Exception], list[Observer]] = defaultdict(list)
 _GLOBAL_OBSERVER_ID_MAP: dict[str, Observer] = {}
 _GLOBAL_OBSERVER_MAP: dict[str, dict[str, list[Observer]]] = defaultdict(lambda: defaultdict(list))
 
 WHEN_DECORATOR = "_textology_when"
 
 
 class Observer:
@@ -41,60 +49,57 @@
     External callbacks should be considered stateless: they should not store or request any
     variables created during previous callbacks, and should only rely on the arguments they provide.
     To share data across external callbacks, use an external storage type such as a database.
     """
 
     def __init__(
         self,
-        publications: list[Published],
-        modifications: list[Modified],
-        selections: list[Select],
-        updates: list[Update],
+        dependencies: dict[type[Dependency], list[Dependency]],
         func: Callable = False,
+        external: bool = False,
     ) -> None:
         """Initialize specifications for observing values.
 
         Args:
-            publications: Component IDs and published event types that provide arguments and trigger the callback.
-            modifications: Component IDs and properties that provide arguments and trigger the callback.
-            selections: Component IDs and properties that provide additional arguments without triggering the callback.
-            updates: Component IDs and properties to update based on the results of the callback.
+            dependencies: Dependencies used to monitor for triggers and results of the callback.
             func: The function to call with input values when triggered.
                 Indirectly called via "callback()" when triggered.
+            external: Whether the callback is handled locally, or sent to an external handler.
         """
-        observer_id = (
-            "..".join(f"{dep.component_id}@{dep.component_property}" for dep in publications + modifications)
-            + "..."
-            + "..".join(f"{dep.component_id}@{dep.component_property}" for dep in updates)
-        )
+        self._dependencies: dict[type[Dependency], list[DependencyType]] = dependencies or {}
+        for dependency_type in (Modified, Published, Raised, Select, Update):
+            self._dependencies.setdefault(dependency_type, [])
         self._method_ref: weakref.ReferenceType | None = None
-        self.observer_id = observer_id
-        self.publications = publications
-        self.modifications = modifications
-        self.selections = selections
-        self.updates = updates
-        self.external = False
+        self.external = external
         self.func = func
+        self._callback_arguments = self.publications + self.modifications + self.selections
+        inputs = self.publications + self.modifications + self.raises + self.selections
+        outputs = self.updates
+        self.id = (
+            "+".join(f"{dep.component_id}@{dep.component_property}" for dep in inputs)
+            + "->"
+            + "+".join(f"{dep.component_id}@{dep.component_property}" for dep in outputs)
+        )
+
+        # If the function is not a method (object pre-attached), then tag it in case an object needs to be added.
+        # Tagged functions can be searched later, such as during object init, to convert the callback into a method.
+        if type(func).__name__ != "method":
+            if not hasattr(func, WHEN_DECORATOR):
+                setattr(func, WHEN_DECORATOR, [])
+            getattr(func, WHEN_DECORATOR).append(self)
 
     def __hash__(self) -> int:
         """Convert object into hash usable in maps."""
         return hash(str(self))
 
     def __repr__(self) -> str:
         """Convert object into human-readable, machine loadable, text."""
-        return (
-            f"{self.__class__.__name__}("
-            f"'{self.publications}',"
-            f" {self.modifications},"
-            f" {self.selections},"
-            f" {self.updates},"
-            f"external={self.external})"
-        )
+        return f"{self.__class__.__name__}({self._dependencies})"
 
-    async def callback(self, *args: Any, **kwargs: Any) -> dict[str, dict[str, Any]] | None:
+    async def callback(self, *args: Any, **kwargs: Any) -> UpdateResultType | None:
         """Call the original function with additional callback management, such as conversion to standardized results.
 
         Args:
             args: Original positional arguments for function.
             kwargs: Original keyword arguments for function.
 
         Returns:
@@ -104,65 +109,96 @@
         if self._method_ref:
             ref = self._method_ref()
             if ref:
                 func = func.__get__(ref)  # Required to access the method. pylint: disable=unnecessary-dunder-call
         results = func(*args, **kwargs)  # Invoke original callback.
         results = await results if isawaitable(results) else results
 
-        if results is NoUpdate or isinstance(results, NoUpdate) or not self.updates:
+        if isinstance(results, NoUpdate) or not self.updates:
             return None
 
         if len(self.updates) == 1:
             results = [results]
 
         component_updates = defaultdict(dict)
         has_update = False
         for update_val, update in zip(results, self.updates):
-            if update_val is NoUpdate or isinstance(update_val, NoUpdate):
+            if isinstance(update_val, NoUpdate):
                 continue
             has_update = True
             component_updates[update.component_id][update.component_property] = update_val
 
         if not has_update:
             return None
 
         return component_updates
 
+    @property
+    def callback_arguments(self) -> list[Published | Modified | Select]:
+        """Component IDs and properties, or types, that provide arguments to the callback."""
+        return self._callback_arguments
+
+    @property
+    def modifications(self) -> list[Modified]:
+        """Component IDs and properties that provide arguments and trigger the callback."""
+        return self._dependencies[Modified]
+
+    @property
+    def publications(self) -> list[Published]:
+        """Component IDs and published event types that provide arguments and trigger the callback."""
+        return self._dependencies[Published]
+
+    @property
+    def raises(self) -> list[Raised]:
+        """Exception types that provide arguments and trigger the callback when an exception is raised."""
+        return self._dependencies[Raised]
+
+    @property
+    def selections(self) -> list[Select]:
+        """Component IDs and properties that provide additional arguments without triggering the callback."""
+        return self._dependencies[Select]
+
     def update_method_ref(self, obj: Any) -> None:
         """Update the weak reference used when the callback is a method.
 
         Args:
             obj: Object to store a new weak reference for, and use during callbacks.
         """
         self._method_ref = weakref.ref(obj)
 
+    @property
+    def updates(self) -> list[Update]:
+        """Component IDs and properties for output of a callback that will be updated after triggering."""
+        return self._dependencies[Update]
+
 
 class ObserverManager:
     """Register and execute input/output callbacks when observed properties change.
 
     Can be used directly as a nested object within an application, or as a "mixin" for an application class. Example:
         manager = ObserverManager() # Or:
-        class ObservedApp(ObserverManager):
+        class ObservedApp(BaseAppClass, ObserverManager):
             ...
         app = ObservedApp()
     """
 
     def __init__(
         self,
         logger: logging.Logger | None = None,
     ) -> None:
         """Initialize observation trackers and handlers.
 
         Args:
             logger: Custom logger to send messages to.
         """
         super().__init__()
-        self._observer_id_map = {}
-        # Structured as: _observer_map[component_id][component_property] = Observer
-        self._observer_map = defaultdict(lambda: defaultdict(list))
+        self._observer_exc_map: dict[type[Exception], list[Observer]] = defaultdict(list)
+        self._observer_id_map: dict[str, Observer] = {}
+        # Structured as: _observer_map[component_id][component_property] = Observers
+        self._observer_map: dict[str, dict[str, list[Observer]]] = defaultdict(lambda: defaultdict(list))
         self.logger: logging.Logger | None = logger or NullLogger(__name__)
 
     def apply_update(  # Pass all component arguments to allow subclasses to use. pylint: disable=unused-argument
         self,
         observer_id: str,
         component: Any,
         component_id: str,
@@ -192,63 +228,62 @@
         for value in obj.__class__.__dict__.values():
             if callable(value):
                 observers = getattr(value, WHEN_DECORATOR, None)
                 if observers:
                     for observer in observers:
                         observer.update_method_ref(obj)
 
-    def _generate_callback(self, trigger_id: str, modified_property: str, observer: Observer) -> ValueUpdateHandler:
+    def _generate_callback(self, trigger_id: str, trigger_property: str, observer: Observer) -> ValueUpdateHandler:
         """Create a callback wrapper that will call the original function with input/output management applied."""
 
         async def _on_update(old_value: Any, new_value: Any) -> None:
             """Process value changes for a component property and apply the requested update operations."""
             update_components = self._get_update_components(observer)
             if observer.updates and not update_components:
-                # One or more components missing, do not trigger callback.
+                # One or more components are not in the current component tree, do not trigger callback.
+                return
+            callback_components = self._get_callback_components(observer)
+            if not callback_components:
+                # One or more components are not in the current component tree, do not trigger callback.
+                return
+            args = self._get_callback_args(
+                observer,
+                callback_components,
+                trigger_id,
+                trigger_property,
+                old_value,
+                new_value,
+            )
+            if isinstance(args, NoUpdate):
+                # Failed to request one or more component properties, do not continue.
                 return
-            observer_id = observer.observer_id
-            args = []
-            for dep in observer.publications + observer.modifications + observer.selections:
-                if isinstance(dep, Published):
-                    # Published events are stateless; they are not available if they are not the trigger.
-                    # Fill events, other than the triggering event, with empty values.
-                    args.append(new_value if dep.component_id == trigger_id else None)
-                elif dep.component_id == trigger_id and dep.component_property == modified_property:
-                    # Properties are stateful; they are available at all times.
-                    # Use new value if this was the trigger, otherwise use historical value to represent "current" state.
-                    args.append(old_value if isinstance(dep, Select) else new_value)
-                else:
-                    try:
-                        args.append(
-                            self.get_callback_arg(observer.observer_id, dep.component_id, dep.component_property)
-                        )
-                    except Exception as error:  # pylint: disable=broad-exception-caught
-                        self.on_callback_error(observer_id, error)
-                        return
 
             try:
-                updates = observer.callback(*args) if not observer.external else self.send_callback(observer_id, *args)
+                updates = observer.callback(*args) if not observer.external else self.send_callback(observer.id, *args)
                 updates = await updates if isawaitable(updates) else updates
             except PreventUpdate:
                 updates = None
             except BaseException as error:  # pylint: disable=broad-exception-caught
                 # Catch all errors to prevent fatal crashes in application callback loops.
-                self.on_callback_error(observer_id, error)
+                # All error updates will be handled separately, as the components will not be the same.
                 updates = None
+                if not await self._on_update_error(error):
+                    # Send error to the default handler, nothing else was set up to capture.
+                    self.on_callback_error(observer.id, error)
 
-            if updates:
-                try:
-                    for update_id, properties in updates.items():
-                        for update_property, value in properties.items():
-                            self.apply_update(
-                                observer_id, update_components[update_id], update_id, update_property, value
-                            )
-                except BaseException as error:  # pylint: disable=broad-exception-caught
-                    # Catch all errors to prevent fatal crashes in application callback loops.
-                    self.on_callback_error(observer_id, error)
+            if not updates:
+                # There are no update types, updates were requested to be skipped, or generating updates failed.
+                return
+
+            try:
+                for comp_id, comp_property, value in _iter_updates(updates):
+                    self.apply_update(observer.id, update_components[comp_id], comp_id, comp_property, value)
+            except BaseException as error:  # pylint: disable=broad-exception-caught
+                # Catch all errors to prevent fatal crashes in application callback loops.
+                self.on_callback_error(observer.id, error)
 
         return _on_update
 
     def generate_callbacks(self, component_id: str, component_property: str) -> list[ValueUpdateHandler]:
         """Create callbacks that will manage input/output operations for all functions registered to id/property combo.
 
         Args:
@@ -263,55 +298,88 @@
             callbacks.append(self._generate_callback(component_id, component_property, observer))
         for observer in self._observer_map[component_id][component_property]:
             callbacks.append(self._generate_callback(component_id, component_property, observer))
         return callbacks
 
     def get_callback_arg(
         self,
-        observer_id: str,
-        component_id: str,
-        component_property: str,
+        component: Any,
+        property_name: str,
     ) -> Any:
         """Find a value from a component to be passed to a callback.
 
         Default behavior is a standard attribute request. Override to provide more complex request to properties.
 
         Args:
-            observer_id: ID of the observer that triggered.
-            component_id: ID of the component that contains the requested property.
-            component_property: Property name on the component that is being requested.
+            component: Component with properties usable in a callback.
+            property_name: Name of the property on the component that is being requested.
 
         Returns:
             The property value from the requested component.
         """
-        component = self.get_component(component_id)
-        if not component:
-            raise PreventUpdate(f"Skipping callback for {observer_id}: Component {component_id} not available")
-        return getattr(component, component_property)
+        return getattr(component, property_name)
+
+    def _get_callback_args(  # pylint: disable=too-many-arguments
+        self,
+        observer: Observer,
+        components: dict,
+        trigger_id: str | None,
+        trigger_property: str | None,
+        old_value: Any,
+        new_value: Any,
+    ) -> list | NoUpdate:
+        """Find all arguments from components that will be used by a callback."""
+        args = []
+        for dep in observer.callback_arguments:
+            if isinstance(dep, Published):
+                # Published events are stateless; they are not available if they are not the trigger.
+                # Fill events, other than the triggering event, with empty values.
+                args.append(new_value if dep.component_id == trigger_id else None)
+            elif dep.component_id == trigger_id and dep.component_property == trigger_property:
+                # Properties are stateful; they are available at all times.
+                # Use new value if this was the trigger, otherwise use historical value to represent "current" state.
+                args.append(old_value if isinstance(dep, Select) else new_value)
+            else:
+                try:
+                    args.append(self.get_callback_arg(components[dep.component_id], dep.component_property))
+                except Exception as error:  # pylint: disable=broad-exception-caught
+                    self.on_callback_error(observer.id, error)
+                    return no_update
+        return args
+
+    def _get_callback_components(self, observer: Observer) -> dict[str, Any] | None:
+        """Find all components that will be used as arguments by a callback."""
+        output_components = {}
+        for dep in observer.callback_arguments:
+            component = self.get_component(dep.component_id)
+            if not component:
+                return None
+            output_components[dep.component_id] = component
+        return output_components
 
     @abc.abstractmethod
     def get_component(self, component_id: str) -> Any:
         """Fina a component for use in a callback.
 
         Args:
             component_id: ID of the component being requested.
 
         Returns:
             Component with properties usable in a callback.
         """
 
     def _get_update_components(self, observer: Observer) -> dict[str, Any] | None:
         """Find all components that will be updated by a callback."""
-        output_components = {}
+        components = {}
         for dep in observer.updates:
             component = self.get_component(dep.component_id)
             if not component:
                 return None
-            output_components[dep.component_id] = component
-        return output_components
+            components[dep.component_id] = component
+        return components
 
     @property
     def _observer_id_map_global(self) -> dict[str, Observer]:
         """Return the global observer ID map used across all managers.
 
         The global observer ID map is populated when functions are decorated at the class or module level.
         """
@@ -339,15 +407,76 @@
             # Unhandled fatal error; reraise.
             raise error
         # Not all third party loggers have ".exception()" to print stacktraces, collect manually and use error.
         full_trace = traceback.format_exc()
         # Standard error, log and continue.
         self.logger.error(f"Failed callback for {observer_id}: {type(error).__name__} {error}\n{full_trace}")
 
-    def send_callback(self, observer_id: str, *callback_args: Any) -> dict[str, dict[str, Any]]:
+    async def _on_update_error(self, error: BaseException) -> bool:
+        """Handle callback exception raises and apply the requested update operations."""
+        handlers = None
+        handled = False
+        for exc_type in error.__class__.__mro__[:-1]:
+            # Stop on the first match for the class, this will be the best match (most specific) for the type.
+            if handlers := self._observer_exc_map.get(exc_type):
+                break
+
+        if not handlers:
+            return handled
+
+        for observer in handlers:
+            update_components = self._get_update_components(observer)
+            if observer.updates and not update_components:
+                # One or more components are not in the current component tree, do not trigger callback.
+                continue
+            callback_components = self._get_callback_components(observer)
+            if observer.callback_arguments and not callback_components:
+                # One or more components are not in the current component tree, do not trigger callback.
+                continue
+            args = self._get_callback_args(
+                observer,
+                callback_components,
+                None,
+                None,
+                None,
+                None,
+            )
+            if isinstance(args, NoUpdate):
+                # Failed to request one or more component properties, do not continue.
+                continue
+
+            try:
+                updates = (
+                    observer.callback(error, *args)
+                    if not observer.external
+                    else self.send_callback(
+                        observer.id,
+                        error,
+                        *args,
+                    )
+                )
+                updates = await updates if isawaitable(updates) else updates
+
+                if not updates:
+                    if not update_components:
+                        # No updates were expected, consider the exception handled by the callback.
+                        handled = True
+                    continue
+
+                for comp_id, comp_property, value in _iter_updates(updates):
+                    self.apply_update(observer.id, update_components[comp_id], comp_id, comp_property, value)
+                    handled = True
+            except PreventUpdate:
+                pass
+            except BaseException as new_error:  # pylint: disable=broad-exception-caught
+                # Catch all errors to prevent fatal crashes in application callback loops.
+                self.on_callback_error(observer.id, new_error)
+        return handled
+
+    async def send_callback(self, observer_id: str, *callback_args: Any) -> dict[str, dict[str, Any]]:
         """Forward a callback request to be handled externally.
 
         Override to send the request to an external endpoint, and wait for the response.
         Any callbacks handled externally should be considered stateless: they should not store or request any
         variables created during a previous callback, and should only rely on the callback arguments they provide.
 
         Args:
@@ -360,40 +489,41 @@
         # Default behavior directly forwards to the callback receiver (local callback). Override to send externally.
         observer = self._observer_id_map.get(observer_id)
         if not observer:
             raise UnknownObserver(f"Callback {observer_id} was requested but could not be found.")
         self.logger.warning(
             f'External callback {observer_id} is forwarding to local callback: override "send_callback" in {type(self)} or remove "external" from callback'
         )
-        return observer.callback(*callback_args)
+        return await observer.callback(*callback_args)
 
     def when(
         self,
-        *args: Dependency,
+        *dependencies: Dependency,
     ) -> Callable:
         """Register a callback that triggers when observed values change while this instance is active.
 
         Example:
             @app.when(
                 Modified('url', 'path'),
                 Update('content-wrapper', 'content'),
             )
             def route_url(path: str) -> str:
                 ...
 
         Args:
-            args: Positional arguments containing one or more observation Dependencies.
+            dependencies: Positional arguments containing one or more observation Dependencies.
 
         Returns:
             Decorator to register a function as an input/output reaction to one or more property changes.
         """
         return create_observer_register(
-            self._observer_map,
-            self._observer_id_map,
-            *args,
+            *dependencies,
+            observer_exc_map=self._observer_exc_map,
+            observer_id_map=self._observer_id_map,
+            observer_map=self._observer_map,
         )
 
 
 class ObservedObject:
     """Basic object that triggers callbacks when observed values change.
 
     Example:
@@ -459,95 +589,130 @@
             callback: Where to send old and new values on update.
         """
         self.value = value
         self.callback = callback
 
 
 def create_observer_register(
-    observer_map: dict[str, dict[str, list[Observer]]],
-    observer_id_map: dict[str, Observer],
-    *observer_args: Dependency,
-    split_publications: bool = False,
+    *dependencies: Dependency,
+    observer_exc_map: dict[type[Exception], list[Observer]] | None = None,
+    observer_id_map: dict[str, Observer] | None = None,
+    observer_map: dict[str, dict[str, list[Observer]]] | None = None,
+    split_publications: bool = True,
     split_modifications: bool = False,
+    split_raises: bool = True,
     external: bool = False,
 ) -> Callable:
     """Create a decorator that will wrap a function with additional callback management, and register the observer.
 
     Args:
-        observer_map: All currently registered observers by component ID and component property.
-            Modified in place when new observer is registered.
+        dependencies: Positional arguments containing one or more Dependencies.
+        observer_exc_map: All currently registered observers for Exception types.
+            Modified in place when observer is registered. Defaults to global exception observers shared across apps.
         observer_id_map: All currently registered observers by full observer ID.
-            Modified in place when new observer is registered.
-        observer_args: Positional arguments containing one or more Dependencies.
+            Modified in place when observer is registered. Defaults to global observers shared across apps.
+        observer_map: All currently registered observers by component ID and component property.
+            Modified in place when observer is registered. Defaults to global observers shared across apps.
         split_publications: Register the observer once per publication, instead of once per all publications.
         split_modifications: Register the observer once per modification, instead of once per all modifications.
+        split_raises: Register the observer once per exception raise type, instead of once per all raise types.
         external: Whether the callback is handled by an external endpoint, or locally.
             Any callbacks handled externally should be considered stateless: they should not store or request any
             variables created during a previous callback, and should only rely on the callback arguments they provide.
 
     Returns:
         Decorator to register a function as an input/output reaction to one or more property changes.
     """
+    validate_dependencies(*dependencies)
+
+    observer_exc_map = observer_exc_map if observer_exc_map is not None else _GLOBAL_OBSERVER_EXC_MAP
+    observer_id_map = observer_id_map if observer_id_map is not None else _GLOBAL_OBSERVER_ID_MAP
+    observer_map = observer_map if observer_map is not None else _GLOBAL_OBSERVER_MAP
 
     def _decorator(func: Callable) -> Callable:
         """Wrap the original function with additional callback management, and register the final observer."""
-        publications, modifications, selections, updates = flatten_dependencies(observer_args)
+        observers = []
+        flattened = flatten_dependencies(dependencies)
+        publications = flattened.get(Published, [])
+        modifications = flattened.get(Modified, [])
+        raises = flattened.get(Raised, [])
+        selections = flattened.get(Select, [])
+        updates = flattened.get(Update, [])
 
+        # Create all standard observers, those that are not based on exceptions will all combinations.
         # Triggers can be 1 input/argument per callback, or all per callback.
         if publications:
             publications = [[dep] for dep in publications] if split_publications else [publications]
         if modifications:
             modifications = [[dep] for dep in modifications] if split_modifications else [modifications]
-
-        observers = []
         for publication_group, modification_group in itertools.product(publications or [[]], modifications or [[]]):
             observers.append(
                 Observer(
-                    publication_group,
-                    modification_group,
-                    selections,
-                    updates,
+                    {
+                        Published: publication_group,
+                        Modified: modification_group,
+                        Select: selections,
+                        Update: updates,
+                    },
                     func=func,
+                    external=external,
                 )
             )
+
+        # Create all special exception observers with only raise types, selections, and updates.
+        if raises:
+            raises = [[dep] for dep in raises] if split_raises else [raises]
+        for raise_group in raises:
+            observers.append(
+                Observer(
+                    {
+                        Raised: raise_group,
+                        Select: selections,
+                        Update: updates,
+                    },
+                    func=func,
+                    external=external,
+                )
+            )
+
         for observer in observers:
-            observer.external = external
-            # If the function is not a method (object pre-attached), then tag it in case an object needs to be added.
-            # Tagged functions can be searched later, such as during object init, to convert the callback into a method.
-            if type(func).__name__ != "method":
-                if not hasattr(func, WHEN_DECORATOR):
-                    setattr(func, WHEN_DECORATOR, [])
-                getattr(func, WHEN_DECORATOR).append(observer)
-            observer_id_map[observer.observer_id] = observer
+            observer_id_map[observer.id] = observer
             for dep in observer.publications + observer.modifications:
                 observer_map.setdefault(dep.component_id, {}).setdefault(dep.component_property, []).append(observer)
+            for dep in observer.raises:
+                observer_exc_map.setdefault(dep.exception_type, []).append(observer)
 
         # Return the original, unmodified, function; the decorator only tags and/or maps for later usage.
         return func
 
     return _decorator
 
 
+def _iter_updates(updates: UpdateResultType) -> Generator[tuple[str, str, Any], None, None]:
+    """Iterate over the standard update multi-level format."""
+    for update_id, properties in updates.items():
+        for update_property, value in properties.items():
+            yield update_id, update_property, value
+
+
 def when(
-    *args: Dependency,
+    *dependencies: Dependency,
 ) -> Callable:
     """Register a callback that triggers when observed values change globally.
 
     Example:
         @when(
             Modified('url', 'path'),
             Update('content-wrapper', 'content'),
         )
         def route_url(path: str) -> str:
             ...
 
     Args:
-        args: Positional arguments containing one or more observation Dependencies.
+        dependencies: Positional arguments containing one or more observation Dependencies.
 
     Returns:
         Decorator to register a function as an input/output reaction to one or more property changes.
     """
     return create_observer_register(
-        _GLOBAL_OBSERVER_MAP,
-        _GLOBAL_OBSERVER_ID_MAP,
-        *args,
+        *dependencies,
     )
```

### Comparing `textology-0.0.6/textology/pytest_utils.py` & `textology-0.2.0/textology/pytest_utils.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/router.py` & `textology-0.2.0/textology/router.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/__init__.py` & `textology-0.2.0/textology/widgets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 any extension functionality is used. All Textual basic widgets should be 100% forward compatible with Textology widgets,
 and all Textology widgets should be 100% backwards compatible with Textual widgets, in settings where no extended
 functionality is being used.
 """
 
 from ._button import Button
 from ._containers import Container
+from ._containers import PageContainer
 from ._extensions import Clickable
 from ._extensions import ExtendedWidget
 from ._extensions import WidgetExtension
 from ._horizontal_menus import HorizontalMenus
 from ._label import Label
 from ._list_item import LIST_ITEM_EVENT_IGNORES
 from ._list_item import ListItem
```

### Comparing `textology-0.0.6/textology/widgets/_button.py` & `textology-0.2.0/textology/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_extensions.py` & `textology-0.2.0/textology/widgets/_extensions.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_horizontal_menus.py` & `textology-0.2.0/textology/widgets/_horizontal_menus.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_label.py` & `textology-0.2.0/textology/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_list_item.py` & `textology-0.2.0/textology/widgets/_list_item.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_list_item_header.py` & `textology-0.2.0/textology/widgets/_list_item_header.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_list_item_meta.py` & `textology-0.2.0/textology/widgets/_list_item_meta.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_list_view.py` & `textology-0.2.0/textology/widgets/_list_view.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_location.py` & `textology-0.2.0/textology/widgets/_location.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_modal_dialog.py` & `textology-0.2.0/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_static.py` & `textology-0.2.0/textology/widgets/_static.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology/widgets/_store.py` & `textology-0.2.0/textology/widgets/_store.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.6/textology.egg-info/PKG-INFO` & `textology-0.2.0/textology.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.0.6
+Version: 0.2.0
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -132,61 +132,66 @@
 developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
 ```shell
 pip install textology[full-dev]
 ```
 
 ### Extended Applications
 
-Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
-extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
+Textology app classes, such as `ExtendedApp`, can replace any regular Textual App, and be used as is without any
+extensions turned on. Here is an example of the most commonly used application subclass, `ExtendedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
+
 ```python
-from textology.apps import ObservedApp
+from textology.apps import ExtendedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-app = ObservedApp(
+app = ExtendedApp(
     layout=Container(
         Button("Ping", id="ping-btn"),
         Button("Pong", id="pong-btn"),
         Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
+
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
 
+
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def pong(clicks):
     return Label(f"Pong pressed {clicks}")
 
+
 @app.when(
     Modified("sing-btn", "n_clicks"),
     Select("ping-btn", "n_clicks"),
     Select("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 def song(song_clicks, ping_clicks, pong_clicks):
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
+
 app.run()
 ```
 
 - Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
@@ -194,23 +199,32 @@
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
 
+- Callbacks can also catch Exceptions from other callbacks:
+```python
+@app.when(
+    Raised(Exception),
+)
+def error_notification(error):
+    app.notify(f"An unknown error occurred: {error}", title="Error")
+```
+
 - <details>
   <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update
     from textology.widgets import Button, Container, Label
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Container(
             Button("Ping", id="ping-btn"),
             Button("Pong", id="pong-btn"),
             Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
@@ -246,15 +260,15 @@
     ```
 
 
 - <details>
   <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
 
     ```python
-    from textology.apps import ObservedApp
+    from textology.apps import ExtendedApp
     from textology.observers import Published, Select, Update, when
     from textology.widgets import Button, Container, Label
     
     
     class Page(Container):
         def compose(self):
             yield Button("Ping", id="ping-btn")
@@ -286,15 +300,15 @@
         )
         def song(self, event, ping_clicks, pong_clicks):
             if not ping_clicks or not pong_clicks:
                 return Label(f"Press Ping and Pong first to complete the song!")
             return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
     
     
-    app = ObservedApp(
+    app = ExtendedApp(
         layout=Page()
     )
     
     app.run()
     ```
 
 
@@ -418,14 +432,14 @@
 
 @pytest.mark.asyncio
 async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
-- Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
+- Ability to pass an App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
 
 View all options by running `pytest -h` and referring to `Custom options:` section.
```

### Comparing `textology-0.0.6/textology.egg-info/SOURCES.txt` & `textology-0.2.0/textology.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 textology/__init__.py
 textology/apps.py
 textology/dash_compat.py
 textology/history.py
 textology/logging.py
+textology/pages.py
 textology/pytest_utils.py
 textology/router.py
 textology/test-template.html
 textology.egg-info/PKG-INFO
 textology.egg-info/SOURCES.txt
 textology.egg-info/dependency_links.txt
 textology.egg-info/requires.txt
```

