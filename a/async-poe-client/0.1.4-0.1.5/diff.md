# Comparing `tmp/async_poe_client-0.1.4.tar.gz` & `tmp/async_poe_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_poe_client-0.1.4.tar", max compression
+gzip compressed data, was "async_poe_client-0.1.5.tar", max compression
```

## Comparing `async_poe_client-0.1.4.tar` & `async_poe_client-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.1.4/async_poe_client/__init__.py
--rw-r--r--   0        0        0    48142 2023-07-23 16:01:36.759102 async_poe_client-0.1.4/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.1.4/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.1.4/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.1.4/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.1.4/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.1.4/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.1.4/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.1.4/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.1.4/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.1.4/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.1.4/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.1.4/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.1.4/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.1.4/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.1.4/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.1.4/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.1.4/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.1.4/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.1.4/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.1.4/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     2503 2023-07-23 15:04:11.447268 async_poe_client-0.1.4/async_poe_client/util.py
--rw-r--r--   0        0        0      449 2023-07-23 16:13:07.483628 async_poe_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    16803 2023-07-23 15:24:44.339601 async_poe_client-0.1.4/README.md
--rw-r--r--   0        0        0    17055 1970-01-01 00:00:00.000000 async_poe_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.1.5/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    48195 2023-07-24 06:00:08.496045 async_poe_client-0.1.5/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.1.5/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.1.5/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.1.5/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.1.5/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.1.5/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.1.5/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.1.5/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.1.5/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.1.5/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.1.5/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.1.5/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.1.5/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.1.5/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.1.5/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.1.5/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.1.5/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.1.5/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.1.5/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.1.5/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1757 2023-07-24 05:51:55.142681 async_poe_client-0.1.5/async_poe_client/util.py
+-rw-r--r--   0        0        0      466 2023-07-24 06:32:51.303458 async_poe_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    16836 2023-07-24 06:32:46.931339 async_poe_client-0.1.5/README.md
+-rw-r--r--   0        0        0    17124 1970-01-01 00:00:00.000000 async_poe_client-0.1.5/PKG-INFO
```

### Comparing `async_poe_client-0.1.4/async_poe_client/client.py` & `async_poe_client-0.1.5/async_poe_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,25 @@
     HOME_URL,
     GQL_URL,
     GQL_RECV_URL,
     SETTING_URL,
     CONST_NAMESPACE,
     generate_data,
     QUERIES,
-    generate_nonce, extract_formkey,
+    generate_nonce,
 )
 
 Websocket_Use_Count = 0
 
 
 class Poe_Client:
-    def __init__(self, p_b: str, proxy: str = ""):
+    def __init__(self, p_b: str, formkey: str, proxy: str = ""):
         self.bots: dict = {}
         self.bot_list_url: str = ""
-        self.formkey: str = ""
+        self.formkey: str = formkey
         self.home_bot_list: List[str] = []
         self.next_data: dict = {}
         self.p_b: str = p_b
         self.sdid: str = ""
         self.subscription: dict = {}
         self.tchannel_data: dict = {}
         self.user_id: str = ""
@@ -42,14 +42,15 @@
         self.proxy = proxy
         self.headers = {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
             'Accept-Encoding': 'gzip, deflate, br',
             'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
             'Cache-Control': 'max-age=0',
             "Cookie": f"p-b={self.p_b}; SL_G_WPT_TO=zh-CN; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1;",
+            "poe-formkey": self.formkey,
             'Sec-Ch-Ua': '"Microsoft Edge";v="117", "Not;A Brand";v="8", "Chromium";v="117"',
             'Sec-Ch-Ua-Mobile': '?0',
             'Sec-Ch-Ua-Platform': '"Windows"',
             'Sec-Fetch-Dest': 'document',
             'Sec-Fetch-Mode': 'navigate',
             'Sec-Fetch-Site': 'same-origin',
             'Sec-Fetch-User': '?1',
@@ -105,23 +106,23 @@
                 self.home_bot_list.append(bot["node"]["handle"])
             self.sdid = str(uuid.uuid5(CONST_NAMESPACE, self.viewer["poeUser"]["id"]))
         except KeyError as e:
             raise ValueError(
                 "Failed to extract 'viewer' or 'user_id' from 'next_data'."
             ) from e
 
-        """extract formkey from response html"""
-        # by @aditiaryan and @ading2210
-        try:
-            self.formkey = extract_formkey(text)
-            self.headers["poe-formkey"] = self.formkey
-        except AttributeError as e:
-            raise ValueError(
-                "Failed to extract 'formkey' from the response text."
-            ) from e
+        # """extract formkey from response html"""
+        # # by @aditiaryan and @ading2210
+        # try:
+        #     self.formkey = extract_formkey(text)
+        #     self.headers["poe-formkey"] = self.formkey
+        # except Exception as e:
+        #     raise ValueError(
+        #         "Failed to extract 'formkey' from the response text."
+        #     ) from e
 
     async def get_channel_data(self) -> None:
         """
         This function fetches the channel data from the SETTING_URL and sets the 'tchanneldata' attribute of the object.
 
         Raises:
             Raises a ValueError if it fails to extract the channel data from the response.
@@ -788,15 +789,15 @@
         """
         ua = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36 Edg/117.0.0.0'
         async with aiohttp.ClientSession(headers={'User-Agent': ua}) as session:
             async with session.ws_connect(self.get_websocket_url(), timeout=3, proxy=self.proxy) as ws:
                 global Websocket_Use_Count
                 if Websocket_Use_Count % 3 == 0:
                     await self.subscribe()
-                    Websocket_Use_Count += 1
+                Websocket_Use_Count += 1
                 human_message_id = await self.send_message(
                     url_botname, question, with_chat_break
                 )
                 last_text = ""
                 message = None
                 yield_header = False
                 suggestion_list = []
```

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `async_poe_client-0.1.5/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.4/README.md` & `async_poe_client-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
 a `Poe_Client` object. You need to pass the `p_b token` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
 from async_poe_client import Poe_Client
 
-poe_client = await Poe_Client("your p_b token").create()
+poe_client = await Poe_Client("your p_b token", "your formkey").create()
 # or with a proxy
-poe_client = await Poe_Client("your p_b token",proxy="socks5://127.0.0.1:7890").create()
+poe_client = await Poe_Client("your p_b token", "your formkey", proxy="socks5://127.0.0.1:7890").create()
 ```
 
 Here, `"your p_b token"` should be replaced with your actual p_b token.
 
 ## Step 2: Use Poe_Client
 
 After creating the `Poe_Client`, you can use it to perform a lot of operations.
```

### Comparing `async_poe_client-0.1.4/PKG-INFO` & `async_poe_client-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: async-poe-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A stable, fast and convenient async client for poe.com
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
+Requires-Dist: js2py (>=0.74,<0.75)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # User Guide
 
 [中文版本](README_zh_CN.md)
 
@@ -64,17 +65,17 @@
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
 a `Poe_Client` object. You need to pass the `p_b token` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
 from async_poe_client import Poe_Client
 
-poe_client = await Poe_Client("your p_b token").create()
+poe_client = await Poe_Client("your p_b token", "your formkey").create()
 # or with a proxy
-poe_client = await Poe_Client("your p_b token",proxy="socks5://127.0.0.1:7890").create()
+poe_client = await Poe_Client("your p_b token", "your formkey", proxy="socks5://127.0.0.1:7890").create()
 ```
 
 Here, `"your p_b token"` should be replaced with your actual p_b token.
 
 ## Step 2: Use Poe_Client
 
 After creating the `Poe_Client`, you can use it to perform a lot of operations.
```

