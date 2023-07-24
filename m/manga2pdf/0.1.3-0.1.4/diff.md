# Comparing `tmp/manga2pdf-0.1.3.tar.gz` & `tmp/manga2pdf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga2pdf-0.1.3.tar", last modified: Wed Jul 19 12:01:01 2023, max compression
+gzip compressed data, was "manga2pdf-0.1.4.tar", last modified: Mon Jul 24 01:50:58 2023, max compression
```

## Comparing `manga2pdf-0.1.3.tar` & `manga2pdf-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.024741 manga2pdf-0.1.3/
--rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.3/LICENSE
--rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-19 12:01:01.024643 manga2pdf-0.1.3/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)     5623 2023-05-03 09:26:06.000000 manga2pdf-0.1.3/README.md
--rw-r--r--   0 shun       (501) staff       (20)       38 2023-07-19 12:01:01.024778 manga2pdf-0.1.3/setup.cfg
--rw-r--r--   0 shun       (501) staff       (20)     1065 2023-07-19 09:51:27.000000 manga2pdf-0.1.3/setup.py
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.023934 manga2pdf-0.1.3/src/
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.024519 manga2pdf-0.1.3/src/manga2pdf.egg-info/
--rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)      288 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 shun       (501) staff       (20)        1 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 shun       (501) staff       (20)       45 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/entry_points.txt
--rw-r--r--   0 shun       (501) staff       (20)       52 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/requires.txt
--rw-r--r--   0 shun       (501) staff       (20)       24 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/top_level.txt
--rw-r--r--   0 shun       (501) staff       (20)    18928 2023-07-19 09:51:11.000000 manga2pdf-0.1.3/src/manga2pdf.py
--rw-r--r--   0 shun       (501) staff       (20)    18123 2023-07-19 11:42:46.000000 manga2pdf-0.1.3/src/manga2pdf_gui.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-24 01:50:58.899622 manga2pdf-0.1.4/
+-rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.4/LICENSE
+-rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-24 01:50:58.899519 manga2pdf-0.1.4/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)     5623 2023-05-03 09:26:06.000000 manga2pdf-0.1.4/README.md
+-rw-r--r--   0 shun       (501) staff       (20)       38 2023-07-24 01:50:58.899700 manga2pdf-0.1.4/setup.cfg
+-rw-r--r--   0 shun       (501) staff       (20)     1065 2023-07-24 01:43:08.000000 manga2pdf-0.1.4/setup.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-24 01:50:58.898517 manga2pdf-0.1.4/src/
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-24 01:50:58.899391 manga2pdf-0.1.4/src/manga2pdf.egg-info/
+-rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)      288 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 shun       (501) staff       (20)        1 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 shun       (501) staff       (20)       45 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 shun       (501) staff       (20)       52 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/requires.txt
+-rw-r--r--   0 shun       (501) staff       (20)       24 2023-07-24 01:50:58.000000 manga2pdf-0.1.4/src/manga2pdf.egg-info/top_level.txt
+-rw-r--r--   0 shun       (501) staff       (20)    18928 2023-07-19 09:51:11.000000 manga2pdf-0.1.4/src/manga2pdf.py
+-rw-r--r--   0 shun       (501) staff       (20)    20154 2023-07-24 01:42:44.000000 manga2pdf-0.1.4/src/manga2pdf_gui.py
```

### Comparing `manga2pdf-0.1.3/LICENSE` & `manga2pdf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.3/PKG-INFO` & `manga2pdf-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.1.3/README.md` & `manga2pdf-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.3/setup.py` & `manga2pdf-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 INSTALL_REQUIRES = (
     "numpy",
     "img2pdf",
     "Pillow",
     "pikepdf",
     "rarfile",
```

### Comparing `manga2pdf-0.1.3/src/manga2pdf.egg-info/PKG-INFO` & `manga2pdf-0.1.4/src/manga2pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.1.3/src/manga2pdf.py` & `manga2pdf-0.1.4/src/manga2pdf.py`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.3/src/manga2pdf_gui.py` & `manga2pdf-0.1.4/src/manga2pdf_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,126 +1,155 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2023 mashu3
 # This software is released under the MIT License, see LICENSE.
 
 import os
 import sys
+import platform
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog
 from tkinter import messagebox
 from manga2pdf import MangaPdfConverter
 
 class MangaPdfConverterGUI:
     def __init__(self, master):
         self.master = master
         self.language = "en" # Set default language to english
         master.title("Manga PDF Converter")
         self.master.resizable(0, 0)
         self.processing_window = None
+        self.system = platform.system()
 
         # Create five frames
         path_frame =ttk.Frame(master)
         conversion_frame = ttk.Frame(master)
-        pagelayout_frame = ttk.Frame(master)
         direction_frame = ttk.Frame(master)
+        pagelayout_frame = ttk.Frame(master)
+        pagemode_frame = ttk.Frame(master)
         button_frame = ttk.Frame(master)
 
         # Set grid layout
         path_frame.grid(row=0, column=0, columnspan=3, sticky='we')
         conversion_frame.grid(row=1, column=0, sticky='nswe')
-        pagelayout_frame.grid(row=1, column=1, sticky='nswe')
-        direction_frame.grid(row=1, column=2, sticky='nswe')
-        button_frame.grid(row=2, column=0, columnspan=3, sticky='we')
+        direction_frame.grid(row=2, column=0, sticky='nswe')
+        pagelayout_frame.grid(row=1, column=1, rowspan=2, sticky='nswe')
+        pagemode_frame.grid(row=1, column=2, rowspan=2, sticky='nswe')
+        button_frame.grid(row=3, column=0, columnspan=3, sticky='we')
 
         # Add input path label and entry
         input_frame = ttk.Frame(path_frame)
         input_frame.grid(row=0, column=0, columnspan=3, padx=5, pady=5, sticky="ew")
         self.input_label_text = {"en": "Input Path:", "ja": "入力パス:"}
         self.input_label = ttk.Label(input_frame, text=self.input_label_text[self.language])
         self.input_label.pack(side="left", padx=10, pady=5)
         self.input_file_button_text = {"en": "Select File", "ja": "ファイル選択"}
         self.input_file_button = ttk.Button(input_frame, text=self.input_file_button_text[self.language], command=self.browse_input_file)
         self.input_file_button.pack(side="right", pady=5)
         self.input_directory_button_text = {"en": "Select Directory", "ja": "フォルダ選択"}
         self.input_directory_button = ttk.Button(input_frame, text=self.input_directory_button_text[self.language], command=self.browse_input_directory)
         self.input_directory_button.pack(side="right", padx=10, pady=5)
-        self.input_entry = ttk.Entry(path_frame, width=65)
+        if self.system == "Windows":
+            self.input_entry = ttk.Entry(path_frame, width=90)
+        else:
+            self.input_entry = ttk.Entry(path_frame, width=65)
         self.input_entry.grid(row=1, column=0, columnspan=3, padx=10, pady=5, sticky="ew")
 
         # Add output path label and entry
         output_frame = tk.Frame(path_frame)
         output_frame.grid(row=2, column=0, columnspan=3, padx=5, pady=5, sticky="ew")
         self.output_label_text = {"en": "Output Path:", "ja": "出力パス:"}
         self.output_label = ttk.Label(output_frame, text=self.output_label_text[self.language])
         self.output_label.pack(side="left", padx=10, pady=5)
         self.output_browse_button_text = {"en": "Browse", "ja": "参照"}
         self.output_browse_button = ttk.Button(output_frame, text=self.output_browse_button_text[self.language], command=self.browse_output_path)
         self.output_browse_button.pack(side="right", pady=5)
         self.auto_output_button_text = {"en": "Auto", "ja": "自動設定"}
         self.auto_output_button = ttk.Button(output_frame, text=self.auto_output_button_text[self.language], command=self.auto_output_path)
         self.auto_output_button.pack(side="right", padx=10, pady=5)
-        self.output_entry = ttk.Entry(path_frame, width=65)
+        if self.system == "Windows":
+            self.output_entry = ttk.Entry(path_frame, width=90)
+        else:
+            self.output_entry = ttk.Entry(path_frame, width=65)
         self.output_entry.grid(row=3, column=0, columnspan=3, padx=10, pady=5, sticky="ew")
 
         # Create a LabelFrame for the conversion options
         self.conversion_label_text = {"en": "Conversion Options:", "ja": "圧縮方式:"}
         self.conversion_labelframe = ttk.LabelFrame(conversion_frame, text=self.conversion_label_text[self.language], padding=5)
-        self.conversion_labelframe.grid(row=0, column=0, rowspan=10, sticky="nsew", padx=5, pady=1)
+        self.conversion_labelframe.grid(row=0, column=0, rowspan=5, sticky="nsew", padx=2, pady=1)
 
         self.conversion_var = tk.StringVar(value="none")
         self.conversion_text = {
             "en": ["No Compression", "Convert images to JPEG", "Convert images to grayscale"],
             "ja": ["圧縮なし", "JPEG画像に変換", "グレースケール画像に変換"],
         }
         self.conversion_value = ["none", "jpeg", "grayscale"]
         self.conversion_radio = []
         for i, conversion in enumerate(self.conversion_text[self.language]):
             conversion_radio = ttk.Radiobutton(
                 self.conversion_labelframe, text=conversion, variable=self.conversion_var, value=self.conversion_value[i]
             )
             self.conversion_radio.append(conversion_radio)
-            conversion_radio.grid(row=i+1, column=0, sticky="nsew", padx=5, pady=1)
+            conversion_radio.grid(row=i+1, column=0, sticky="nsew", padx=2, pady=1)
+
+        # Create a LabelFrame for the direction options
+        self.direction_label_text = {"en": "Direction:", "ja": "綴じ方向:"}
+        self.direction_labelframe = ttk.LabelFrame(direction_frame, text=self.direction_label_text[self.language], padding=5)
+        self.direction_labelframe.grid(row=0, column=0, rowspan=5, sticky="nsew", padx=2, pady=1)
+
+        self.direction_var = tk.StringVar(value="R2L")
+        self.direction_text = {
+            "en": ["L2R", "R2L"],
+            "ja": ["左綴じ", "右綴じ"],
+        }
+        self.direction_value = ["L2R", "R2L"]
+        self.direction_radio = []
+        for i, direction in enumerate(self.direction_text[self.language]):
+            direction_radio = ttk.Radiobutton(
+                self.direction_labelframe, text=direction, variable=self.direction_var, value=self.direction_value[i])
+            self.direction_radio.append(direction_radio)
+            direction_radio.grid(row=i+1, column=0, sticky="nsew", padx=2, pady=1)
         
         # Create a LabelFrame for the page layout options
         self.pagelayout_label_text = {"en": "Page Layout:", "ja": "ページレイアウト:"}
         self.pagelayout_labelframe = ttk.LabelFrame(pagelayout_frame, text=self.pagelayout_label_text[self.language], padding=5)
-        self.pagelayout_labelframe.grid(row=0, column=1, rowspan=10, sticky="nsew", padx=5, pady=1)
+        self.pagelayout_labelframe.grid(row=0, column=0, rowspan=10, sticky="nsew", padx=2, pady=1)
 
         self.pagelayout_var = tk.StringVar(value="TwoPageRight")
         self.pagelayout_text = {
             "en": ["SinglePage", "OneColumn", "TwoPageLeft", "TwoColumnLeft", "TwoPageRight", "TwoColumnRight"],
             "ja": ["単一ページ表示", "スクロールを有効にする", "見開きページ表示", "見開きページでスクロール", "見開きページ\n(表紙は単独表示)", "見開きページでスクロール\n(表紙は単独表示)"],
         }
         self.pagelayout_value = ["SinglePage", "OneColumn", "TwoPageLeft", "TwoColumnLeft", "TwoPageRight", "TwoColumnRight"]
         self.pagelayout_radio = []
         for i, pagelayout in enumerate(self.pagelayout_text[self.language]):
             pagelayout_radio = ttk.Radiobutton(
                 self.pagelayout_labelframe, text=pagelayout, variable=self.pagelayout_var, value=self.pagelayout_value[i]
             )
             self.pagelayout_radio.append(pagelayout_radio)
-            pagelayout_radio.grid(row=i+1, column=1, sticky="nsew", padx=5, pady=1)
+            pagelayout_radio.grid(row=i+1, column=0, sticky="nsew", padx=2, pady=1)
 
-        # Create a LabelFrame for the direction options
-        self.direction_label_text = {"en": "Direction:", "ja": "綴じ方向:"}
-        self.direction_labelframe = ttk.LabelFrame(direction_frame, text=self.direction_label_text[self.language], padding=5)
-        self.direction_labelframe.grid(row=0, column=2, rowspan=10, sticky="nsew", padx=5, pady=1)
-
-        self.direction_var = tk.StringVar(value="R2L")
-        self.direction_text = {
-            "en": ["L2R", "R2L"],
-            "ja": ["左綴じ", "右綴じ"],
+        # Create a LabelFrame for the page mode options
+        self.pagemode_label_text = {"en": "Page Mode:", "ja": "ページモード:"}
+        self.pagemode_labelframe = ttk.LabelFrame(pagemode_frame, text=self.pagemode_label_text[self.language], padding=5)
+        self.pagemode_labelframe.grid(row=0, column=0, rowspan=10, sticky="nsew", padx=2, pady=1)
+
+        self.pagemode_var = tk.StringVar(value="UseNone")
+        self.pagemode_text = {
+            "en": ["UseNone", "UseOutlines", "UseThumbs", "FullScreen", "UseOC", "UseAttachments"],
+            "ja": ["デフォルト表示", "アウトラインパネルを表示", "サムネイルパネルを表示", "フルスクリーンモード", "コンテンツパネルを表示", "添付ファイルパネルを表示"],
         }
-        self.direction_value = ["L2R", "R2L"]
-        self.direction_radio = []
-        for i, direction in enumerate(self.direction_text[self.language]):
-            direction_radio = ttk.Radiobutton(
-                self.direction_labelframe, text=direction, variable=self.direction_var, value=self.direction_value[i])
-            self.direction_radio.append(direction_radio)
-            direction_radio.grid(row=i+1, column=2, sticky="nsew", padx=5, pady=1)
+        self.pagemode_value = ["UseNone", "UseOutlines", "UseThumbs", "FullScreen", "UseOC", "UseAttachments"]
+        self.pagemode_radio = []
+        for i, pagemode in enumerate(self.pagemode_text[self.language]):
+            pagemode_radio = ttk.Radiobutton(
+                self.pagemode_labelframe, text=pagemode, variable=self.pagemode_var, value=self.pagemode_value[i]
+            )
+            self.pagemode_radio.append(pagemode_radio)
+            pagemode_radio.grid(row=i+1, column=0, sticky="nsew", padx=2, pady=1)
 
         # Add language toggle button
         self.language_button_text = {"en": "日本語表示に切替", "ja": "Display in English"}
         self.language_button = ttk.Button(button_frame, text=self.language_button_text[self.language], command=self.toggle_language)
         self.language_button.pack(side="left", padx=15, pady=5)
 
         # Add quit button
@@ -160,22 +189,26 @@
         self.output_label.configure(text=self.output_label_text[self.language])
         self.output_browse_button.configure(text=self.output_browse_button_text[self.language])
         self.auto_output_button.configure(text=self.auto_output_button_text[self.language])
         self.conversion_labelframe.configure(text=self.conversion_label_text[self.language])
         for i, conversion in enumerate(self.conversion_text[self.language]):
             self.conversion_radio[i].configure(text=conversion)
         self.conversion_var.set(self.conversion_var.get())
-        self.pagelayout_labelframe.configure(text=self.pagelayout_label_text[self.language])
-        for i, pagelayout in enumerate(self.pagelayout_text[self.language]):
-            self.pagelayout_radio[i].configure(text=pagelayout)
-        self.pagelayout_var.set(self.pagelayout_var.get())
         self.direction_labelframe.configure(text=self.direction_label_text[self.language])
         for i, direction in enumerate(self.direction_text[self.language]):
             self.direction_radio[i].configure(text=direction)
         self.direction_var.set(self.direction_var.get())
+        self.pagelayout_labelframe.configure(text=self.pagelayout_label_text[self.language])
+        for i, pagelayout in enumerate(self.pagelayout_text[self.language]):
+            self.pagelayout_radio[i].configure(text=pagelayout)
+        self.pagemode_var.set(self.pagemode_var.get())
+        self.pagemode_labelframe.configure(text=self.pagemode_label_text[self.language])
+        for i, pagemode in enumerate(self.pagemode_text[self.language]):
+            self.pagemode_radio[i].configure(text=pagemode)
+        self.pagelayout_var.set(self.pagelayout_var.get())
         self.language_button.configure(text=self.language_button_text[self.language])
         self.convert_button.configure(text=self.convert_button_text[self.language])
         self.quit_button.configure(text=self.quit_button_text[self.language])
 
     def set_output_path(self, path):
         self.output_path = path
         self.output_entry.delete(0, tk.END)
@@ -266,15 +299,15 @@
         
         # Determine the conversion options
         convert_to_jpeg = self.conversion_var.get() == "jpeg"
         convert_to_grayscale = self.conversion_var.get() == "grayscale"
 
         # Call MangaPdfConverter with the appropriate arguments
         try:
-            converter = MangaPdfConverter(input_path=input_path, output_path=output_path, pagelayout=self.pagelayout_var.get(), pagemode='UseNone', direction=self.direction_var.get())
+            converter = MangaPdfConverter(input_path=input_path, output_path=output_path, pagelayout=self.pagelayout_var.get(), pagemode=self.pagemode_var.get(), direction=self.direction_var.get())
 
             # Ask user if they want to convert
             confirm_text = {"en": "Are you sure you want to convert?", "ja": "変換処理を開始しますか？"}
             answer = messagebox.askyesno("Confirm Conversion", confirm_text[self.language], parent=self.master)
 
             if not answer:
                 cancele_text = {"en": "Conversion canceled.", "ja": "変換処理を中止しました"}
```

