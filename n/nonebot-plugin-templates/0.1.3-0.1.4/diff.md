# Comparing `tmp/nonebot_plugin_templates-0.1.3.tar.gz` & `tmp/nonebot_plugin_templates-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_templates-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_templates-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_templates-0.1.3.tar` & `nonebot_plugin_templates-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      397 2023-07-18 03:49:45.298270 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/__init__.py
--rw-r--r--   0        0        0     5861 2023-07-18 02:38:35.241359 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/template_types.py
--rw-r--r--   0        0        0     4545 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/cards.html
--rw-r--r--   0        0        0     4336 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/colorlist.html
--rw-r--r--   0        0        0     3821 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/menus.html
--rw-r--r--   0        0        0 10968356 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/PingFang.ttf
--rw-r--r--   0        0        0     6543 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates_render.py
--rw-r--r--   0        0        0      471 2023-07-18 03:49:50.855209 nonebot_plugin_templates-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3450 2023-07-18 03:34:04.186661 nonebot_plugin_templates-0.1.3/README.md
--rw-r--r--   0        0        0     4011 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      397 2023-07-18 03:49:45.298270 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/__init__.py
+-rw-r--r--   0        0        0     5861 2023-07-18 02:38:35.241359 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/template_types.py
+-rw-r--r--   0        0        0     4545 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/cards.html
+-rw-r--r--   0        0        0     4336 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/colorlist.html
+-rw-r--r--   0        0        0     3623 2023-07-24 06:56:16.187282 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/menus.html
+-rw-r--r--   0        0        0 10968356 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/PingFang.ttf
+-rw-r--r--   0        0        0     6543 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates_render.py
+-rw-r--r--   0        0        0      471 2023-07-24 06:56:16.183277 nonebot_plugin_templates-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3449 2023-07-18 04:01:13.672237 nonebot_plugin_templates-0.1.4/README.md
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/template_types.py` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/template_types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/cards.html` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/cards.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/colorlist.html` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/colorlist.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/menus.html` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/menus.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,14 @@
             white-space: pre-line;
             grid-gap: 2px;
             background-color: {{ colors['func_grid'] }};
             border-radius: 0 0 10px 10px;
             padding: 2px;
         }
 
-        .func-name::before {
-            font-family: "Custom Font";
-            content: "#";
-            color: {{ colors['func_name_pre'] }};
-            white-space: pre-line;
-        }
-
         .func-name {
             font-family: "Custom Font";
             margin: 0;
             display: inline-block;
             white-space: normal;
         }
```

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates/PingFang.ttf` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/PingFang.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.3/nonebot_plugin_templates/templates_render.py` & `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.3/README.md` & `nonebot_plugin_templates-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,37 +16,40 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_templates" alt="github">
     </a>
 </p>
 <div align="left">
 
-## 最新版本号0.1.1
+## 最新版本号0.1.3
 
 # 功能:提供一些jinja2 templates渲染,并提供构建所需参数的类
 
 > 构建一个菜单的示例
 
 ```python
 from nonebot_plugin_templates.template_types import *
 from nonebot_plugin_templates.templates_render import menu_render, colorlist_render
 
 menu = Menu("私有bot", des="使用和管理自己独有的bot的命令,私有bot只有主人可使用,其他人无法使用",
-            funcs=Funcs(Func("/bot名称+询问的问题",
-                             "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
-                        Func("/所有bot",
-                             "查询所有的可用的私有的bot,以获取bot名称和相关信息") +
-                        Func("/创建bot", "创建新的私有的bot") +
-                        Func("/改名bot", "更改自己的bot的名称") +
-                        Func("/删除bot", "删除指定自己的bot")))
+            funcs=Funcs(
+                Func("/bot名称+询问的问题",
+                     "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
+                Func("/所有bot",
+                     "查询所有的可用的私有的bot,以获取bot名称和相关信息") +
+                Func("/创建bot", "创建新的私有的bot") +
+                Func("/改名bot", "更改自己的bot的名称") +
+                Func("/删除bot", "删除指定自己的bot")))
 menu += Menu("公有bot", des="使用和管理公有的bot的命令",
              funcs=Funcs(
                  Func("bot名称+询问的问题",
                       "与指定属于公共的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
                  Func("所有bot", "查询所有的可用的公共的bot,以获取bot名称和相关信息") +
                  Func("创建bot", "创建新的公用的bot") +
                  Func("改名bot", "更改公用的bot的名称") +
                  Func("删除bot", "删除指定公用的bot")))
 pic_bytes = await menu_render(menu, 800)
 ```
 
+![menu.png](src/menu.png)
+
 > 构建一个卡片列表的示例
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
          [https://socialify.git.ci/canxin121/nonebot_plugin_templates/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                     ****** Nonebot_plugin_templates ******
                             [pypi] [python] [pypi]
                                [onebot]_[github]
-## ææ°çæ¬å·0.1.1 # åè½:æä¾ä¸äºjinja2
+## ææ°çæ¬å·0.1.3 # åè½:æä¾ä¸äºjinja2
 templatesæ¸²æ,å¹¶æä¾æå»ºæéåæ°çç±» > æå»ºä¸ä¸ªèåçç¤ºä¾
 ```python from nonebot_plugin_templates.template_types import * from
 nonebot_plugin_templates.templates_render import menu_render, colorlist_render
 menu = Menu("ç§æbot",
 des="ä½¿ç¨åç®¡çèªå·±ç¬æçbotçå½ä»¤,ç§æbotåªæä¸»äººå¯ä½¿ç¨,å¶ä»äººæ æ³ä½¿ç¨",
-funcs=Funcs(Func("/botåç§°+è¯¢é®çé®é¢",
+funcs=Funcs( Func("/botåç§°+è¯¢é®çé®é¢",
 "ä¸æå®å±äºèªå·±çbotå¯¹è¯\n
 (å¯ä½¿ç¨'åå¤'æbotæåä¸ä¸ªç­æ¡æ¥è¿ç»­åå®å¯¹è¯)\n
 (å¯åå¤'æ¸é¤åå²','å·æ°å¯¹è¯'æ¥æ¸é¤botçå¯¹è¯è®°å¿)") + Func("/
 ææbot",
 "æ¥è¯¢ææçå¯ç¨çç§æçbot,ä»¥è·åbotåç§°åç¸å³ä¿¡æ¯") +
 Func("/åå»ºbot", "åå»ºæ°çç§æçbot") + Func("/æ¹åbot",
 "æ´æ¹èªå·±çbotçåç§°") + Func("/å é¤bot",
@@ -22,9 +22,9 @@
 ("botåç§°+è¯¢é®çé®é¢", "ä¸æå®å±äºå¬å±çbotå¯¹è¯\n
 (å¯ä½¿ç¨'åå¤'æbotæåä¸ä¸ªç­æ¡æ¥è¿ç»­åå®å¯¹è¯)\n
 (å¯åå¤'æ¸é¤åå²','å·æ°å¯¹è¯'æ¥æ¸é¤botçå¯¹è¯è®°å¿)") + Func
 ("ææbot",
 "æ¥è¯¢ææçå¯ç¨çå¬å±çbot,ä»¥è·åbotåç§°åç¸å³ä¿¡æ¯") +
 Func("åå»ºbot", "åå»ºæ°çå¬ç¨çbot") + Func("æ¹åbot",
 "æ´æ¹å¬ç¨çbotçåç§°") + Func("å é¤bot",
-"å é¤æå®å¬ç¨çbot"))) pic_bytes = await menu_render(menu, 800) ``` >
-æå»ºä¸ä¸ªå¡çåè¡¨çç¤ºä¾
+"å é¤æå®å¬ç¨çbot"))) pic_bytes = await menu_render(menu, 800) ``` !
+[menu.png](src/menu.png) > æå»ºä¸ä¸ªå¡çåè¡¨çç¤ºä¾
```

### Comparing `nonebot_plugin_templates-0.1.3/PKG-INFO` & `nonebot_plugin_templates-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-templates
-Version: 0.1.3
+Version: 0.1.4
 Summary: 为nonebot提供一系列jinja2 template模板,方便的生成图片
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,37 +32,40 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_templates" alt="github">
     </a>
 </p>
 <div align="left">
 
-## 最新版本号0.1.1
+## 最新版本号0.1.3
 
 # 功能:提供一些jinja2 templates渲染,并提供构建所需参数的类
 
 > 构建一个菜单的示例
 
 ```python
 from nonebot_plugin_templates.template_types import *
 from nonebot_plugin_templates.templates_render import menu_render, colorlist_render
 
 menu = Menu("私有bot", des="使用和管理自己独有的bot的命令,私有bot只有主人可使用,其他人无法使用",
-            funcs=Funcs(Func("/bot名称+询问的问题",
-                             "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
-                        Func("/所有bot",
-                             "查询所有的可用的私有的bot,以获取bot名称和相关信息") +
-                        Func("/创建bot", "创建新的私有的bot") +
-                        Func("/改名bot", "更改自己的bot的名称") +
-                        Func("/删除bot", "删除指定自己的bot")))
+            funcs=Funcs(
+                Func("/bot名称+询问的问题",
+                     "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
+                Func("/所有bot",
+                     "查询所有的可用的私有的bot,以获取bot名称和相关信息") +
+                Func("/创建bot", "创建新的私有的bot") +
+                Func("/改名bot", "更改自己的bot的名称") +
+                Func("/删除bot", "删除指定自己的bot")))
 menu += Menu("公有bot", des="使用和管理公有的bot的命令",
              funcs=Funcs(
                  Func("bot名称+询问的问题",
                       "与指定属于公共的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)") +
                  Func("所有bot", "查询所有的可用的公共的bot,以获取bot名称和相关信息") +
                  Func("创建bot", "创建新的公用的bot") +
                  Func("改名bot", "更改公用的bot的名称") +
                  Func("删除bot", "删除指定公用的bot")))
 pic_bytes = await menu_render(menu, 800)
 ```
 
+![menu.png](src/menu.png)
+
 > 构建一个卡片列表的示例
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-templates Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-templates Version: 0.1.4 Summary:
 ä¸ºnonebotæä¾ä¸ç³»åjinja2 templateæ¨¡æ¿,æ¹ä¾¿ççæå¾ç Author:
 canxin Author-email: 1969730106@qq.com Requires-Python: >=3.8,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-Content-Type: text/
 markdown
          [https://socialify.git.ci/canxin121/nonebot_plugin_templates/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                     ****** Nonebot_plugin_templates ******
                             [pypi] [python] [pypi]
                                [onebot]_[github]
-## ææ°çæ¬å·0.1.1 # åè½:æä¾ä¸äºjinja2
+## ææ°çæ¬å·0.1.3 # åè½:æä¾ä¸äºjinja2
 templatesæ¸²æ,å¹¶æä¾æå»ºæéåæ°çç±» > æå»ºä¸ä¸ªèåçç¤ºä¾
 ```python from nonebot_plugin_templates.template_types import * from
 nonebot_plugin_templates.templates_render import menu_render, colorlist_render
 menu = Menu("ç§æbot",
 des="ä½¿ç¨åç®¡çèªå·±ç¬æçbotçå½ä»¤,ç§æbotåªæä¸»äººå¯ä½¿ç¨,å¶ä»äººæ æ³ä½¿ç¨",
-funcs=Funcs(Func("/botåç§°+è¯¢é®çé®é¢",
+funcs=Funcs( Func("/botåç§°+è¯¢é®çé®é¢",
 "ä¸æå®å±äºèªå·±çbotå¯¹è¯\n
 (å¯ä½¿ç¨'åå¤'æbotæåä¸ä¸ªç­æ¡æ¥è¿ç»­åå®å¯¹è¯)\n
 (å¯åå¤'æ¸é¤åå²','å·æ°å¯¹è¯'æ¥æ¸é¤botçå¯¹è¯è®°å¿)") + Func("/
 ææbot",
 "æ¥è¯¢ææçå¯ç¨çç§æçbot,ä»¥è·åbotåç§°åç¸å³ä¿¡æ¯") +
 Func("/åå»ºbot", "åå»ºæ°çç§æçbot") + Func("/æ¹åbot",
 "æ´æ¹èªå·±çbotçåç§°") + Func("/å é¤bot",
@@ -31,9 +31,9 @@
 ("botåç§°+è¯¢é®çé®é¢", "ä¸æå®å±äºå¬å±çbotå¯¹è¯\n
 (å¯ä½¿ç¨'åå¤'æbotæåä¸ä¸ªç­æ¡æ¥è¿ç»­åå®å¯¹è¯)\n
 (å¯åå¤'æ¸é¤åå²','å·æ°å¯¹è¯'æ¥æ¸é¤botçå¯¹è¯è®°å¿)") + Func
 ("ææbot",
 "æ¥è¯¢ææçå¯ç¨çå¬å±çbot,ä»¥è·åbotåç§°åç¸å³ä¿¡æ¯") +
 Func("åå»ºbot", "åå»ºæ°çå¬ç¨çbot") + Func("æ¹åbot",
 "æ´æ¹å¬ç¨çbotçåç§°") + Func("å é¤bot",
-"å é¤æå®å¬ç¨çbot"))) pic_bytes = await menu_render(menu, 800) ``` >
-æå»ºä¸ä¸ªå¡çåè¡¨çç¤ºä¾
+"å é¤æå®å¬ç¨çbot"))) pic_bytes = await menu_render(menu, 800) ``` !
+[menu.png](src/menu.png) > æå»ºä¸ä¸ªå¡çåè¡¨çç¤ºä¾
```

