# Comparing `tmp/nonebot_plugin_impact-0.1.114514.tar.gz` & `tmp/nonebot_plugin_impact-0.2.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.1.114514.tar", last modified: Tue Jul 11 19:57:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.2.114514.tar", last modified: Mon Jul 24 16:07:12 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.1.114514.tar` & `nonebot_plugin_impact-0.2.114514.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.342784 nonebot_plugin_impact-0.1.114514/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.1.114514/LICENSE
--rw-rw-rw-   0        0        0      306 2023-07-11 19:57:05.341784 nonebot_plugin_impact-0.1.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.334574 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     2047 2023-07-11 19:53:35.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0    20576 2023-07-11 19:49:13.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2041 2023-07-11 19:49:23.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8628 2023-07-11 19:54:40.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.340783 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      306 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 19:57:05.342784 nonebot_plugin_impact-0.1.114514/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-07-11 19:56:34.000000 nonebot_plugin_impact-0.1.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.186682 nonebot_plugin_impact-0.2.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.2.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-07-24 16:07:12.185680 nonebot_plugin_impact-0.2.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.137789 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2047 2023-07-24 16:03:28.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0     9171 2023-07-24 16:00:38.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/draw_img.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.144760 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/fonts/
+-rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
+-rw-rw-rw-   0        0        0    20206 2023-07-24 15:51:35.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2205 2023-07-24 16:03:09.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8628 2023-07-24 15:22:41.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:07:12.143788 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-24 16:07:12.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 16:07:11.000000 nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 16:07:12.186682 nonebot_plugin_impact-0.2.114514/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-07-24 16:07:02.000000 nonebot_plugin_impact-0.2.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.1.114514/LICENSE` & `nonebot_plugin_impact-0.2.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,11 +83,11 @@
         description="让群友们眼前一黑的nonebot2淫趴插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_impact",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
-            "version": "0.01.114514",
+            "version": "0.02.114514",
             "priority": 20,
         },
     )
```

### Comparing `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/handle.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from random import choice
 from typing import Tuple
 
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, Message, MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup
 
-from .txt2img import txt_to_img
+from .draw_img import draw_bar_chart
 from .utils import utils
 
 
 class Impart:
     @staticmethod
     async def pk(matcher: Matcher, event: GroupMessageEvent) -> None:
         """pk的响应器"""
@@ -212,25 +212,20 @@
         # top5和end5的信息，然后获取其网名
         top5info = [await bot.get_stranger_info(user_id=int(name[0])) for name in top5]
         last5info = [
             await bot.get_stranger_info(user_id=int(name[0])) for name in last5
         ]
         top5names = [name["nickname"] for name in top5info]
         last5names = [name["nickname"] for name in last5info]
-        # 构造消息，手搓
-        reply = "咱只展示前五名和后五名喵\n"
-        top5txt = f"{top5names[0]} ------> {top5[0][1]}cm\n{top5names[1]} ------> {top5[1][1]}cm\n{top5names[2]} ------> {top5[2][1]}cm\n{top5names[3]} ------> {top5[3][1]}cm\n{top5names[4]} ------> {top5[4][1]}cm\n"
-        last5txt = f"{last5names[0]} ------> {last5[0][1]}cm\n{last5names[1]} ------> {last5[1][1]}cm\n{last5names[2]} ------> {last5[2][1]}cm\n{last5names[3]} ------> {last5[3][1]}cm\n{last5names[4]} ------> {last5[4][1]}cm\n"
-        img_bytes = await txt_to_img.txt_to_img(
-            top5txt + ".................................\n" * 3 + last5txt
-        )  # 生成图片
+        data = {top5names[i]: top5[i][1] for i in range(len(top5))}
+        for i in range(len(last5)):
+            data[last5names[i]] = last5[i][1]
+        img_bytes = await draw_bar_chart.draw_bar_chart(data)
         reply2 = f"你的排名为{index[0]+1}喵"
-        await matcher.finish(
-            reply + MessageSegment.image(img_bytes) + reply2, at_sender=True
-        )
+        await matcher.finish(MessageSegment.image(img_bytes) + reply2, at_sender=True)
 
     @staticmethod
     async def yinpa_prehandle(
         bot: Bot,
         args: Tuple,
         matcher: Matcher,
         event: GroupMessageEvent,
@@ -398,23 +393,27 @@
         )
         ejaculation = 0  # 先初始化0
         if "历史" in target or "全部" in target:
             try:
                 date = utils.ejaculation_data[object_id]  # 对象不存在直接输出0
             except Exception:
                 await matcher.finish(f"{replay1}历史总被注射量为0ml")
-            pic_string: str = ""  # 文字， 准备弄成图片
+            inject_data = {}
             for key in date:  # 遍历所有的日期
                 temp = date[key]["ejaculation"]
                 ejaculation += temp  # 注入量求和
-                pic_string += f"{key}\t\t{temp}\n"
+                inject_data[key] = temp
+            if len(inject_data) < 2:
+                await matcher.finish(f"{replay1}历史总被注射量为{ejaculation}ml")
 
             await matcher.finish(
                 MessageSegment.text(f"{replay1}历史总被注射量为{ejaculation}ml")
-                + MessageSegment.image(await txt_to_img.txt_to_img(pic_string))
+                + MessageSegment.image(
+                    await draw_bar_chart.draw_line_chart(inject_data)
+                )
             )
         else:
             ejaculation = utils.get_today_ejaculation(object_id)  # 获取对象当天的注入量
             await matcher.finish(f"{replay1}当日总被注射量为{ejaculation}ml")
 
     @staticmethod
     async def yinpa_introduce(matcher: Matcher) -> None:
```

### Comparing `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/txt2img.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from io import BytesIO
 
 from PIL import Image, ImageDraw, ImageFont
+from pathlib import Path
 
 
 class TxtToImg:
     def __init__(self) -> None:
         self.LINE_CHAR_COUNT = 30 * 2
         self.CHAR_SIZE = 30
         self.TABLE_WIDTH = 4
-
+        self.module_path: Path = Path(__file__).parent
+        self.font = str(self.module_path / "fonts" / "SIMYOU.TTF")
 
     async def line_break(self, line: str) -> str:
         """将一行文本按照指定宽度进行换行"""
         ret = ""
         width = 0
         for c in line:
             if len(c.encode("utf8")) == 3:  # 中文
@@ -22,38 +24,40 @@
                 else:  # 中文宽度加2，注意换行边界
                     width += 2
                     ret += c
             elif c == "\n":
                 width = 0
                 ret += c
             elif c == "\t":
-                space_c = self.TABLE_WIDTH - width % self.TABLE_WIDTH  # 已有长度对TABLE_WIDTH取余
+                space_c = (
+                    self.TABLE_WIDTH - width % self.TABLE_WIDTH
+                )  # 已有长度对TABLE_WIDTH取余
                 ret += " " * space_c
                 width += space_c
             else:
                 width += 1
                 ret += c
             if width >= self.LINE_CHAR_COUNT:
                 ret += "\n"
                 width = 0
         return ret if ret.endswith("\n") else ret + "\n"
 
-
-    async def txt_to_img(self, text: str, font_size: int=30, font_path: str="simsun.ttc") -> bytes:
+    async def txt_to_img(self, text: str, font_size: int = 30) -> bytes:
         """将文本转换为图片"""
         text = await self.line_break(text)
-        d_font = ImageFont.truetype(font_path, font_size)
+        d_font = ImageFont.truetype(self.font, font_size)
         lines = text.count("\n")
         image = Image.new(
-            "L", (self.LINE_CHAR_COUNT * font_size // 2 + 50, font_size * lines + 50), "white"
+            "L",
+            (self.LINE_CHAR_COUNT * font_size // 2 + 50, font_size * lines + 50),
+            "white",
         )
         draw_table = ImageDraw.Draw(im=image)
-        draw_table.text(
-            xy=(25, 25), text=text, fill="#000000", font=d_font, spacing=4
-        )
+        draw_table.text(xy=(25, 25), text=text, fill="#000000", font=d_font, spacing=4)
         new_img = image.convert("RGB")
         img_byte = BytesIO()
         new_img.save(img_byte, format="PNG")
         return img_byte.getvalue()
-    
+
+
 # 创建一个实例
-txt_to_img = TxtToImg()
+txt_to_img = TxtToImg()
```

### Comparing `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.2.114514/nonebot_plugin_impact/utils.py`

 * *Files identical despite different names*

