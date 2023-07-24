# Comparing `tmp/vprikol_api_python-1.4.tar.gz` & `tmp/vprikol_api_python-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.4.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.5.tar", max compression
```

## Comparing `vprikol_api_python-1.4.tar` & `vprikol_api_python-1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/README.md
--rw-r--r--   0        0        0      349 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/api.py
--rw-r--r--   0        0        0     5567 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/main.py
--rw-r--r--   0        0        0     3703 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/model.py
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.4/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/README.md
+-rw-r--r--   0        0        0      349 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/api.py
+-rw-r--r--   0        0        0     5949 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/main.py
+-rw-r--r--   0        0        0     3940 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/model.py
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.5/PKG-INFO
```

### Comparing `vprikol_api_python-1.4/vprikol_api/api.py` & `vprikol_api_python-1.5/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.4/vprikol_api/main.py` & `vprikol_api_python-1.5/vprikol_api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from .model import IpAPIResponse, MembersAPIResponse, PlayerInfoRodinaAPIResponse, PlayerInfoArizonaAPIResponse, \
     CreatedFindTaskAPIResponse, \
     ServerStatusAPIResponse, RatingAPIResponse, CheckRPUsernameAPIResponse, GenerateRPUsernameAPIResponse, \
     PlayerInfoNotFound
 
 from .api import get, post
-
 from typing import Literal
 import asyncio
-
 from pydantic import parse_obj_as, ValidationError
 
 
 class VprikolAPI:
     def __init__(self, token: str, base_url: str = 'https://api.vprikol.dev/'):
         if len(token) < 1:
             raise Exception('Токен передан неправильно.')
@@ -37,15 +35,19 @@
             if not fraction_id.isdigit():
                 continue
             for player in result.data[fraction_id]['players']:
                 players.append({'username': player, 'id': result.data[fraction_id]['players'][player]['id'],
                                 'isOnline': result.data[fraction_id]['players'][player]['isOnline'],
                                 'isLeader': result.data[fraction_id]['players'][player]['isLeader'],
                                 'rank': result.data[fraction_id]['players'][player]['rank'],
-                                'rankLabel': result.data[fraction_id]['players'][player]['rankLabel']})
+                                'rankLabel': result.data[fraction_id]['players'][player]['rankLabel'],
+                                'ingameId': result.data[fraction_id]['players'][player]['ingameId'],
+                                'lvl': result.data[fraction_id]['players'][player]['lvl'],
+                                'ping': result.data[fraction_id]['players'][player]['ping'],
+                                'color': result.data[fraction_id]['players'][player]['color']})
             result.data[fraction_id]['players'] = players
             response[fraction_id] = MembersAPIResponse(**result.data[fraction_id])
 
         return response
 
     async def get_player_information(self, server_id: int, nickname: str) -> PlayerInfoRodinaAPIResponse \
                                                                              | PlayerInfoArizonaAPIResponse \
@@ -53,19 +55,19 @@
         task = await post(url=f'{self.base_url}find/createTask', headers=self.headers,
                           params={'server': server_id, 'nick': nickname})
         if not task.success:
             raise Exception(task.error)
 
         task = CreatedFindTaskAPIResponse(**task.data)
         while True:
-            await asyncio.sleep(1)
             result = await get(url=f'{self.base_url}find/getTaskResult', headers=self.headers,
                                params={'request_id': task.request_id})
 
             if not result.success and result.error.error_code and result.error.error_code == 425:
+                await asyncio.sleep(1)
                 continue
 
             if result.error and result.error.error_code == 422:
                 return PlayerInfoNotFound(**result.error.dict())
 
             try:
                 return PlayerInfoArizonaAPIResponse(**result.data)
```

### Comparing `vprikol_api_python-1.4/vprikol_api/model.py` & `vprikol_api_python-1.5/vprikol_api/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 
 class FastApiErrorResponse(BaseModel):
     detail: FastAPIErrorDetail | str
 
 
 class APIErrorResponse(BaseModel):
-    error_code: int
+    status_code: int
     detail: str
+    request_queue: int | None = None
 
 
 class Response(GenericModel):
     data: DataT | None
     error: APIErrorResponse | FastApiErrorResponse | None
     success: bool = True
 
@@ -30,39 +31,51 @@
 class MembersAPIPlayer(BaseModel):
     username: str
     id: int | None
     is_online: bool = Field(alias='isOnline')
     is_leader: bool = Field(alias='isLeader')
     rank: int
     rank_label: str | None = Field(alias='rankLabel')
+    ingame_id: int = Field(alias='ingameId')
+    ping: int
+    lvl: int
+    color: int
+
+
+class MembersAPIRecord(BaseModel):
+    count: int
+    date: str
+    leader: str
 
 
 class MembersAPIResponse(BaseModel):
+    server_label: str = Field(alias='serverName')
     fraction_label: str = Field(alias='fractionLabel')
     players: list[MembersAPIPlayer]
+    record: MembersAPIRecord
     total_players: int = Field(alias='totalPlayers')
     total_online: int = Field(alias='totalOnline')
     leader_nickname: str | None = Field(alias='leaderNick')
     is_leader_online: bool = Field(alias='isLeaderOnline')
 
 
-
 class ServerStatusAPIResponse(BaseModel):
-    hostname: str
-    payday_multiplier: int = Field(alias='paydayMultiplier')
+    server_number: int = Field(alias='number')
+    ip: str
+    port: int
     online_players: int = Field(alias='onlinePlayers')
     max_players: int = Field(alias='maxPlayers')
     is_closed: bool = Field(alias='isClosed')
-    ip: str
     server_label: str = Field(alias='serverLabel')
 
 
 class CreatedFindTaskAPIResponse(BaseModel):
     request_id: str
     request_time: int
+    request_queue: int
 
 
 class PlayerInfoArizonaAPIResponse(BaseModel):
     account_id: int = Field(alias='accountId')
     player_id: int | None = Field(alias='playerId')
     lvl: int
     cash: int
@@ -78,15 +91,14 @@
     is_leader: bool = Field(alias='isLeader')
     org_label: str = Field(alias='orgLabel')
     org_id: int = Field(alias='orgId')
     vip_lvl: int = Field(alias='vipLvl')
     vip_label: str = Field(alias='vipLabel')
     phone_number: int | None = Field(alias='phoneNumber')
     updated_at: int = Field(alias='updatedAt')
-    is_new_request: bool = Field(alias='newRequest')
     player_nick: str = Field(alias='playerNick')
     player_server: int = Field(alias='playerServer')
     server_name: str = Field(alias='serverName')
 
 
 class PlayerInfoNotFound(APIErrorResponse):
     pass
```

