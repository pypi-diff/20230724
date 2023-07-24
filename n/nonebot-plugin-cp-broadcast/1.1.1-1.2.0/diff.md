# Comparing `tmp/nonebot_plugin_cp_broadcast-1.1.1.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-1.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-1.2.0.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-1.1.1.tar` & `nonebot_plugin_cp_broadcast-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-16 02:14:37.191455 nonebot_plugin_cp_broadcast-1.1.1/LICENSE
--rw-r--r--   0        0        0     5432 2023-07-16 02:14:37.191455 nonebot_plugin_cp_broadcast-1.1.1/README.md
--rw-r--r--   0        0        0     8511 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2699 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     3665 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      589 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0     7803 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/sqlite3.py
--rw-r--r--   0        0        0      732 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 16:02:39.141584 nonebot_plugin_cp_broadcast-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5779 2023-07-24 16:02:39.141584 nonebot_plugin_cp_broadcast-1.2.0/README.md
+-rw-r--r--   0        0        0     8839 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2699 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     3665 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      669 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0     8172 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/sqlite3.py
+-rw-r--r--   0        0        0      732 2023-07-24 16:02:39.157584 nonebot_plugin_cp_broadcast-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/LICENSE` & `nonebot_plugin_cp_broadcast-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/README.md` & `nonebot_plugin_cp_broadcast-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 除了简单的指令外，它支持每天定时发送三种比赛的信息。
 
 查询的结果会存到列表里，以减少网站爬取的次数。
 
 由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
 
-除了爬取比赛这一基本功能外，它还支持 Codeforces 平台一些信息的查询，具体指令将在下文介绍。
+除了爬取比赛信息这一基本功能外，它还支持 Codeforces 平台一些信息的查询，譬如监视某个 id 的 rating 变化情况，具体指令将在下文介绍。
 
 为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
 
-这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
+插件可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
 
 有任何问题可联系QQ：3411907440。
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -86,14 +86,17 @@
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
 | cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
 | cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
+| cp_broadcast_cf_list | 否 | [ ] | 开启 Codeforces 播报功能的群聊，cf监视的相关功能只在指定群聊里发送 |
+| cp_broadcast_cf_interval | 否 | 10 | 更新 Codeforces 监视信息的时间间隙，默认为 10 分钟 |
+
 
 该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你未安装此依赖的话，将无法触发与定时相关的功能。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
@@ -117,18 +120,22 @@
 
 <img src="./docs/atc.JPG" style="zoom:30%;" />
 
 <img src="./docs/today.JPG" style="zoom:30%;" />
 
 <img src="./docs/next.JPG" style="zoom:30%;" />
 
-<img src="./docs/help.JPG" style="zoom:30%;" />
+<img src="./docs/help.jpg" style="zoom:30%;" />
 
 <img src="./docs/update.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
 
 <img src="./docs/remove.png" style="zoom:30%;" />
 
 <img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
+
+<img src="./docs/cf_change.png" style="zoom:30%;" />
+
+<img src="./docs/cf_change2.jpg" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -6,22 +6,21 @@
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
 è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
 é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
 æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
 AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
 APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
-é¤äºç¬åæ¯èµè¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
-å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å
-cp-broadcast
+é¤äºç¬åæ¯èµä¿¡æ¯è¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
+å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼è­¬å¦çè§æä¸ª id ç rating
+ååæåµï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å cp-broadcast
 è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
 Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
 æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
-è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
-é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
+æä»¶å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
 requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cp-broadcast
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cp-broadcast   pdm pdm add nonebot-plugin-cp-
 broadcast   poetry poetry add nonebot-plugin-cp-broadcast   conda conda install
@@ -35,26 +34,30 @@
 | å¡«å¥ä½  bot çåå­ï¼å¨ `help` æä»¤ä¸ä¼ä½¿ç¨å°ä½ ç bot
 çåå­ | | cp_broadcast_time | å¦ | {"hour":"7", "minute":"20"} |
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
 20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
 | cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
 åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
-| è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
-plugin-apscheduler)
+| | cp_broadcast_cf_list | å¦ | [ ] | å¼å¯ Codeforces
+æ­æ¥åè½çç¾¤èï¼cfçè§çç¸å³åè½åªå¨æå®ç¾¤èéåé | |
+cp_broadcast_cf_interval | å¦ | 10 | æ´æ° Codeforces
+çè§ä¿¡æ¯çæ¶é´é´éï¼é»è®¤ä¸º 10 åé | è¯¥æä»¶ä¾èµ
+[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)
 å®ç°å®æ¶åéåè½ï¼å¦æä½ æªå®è£æ­¤ä¾èµçè¯ï¼å°æ æ³è§¦åä¸å®æ¶ç¸å³çåè½ã
 ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
 çè§æäººç rating åå | | `cfçè§ç§»é¤` | ç¾¤å | æ¯ | ç¾¤è |
 ç§»é¤çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ |
 ç¾¤è | å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è
 | æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/
-nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG]
+nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.jpg]
 [./docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/remove.png] [./docs/
-cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG]
+cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG] [./docs/cf_change.png] [./docs/
+cf_change2.jpg]
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 from nonebot.log import logger
 import asyncio
 
 cp_broadcast_list = cp_broadcast_config.cp_broadcast_list
 cp_broadcast_botname = cp_broadcast_config.cp_broadcast_botname
 cp_broadcast_time = cp_broadcast_config.cp_broadcast_time
 cp_broadcast_updatetime = cp_broadcast_config.cp_broadcast_updatetime
+cp_broadcast_cf_list = cp_broadcast_config.cp_broadcast_cf_list
+cp_broadcast_cf_interval = cp_broadcast_config.cp_broadcast_cf_interval
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="算法竞赛比赛查询",
     description="可以查询牛客、atcoder、codeforces平台的今天和近几天的比赛信息",
     usage=\
         "cf->查询cf比赛\n"\
         "@{botname} cf查询+id->查询某人信息\n"\
         "@{botname} cf监视+id->监视某人rating变化\n"\
-        "@{botname} cf监视移除+id->不再监视某人rating变化"\
+        "@{botname} cf监视移除+id->不再监视某人rating变化\n"\
         "@{botname} cf监视列表->展示已监视的选手id\n"\
         "nc/牛客->查询牛客比赛\n"\
         "atc->查询atcoder比赛\n"\
         "today->查询今天的比赛\n"\
         "next->查询明天之后的部分比赛\n"
         "update->更新比赛数据\n"\
         "about->{botname}的一些信息\n",
@@ -234,25 +236,30 @@
 update_matcher = on_fullmatch('update', priority=70, block=True)
 @update_matcher.handle()
 async def reply():
     await update()
     await update_matcher.finish('数据已更新完成')
 
 
-#cf分数变化提醒
-async def ratingReminder():
+#cf分数变化提醒、cf上线提醒
+async def cfBroadcast():
     await asyncio.sleep(1)
     logger.info('cf分数变化检测开始')
-    messList = await returRatingChangeInfo()
+    messList = await returChangeInfo()
     if len(messList) == 0:
         return
-    for id in cp_broadcast_list:
+    for id in cp_broadcast_cf_list:
         await asyncio.sleep(2)
-        for mess in messList:
-            await get_bot().send_group_msg(group_id=id, message=mess['output'])
+        for mess in messList['ratingChange']:
+            await get_bot().send_group_msg(group_id=id, message=mess)
+            await asyncio.sleep(2)
+
+        for mess in messList['cfOnline']:
+            await get_bot().send_group_msg(group_id=id, message=mess)
             await asyncio.sleep(2)
+        
 
 
 if scheduler:
     scheduler.add_job(
-        ratingReminder, "interval", minutes=20, id="ratingReminder"
+        cfBroadcast, "interval", minutes=cp_broadcast_cf_interval, id="cfBroadcast"
     )
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/config.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,13 +5,15 @@
 from nonebot import get_driver
 
 class Config(BaseModel, extra=Extra.ignore):
     cp_broadcast_list: List[str] = []
     cp_broadcast_botname: str = "bot"
     cp_broadcast_time: Dict[str, str] = {"hour" : "7", "minute" : "20"}
     cp_broadcast_updatetime: Dict[str, str] = {"hour" : "0", "minute" : "0"}
+    cp_broadcast_cf_list: List[str] = []
+    cp_broadcast_cf_interval: int = 10
 
 cp_broadcast_path = Path() / "data" / "cp_broadcast"
 cf_user_info_baseurl = 'https://codeforces.com/api/user.info?handles='
 
 
 cp_broadcast_config = Config.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/sqlite3.py` & `nonebot_plugin_cp_broadcast-1.2.0/nonebot_plugin_cp_broadcast/sqlite3.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     )
 """
 )
 
 class CF_UserType:
     def __init__(self, id, now_rating, update_time, QQ, status, last_rating, avatar_url):
         self.id = id
-        self.now_rating = now_rating if now_rating is not None else 0
+        self.now_rating = now_rating if now_rating is not None else 0                  # cf上次上线时间
         self.update_time = update_time if update_time is not None else 0
         self.QQ = QQ if QQ is not None else 0
         self.status = status if status is not None else 1
         self.last_rating = last_rating if last_rating is not None else 0
         self.avatar_url = avatar_url
 
 async def addUser(id: str, QQ: int):
@@ -50,15 +50,15 @@
         logger.warning(e)
         return False
     
     if data['status'] == 'OK':
         results = data['result']
 
         for result in results:
-            update_time = int(datetime.datetime.now().timestamp())
+            update_time = int(result["lastOnlineTimeSeconds"])
             user = CF_UserType(result["handle"], result["rating"], update_time, QQ, 1, result["rating"], result["avatar"])
             cursor.execute('''
             INSERT OR REPLACE INTO CF_User (id, now_rating, update_time,QQ,status,last_rating,avatar_url)
             VALUES (?, ?, ?, ?, ?, ?, ?)
         ''', (
                 user.id,
                 user.now_rating,
@@ -106,15 +106,15 @@
     
     conn.execute('DELETE FROM CF_User WHERE id = ?', (cfid,))
     conn.commit()
 
     return True
         
 async def updateUser():
-    Users = []
+    Users = {'ratingChange' : [], 'cfOnline' : []}
     global cf_user_info_baseurl, cursor, conn
 
     cursor.execute('SELECT * FROM CF_User')
     RS = cursor.fetchall()
     for row in RS:
         Oid, Onow_rating, Oupdate_time, OQQ, Ostatus, Olast_rating, Oavatar_url = row
         user_info_url = cf_user_info_baseurl + Oid
@@ -130,17 +130,21 @@
 
         if data["status"] == "OK":
             # 获取result列表
             results = data["result"]
             
             # 遍历每个结果并储存键值
             for result in results:
-                update_time = int(datetime.datetime.now().timestamp())
+                update_time = int(result["lastOnlineTimeSeconds"])
+
+                if update_time != Oupdate_time:
+                    Users['cfOnline'].append(str(Oid))
+
                 user = CF_UserType(Oid, result["rating"], update_time, OQQ, Ostatus, Onow_rating, result["avatar"])
-                Users.append(user)
+                Users['ratingChange'].append(user)
 
                 cursor.execute('''
                 INSERT OR REPLACE INTO CF_User (id, now_rating, update_time,QQ,status,last_rating,avatar_url)
                 VALUES (?, ?, ?, ?, ?, ?, ?)
             ''', (
                 user.id,
                 user.now_rating,
@@ -152,28 +156,32 @@
             ))
                 conn.commit()
         else:
             logger.warning("数据请求失败")
 
     return Users
 
-async def returRatingChangeInfo():
-    outputlist = []
+async def returChangeInfo():
+    outputlist = {'ratingChange' : [], 'cfOnline' : []}
     Users = await updateUser()
 
     global cursor, conn
-    for user in Users:
+    for user in Users['ratingChange']:
         output=f"当前时间：{time.strftime('%Y-%m-%d %H:%M:%S', time.localtime())}\n"
         cursor.execute('SELECT now_rating,last_rating,QQ FROM CF_User WHERE id = ?', (user.id,))
         row = cursor.fetchone()
         now_rating, last_rating, QQ = row
         if last_rating != now_rating:
             change = now_rating - last_rating
             output += f"cf用户 {user.id} 分数发生变化，从 {last_rating} → {now_rating}，变动了{change}分！\n"
-            outputlist.append({'QQ':QQ,'output':output})
+            outputlist['ratingChange'].append(output)
+
+    for id in Users['cfOnline']:
+        ouput = f'卷王 {id} 又开始上cf做题啦！'
+        outputlist['cfOnline'].append(ouput)
 
     return outputlist
 
 
 async def returnBindList():
     global cursor, conn
     cursor.execute('SELECT id FROM CF_User')
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/pyproject.toml` & `nonebot_plugin_cp_broadcast-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "1.1.1"
+version = "1.2.0"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.1/PKG-INFO` & `nonebot_plugin_cp_broadcast-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 1.1.1
+Version: 1.2.0
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -51,19 +51,19 @@
 
 除了简单的指令外，它支持每天定时发送三种比赛的信息。
 
 查询的结果会存到列表里，以减少网站爬取的次数。
 
 由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
 
-除了爬取比赛这一基本功能外，它还支持 Codeforces 平台一些信息的查询，具体指令将在下文介绍。
+除了爬取比赛信息这一基本功能外，它还支持 Codeforces 平台一些信息的查询，譬如监视某个 id 的 rating 变化情况，具体指令将在下文介绍。
 
 为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
 
-这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
+插件可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
 
 有任何问题可联系QQ：3411907440。
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
@@ -110,14 +110,17 @@
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
 | cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
 | cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
+| cp_broadcast_cf_list | 否 | [ ] | 开启 Codeforces 播报功能的群聊，cf监视的相关功能只在指定群聊里发送 |
+| cp_broadcast_cf_interval | 否 | 10 | 更新 Codeforces 监视信息的时间间隙，默认为 10 分钟 |
+
 
 该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你未安装此依赖的话，将无法触发与定时相关的功能。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
@@ -141,19 +144,22 @@
 
 <img src="./docs/atc.JPG" style="zoom:30%;" />
 
 <img src="./docs/today.JPG" style="zoom:30%;" />
 
 <img src="./docs/next.JPG" style="zoom:30%;" />
 
-<img src="./docs/help.JPG" style="zoom:30%;" />
+<img src="./docs/help.jpg" style="zoom:30%;" />
 
 <img src="./docs/update.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
 
 <img src="./docs/remove.png" style="zoom:30%;" />
 
 <img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
 
+<img src="./docs/cf_change.png" style="zoom:30%;" />
+
+<img src="./docs/cf_change2.jpg" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.2.0 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
@@ -19,22 +19,21 @@
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
 è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
 é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
 æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
 AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
 APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
-é¤äºç¬åæ¯èµè¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
-å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å
-cp-broadcast
+é¤äºç¬åæ¯èµä¿¡æ¯è¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
+å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼è­¬å¦çè§æä¸ª id ç rating
+ååæåµï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å cp-broadcast
 è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
 Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
 æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
-è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
-é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
+æä»¶å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
 requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cp-broadcast
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cp-broadcast   pdm pdm add nonebot-plugin-cp-
 broadcast   poetry poetry add nonebot-plugin-cp-broadcast   conda conda install
@@ -48,26 +47,30 @@
 | å¡«å¥ä½  bot çåå­ï¼å¨ `help` æä»¤ä¸ä¼ä½¿ç¨å°ä½ ç bot
 çåå­ | | cp_broadcast_time | å¦ | {"hour":"7", "minute":"20"} |
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
 20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
 | cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
 åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
-| è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
-plugin-apscheduler)
+| | cp_broadcast_cf_list | å¦ | [ ] | å¼å¯ Codeforces
+æ­æ¥åè½çç¾¤èï¼cfçè§çç¸å³åè½åªå¨æå®ç¾¤èéåé | |
+cp_broadcast_cf_interval | å¦ | 10 | æ´æ° Codeforces
+çè§ä¿¡æ¯çæ¶é´é´éï¼é»è®¤ä¸º 10 åé | è¯¥æä»¶ä¾èµ
+[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)
 å®ç°å®æ¶åéåè½ï¼å¦æä½ æªå®è£æ­¤ä¾èµçè¯ï¼å°æ æ³è§¦åä¸å®æ¶ç¸å³çåè½ã
 ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
 çè§æäººç rating åå | | `cfçè§ç§»é¤` | ç¾¤å | æ¯ | ç¾¤è |
 ç§»é¤çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ |
 ç¾¤è | å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è
 | æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/
-nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG]
+nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.jpg]
 [./docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/remove.png] [./docs/
-cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG]
+cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG] [./docs/cf_change.png] [./docs/
+cf_change2.jpg]
```

