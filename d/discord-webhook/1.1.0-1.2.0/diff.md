# Comparing `tmp/discord-webhook-1.1.0.tar.gz` & `tmp/discord-webhook-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-webhook-1.1.0.tar", max compression
+gzip compressed data, was "discord-webhook-1.2.0.tar", max compression
```

## Comparing `discord-webhook-1.1.0.tar` & `discord-webhook-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      172 2022-11-13 20:16:03.212707 discord-webhook-1.1.0/discord_webhook/__init__.py
--rw-r--r--   0        0        0     1027 2022-11-15 13:38:51.626949 discord-webhook-1.1.0/discord_webhook/__main__.py
--rw-r--r--   0        0        0     6765 2023-02-15 18:07:55.326537 discord-webhook-1.1.0/discord_webhook/async_webhook.py
--rw-r--r--   0        0        0        0 2022-11-13 20:16:03.212707 discord-webhook-1.1.0/discord_webhook/py.typed
--rw-r--r--   0        0        0    19578 2023-02-15 18:11:14.736962 discord-webhook-1.1.0/discord_webhook/webhook.py
--rw-r--r--   0        0        0      657 2022-11-13 20:16:03.213707 discord-webhook-1.1.0/discord_webhook/webhook_exceptions.py
--rw-r--r--   0        0        0     1093 2022-11-13 20:16:03.211707 discord-webhook-1.1.0/LICENSE
--rw-r--r--   0        0        0     1204 2023-02-15 18:11:21.138057 discord-webhook-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11939 2023-02-15 18:07:55.351592 discord-webhook-1.1.0/README.md
--rw-r--r--   0        0        0    13042 1970-01-01 00:00:00.000000 discord-webhook-1.1.0/setup.py
--rw-r--r--   0        0        0    12334 1970-01-01 00:00:00.000000 discord-webhook-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-24 19:51:39.962891 discord-webhook-1.2.0/discord_webhook/__init__.py
+-rw-r--r--   0        0        0     1027 2023-05-24 20:56:22.801847 discord-webhook-1.2.0/discord_webhook/__main__.py
+-rw-r--r--   0        0        0     7127 2023-07-20 21:31:33.181731 discord-webhook-1.2.0/discord_webhook/async_webhook.py
+-rw-r--r--   0        0        0        0 2022-11-13 20:16:03.212707 discord-webhook-1.2.0/discord_webhook/py.typed
+-rw-r--r--   0        0        0    19367 2023-07-24 19:51:39.963894 discord-webhook-1.2.0/discord_webhook/webhook.py
+-rw-r--r--   0        0        0      626 2023-07-24 19:51:39.964891 discord-webhook-1.2.0/discord_webhook/webhook_exceptions.py
+-rw-r--r--   0        0        0     1093 2022-11-13 20:16:03.211707 discord-webhook-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1160 2023-07-24 19:56:07.714452 discord-webhook-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12311 2023-07-11 19:35:36.873610 discord-webhook-1.2.0/README.md
+-rw-r--r--   0        0        0    13248 1970-01-01 00:00:00.000000 discord-webhook-1.2.0/setup.py
+-rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 discord-webhook-1.2.0/PKG-INFO
```

### Comparing `discord-webhook-1.1.0/discord_webhook/__main__.py` & `discord-webhook-1.2.0/discord_webhook/__main__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Entry point to trigger webhook(s). """
-import sys
 import argparse
+import sys
 
 from discord_webhook import DiscordWebhook
 
 
 def main() -> bool:
     parser = argparse.ArgumentParser(
         prog="discord_webhook", description="Trigger discord webhook(s)."
```

### Comparing `discord-webhook-1.1.0/discord_webhook/async_webhook.py` & `discord-webhook-1.2.0/discord_webhook/async_webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,73 +30,77 @@
             raise ImportError(
                 "You're attempting to use the async version of discord-webhooks but"
                 " didn't install it using `pip install discord-webhook[async]`."
             ) from None
 
     @property
     @asynccontextmanager
-    async def http_client(self):
+    async def http_client(self) -> "httpx.AsyncClient":
         """
         A property that returns a httpx.AsyncClient instance that is used for a 'with' statement.
         Example:
             async with self.http_client as client:
                 client.post(url, data=data)
         It will automatically close the client when the context is exited.
         :return: httpx.AsyncClient
         """
         client = httpx.AsyncClient(proxies=self.proxies)
         yield client
         await client.aclose()
 
-    async def api_post_request(self):
+    async def api_post_request(self) -> "httpx.Response":
+        """
+        Post the JSON converted webhook data to the specified url.
+        :return:
+        """
         async with self.http_client as client:  # type: httpx.AsyncClient
             if bool(self.files) is False:
                 response = await client.post(
                     self.url,
                     json=self.json,
-                    params={'wait': True},
+                    params={"wait": True},
                     timeout=self.timeout,
                 )
             else:
                 self.files["payload_json"] = (
                     None,
-                    json.dumps(self.json).encode('utf-8'),
+                    json.dumps(self.json).encode("utf-8"),
                 )
                 response = await client.post(
                     self.url, files=self.files, timeout=self.timeout
                 )
         return response
 
-    async def handle_rate_limit(self, response, request):
+    async def handle_rate_limit(self, response, request) -> "httpx.Response":
         """
-        Handle the rate limit.
+        Handle the rate limit by resending the webhook until a successful response.
         :param response: Response
         :param request: request function
-        :return: Response
+        :return: Response of the sent webhook
         """
         while response.status_code == 429:
             errors = response.json()
-            if not response.headers.get('Via'):
+            if not response.headers.get("Via"):
                 raise HTTPException(errors)
-            wh_sleep = (int(errors['retry_after']) / 1000) + 0.15
+            wh_sleep = float(errors["retry_after"]) + 0.15
             logger.error(
                 "Webhook rate limited: sleeping for {wh_sleep} seconds...".format(
-                    wh_sleep=wh_sleep
+                    wh_sleep=round(wh_sleep, 2)
                 )
             )
             await asyncio.sleep(wh_sleep)
             response = await request()
             if response.status_code in [200, 204]:
                 return response
 
-    async def execute(self, remove_embeds=False):
+    async def execute(self, remove_embeds=False) -> "httpx.Response":
         """
-        executes the Webhook
-        :param remove_embeds: if set to True, calls `self.remove_embeds()` to empty `self.embeds` after webhook is executed
-        :return: Webhook response
+        Execute the sending of the webhook with the given data.
+        :param bool remove_embeds: clear the stored embeds after webhook is executed
+        :return: Response of the sent webhook
         """
         response = await self.api_post_request()
         if response.status_code in [200, 204]:
             logger.debug("Webhook executed")
         elif response.status_code == 429 and self.rate_limit_retry:
             response = await self.handle_rate_limit(response, self.api_post_request)
         else:
@@ -105,40 +109,40 @@
                     status_code=response.status_code,
                     content=response.content.decode("utf-8"),
                 )
             )
         if remove_embeds:
             self.remove_embeds()
         self.remove_files(clear_attachments=False)
-        if webhook_id := json.loads(response.content.decode("utf-8")).get('id'):
+        if webhook_id := json.loads(response.content.decode("utf-8")).get("id"):
             self.id = webhook_id
         return response
 
-    async def edit(self):
+    async def edit(self) -> "httpx.Response":
         """
-        Edit the given webhook.
-        :return: webhook response
+        Edit an already sent webhook with updated data.
+        :return: Response of the sent webhook
         """
         assert isinstance(
             self.id, str
         ), "Webhook ID needs to be set in order to edit the webhook."
         assert isinstance(
             self.url, str
         ), "Webhook URL needs to be set in order to edit the webhook."
         async with self.http_client as client:  # type: httpx.AsyncClient
             url = f"{self.url}/messages/{self.id}"
             if bool(self.files) is False:
                 patch_kwargs = {
-                    'json': self.json,
-                    'params': {'wait': True},
-                    'timeout': self.timeout,
+                    "json": self.json,
+                    "params": {"wait": True},
+                    "timeout": self.timeout,
                 }
             else:
                 self.files["payload_json"] = (None, json.dumps(self.json))
-                patch_kwargs = {'files': self.files, 'timeout': self.timeout}
+                patch_kwargs = {"files": self.files, "timeout": self.timeout}
             request = partial(client.patch, url, **patch_kwargs)
             response = await request()
             if response.status_code in [200, 204]:
                 logger.debug("Webhook with id {id} edited".format(id=self.id))
             elif response.status_code == 429 and self.rate_limit_retry:
                 response = await self.handle_rate_limit(response, request)
                 logger.debug("Webhook edited")
@@ -147,17 +151,17 @@
                     "Webhook status code {status_code}: {content}".format(
                         status_code=response.status_code,
                         content=response.content.decode("utf-8"),
                     )
                 )
             return response
 
-    async def delete(self):
+    async def delete(self) -> "httpx.Response":
         """
-        Delete the given webhook.
+        Delete the already sent webhook.
         :return: webhook response
         """
         assert isinstance(
             self.id, str
         ), "Webhook ID needs to be set in order to delete the webhook."
         assert isinstance(
             self.url, str
```

### Comparing `discord-webhook-1.1.0/discord_webhook/webhook.py` & `discord-webhook-1.2.0/discord_webhook/webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,188 +1,186 @@
-import datetime
 import json
 import logging
 import time
+from datetime import datetime
 from functools import partial
 from http.client import HTTPException
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
-
+from typing import Any, Dict, List, Optional, Tuple, Union
 import requests
 
 from .webhook_exceptions import ColorNotInRangeException
 
 logger = logging.getLogger(__name__)
 
 
 class DiscordEmbed:
     """
     Discord Embed
     """
 
-    title: Optional[str]
-    description: Optional[str]
-    url: Optional[str]
-    timestamp: Optional[str]
+    author: Optional[Dict[str, Optional[str]]]
     color: Optional[int]
+    description: Optional[str]
+    fields: List[Dict[str, Optional[Any]]]
     footer: Optional[Dict[str, Optional[str]]]
     image: Optional[Dict[str, Optional[Union[str, int]]]]
-    thumbnail: Optional[Union[str, Dict[str, Optional[Union[str, int]]]]]
-    video: Optional[Union[str, Dict[str, Optional[Union[str, int]]]]]
     provider: Optional[Dict[str, Any]]
-    author: Optional[Dict[str, Optional[str]]]
-    fields: List[Dict[str, Optional[Any]]]
+    thumbnail: Optional[Dict[str, Optional[Union[str, int]]]]
+    timestamp: Optional[str]
+    title: Optional[str]
+    url: Optional[str]
+    video: Optional[Dict[str, Optional[Union[str, int]]]]
 
     def __init__(
         self,
         title: Optional[str] = None,
         description: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """
         Init Discord Embed
         -----------
-        :keyword ``title:`` title of embed\n
-        :keyword ``description:`` description body of embed\n
-        :keyword ``url:`` add an url to make your embedded title a clickable
-        link\n
-        :keyword ``timestamp:`` timestamp of embed content\n
-        :keyword ``color:`` color code of the embed as int\n
-        :keyword ``footer:`` footer texts\n
-        :keyword ``image:`` your image url here\n
-        :keyword ``thumbnail:`` your thumbnail url here\n
-        :keyword ``video:``  to apply video with embedded, your video source
-        url here\n
-        :keyword ``provider:`` provider information\n
-        :keyword ``author:`` author information\n
-        :keyword ``fields:`` fields information
+        :keyword dict author: information about the author
+        :keyword color: color code of the embed as decimal or hexadecimal
+        :keyword str description: description of the embed
+        :keyword list fields: embed fields as a list of dicts with name and value
+        :keyword dict footer: information that will be displayed in the footer
+        :keyword dict image: image that will be displayed in the embed
+        :keyword dict provider: information about the provider
+        :keyword dict thumbnail: thumbnail that will be displayed in the embed
+        :keyword str timestamp: timestamp that will be displayed in the embed
+        :keyword str title: title of embed
+        :keyword str url: add an url to make your embedded title a clickable link
+        :keyword dict video: video that will be displayed in the embed
         """
         self.title = title
         self.description = description
-        self.url = cast(str, kwargs.get("url"))
-        self.timestamp = cast(str, kwargs.get("timestamp"))
+        self.url = kwargs.get("url")
         self.footer = kwargs.get("footer")
         self.image = kwargs.get("image")
         self.thumbnail = kwargs.get("thumbnail")
         self.video = kwargs.get("video")
         self.provider = kwargs.get("provider")
         self.author = kwargs.get("author")
         self.fields = kwargs.get("fields", [])
         self.set_color(kwargs.get("color"))
+        if timestamp := kwargs.get("timestamp"):
+            self.set_timestamp(timestamp)
 
     def set_title(self, title: str) -> None:
         """
-        set title of embed
-        :param title: title of embed
+        Set the title of the embed.
+        :param str title: title of embed
         """
         self.title = title
 
     def set_description(self, description: str) -> None:
         """
-        set description of embed
-        :param description: description of embed
+        Set the description of the embed.
+        :param str description: description of embed
         """
         self.description = description
 
     def set_url(self, url: str) -> None:
         """
-        set url of embed
-        :param url: url of embed
+        Set the url of the embed.
+        :param str url: url of embed
         """
         self.url = url
 
-    def set_timestamp(self, timestamp: Optional[float] = None) -> None:
+    def set_timestamp(
+        self, timestamp: Optional[Union[float, int, datetime]] = None
+    ) -> None:
         """
-        set timestamp of embed content
-        :param timestamp: (optional) timestamp of embed content
+        Set timestamp of the embed content.
+        :param timestamp: timestamp of embed content
         """
         if timestamp is None:
-            timestamp = time.time()
-        self.timestamp = str(datetime.datetime.utcfromtimestamp(timestamp))
+            timestamp = datetime.utcnow()
+        elif isinstance(timestamp, float) or isinstance(timestamp, int):
+            timestamp = datetime.utcfromtimestamp(timestamp)
+
+        self.timestamp = timestamp.isoformat()
 
     def set_color(self, color: Union[str, int]) -> None:
         """
-        set color code of the embed as decimal(int) or hex(string)
-        :param color: color code of the embed as decimal(int) or hex(string)
+        Set the color of the embed.
+        :param color: color code as decimal(int) or hex(string)
         """
         self.color = int(color, 16) if isinstance(color, str) else color
         if self.color is not None and self.color not in range(16777216):
             raise ColorNotInRangeException(color)
 
-    def set_footer(self, **kwargs: str) -> None:
+    def set_footer(self, text: str, **kwargs) -> None:
         """
-        set footer information of embed
-        :keyword text: footer text
-        :keyword icon_url: url of footer icon (only supports http(s) and
-        attachments)
-        :keyword proxy_icon_url: a proxied url of footer icon
+        Set footer information in the embed.
+        :param str text: footer text
+        :keyword str icon_url: url of footer icon (only http(s) and attachments)
+        :keyword str proxy_icon_url: proxied url of footer icon
         """
         self.footer = {
-            "text": kwargs.get("text"),
+            "text": text,
             "icon_url": kwargs.get("icon_url"),
             "proxy_icon_url": kwargs.get("proxy_icon_url"),
         }
 
     def set_image(self, url: str, **kwargs: Union[str, int]) -> None:
         """
-        set image of embed
-        :param url: source url of image (only supports http(s) and attachments)
-        :keyword proxy_url: a proxied url of the image
-        :keyword height: height of image
-        :keyword width: width of image
+        Set the image that will be displayed in the embed.
+        :param str url: source url of image (only supports http(s) and attachments)
+        :keyword str proxy_url: a proxied url of the image
+        :keyword int height: height of image
+        :keyword int width: width of image
         """
         self.image = {
             "url": url,
-            "proxy_url": cast(Optional[str], kwargs.get("proxy_url")),
-            "height": cast(Optional[int], kwargs.get("height")),
-            "width": cast(Optional[int], kwargs.get("width")),
+            "proxy_url": kwargs.get("proxy_url"),
+            "height": kwargs.get("height"),
+            "width": kwargs.get("width"),
         }
 
     def set_thumbnail(self, url: str, **kwargs: Union[str, int]) -> None:
         """
-        set thumbnail of embed
-        :param url: source url of thumbnail (only supports http(s) and
-        attachments)
-        :keyword proxy_url: a proxied thumbnail of the image
-        :keyword height: height of thumbnail
-        :keyword width: width of thumbnail
+        Set the thumbnail that will be displayed in the embed.
+        :param str url: source url of thumbnail (only supports http(s) and attachments)
+        :keyword str proxy_url: a proxied thumbnail of the image
+        :keyword int height: height of thumbnail
+        :keyword int width: width of thumbnail
         """
         self.thumbnail = {
             "url": url,
-            "proxy_url": cast(Optional[str], kwargs.get("proxy_url")),
-            "height": cast(Optional[int], kwargs.get("height")),
-            "width": cast(Optional[str], kwargs.get("width")),
+            "proxy_url": kwargs.get("proxy_url"),
+            "height": kwargs.get("height"),
+            "width": kwargs.get("width"),
         }
 
     def set_video(self, **kwargs: Union[str, int]) -> None:
         """
-        set video of embed
-        :keyword url: source url of video
-        :keyword height: height of video
-        :keyword width: width of video
+        Set the video that will be displayed in the embed.
+        :keyword str url: source url of video
+        :keyword int height: height of video
+        :keyword int width: width of video
         """
         self.video = {
-            "url": cast(Optional[str], kwargs.get("url")),
-            "height": cast(Optional[int], kwargs.get("height")),
-            "width": cast(Optional[int], kwargs.get("width")),
+            "url": kwargs.get("url"),
+            "height": kwargs.get("height"),
+            "width": kwargs.get("width"),
         }
 
     def set_provider(self, **kwargs: str) -> None:
         """
-        set provider of embed
-        :keyword name: name of provider
-        :keyword url: url of provider
+        Set the provider information of the embed.
+        :keyword str name: name of provider
+        :keyword str url: url of provider
         """
-        self.provider = {
-            "name": kwargs.get("name"),
-            "url": kwargs.get("url"),
-        }
+        self.provider = {"name": kwargs.get("name"), "url": kwargs.get("url")}
 
     def set_author(self, name: str, **kwargs: str) -> None:
         """
-        set author of embed
+        Set information about the author of the embed.
         :param name: name of author
         :keyword url: url of author
         :keyword icon_url: url of author icon (only supports http(s) and
         attachments)
         :keyword proxy_icon_url: a proxied url of author icon
         """
         self.author = {
@@ -190,231 +188,196 @@
             "url": kwargs.get("url"),
             "icon_url": kwargs.get("icon_url"),
             "proxy_icon_url": kwargs.get("proxy_icon_url"),
         }
 
     def add_embed_field(self, name: str, value: str, inline: bool = True) -> None:
         """
-        set field of embed
-        :param name: name of the field
-        :param value: value of the field
-        :param inline: (optional) whether this field should display inline
-        """
-        self.fields.append(
-            {
-                "name": name,
-                "value": value,
-                "inline": inline,
-            }
-        )
+        Set a field with information for the embed
+        :param str name: name of the field
+        :param str value: value of the field
+        :param bool inline: (optional) whether this field should display inline
+        """
+        self.fields.append({"name": name, "value": value, "inline": inline})
 
     def delete_embed_field(self, index: int) -> None:
         """
-        remove field from `self.fields`
-        :param index: index of field in `self.fields`
+        Remove a field from the already stored embed fields.
+        :param int index: index of field in `self.fields`
         """
         self.fields.pop(index)
 
     def get_embed_fields(self) -> List[Dict[str, Optional[Any]]]:
         """
-        get all `self.fields` as list
-        :return: `self.fields`
+        Get all stored fields of the embed as a list.
+        :return: fields of the embed
         """
         return self.fields
 
 
 class DiscordWebhook:
     """
     Webhook for Discord
     """
 
-    url: str
-    id: Optional[str]
-    content: Optional[Union[str, bytes]]
-    username: Optional[str]
-    avatar_url: Optional[str]
-    tts: bool
+    allowed_mentions: List[str]
     attachments: Optional[List[Dict[str, Any]]]
-    files: Dict[str, Tuple[Optional[str], Union[bytes, str]]]
+    avatar_url: Optional[str]
+    components: Optional[list]
+    content: Optional[Union[str, bytes]]
     embeds: List[Dict[str, Any]]
+    files: Dict[str, Tuple[Optional[str], Union[bytes, str]]]
+    id: Optional[str]
     proxies: Optional[Dict[str, str]]
-    allowed_mentions: List[str]
-    timeout: Optional[float]
     rate_limit_retry: bool = False
+    timeout: Optional[float]
+    tts: bool
+    url: str
+    username: Optional[str]
 
-    def __init__(
-        self,
-        url: str,
-        *,
-        id: Optional[str] = None,
-        content: Optional[str] = None,
-        username: Optional[str] = None,
-        avatar_url: Optional[str] = None,
-        tts: bool = False,
-        attachments: Optional[List[Dict[str, Any]]] = None,
-        files: Optional[Dict[str, Tuple[Optional[str], Union[bytes, str]]]] = None,
-        embeds: Optional[List[Dict[str, Any]]] = None,
-        proxies: Optional[Dict[str, str]] = None,
-        timeout: Optional[float] = None,
-        rate_limit_retry: bool = False,
-        allowed_mentions: Optional[List[str]] = None,
-    ) -> None:
+    def __init__(self, url: str, **kwargs) -> None:
         """
         Init Webhook for Discord.
         ---------
-        :param ``url``: your discord webhook url (type: str)\n
-        :keyword ``id:`` webhook id (type: str)\n
-        :keyword ``content:`` the message contents (type: str)\n
-        :keyword ``username:`` override the default username of the webhook\n
-        :keyword ``avatar_url:`` override the default avatar of the webhook\n
-        :keyword ``tts:`` true if this is a TTS message\n
-        :keyword ``attachments`` optional dict of attachments.
-        Will be set after executing a webhook\n
-        :keyword ``files``: to apply file(s) with message
-        (For example: file=f.read() (here, f = variable that contains the
-        attachment path as "rb" mode))\n
-        :keyword ``embeds:`` list of embedded rich content\n
-        :keyword ``allowed_mentions:`` allowed mentions for the message\n
-        :keyword ``proxies:`` dict of proxies\n
-        :keyword ``timeout:`` (optional) amount of seconds to wait for a
-        response from Discord
-        """
-        if embeds is None:
-            embeds = []
-        if files is None:
-            files = {}
-        if allowed_mentions is None:
-            allowed_mentions = []
-        if attachments is None:
-            attachments = []
+        :param str url: your discord webhook url
+        :keyword list allowed_mentions: allowed mentions for the message
+        :keyword dict attachments: attachments that should be included
+        :keyword str avatar_url: override the default avatar of the webhook
+        :keyword str content: the message contents
+        :keyword list embeds: list of embedded rich content
+        :keyword dict files: to apply file(s) with message
+        :keyword str id: webhook id
+        :keyword dict proxies: proxies that should be used
+        :keyword bool rate_limit_retry: whether the message should be sent again when being rate limited
+        :keyword int timeout: seconds to wait for a response from Discord
+        :keyword bool tts: indicates if this is a TTS message
+        :keyword str username: override the default username of the webhook
+        """
+        self.allowed_mentions = kwargs.get("allowed_mentions", [])
+        self.attachments = kwargs.get("attachments", [])
+        self.avatar_url = kwargs.get("avatar_url")
+        self.content = kwargs.get("content")
+        self.embeds = kwargs.get("embeds", [])
+        self.files = kwargs.get("files", {})
+        self.id = kwargs.get("id")
+        self.proxies = kwargs.get("proxies")
+        self.rate_limit_retry = kwargs.get("rate_limit_retry", False)
+        self.timeout = kwargs.get("timeout")
+        self.tts = kwargs.get("timeout", False)
         self.url = url
-        self.id = id
-        self.content = content
-        self.username = username
-        self.avatar_url = avatar_url
-        self.tts = tts
-        self.attachments = attachments
-        self.files = files
-        self.embeds = embeds
-        self.proxies = proxies
-        self.allowed_mentions = allowed_mentions
-        self.timeout = timeout
-        self.rate_limit_retry = rate_limit_retry
-
-    def add_file(self, file: bytes, filename: str) -> None:
-        """
-        Add a file to the webhook.
-        :param file: file content
-        :param filename: filename
-        :return:
-        """
-        self.files[f"_{filename}"] = (filename, file)
+        self.username = kwargs.get("username", False)
 
     def add_embed(self, embed: Union[DiscordEmbed, Dict[str, Any]]) -> None:
         """
         Add an embedded rich content.
         :param embed: embed object or dict
         """
         self.embeds.append(embed.__dict__ if isinstance(embed, DiscordEmbed) else embed)
 
+    def get_embeds(self) -> List[Dict[str, Any]]:
+        """
+        Get all embeds as a list.
+        :return: embeds
+        """
+        return self.embeds
+
     def remove_embed(self, index: int) -> None:
         """
-        Remove embedded rich content from `self.embeds`.
-        :param index: index of embed in `self.embeds`
+        Remove an embed from already added embeds to the webhook.
+        :param int index: index of embed
         """
         self.embeds.pop(index)
 
+    def remove_embeds(self) -> None:
+        """
+        Remove all embeds.
+        """
+        self.embeds = []
+
+    def add_file(self, file: bytes, filename: str) -> None:
+        """
+        Add a file to the webhook.
+        :param bytes file: file content
+        :param str filename: filename
+        """
+        self.files[f"_{filename}"] = (filename, file)
+
     def remove_file(self, filename: str) -> None:
         """
-        Remove file by given `filename` if it exists.
-        :param filename: filename
+        Remove the file by the given filename if it exists.
+        :param str filename: filename
         """
-        self.files.pop(f'_{filename}', None)
+        self.files.pop(f"_{filename}", None)
         if self.attachments:
             index = next(
                 (
                     i
                     for i, item in enumerate(self.attachments)
-                    if item.get('filename') == filename
+                    if item.get("filename") == filename
                 ),
                 None,
             )
             if index is not None:
                 self.attachments.pop(index)
 
-    def remove_embeds(self) -> None:
-        """
-        Remove all embeds.
-        :return: None
-        """
-        self.embeds = []
-
     def remove_files(self, clear_attachments: bool = True) -> None:
         """
         Remove all files and optionally clear the attachments.
-        :keyword clear_attachments: Clear the attachments.
-        :type clear_attachments: bool
-        :return: None
+        :param bool clear_attachments: Clear the attachments
         """
         self.files = {}
         if clear_attachments:
             self.clear_attachments()
 
     def clear_attachments(self) -> None:
         """
         Remove all attachments.
-        :return: None
         """
         self.attachments = []
 
-    def get_embeds(self) -> List[Dict[str, Any]]:
-        """
-        Get all embeds as a list.
-        :return: self.embeds
-        """
-        return self.embeds
-
     def set_proxies(self, proxies: Dict[str, str]) -> None:
         """
-        Set proxies.
-        :param proxies: dict of proxies
-        :type proxies: dict
+        Set proxies that should be used when sending the webhook.
+        :param dict proxies: dict of proxies
         """
         self.proxies = proxies
 
     def set_content(self, content: str) -> None:
         """
-        Set content.
-        :param content: content string
-        :type content: string
+        Set the content of the webhook.
+        :param str content: content of the webhook
         """
         self.content = content
 
     @property
     def json(self) -> Dict[str, Any]:
         """
-        Convert webhook data to json.
-        :return webhook data as json:
+        Convert data of the webhook to JSON.
+        :return: webhook data as json
         """
         embeds = self.embeds
         self.embeds = []
         # convert DiscordEmbed to dict
         for embed in embeds:
             self.add_embed(embed)
         data = {
             key: value
             for key, value in self.__dict__.items()
-            if value and key not in ['url', 'files'] or key in ['embeds', 'attachments']
+            if value and key not in ["url", "files"] or key in ["embeds", "attachments"]
         }
         embeds_empty = not any(data["embeds"]) if "embeds" in data else True
         if embeds_empty and "content" not in data and bool(self.files) is False:
             logger.error("webhook message is empty! set content or embed data")
         return data
 
-    def api_post_request(self) -> requests.post:
+    def api_post_request(self) -> "requests.Response":
+        """
+        Post the JSON converted webhook data to the specified url.
+        :return: Response of the sent webhook
+        """
         if bool(self.files) is False:
             return requests.post(
                 self.url,
                 json=self.json,
                 proxies=self.proxies,
                 params={"wait": True},
                 timeout=self.timeout,
@@ -426,67 +389,65 @@
             files=self.files,
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
     def handle_rate_limit(self, response, request):
         """
-        Handle the rate limit.
+        Handle the rate limit by resending the webhook until a successful response.
         :param response: Response
         :param request: request function
-        :return: Response
+        :return: Response of the sent webhook
         """
         while response.status_code == 429:
             errors = json.loads(response.content.decode("utf-8"))
-            if not response.headers.get('Via'):
+            if not response.headers.get("Via"):
                 raise HTTPException(errors)
-            wh_sleep = (int(errors["retry_after"]) / 1000) + 0.15
-            logger.error(f"Webhook rate limited: sleeping for {wh_sleep} seconds...")
+            wh_sleep = float(errors["retry_after"]) + 0.15
+            logger.error(
+                f"Webhook rate limited: sleeping for {wh_sleep:.2f} seconds..."
+            )
             time.sleep(wh_sleep)
             response = request()
             if response.status_code in [200, 204]:
                 return response
 
-    def execute(
-        self,
-        remove_embeds: bool = False,
-    ) -> requests.Response:
+    def execute(self, remove_embeds: bool = False) -> "requests.Response":
         """
-        Execute the Webhook.
-        :param remove_embeds: if set to True, calls `self.remove_embeds()`
-        to empty `self.embeds` after webhook is executed
-        :return: Webhook response
+        Execute the sending of the webhook with the given data.
+        :param bool remove_embeds: clear the stored embeds after webhook is executed
+        :return: Response of the sent webhook
         """
         response = self.api_post_request()
         if response.status_code in [200, 204]:
             logger.debug("Webhook executed")
         elif response.status_code == 429 and self.rate_limit_retry:
             response = self.handle_rate_limit(response, self.api_post_request)
             logger.debug("Webhook executed")
         else:
             logger.error(
                 "Webhook status code {status_code}: {content}".format(
                     status_code=response.status_code,
-                    content=response.content.decode('utf-8'),
+                    content=response.content.decode("utf-8"),
                 )
             )
         if remove_embeds:
             self.remove_embeds()
         self.remove_files(clear_attachments=False)
         response_content = json.loads(response.content.decode("utf-8"))
-        if webhook_id := response_content.get('id'):
+        if webhook_id := response_content.get("id"):
             self.id = webhook_id
-        if attachments := response_content.get('attachments'):
+        if attachments := response_content.get("attachments"):
             self.attachments = attachments
         return response
 
-    def edit(self) -> requests.Response:
+    def edit(self) -> "requests.Response":
         """
-        Edit the given webhook.
-        :return: webhook response
+        Edit an already sent webhook with updated data.
+        :return: Response of the sent webhook
         """
         assert isinstance(
             self.id, str
         ), "Webhook ID needs to be set in order to edit the webhook."
         assert isinstance(
             self.url, str
         ), "Webhook URL needs to be set in order to edit the webhook."
@@ -520,17 +481,17 @@
                 "Webhook status code {status_code}: {content}".format(
                     status_code=response.status_code,
                     content=response.content.decode("utf-8"),
                 )
             )
         return response
 
-    def delete(self) -> requests.Response:
+    def delete(self) -> "requests.Response":
         """
-        Delete the given webhook.
+        Delete the already sent webhook.
         :return: webhook response
         """
         assert isinstance(
             self.id, str
         ), "Webhook ID needs to be set in order to delete the webhook."
         assert isinstance(
             self.url, str
@@ -544,16 +505,17 @@
             logger.debug("Webhook deleted")
         elif response.status_code == 429 and self.rate_limit_retry:
             response = self.handle_rate_limit(response, request)
             logger.debug("Webhook edited")
         return response
 
     @classmethod
-    def create_batch(cls, urls: List[str], **kwargs) -> Tuple['DiscordWebhook', ...]:
+    def create_batch(cls, urls: List[str], **kwargs) -> Tuple["DiscordWebhook", ...]:
         """
-        Create multiple instances of webhook.
-        :param urls: list of webhook URLs.
+        Create a webhook instance for each specified URL.
+        :param list urls: webhook URLs to be used for the instances
+        :param kwargs: the same kwargs that are used for an instance of the class
         :return: tuple of webhook instances
         """
-        if 'url' in kwargs:
+        if "url" in kwargs:
             raise TypeError("'url' can't be used as a keyword argument.")
         return tuple([cls(url, **kwargs) for url in urls])
```

### Comparing `discord-webhook-1.1.0/LICENSE` & `discord-webhook-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.1.0/pyproject.toml` & `discord-webhook-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "discord-webhook"
-version = "1.1.0"
-description = "execute discord webhooks"
+version = "1.2.0"
+description = "Easily send Discord webhooks with Python"
 authors = ["lovvskillz <14542790+lovvskillz@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "discord_webhook"}]
 repository = "https://github.com/lovvskillz/python-discord-webhook"
 keywords = ["discord", "webhook"]
 
@@ -15,28 +15,26 @@
 requests = "^2.28.1"
 httpx = { version = "^0.23.0", optional = true }
 
 [tool.poetry.extras]
 async = ["httpx"]
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-pre-commit = "^2.20.0"
-pylint = "^2.15.5"
-flake8 = "^5.0.4"
+black = "^23.7.0"
+pre-commit = "^3.3.3"
 types-requests = "^2.28.11.4"
-pytest = "^7.2.0"
+pytest = "^7.4.0"
+ruff = "^0.0.278"
 
 [tool.poetry.scripts]
 discord_webhook = "discord_webhook.__main__:main"
 
 [tool.black]
 line-length = 88
-skip-string-normalization=true
-experimental-string-processing = true
+preview = true
 target-version = ["py310"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.mypy_cache
@@ -46,13 +44,14 @@
   | buck-out
   | build
   | dist
   | frontend
 )/
 '''
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+line-length = 88
+ignore = ["E501"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `discord-webhook-1.1.0/README.md` & `discord-webhook-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,400 +1,432 @@
-# python-discord-webhook
-
-[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/lovvskillz/python-discord-webhook/master/LICENSE)
-[![PyPI version](https://badge.fury.io/py/discord-webhook.svg)](https://badge.fury.io/py/discord-webhook)
-[![Downloads](https://pepy.tech/badge/discord-webhook)](https://pepy.tech/project/discord-webhook)
-
-Execute Discord Webhooks (also has [async support](#async-support))
-
-## Install
-
-Install via pip:
-```
-pip install discord-webhook
-```
-
-## Examples
-
-* [Basic Webhook](#basic-webhook)
-* [Create Multiple Instances / Use multiple URLs](#create-multiple-instances)
-* [Manage Being Rate Limited](#manage-being-rate-limited)
-* [Embedded Content](#webhook-with-embedded-content)
-* [Edit Webhook Message](#edit-webhook-messages)
-* [Delete Webhook Message](#delete-webhook-messages)
-* [Send Files](#send-files)
-* [Remove Embeds and Files](#remove-embeds-and-files)
-* [Allowed Mentions](#allowed-mentions)
-* [Use Proxies](#use-proxies)
-* [Timeout](#timeout)
-* [Async Support](#async-support)
-
-### Basic Webhook
-
-```python
-from discord_webhook import DiscordWebhook
-
-webhook = DiscordWebhook(url='your webhook url', content='Webhook Message')
-response = webhook.execute()
-```
-
-### Create multiple instances
-If you want to use multiple URLs you need to create multiple instances.
-
-```python
-from discord_webhook import DiscordWebhook
-
-# you can provide any kwargs except url
-webhook1, webhook2 = DiscordWebhook.create_batch(urls=['first url', 'second url'], content='Webhook Message')
-response1 = webhook1.execute()
-response2 = webhook2.execute()
-```
-![Image](img/multiple_urls.png "Multiple Urls Result")
-
-### Manage being Rate Limited
-
-```python
-from discord_webhook import DiscordWebhook
-
-# if rate_limit_retry is True then in the event that you are being rate 
-# limited by Discord your webhook will automatically be sent once the 
-# rate limit has been lifted
-webhook = DiscordWebhook(url='your webhook url', rate_limit_retry=True,
-                         content='Webhook Message')
-response = webhook.execute()
-```
-
-![Image](img/basic_webhook.png "Basic Example Result")
-
-### Webhook with Embedded Content
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url='your webhook url')
-
-# create embed object for webhook
-# you can set the color as a decimal (color=242424) or hex (color='03b2f8') number
-embed = DiscordEmbed(title='Your Title', description='Lorem ipsum dolor sit', color='03b2f8')
-
-# add embed object to webhook
-webhook.add_embed(embed)
-
-response = webhook.execute()
-```
-
-![Image](img/simple_embed.png "Basic Embed Example Result")
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url='your webhook url')
-
-# create embed object for webhook
-embed = DiscordEmbed(title='Your Title', description='Lorem ipsum dolor sit', color='03b2f8')
-
-# set author
-embed.set_author(name='Author Name', url='author url', icon_url='author icon url')
-
-# set image
-embed.set_image(url='your image url')
-
-# set thumbnail
-embed.set_thumbnail(url='your thumbnail url')
-
-# set footer
-embed.set_footer(text='Embed Footer Text', icon_url='URL of icon')
-
-# set timestamp (default is now)
-embed.set_timestamp()
-
-# add fields to embed
-embed.add_embed_field(name='Field 1', value='Lorem ipsum')
-embed.add_embed_field(name='Field 2', value='dolor sit')
-
-# add embed object to webhook
-webhook.add_embed(embed)
-
-response = webhook.execute()
-```
-
-![Image](img/extended_embed.png "Basic Embed Example Result")
-
-This is another example with embedded content
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url='your webhook url', username="New Webhook Username")
-
-embed = DiscordEmbed(title='Embed Title', description='Your Embed Description', color='03b2f8')
-embed.set_author(name='Author Name', url='https://github.com/lovvskillz', icon_url='https://avatars0.githubusercontent.com/u/14542790')
-embed.set_footer(text='Embed Footer Text')
-embed.set_timestamp()
-embed.add_embed_field(name='Field 1', value='Lorem ipsum')
-embed.add_embed_field(name='Field 2', value='dolor sit')
-embed.add_embed_field(name='Field 3', value='amet consetetur')
-embed.add_embed_field(name='Field 4', value='sadipscing elitr')
-
-webhook.add_embed(embed)
-response = webhook.execute()
-```
-
-![Image](img/extended_embed2.png "Example Embed Result")
-
-By Default, the Embed fields are placed side by side. We can arrange them in a new line by setting `inline=False` as follows:
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")
-
-embed = DiscordEmbed(
-    title="Embed Title", description="Your Embed Description", color='03b2f8'
-)
-embed.set_author(
-    name="Author Name",
-    url="https://github.com/lovvskillz",
-    icon_url="https://avatars0.githubusercontent.com/u/14542790",
-)
-embed.set_footer(text="Embed Footer Text")
-embed.set_timestamp()
-# Set `inline=False` for the embed field to occupy the whole line
-embed.add_embed_field(name="Field 1", value="Lorem ipsum", inline=False)
-embed.add_embed_field(name="Field 2", value="dolor sit", inline=False)
-embed.add_embed_field(name="Field 3", value="amet consetetur")
-embed.add_embed_field(name="Field 4", value="sadipscing elitr")
-
-webhook.add_embed(embed)
-response = webhook.execute()
-```
-
-![Image](img/extended_embed3.png "Example Non-Inline Embed Result")
-
-### Edit Webhook Messages
-
-```python
-from discord_webhook import DiscordWebhook
-from time import sleep
-
-webhook = DiscordWebhook(url='your webhook url', content='Webhook content before edit')
-webhook.execute()
-webhook.content = 'After Edit'
-sleep(10)
-webhook.edit()
-```
-
-### Delete Webhook Messages
-
-```python
-from discord_webhook import DiscordWebhook
-from time import sleep
-
-webhook = DiscordWebhook(url='your webhook url', content='Webhook Content')
-webhook.execute()
-sleep(10)
-webhook.delete()
-```
-
-### Send Files
-
-```python
-from discord_webhook import DiscordWebhook
-
-webhook = DiscordWebhook(url='your webhook url', username="Webhook with files")
-
-# send two images
-with open("path/to/first/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example.jpg')
-with open("path/to/second/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example2.jpg')
-
-response = webhook.execute()
-```
-
-![Image](img/webhook_files.png "Example Files Result")
-
-You can use uploaded attachments in Embeds:
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url='your webhook url')
-
-with open("path/to/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example.jpg')
-
-embed = DiscordEmbed(title='Embed Title', description='Your Embed Description', color='03b2f8')
-embed.set_thumbnail(url='attachment://example.jpg')
-
-webhook.add_embed(embed)
-response = webhook.execute()
-```
-
-### Remove Embeds and Files
-
-```python
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-webhook = DiscordWebhook(url='your webhook url')
-
-with open("path/to/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example.jpg')
-
-embed = DiscordEmbed(title='Embed Title', description='Your Embed Description', color='03b2f8')
-embed.set_thumbnail(url='attachment://example.jpg')
-
-webhook.add_embed(embed)
-response = webhook.execute(remove_embeds=True)
-# webhook.embeds will be empty after webhook is executed
-# You could also manually call the function webhook.remove_embeds()
-```
-
-`.remove_file()` removes the given file
-
-```python
-from discord_webhook import DiscordWebhook
-
-webhook = DiscordWebhook(url='your webhook url', username="Webhook with files")
-
-# send two images
-with open("path/to/first/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example.jpg')
-with open("path/to/second/image.jpg", "rb") as f:
-    webhook.add_file(file=f.read(), filename='example2.jpg')
-# remove 'example.jpg'
-webhook.remove_file('example.jpg')
-# only 'example2.jpg' is sent to the webhook
-response = webhook.execute()
-```
-
-### Allowed Mentions
-
-Look into the [Discord Docs](https://discord.com/developers/docs/resources/channel#allowed-mentions-object) for examples and for more explanation
-
-This example would only ping user `123` and `124` but not everyone else.
-
-```python
-from discord_webhook import DiscordWebhook
-
-content = "@everyone say hello to our new friends <@123> and <@124>"
-allowed_mentions = {
-    "users": ["123", "124"]
-}
-
-webhook = DiscordWebhook(url='your webhook url', content=content, allowed_mentions=allowed_mentions)
-response = webhook.execute()
-```
-
-### Use Proxies
-
-```python
-from discord_webhook import DiscordWebhook
-
-proxies = {
-  'http': 'http://10.10.1.10:3128',
-  'https': 'http://10.10.1.10:1080',
-}
-webhook = DiscordWebhook(url='your webhook url', content='Webhook Message', proxies=proxies)
-response = webhook.execute()
-```
-or
-```python
-from discord_webhook import DiscordWebhook
-
-proxies = {
-  'http': 'http://10.10.1.10:3128',
-  'https': 'http://10.10.1.10:1080',
-}
-webhook = DiscordWebhook(url='your webhook url', content='Webhook Message')
-webhook.set_proxies(proxies)
-response = webhook.execute()
-```
-
-### Use CLI
-
-```
-usage: discord_webhook [-h] -u URL [URL ...] -c CONTENT [--username USERNAME]
-                       [--avatar_url AVATAR_URL]
-
-Trigger discord webhook(s).
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -u URL [URL ...], --url URL [URL ...]
-                        Webhook(s) url(s)
-  -c CONTENT, --content CONTENT
-                        Message content
-  --username USERNAME   override the default username of the webhook
-  --avatar_url AVATAR_URL
-                        override the default avatar of the webhook
-```
-
-### Timeout
-
-```python
-from requests.exceptions import Timeout
-from discord_webhook import DiscordWebhook, DiscordEmbed
-
-# We will set ridiculously low timeout threshold for testing purposes
-webhook = DiscordWebhook(url='your webhook url', timeout=0.1)
-
-# You can also set timeout later using
-# webhook.timeout = 0.1
-
-embed = DiscordEmbed(title='Embed Title', description='Your Embed Description', color='03b2f8')
-
-webhook.add_embed(embed)
-
-# Handle timeout exception
-try:
-    response = webhook.execute()
-except Timeout as err:
-    print(f'Oops! Connection to Discord timed out: {err}')
-```
-
-### Async support
-In order to use the async version, you need to install the package using:
-```
-pip install discord-webhook[async]
-```
-Example usage:
-```python
-import asyncio
-from discord_webhook import AsyncDiscordWebhook
-
-
-async def send_webhook(message):
-    webhook = AsyncDiscordWebhook(url='your webhook url', content=message)
-    await webhook.execute()
-
-
-async def main():
-    await asyncio.gather(
-        send_webhook('Async webhook message 1'),
-        send_webhook('Async webhook message 2'),
-    )  # sends both messages asynchronously
-
-
-asyncio.run(main())
-```
-
-## Development
-
-### Dev Setup
-This project uses [Poetry](https://python-poetry.org/docs/) for dependency management and packaging.
-
-Install Poetry and add Poetry to [Path](https://python-poetry.org/docs/#installation).
-
-**Debian / Ubuntu / Mac**
-
-`curl -sSL https://install.python-poetry.org | python3 -`
-
-**Windows**
-
-open powershell and run: `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`
-
-Install dependencies: `poetry install`
-
-Install the defined pre-commit hooks: `poetry run pre-commit install`
-
-Activate the virtualenv: `poetry shell`
+Metadata-Version: 2.1
+Name: discord-webhook
+Version: 1.2.0
+Summary: Easily send Discord webhooks with Python
+Home-page: https://github.com/lovvskillz/python-discord-webhook
+License: MIT
+Keywords: discord,webhook
+Author: lovvskillz
+Author-email: 14542790+lovvskillz@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: async
+Requires-Dist: httpx (>=0.23.0,<0.24.0); extra == "async"
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/lovvskillz/python-discord-webhook
+Description-Content-Type: text/markdown
+
+# Python Discord webhook
+
+[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/lovvskillz/python-discord-webhook/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/discord-webhook.svg)](https://badge.fury.io/py/discord-webhook)
+[![Downloads](https://pepy.tech/badge/discord-webhook)](https://pepy.tech/project/discord-webhook)
+
+Easily send Discord webhooks with Python (also has [async support](#async-support))
+
+## Install
+
+Install via pip:
+```
+pip install discord-webhook
+```
+
+## Examples
+
+* [Basic Webhook](#basic-webhook)
+* [Create Multiple Instances / Use multiple URLs](#create-multiple-instances)
+* [Get Webhook by ID](#get-webhook-by-id)
+* [Manage Being Rate Limited](#manage-being-rate-limited)
+* [Embedded Content](#webhook-with-embedded-content)
+* [Edit Webhook Message](#edit-webhook-messages)
+* [Delete Webhook Message](#delete-webhook-messages)
+* [Send Files](#send-files)
+* [Remove Embeds and Files](#remove-embeds-and-files)
+* [Allowed Mentions](#allowed-mentions)
+* [Use Proxies](#use-proxies)
+* [Timeout](#timeout)
+* [Async Support](#async-support)
+
+### Basic Webhook
+
+```python
+from discord_webhook import DiscordWebhook
+
+webhook = DiscordWebhook(url="your webhook url", content="Webhook Message")
+response = webhook.execute()
+```
+
+### Create multiple instances
+If you want to use multiple URLs you need to create multiple instances.
+
+```python
+from discord_webhook import DiscordWebhook
+
+# you can provide any kwargs except url
+webhook1, webhook2 = DiscordWebhook.create_batch(urls=["first url", "second url"], content="Webhook Message")
+response1 = webhook1.execute()
+response2 = webhook2.execute()
+```
+![Image](img/multiple_urls.png "Multiple Urls Result")
+
+### Get Webhook by ID
+You can access a webhook that has already been sent by providing the ID.
+
+````python
+from discord_webhook import DiscordWebhook
+
+webhook = DiscordWebhook(url="your webhook url", id="your webhook message id")
+# now you could delete or edit the webhook
+# ...
+````
+
+### Manage being Rate Limited
+
+```python
+from discord_webhook import DiscordWebhook
+
+# if rate_limit_retry is True then in the event that you are being rate 
+# limited by Discord your webhook will automatically be sent once the 
+# rate limit has been lifted
+webhook = DiscordWebhook(url="your webhook url", rate_limit_retry=True, content="Webhook Message")
+response = webhook.execute()
+```
+
+![Image](img/basic_webhook.png "Basic Example Result")
+
+### Webhook with Embedded Content
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url")
+
+# create embed object for webhook
+# you can set the color as a decimal (color=242424) or hex (color="03b2f8") number
+embed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")
+
+# add embed object to webhook
+webhook.add_embed(embed)
+
+response = webhook.execute()
+```
+
+![Image](img/simple_embed.png "Basic Embed Example Result")
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url")
+
+# create embed object for webhook
+embed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")
+
+# set author
+embed.set_author(name="Author Name", url="author url", icon_url="author icon url")
+
+# set image
+embed.set_image(url="your image url")
+
+# set thumbnail
+embed.set_thumbnail(url="your thumbnail url")
+
+# set footer
+embed.set_footer(text="Embed Footer Text", icon_url="URL of icon")
+
+# set timestamp (default is now) accepted types are int, float and datetime
+embed.set_timestamp()
+
+# add fields to embed
+embed.add_embed_field(name="Field 1", value="Lorem ipsum")
+embed.add_embed_field(name="Field 2", value="dolor sit")
+
+# add embed object to webhook
+webhook.add_embed(embed)
+
+response = webhook.execute()
+```
+
+![Image](img/extended_embed.png "Basic Embed Example Result")
+
+This is another example with embedded content
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")
+
+embed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")
+embed.set_author(name="Author Name", url="https://github.com/lovvskillz", icon_url="https://avatars0.githubusercontent.com/u/14542790")
+embed.set_footer(text="Embed Footer Text")
+embed.set_timestamp()
+embed.add_embed_field(name="Field 1", value="Lorem ipsum")
+embed.add_embed_field(name="Field 2", value="dolor sit")
+embed.add_embed_field(name="Field 3", value="amet consetetur")
+embed.add_embed_field(name="Field 4", value="sadipscing elitr")
+
+webhook.add_embed(embed)
+response = webhook.execute()
+```
+
+![Image](img/extended_embed2.png "Example Embed Result")
+
+By Default, the Embed fields are placed side by side. We can arrange them in a new line by setting `inline=False` as follows:
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")
+
+embed = DiscordEmbed(
+    title="Embed Title", description="Your Embed Description", color="03b2f8"
+)
+embed.set_author(
+    name="Author Name",
+    url="https://github.com/lovvskillz",
+    icon_url="https://avatars0.githubusercontent.com/u/14542790",
+)
+embed.set_footer(text="Embed Footer Text")
+embed.set_timestamp()
+# Set `inline=False` for the embed field to occupy the whole line
+embed.add_embed_field(name="Field 1", value="Lorem ipsum", inline=False)
+embed.add_embed_field(name="Field 2", value="dolor sit", inline=False)
+embed.add_embed_field(name="Field 3", value="amet consetetur")
+embed.add_embed_field(name="Field 4", value="sadipscing elitr")
+
+webhook.add_embed(embed)
+response = webhook.execute()
+```
+
+![Image](img/extended_embed3.png "Example Non-Inline Embed Result")
+
+### Edit Webhook Messages
+
+```python
+from discord_webhook import DiscordWebhook
+from time import sleep
+
+webhook = DiscordWebhook(url="your webhook url", content="Webhook content before edit")
+webhook.execute()
+webhook.content = "After Edit"
+sleep(10)
+webhook.edit()
+```
+
+### Delete Webhook Messages
+
+```python
+from discord_webhook import DiscordWebhook
+from time import sleep
+
+webhook = DiscordWebhook(url="your webhook url", content="Webhook Content")
+webhook.execute()
+sleep(10)
+webhook.delete()
+```
+
+### Send Files
+
+```python
+from discord_webhook import DiscordWebhook
+
+webhook = DiscordWebhook(url="your webhook url", username="Webhook with files")
+
+# send two images
+with open("path/to/first/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example.jpg")
+with open("path/to/second/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example2.jpg")
+
+response = webhook.execute()
+```
+
+![Image](img/webhook_files.png "Example Files Result")
+
+You can use uploaded attachments in Embeds:
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url")
+
+with open("path/to/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example.jpg")
+
+embed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")
+embed.set_thumbnail(url="attachment://example.jpg")
+
+webhook.add_embed(embed)
+response = webhook.execute()
+```
+
+### Remove Embeds and Files
+
+```python
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+webhook = DiscordWebhook(url="your webhook url")
+
+with open("path/to/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example.jpg")
+
+embed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")
+embed.set_thumbnail(url="attachment://example.jpg")
+
+webhook.add_embed(embed)
+response = webhook.execute(remove_embeds=True)
+# webhook.embeds will be empty after webhook is executed
+# You could also manually call the function webhook.remove_embeds()
+```
+
+`.remove_file()` removes the given file
+
+```python
+from discord_webhook import DiscordWebhook
+
+webhook = DiscordWebhook(url="your webhook url", username="Webhook with files")
+
+# send two images
+with open("path/to/first/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example.jpg")
+with open("path/to/second/image.jpg", "rb") as f:
+    webhook.add_file(file=f.read(), filename="example2.jpg")
+# remove "example.jpg"
+webhook.remove_file("example.jpg")
+# only "example2.jpg" is sent to the webhook
+response = webhook.execute()
+```
+
+### Allowed Mentions
+
+Look into the [Discord Docs](https://discord.com/developers/docs/resources/channel#allowed-mentions-object) for examples and for more explanation
+
+This example would only ping user `123` and `124` but not everyone else.
+
+```python
+from discord_webhook import DiscordWebhook
+
+content = "@everyone say hello to our new friends <@123> and <@124>"
+allowed_mentions = {
+    "users": ["123", "124"]
+}
+
+webhook = DiscordWebhook(url="your webhook url", content=content, allowed_mentions=allowed_mentions)
+response = webhook.execute()
+```
+
+### Use Proxies
+
+```python
+from discord_webhook import DiscordWebhook
+
+proxies = {
+  "http": "http://10.10.1.10:3128",
+  "https": "http://10.10.1.10:1080",
+}
+webhook = DiscordWebhook(url="your webhook url", content="Webhook Message", proxies=proxies)
+response = webhook.execute()
+```
+or
+```python
+from discord_webhook import DiscordWebhook
+
+proxies = {
+  "http": "http://10.10.1.10:3128",
+  "https": "http://10.10.1.10:1080",
+}
+webhook = DiscordWebhook(url="your webhook url", content="Webhook Message")
+webhook.set_proxies(proxies)
+response = webhook.execute()
+```
+
+### Timeout
+
+```python
+from requests.exceptions import Timeout
+from discord_webhook import DiscordWebhook, DiscordEmbed
+
+# We will set ridiculously low timeout threshold for testing purposes
+webhook = DiscordWebhook(url="your webhook url", timeout=0.1)
+
+# You can also set timeout later using
+# webhook.timeout = 0.1
+
+embed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")
+
+webhook.add_embed(embed)
+
+# Handle timeout exception
+try:
+    response = webhook.execute()
+except Timeout as err:
+    print(f"Oops! Connection to Discord timed out: {err}")
+```
+
+### Async support
+In order to use the async version, you need to install the package using:
+```
+pip install discord-webhook[async]
+```
+Example usage:
+```python
+import asyncio
+from discord_webhook import AsyncDiscordWebhook
+
+
+async def send_webhook(message):
+    webhook = AsyncDiscordWebhook(url="your webhook url", content=message)
+    await webhook.execute()
+
+
+async def main():
+    await asyncio.gather(
+        send_webhook("Async webhook message 1"),
+        send_webhook("Async webhook message 2"),
+    )  # sends both messages asynchronously
+
+
+asyncio.run(main())
+```
+
+### Use CLI
+
+```
+usage: discord_webhook [-h] -u URL [URL ...] -c CONTENT [--username USERNAME]
+                       [--avatar_url AVATAR_URL]
+
+Trigger discord webhook(s).
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -u URL [URL ...], --url URL [URL ...]
+                        Webhook(s) url(s)
+  -c CONTENT, --content CONTENT
+                        Message content
+  --username USERNAME   override the default username of the webhook
+  --avatar_url AVATAR_URL
+                        override the default avatar of the webhook
+```
+
+## Development
+
+### Dev Setup
+This project uses [Poetry](https://python-poetry.org/docs/) for dependency management and packaging.
+
+Install Poetry and add Poetry to [Path](https://python-poetry.org/docs/#installation).
+
+**Debian / Ubuntu / Mac**
+
+`curl -sSL https://install.python-poetry.org | python3 -`
+
+**Windows**
+
+open powershell and run: `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`
+
+Install dependencies: `poetry install`
+
+Install the defined pre-commit hooks: `poetry run pre-commit install`
+
+Activate the virtualenv: `poetry shell`
```

### Comparing `discord-webhook-1.1.0/setup.py` & `discord-webhook-1.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 {'async': ['httpx>=0.23.0,<0.24.0']}
 
 entry_points = \
 {'console_scripts': ['discord_webhook = discord_webhook.__main__:main']}
 
 setup_kwargs = {
     'name': 'discord-webhook',
-    'version': '1.1.0',
-    'description': 'execute discord webhooks',
-    'long_description': '# python-discord-webhook\n\n[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/lovvskillz/python-discord-webhook/master/LICENSE)\n[![PyPI version](https://badge.fury.io/py/discord-webhook.svg)](https://badge.fury.io/py/discord-webhook)\n[![Downloads](https://pepy.tech/badge/discord-webhook)](https://pepy.tech/project/discord-webhook)\n\nExecute Discord Webhooks (also has [async support](#async-support))\n\n## Install\n\nInstall via pip:\n```\npip install discord-webhook\n```\n\n## Examples\n\n* [Basic Webhook](#basic-webhook)\n* [Create Multiple Instances / Use multiple URLs](#create-multiple-instances)\n* [Manage Being Rate Limited](#manage-being-rate-limited)\n* [Embedded Content](#webhook-with-embedded-content)\n* [Edit Webhook Message](#edit-webhook-messages)\n* [Delete Webhook Message](#delete-webhook-messages)\n* [Send Files](#send-files)\n* [Remove Embeds and Files](#remove-embeds-and-files)\n* [Allowed Mentions](#allowed-mentions)\n* [Use Proxies](#use-proxies)\n* [Timeout](#timeout)\n* [Async Support](#async-support)\n\n### Basic Webhook\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url=\'your webhook url\', content=\'Webhook Message\')\nresponse = webhook.execute()\n```\n\n### Create multiple instances\nIf you want to use multiple URLs you need to create multiple instances.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# you can provide any kwargs except url\nwebhook1, webhook2 = DiscordWebhook.create_batch(urls=[\'first url\', \'second url\'], content=\'Webhook Message\')\nresponse1 = webhook1.execute()\nresponse2 = webhook2.execute()\n```\n![Image](img/multiple_urls.png "Multiple Urls Result")\n\n### Manage being Rate Limited\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# if rate_limit_retry is True then in the event that you are being rate \n# limited by Discord your webhook will automatically be sent once the \n# rate limit has been lifted\nwebhook = DiscordWebhook(url=\'your webhook url\', rate_limit_retry=True,\n                         content=\'Webhook Message\')\nresponse = webhook.execute()\n```\n\n![Image](img/basic_webhook.png "Basic Example Result")\n\n### Webhook with Embedded Content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url=\'your webhook url\')\n\n# create embed object for webhook\n# you can set the color as a decimal (color=242424) or hex (color=\'03b2f8\') number\nembed = DiscordEmbed(title=\'Your Title\', description=\'Lorem ipsum dolor sit\', color=\'03b2f8\')\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/simple_embed.png "Basic Embed Example Result")\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url=\'your webhook url\')\n\n# create embed object for webhook\nembed = DiscordEmbed(title=\'Your Title\', description=\'Lorem ipsum dolor sit\', color=\'03b2f8\')\n\n# set author\nembed.set_author(name=\'Author Name\', url=\'author url\', icon_url=\'author icon url\')\n\n# set image\nembed.set_image(url=\'your image url\')\n\n# set thumbnail\nembed.set_thumbnail(url=\'your thumbnail url\')\n\n# set footer\nembed.set_footer(text=\'Embed Footer Text\', icon_url=\'URL of icon\')\n\n# set timestamp (default is now)\nembed.set_timestamp()\n\n# add fields to embed\nembed.add_embed_field(name=\'Field 1\', value=\'Lorem ipsum\')\nembed.add_embed_field(name=\'Field 2\', value=\'dolor sit\')\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed.png "Basic Embed Example Result")\n\nThis is another example with embedded content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url=\'your webhook url\', username="New Webhook Username")\n\nembed = DiscordEmbed(title=\'Embed Title\', description=\'Your Embed Description\', color=\'03b2f8\')\nembed.set_author(name=\'Author Name\', url=\'https://github.com/lovvskillz\', icon_url=\'https://avatars0.githubusercontent.com/u/14542790\')\nembed.set_footer(text=\'Embed Footer Text\')\nembed.set_timestamp()\nembed.add_embed_field(name=\'Field 1\', value=\'Lorem ipsum\')\nembed.add_embed_field(name=\'Field 2\', value=\'dolor sit\')\nembed.add_embed_field(name=\'Field 3\', value=\'amet consetetur\')\nembed.add_embed_field(name=\'Field 4\', value=\'sadipscing elitr\')\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed2.png "Example Embed Result")\n\nBy Default, the Embed fields are placed side by side. We can arrange them in a new line by setting `inline=False` as follows:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")\n\nembed = DiscordEmbed(\n    title="Embed Title", description="Your Embed Description", color=\'03b2f8\'\n)\nembed.set_author(\n    name="Author Name",\n    url="https://github.com/lovvskillz",\n    icon_url="https://avatars0.githubusercontent.com/u/14542790",\n)\nembed.set_footer(text="Embed Footer Text")\nembed.set_timestamp()\n# Set `inline=False` for the embed field to occupy the whole line\nembed.add_embed_field(name="Field 1", value="Lorem ipsum", inline=False)\nembed.add_embed_field(name="Field 2", value="dolor sit", inline=False)\nembed.add_embed_field(name="Field 3", value="amet consetetur")\nembed.add_embed_field(name="Field 4", value="sadipscing elitr")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed3.png "Example Non-Inline Embed Result")\n\n### Edit Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url=\'your webhook url\', content=\'Webhook content before edit\')\nwebhook.execute()\nwebhook.content = \'After Edit\'\nsleep(10)\nwebhook.edit()\n```\n\n### Delete Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url=\'your webhook url\', content=\'Webhook Content\')\nwebhook.execute()\nsleep(10)\nwebhook.delete()\n```\n\n### Send Files\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url=\'your webhook url\', username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example.jpg\')\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example2.jpg\')\n\nresponse = webhook.execute()\n```\n\n![Image](img/webhook_files.png "Example Files Result")\n\nYou can use uploaded attachments in Embeds:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url=\'your webhook url\')\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example.jpg\')\n\nembed = DiscordEmbed(title=\'Embed Title\', description=\'Your Embed Description\', color=\'03b2f8\')\nembed.set_thumbnail(url=\'attachment://example.jpg\')\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n### Remove Embeds and Files\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url=\'your webhook url\')\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example.jpg\')\n\nembed = DiscordEmbed(title=\'Embed Title\', description=\'Your Embed Description\', color=\'03b2f8\')\nembed.set_thumbnail(url=\'attachment://example.jpg\')\n\nwebhook.add_embed(embed)\nresponse = webhook.execute(remove_embeds=True)\n# webhook.embeds will be empty after webhook is executed\n# You could also manually call the function webhook.remove_embeds()\n```\n\n`.remove_file()` removes the given file\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url=\'your webhook url\', username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example.jpg\')\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename=\'example2.jpg\')\n# remove \'example.jpg\'\nwebhook.remove_file(\'example.jpg\')\n# only \'example2.jpg\' is sent to the webhook\nresponse = webhook.execute()\n```\n\n### Allowed Mentions\n\nLook into the [Discord Docs](https://discord.com/developers/docs/resources/channel#allowed-mentions-object) for examples and for more explanation\n\nThis example would only ping user `123` and `124` but not everyone else.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\ncontent = "@everyone say hello to our new friends <@123> and <@124>"\nallowed_mentions = {\n    "users": ["123", "124"]\n}\n\nwebhook = DiscordWebhook(url=\'your webhook url\', content=content, allowed_mentions=allowed_mentions)\nresponse = webhook.execute()\n```\n\n### Use Proxies\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  \'http\': \'http://10.10.1.10:3128\',\n  \'https\': \'http://10.10.1.10:1080\',\n}\nwebhook = DiscordWebhook(url=\'your webhook url\', content=\'Webhook Message\', proxies=proxies)\nresponse = webhook.execute()\n```\nor\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  \'http\': \'http://10.10.1.10:3128\',\n  \'https\': \'http://10.10.1.10:1080\',\n}\nwebhook = DiscordWebhook(url=\'your webhook url\', content=\'Webhook Message\')\nwebhook.set_proxies(proxies)\nresponse = webhook.execute()\n```\n\n### Use CLI\n\n```\nusage: discord_webhook [-h] -u URL [URL ...] -c CONTENT [--username USERNAME]\n                       [--avatar_url AVATAR_URL]\n\nTrigger discord webhook(s).\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u URL [URL ...], --url URL [URL ...]\n                        Webhook(s) url(s)\n  -c CONTENT, --content CONTENT\n                        Message content\n  --username USERNAME   override the default username of the webhook\n  --avatar_url AVATAR_URL\n                        override the default avatar of the webhook\n```\n\n### Timeout\n\n```python\nfrom requests.exceptions import Timeout\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\n# We will set ridiculously low timeout threshold for testing purposes\nwebhook = DiscordWebhook(url=\'your webhook url\', timeout=0.1)\n\n# You can also set timeout later using\n# webhook.timeout = 0.1\n\nembed = DiscordEmbed(title=\'Embed Title\', description=\'Your Embed Description\', color=\'03b2f8\')\n\nwebhook.add_embed(embed)\n\n# Handle timeout exception\ntry:\n    response = webhook.execute()\nexcept Timeout as err:\n    print(f\'Oops! Connection to Discord timed out: {err}\')\n```\n\n### Async support\nIn order to use the async version, you need to install the package using:\n```\npip install discord-webhook[async]\n```\nExample usage:\n```python\nimport asyncio\nfrom discord_webhook import AsyncDiscordWebhook\n\n\nasync def send_webhook(message):\n    webhook = AsyncDiscordWebhook(url=\'your webhook url\', content=message)\n    await webhook.execute()\n\n\nasync def main():\n    await asyncio.gather(\n        send_webhook(\'Async webhook message 1\'),\n        send_webhook(\'Async webhook message 2\'),\n    )  # sends both messages asynchronously\n\n\nasyncio.run(main())\n```\n\n## Development\n\n### Dev Setup\nThis project uses [Poetry](https://python-poetry.org/docs/) for dependency management and packaging.\n\nInstall Poetry and add Poetry to [Path](https://python-poetry.org/docs/#installation).\n\n**Debian / Ubuntu / Mac**\n\n`curl -sSL https://install.python-poetry.org | python3 -`\n\n**Windows**\n\nopen powershell and run: `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`\n\nInstall dependencies: `poetry install`\n\nInstall the defined pre-commit hooks: `poetry run pre-commit install`\n\nActivate the virtualenv: `poetry shell`',
+    'version': '1.2.0',
+    'description': 'Easily send Discord webhooks with Python',
+    'long_description': '# Python Discord webhook\n\n[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/lovvskillz/python-discord-webhook/master/LICENSE)\n[![PyPI version](https://badge.fury.io/py/discord-webhook.svg)](https://badge.fury.io/py/discord-webhook)\n[![Downloads](https://pepy.tech/badge/discord-webhook)](https://pepy.tech/project/discord-webhook)\n\nEasily send Discord webhooks with Python (also has [async support](#async-support))\n\n## Install\n\nInstall via pip:\n```\npip install discord-webhook\n```\n\n## Examples\n\n* [Basic Webhook](#basic-webhook)\n* [Create Multiple Instances / Use multiple URLs](#create-multiple-instances)\n* [Get Webhook by ID](#get-webhook-by-id)\n* [Manage Being Rate Limited](#manage-being-rate-limited)\n* [Embedded Content](#webhook-with-embedded-content)\n* [Edit Webhook Message](#edit-webhook-messages)\n* [Delete Webhook Message](#delete-webhook-messages)\n* [Send Files](#send-files)\n* [Remove Embeds and Files](#remove-embeds-and-files)\n* [Allowed Mentions](#allowed-mentions)\n* [Use Proxies](#use-proxies)\n* [Timeout](#timeout)\n* [Async Support](#async-support)\n\n### Basic Webhook\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message")\nresponse = webhook.execute()\n```\n\n### Create multiple instances\nIf you want to use multiple URLs you need to create multiple instances.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# you can provide any kwargs except url\nwebhook1, webhook2 = DiscordWebhook.create_batch(urls=["first url", "second url"], content="Webhook Message")\nresponse1 = webhook1.execute()\nresponse2 = webhook2.execute()\n```\n![Image](img/multiple_urls.png "Multiple Urls Result")\n\n### Get Webhook by ID\nYou can access a webhook that has already been sent by providing the ID.\n\n````python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", id="your webhook message id")\n# now you could delete or edit the webhook\n# ...\n````\n\n### Manage being Rate Limited\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# if rate_limit_retry is True then in the event that you are being rate \n# limited by Discord your webhook will automatically be sent once the \n# rate limit has been lifted\nwebhook = DiscordWebhook(url="your webhook url", rate_limit_retry=True, content="Webhook Message")\nresponse = webhook.execute()\n```\n\n![Image](img/basic_webhook.png "Basic Example Result")\n\n### Webhook with Embedded Content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\n# create embed object for webhook\n# you can set the color as a decimal (color=242424) or hex (color="03b2f8") number\nembed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/simple_embed.png "Basic Embed Example Result")\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\n# create embed object for webhook\nembed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")\n\n# set author\nembed.set_author(name="Author Name", url="author url", icon_url="author icon url")\n\n# set image\nembed.set_image(url="your image url")\n\n# set thumbnail\nembed.set_thumbnail(url="your thumbnail url")\n\n# set footer\nembed.set_footer(text="Embed Footer Text", icon_url="URL of icon")\n\n# set timestamp (default is now) accepted types are int, float and datetime\nembed.set_timestamp()\n\n# add fields to embed\nembed.add_embed_field(name="Field 1", value="Lorem ipsum")\nembed.add_embed_field(name="Field 2", value="dolor sit")\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed.png "Basic Embed Example Result")\n\nThis is another example with embedded content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_author(name="Author Name", url="https://github.com/lovvskillz", icon_url="https://avatars0.githubusercontent.com/u/14542790")\nembed.set_footer(text="Embed Footer Text")\nembed.set_timestamp()\nembed.add_embed_field(name="Field 1", value="Lorem ipsum")\nembed.add_embed_field(name="Field 2", value="dolor sit")\nembed.add_embed_field(name="Field 3", value="amet consetetur")\nembed.add_embed_field(name="Field 4", value="sadipscing elitr")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed2.png "Example Embed Result")\n\nBy Default, the Embed fields are placed side by side. We can arrange them in a new line by setting `inline=False` as follows:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")\n\nembed = DiscordEmbed(\n    title="Embed Title", description="Your Embed Description", color="03b2f8"\n)\nembed.set_author(\n    name="Author Name",\n    url="https://github.com/lovvskillz",\n    icon_url="https://avatars0.githubusercontent.com/u/14542790",\n)\nembed.set_footer(text="Embed Footer Text")\nembed.set_timestamp()\n# Set `inline=False` for the embed field to occupy the whole line\nembed.add_embed_field(name="Field 1", value="Lorem ipsum", inline=False)\nembed.add_embed_field(name="Field 2", value="dolor sit", inline=False)\nembed.add_embed_field(name="Field 3", value="amet consetetur")\nembed.add_embed_field(name="Field 4", value="sadipscing elitr")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed3.png "Example Non-Inline Embed Result")\n\n### Edit Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook content before edit")\nwebhook.execute()\nwebhook.content = "After Edit"\nsleep(10)\nwebhook.edit()\n```\n\n### Delete Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Content")\nwebhook.execute()\nsleep(10)\nwebhook.delete()\n```\n\n### Send Files\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example2.jpg")\n\nresponse = webhook.execute()\n```\n\n![Image](img/webhook_files.png "Example Files Result")\n\nYou can use uploaded attachments in Embeds:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_thumbnail(url="attachment://example.jpg")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n### Remove Embeds and Files\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_thumbnail(url="attachment://example.jpg")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute(remove_embeds=True)\n# webhook.embeds will be empty after webhook is executed\n# You could also manually call the function webhook.remove_embeds()\n```\n\n`.remove_file()` removes the given file\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example2.jpg")\n# remove "example.jpg"\nwebhook.remove_file("example.jpg")\n# only "example2.jpg" is sent to the webhook\nresponse = webhook.execute()\n```\n\n### Allowed Mentions\n\nLook into the [Discord Docs](https://discord.com/developers/docs/resources/channel#allowed-mentions-object) for examples and for more explanation\n\nThis example would only ping user `123` and `124` but not everyone else.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\ncontent = "@everyone say hello to our new friends <@123> and <@124>"\nallowed_mentions = {\n    "users": ["123", "124"]\n}\n\nwebhook = DiscordWebhook(url="your webhook url", content=content, allowed_mentions=allowed_mentions)\nresponse = webhook.execute()\n```\n\n### Use Proxies\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  "http": "http://10.10.1.10:3128",\n  "https": "http://10.10.1.10:1080",\n}\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message", proxies=proxies)\nresponse = webhook.execute()\n```\nor\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  "http": "http://10.10.1.10:3128",\n  "https": "http://10.10.1.10:1080",\n}\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message")\nwebhook.set_proxies(proxies)\nresponse = webhook.execute()\n```\n\n### Timeout\n\n```python\nfrom requests.exceptions import Timeout\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\n# We will set ridiculously low timeout threshold for testing purposes\nwebhook = DiscordWebhook(url="your webhook url", timeout=0.1)\n\n# You can also set timeout later using\n# webhook.timeout = 0.1\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\n\nwebhook.add_embed(embed)\n\n# Handle timeout exception\ntry:\n    response = webhook.execute()\nexcept Timeout as err:\n    print(f"Oops! Connection to Discord timed out: {err}")\n```\n\n### Async support\nIn order to use the async version, you need to install the package using:\n```\npip install discord-webhook[async]\n```\nExample usage:\n```python\nimport asyncio\nfrom discord_webhook import AsyncDiscordWebhook\n\n\nasync def send_webhook(message):\n    webhook = AsyncDiscordWebhook(url="your webhook url", content=message)\n    await webhook.execute()\n\n\nasync def main():\n    await asyncio.gather(\n        send_webhook("Async webhook message 1"),\n        send_webhook("Async webhook message 2"),\n    )  # sends both messages asynchronously\n\n\nasyncio.run(main())\n```\n\n### Use CLI\n\n```\nusage: discord_webhook [-h] -u URL [URL ...] -c CONTENT [--username USERNAME]\n                       [--avatar_url AVATAR_URL]\n\nTrigger discord webhook(s).\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u URL [URL ...], --url URL [URL ...]\n                        Webhook(s) url(s)\n  -c CONTENT, --content CONTENT\n                        Message content\n  --username USERNAME   override the default username of the webhook\n  --avatar_url AVATAR_URL\n                        override the default avatar of the webhook\n```\n\n## Development\n\n### Dev Setup\nThis project uses [Poetry](https://python-poetry.org/docs/) for dependency management and packaging.\n\nInstall Poetry and add Poetry to [Path](https://python-poetry.org/docs/#installation).\n\n**Debian / Ubuntu / Mac**\n\n`curl -sSL https://install.python-poetry.org | python3 -`\n\n**Windows**\n\nopen powershell and run: `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`\n\nInstall dependencies: `poetry install`\n\nInstall the defined pre-commit hooks: `poetry run pre-commit install`\n\nActivate the virtualenv: `poetry shell`',
     'author': 'lovvskillz',
     'author_email': '14542790+lovvskillz@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lovvskillz/python-discord-webhook',
     'packages': packages,
     'package_data': package_data,
```

