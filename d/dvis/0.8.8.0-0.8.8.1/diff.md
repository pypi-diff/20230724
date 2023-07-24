# Comparing `tmp/dvis-0.8.8.0-py3-none-any.whl.zip` & `tmp/dvis-0.8.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18733 bytes, number of entries: 11
+Zip file size: 18730 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       35 b- defN 23-Jul-24 19:46 dvis/__init__.py
 -rw-r--r--  2.0 unx    39221 b- defN 23-Jul-24 20:08 dvis/dvis.py
--rw-r--r--  2.0 unx     1525 b- defN 23-Jul-24 19:46 dvis/dvis_cli.py
--rw-r--r--  2.0 unx     8314 b- defN 23-Jul-24 20:10 dvis/dvis_client.py
+-rw-r--r--  2.0 unx     1507 b- defN 23-Jul-24 20:49 dvis/dvis_cli.py
+-rw-r--r--  2.0 unx     8294 b- defN 23-Jul-24 20:52 dvis/dvis_client.py
 -rw-r--r--  2.0 unx     6060 b- defN 23-Jul-24 19:46 dvis/dvis_client_old.py
 -rw-r--r--  2.0 unx     5510 b- defN 23-Jul-24 19:46 dvis/utils.py
--rw-r--r--  2.0 unx     4282 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      827 b- defN 23-Jul-24 20:30 dvis-0.8.8.0.dist-info/RECORD
-11 files, 65964 bytes uncompressed, 17351 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     4282 b- defN 23-Jul-24 20:54 dvis-0.8.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:54 dvis-0.8.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-24 20:54 dvis-0.8.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 20:54 dvis-0.8.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      827 b- defN 23-Jul-24 20:54 dvis-0.8.8.1.dist-info/RECORD
+11 files, 65926 bytes uncompressed, 17348 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: dvis/dvis_client_old.py
 Comment: 
 
 Filename: dvis/utils.py
 Comment: 
 
-Filename: dvis-0.8.8.0.dist-info/METADATA
+Filename: dvis-0.8.8.1.dist-info/METADATA
 Comment: 
 
-Filename: dvis-0.8.8.0.dist-info/WHEEL
+Filename: dvis-0.8.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: dvis-0.8.8.0.dist-info/entry_points.txt
+Filename: dvis-0.8.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: dvis-0.8.8.0.dist-info/top_level.txt
+Filename: dvis-0.8.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dvis-0.8.8.0.dist-info/RECORD
+Filename: dvis-0.8.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dvis/dvis_cli.py

```diff
@@ -20,18 +20,19 @@
     parser.add_argument("--port", type=int, default=5001)
     parser.add_argument("--visdom_port", type=int, default=4999)
     parser.add_argument("--no_visdom", action="store_true")
     args = parser.parse_args()
 
     from subprocess import Popen
     # start dvis server:
-    dvis_server_cmd = f"cd server; conda run -n dvis_server python server.py --port {args.port}"
+    DVIS_ROOT = "."
+    dvis_server_cmd = f"cd {DVIS_ROOT}/server; python server.py --port {args.port}"
     commands = [dvis_server_cmd]
     print(f"DVIS server at: http://localhost:{args.port}")
     if not args.no_visdom:
-        visdom_cmd = f"conda run -n dvis_server visdom -p {args.visdom_port}"
+        visdom_cmd = f"visdom -p {args.visdom_port}"
         commands.append(visdom_cmd)
         print(f"Visdom server at: http://localhost:{args.visdom_port}")
     procs = [Popen(cmd, shell=True) for cmd in commands]
 
     for p in procs:
         p.wait()
```

## dvis/dvis_client.py

```diff
@@ -90,15 +90,14 @@
                 "t": t,
                 "graph_info": {"name": name},
                 "meta_data": meta_data,
                 "vis_conf": vis_conf,
                 "shape": shape,
             },
         )
-        print(PORT)
 
 
 def send_plotly(data, layout):
     vis = visdom.Visdom(port=VIS_PORT)
     print(f"Sending plolty {data['type']}")
     vis._send({"data": [data], "layout": layout})
```

## Comparing `dvis-0.8.8.0.dist-info/METADATA` & `dvis-0.8.8.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvis
-Version: 0.8.8.0
+Version: 0.8.8.1
 Summary: The best web-based visualizer
 Home-page: https://github.com/SirWyver/dvis
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

