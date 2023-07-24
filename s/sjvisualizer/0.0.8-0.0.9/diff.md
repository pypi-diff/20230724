# Comparing `tmp/sjvisualizer-0.0.8-py2.py3-none-any.whl.zip` & `tmp/sjvisualizer-0.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 37972 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     8895 b- defN 23-Jul-05 12:35 sjvisualizer/Axis.py
+Zip file size: 38309 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     9045 b- defN 23-Jul-24 18:45 sjvisualizer/Axis.py
 -rw-rw-rw-  2.0 fat    26664 b- defN 23-May-17 13:54 sjvisualizer/BarRace.py
--rw-rw-rw-  2.0 fat    13495 b- defN 23-Jul-05 15:11 sjvisualizer/Canvas.py
+-rw-rw-rw-  2.0 fat    13890 b- defN 23-Jul-24 18:51 sjvisualizer/Canvas.py
 -rw-rw-rw-  2.0 fat     5723 b- defN 23-Jun-07 18:56 sjvisualizer/DataHandler.py
 -rw-rw-rw-  2.0 fat     4531 b- defN 22-Aug-24 13:17 sjvisualizer/Date.py
 -rw-rw-rw-  2.0 fat     8475 b- defN 23-Jun-24 16:59 sjvisualizer/Legend.py
--rw-rw-rw-  2.0 fat    13101 b- defN 23-Jul-05 15:07 sjvisualizer/LineChart.py
+-rw-rw-rw-  2.0 fat    13424 b- defN 23-Jul-24 18:46 sjvisualizer/LineChart.py
 -rw-rw-rw-  2.0 fat    20653 b- defN 23-May-17 13:54 sjvisualizer/PieRace.py
 -rw-rw-rw-  2.0 fat    15424 b- defN 23-May-17 13:54 sjvisualizer/StackedBarChart.py
 -rw-rw-rw-  2.0 fat     3094 b- defN 22-Aug-24 10:37 sjvisualizer/StaticImage.py
 -rw-rw-rw-  2.0 fat     4558 b- defN 23-May-17 13:54 sjvisualizer/StaticText.py
 -rw-rw-rw-  2.0 fat     3070 b- defN 23-Jul-05 15:03 sjvisualizer/Total.py
 -rw-rw-rw-  2.0 fat      343 b- defN 23-Jul-05 14:57 sjvisualizer/__init__.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-Jul-05 15:13 sjvisualizer-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3331 b- defN 23-Jul-05 15:13 sjvisualizer-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-05 15:13 sjvisualizer-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-05 15:13 sjvisualizer-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1468 b- defN 23-Jul-05 15:13 sjvisualizer-0.0.8.dist-info/RECORD
-18 files, 134038 bytes uncompressed, 35592 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-Jul-24 18:51 sjvisualizer-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3636 b- defN 23-Jul-24 18:51 sjvisualizer-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-24 18:51 sjvisualizer-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-24 18:51 sjvisualizer-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1468 b- defN 23-Jul-24 18:51 sjvisualizer-0.0.9.dist-info/RECORD
+18 files, 135211 bytes uncompressed, 35929 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: sjvisualizer/Total.py
 Comment: 
 
 Filename: sjvisualizer/__init__.py
 Comment: 
 
-Filename: sjvisualizer-0.0.8.dist-info/LICENSE
+Filename: sjvisualizer-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: sjvisualizer-0.0.8.dist-info/METADATA
+Filename: sjvisualizer-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sjvisualizer-0.0.8.dist-info/WHEEL
+Filename: sjvisualizer-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sjvisualizer-0.0.8.dist-info/top_level.txt
+Filename: sjvisualizer-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sjvisualizer-0.0.8.dist-info/RECORD
+Filename: sjvisualizer-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sjvisualizer/Axis.py

```diff
@@ -122,14 +122,17 @@
                 if not "i" in locals():
                     i = 0
 
                 for j in range(i, self.n * 3):
                     self.ticks[j].update(value=1, draw=False)
 
     def calc_positions(self, value):
+        if self.min == 0 and self.max == 0:
+            self.max = 0.1
+
         if not self.is_date:
             if not self.is_log_scale:
                 return self.length * (value - self.min) / (self.max - self.min)
             else:
                 return self.length * math.log10(value) / (math.log10(self.max) - math.log10(self.min))
         else:
             try:
@@ -153,15 +156,15 @@
     def update(self, value=0, draw=True, l=0):
         pos = self.axis.calc_positions(value)
         if draw:
             if self.axis.is_date:
                 t = datetime.datetime(1800,1,1) + datetime.timedelta(days=value)
                 label = cv.format_date(t, self.axis.time_indicator)
             else:
-                label = str(value)
+                label = cv.format_value(value)
             if self.axis.orientation == "horizontal":
                 self.canvas.coords(self.line, self.axis.x + pos, self.axis.y - self.length - l, self.axis.x + pos, self.axis.y + 10)
                 self.canvas.itemconfig(self.text, text=label + self.axis.unit)
                 if self.label_pos == "s":
                     self.canvas.coords(self.text, self.axis.x + pos, self.axis.y + 11)
                 elif self.label_pos == "n":
                     self.canvas.coords(self.text, self.axis.x + pos, self.axis.y - self.length - 1)
@@ -187,14 +190,17 @@
 
 
 def calculate_nice_ticks(min_val, max_val, num_ticks, is_log_scale=False):
     if is_log_scale:
         min_val = math.log10(min_val)
         max_val = math.log10(max_val)
 
+    if min_val == max_val:
+        max_val = min_val + 0.1
+
     # Calculate the rough range
     rough_range = max_val - min_val
 
     # Calculate the rough tick increment
     rough_tick_incr = rough_range / num_ticks
 
     # Calculate the exponent of the rough tick increment in base 10
```

## sjvisualizer/Canvas.py

```diff
@@ -417,9 +417,23 @@
         if format == "USA":
             text = str("{} {} {}".format(months[time.month], time.day, time.year))
         else:
             text = str("{} {} {}".format(time.day, months[time.month], time.year))
 
     return text
 
+def format_value(number, decimal=decimal_places):
+    units = ['k', 'm', 'b', 't']
+    unit_index = 0
+
+    while number >= 1000 and unit_index < len(units):
+        number /= 1000.0
+        unit_index += 1
+
+    formatted_number = "{:.3f}".format(number).rstrip('0').rstrip('.')
+    if unit_index > 0:
+        formatted_number += units[unit_index - 1]
+
+    return formatted_number
+
 def hex_to_rgb(h):
     return tuple(int(h.lstrip("#")[i:i + 2], 16) for i in (0, 2, 4))
```

## sjvisualizer/LineChart.py

```diff
@@ -118,25 +118,31 @@
                 "{EVENT NAME}": ["START DATE DD/MM/YYYY", "END DATE DD/MM/YYYY"],
                 "Event 1": ["28/01/2017", "28/01/2018"],
                 "Event 2": ["28/01/2019", "28/01/2020"],
                 "Last event": ["28/05/2020", "28/01/2021"]
             }
             :type events: dict
 
+            :param event_color: color of the event indication, default is (225,225,225)
+            :type event_color: tuple
+
             :param draw_all_events: by default only the label will be added to the most recent event. Set this value to True to keep the labels for all events
             :type draw_all_events: boolean
 
             """
 
     def draw(self, time):
         if hasattr(self, "font_size"):
-            self.font_size = font_size / SCALEFACTOR
+            self.font_size = self.font_size / SCALEFACTOR
         else:
             self.font_size = self.height / 33 / SCALEFACTOR
 
+        if not hasattr(self, "event_color"):
+            self.event_color = (225,225,225)
+
         if not hasattr(self, "draw_points"):
             self.draw_points = True
 
         if not hasattr(self, "events"):
             self.events = {}
 
         if not hasattr(self, "draw_all_events"):
@@ -176,62 +182,63 @@
             else:
                 n_y = len(self.df.columns)
             self.legend = Legend.legend(canvas=self.canvas, height=self.height, width=500, x_pos=self.x_pos + self.width + 5*self.font_size, y_pos=self.y_pos, df=self.df, colors=self.colors, n=10, font_size=self.font_size, font_color=self.font_color)
             self.sjcanvas.add_sub_plot(self.legend)
 
         self.event_obj = []
         for name, dates in self.events.items():
-            self.event_obj.append(event(name=name, canvas=self.canvas, start_date=dates[0], end_date=dates[1], font_color=self.font_color, font_size=self.font_size, parent=self))
+            self.event_obj.append(event(name=name, canvas=self.canvas, start_date=dates[0], end_date=dates[1], font_color=self.font_color, font_size=self.font_size, parent=self, event_color=self.event_color))
 
     def update(self, time):
         self.max_time = time
         data = self._get_data_for_frame(time)
         self.axis1.update(min=self.min_time, max=self.max_time)
         if min(data) > self.default_min_value:
             self.axis2.update(min=0, max=max(data))
         else:
             self.axis2.update(min=min(data), max=max(data))
 
         if self.draw_points:
             total_points = sum([len(line.points) for name, line in self.lines.items()])
 
         for name, d in data.items():
-            if MAX_POINTS < total_points:
-                self.lines[name].point_radius = self.lines[name].point_radius - 0.25
-            if self.lines[name].point_radius < 0:
-                self.lines[name].remove_points()
+            if self.draw_points:
+                if MAX_POINTS < total_points:
+                    self.lines[name].point_radius = self.lines[name].point_radius - 0.25
+                if self.lines[name].point_radius < 0:
+                    self.lines[name].remove_points()
             self.lines[name].update(d, time)
 
         for e in self.event_obj:
             if self.draw_all_events:
                 e.draw_label = True
             e.update(time)
 
 class event():
 
-    def __init__(self, name=None, canvas=None, start_date=None, end_date=None, color=(225,225,225), font_color=(0,0,0), font_size=12, text_font="Microsoft JhengHei UI", parent=None):
+    def __init__(self, name=None, canvas=None, start_date=None, end_date=None, font_color=(0,0,0), font_size=12, text_font="Microsoft JhengHei UI", parent=None, event_color=(255, 255, 255)):
         self.name = name
         self.canvas = canvas
         self.start_date = datetime.datetime.strptime(start_date, "%d/%m/%Y")
         self.end_date = datetime.datetime.strptime(end_date, "%d/%m/%Y")
-        self.color = cv._from_rgb(color)
+        self.color = cv._from_rgb(event_color)
         self.font_color = font_color
         self.font_size = font_size
         self.text_font = text_font
         self.font = font.Font(family=self.text_font, size=int(self.font_size))
         self.parent = parent
 
         self.drawn = False
         self.draw_label = False
 
         self.draw()
 
     def draw(self):
         self.rect = self.canvas.create_rectangle(-1000, -1000, -1000, -1000, fill=self.color, outline="")
-        self.label = self.canvas.create_text(-1000, -1000, text=self.name, font=self.font, fill=cv._from_rgb(self.font_color), anchor="s")
+        self.label = self.canvas.create_text(-1000, -1000, text=self.name, font=self.font, fill=cv._from_rgb(self.font_color), anchor="se")
 
     def update(self, date):
         if date > self.start_date:
             if not self.drawn:
                 self.drawn = True
                 for e in self.parent.event_obj:
                     e.draw_label = False
@@ -241,15 +248,15 @@
             if self.end_date > date:
                 pos2 = self.parent.axis1.calc_positions(
                     (date - datetime.datetime(1800, 1, 1)).days) + self.parent.x_pos
             else:
                 pos2 = self.parent.axis1.calc_positions((self.end_date - datetime.datetime(1800,1,1)).days) + self.parent.x_pos
 
             if self.draw_label:
-                self.canvas.coords(self.label, (pos1 + pos2) / 2, self.parent.y_pos - 3)
+                self.canvas.coords(self.label, (pos2 + pos2) / 2, self.parent.y_pos - 3)
             else:
                 self.canvas.itemconfig(self.label, text="")
 
             self.canvas.coords(self.rect, pos1, self.parent.y_pos, pos2, self.parent.y_pos + self.parent.height)
 
 
 class line():
```

## Comparing `sjvisualizer-0.0.8.dist-info/LICENSE` & `sjvisualizer-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sjvisualizer-0.0.8.dist-info/METADATA` & `sjvisualizer-0.0.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: sjvisualizer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to animate your data
 Author: Sjoerd Tilmans
 Author-email: info@sjdataviz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=2.0)
 Requires-Dist: screeninfo (>=0.7)
 Requires-Dist: Pillow (>9)
 Requires-Dist: openpyxl (>3)
 
+[![Downloads](https://static.pepy.tech/badge/sjvisualizer)](https://pepy.tech/project/sjvisualizer)
 # sjvisualizer 📊
 sjvisualizer is a data visualization and animation library for Python. 
 
-https://github.com/SjoerdTilmans/sjvisualizer/assets/37220662/91b54d89-78c2-4425-9e75-c942d2457fbf
+https://github.com/SjoerdTilmans/sjvisualizer/assets/37220662/a9a01f5b-50f4-411f-8e7c-dcd4a805501b
 
 Please find the catalogue example [here](https://github.com/SjoerdTilmans/sjvisualizer/blob/main/Examples/Catalogue.py) to run the above animation. sjvisualizer currently supports the following chart types:
 - Bar races
 - Animated pie charts
 - Animated stacked bar charts
+- Animated line charts
 
 More chart types to follow! 
 
 There are two ways of learning sjvisualizer:
 - Find additional examples and full documentation on my [website](https://www.sjdataviz.com/software)
 - Or follow my course on [Udemy](https://www.sjdataviz.com/course-link)
 
@@ -75,14 +77,17 @@
     canvas.add_time(df=df, time_indicator="month")
 
     canvas.play(fps=fps)
 
 if __name__ == "__main__":
     main()
 ```
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=SjoerdTilmans/sjvisualizer&type=Date)](https://star-history.com/#SjoerdTilmans/sjvisualizer&Date)
 
 ## Support this project
 If you like this project, please consider buying me a cup of coffee on [buymeacoffee](https://www.buymeacoffee.com/SjoerdTilmans).
     
 ## Contributing
 Contributions are always welcome! Here are some ways to get involved:
```

## Comparing `sjvisualizer-0.0.8.dist-info/RECORD` & `sjvisualizer-0.0.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-sjvisualizer/Axis.py,sha256=kVuIggzL5AzfNfkECMsHOmAYG0LSEyfqWSIARatfNy0,8895
+sjvisualizer/Axis.py,sha256=aVRWpWWIvQ2OeJ-lwT8PJux7j7787LNY2YeoQe0s1O8,9045
 sjvisualizer/BarRace.py,sha256=yCImPGh2bOKyz2TU8RtTOfJWS8CmOu7bbh2BugPMn1o,26664
-sjvisualizer/Canvas.py,sha256=jMtH02R3jDWtEsLsOuywLA7bbgRoidFDchnRU0y_W3E,13495
+sjvisualizer/Canvas.py,sha256=V-UZ-OS62ohfrJqqbXxHm2ukpnt0zNH0e88R_RLagd0,13890
 sjvisualizer/DataHandler.py,sha256=r-UkAnGe_CF38YNc9lb4RDXUufw0_yYBjJyJqjUoLpY,5723
 sjvisualizer/Date.py,sha256=37Rf46d6ODLBmV0l-PUMVjg0kyaGbnKcPTBey2xkW9E,4531
 sjvisualizer/Legend.py,sha256=mT1-VlFt5HyHzLInstI7XBSokw6g7jwggj7GG4cjbVI,8475
-sjvisualizer/LineChart.py,sha256=Gul-wK64Oaaqcl7apIcIXFaADXfhI1p7DeSg4XGOz38,13101
+sjvisualizer/LineChart.py,sha256=ns8co4-Q8qWZU4LMF_6V0SuquxPNkUnF4P-gI_OYfns,13424
 sjvisualizer/PieRace.py,sha256=Lvij_L_KU-xxK-iIUSv1VIyBZ8yo_D7iWXe9--xcuKc,20653
 sjvisualizer/StackedBarChart.py,sha256=5C7D0URuKIPGccxuxcv15vGeXBhC_Kw5I0O5wBFG8vg,15424
 sjvisualizer/StaticImage.py,sha256=CL3FfxB9jFodUlR4US9wiy8YYnHuOTiJwdmXHIvTJGs,3094
 sjvisualizer/StaticText.py,sha256=b1W6m8VqYEyX2ivPIDSVPZxIIXacIIltHAJOs5xIFKA,4558
 sjvisualizer/Total.py,sha256=03TzUQm1lEo-F-EOL12pZkksGHY_aEmVp8ldxHvvZlI,3070
 sjvisualizer/__init__.py,sha256=6UHQaZTJv-WRGLh4sxiNgmaNrO1h-3R9Zr8Mf4PO9No,343
-sjvisualizer-0.0.8.dist-info/LICENSE,sha256=KAfD2XNwf2yYdRBt6P8rEXgUhPkgFpmUo8E6-iPvpg8,1090
-sjvisualizer-0.0.8.dist-info/METADATA,sha256=vZ6Ytruk5G_HxU4MkzEsrs33Wr2K-f-Zou68XXUwf80,3331
-sjvisualizer-0.0.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-sjvisualizer-0.0.8.dist-info/top_level.txt,sha256=j1koak1fnQdqGUuXIniC64CXQt1TdR01rWTuJVaGz5I,13
-sjvisualizer-0.0.8.dist-info/RECORD,,
+sjvisualizer-0.0.9.dist-info/LICENSE,sha256=KAfD2XNwf2yYdRBt6P8rEXgUhPkgFpmUo8E6-iPvpg8,1090
+sjvisualizer-0.0.9.dist-info/METADATA,sha256=c4Me2bb6-7fJoudPZtMaoSc4c_ithKC7Pic5w6v9sRs,3636
+sjvisualizer-0.0.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+sjvisualizer-0.0.9.dist-info/top_level.txt,sha256=j1koak1fnQdqGUuXIniC64CXQt1TdR01rWTuJVaGz5I,13
+sjvisualizer-0.0.9.dist-info/RECORD,,
```

