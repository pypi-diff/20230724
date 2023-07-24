# Comparing `tmp/multicloud_diagrams-0.3.7.tar.gz` & `tmp/multicloud_diagrams-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.3.7.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.3.8.tar", max compression
```

## Comparing `multicloud_diagrams-0.3.7.tar` & `multicloud_diagrams-0.3.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.7/LICENSE
--rw-r--r--   0        0        0     8567 2023-07-23 08:37:02.246004 multicloud_diagrams-0.3.7/README.md
--rw-r--r--   0        0        0    16785 2023-07-23 19:43:42.165414 multicloud_diagrams-0.3.7/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0     3868 2023-07-23 07:39:33.823106 multicloud_diagrams-0.3.7/multicloud_diagrams/providers/aws_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.7/multicloud_diagrams/providers/azure_services.json
--rw-r--r--   0        0        0      207 2023-05-19 12:11:15.381235 multicloud_diagrams-0.3.7/multicloud_diagrams/providers/fallback.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.7/multicloud_diagrams/providers/gcp_services.json
--rw-r--r--   0        0        0      616 2023-07-23 07:39:33.816960 multicloud_diagrams-0.3.7/multicloud_diagrams/providers/on_prem_services.json
--rw-r--r--   0        0        0      525 2023-07-23 19:45:33.566284 multicloud_diagrams-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     9085 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.8/LICENSE
+-rw-r--r--   0        0        0     8567 2023-07-23 08:37:02.246004 multicloud_diagrams-0.3.8/README.md
+-rw-r--r--   0        0        0    17771 2023-07-24 07:50:24.803328 multicloud_diagrams-0.3.8/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0     3868 2023-07-23 07:39:33.823106 multicloud_diagrams-0.3.8/multicloud_diagrams/providers/aws_services.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.8/multicloud_diagrams/providers/azure_services.json
+-rw-r--r--   0        0        0      207 2023-05-19 12:11:15.381235 multicloud_diagrams-0.3.8/multicloud_diagrams/providers/fallback.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.8/multicloud_diagrams/providers/gcp_services.json
+-rw-r--r--   0        0        0      616 2023-07-23 07:39:33.816960 multicloud_diagrams-0.3.8/multicloud_diagrams/providers/on_prem_services.json
+-rw-r--r--   0        0        0      525 2023-07-24 07:51:35.502861 multicloud_diagrams-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     9085 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.8/PKG-INFO
```

### Comparing `multicloud_diagrams-0.3.7/LICENSE` & `multicloud_diagrams-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.7/README.md` & `multicloud_diagrams-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.7/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.3.8/multicloud_diagrams/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,20 @@
                                                 'mxGeometry',
                                                 relative="1"
                                                 )
                     mx_geometry.set('as', 'geometry')
                     # <mxPoint as="offset"/>
                     mx_geometry = et.SubElement(mx_geometry, 'mxPoint')
                     mx_geometry.set('as', 'offset')
+                    if f'label:{src_node_id}:to:{dest_node_id}' in self.prev_coords:
+                        if 'x' in self.prev_coords[f'label:{src_node_id}:to:{dest_node_id}']:
+                            mx_geometry.set('x', self.prev_coords[f'label:{src_node_id}:to:{dest_node_id}']['x'])
+                        if 'y' in self.prev_coords[f'label:{src_node_id}:to:{dest_node_id}']:
+                            mx_geometry.set('y', self.prev_coords[f'label:{src_node_id}:to:{dest_node_id}']['y'])
+
                     # </mxGeometry>
                     # </mxCell>
             else:
                 logging.warning(
                     f'Already exist edge:{src_node_id}:to:{dest_node_id}')
         else:
             logging.error(
@@ -334,13 +340,23 @@
                         cords['y'] = data.get('y')
                     if data.get('height') is not None:
                         cords['height'] = data.get('height')
                     if data.get('width') is not None:
                         cords['width'] = data.get('width')
                     self.prev_coords[neighbor.get('id')] = cords
 
+                elif neighbor.get('id').startswith("label:"):
+                    data = neighbor.find('mxGeometry')
+                    mx_point = data.find('mxPoint')
+                    cords = {}
+                    if mx_point.get('x') is not None:
+                        cords['x'] = mx_point.get('x')
+                    if mx_point.get('y') is not None:
+                        cords['y'] = mx_point.get('y')
+                    self.prev_coords[neighbor.get('id')] = cords
+
     def export_to_file(self, file_path):
         with open(file_path, 'wb') as file:
             tree = et.ElementTree(self.mxfile)
             et.indent(tree, space="\t", level=0)
             tree.write(file, encoding='utf-8')
         return
```

### Comparing `multicloud_diagrams-0.3.7/multicloud_diagrams/providers/aws_services.json` & `multicloud_diagrams-0.3.8/multicloud_diagrams/providers/aws_services.json`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.7/multicloud_diagrams/providers/on_prem_services.json` & `multicloud_diagrams-0.3.8/multicloud_diagrams/providers/on_prem_services.json`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.7/pyproject.toml` & `multicloud_diagrams-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicloud-diagrams"
-version = "0.3.7"
+version = "0.3.8"
 description = "Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported."
 authors = ["Roman Tsypuk <tsypuk.conf@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "multicloud_diagrams"}]
 
 [tool.poetry.dependencies]
```

### Comparing `multicloud_diagrams-0.3.7/PKG-INFO` & `multicloud_diagrams-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.3.7
+Version: 0.3.8
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

