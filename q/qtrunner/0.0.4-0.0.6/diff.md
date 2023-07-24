# Comparing `tmp/qtrunner-0.0.4-py2.py3-none-any.whl.zip` & `tmp/qtrunner-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 12214 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      165 b- defN 22-Jul-07 08:17 runner/__init__.py
+Zip file size: 16336 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-24 09:48 runner/__init__.py
 -rw-rw-rw-  2.0 fat      632 b- defN 22-Jun-20 14:04 runner/config.json
 -rw-rw-rw-  2.0 fat     2743 b- defN 22-Jul-07 07:46 runner/highlighter.py
--rw-rw-rw-  2.0 fat    12997 b- defN 22-Jul-07 08:18 runner/runner.py
+-rw-rw-rw-  2.0 fat    13495 b- defN 23-Jul-24 09:38 runner/main.py
+-rw-rw-rw-  2.0 fat    13266 b- defN 22-Sep-03 06:29 runner/runner.py
 -rw-rw-rw-  2.0 fat     1500 b- defN 22-Jun-19 09:40 runner/runner_adb.json
--rw-rw-rw-  2.0 fat      941 b- defN 22-Jul-07 07:46 runner/runner_common.json
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jul-24 09:44 runner/runner_common.json
 -rw-rw-rw-  2.0 fat      992 b- defN 22-Jun-19 15:13 runner/runner_network.json
 -rw-rw-rw-  2.0 fat     5700 b- defN 22-Jun-18 16:11 runner/runner_ui.py
 -rw-rw-rw-  2.0 fat     1306 b- defN 22-Jun-19 15:48 runner/runner_windwos.json
--rw-rw-rw-  2.0 fat     1067 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2023 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       40 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1188 b- defN 22-Jul-07 08:23 qtrunner-0.0.4.dist-info/RECORD
-15 files, 31411 bytes uncompressed, 10260 bytes compressed:  67.3%
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2148 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1260 b- defN 23-Jul-24 09:55 qtrunner-0.0.6.dist-info/RECORD
+16 files, 45504 bytes uncompressed, 14278 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: runner/config.json
 Comment: 
 
 Filename: runner/highlighter.py
 Comment: 
 
+Filename: runner/main.py
+Comment: 
+
 Filename: runner/runner.py
 Comment: 
 
 Filename: runner/runner_adb.json
 Comment: 
 
 Filename: runner/runner_common.json
@@ -21,26 +24,26 @@
 
 Filename: runner/runner_ui.py
 Comment: 
 
 Filename: runner/runner_windwos.json
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/LICENSE
+Filename: qtrunner-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/METADATA
+Filename: qtrunner-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/WHEEL
+Filename: qtrunner-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/entry_points.txt
+Filename: qtrunner-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/top_level.txt
+Filename: qtrunner-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: qtrunner-0.0.4.dist-info/RECORD
+Filename: qtrunner-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## runner/__init__.py

```diff
@@ -1,8 +1,8 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-__version__ = '0.0.4'
+__version__ = '0.0.6'
 __author__ = 'hufeng.mao'
 __author_email__ = 'hufeng.mao@carota.ai'
 
-from .runner import main
+from .main import main, Window
```

## runner/runner.py

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 '''
 Author: hufeng.mao@carota.ai
 Date: 2022-04-25 21:23:55
-LastEditTime: 2022-06-20 23:55:48
+LastEditTime: 2022-09-03 14:29:09
 Description: 快速启动器
 '''
 
 import json
 import sys
 import os
 import qtawesome as qta
@@ -80,15 +80,21 @@
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
         self.setupButtons()
         self.setupQss()
 
     def setupToolboxButtons(self, configPath):
         if not os.path.exists(configPath):
-            configPath = os.path.join(self.rp, configPath)
+            rp_configPath = os.path.join(self.rp, configPath)
+            if not os.path.exists(rp_configPath):
+                home_dir = os.path.expanduser('~')
+                configPath = os.path.join(home_dir, configPath)
+                print(configPath)
+            else:
+                configPath = rp_configPath
         with open(configPath, encoding="utf-8") as f:
             config = json.load(f)
 
             self.fadeIn(self.ui.toolBox)
             self.removeAll(self.ui.toolBoxLayout)
             for i, item in enumerate(config):
                 # print(cmd)
```

## runner/runner_common.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'insert': "[(7, OrderedDict([('title', '查看环境变量'), ('cmd', 'env'), ('env', "*

 * *           "OrderedDict([('GP_LANGUAGES', 'zh_CN')]))]))]"}*

```diff
@@ -32,9 +32,16 @@
         "qss": "color: rgb(150, 0, 0);",
         "title": "\u5207\u6362codepage\u5230gbk(\u614e\u7528)"
     },
     {
         "cmd": "cmd /c firewall.cpl",
         "cwd": "test",
         "title": "\u6253\u5f00\u9632\u706b\u5899"
+    },
+    {
+        "cmd": "env",
+        "env": {
+            "GP_LANGUAGES": "zh_CN"
+        },
+        "title": "\u67e5\u770b\u73af\u5883\u53d8\u91cf"
     }
 ]
```

## Comparing `qtrunner-0.0.4.dist-info/LICENSE` & `qtrunner-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qtrunner-0.0.4.dist-info/METADATA` & `qtrunner-0.0.6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtrunner
-Version: 0.0.4
+Version: 0.0.6
 Summary: 快速命令启动器
 Home-page: https://github.com/notmmao/runner
 Author: hufeng.mao
 Author-email: hufeng.mao@carota.ai
 License: MIT
 Keywords: qt,launcher
 Platform: windows
@@ -69,20 +69,23 @@
    }
 
 sub configuration file
 ~~~~~~~~~~~~~~~~~~~~~~
 
 runner_xxxx.json
 
-.. code:: json
+.. code:: js
 
    [
        {
            "title": "change codepage to gbk(use with caution)",  // title in ui
            "cmd": "cmd /c  chcp 936",          // command ling
            "encoding": "gbk",                  // output encoding
            "qss": "color: rgb(150, 0, 0);",    // ui styles in qss format
-           "cwd": ""                           // current working directory
-       }
+           "cwd": "",                          // current working directory
+           "env": {                            // environment variables 
+                "GP_LANGUAGE": "zh_CN"
+            }
+        }
    ]
```

## Comparing `qtrunner-0.0.4.dist-info/RECORD` & `qtrunner-0.0.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-runner/__init__.py,sha256=bMMjyWTO2OFRDDMxl1dVtvM9_HaX1Gm0E0DfWiqOS3E,165
+runner/__init__.py,sha256=ONR1uDxr_IW43_Zbg9Ijb8lDhFdJdaOjGlY_7CbwaPw,171
 runner/config.json,sha256=qYT9JfEOhMc10fFRc2MA1RIKata4zMkPZ8pN1hjc7lc,632
 runner/highlighter.py,sha256=IkgI0Hy3kYTCgGQGvroUGOpEU2_wVIg4dxbGL8o_88c,2743
-runner/runner.py,sha256=2GxZ-S2B63d_bRi9zKbMNJh0Wolu2w2lGjk3rwUTX8w,12997
+runner/main.py,sha256=8p4lxfNeeeQqaS7iBhQUv9cRY51ZuQqiAwdxabxjs0Y,13495
+runner/runner.py,sha256=q_kIsFTF9vbqZEKi6ABhdK7AW0o_7X8ffOb6mxvTQTI,13266
 runner/runner_adb.json,sha256=8AEvY4LE3F2zsZMj32lbfQWP8koJ5exHD3cyXI3G8gA,1500
-runner/runner_common.json,sha256=88FhihGivAmtwqd9A1jZU7AFRRF2D7YocATSs1sSSBI,941
+runner/runner_common.json,sha256=kGoZzARDXtXianSjWETDuDmtWcXERTfo2X1u2D7S6lw,1085
 runner/runner_network.json,sha256=o4wlfvjPGMykXfLvc8kw0bSlkmEV1qeDroTOeToebjo,992
 runner/runner_ui.py,sha256=YurVTck2pUG0wMPaFcHi05BK4Co1H8m0B0UHUzLn6Do,5700
 runner/runner_windwos.json,sha256=IFyqqZpiHoshCBD5mf0_16ansQaLQNxPz1ETY6frXYo,1306
-qtrunner-0.0.4.dist-info/LICENSE,sha256=-2R_b055eNF8rH_i7ibW4Fs3mnuWRasx7TgUVyDPNC4,1067
-qtrunner-0.0.4.dist-info/METADATA,sha256=ODCbVFAX6PtAEkLVnb0cfp1skar70OfRz2m3I4Pd8fM,2023
-qtrunner-0.0.4.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-qtrunner-0.0.4.dist-info/entry_points.txt,sha256=GwkXQ0eVfLZmag45M-k4NKjUCDhncz932Gsa4rmWcj4,40
-qtrunner-0.0.4.dist-info/top_level.txt,sha256=q0nz6xQujhjJT6edIBf1e2FBscTNwELxoNDj3lKXCQ4,7
-qtrunner-0.0.4.dist-info/RECORD,,
+qtrunner-0.0.6.dist-info/LICENSE,sha256=-2R_b055eNF8rH_i7ibW4Fs3mnuWRasx7TgUVyDPNC4,1067
+qtrunner-0.0.6.dist-info/METADATA,sha256=IRddxTNBlA6ayN-zLmattdnG23yUaLYJIEqk-zk_lb0,2148
+qtrunner-0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+qtrunner-0.0.6.dist-info/entry_points.txt,sha256=GwkXQ0eVfLZmag45M-k4NKjUCDhncz932Gsa4rmWcj4,40
+qtrunner-0.0.6.dist-info/top_level.txt,sha256=q0nz6xQujhjJT6edIBf1e2FBscTNwELxoNDj3lKXCQ4,7
+qtrunner-0.0.6.dist-info/RECORD,,
```

