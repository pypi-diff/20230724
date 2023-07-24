# Comparing `tmp/dynrender_skia-0.1.2.tar.gz` & `tmp/dynrender_skia-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynrender_skia-0.1.2.tar", max compression
+gzip compressed data, was "dynrender_skia-0.1.5.tar", max compression
```

## Comparing `dynrender_skia-0.1.2.tar` & `dynrender_skia-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/LICENSE
--rw-r--r--   0        0        0     1501 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/README.md
--rw-r--r--   0        0        0     2225 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/Core.py
--rw-r--r--   0        0        0    18382 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynAdditional.py
--rw-r--r--   0        0        0     5499 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynConfig.py
--rw-r--r--   0        0        0    11153 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynHeader.py
--rw-r--r--   0        0        0    28444 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynMajor.py
--rw-r--r--   0        0        0     1204 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynRepost.py
--rw-r--r--   0        0        0      849 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynStyle.py
--rw-r--r--   0        0        0    12798 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynText.py
--rw-r--r--   0        0        0     4084 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/DynTools.py
--rw-r--r--   0        0        0   334112 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/Static.zip
--rw-r--r--   0        0        0        0 2023-07-23 04:40:30.049036 dynrender_skia-0.1.2/dynrender_skia/__init__.py
--rw-r--r--   0        0        0      519 2023-07-23 04:40:30.053036 dynrender_skia-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 dynrender_skia-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1504 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/README.md
+-rw-r--r--   0        0        0     2225 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/Core.py
+-rw-r--r--   0        0        0    18382 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynAdditional.py
+-rw-r--r--   0        0        0     5499 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynConfig.py
+-rw-r--r--   0        0        0    11153 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynHeader.py
+-rw-r--r--   0        0        0    30723 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynMajor.py
+-rw-r--r--   0        0        0     1204 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynRepost.py
+-rw-r--r--   0        0        0      849 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynStyle.py
+-rw-r--r--   0        0        0    12798 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynText.py
+-rw-r--r--   0        0        0     4084 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynTools.py
+-rw-r--r--   0        0        0   334112 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/Static.zip
+-rw-r--r--   0        0        0        0 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-24 12:25:53.013645 dynrender_skia-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 dynrender_skia-0.1.5/PKG-INFO
```

### Comparing `dynrender_skia-0.1.2/LICENSE` & `dynrender_skia-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/README.md` & `dynrender_skia-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```
 
 # 使用方法
 
 ## 安装必要依赖
 ```bash
-pip install dynamicadaptor skia-python
+pip install dynamicadaptor dynrender-skia
 ```
 
 ## 测试
 
 ```python
 import httpx
 import asyncio
```

### Comparing `dynrender_skia-0.1.2/dynrender_skia/Core.py` & `dynrender_skia-0.1.5/dynrender_skia/Core.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynAdditional.py` & `dynrender_skia-0.1.5/dynrender_skia/DynAdditional.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynConfig.py` & `dynrender_skia-0.1.5/dynrender_skia/DynConfig.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynHeader.py` & `dynrender_skia-0.1.5/dynrender_skia/DynHeader.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynMajor.py` & `dynrender_skia-0.1.5/dynrender_skia/DynMajor.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,16 @@
             if major_type == "MAJOR_TYPE_DRAW":
                 return await DynMajorDraw(self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_ARCHIVE":
                 return await DynMajorArchive(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_LIVE_RCMD":
                 return await DynMajorLiveRcmd(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_OPUS":
+                return await DynMajorOpus(self.src_path, self.style, dyn_major).run(repost)
+            elif major_type == "MAJOR_TYPE_ARTICLE":
                 return await DynMajorArticle(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_COMMON":
                 return await DynMajorCommon(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_MUSIC":
                 return await DynMajorMusic(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_PGC":
                 return await DynMajorPgc(self.src_path, self.style, dyn_major).run(repost)
@@ -167,14 +169,15 @@
             elif major_type == "MAJOR_TYPE_COURSES":
                 return await DynMajorCourses(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_UGC_SEASON":
                 return await DynMajorUgc(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_LIVE":
                 return await DynMajorLive(self.src_path, self.style, dyn_major).run(repost)
             else:
+                
                 logger.warning(f"{major_type} is not supported")
                 return None
         except Exception as e:
             logger.exception(e)
             return None
 
 
@@ -326,15 +329,15 @@
                                     self.style.font.font_size.title)
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception:
             logger.exception("Error")
             return None
 
 
-class DynMajorArticle(AbstractMajor):
+class DynMajorOpus(AbstractMajor):
 
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 640)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
@@ -369,14 +372,56 @@
                                  self.style.color.font_color.text)
         desc = self.major.opus.summary.text
         await self.draw_text(self.canvas, desc, self.style.font.font_size.title,
                              (65, 460, 980, 620, int(self.style.font.font_size.title * 1.8)),
                              self.style.color.font_color.sub_title)
 
 
+class DynMajorArticle(AbstractMajor):
+
+    async def run(self, repost) -> Optional[np.ndarray]:
+        background_color = self.style.color.background.repost if repost else self.style.color.background.normal
+        surface = skia.Surface(1080, 640)
+        self.canvas = surface.getCanvas()
+        self.canvas.clear(skia.Color(*background_color))
+        try:
+            await self.draw_shadow(self.canvas, (35, 20, 1010, 600), 20, background_color)
+
+            rec = skia.Rect.MakeXYWH(35, 20, 1010, 600)
+            self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
+            await self.draw_title_and_desc()
+            await self.make_cover()
+            return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
+        except Exception as e:
+            logger.exception(e)
+            return None
+
+    async def make_cover(self):
+        if len(self.major.article.covers) > 1:
+            url_list = [f"{i}@360w_360h_1c" for i in self.major.article.covers]
+            imgs = await get_pictures(url_list, (330, 330))
+            for i, j in enumerate(imgs):
+                await paste(self.canvas, j, (35 + i * 340, 20))
+        else:
+            img = await get_pictures(f"{self.major.article.covers[0]}@647w_150h_1c.webp", (1010, 300))
+            await paste(self.canvas, img, (35, 20))
+
+    async def draw_title_and_desc(self):
+        title = self.major.article.title
+        if len(self.major.article.covers) > 1:
+            await self.draw_text(self.canvas, title, self.style.font.font_size.text, (50, 410, 960, 330, 0),
+                                 self.style.color.font_color.text)
+        else:
+            await self.draw_text(self.canvas, title, self.style.font.font_size.text, (50, 390, 960, 330, 0),
+                                 self.style.color.font_color.text)
+        desc = self.major.article.desc
+        await self.draw_text(self.canvas, desc, self.style.font.font_size.title,
+                             (65, 460, 980, 620, int(self.style.font.font_size.title * 1.8)),
+                             self.style.color.font_color.sub_title)
+
 class DynMajorCommon(AbstractMajor):
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 285)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
```

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynRepost.py` & `dynrender_skia-0.1.5/dynrender_skia/DynRepost.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynStyle.py` & `dynrender_skia-0.1.5/dynrender_skia/DynStyle.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynText.py` & `dynrender_skia-0.1.5/dynrender_skia/DynText.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/DynTools.py` & `dynrender_skia-0.1.5/dynrender_skia/DynTools.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/dynrender_skia/Static.zip` & `dynrender_skia-0.1.5/dynrender_skia/Static.zip`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.2/pyproject.toml` & `dynrender_skia-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "dynrender-skia"
-version = "0.1.2"
+version = "0.1.5"
 description = "使用skia-python将BiliBili动态渲染为图片"
 authors = ["DMC <lzxder@outlook.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 packages = [{include = "dynrender_skia"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 skia-python = "^87.5"
 httpx = "^0.24.1"
 emoji = "^2.6.0"
 dynamicadaptor = "^0.4.5"
+bilirpc = "^0.1.3"
 
 
 [tool.poetry.group.dev.dependencies]
 viztracer = "^0.15.6"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dynrender_skia-0.1.2/PKG-INFO` & `dynrender_skia-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dynrender-skia
-Version: 0.1.2
+Version: 0.1.5
 Summary: 使用skia-python将BiliBili动态渲染为图片
 License: GNU GPLv3
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bilirpc (>=0.1.3,<0.2.0)
 Requires-Dist: dynamicadaptor (>=0.4.5,<0.5.0)
 Requires-Dist: emoji (>=2.6.0,<3.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: skia-python (>=87.5,<88.0)
 Description-Content-Type: text/markdown
 
 # DynRender-skia
@@ -47,15 +48,15 @@
 
 ```
 
 # 使用方法
 
 ## 安装必要依赖
 ```bash
-pip install dynamicadaptor skia-python
+pip install dynamicadaptor dynrender-skia
 ```
 
 ## 测试
 
 ```python
 import httpx
 import asyncio
```

