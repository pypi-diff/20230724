# Comparing `tmp/pynamicui-0.0.9.tar.gz` & `tmp/pynamicui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.9.tar", last modified: Sun Jul 23 02:16:39 2023, max compression
+gzip compressed data, was "pynamicui-0.1.0.tar", last modified: Mon Jul 24 19:26:07 2023, max compression
```

## Comparing `pynamicui-0.0.9.tar` & `pynamicui-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.758376 pynamicui-0.0.9/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     7598 2023-07-23 02:16:39.756380 pynamicui-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7115 2023-07-19 21:40:59.000000 pynamicui-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.677227 pynamicui-0.0.9/pynamicui/
--rw-rw-rw-   0        0        0      752 2023-07-23 02:11:12.000000 pynamicui-0.0.9/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.737242 pynamicui-0.0.9/pynamicui/createDom/
--rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.9/pynamicui/createDom/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-07-19 05:26:39.000000 pynamicui-0.0.9/pynamicui/createDom/createDom.py
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.745377 pynamicui-0.0.9/pynamicui/createElement/
--rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.9/pynamicui/createElement/__init__.py
--rw-rw-rw-   0        0        0    11791 2023-07-23 01:28:16.000000 pynamicui-0.0.9/pynamicui/createElement/createElement.py
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.752373 pynamicui-0.0.9/pynamicui/createStylesheet/
--rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.9/pynamicui/createStylesheet/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.9/pynamicui/createStylesheet/createStylesheet.py
-drwxrwxrwx   0        0        0        0 2023-07-23 02:16:39.729256 pynamicui-0.0.9/pynamicui.egg-info/
--rw-rw-rw-   0        0        0     7598 2023-07-23 02:16:39.000000 pynamicui-0.0.9/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-23 02:16:39.000000 pynamicui-0.0.9/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 02:16:39.000000 pynamicui-0.0.9/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-23 02:16:39.000000 pynamicui-0.0.9/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-23 02:16:39.000000 pynamicui-0.0.9/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-07-23 02:02:01.000000 pynamicui-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 02:16:39.758376 pynamicui-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-07-23 02:02:05.000000 pynamicui-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.864783 pynamicui-0.1.0/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7598 2023-07-24 19:26:07.863782 pynamicui-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7115 2023-07-19 21:40:59.000000 pynamicui-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.774266 pynamicui-0.1.0/pynamicui/
+-rw-rw-rw-   0        0        0      800 2023-07-24 19:24:15.000000 pynamicui-0.1.0/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.839273 pynamicui-0.1.0/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.1.0/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     2346 2023-07-23 19:53:02.000000 pynamicui-0.1.0/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.846787 pynamicui-0.1.0/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.1.0/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0    13714 2023-07-24 18:32:34.000000 pynamicui-0.1.0/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.852785 pynamicui-0.1.0/pynamicui/createPageViewer/
+-rw-rw-rw-   0        0        0       46 2023-07-24 18:50:13.000000 pynamicui-0.1.0/pynamicui/createPageViewer/__init__.py
+-rw-rw-rw-   0        0        0     2777 2023-07-24 19:09:35.000000 pynamicui-0.1.0/pynamicui/createPageViewer/createPageViewer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.858795 pynamicui-0.1.0/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.1.0/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.1.0/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:26:07.822281 pynamicui-0.1.0/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0     7598 2023-07-24 19:26:07.000000 pynamicui-0.1.0/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-07-24 19:26:07.000000 pynamicui-0.1.0/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 19:26:07.000000 pynamicui-0.1.0/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 19:26:07.000000 pynamicui-0.1.0/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-24 19:26:07.000000 pynamicui-0.1.0/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-24 19:24:01.000000 pynamicui-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 19:26:07.865783 pynamicui-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-07-24 19:23:56.000000 pynamicui-0.1.0/setup.py
```

### Comparing `pynamicui-0.0.9/LICENSE` & `pynamicui-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.9/PKG-INFO` & `pynamicui-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.9
+Version: 0.1.0
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `pynamicui-0.0.9/README.md` & `pynamicui-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.9/pynamicui/__init__.py` & `pynamicui-0.1.0/pynamicui/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 
 import customtkinter as tk
 from PIL import Image
 
 from .createDom import createDom
 from .createElement import createElement
 from .createStylesheet import createStylesheet
+from .createPageViewer import createPageViewer
 
 def setAppearanceMode(mode):
     tk.set_appearance_mode(mode)
 
 def setDefaultColorTheme(theme):
     tk.set_default_color_theme(theme)
```

### Comparing `pynamicui-0.0.9/pynamicui/createDom/createDom.py` & `pynamicui-0.1.0/pynamicui/createDom/createDom.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     def useState(self, attr, value, callback):
         st = self.states.get(attr)
         if st:
             self.states[attr] = {"value": value, "callbacks": st.callbacks.append(callback)}
         else:
             self.states[attr] = {"value": value, "callbacks": [callback]}
         # Register a state with its initial value and associated callback
+        # Return two anonymous functions for getting and setting state
+        return lambda a=attr: self.getState(a), lambda val, a=attr: self.setState(a, val)
 
     def setStylesheet(self, sheet):
         self.stylesheet=sheet.stylesheet
 
     def setGeometry(self, val):
         if self.widget:
             self.widget.geometry(val)
```

### Comparing `pynamicui-0.0.9/pynamicui/createElement/createElement.py` & `pynamicui-0.1.0/pynamicui/createElement/createElement.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import customtkinter as tk
+import warnings
 
 def findDom(parent):
     if hasattr(parent, "root"):
         return parent
     elif hasattr(parent, "parent"):
         return findDom(parent.parent)
     else:
@@ -63,15 +64,38 @@
                 # The relative x and y coordinates are calculated as the column/row number divided by the total number of columns/rows
                 "relx": col / cols,
                 "rely": row / rows
             }
     # Return the parsed grid
     return parsed_grid
 
+def applyMarginToGeometry(geometry, marx, mary):
+    """
+    Adjust the geometry with marx and mary values relative to the parent element.
+
+    Parameters:
+        geometry (dict): A dictionary representing the geometry with keys 'relwidth', 'relheight', 'relx', and 'rely'.
+        marx (float): The margin value to be applied relative to the parent element.
+        mary (float): The margin value to be applied relative to the parent element.
 
+    Returns:
+        dict: A new dictionary with adjusted geometry values after applying margin.
+    """
+    adjustedGeometry = {}
+
+    scale_width = geometry.get('relwidth', 1)
+    scale_height = geometry.get('relheight', 1)
+
+    adjustedGeometry['relwidth'] = scale_width - marx
+    adjustedGeometry['relheight'] = scale_height - mary
+
+    adjustedGeometry['relx'] = geometry.get('relx', 0) + (.5 * marx)
+    adjustedGeometry['rely'] = geometry.get('rely', 0) + (.5 * mary)
+
+    return adjustedGeometry
 
 def applyPaddingToGeometry(geometry, padx, pady):
     """
     Adjust the geometry with padx and pady values relative to the scale of relwidth and relheight.
 
     Parameters:
         geometry (dict): A dictionary representing the geometry with keys 'relwidth', 'relheight', 'relx', and 'rely'.
@@ -91,62 +115,69 @@
 
     adjustedGeometry['relx'] = geometry.get('relx', 0) + (.5 * scale_width * padx)
     adjustedGeometry['rely'] = geometry.get('rely', 0) + (.5 * scale_height * pady)
 
     return adjustedGeometry
 
 class createElement:
-    def __init__(self, parent, tag, id=None, name=None, props=None, children=None, place=None, visible=True, hooks=None, style=None, spacing=None):
+    def __init__(self, parent, tag, id=None, name=None, spawnProps=None, props=None, children=None, place=None, visible=True, hooks=None, style=None, spacing=None):
         self.parent = parent
         self.name = name or "Pynamic" + tag + "Element"  # Name of the virtual element
         self.tag = "CTk" + tag  # Tag name for tkinter widget
         self.props = props or {}  # Dictionary to store widget properties
         self.children = children or []  # List of child elements
         self.widget = None  # Reference to the tkinter widget instance
         self.currentPlace = place or {}  # Placement options for the widget
-        self.spacing = spacing or {"padx": 0, "pady": 0} # padx and pady
+        self.spacing = {"padx": 0, "pady": 0, "marx": 0, "mary": 0} # padx and pady
         self.visible = visible  # Flag to indicate element visibility
         self.hooks = hooks or {}  # Dictionary to store hooks
         self.style = style or ""
         self.mounted = False
         self.id = id or None
         self.grid = None
+        self.styleConfig = {}
+        self.spawnProps = spawnProps or {}
 
         if hasattr(self.parent, "root"):
             self.dom = self.parent
             self.dom.appendChild(self)
         elif self.parent:
             self.dom = findDom(self.parent.parent)
             self.parent.appendChild(self)
 
+        if spacing:
+            self.spacing.update(spacing)
+
+        self.updateStyle()
+
     def render(self):
         """
         Render the element and its descendents
         """
         if self.visible:
             
-            if self.widget:
-                self.widget.destroy()
-            self.widget = getattr(tk, self.tag)(self.parent.widget)  # Create the tkinter widget
-            for prop, value in self.props.items():
-                self.widget.configure(**{prop: value})  # Configure widget properties
-            
-            self.updateStyle()
+            if not self.widget:
+                self.widget = getattr(tk, self.tag)(self.parent.widget, **self.spawnProps)  # Create the tkinter widget
 
+            self.widget.configure(**self.props)  # Configure widget properties
+            self.widget.configure(**self.styleConfig)
 
             for child in self.children:
                 if child.visible:
                     if self.grid and child.id:
                         pos = self.grid.get(child.id)
                         if pos:
-                            child.place(pos)
+                            child.currentPlace = pos
                     child.render()  # Render each child element
 
             self.place(self.currentPlace)  # Place the widget in the parent
 
+    def setId(self, id):
+        self.id = id
+
     def unmount(self):
         """
         PRIVATE: Unmount the element to virtual dom (interal use)
         """
         self.mounted = False
         for prop, hook in self.hooks.items():
             if hook[1] is not None:
@@ -176,15 +207,16 @@
             self.hooks[prop] = [hook, unmount]  # Register a hook with its callback and unmount function
 
     def setProp(self, prop, value):
         """
         Set a Widget prop value (Must be a valid element prop (refer to wiki))
         """
         self.props[prop] = value  # Update the property value
-        self.widget.configure(**{prop: value})  # Configure the updated property
+        if self.widget:
+            self.widget.configure(**{prop: value})  # Configure the updated property
         
         if self.hooks.get(prop):
             self.hooks[prop][0](prop, self, value)  # Invoke the hook callback if present
 
     def hide(self):
         """
         Hide element and its descendants (Will call unmount event)
@@ -209,26 +241,36 @@
 
     def place(self, geometry):
         """
         Set the element's geometry and place the widget if it exists
         """
         self.currentPlace = geometry
         if self.widget:
-            self.widget.place(**applyPaddingToGeometry(self.currentPlace, self.spacing.get("padx", 0), self.spacing.get("pady", 0)))
+            pad = applyPaddingToGeometry(self.currentPlace, self.spacing.get("padx", 0), self.spacing.get("pady", 0))
+            self.widget.place(**applyMarginToGeometry(pad, self.spacing.get("marx", 0), self.spacing.get("mary", 0)))
 
     def updateStyle(self):
         """
         This will apply any styling to the element's widget.
         """
-        if self.style != "" and self.widget:
-            for item, value in self.dom.stylesheet[self.style].items():
-                if item in self.spacing:
-                    self.spacing[item] = value
-                else:
-                    self.widget.configure(**{item: value})
+        if self.style != "":
+            if not self.style in self.dom.stylesheet:
+                warnings.warn("Invalid stylename: " + self.style)
+            else:
+                config = {}
+                for item, value in self.dom.stylesheet[self.style].items():
+                    if item in self.spacing:
+                        self.spacing[item] = value
+                    else:
+                        config[item] = value
+                self.styleConfig = config
+                if self.widget:
+                    self.widget.configure(**config)
+        else:
+            self.styleConfig = {}
 
     def appendChild(self, child):
         """
         Append a child to this element and remove the child from any other element's child list
         """
         if child in child.parent.children:
             index_to_remove = child.parent.children.index(child)
@@ -279,17 +321,30 @@
     def destroy(self):
         """
         Destroy the element and all its children from the virtual DOM
         """
         if self in self.parent.children:
             index_to_remove = self.parent.children.index(self)
             self.parent.children.pop(index_to_remove)
+
         self.parent = None
         if self.widget:
             self.widget.destroy()
         self.props = {}
         self.hooks = {}
+
+
+    def destroyChildren(self):
+        """
+        Save the element but destroy all its children from the virtual DOM
+        """
         for child in self.children:
-            child.destroy()
-        del self
+            if child.widget:
+                child.widget.destroy()
+                child.props = {}
+                child.hooks = {}
+
+        self.children=[]
+        
+
```

### Comparing `pynamicui-0.0.9/pynamicui/createStylesheet/createStylesheet.py` & `pynamicui-0.1.0/pynamicui/createStylesheet/createStylesheet.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.9/pynamicui.egg-info/PKG-INFO` & `pynamicui-0.1.0/pynamicui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.9
+Version: 0.1.0
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `pynamicui-0.0.9/pyproject.toml` & `pynamicui-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.9"
+current = "0.1.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pynamicui-0.0.9/setup.py` & `pynamicui-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pynamicui',
-    version='0.0.9',
+    version='0.1.0',
     description='dynamic web-like UIs using a declarative syntax',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zacharie410/PynamicUI',
     author='zacharie410',
     license='Apache Software License',
     classifiers=[
```

