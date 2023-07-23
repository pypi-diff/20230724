# Comparing `tmp/fruitcraft-0.0.5.tar.gz` & `tmp/fruitcraft-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fruitcraft-0.0.5.tar", max compression
+gzip compressed data, was "fruitcraft-0.0.6.tar", max compression
```

## Comparing `fruitcraft-0.0.5.tar` & `fruitcraft-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-23 16:00:17.704127 fruitcraft-0.0.5/LICENSE
--rw-r--r--   0        0        0      128 2023-07-23 16:00:17.704127 fruitcraft-0.0.5/README.md
--rw-r--r--   0        0        0       99 2023-07-23 16:00:17.704127 fruitcraft-0.0.5/fruitcraft/__init__.py
--rw-r--r--   0        0        0    20184 2023-07-23 16:00:17.704127 fruitcraft-0.0.5/fruitcraft/client.py
--rw-r--r--   0        0        0    23243 2023-07-23 16:00:17.708127 fruitcraft-0.0.5/fruitcraft/f_types/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-23 16:00:17.708127 fruitcraft-0.0.5/fruitcraft/f_types/errors.py
--rw-r--r--   0        0        0     3985 2023-07-23 16:00:17.708127 fruitcraft-0.0.5/fruitcraft/f_types/utils.py
--rw-r--r--   0        0        0      809 2023-07-23 16:00:17.708127 fruitcraft-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/LICENSE
+-rw-r--r--   0        0        0      128 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/README.md
+-rw-r--r--   0        0        0      157 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/__init__.py
+-rw-r--r--   0        0        0    23815 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/client.py
+-rw-r--r--   0        0        0    23696 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/errors.py
+-rw-r--r--   0        0        0     3985 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/utils.py
+-rw-r--r--   0        0        0      809 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.6/PKG-INFO
```

### Comparing `fruitcraft-0.0.5/LICENSE` & `fruitcraft-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.5/fruitcraft/client.py` & `fruitcraft-0.0.6/fruitcraft/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from typing import Optional, List
 import string
 import random
 import time
 import httpx
 import asyncio
-import pydantic
 from .f_types import (
     DScaffold,
     APIResponse,
-    Achievements,
     AttackCardInfo,
     BattleRequest,
     BattleResponse,
-    Bundles,
     CardsSelection,
     CardInfo,
-    Coaching,
     CoolOffRequest,
     CoolOffResponse,
-    DailyReward,
     DeviceConstants,
     DeviceConstantsRequest,
     ErrorMessages,
     ErrorMessagesRequest,
     FillPotionRequest,
     FillPotionResponse,
     FruitCardInfo,
@@ -30,49 +25,34 @@
     FruitJsonExportRequest,
     GetOpponentsRequest,
     GetOpponentsResponse,
     GetPlayerInfoRequest,
     GetPlayerInfoResponse,
     GlobalRankingsRequest,
     GlobalRankingsResponse,
-    GoldPackInfo,
-    HeroIDSet,
-    HeroItems,
-    IntArray,
-    HeroItemInfo,
     LanguagePatchRequest,
     LanguagePathResponse,
     LeagueRankingsRequest,
     LeagueRankingsResponse,
     LeagueWinnerRanges,
     LiveBattleHelpRequest,
+    LiveBattleHelpResponse,
     LiveBattleRequest,
     LiveBattleResponse,
-    ModulesVersion,
     new_int_array,
-    Onsale,
-    OpponentInfo,
-    PlayerLeagueRankingInfo,
     PlayerComebackRequest,
     PlayerComebackResponse,
     PlayerLoadRequest,
     PlayerLoadResponse,
-    PlayerMedals,
-    PlayerRankingInfo,
     PotionizeRequest,
     PotionizeResponse,
-    Price,
     QuestRequest,
     QuestResponse,
-    Scaffold,
     SetCardForLiveBattleRequest,
     SetCardForLiveBattleResponse,
-    Tribe,
-    TribeInfo,
-    TribeMemberInfo,
     TribeMembersRequest,
     TribeMembersResponse,
     TribeRankingsRequest,
     TribeRankingsResponse,
 )
 from .f_types.utils import (
     xor_decrypt,
@@ -123,26 +103,104 @@
         
         self.mut = asyncio.Lock()
         self.http_client = httpx.AsyncClient()
         self.passport = passport
         if not self.logger:
             self.logger = logging.getLogger(__name__)
     
+    async def get_player_info(self, player_id: int) -> GetPlayerInfoResponse:
+        return await self.get_player_info_with_options(GetPlayerInfoRequest(player_id=player_id))
+    
+    async def get_player_info_with_options(self, opt: GetPlayerInfoRequest) -> GetPlayerInfoResponse:
+        api_response: APIResponse = await self.send_and_parse(
+            "player/getplayerinfo", opt, GetPlayerInfoResponse)
+        return api_response.data
+    
+    async def potionize(self, hero_id: int, amount: int) -> PotionizeResponse:
+        return await self.potionize_with_options(PotionizeRequest(potion=amount, hero_id=hero_id))
+    
+    async def potionize_with_options(self, opt: PotionizeRequest) -> PotionizeResponse:
+        api_response: APIResponse = await self.send_and_parse(
+            "cards/potionize", opt, PotionizeResponse)
+        return api_response.data
+    
+    async def fill_potions(self, amount: int = 50) -> FillPotionResponse:
+        return await self.fill_potions_with_options(FillPotionRequest(amount=amount))
+    
+    async def fill_potions_with_options(self, opt: FillPotionRequest) -> FillPotionResponse:
+        api_response: APIResponse = await self.send_and_parse(
+            "player/fillpotion", opt, FillPotionResponse)
+        
+        fill_result = api_response.data
+        if not isinstance(fill_result, FillPotionResponse):
+            return None
+        
+        if self.last_loaded_player:
+            self.last_loaded_player.potion_number = fill_result.potion_number
+        
+        return api_response.data
+    
+    async def get_league_rankings(self) -> LeagueRankingsResponse:
+        return await self.get_league_rankings_with_options(LeagueRankingsRequest())
+    
+    async def get_league_rankings_with_options(self, opt: LeagueRankingsRequest) -> LeagueRankingsResponse:
+        opt.set_default_values()
+        
+        api_response: APIResponse = await self.send_and_parse(
+            "ranking/league", opt, LeagueRankingsResponse)
+        return api_response.data
+    
+    async def get_global_rankings(self) -> GlobalRankingsResponse:
+        return await self.get_global_rankings_with_options(GlobalRankingsRequest())
+    
+    async def get_global_rankings_with_options(self, opt: GlobalRankingsRequest) -> GlobalRankingsResponse:
+        opt.set_default_values()
+        
+        api_response: APIResponse = await self.send_and_parse(
+            "ranking/global", opt, GlobalRankingsResponse)
+        return api_response.data
+    
+    async def get_tribe_rankings(self) -> TribeRankingsResponse:
+        return await self.get_tribe_rankings_with_options(TribeRankingsRequest())
+    
+    async def get_tribe_rankings_with_options(self, opt: TribeRankingsRequest) -> TribeRankingsResponse:
+        opt.set_default_values()
+        
+        api_response: APIResponse = await self.send_and_parse(
+            "ranking/tribe", opt, TribeRankingsResponse)
+        return api_response.data
+    
+    async def live_battle_help(self, battle_id: int) -> bool:
+        return await self.live_battle_help_with_options(LiveBattleHelpRequest(
+            battle_id=battle_id,
+        ))
+    
+    async def live_battle_help_with_options(self, opt: LiveBattleHelpRequest) -> bool:
+        api_response: APIResponse = await self.send_and_parse(
+            "live-battle/help", opt, LiveBattleHelpResponse)
+        return api_response.status
+    
+    async def set_card_for_live_battle(self, opt: SetCardForLiveBattleRequest) -> SetCardForLiveBattleResponse:
+        api_response: APIResponse = await self.send_and_parse(
+            "live-battle/setcardforlivebattle", opt, SetCardForLiveBattleResponse)
+        return api_response.data
+    
     async def do_live_battle(self, opponent_id: int) -> LiveBattleResponse:
         return await self.do_live_battle_with_options(LiveBattleRequest(
             opponent_id=opponent_id,
         ))
     
     async def do_live_battle_with_options(self, opt: LiveBattleRequest) -> LiveBattleResponse:
         if not isinstance(opt.opponent_id, int) and opt.opponent_id != None:
             tmp_id = getattr(opt.opponent_id, "id", None)
             if isinstance(tmp_id, int):
                 opt.opponent_id = tmp_id
         
-        api_response: APIResponse = await self.send_and_parse("live-battle/livebattle", opt, LiveBattleResponse)
+        api_response: APIResponse = await self.send_and_parse(
+            "live-battle/livebattle", opt, LiveBattleResponse)
         return api_response.data
     
     def set_cool_off_sleep_amount(self, sleep_amount: int) -> None:
         self.cool_off_sleep_time = sleep_amount
     
     async def heal_all(self, cards: CardsSelection) -> List[CoolOffResponse]:
         return await self.heal_all_with_ids(*cards.cards)
@@ -167,14 +225,19 @@
             )
         )
     
     async def cool_off_with_options(self, opt: CoolOffRequest) -> CoolOffResponse:
         api_response: APIResponse = await self.send_and_parse("cards/cooloff", opt, CoolOffResponse)
         return api_response.data
     
+    async def do_battle_and_heal(self, opponent_id: int, cards: CardsSelection) -> BattleResponse:
+        battle_result = await self.do_battle(opponent_id=opponent_id, cards=cards)
+        await self.heal_all(cards=cards)
+        return battle_result
+    
     async def do_battle(self, opponent_id: int, cards: CardsSelection) -> BattleResponse:
         return await self.do_battle_with_options(
             BattleRequest(
                 cards=new_int_array(cards.cards),
                 _cards_selection=cards,
                 hero_id=cards.hero_id,
                 opponent_id=opponent_id,
```

### Comparing `fruitcraft-0.0.5/fruitcraft/f_types/__init__.py` & `fruitcraft-0.0.6/fruitcraft/f_types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from pydantic import BaseModel
 from .utils import xor_encrypt
 from typing import (
     Any, List, Dict, Optional
 )
 import time
+import random
 
 class IntArray(str):
     pass
 
 LeagueWinnerRanges = Dict[str, int]
 
 class LoadRequestDefaults:
 	DEFAULT_GAME_VERSION      = "1.9.10691"
-	DEFAULT_U_DID             = "a341224a6fa458c8"
 	DEFAULT_OS_TYPE           = 2
 	DEFAULT_OS_VERSION        = "7.1.2"
 	DEFAULT_PHONE_MODEL       = "google pixel 2"
 	DEFAULT_METRIX_UID        = "-"
 	DEFAULT_APPS_FLYER_UID     = "1686402669312-333768616178664406"
 	DEFAULT_DEVICE_NAME       = "unknown"
 	DEFAULT_CONSTANTS_VERSION = "142"
@@ -416,15 +416,15 @@
     store_type: Optional[str] = ""
     
     def set_default_values(self):
         if not self.game_version:
             self.game_version = LoadRequestDefaults.DEFAULT_GAME_VERSION
         
         if not self.udid:
-            self.udid = LoadRequestDefaults.DEFAULT_U_DID
+            self.udid = ''.join(random.choices("abcdef0123456789", k=16))
         
         if not self.os_type:
             self.os_type = LoadRequestDefaults.DEFAULT_OS_TYPE
         
         if not self.os_version:
             self.os_version = LoadRequestDefaults.DEFAULT_OS_VERSION
         
@@ -502,15 +502,15 @@
     _cards_selection: Optional[CardsSelection] = None
 
 
 class TribeMemberInfo(DScaffold):
     id: Optional[int] = 0
     name: Optional[str] = ""
     rank: Optional[int] = 0
-    exp: Optional[int] = 0
+    xp: Optional[int] = 0
     gold: Optional[int] = 0
     tribe_permission: Optional[int] = 0
     level: Optional[int] = 0
     def_power: Optional[int] = 0
     status: Optional[int] = 0
     league_id: Optional[int] = 0
     league_rank: Optional[int] = 0
@@ -518,15 +518,15 @@
     poke_status: Optional[bool] = False
 
 
 class OpponentInfo(DScaffold):
     id: Optional[int] = 0
     name: Optional[str] = ""
     rank: Optional[int] = 0
-    exp: Optional[int] = 0
+    xp: Optional[int] = 0
     gold: Optional[int] = 0
     tribe_permission: Optional[int] = 0
     level: Optional[int] = 0
     def_power: Optional[int] = 0
     status: Optional[int] = 0
     league_id: Optional[int] = 0
     league_rank: Optional[int] = 0
@@ -650,38 +650,49 @@
     top_tribes: Optional[List[TribeInfo]] = []
     near_tribes: Optional[List[TribeInfo]] = []
     tribe_rank: Optional[int] = 0
 
 
 class TribeRankingsRequest(DScaffold):
     client: Optional[str] = ""
+    
+    def set_default_values(self):
+        if not self.client:
+            self.client = LoadRequestDefaults.DEFAULT_CLIENT_VALUE
 
 
 class LiveBattleHelpRequest(DScaffold):
     battle_id: Optional[int] = 0
 
+class LiveBattleHelpResponse(DScaffold):
+    dummy: Optional[str] = ""
+
 class PlayerRankingInfo(DScaffold):
     id: Optional[int] = 0
     name: Optional[str] = ""
     rank: Optional[int] = 0
-    exp: Optional[int] = 0
+    xp: Optional[int] = 0
     level: Optional[int] = 0
     tribe_id: Optional[int] = 0
     tribe_name: Optional[str] = ""
     avatar_id: Optional[int] = 0
 
 
 class GlobalRankingsResponse(DScaffold):
     top_players: Optional[List[PlayerRankingInfo]] = []
     near_players: Optional[List[PlayerRankingInfo]] = []
     rank: Optional[int] = 0
 
 
 class GlobalRankingsRequest(DScaffold):
     client: Optional[str] = ""
+    
+    def set_default_values(self):
+        if not self.client:
+            self.client = LoadRequestDefaults.DEFAULT_CLIENT_VALUE
 
 
 class PlayerLeagueRankingInfo(DScaffold):
     id: Optional[int] = 0
     name: Optional[str] = ""
     league_rank: Optional[int] = 0
     overall_score: Optional[int] = 0
@@ -748,7 +759,11 @@
     league_rank: Optional[int] = 0
     prev_league_id: Optional[int] = 0
     medals: Optional[Any] = None
 
 
 class LeagueRankingsRequest(DScaffold):
     client: Optional[str] = ""
+    
+    def set_default_values(self):
+        if not self.client:
+            self.client = LoadRequestDefaults.DEFAULT_CLIENT_VALUE
```

### Comparing `fruitcraft-0.0.5/fruitcraft/f_types/errors.py` & `fruitcraft-0.0.6/fruitcraft/f_types/errors.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.5/fruitcraft/f_types/utils.py` & `fruitcraft-0.0.6/fruitcraft/f_types/utils.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.5/pyproject.toml` & `fruitcraft-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fruitcraft"
-version = "0.0.5"
+version = "0.0.6"
 description = "Full Python Wrapper for fruitcraft game API. By Mr.AW ."
 authors = ["Mr. AW <mrawfruitly@gmail.com>"]
 packages = [
     { include = "fruitcraft" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fruitcraft-0.0.5/PKG-INFO` & `fruitcraft-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fruitcraft
-Version: 0.0.5
+Version: 0.0.6
 Summary: Full Python Wrapper for fruitcraft game API. By Mr.AW .
 Home-page: https://github.com/MrAwFruitly/FruitcraftClient-py
 Keywords: fruit,fruitcraft,fruit-craft,game-library
 Author: Mr. AW
 Author-email: mrawfruitly@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

