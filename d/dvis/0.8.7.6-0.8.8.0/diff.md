# Comparing `tmp/dvis-0.8.7.6-py3-none-any.whl.zip` & `tmp/dvis-0.8.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18598 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       35 b- defN 22-Aug-10 15:03 dvis/__init__.py
--rw-rw-r--  2.0 unx    39040 b- defN 23-Jul-11 10:21 dvis/dvis.py
--rw-rw-r--  2.0 unx     1525 b- defN 23-Jan-04 10:29 dvis/dvis_cli.py
--rw-rw-r--  2.0 unx     8263 b- defN 23-Jan-02 10:43 dvis/dvis_client.py
--rw-rw-r--  2.0 unx     6060 b- defN 22-Aug-10 15:03 dvis/dvis_client_old.py
--rw-rw-r--  2.0 unx     5510 b- defN 23-Jul-11 09:52 dvis/utils.py
--rw-rw-r--  2.0 unx     4228 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/RECORD
-11 files, 65677 bytes uncompressed, 17216 bytes compressed:  73.8%
+Zip file size: 18733 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       35 b- defN 23-Jul-24 19:46 dvis/__init__.py
+-rw-r--r--  2.0 unx    39221 b- defN 23-Jul-24 20:08 dvis/dvis.py
+-rw-r--r--  2.0 unx     1525 b- defN 23-Jul-24 19:46 dvis/dvis_cli.py
+-rw-r--r--  2.0 unx     8314 b- defN 23-Jul-24 20:10 dvis/dvis_client.py
+-rw-r--r--  2.0 unx     6060 b- defN 23-Jul-24 19:46 dvis/dvis_client_old.py
+-rw-r--r--  2.0 unx     5510 b- defN 23-Jul-24 19:46 dvis/utils.py
+-rw-r--r--  2.0 unx     4282 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      827 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/RECORD
+11 files, 65964 bytes uncompressed, 17351 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: dvis/dvis_client_old.py
 Comment: 
 
 Filename: dvis/utils.py
 Comment: 
 
-Filename: dvis-0.8.7.6.dist-info/METADATA
+Filename: dvis-0.8.8.0.dist-info/METADATA
 Comment: 
 
-Filename: dvis-0.8.7.6.dist-info/WHEEL
+Filename: dvis-0.8.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: dvis-0.8.7.6.dist-info/entry_points.txt
+Filename: dvis-0.8.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dvis-0.8.7.6.dist-info/top_level.txt
+Filename: dvis-0.8.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dvis-0.8.7.6.dist-info/RECORD
+Filename: dvis-0.8.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dvis/dvis.py

```diff
@@ -10,28 +10,18 @@
     from torch import Tensor as torch_tensor
     from torch import float as torch_float
     from torch import double as torch_double
 except:
     torch_tensor = None
     torch_float = None
     torch_double = None
-from .dvis_client_old import (
-    sendMesh2server,
-    send_clear,
-    send_config,
-    sendTrack2server,
-    send_camera,
-    sendCmd2server,
-    sendPose2server,
-    sendInject2server,
-    send_objectKFState,
-    sendCamImage2server,
-)
 
-from .dvis_client import send2server, send_payload2server, send_plotly
+from .dvis_client import send2server, send_payload2server
+from .dvis_client import send_plotly, sendMesh2server, send_clear, send_config, sendTrack2server, sendCmd2server,sendPose2server,sendInject2server, send_objectKFState, sendCamImage2server
+from .dvis_client import set_port, set_vis_port
 import trimesh
 from .utils import get_color, visualize_label, visualize_range, get_color_batched, rgb2hex
 import json
 from PIL import Image, ImageFile
 import os
 from pathlib import Path
 import matplotlib
@@ -98,14 +88,15 @@
         else:
             return data_np, fmt
     elif fmt == "xyz" or fmt == "bbox" or fmt == "corners" or fmt == "line" or fmt == "hbboxes" or fmt == "hbboxes_c":
         return data_np, fmt
     elif fmt == "transform" or fmt == "arrow":
         if data_np.shape[0] == 3 and data_np.shape[1] == 3:
             fmtted = np.eye(4)
+
             fmtted[:3, :3] = data_np
 
             return fmtted, fmt
         return data_np, fmt
     elif fmt == "uv" or fmt == "uvrgb":
         if bounds is None:
             bounds = np.min(data_np[:, :2], 0), np.max(data_np[:, :2], 0)
@@ -1052,15 +1043,15 @@
     if c != 0:
         layout['colorway']= [rgb2hex(get_color(c))]
     return layout
 
 
 
 def dvis(
-    data,
+    data=None,
     fmt=None,
     s=1,
     vs=None,
     bs=None,
     c=0,
     l=0,
     t=None,
@@ -1091,14 +1082,22 @@
             - castShadows (bool): Mesh casts shadows?
             - receiveShadows (bool): Mesh receives shadows?
             - opacity (float): Material opacity (0-1)
             - transparent (bool): Material transparent?
         shape (str, optional): [description]. Defaults to "v".
 
     """
+    # direct config setting
+    if "port" in kwargs:
+        set_port(kwargs["port"])
+        return
+    if "vis_port" in kwargs:
+        set_vis_port(kwargs["vis_port"])
+        return
+    
     if isinstance(l, int):
         l = [l]
     if isinstance(t, int):
         t = [t]
     if isinstance(c, str):
         c = int_hash(c)
```

## dvis/dvis_client.py

```diff
@@ -6,44 +6,54 @@
 import trimesh
 from .utils import get_color
 from PIL import ImageFile, Image
 import gzip
 import base64
 
 
+PORT = 5001
+VIS_PORT = 4999
+
+def set_port(port):
+    global PORT
+    PORT = port
+
+def set_vis_port(port):
+    global VIS_PORT
+    VIS_PORT = port
+
 def encode_to_base64(x):
     if isinstance(x, str):
         return x
     return base64.b64encode(x).decode("utf8")
 
 
 def send2server(data, data_format, size, color, layers, t, name="", meta_data=None, vis_conf=None, shape="v", compression="gzip", sub_format=None):
-    port = 5001
     if data is not None:
         if isinstance(data, np.ndarray):
             if sub_format is None:
                 print(f"Sending {data_format} with shape {data.shape}")
             else:
                 print(f"Sending {data_format}[{sub_format}] with shape {data.shape}")
 
     else:
         print("Sending group")
     if data_format in ["hwc",  "img", "seq"]:
-        vis = visdom.Visdom(port=4999)
+        vis = visdom.Visdom(port=VIS_PORT)
         if data_format == "seq":
             for img in data:
                 vis.image(img, opts=dict(store_history=True), win=name)
         else:
             if isinstance(color, int):
                 pass
             else:
                 data[np.all(data == 255, 2)] = np.array(color)
             vis.image(data.transpose(2, 0, 1), opts={"caption": name})
     elif data_format in ["gif"]:
-        vis = visdom.Visdom(port=4999)
+        vis = visdom.Visdom(port=VIS_PORT)
         vis.text(f'<img src="data:image/gif;base64,{data} ">', opts={"caption": name})
     else:
         if compression == "pkl":
             if isinstance(data, np.ndarray):
                 data = pickle.dumps(data.astype(np.float32).copy(order="C"))
             else:
                 data = pickle.dumps(data)
@@ -65,47 +75,47 @@
             pass
 
         if compression is None:
             send_data = data
         else:
             send_data = encode_to_base64(data)
         requests.post(
-            url=f"http://localhost:{port}/show",
+            url=f"http://localhost:{PORT}/show",
             json={
                 "data": send_data,
                 "compression": compression,
                 "data_format": data_format,
                 "size": size,
                 "color": color,
                 "layers": layers,
                 "t": t,
                 "graph_info": {"name": name},
                 "meta_data": meta_data,
                 "vis_conf": vis_conf,
                 "shape": shape,
             },
         )
+        print(PORT)
 
 
 def send_plotly(data, layout):
-    vis = visdom.Visdom(port=4999)
+    vis = visdom.Visdom(port=VIS_PORT)
     print(f"Sending plolty {data['type']}")
     vis._send({"data": [data], "layout": layout})
 
 def send_payload2server(
     payload, data_format, size, color, layers, t, name="", meta_data=None, vis_conf=None, shape="v", compression="pkl"
 ):
-    port = 5001
     if data_format == "cam_img":
         payload["image"] = img_to_base64(payload["image"])
     if "trs" in payload:
         payload["trs"] = encode_to_base64(payload["trs"].astype(np.float32).copy(order="C"))
 
     requests.post(
-        url=f"http://localhost:{port}/show_payload",
+        url=f"http://localhost:{PORT}/show_payload",
         json={
             "payload": encode_to_base64(pickle.dumps(payload)),
             "compression": compression,
             "data_format": data_format,
             "size": size,
             "color": color,
             "layers": layers,
@@ -125,15 +135,15 @@
     buffered = BytesIO()
     image.save(buffered, format="JPEG")
     img_str = base64.b64encode(buffered.getvalue()).decode()
     img_str = "data:image/jpeg;base64," + img_str
     return img_str
 
 
-def sendCamImage2server(image_data, cam_name, layers, t, name, vs=1, port=5001):
+def sendCamImage2server(image_data, cam_name, layers, t, name, vs=1):
     if isinstance(image_data, (ImageFile.ImageFile, Image.Image)):
         image = image_data
     elif isinstance(image_data, np.ndarray):
         image = Image.fromarray(image_data)
     else:
         raise NotImplementedError("Image data format not supported!")
     img_str = img_to_base64(image)
@@ -141,87 +151,87 @@
         "image_str": img_str,
         "cam_name": cam_name,
         "name": name,
         "t": t,
         "layers": layers,
         "vs": vs,
     }
-    requests.post(url=f"http://localhost:{port}/cam_image", json=cam_image)
+    requests.post(url=f"http://localhost:{PORT}/cam_image", json=cam_image)
     print(f"Sending cam image for cam {cam_name} at {t}")
 
 
-def send_config(config, port=5001):
-    requests.post(url=f"http://localhost:{port}/config", json=config)
+def send_config(config):
+    requests.post(url=f"http://localhost:{PORT}/config", json=config)
 
 
-def send_camera(cam_data, port=5001):
+def send_camera(cam_data):
     cam_data["trs"] = codecs.encode(pickle.dumps(cam_data["trs"]), "base64").decode()
-    requests.post(url=f"http://localhost:{port}/add_camera", json=cam_data)
+    requests.post(url=f"http://localhost:{PORT}/add_camera", json=cam_data)
 
 
-def sendCmd2server(cmd_data, port=5001):
-    requests.post(url=f"http://localhost:{port}/send_cmd", json=cmd_data)
+def sendCmd2server(cmd_data):
+    requests.post(url=f"http://localhost:{PORT}/send_cmd", json=cmd_data)
 
 
-def sendInject2server(cmd_data, port=5001):
-    requests.post(url=f"http://localhost:{port}/inject", json=cmd_data)
+def sendInject2server(cmd_data):
+    requests.post(url=f"http://localhost:{PORT}/inject", json=cmd_data)
 
 
-def sendPose2server(pose_data, port=5001):
-    requests.post(url=f"http://localhost:{port}/send_pose", json=codecs.encode(pickle.dumps(pose_data), "base64").decode())
+def sendPose2server(pose_data):
+    requests.post(url=f"http://localhost:{PORT}/send_pose", json=codecs.encode(pickle.dumps(pose_data), "base64").decode())
 
 
-def send_objectKFState(object_kf_state, port=5001):
+def send_objectKFState(object_kf_state):
     object_kf_state["trs"] = codecs.encode(pickle.dumps(object_kf_state["trs"]), "base64").decode()
-    requests.post(url=f"http://localhost:{port}/send_object_kf_state", json=object_kf_state)
+    requests.post(url=f"http://localhost:{PORT}/send_object_kf_state", json=object_kf_state)
     print(f"Sending kf state for {object_kf_state['name']} at {object_kf_state['kf']}")
 
 
-def sendTrack2server(track_data, traj=None, from_json=True, vs=1, c=0, l=0, port=5001):
+def sendTrack2server(track_data, traj=None, from_json=True, vs=1, c=0, l=0):
 
     if isinstance(track_data, str):
-        requests.post(url=f"http://localhost:{port}/local_track", json={"fn": track_data, "traj": traj, "c": c, "l": l, "vs": vs})
+        requests.post(url=f"http://localhost:{PORT}/local_track", json={"fn": track_data, "traj": traj, "c": c, "l": l, "vs": vs})
     else:
         if from_json:
-            requests.post(url=f"http://localhost:{port}/track", json=track_data)
+            requests.post(url=f"http://localhost:{PORT}/track", json=track_data)
         else:
             track_dict = dict()
             track_dict["name"] = track_data.get("name")
             track_dict["data"] = {}
             for kf, kf_data in track_data["data"].items():
                 if isinstance(kf_data, np.ndarray):
                     track_dict["data"][kf] = dict(trs=kf_data, visible=True)
                 elif isinstance(kf_data, dict):
                     track_dict["data"][kf] = dict(trs=kf_data["trs"], visible=kf_data["visible"])
 
             track_dict = pickle.dumps(track_dict)
 
-            requests.post(url=f"http://localhost:{port}/track_dict", json=codecs.encode(track_dict, "base64").decode())
+            requests.post(url=f"http://localhost:{PORT}/track_dict", json=codecs.encode(track_dict, "base64").decode())
 
 
 def send_clear(reset_cam):
-    requests.post(url="http://localhost:5001/clear", json={"reset_cam": reset_cam})
+    requests.post(url=f"http://localhost:{PORT}/clear", json={"reset_cam": reset_cam})
 
 
-def sendMesh2server(tm, color, layers, t, add, name="", meta_data=None, compression="glb", port=5001, vis_conf=None):
+def sendMesh2server(tm, color, layers, t, add, name="", meta_data=None, compression="glb", vis_conf=None):
     if compression == "glb":
         data = tm.export(file_type="glb")
         data = codecs.encode(data, "base64").decode()
         print(f"Sending scene of {len(tm.triangles)} triangles")
     elif compression == "obj":
         if color > 0:
             tm.visual.vertex_colors = get_color(color)
         try:
             data = tm.export(file_type="obj")
         except:
             data = trimesh.Trimesh(vertices=tm.vertices, faces=tm.faces).export(file_type="obj")
         print(f"Sending trimesh of {len(tm.vertices)} vertices and {len(tm.faces)} faces")
 
     requests.post(
-        url=f"http://localhost:{port}/showMesh",
+        url=f"http://localhost:{PORT}/showMesh",
         json={
             "data": data,
             "layers": layers,
             "t": t,
             "compression": compression,
             "data_format": "trimesh",
             "graph_info": {"add": add, "name": name},
```

## Comparing `dvis-0.8.7.6.dist-info/METADATA` & `dvis-0.8.8.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: dvis
-Version: 0.8.7.6
+Version: 0.8.8.0
 Summary: The best web-based visualizer
 Home-page: https://github.com/SirWyver/dvis
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: visdom
-Requires-Dist: trimesh
-Requires-Dist: pillow
-Requires-Dist: flask (==1.1.2)
-Requires-Dist: flask-socketio (==4.3.0)
-Requires-Dist: simple-websocket (==0.2.0)
-Requires-Dist: python-socketio (==4.6.1)
 Requires-Dist: eventlet
-Requires-Dist: fabric
-Requires-Dist: matplotlib
+Requires-Dist: flask (>=2.3.2)
+Requires-Dist: flask-socketio (>=5.3.4)
+Requires-Dist: jinja2 (>=3.0.2)
+Requires-Dist: numpy
 Requires-Dist: opencv-python
+Requires-Dist: pillow
+Requires-Dist: python-socketio (>=4.6.1)
+Requires-Dist: simple-websocket (>=0.2.0)
+Requires-Dist: trimesh
+Requires-Dist: werkzeug (>=2.0.3)
 
 <p align="center"><a  target="_blank" rel="noopener noreferrer"><img width="100" src="./static/icon.png"></a></p>
 <h1 align="center">DVIS: 3D Visualizations made easy</h1>
 <h2 align="center">Visualize your data with just one line of code </h2>
 <h2 align="center">Python -> Browser </h2>
 
 
@@ -146,7 +148,9 @@
 | .      | Next frame          |
 | ,      | Previous frame          |
 | t      | Switch camera          |
 | [      | Download screenshot         |
 
 
 
+
+
```

## Comparing `dvis-0.8.7.6.dist-info/RECORD` & `dvis-0.8.8.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dvis/__init__.py,sha256=bfwoJN9nz_CchjmbhA9LJ0RKF1sHsInHrU4y79KfKpg,35
-dvis/dvis.py,sha256=i0KKL1ReHPpfcBJvM0DB__wYLrAnV_0pJlNDkQXVmrU,39040
+dvis/dvis.py,sha256=Dn_qauz74TAc91YcCWsmbMYBlMaItXzcXu2p2gigDnw,39221
 dvis/dvis_cli.py,sha256=ON6Hgf4fZLldr2kRYlcDszVr5aONASkJOv3fhW_B5cE,1525
-dvis/dvis_client.py,sha256=IuyqDe6B2K0pc9gJv0zCH3xUBKGuJTnPZRrJlFmmv-w,8263
+dvis/dvis_client.py,sha256=0YVf9-QfuK5e13QHjj042YnUJHiPjeDGyXwIyX0Ksgg,8314
 dvis/dvis_client_old.py,sha256=kJCMvv9fMB0o2xT1rXeFknTlYwxVipsmtR4XZD6jgHM,6060
 dvis/utils.py,sha256=HqiY7EByL6jGPmtFn01vrUOSYjqN9rGHwijWsr6uTJc,5510
-dvis-0.8.7.6.dist-info/METADATA,sha256=tEJ4LH3OwqEniTRQqzLakvHpww4lavFoQMupZiXIaHo,4228
-dvis-0.8.7.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dvis-0.8.7.6.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
-dvis-0.8.7.6.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
-dvis-0.8.7.6.dist-info/RECORD,,
+dvis-0.8.8.0.dist-info/METADATA,sha256=O1g3ap1tPM5N97dGNTZMdSzD5I9T_N8HpoHQqyEwmd0,4282
+dvis-0.8.8.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+dvis-0.8.8.0.dist-info/entry_points.txt,sha256=AK57kGESy22RMs5K6Ha2OWZhWcKpQ4C_77hPjfH9yuY,93
+dvis-0.8.8.0.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
+dvis-0.8.8.0.dist-info/RECORD,,
```

