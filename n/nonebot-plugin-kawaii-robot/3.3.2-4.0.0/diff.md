# Comparing `tmp/nonebot_plugin_kawaii_robot-3.3.2.tar.gz` & `tmp/nonebot-plugin-kawaii-robot-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kawaii_robot-3.3.2.tar", last modified: Thu May 25 05:08:22 2023, max compression
+gzip compressed data, was "nonebot-plugin-kawaii-robot-4.0.0.tar", last modified: Mon Jul 24 10:40:04 2023, max compression
```

## Comparing `nonebot_plugin_kawaii_robot-3.3.2.tar` & `nonebot-plugin-kawaii-robot-4.0.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.254099 nonebot_plugin_kawaii_robot-3.3.2/
--rw-rw-rw-   0        0        0    35184 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/LICENSE
--rw-rw-rw-   0        0        0       63 2022-07-08 21:05:45.000000 nonebot_plugin_kawaii_robot-3.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      334 2023-05-25 05:08:22.253598 nonebot_plugin_kawaii_robot-3.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3285 2022-12-24 11:13:16.000000 nonebot_plugin_kawaii_robot-3.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.235082 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/
--rw-rw-rw-   0        0        0     5220 2023-05-25 04:47:57.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/__init__.py
--rw-rw-rw-   0        0        0      912 2023-05-25 04:43:40.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/config.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.250596 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/
--rw-rw-rw-   0        0        0    81633 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/data.json
--rw-rw-rw-   0        0        0    12541 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/leaf.json
--rw-rw-rw-   0        0        0     3944 2023-05-25 04:42:06.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.244090 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/
--rw-rw-rw-   0        0        0      334 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 05:08:22.254599 nonebot_plugin_kawaii_robot-3.3.2/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-05-25 05:08:17.000000 nonebot_plugin_kawaii_robot-3.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:04.337773 nonebot-plugin-kawaii-robot-4.0.0/
+-rw-rw-rw-   0        0        0    35184 2022-08-21 05:19:27.000000 nonebot-plugin-kawaii-robot-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0       63 2022-07-08 21:05:45.000000 nonebot-plugin-kawaii-robot-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8812 2023-07-24 10:40:04.337271 nonebot-plugin-kawaii-robot-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8286 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:04.322303 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/
+-rw-rw-rw-   0        0        0      514 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/__init__.py
+-rw-rw-rw-   0        0        0     5339 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/__main__.py
+-rw-rw-rw-   0        0        0     2962 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/config.py
+-rw-rw-rw-   0        0        0     1471 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/const.py
+-rw-rw-rw-   0        0        0     5269 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/data_source.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:04.335315 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/resource/
+-rw-rw-rw-   0        0        0    78416 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/resource/data.json
+-rw-rw-rw-   0        0        0    10765 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/resource/leaf.json
+-rw-rw-rw-   0        0        0     3700 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:04.330811 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/
+-rw-rw-rw-   0        0        0     8812 2023-07-24 10:40:04.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-24 10:40:04.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:40:04.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-24 10:40:04.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-24 10:40:04.000000 nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      704 2023-07-24 10:33:37.000000 nonebot-plugin-kawaii-robot-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:40:04.337773 nonebot-plugin-kawaii-robot-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-07-24 10:40:00.000000 nonebot-plugin-kawaii-robot-4.0.0/setup.py
```

### Comparing `nonebot_plugin_kawaii_robot-3.3.2/LICENSE` & `nonebot-plugin-kawaii-robot-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/__init__.py` & `nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,192 @@
-from nonebot.plugin.on import on_message,on_notice
-from nonebot.rule import to_me
+import asyncio
+import random
+from typing import Dict
+
 from nonebot.adapters.onebot.v11 import (
     GROUP,
+    Bot,
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
     PokeNotifyEvent,
 )
-
-import nonebot
-import asyncio
-import re
-import random
-
+from nonebot.matcher import Matcher
+from nonebot.plugin.on import on_message, on_notice
+from nonebot.rule import Rule, to_me
+
+from .config import config
+from .data_source import (
+    LOADED_HELLO_REPLY,
+    LOADED_INTERRUPT_MSG,
+    LOADED_POKE_REPLY,
+    LOADED_REPLY_DICT,
+    LOADED_UNKNOWN_REPLY,
+)
 from .utils import (
-    MyThesaurus,
-    LeafThesaurus,
-    AnimeThesaurus,
+    check_percentage,
+    choice_reply,
+    finish_multi_msg,
+    format_sender_username,
+    format_username_from_event,
+    full_match_search,
+    get_username_by_id,
     keyword_search,
-    hello__reply,
-    poke__reply,
-    unknow_reply,
-    interrupt_msg,
-    messagePreprocess
-    )
+    transform_message,
+)
 
-from .config import Config
+# region 词库回复
 
-# 加载全局配置
-global_config = nonebot.get_driver().config
-leaf = Config.parse_obj(global_config.dict())
 
-reply_type = leaf.leaf_reply_type
-poke_rand = leaf.leaf_poke_rand
+async def ignore_rule(event: MessageEvent) -> bool:
+    msg = event.get_plaintext().strip()
 
-repeater_limit = leaf.leaf_repeater_limit
-interrupt = leaf.leaf_interrupt
+    # 消息以忽略词开头
+    if next(
+        (x for x in config.leaf_ignore if msg.startswith(x)),
+        None,
+    ):
+        return False
+
+    # at 始终触发
+    if event.is_tome():
+        return True
+
+    # 没 at，启用非 at 回复，并且概率满足
+    if (
+        # (not event.is_tome()) and
+        (not config.leaf_need_at)
+        and check_percentage(config.leaf_trigger_percent)
+    ):
+        return True
+
+    return False
+
+
+async def talk_matcher_handler(matcher: Matcher, event: MessageEvent):
+    # 获取消息文本
+    msg = event.get_plaintext().strip()
+
+    # 用户 id 和昵称处理
+    user_id = event.get_user_id()
+    username = format_username_from_event(event)
+
+    # 如果是光艾特bot(没消息返回)，就回复以下内容
+    if (not msg) and event.is_tome():
+        await finish_multi_msg(
+            matcher,
+            choice_reply(LOADED_HELLO_REPLY, user_id, username),
+        )
 
-ignore = leaf.leaf_ignore
+    # 从词库中获取回复
+    search_function = (
+        keyword_search if config.leaf_match_pattern == 1 else full_match_search
+    )
+    if reply_list := search_function(LOADED_REPLY_DICT, msg):
+        await finish_multi_msg(
+            matcher,
+            choice_reply(reply_list, user_id, username),
+        )
 
-match_pattern = leaf.leaf_match_pattern
+    # 不明白的内容，开启所有回复并 @bot 才会回复
+    if event.is_tome() and config.leaf_reply_type == 1:
+        await finish_multi_msg(
+            matcher,
+            choice_reply(LOADED_UNKNOWN_REPLY, user_id, username),
+        )
 
-if match_pattern == 0:
-    get_chat_result = lambda resource,key:resource.get(key,"")
-else:
-    get_chat_result = keyword_search
 
-at_mod = leaf.leaf_at_mod
+DICT_REPLY_PERM = GROUP if config.leaf_permission == "GROUP" else None
+talk = on_message(
+    rule=Rule(ignore_rule) & (to_me() if config.leaf_need_at else None),
+    permission=DICT_REPLY_PERM,
+    priority=99,
+    block=False,
+)
+if config.leaf_reply_type >= 0:
+    talk.handle()(talk_matcher_handler)
 
-# 配置合法检测
 
-if repeater_limit[0] < 2 or repeater_limit[0] > repeater_limit[1]:
-    raise Exception('config error: repeater_limit')
+# endregion
 
-# 权限判断
 
-if leaf.leaf_permission == "GROUP":
-    permission = GROUP
-else:
-    permission = None
+# region 戳一戳
 
-# 优先级99，条件：艾特bot就触发
 
-if reply_type > -1:
-    talk = on_message(
-        rule = to_me() if at_mod == 0 else None,
-        permission = permission,
-        priority = 99,
-        block = False
+async def poke_matcher_handler(bot: Bot, matcher: Matcher, event: PokeNotifyEvent):
+    await asyncio.sleep(random.uniform(*config.leaf_poke_action_delay))
+
+    if check_percentage(config.leaf_poke_rand):
+        await finish_multi_msg(
+            matcher,
+            choice_reply(
+                LOADED_POKE_REPLY,
+                event.get_user_id(),
+                format_sender_username(
+                    await get_username_by_id(bot, event.user_id, event.group_id),
+                ),
+            ),
         )
 
-    @talk.handle()
-    async def _(event: MessageEvent):
-        # 获取消息文本
-        msg = str(event.get_message())
-        # 去掉带中括号的内容(去除cq码)
-        msg = re.sub(r"\[.*?\]", "", msg)
-
-        # 如果是光艾特bot(没消息返回)，就回复以下内容
-        if (not msg) or msg.isspace():
-            if at_mod == 0:
-                await talk.finish(Message(random.choice(hello__reply)))
-
-        # 如果是已配置的忽略项，直接结束事件
-        for i in range(len(ignore)):
-            if msg.startswith(ignore[i]):
-                await talk.finish()
-
-        # 获取用户nickname
-        if isinstance(event, GroupMessageEvent):
-            nickname = event.sender.card or event.sender.nickname
-        else:
-            nickname = event.sender.nickname
-
-        if len(nickname) > 10:
-            nickname = nickname[:2] + \
-                random.choice(["酱", "亲", "ちゃん", "同志", "老师"])
-
-        # 从个人字典里获取结果
-        if result := get_chat_result(MyThesaurus, msg):
-            await talk.finish(Message(result))
-
-        # 从 LeafThesaurus 里获取结果
-        if result := get_chat_result(LeafThesaurus, msg):
-            await talk.finish(Message(result.replace("name", nickname)))
-
-        # 从 AnimeThesaurus 里获取结果
-        if result := get_chat_result(AnimeThesaurus, msg):
-            await talk.finish(Message(result.replace("你", nickname)))
-
-        # 不明白的内容
-        if at_mod == 0 and reply_type == 1:
-            await talk.finish(Message(random.choice(unknow_reply)))
-
-# 优先级10，不会向下阻断，条件：戳一戳bot触发
-
-if poke_rand > -1:
-    poke_ = on_notice(rule = to_me(), priority=10, block=False)
-    @poke_.handle()
-    async def _poke_event(event: PokeNotifyEvent):
-        if event.is_tome:
-            if poke_rand == 0:
-                await asyncio.sleep(1.0)
-                await poke_.finish(Message(f'[CQ:poke,qq={event.user_id}]'))
-            else:
-                if random.randint(1,100) <= poke_rand:
-                    await asyncio.sleep(1.0)
-                    await poke_.finish(Message(random.choice(poke__reply)))
-                else:
-                    await asyncio.sleep(1.0)
-                    await poke_.finish(Message(f'[CQ:poke,qq={event.user_id}]'))
-
-# 打断/复读姬
-
-if interrupt > -1:
-    global msg_last,msg_times,repeater_times
-    msg_last = {}
-    msg_times = {}
-    repeater_times = {}
-
-    async def repeat(event: GroupMessageEvent) -> bool:
-        global msg_last, msg_times,repeater_times
-        group_id = event.group_id
-        msg = messagePreprocess(event.message)
-        if msg_last.get(group_id) == msg:
-            repeater_times.setdefault(group_id,random.randint(repeater_limit[0], repeater_limit[1]))
-            msg_times[group_id] += 1
-            if msg_times[group_id] == repeater_times[group_id]:
-                repeater_times[group_id] = random.randint(repeater_limit[0], repeater_limit[1])
-                msg_times[group_id] += repeater_limit[1]
-                return True
-            else:
-                return False
-        else:
-            msg_last[group_id] = msg
-            msg_times[group_id] = 1
+    await matcher.finish(MessageSegment("poke", {"qq": event.user_id}))
+
+
+poke_matcher = on_notice(rule=to_me(), priority=10, block=False)
+if config.leaf_poke_rand >= 0:
+    poke_matcher.handle()(poke_matcher_handler)
+
+
+# endregion
+
+
+# region 打断/复读姬
+
+msg_last: Dict[int, Message] = {}  # 存储群内最后一条消息
+msg_times: Dict[int, int] = {}  # 存储群内最后一条消息被复读的次数
+repeater_times: Dict[int, int] = {}  # 存储随机生成的复读上限
+
+
+async def repeat_rule(event: GroupMessageEvent) -> bool:
+    group_id = event.group_id
+
+    # 复读
+    if msg_last.get(group_id) == event.message:
+        if group_id not in msg_times:
             return False
 
-    repeater = on_message(rule=repeat, permission=GROUP, priority=99, block=False)
+        msg_times[group_id] += 1
+        if group_id not in repeater_times:
+            repeater_times[group_id] = random.randint(*config.leaf_repeater_limit)
+
+        if msg_times[group_id] >= repeater_times[group_id]:
+            del msg_times[group_id]  # del 掉防止继续复读
+            del repeater_times[group_id]
+            return True
+
+        return False
+
+    # 不同消息，未复读
+    msg_last[group_id] = event.message
+    msg_times[group_id] = 1
+    return False
+
+
+async def repeater_matcher_handler(matcher: Matcher, event: GroupMessageEvent):
+    if check_percentage(config.leaf_interrupt):
+        msg_times[event.group_id] = 0  # 让下次复读计入次数统计，以便再次打断或复读
+        await finish_multi_msg(
+            matcher,
+            choice_reply(
+                LOADED_INTERRUPT_MSG,
+                event.get_user_id(),
+                format_username_from_event(event),
+            ),
+        )
+    await matcher.finish(transform_message(event.message))
+
+
+repeater = on_message(rule=repeat_rule, permission=GROUP, priority=99, block=False)
+if config.leaf_interrupt >= 0:
+    repeater.handle()(repeater_matcher_handler)
 
-    @repeater.handle()
-    async def _(event: GroupMessageEvent):
-        if random.randint(1,100) <= interrupt:
-            await repeater.finish(random.choice(interrupt_msg))
-        else:
-            await repeater.finish(event.message)
+# endregion
```

### Comparing `nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/leaf.json` & `nonebot-plugin-kawaii-robot-4.0.0/nonebot_plugin_kawaii_robot/resource/leaf.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9556092056092058%*

 * *Differences: {"'fw'": "{insert: [(2, '咱才不是废物...标记[CQ:at,qq={user_id}]')], delete: [2]}",*

 * * "'口爆'": "{insert: [(9, '呜呜呜...{username}大坏蛋 ~ ♡')], delete: [9]}",*

 * * "'后入'": "{insert: [(9, '呜呜呜...{username}大坏蛋 ~ ♡')], delete: [9]}",*

 * * "'干烂'": "{insert: [(9, '呜呜呜...{username}大坏蛋 ~ ♡')], delete: [9]}",*

 * * "'废物'": "{insert: [(2, '咱才不是废物...标记[CQ:at,qq={user_id}]')], delete: [2]}",*

 * * "'标记'": "['...标记[CQ:at,qq={user_id}]', '[CQ:at,qq={user_id}] 已标记✓', '[CQ:at,qq={user_id}] "*

 * *         "标记成功喵(´▽｀)', '[CQ:at,qq={user_id}] ✓']",*

 * * "'烧杯'": "{i […]*

```diff
@@ -1,12 +1,12 @@
 {
     "fw": [
         " \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u554a...(\u00b0\u30fc\u00b0\u3003)",
-        "\u54b1\u624d\u4e0d\u662f\u5e9f\u7269...\u6807\u8bb0@name",
+        "\u54b1\u624d\u4e0d\u662f\u5e9f\u7269...\u6807\u8bb0[CQ:at,qq={user_id}]",
         "\u624d\u4e0d\u662f...",
         "\u679c\u54a9 ~ ",
         "\u545c...",
         "\u545c\u545c...\u5bf9\u4e0d\u8d77QAQ"
     ],
     "jb": [
         "\uff08\u5438\u6e9c\u5438\u6e9c\uff09",
@@ -52,15 +52,15 @@
         "\u545c...\u8e6d\u8e6d...\u2661",
         "\u8e6d\u8e6d...\u2661",
         "\u5416 ~\u266a",
         "\u55ef\u2661...\u545c\u2661",
         "\u545c\u55b5\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u5e72\u561bqwq",
         "\u545c\u54c7\uff01..\u55b5\u545c ~ \u2661",
-        "\u545c\u545c\u545c...name\u5927\u574f\u86cb ~ \u2661"
+        "\u545c\u545c\u545c...{username}\u5927\u574f\u86cb ~ \u2661"
     ],
     "\u53eb\u7238": [
         "\u55b5\u2661",
         "\u54d2\u54a9~",
         "\u4e0d\u8981ww",
         "\uff08\u5c0f\u58f0\uff09\u545c\u55b5 ~ \u7238\u7238\u2661",
         "\u7238\u7238(*/\u03c9\uff3c*)",
@@ -99,15 +99,15 @@
         "\u545c...\u8e6d\u8e6d...\u2661",
         "\u8e6d\u8e6d...\u2661",
         "\u5416 ~\u266a",
         "\u55ef\u2661...\u545c\u2661",
         "\u545c\u55b5\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u5e72\u561bqwq",
         "\u545c\u54c7\uff01..\u55b5\u545c ~ \u2661",
-        "\u545c\u545c\u545c...name\u5927\u574f\u86cb ~ \u2661"
+        "\u545c\u545c\u545c...{username}\u5927\u574f\u86cb ~ \u2661"
     ],
     "\u5582\u4f60": [
         "\u55ef~",
         "\u597d\u8036~",
         "\u55b5\u2661 ~\u597d\u597d\u5403 ~",
         "\u545c...",
         "\u597d\u8036~\uff08\u5f00\u5fc3\uff09",
@@ -166,20 +166,20 @@
         "\u545c...\u8e6d\u8e6d...\u2661",
         "\u8e6d\u8e6d...\u2661",
         "\u5416 ~\u266a",
         "\u55ef\u2661...\u545c\u2661",
         "\u545c\u55b5\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u5e72\u561bqwq",
         "\u545c\u54c7\uff01..\u55b5\u545c ~ \u2661",
-        "\u545c\u545c\u545c...name\u5927\u574f\u86cb ~ \u2661"
+        "\u545c\u545c\u545c...{username}\u5927\u574f\u86cb ~ \u2661"
     ],
     "\u5e9f\u7269": [
         " \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u554a...(\u00b0\u30fc\u00b0\u3003)",
-        "\u54b1\u624d\u4e0d\u662f\u5e9f\u7269...\u6807\u8bb0@name",
+        "\u54b1\u624d\u4e0d\u662f\u5e9f\u7269...\u6807\u8bb0[CQ:at,qq={user_id}]",
         "\u624d\u4e0d\u662f...",
         "\u679c\u54a9 ~ ",
         "\u545c...",
         "\u545c\u545c...\u5bf9\u4e0d\u8d77QAQ"
     ],
     "\u5f20\u5634": [
         "\u554a\u545c ~ ",
@@ -205,18 +205,18 @@
     ],
     "\u6574\u6d3b": [
         "\u4e0d\u8981QAQ",
         "\u54d2\u54a9\u00d7",
         "\u133f \u1288 \u127c \u12fd \u133f"
     ],
     "\u6807\u8bb0": [
-        "...\u6807\u8bb0@name",
-        "@name\u5df2\u6807\u8bb0\u2713",
-        "@name\u6807\u8bb0\u6210\u529f\u55b5(\u00b4\u25bd\uff40)",
-        "@name\u2713"
+        "...\u6807\u8bb0[CQ:at,qq={user_id}]",
+        "[CQ:at,qq={user_id}] \u5df2\u6807\u8bb0\u2713",
+        "[CQ:at,qq={user_id}] \u6807\u8bb0\u6210\u529f\u55b5(\u00b4\u25bd\uff40)",
+        "[CQ:at,qq={user_id}] \u2713"
     ],
     "\u6a44\u6984": [
         "nya\u2661",
         "\u8e6d\u8e6d...\u2661",
         "\u5416 ~\u266a",
         "\u55ef\u2661...\u545c\u2661",
         "\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
@@ -230,30 +230,30 @@
         "\u4f60\u518d\u8fd9\u6837\u54b1\u5c31\u4e0d\u7406\u4f60\u4e86\uff08\uff1e\u0434\uff1c\uff09",
         "...\u8d85\u5e02",
         "\u545c...",
         "\u7b28\u86cb...(\u5c0f\u5c0f\u58f0)",
         "\u624d\u4e0d\u662f\uff01 \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "///////",
         "\uff08\u5bb3\u6015\uff09\u54b1...\u6ca1\u6709QAQ",
-        "@name\u8bf7\u4f60show show way ~ ",
+        "[CQ:at,qq={user_id}] \u8bf7\u4f60show show way ~ ",
         "\u4e0d\u662f\u55b5\uff01",
         "no\uff01",
         "(\u5f31\u5f31\u5730)\u545c...\u679c\u54a9...",
         "\u5440 ~ hentai>_<"
     ],
     "\u70e7\u9e21": [
         " \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u4f60\u518d\u8fd9\u6837\u54b1\u5c31\u4e0d\u7406\u4f60\u4e86\uff08\uff1e\u0434\uff1c\uff09",
         "...\u8d85\u5e02",
         "\u545c...",
         "\u7b28\u86cb...(\u5c0f\u5c0f\u58f0)",
         "\u624d\u4e0d\u662f\uff01 \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "///////",
         "\uff08\u5bb3\u6015\uff09\u54b1...\u6ca1\u6709QAQ",
-        "@name\u8bf7\u4f60show show way ~ ",
+        "[CQ:at,qq={user_id}] \u8bf7\u4f60show show way ~ ",
         "\u4e0d\u662f\u55b5\uff01",
         "no\uff01",
         "(\u5f31\u5f31\u5730)\u545c...\u679c\u54a9...",
         "\u5440 ~ hentai>_<"
     ],
     "\u7206\u7092": [
         "nya\u2661",
@@ -367,23 +367,23 @@
         "\u545c...\u8e6d\u8e6d...\u2661",
         "\u8e6d\u8e6d...\u2661",
         "\u5416 ~\u266a",
         "\u55ef\u2661...\u545c\u2661",
         "\u545c\u55b5\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u5e72\u561bqwq",
         "\u545c\u54c7\uff01..\u55b5\u545c ~ \u2661",
-        "\u545c\u545c\u545c...name\u5927\u574f\u86cb ~ \u2661"
+        "\u545c\u545c\u545c...{username}\u5927\u574f\u86cb ~ \u2661"
     ],
     "\u8bc4\u4ef7": [
         "\u5982\u4f55\u8bc4\u4ef7\u5982\u4f55\u8bc4\u4ef7\u55b5\uff1f",
         "\u55b5\uff1f",
         "\u5e0c\u814a\u5976~",
         "\u8c22\u9080\uff0c\u54b1\u4e0d\u4f1a\u8bc4\u4ef7\u5462,,,",
         "\u8c22\u9080\uff0c\u4e4b\u540e\u5fd8\u4e86www",
-        "\u8bc4\u4ef7\u4ec0\u4e48\u8bc4\u4ef7\uff0c>_<name\u4e2a\u5927\u7b28\u86cb\uff01",
+        "\u8bc4\u4ef7\u4ec0\u4e48\u8bc4\u4ef7\uff0c>_<{username}\u4e2a\u5927\u7b28\u86cb\uff01",
         "\u4e0d\u77e5\u9053...",
         "\u54b1\u89c9\u5f97......\u55ef......\u54b1\u4e0d\u77e5\u9053\u03bf(=\u00b7\u03c9\uff1c=)\u2606kira",
         "(\u5077\u770b ~)|\u2e1d\u2022\u1d17\u2022\u2e1d\u2e1d)",
         "\u8bc4\u4ef7\u4e3a\uff1a(\u0e51\uff1e \uff1c)\u2606"
     ],
     "\u8d85\u5e02": [
         " \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
@@ -412,25 +412,25 @@
         "\u2570(*\u00b0\u25bd\u00b0*)\u256f",
         "~~( \ufe41 \ufe41 ) ~~~",
         "\u55ef\u2661"
     ],
     "\u94f8\u5e01": [
         " \u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
         "\u554a...(\u00b0\u30fc\u00b0\u3003)",
-        "\u54b1\u624d\u4e0d\u662f\u94f8\u5e01...\u6807\u8bb0@name",
+        "\u54b1\u624d\u4e0d\u662f\u94f8\u5e01...\u6807\u8bb0[CQ:at,qq={user_id}]",
         "\u624d\u4e0d\u662f...",
         "\u679c\u54a9 ~ ",
         "\u545c...",
         "\u545c\u545c...\u5bf9\u4e0d\u8d77QAQ",
         "\u55b5\uff01\uff08\u751f\u6c14\u55b5\uff09"
     ],
     "\u9a82\u6211": [
         "\u4f60\u600e\u4e48\u50bbfufu\u7684\u2661 ~ ",
         "no ~ ",
-        "\u6807\u8bb0\u4e3a\u5c0fm~\u266a @name",
-        "...\u545c...name\u662f\u4e2a\u5927\u7b28\u86cb\uff01",
+        "\u6807\u8bb0\u4e3a\u5c0fm~\u266a [CQ:at,qq={user_id}]",
+        "...\u545c...{username}\u662f\u4e2a\u5927\u7b28\u86cb\uff01",
         "\u554a...\u03a3( \u00b0 \u25b3 \u00b0|||)\ufe34",
-        "\u6211\u61c2\u4e86www ~ name\u662f\u4e2a\u574f\u5b69\u5b50o(*\u2267\u25bd\u2266)\u30c4",
+        "\u6211\u61c2\u4e86www ~ {username}\u662f\u4e2a\u574f\u5b69\u5b50o(*\u2267\u25bd\u2266)\u30c4",
         "\u545c\u55b5\uff1f\u2570(*\u00b0\u25bd\u00b0*)\u256f",
         "\u4e0d\u8981 ~~( \ufe41 \ufe41 ) ~~~"
     ]
 }
```

### Comparing `nonebot_plugin_kawaii_robot-3.3.2/setup.py` & `nonebot-plugin-kawaii-robot-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_kawaii_robot',
-version='3.3.2',
+version='4.0.0',
 description='使用Kyomotoi / AnimeThesaurus的nonebot2的回复（文i）插件',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='AGPLv3 License',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_kawaii_robot","nonebot_plugin_kawaii_robot.*"]),
```

