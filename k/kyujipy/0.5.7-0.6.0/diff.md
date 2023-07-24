# Comparing `tmp/kyujipy-0.5.7.tar.gz` & `tmp/kyujipy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyujipy-0.5.7.tar", max compression
+gzip compressed data, was "kyujipy-0.6.0.tar", max compression
```

## Comparing `kyujipy-0.5.7.tar` & `kyujipy-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1077 2021-11-14 00:57:05.859995 kyujipy-0.5.7/LICENSE
--rw-r--r--   0        0        0     1510 2023-07-05 11:49:55.172738 kyujipy-0.5.7/README.md
--rw-r--r--   0        0        0       93 2021-11-14 00:57:05.860195 kyujipy-0.5.7/kyujipy/__init__.py
--rw-r--r--   0        0        0     6460 2021-11-14 00:57:05.860273 kyujipy-0.5.7/kyujipy/converter.py
--rw-r--r--   0        0        0      850 2021-11-14 00:57:05.860338 kyujipy-0.5.7/kyujipy/export_to_json.py
--rw-r--r--   0        0        0    16420 2021-11-14 00:57:05.860496 kyujipy-0.5.7/kyujipy/kakikae_simplified.cson
--rw-r--r--   0        0        0    25066 2021-11-14 00:57:05.860575 kyujipy-0.5.7/kyujipy/kakikae_variants.cson
--rw-r--r--   0        0        0     9740 2021-11-14 00:57:05.860670 kyujipy-0.5.7/kyujipy/kyujitai.cson
--rw-r--r--   0        0        0      573 2023-07-20 17:30:07.766385 kyujipy-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 kyujipy-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-11-14 00:57:05.859995 kyujipy-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1510 2023-07-22 12:52:54.739419 kyujipy-0.6.0/README.md
+-rw-r--r--   0        0        0       93 2021-11-14 00:57:05.860195 kyujipy-0.6.0/kyujipy/__init__.py
+-rw-r--r--   0        0        0     6938 2023-07-24 18:02:46.122467 kyujipy-0.6.0/kyujipy/converter.py
+-rw-r--r--   0        0        0      882 2023-07-22 23:28:08.240324 kyujipy-0.6.0/kyujipy/export_to_json.py
+-rw-r--r--   0        0        0    16411 2023-07-24 18:19:29.653935 kyujipy-0.6.0/kyujipy/kakikae_simplified.cson
+-rw-r--r--   0        0        0    25084 2023-07-24 18:19:29.672204 kyujipy-0.6.0/kyujipy/kakikae_variants.cson
+-rw-r--r--   0        0        0     9700 2023-07-24 17:10:55.672160 kyujipy-0.6.0/kyujipy/kyujitai_simplified.cson
+-rw-r--r--   0        0        0      542 2023-07-22 23:18:01.161020 kyujipy-0.6.0/kyujipy/kyujitai_variants.cson
+-rw-r--r--   0        0        0      573 2023-07-24 18:20:29.209199 kyujipy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 kyujipy-0.6.0/PKG-INFO
```

### Comparing `kyujipy-0.5.7/LICENSE` & `kyujipy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.7/README.md` & `kyujipy-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.7/kyujipy/converter.py` & `kyujipy-0.6.0/kyujipy/converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import cson
 import os
 
 EXCEPTIONS_KYUJITAI = {
     '缺缺': '欠缺',
-    '共倭國': '共和國',
 }
 
 EXCEPTIONS_SHINJITAI = {
     '欠欠': '欠缺',
 }
 
+
 class BasicConverter(object):
     """
     Basic converter, only converting Shinjitai to Kyujitai, and vice versa (WITHOUT kakikae)
     """
 
     def __init__(self):
 
         # Determine Shinjitai/Kyujitai database path
         current_path = os.path.abspath(os.path.dirname(__file__))
-        kyujitai_db_path = os.path.join(current_path, 'kyujitai.cson')
+        kyujitai_simplified_db_path = os.path.join(current_path, 'kyujitai_simplified.cson')
+        kyujitai_variants_db_path = os.path.join(current_path, 'kyujitai_variants.cson')
 
         # Parse Kyujitai database
-        kyujitai_db_file = open(kyujitai_db_path, 'r', encoding="utf-8")
-        self.kyujitai_data = cson.load(kyujitai_db_file)
-        kyujitai_db_file.close()
+        with open(kyujitai_simplified_db_path, 'r', encoding="utf-8") as kyujitai_simplified_db_file:
+            self.kyujitai_data_simplified = cson.load(kyujitai_simplified_db_file)
+        with open(kyujitai_variants_db_path, 'r', encoding="utf-8") as kyujitai_variants_db_file:
+            self.kyujitai_data_variants = cson.load(kyujitai_variants_db_file)
 
         # Build Shinjitai to Kyujitai conversion databases
         self.shinjitai_to_kyujitai_database = {}
         self.kyujitai_to_shinjitai_database = {}
 
         # create Shinjitai/Kyujitai dictionaries
-        for entry in self.kyujitai_data:
+        for entry in self.kyujitai_data_simplified:
             shinjitai = entry[0]
             kyujitai = entry[1]
             self.shinjitai_to_kyujitai_database[shinjitai] = kyujitai
             self.kyujitai_to_shinjitai_database[kyujitai] = shinjitai
 
+        for entry in self.kyujitai_data_variants:
+            shinjitai = entry[0]
+            kyujitai = entry[1]
+            self.kyujitai_to_shinjitai_database[kyujitai] = shinjitai
+
     def shinjitai_to_kyujitai(self, input_string):
 
         # convert individual characters
         for char in self.shinjitai_to_kyujitai_database:
             input_string = input_string.replace(char, self.shinjitai_to_kyujitai_database[char])
 
         # process conversion exceptions
```

### Comparing `kyujipy-0.5.7/kyujipy/export_to_json.py` & `kyujipy-0.6.0/kyujipy/export_to_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cson
 import json
 import os
 import sys
 
-DATA_FILES = ['kyujitai', 'kakikae_simplified', 'kakikae_variants']
+DATA_FILES = ['kyujitai_simplified', 'kyujitai_variants', 'kakikae_simplified', 'kakikae_variants']
 
 
 if __name__ == '__main__':
 
     if len(sys.argv) != 2:
         raise ValueError('Please give output path as parameter.')
```

### Comparing `kyujipy-0.5.7/kyujipy/kakikae_simplified.cson` & `kyujipy-0.6.0/kyujipy/kakikae_simplified.cson`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,19 @@
     }
     {
         new: "記"
         old: ["徽"]
         words: ["記章"]
     }
     {
+        new: "奇"
+        old: ["詭"]
+        words: ["奇弁"]
+    }
+    {
         new: "弁"
         old: ["辯"]
         words: ["奇弁","弁舌","弁解","弁護","弁難","弁明","弁論","抗弁","陳弁","答弁","論弁","口弁","多弁","駄弁","訥弁","熱弁","能弁","雄弁","大阪弁","関東弁","京都弁","博多弁","広島弁","津軽弁","秋田弁","東北弁","仙台弁","東京弁","新潟弁","信州弁","名古屋弁","関西弁","岡山弁","沖縄弁"]
     }
     {
         new: "技"
         old: ["伎"]
@@ -433,15 +438,15 @@
         new: "集"
         old: ["聚"]
         words: ["集落","積集"]
     }
     {
         new: "集"
         old: ["輯"]
-        words: ["集録","編集","特集"]
+        words: ["編集","特集"]
     }
     {
         new: "俊"
         old: ["駿"]
         words: ["俊馬"]
     }
     {
@@ -793,15 +798,15 @@
         new: "役"
         old: ["軛"]
         words: ["共役"]
     }
     {
         new: "遊"
         old: ["游"]
-        words: ["遊泳","遊動","浮遊"]
+        words: ["遊泳","遊弋","遊動","浮遊"]
     }
     {
         new: "世"
         old: ["輿"]
         words: ["世論"]
     }
     {
@@ -863,15 +868,15 @@
         new: "陵"
         old: ["凌"]
         words: ["陵駕","陵辱"]
     }
     {
         new: "励"
         old: ["厲"]
-        words: ["励声"]
+        words: ["励声","励行"]
     }
     {
         new: "歴"
         old: ["瀝"]
         words: ["披歴"]
     }
     {
@@ -886,19 +891,14 @@
     }
     {
         new: "録"
         old: ["禄"]
         words: ["貫録"]
     }
     {
-        new: "和"
-        old: ["倭"]
-        words: ["和人","和語","和国"]
-    }
-    {
         new: "湾"
         old: ["弯"]
         words: ["湾曲"]
     }
     {
         new: "順"
         old: ["遵"]
```

### Comparing `kyujipy-0.5.7/kyujipy/kakikae_variants.cson` & `kyujipy-0.6.0/kyujipy/kakikae_variants.cson`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         new: "回"
         old: ["洄"]
         words: ["回遊"]
     }
     {
         new: "遊"
         old: ["游"]
-        words: ["回遊","遊弋","遊侠","遊民","遊魚","群遊"]
+        words: ["回遊","遊侠","遊民","遊魚","群遊"]
     }
     {
         new: "貝"
         old: ["頴"]
         words: ["貝割"]
     }
     {
@@ -631,14 +631,19 @@
     }
     {
         new: "集"
         old: ["聚"]
         words: ["群集","凝集"]
     }
     {
+        new: "集"
+        old: ["輯"]
+        words: ["集録"]
+    }
+    {
         new: "俊"
         old: ["駿"]
         words: ["俊才","俊足","優俊"]
     }
     {
         new: "俊"
         old: ["儁"]
@@ -1261,19 +1266,14 @@
     }
     {
         new: "涼"
         old: ["寥"]
         words: ["荒涼"]
     }
     {
-        new: "励"
-        old: ["厲"]
-        words: ["励行"]
-    }
-    {
         new: "練"
         old: ["煉"]
         words: ["練薬","試練","洗練"]
     }
     {
         new: "練"
         old: ["煉","錬"]
@@ -1283,15 +1283,15 @@
         new: "連"
         old: ["聯"]
         words: ["連碁","連珠","連弾","連歌","連絡","連繋","関連"]
     }
     {
         new: "和"
         old: ["倭"]
-        words: ["和学","和歌","和名","和朝"]
+        words: ["和人","和学","和歌","和語","和名","和国","和朝"]
     }
     {
         new: "湾"
         old: ["弯"]
         words: ["湾入","湾月","湾屈","側湾症"]
     }
     {
```

### Comparing `kyujipy-0.5.7/kyujipy/kyujitai.cson` & `kyujipy-0.6.0/kyujipy/kyujitai_simplified.cson`

 * *Files 4% similar despite different names*

```diff
@@ -405,37 +405,32 @@
     ["廊", "廊"],
     ["楼", "樓"],
     ["篭", "籠"],
     ["録", "錄"],
     ["湾", "灣"],
 
     # 人名用漢字
-    ["亘", "亙"],
-    ["凛", "凜"],
     ["尭", "堯"],
     ["巌", "巖"],
     ["掴", "摑"],
-    ["晃", "晄"],
     ["彦", "彥"],
-    ["晋", "晉"],
     ["桧", "檜"],
     ["槙", "槇"],
     ["渚", "渚"],
     ["猪", "猪"],
     ["琢", "琢"],
     ["瑶", "瑤"],
     ["祢", "禰"],
     ["祐", "祐"],
     ["祷", "禱"],
     ["禄", "祿"],
     ["禎", "禎"],
     ["穣", "穰"],
     ["箪", "簞"],
     ["聡", "聰"],
-    ["萌", "萠"],
     ["蓮", "蓮"],
     ["蘭", "蘭"],
     ["遥", "遙"],
     ["遼", "遼"],
     ["靖", "靖"],
 
     # 表外字 (擴張新字體)
@@ -460,16 +455,19 @@
     ["芦", "蘆"],
     ["蝋", "蠟"],
     ["弯", "彎"],
     ["焔", "焰"],
     ["砿", "礦"],
     ["讃", "讚"],
     ["顛", "顚"],
+    ["巔", "巓"],
     ["醗", "醱"],
     ["溌", "潑"],
     ["輌", "輛"],
     ["繋", "繫"],
     ["涜", "瀆"],
     ["侭", "儘"],
     ["薮", "藪"],
     ["蝿", "蠅"],
+    ["媯", "嬀"],
+    ["騨", "驒"],
 ]
```

### Comparing `kyujipy-0.5.7/pyproject.toml` & `kyujipy-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kyujipy"
-version = "0.5.7"
+version = "0.6.0"
 description = "A Python library to convert Japanese texts from Shinjitai to Kyujitai and vice versa"
 authors = ["Emmanuel Ternon <emmanuel.ternon@outlook.com>"]
 license="MIT"
 readme = "README.md"
 homepage = "https://github.com/DrTurnon/kyujipy"
 repository = "https://github.com/DrTurnon/kyujipy"
 include = [
```

### Comparing `kyujipy-0.5.7/PKG-INFO` & `kyujipy-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyujipy
-Version: 0.5.7
+Version: 0.6.0
 Summary: A Python library to convert Japanese texts from Shinjitai to Kyujitai and vice versa
 Home-page: https://github.com/DrTurnon/kyujipy
 License: MIT
 Author: Emmanuel Ternon
 Author-email: emmanuel.ternon@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

