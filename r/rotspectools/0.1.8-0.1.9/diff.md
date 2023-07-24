# Comparing `tmp/rotspectools-0.1.8.tar.gz` & `tmp/rotspectools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.8.tar", max compression
+gzip compressed data, was "rotspectools-0.1.9.tar", max compression
```

## Comparing `rotspectools-0.1.8.tar` & `rotspectools-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.8/LICENSE
--rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.8/README.rst
--rw-r--r--   0        0        0      459 2023-06-16 16:02:57.596675 rotspectools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.8/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-16 16:02:50.726502 rotspectools-0.1.8/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.8/rotspectools/cli.py
--rw-r--r--   0        0        0    25144 2023-06-16 15:59:59.516654 rotspectools-0.1.8/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.9/README.rst
+-rw-r--r--   0        0        0      459 2023-07-24 16:45:19.033525 rotspectools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.9/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-07-24 16:43:26.265311 rotspectools-0.1.9/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.9/rotspectools/cli.py
+-rw-r--r--   0        0        0    27246 2023-07-24 16:40:49.923724 rotspectools-0.1.9/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.9/PKG-INFO
```

### Comparing `rotspectools-0.1.8/LICENSE` & `rotspectools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.8/README.rst` & `rotspectools-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.8/rotspectools/.DS_Store` & `rotspectools-0.1.9/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.8/rotspectools/rotspectools.py` & `rotspectools-0.1.9/rotspectools/rotspectools.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,22 +264,25 @@
         df_IR = df.loc[df["Delta_v"] != 0]
         return df_IR
 
     def get_rot(self, df: DataFrame) -> DataFrame:
         df_rot = df.loc[df["Delta_v"] == 0]
         return df_rot
 
-    def plot_data_dist(self, max_Ka: int, max_J: int):
+    def plot_data_dist_rot_color(self, max_Ka: int, max_J: int):
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
+        text_x_pos = max_Ka - 22
+        text_y_pos = max_J - 10
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
+        dataframes = tuple(map(self.get_rot, dataframes))
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
@@ -332,24 +335,24 @@
         ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[0].set_xlabel("$K_a''$", fontsize=14)
         ax[0].set_ylabel("$J''$", fontsize=14)
         ax[0].set_ylim(0, max_J)
         ax[0].set_xlim(-0.5, max_Ka)
         ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[0].text(38, 110, "R-Branch", fontsize=18)
+        ax[0].text(text_x_pos, text_y_pos, "R-Branch", fontsize=18)
 
         ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[1].set_xlabel("$K_a''$", fontsize=14)
         ax[1].set_ylabel("$J''$", fontsize=14)
         ax[1].set_ylim(0, max_J)
         ax[1].set_xlim(-0.5, max_Ka)
         ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[1].text(38, 110, "Q-Branch", fontsize=18)
+        ax[1].text(text_x_pos, text_y_pos, "Q-Branch", fontsize=18)
 
         c = [
             mpatches.Circle(
                 (0.5, 0.5),
                 radius=0.25,
                 facecolor="#0000FF65",
                 edgecolor="blue",
@@ -406,23 +409,25 @@
             handler_map={mpatches.Circle: HandlerEllipse()},
         )
         frame1 = legend1.get_frame()
         frame1.set_linewidth(0.5)
         file_path = self.file_name + ".jpg"
         fig.savefig(file_path, dpi=800)
 
-    def plot_data_dist_rot(self, max_Ka: int, max_J: int):
+    def plot_data_dist_IR_color(self, max_Ka: int, max_J: int):
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
+        text_x_pos = max_Ka - 22
+        text_y_pos = max_J - 10
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(map(self.get_rot, dataframes))
+        dataframes = tuple(map(self.get_IR, dataframes))
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
@@ -475,24 +480,24 @@
         ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[0].set_xlabel("$K_a''$", fontsize=14)
         ax[0].set_ylabel("$J''$", fontsize=14)
         ax[0].set_ylim(0, max_J)
         ax[0].set_xlim(-0.5, max_Ka)
         ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[0].text(38, 110, "R-Branch", fontsize=18)
+        ax[0].text(text_x_pos, text_y_pos, "R-Branch", fontsize=18)
 
         ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[1].set_xlabel("$K_a''$", fontsize=14)
         ax[1].set_ylabel("$J''$", fontsize=14)
         ax[1].set_ylim(0, max_J)
         ax[1].set_xlim(-0.5, max_Ka)
         ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[1].text(38, 110, "Q-Branch", fontsize=18)
+        ax[1].text(text_x_pos, text_y_pos, "Q-Branch", fontsize=18)
 
         c = [
             mpatches.Circle(
                 (0.5, 0.5),
                 radius=0.25,
                 facecolor="#0000FF65",
                 edgecolor="blue",
@@ -549,37 +554,39 @@
             handler_map={mpatches.Circle: HandlerEllipse()},
         )
         frame1 = legend1.get_frame()
         frame1.set_linewidth(0.5)
         file_path = self.file_name + ".jpg"
         fig.savefig(file_path, dpi=800)
 
-    def plot_data_dist_IR(self, max_Ka: int, max_J: int):
+    def plot_data_dist_rot_pub(self, max_Ka: int, max_J: int):
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
+        text_x_pos = max_Ka - 22
+        text_y_pos = max_J - 10
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(map(self.get_IR, dataframes))
+        dataframes = tuple(map(self.get_rot, dataframes))
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
                 df_normal["J'"],
                 s=4 * df_normal["blend O-C/error"],
                 facecolors=df_normal["Transition Type"].map(
                     {
-                        "a-type": "#0000FF65",
-                        "b-type": "#00800045",
-                        "c-type": "#FFA50020",
+                        "a-type": "#00FFFFFF",
+                        "b-type": "#00FFFFFF",
+                        "c-type": "#00FFFFFF",
                     }
                 ),
                 edgecolors=df_normal["Transition Type"].map(
                     {"a-type": "blue", "b-type": "green", "c-type": "orange"}
                 ),
                 linewidth=0.8,
             )
@@ -603,104 +610,130 @@
             linewidth=0.8,
         )
         ax[1].scatter(
             df_normal_q["Ka'"],
             df_normal_q["J'"],
             s=4 * df_normal_q["blend O-C/error"],
             facecolors=df_normal_q["Transition Type"].map(
-                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFA50020"}
+                {"a-type": "#00FFFFFF", "b-type": "#00FFFFFF", "c-type": "#00FFFFFF"}
             ),
             edgecolors=df_normal_q["Transition Type"].map(
-                {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+                {"a-type": "black", "b-type": "black", "c-type": "black"}
             ),
             linewidth=0.8,
         )
 
         ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[0].set_xlabel("$K_a''$", fontsize=14)
         ax[0].set_ylabel("$J''$", fontsize=14)
         ax[0].set_ylim(0, max_J)
         ax[0].set_xlim(-0.5, max_Ka)
         ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[0].text(38, 110, "R-Branch", fontsize=18)
+        ax[0].text(text_x_pos, text_y_pos, "R-Branch", fontsize=18)
 
         ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
         ax[1].set_xlabel("$K_a''$", fontsize=14)
         ax[1].set_ylabel("$J''$", fontsize=14)
         ax[1].set_ylim(0, max_J)
         ax[1].set_xlim(-0.5, max_Ka)
         ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
         ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[1].text(38, 110, "Q-Branch", fontsize=18)
+        ax[1].text(text_x_pos, text_y_pos, "Q-Branch", fontsize=18)
 
-        c = [
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#0000FF65",
-                edgecolor="blue",
-                label="a-type",
-            ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#00800045",
-                edgecolor="green",
-                label="b-type",
-            ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#FFA50065",
-                edgecolor="orange",
-                label="c-type",
+        file_path = self.file_name + ".jpg"
+        fig.savefig(file_path, dpi=800)
+
+    def plot_data_dist_IR_pub(self, max_Ka: int, max_J: int):
+        mpl.rc("text", usetex=True)
+        plt.style.use(["science", "ieee"])
+        text_x_pos = max_Ka - 22
+        text_y_pos = max_J - 10
+        self.categorize_error()
+        self.res_dataframe = self.res_dataframe.sort_values(
+            by=["Transition Type"], ascending=True
+        )
+        dataframes = self.split_branches()
+        dataframes = tuple(map(self.get_IR, dataframes))
+        fig, ax = plt.subplots(1, 2, figsize=(8, 4))
+        for i in range(0, 2):
+            condition = dataframes[i]["blend O-C/error"] >= 4
+            df_high_error = dataframes[i][condition]
+            df_normal = dataframes[i][~condition]
+            ax[0].scatter(
+                df_normal["Ka'"],
+                df_normal["J'"],
+                s=4 * df_normal["blend O-C/error"],
+                facecolors=df_normal["Transition Type"].map(
+                    {
+                        "a-type": "#00FFFFFF",
+                        "b-type": "#00FFFFFF",
+                        "c-type": "#00FFFFFF",
+                    }
+                ),
+                edgecolors=df_normal["Transition Type"].map(
+                    {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+                ),
+                linewidth=0.8,
+            )
+            ax[0].scatter(
+                df_high_error["Ka'"],
+                df_high_error["J'"],
+                s=4 * df_high_error["blend O-C/error"],
+                facecolors="#FF000065",
+                edgecolors="red",
+                linewidth=0.8,
+            )
+        condition_q = dataframes[2]["blend O-C/error"] >= 4
+        df_high_error_q = dataframes[2][condition_q]
+        df_normal_q = dataframes[2][~condition_q]
+        ax[1].scatter(
+            df_high_error_q["Ka'"],
+            df_high_error_q["J'"],
+            s=4 * df_high_error_q["blend O-C/error"],
+            facecolors="#FF000065",
+            edgecolors="red",
+            linewidth=0.8,
+        )
+        ax[1].scatter(
+            df_normal_q["Ka'"],
+            df_normal_q["J'"],
+            s=4 * df_normal_q["blend O-C/error"],
+            facecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "#00FFFFFF", "b-type": "#00FFFFFF", "c-type": "#00FFFFFF"}
             ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#FF000065",
-                edgecolor="red",
-                label=r"$>$ $3\sigma$",
+            edgecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "black", "b-type": "black", "c-type": "black"}
             ),
-        ]
-        texts = ["a-type", "b-type", "c-type", r"$>$ $3\sigma$"]
-        legend = ax[0].legend(
-            c,
-            texts,
-            loc="lower right",
-            fontsize=8,
-            frameon=True,
-            edgecolor="black",
-            framealpha=1,
-            borderaxespad=0,
-            fancybox=False,
-            handler_map={mpatches.Circle: HandlerEllipse()},
+            linewidth=0.8,
         )
-        frame = legend.get_frame()
-        frame.set_linewidth(0.5)
 
-        legend1 = ax[1].legend(
-            c,
-            texts,
-            loc="lower right",
-            fontsize=8,
-            frameon=True,
-            edgecolor="black",
-            framealpha=1,
-            borderaxespad=0,
-            fancybox=False,
-            handler_map={mpatches.Circle: HandlerEllipse()},
-        )
-        frame1 = legend1.get_frame()
-        frame1.set_linewidth(0.5)
+        ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[0].set_xlabel("$K_a''$", fontsize=14)
+        ax[0].set_ylabel("$J''$", fontsize=14)
+        ax[0].set_ylim(0, max_J)
+        ax[0].set_xlim(-0.5, max_Ka)
+        ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[0].text(text_x_pos, text_y_pos, "R-Branch", fontsize=18)
+
+        ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[1].set_xlabel("$K_a''$", fontsize=14)
+        ax[1].set_ylabel("$J''$", fontsize=14)
+        ax[1].set_ylim(0, max_J)
+        ax[1].set_xlim(-0.5, max_Ka)
+        ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[1].text(text_x_pos, text_y_pos, "Q-Branch", fontsize=18)
+
         file_path = self.file_name + ".jpg"
         fig.savefig(file_path, dpi=800)
 
 
+
 class HandlerEllipse(HandlerPatch):
     def create_artists(
         self,
         legend,
         orig_handle,
         xdescent,
         ydescent,
```

### Comparing `rotspectools-0.1.8/PKG-INFO` & `rotspectools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

