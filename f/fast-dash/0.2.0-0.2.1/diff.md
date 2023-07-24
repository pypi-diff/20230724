# Comparing `tmp/fast_dash-0.2.0.tar.gz` & `tmp/fast_dash-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dash-0.2.0.tar", max compression
+gzip compressed data, was "fast_dash-0.2.1.tar", max compression
```

## Comparing `fast_dash-0.2.0.tar` & `fast_dash-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-03 02:52:18.779733 fast_dash-0.2.0/LICENSE
--rw-r--r--   0        0        0     3585 2023-07-03 02:52:18.779733 fast_dash-0.2.0/README.md
--rw-r--r--   0        0        0    33784 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/Components.py
--rw-r--r--   0        0        0      635 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/__init__.py
--rw-r--r--   0        0        0    24457 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/assets/favicon.ico
--rw-r--r--   0        0        0    16369 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/fast_dash.py
--rw-r--r--   0        0        0     6723 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/utils.py
--rw-r--r--   0        0        0     2269 2023-07-03 02:52:18.895733 fast_dash-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      314 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     3026 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/examples.py
--rw-r--r--   0        0        0     2300 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_examples.py
--rw-r--r--   0        0        0     5831 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_fast_dash.py
--rw-r--r--   0        0        0    21632 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_fast_dash_autodetect.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 fast_dash-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-24 00:13:17.063369 fast_dash-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3824 2023-07-24 00:13:17.063369 fast_dash-0.2.1/README.md
+-rw-r--r--   0        0        0    34285 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/Components.py
+-rw-r--r--   0        0        0      635 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/__init__.py
+-rw-r--r--   0        0        0    24457 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/assets/favicon.ico
+-rw-r--r--   0        0        0    17290 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/fast_dash.py
+-rw-r--r--   0        0        0     7667 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/utils.py
+-rw-r--r--   0        0        0     2325 2023-07-24 00:13:17.195369 fast_dash-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     3538 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/examples.py
+-rw-r--r--   0        0        0     2709 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_examples.py
+-rw-r--r--   0        0        0     6261 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_fast_dash.py
+-rw-r--r--   0        0        0    21632 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_fast_dash_autodetect.py
+-rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 fast_dash-0.2.1/PKG-INFO
```

### Comparing `fast_dash-0.2.0/LICENSE` & `fast_dash-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.0/README.md` & `fast_dash-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     <img src="https://img.shields.io/github/license/dkedar7/fast_dash" alt="MIT License">
 </a>
 
 <a href="https://docs.fastdash.app/">
     <img src="https://img.shields.io/badge/Docs-MkDocs-<COLOR>.svg" alt="Documentation">
 </a>
 
+<a href="https://pepy.tech/project/fast-dash">
+    <img src="https://static.pepy.tech/personalized-badge/fast-dash?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Downloads">
+</a>
+
 </p>
 
 
 ---
 
 * **Documentation**: [https://docs.fastdash.app](https://docs.fastdash.app)
 * **Source code**: [github.com/dkedar7/fast_dash](https://github.com/dkedar7/fast_dash/)
@@ -53,15 +57,15 @@
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
 
 And just like that (🪄), we have a completely functional interactive app!
 
 Output:
-![Simple example](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20text%20to%20text.png)
+![Simple example](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20text%20to%20text.png)
 ---
 
 Fast Dash can read all the function details, like its name, input and output types, docstring, and uses this information to infer which components to use.
 
 For example, here's how to deploy an app that takes a string and an integer as inputs and returns some text.
 
 ```python
@@ -73,15 +77,15 @@
     processed_text = f'Selected text is {text} and the number is {number}.'
     return processed_text
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
 
 Output:
-![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20example%202.png)
+![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20example%202.png)
 
 And with just a few more lines, we can add a title icon, subheader and other social branding details.
 
 ---
 
 ## About
```

### Comparing `fast_dash-0.2.0/fast_dash/Components.py` & `fast_dash-0.2.1/fast_dash/Components.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,14 @@
         self.linkedin_url = linkedin_url
         self.twitter_url = twitter_url
         self.navbar = navbar
         self.footer = footer
         self.minimal = minimal
         self.scale_height = scale_height
 
-        if minimal:
-            self.title = self.subtitle = self.navbar = self.footer = False
-
     def generate_navbar_container(self):
         if not self.navbar:
             return None
 
         # 1. Navbar
         social_media_navigation = []
         if self.github_url:
@@ -101,24 +98,39 @@
                     )
                 )
             )
 
         navbar = dbc.NavbarSimple(
             children=[dbc.NavItem(dbc.NavLink("About", href="#"))]
             + social_media_navigation,
-            brand=self.title or "",
+            brand=[
+                dmc.Group(
+                    [
+                        dmc.Burger(
+                            id="sidebar-button", opened=True, color="white", size=15
+                        ),
+                        self.title,
+                    ],
+                    spacing=5,
+                )
+            ]
+            or "",
             color="primary",
             dark=True,
             fluid=True,
             fixed=None,
             style={"padding": "0 0 0 0"},
         )
 
         navbar_container = dbc.Container(
-            [navbar], fluid=True, style={"padding": "0 0 0 0"}, id="navbar3260780"
+            [navbar],
+            fluid=True,
+            style={"padding": "0 0 0 0"},
+            id="navbar3260780",
+            className="dbc",
         )
 
         return navbar_container
 
     def generate_header_component(self):
         header_children = []
 
@@ -225,14 +237,17 @@
         footer_container = dbc.Container(
             [footer], fluid=True, style={"padding": "0 0 0 2%"}, id="footer5265971"
         )
 
         return footer_container
 
     def generate_layout(self):
+        if self.minimal:
+            self.title = self.subtitle = self.navbar = self.footer = False
+
         layout = dbc.Container(
             [
                 self.generate_navbar_container(),
                 self.generate_header_component(),
                 dbc.Row(
                     [self.generate_input_component(), self.generate_output_component()],
                     justify="evenly",
@@ -440,15 +455,15 @@
             begin_index = i_break
 
         return sub_mosaics
 
     def _get_component(self, axis, width, style=None):
         if axis == 1:
             style = self.col_style if style is None else style
-            # style.update({"max-height": "100%"})
+            style.update({"height": "100%"})
             layout = dbc.Col(
                 [],
                 style=style,
                 width=width,
                 class_name="p-0 d-flex flex-column flex-fill",
             )
 
@@ -506,36 +521,23 @@
                 array, 1 - axis, self._get_component(axis=1 - axis, width=width)
             )
             layout.children.append(child_layout)
 
         return layout
 
     def generate_input_component(self):
-        button = dbc.Row(
-            dmc.Button(
-                id="sidebar-button",
-                n_clicks=0,
-                size="sm",
-                style=dict(width=50),
-                children=DashIconify(id="sidebar-expand-arrow", icon="maki:cross"),
-                variant="subtle",
-                color="black",
-            ),
-            justify="end",
-        )
-
         return dbc.Col(
-            children=[button, dmc.Stack(children=self.inputs)],
+            children=[dmc.Stack(children=self.inputs)],
             id="input-group",
             sm=2,
-            width=10,
+            width=12,
             style={
                 "background-color": "#F5F7F7",
                 "display": "block",
-                "padding": "0 1% 0 2%",
+                "padding": "2% 1% 0 2%",
                 "height": f"{self.scale_height * 110}vh",
             },
             class_name="border border-right",
         )
 
     def generate_output_component(self):
         mosaic = self._normalize_grid_string(self.mosaic)
@@ -552,108 +554,111 @@
         else:
             unique_locations = np.unique(mosaic_arr)
             unique_locations.sort()
             self.output_component_mapper = {
                 m: o for m, o in zip(unique_locations, self.outputs[:-1])
             }
 
+        # Slice along the axis with the most number of unique elements first
+        begin_axis = np.argmax(
+            [
+                max([len(np.unique(arr)) for arr in mosaic_arr]),
+                max([len(np.unique(arr)) for arr in mosaic_arr.transpose()]),
+            ]
+        )
+
         begin = dbc.Row([], justify=True, class_name="g-1 d-flex")
-        layout = self._do_mosaic(mosaic_arr, axis=1, layout=begin)
-        output_layout = dbc.Col(
-            [layout] + [self.outputs[-1]],
-            class_name="g-1 d-flex flex-fill flex-column",
-            style={"height": f"{80 * self.scale_height}vh"},
+        layout = self._do_mosaic(mosaic_arr, axis=1 - begin_axis, layout=begin)
+        output_layout = dmc.LoadingOverlay(
+            dbc.Col(
+                [layout] + [self.outputs[-1]],
+                class_name="g-1 d-flex flex-fill flex-column",
+                style={"height": f"{80 * self.scale_height}vh"},
+            ),
+            loaderProps=dict(variant="bars"),
         )
 
         return output_layout
 
     def generate_footer_container(self):
         return dmc.Affix(
-            dcc.Link(
-                dmc.Button("Made with Fast Dash"),
-                href="https://github.com/dkedar7/fast_dash",
-                target="_blank",
+            dmc.Tooltip(
+                label="Made with Fast Dash!",
+                position="top",
+                withArrow=True,
+                transitionDuration=300,
+                children=dcc.Link(
+                    dmc.Button(
+                        DashIconify(icon="ion:rocket-sharp", width=20), radius=500
+                    ),
+                    href="https://github.com/dkedar7/fast_dash",
+                    target="_blank",
+                ),
             ),
             position={"bottom": "20px", "right": "20px"},
+            id="footer5265971",
         )
 
     def generate_layout(self):
         # There are four main components:
         # navbar, header, input, output, footer
 
-        button_expand = dmc.Affix(
-            dmc.Button(
-                id="button-expand",
-                n_clicks=0,
-                size="sm",
-                style=dict(display="none"),
-                children=DashIconify(icon="material-symbols:arrow-forward-ios-rounded"),
-                variant="subtle",
-                color="black",
-            ),
-            position={"top": "4.5%", "left": "0"},
-        )
+        if self.minimal:
+            self.title = self.subtitle = self.navbar = self.footer = False
 
-        layout = dbc.Container(
-            [
-                self.generate_navbar_container(),
-                button_expand,
-                dbc.Row(
-                    [
-                        self.generate_input_component(),
-                        dbc.Col(
-                            [
-                                self.generate_header_component(),
-                                self.generate_output_component(),
-                            ],
-                            id="output-group-col",
-                            style={"padding": "1% 2% 0 2%"},
-                        ),
-                    ],
-                    class_name="d-flex",
-                ),
-                self.generate_footer_container(),
-            ],
-            fluid=True,
-            style={"padding": "0 0 0 0", "height": "100vh"},
+        layout = dmc.MantineProvider(
+            dbc.Container(
+                [
+                    self.generate_navbar_container(),
+                    dbc.Row(
+                        [
+                            self.generate_input_component(),
+                            dbc.Col(
+                                [
+                                    self.generate_header_component(),
+                                    self.generate_output_component(),
+                                ],
+                                id="output-group-col",
+                                style={"padding": "1% 2% 0 2%"},
+                            ),
+                        ],
+                        class_name="d-flex",
+                    ),
+                    self.generate_footer_container(),
+                ],
+                fluid=True,
+                style={"padding": "0 0 0 0", "height": "100vh"},
+            )
         )
 
         return layout
 
     def callbacks(self, app):
         @app.callback(
-            [
-                Output("input-group", "style"),
-                Output("output-group-col", "width"),
-                Output("button-expand", "style"),
-            ],
-            [Input("sidebar-button", "n_clicks"), Input("button-expand", "n_clicks")],
-            [State("input-group", "style"), State("button-expand", "style")],
+            [Output("input-group", "style"), Output("output-group-col", "width")],
+            [Input("sidebar-button", "opened")],
+            [State("input-group", "style")],
         )
-        def toggle_sidebar(n_clicks, n_clicks_expand, input_style, expand_style):
+        def toggle_sidebar(opened, input_style):
             input_style = {} if input_style is None else input_style
-            expand_style = {} if expand_style is None else expand_style
             width = 10
 
             display = input_style.get("display", "block")
-            opened = display == "block"
 
             # Condition to collapse the sidebar
-            if n_clicks > n_clicks_expand and opened:
+            if not opened:
                 input_style.update({"display": "none"})
                 width = 12
-                expand_style.update(dict(display="block"))
 
             # Expand by default
             else:
                 input_style.update({"display": "block"})
                 width = 10
-                expand_style.update(dict(display="none"))
 
-            return input_style, width, expand_style
+            return input_style, width
 
 
 _map_types_to_readable_names = {
     str: "Text",
     float: "Numeric",
     int: "Numeric",
     complex: "Numeric",
@@ -707,15 +712,15 @@
         if _default_value_type == "Text":
             component = Fastify(dbc.Input(value=default_value), "value")
 
         elif _default_value_type == "Numeric":
             component = Fastify(dbc.Input(value=default_value, type="number"), "value")
 
         elif _default_value_type == "Sequence":
-            component = Fastify(dcc.Dropdown(options=default_value), "options")
+            component = Fastify(dcc.Dropdown(options=default_value), "value")
 
         elif _default_value_type == "Dictionary":
             component = Fastify(dbc.Input(value=str(default_value)), "value")
 
         elif _default_value_type == "Boolean":
             component = Fastify(dbc.Input(value=str(default_value)), "value")
 
@@ -960,36 +965,53 @@
 
     else:
         component = Fastify(html.H1(), "children")
 
     return component
 
 
-def _infer_components(func, is_input=True):
+def _infer_input_components(func):
     signature = inspect.signature(func)
     components = []
 
-    if is_input is True:
-        parameters = signature.parameters.items()
-        for _, value in parameters:
-            hint = value.annotation
-            default = None if value.default == inspect._empty else value.default
+    parameters = signature.parameters.items()
+    for _, value in parameters:
+        hint = value.annotation
+        default = None if value.default == inspect._empty else value.default
 
-            component = _get_component_from_input(hint, default)
-            components.append(component)
+        component = _get_component_from_input(hint, default)
+        components.append(component)
 
-    else:
-        parameters = enumerate(
+    return components
+
+
+def _infer_output_components(func, output_labels):
+    signature = inspect.signature(func)
+    components = []
+
+    parameters = list(
+        enumerate(
             signature.return_annotation
             if isinstance(signature.return_annotation, tuple)
             else [signature.return_annotation]
         )
+    )
+
+    if output_labels is None:
+        output_labels = [None] * len(parameters)
+
+    if isinstance(output_labels, list) and len(output_labels) != len(parameters):
+        raise ValueError(
+            "Length of output labels must be equal to the number of outputs."
+        )
 
-        for _, hint in parameters:
-            components.append(_get_output_components(hint))
+    for (_, hint), label in zip(parameters, output_labels):
+        component = _get_output_components(hint)
+        component.label_ = label
+        components.append(copy.deepcopy(component))
 
     return components
 
 
 ###################################
 # Define default components #
 ###################################
```

### Comparing `fast_dash-0.2.0/fast_dash/__init__.py` & `fast_dash-0.2.1/fast_dash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Fast Dash."""
 
 __author__ = """Kedar Dabhadkar"""
 __email__ = "kedar@fastdash.app"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 from fast_dash.Components import (
     Graph,
     Image,
     Slider,
     Text,
     TextArea,
```

### Comparing `fast_dash-0.2.0/fast_dash/assets/favicon.ico` & `fast_dash-0.2.1/fast_dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.0/fast_dash/fast_dash.py` & `fast_dash-0.2.1/fast_dash/fast_dash.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 import warnings
 
 import dash
 import dash_bootstrap_components as dbc
 import flask
 from dash import Input, Output
 
-from .Components import BaseLayout, SidebarLayout, Text, _infer_components
+from .Components import (
+    BaseLayout,
+    SidebarLayout,
+    Text,
+    _infer_input_components,
+    _infer_output_components,
+)
 from .utils import (
     _assign_ids_to_inputs,
     _assign_ids_to_outputs,
     _make_input_groups,
     _make_output_groups,
     _transform_outputs,
     theme_mapper,
+    _infer_variable_names,
 )
 
 
 class FastDash:
     """
     Fast Dash app object containing automatically generated UI components and callbacks.
 
@@ -31,14 +38,15 @@
     def __init__(
         self,
         callback_fn,
         layout="sidebar",
         mosaic=None,
         inputs=None,
         outputs=None,
+        output_labels="infer",
         title=None,
         title_image_path=None,
         subheader=None,
         github_url=None,
         linkedin_url=None,
         twitter_url=None,
         navbar=True,
@@ -66,14 +74,18 @@
                 Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type
                 hints and default values. In the absence of type hints, default components are all `Text`.
 
             outputs (Fast component, list of Fast components, optional): Components to represent outputs of the callback function.
                 Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type hints.
                 In the absence of type hints, default components are all `Text`.
 
+            output_labels(list of string labels or "infer" or None, optional): Labels given to the output components. If None, inputs are
+                set labeled integers starting at 1 (Output 1, Output 2, and so on). If "infer", labels are inferred from the function
+                signature.
+
             title (str, optional): Title given to the app. Defaults to None. If `None`, function name (assumed to be in snake case)
                 is converted to title case.
 
             title_image_path (str, optional): Path (local or URL) of the app title image. Defaults to None.
 
             subheader (str, optional): Subheader of the app, displayed below the title image and title. Defaults to None.
                 If `None`, Fast Dash tries to use the callback function's docstring instead.
@@ -110,19 +122,22 @@
 
             run_kwargs (dict, optional): All values from this variable are passed to Dash's `.run` method.
         """
 
         self.callback_fn = callback_fn
         self.layout_pattern = layout
         self.mosaic = mosaic
-        self.inputs = (
-            _infer_components(callback_fn, is_input=True) if inputs is None else inputs
-        )
+        self.output_labels = output_labels
+
+        if output_labels:
+            self.output_labels = _infer_variable_names(callback_fn)
+
+        self.inputs = _infer_input_components(callback_fn) if inputs is None else inputs
         self.outputs = (
-            _infer_components(callback_fn, is_input=False)
+            _infer_output_components(callback_fn, self.output_labels)
             if outputs is None
             else outputs
         )
         self.update_live = update_live
         self.mode = mode
         self.disable_logs = disable_logs
         self.scale_height = scale_height
@@ -315,24 +330,26 @@
             elif self.app_initialized:
                 return self.output_state + ack_components
 
             else:
                 return self.output_state_default + ack_components
 
         # Set layout callbacks
-        self.layout_object.callbacks(self.app)
+        if not self.minimal:
+            self.layout_object.callbacks(self.app)
 
 
 def fastdash(
     _callback_fn=None,
     *,
     layout="sidebar",
     mosaic=None,
     inputs=None,
     outputs=None,
+    output_labels="infer",
     title=None,
     title_image_path=None,
     subheader=None,
     github_url=None,
     linkedin_url=None,
     twitter_url=None,
     navbar=True,
@@ -360,14 +377,18 @@
             Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type
             hints and default values. In the absence of type hints, default components are all `Text`.
 
         outputs (Fast component, list of Fast components, optional): Components to represent outputs of the callback function.
             Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type hints.
             In the absence of type hints, default components are all `Text`.
 
+        output_labels(list of string labels or "infer" or None, optional): Labels given to the output components. If None, inputs are
+            set labeled integers starting at 1 (Output 1, Output 2, and so on). If "infer", labels are inferred from the function
+            signature.
+
         title (str, optional): Title given to the app. Defaults to None. If `None`, function name (assumed to be in snake case)
             is converted to title case.
 
         title_image_path (str, optional): Path (local or URL) of the app title image. Defaults to None.
 
         subheader (str, optional): Subheader of the app, displayed below the title image and title. Defaults to None.
             If `None`, Fast Dash tries to use the callback function's docstring instead.
@@ -415,14 +436,15 @@
             return callback_fn
 
         return wrapper_fastdash(
             layout=layout,
             mosaic=mosaic,
             inputs=inputs,
             outputs=outputs,
+            output_labels=output_labels,
             title=title,
             title_image_path=title_image_path,
             subheader=subheader,
             github_url=github_url,
             linkedin_url=linkedin_url,
             twitter_url=twitter_url,
             navbar=navbar,
```

### Comparing `fast_dash-0.2.0/fast_dash/utils.py` & `fast_dash-0.2.1/fast_dash/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from io import BytesIO
 
 import dash_bootstrap_components as dbc
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from dash import html
 from PIL import ImageFile
+import re
 
 
 def Fastify(component, component_property, ack=None, placeholder=None, label_=None):
     """
     Modify a Dash component to a FastComponent.
 
     Args:
@@ -139,15 +140,14 @@
         input_.id = parameter_name
         inputs_with_ids.append(copy.deepcopy(input_))
 
     return inputs_with_ids
 
 
 def _make_input_groups(inputs_with_ids, update_live):
-
     input_groups = []
 
     input_groups.append(html.H4("INPUTS"))
 
     for idx, input_ in enumerate(inputs_with_ids):
         label = f"{input_.id}" if input_.label_ is None else input_.label_
         label = label.replace("_", " ").upper()
@@ -201,15 +201,14 @@
         output_.id = f"output-{idx + 1}"
         outputs_with_ids.append(copy.deepcopy(output_))
 
     return outputs_with_ids
 
 
 def _make_output_groups(outputs, update_live):
-
     output_groups = []
     # output_groups.append(html.H6("OUTPUT"))
 
     for idx, output_ in enumerate(outputs):
         label = f"Output {idx + 1}" if output_.label_ is None else output_.label_
         label = label.replace("_", " ")
         output_groups.append(
@@ -247,7 +246,33 @@
 
     _transform_mapper = {plt.Figure: _mpl_to_b64, ImageFile.ImageFile: _pil_to_b64}
 
     return [
         _transform_mapper[type(o)](o) if type(o) in _transform_mapper else o
         for o in outputs
     ]
+
+
+def _clean_text(string):
+    # Use regular expression to replace non-alphanumeric characters with underscores
+    pattern_non_alpha_numeric = r"\W"  # \W matches any non-alphanumeric character
+    replacement_non_alpha_numeric = "_"
+    string = re.sub(pattern_non_alpha_numeric, replacement_non_alpha_numeric, string)
+
+    # Use regular expression to remove consecutive underscores and boundary underscores
+    pattern_consecutive_underscores = r"(^_+)|(_{2,})|(_+$)"
+    replacement_consecutive_underscores = ""
+    string = re.sub(
+        pattern_consecutive_underscores, replacement_consecutive_underscores, string
+    )
+
+    return string.upper()
+
+
+def _infer_variable_names(func):
+    s = inspect.getsource(func)
+    final_line = s.split("return")[-1].strip()
+    line_without_comment = final_line.split("#")[0].strip().split(",")
+
+    variable_names = [_clean_text(s) for s in line_without_comment]
+
+    return variable_names
```

### Comparing `fast_dash-0.2.0/pyproject.toml` & `fast_dash-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "fast_dash"
-version = "0.2.0"
+version = "0.2.1"
 homepage = "https://github.com/dkedar7/fast_dash"
 description = "Build Machine Learning prototypes web applications lightning fast."
 authors = ["Kedar Dabhadkar <kedar@fastdash.app>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 4 - Beta',
@@ -53,42 +53,45 @@
 doc = [
     "mkdocs",
     "livereload",
     "mkdocs-include-markdown-plugin",
     "mkdocs-material",
     "mkdocstrings",
     "mkdocs-material-extension",
-    "mkdocs-autorefs"
+    "mkdocs-autorefs",
+    "mkdocs-jupyter"
     ]
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8-docstrings = "^1.6.0"
 pytest-cov = "^3.0.0"
 tox = "^3.25.1"
 pre-commit = "^2.20.0"
 virtualenv = "^20.16.3"
 twine = "^4.0.1"
 toml = "^0.10.2"
 mkdocs = "^1.3.1"
 livereload = "^2.6.3"
 mkdocs-include-markdown-plugin = "^3.6.1"
-mkdocs-material = "^8.3.9"
+mkdocs-material = "9.1.18"
 mkdocstrings = "^0.19.0"
 mkdocs-autorefs = "^0.4.1"
 jupyter-dash = "^0.4.2"
 dash = {extras = ["testing"], version = "^2.6.1"}
 mkdocstrings-python = "^0.7.1"
+mkdocs-jupyter = "^0.24.1"
 
 [tool.poetry.group.test.dependencies]
 urllib3 = "1.26.15"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `fast_dash-0.2.0/tests/examples.py` & `fast_dash-0.2.1/tests/examples.py`

 * *Files 27% similar despite different names*

```diff
@@ -100,16 +100,39 @@
         return _pil_to_b64(processed_image)
 
     app = FastDash(
         callback_fn=image_to_image,
         inputs=UploadImage,
         outputs=Image,
         title="Fast Dash example 5",
-        title_image_path="https://tinyurl.com/mr44nn5y",
+        title_image_path="https://raw.githubusercontent.com/dkedar7/fast_dash/docs/docs/assets/favicon.jpg",
         subheader="Build ML prototypes lightning fast!",
         github_url="https://github.com/dkedar7/fast_dash/",
         linkedin_url="https://linkedin.com/in/dkedar7/",
         twitter_url="https://twitter.com/dkedar7/",
         theme="FLATLY",
     )
 
     return app
+
+
+def example_6_text_to_plt():
+    "Fast Dash example 5. Input is UploadImage. Output is Image."
+
+    import matplotlib.pyplot as plt
+
+    def text_to_plt(some_text) -> plt.Figure:
+
+        fig, ax = plt.subplots(1, 1)
+        ax.plot([1, 2, 3], [4, 5, 6])
+
+        return fig
+
+    app = FastDash(
+        callback_fn=text_to_plt,
+        inputs=Text,
+        outputs=Image,
+        title="Fast Dash example 6",
+        disable_logs=True
+    )
+
+    return app
```

### Comparing `fast_dash-0.2.0/tests/test_examples.py` & `fast_dash-0.2.1/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from .examples import (
     example_1_simple_text_to_text,
     example_2_text_with_slider,
     example_3_image_to_image,
     example_4_image_slider_to_image_text,
     example_5_uploadimage_to_image,
+    example_6_text_to_plt
 )
 
 
 def test_example_1(dash_duo):
     "Test example_1_simple_text_to_text"
 
     app = example_1_simple_text_to_text().app
@@ -65,7 +66,18 @@
     app = example_5_uploadimage_to_image().app
 
     dash_duo.start_server(app)
     dash_duo.wait_for_text_to_equal("#title8888928", "Fast Dash example 5", timeout=4)
 
     assert dash_duo.find_element("#title8888928").text == "Fast Dash example 5"
     assert dash_duo.get_logs() == [], "browser console should contain no error"
+
+def test_example_6(dash_duo):
+    "Test example_6_text_to_plt"
+
+    app = example_6_text_to_plt().app
+
+    dash_duo.start_server(app)
+    dash_duo.wait_for_text_to_equal("#title8888928", "Fast Dash example 6", timeout=4)
+
+    assert dash_duo.find_element("#title8888928").text == "Fast Dash example 6"
+    assert dash_duo.get_logs() == [], "browser console should contain no error"
```

### Comparing `fast_dash-0.2.0/tests/test_fast_dash.py` & `fast_dash-0.2.1/tests/test_fast_dash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 """Tests for `fast_dash` package."""
 # pylint: disable=redefined-outer-name
 
 from fast_dash import FastDash
 from fast_dash.Components import Text
+import matplotlib.pyplot as plt
 
 import time
 
 import pytest
 from selenium.common.exceptions import NoSuchElementException
 
 
@@ -17,14 +18,25 @@
     return input_text
 
 
 def simple_text_to_multiple_text_function(input_text):
     return input_text, input_text
 
 
+def simple_text_to_multiple_outputs(
+    input_text: str,
+) -> (plt.Figure, str):
+    "Something"
+
+    fig, ax = plt.subplots(1, 1)
+    ax.plot([1, 2, 3], [1, 2, 3])
+
+    return fig, "Return some text"
+
+
 def test_fdfd001_set_title(dash_duo):
     "Test title element"
     app = FastDash(
         callback_fn=simple_text_to_text_function,
         inputs=Text,
         outputs=Text,
         title="App title",
@@ -186,13 +198,19 @@
 
 def test_fdfd009_jupyter_dash(dash_duo):
     "Test Fast Dash's mode argument"
 
     app = FastDash(
         callback_fn=simple_text_to_text_function,
         inputs=Text,
-        outputs=Text,
         mode="inline",
     ).app
 
     dash_duo.start_server(app)
     time.sleep(4)
+
+
+def test_fdfd010_output_labels(dash_duo):
+    "Test the auto-infer variable name feature"
+
+    app = FastDash(callback_fn=simple_text_to_multiple_outputs)
+    assert app.output_labels == ["FIG", "RETURN_SOME_TEXT"]
```

### Comparing `fast_dash-0.2.0/tests/test_fast_dash_autodetect.py` & `fast_dash-0.2.1/tests/test_fast_dash_autodetect.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     assert input_component.__doc__ == UploadImage.__doc__
 
     # Defualt value is image
     from PIL import Image
     import requests
     from io import BytesIO
 
-    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/favicon.jpg"
+    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/docs/docs/assets/favicon.jpg"
     response = requests.get(url)
     img = Image.open(BytesIO(response.content))
 
     def simple_image(image=img):
         return image
 
     app = FastDash(callback_fn=simple_image)
@@ -386,15 +386,15 @@
 
     # 1. Default value is PIL image
     import PIL
     from PIL import Image
     import requests
     from io import BytesIO
 
-    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/favicon.jpg"
+    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/docs/docs/assets/favicon.jpg"
     response = requests.get(url)
     img = Image.open(BytesIO(response.content))
 
     def simple_img(img_: PIL.ImageFile.ImageFile = img):
         return img_
 
     app = FastDash(callback_fn=simple_img)
@@ -655,15 +655,15 @@
     )
 
     # 2. Output is an image object
     from PIL import Image
     import requests
     from io import BytesIO
 
-    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/favicon.jpg"
+    url = "https://raw.githubusercontent.com/dkedar7/fast_dash/docs/docs/assets/favicon.jpg"
     response = requests.get(url)
     img = Image.open(BytesIO(response.content))
 
     def simple_image(img_) -> img:
         return img_
 
     app = FastDash(callback_fn=simple_image)
```

### Comparing `fast_dash-0.2.0/PKG-INFO` & `fast_dash-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dash
-Version: 0.2.0
+Version: 0.2.1
 Summary: Build Machine Learning prototypes web applications lightning fast.
 Home-page: https://github.com/dkedar7/fast_dash
 License: MIT
 Author: Kedar Dabhadkar
 Author-email: kedar@fastdash.app
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -53,14 +53,18 @@
     <img src="https://img.shields.io/github/license/dkedar7/fast_dash" alt="MIT License">
 </a>
 
 <a href="https://docs.fastdash.app/">
     <img src="https://img.shields.io/badge/Docs-MkDocs-<COLOR>.svg" alt="Documentation">
 </a>
 
+<a href="https://pepy.tech/project/fast-dash">
+    <img src="https://static.pepy.tech/personalized-badge/fast-dash?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Downloads">
+</a>
+
 </p>
 
 
 ---
 
 * **Documentation**: [https://docs.fastdash.app](https://docs.fastdash.app)
 * **Source code**: [github.com/dkedar7/fast_dash](https://github.com/dkedar7/fast_dash/)
@@ -86,15 +90,15 @@
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
 
 And just like that (🪄), we have a completely functional interactive app!
 
 Output:
-![Simple example](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20text%20to%20text.png)
+![Simple example](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20text%20to%20text.png)
 ---
 
 Fast Dash can read all the function details, like its name, input and output types, docstring, and uses this information to infer which components to use.
 
 For example, here's how to deploy an app that takes a string and an integer as inputs and returns some text.
 
 ```python
@@ -106,15 +110,15 @@
     processed_text = f'Selected text is {text} and the number is {number}.'
     return processed_text
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
 
 Output:
-![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20example%202.png)
+![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20example%202.png)
 
 And with just a few more lines, we can add a title icon, subheader and other social branding details.
 
 ---
 
 ## About
```

