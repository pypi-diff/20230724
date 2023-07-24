# Comparing `tmp/mcc_api-1.0.4.tar.gz` & `tmp/mcc_api-1.0.5.tar.gz`

## Comparing `mcc_api-1.0.4.tar` & `mcc_api-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.4/docs/conf.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.4/docs/index.rst
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/exceptions.py
--rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/responses.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/run_tests.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_event.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_halloffame.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_participants.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_rundown.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_halloffame_game.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_participants_team.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.4/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.4/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.5/docs/conf.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.5/docs/index.rst
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/exceptions.py
+-rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/responses.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/run_tests.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_event.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_halloffame.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_participants.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_halloffame_game.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_participants_team.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.5/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.5/PKG-INFO
```

### Comparing `mcc_api-1.0.4/.github/workflows/docs.yml` & `mcc_api-1.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/.github/workflows/pypi_publish.yml` & `mcc_api-1.0.5/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/.github/workflows/tests.yml` & `mcc_api-1.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/docs/index.rst` & `mcc_api-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/mcc_api/__init__.py` & `mcc_api-1.0.5/mcc_api/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,110 +21,129 @@
     "get_rundown",
     "get_participants",
 
     "enums",
     "exceptions",
     "responses"
 ]
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 __base_url: t.Final[str] = "https://api.mcchampionship.com/v1"
 __user_agent: t.Final[str] = f"python_mcc_api/{__version__} (https://github.com/JamesMCo/python_mcc_api)"
 
 
 @ratelimit.sleep_and_retry
 @ratelimit.limits(calls=40, period=60)
-def __request(endpoint: str) -> requests.Response:
+def __request(endpoint: str, timeout: int) -> requests.Response:
     """Make and return a request to the given endpoint of the MCC API.
     
-    Limited to 40 calls per minute, and will sleep until the rate limit resets if exceeded."""
-    return requests.get(f"{__base_url.rstrip('/')}/{endpoint}", headers={"User-Agent": __user_agent})
+    Limited to 40 calls per minute, and will sleep until the rate limit resets if exceeded.
+    Timeout parameter is passed to requests module directly."""
+    return requests.get(
+        f"{__base_url.rstrip('/')}/{endpoint}",
+        headers={"User-Agent": __user_agent},
+        timeout=timeout
+    )
 
 
-def get_event() -> EventInformationResponse:
+def get_event(*, timeout: int = 5) -> EventInformationResponse:
     """Get event data for the current event cycle.
     
     - Calls the `/event <https://api.mcchampionship.com/docs/#/v1/AppController_getEventInformation>`_ endpoint.
     - Returns an :class:`mcc_api.EventInformationResponse` representing the current event cycle's event.
+    - May raise a :class:`requests.Timeout` exception, with the number of seconds before timing out specified by the
+      `timeout` parameter and defaulting to 5.
     """
-    return EventInformationResponse(__request("event"))
+    return EventInformationResponse(__request("event", timeout))
 
 
 @t.overload
-def get_hall_of_fame() -> HallOfFameResponse: ...
+def get_hall_of_fame(*, timeout: int = 5) -> HallOfFameResponse: ...
 @t.overload
-def get_hall_of_fame(game: Game) -> HallOfFameGameResponse: ...
+def get_hall_of_fame(game: Game, *, timeout: int = 5) -> HallOfFameGameResponse: ...
 
 
-def get_hall_of_fame(game: t.Optional[Game] = None):
+def get_hall_of_fame(game: t.Optional[Game] = None, *, timeout: int = 5):
     """Get hall of fame data, optionally restricted to a single game.
     
     When called with no `game` parameter:
         - Calls the `/halloffame <https://api.mcchampionship.com/docs/#/[Deprecated]%20v1/AppController_getHallOfFame>`_
           endpoint.
         - Returns a :class:`mcc_api.HallOfFameResponse` representing the entire Hall of Fame.
 
     When called with a `game` parameter:
         - Calls the `/halloffame/{game}
           <https://api.mcchampionship.com/docs/#/[Deprecated]%20v1/AppController_getHallOfFameByGame>`_ endpoint.
         - Returns a :class:`mcc_api.HallOfFameGameResponse` representing a single game from the Hall of Fame.
         - May raise an :class:`mcc_api.exceptions.InvalidGameError` exception, which can be avoided by passing an
           :class:`mcc_api.Game` enum.
 
+    In either case:
+        - May raise a :class:`requests.Timeout` exception, with the number of seconds before timing out specified by the
+          `timeout` parameter and defaulting to 5.
+
     .. warning::
        The /halloffame endpoint is deprecated and will be removed in a future release of the API.
        See https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.0
     """
     warnings.warn("The /halloffame endpoint is deprecated and will be removed in a future release of the API. "
                   "See https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.0",
                   DeprecationWarning, stacklevel=2)
     if game:
-        return HallOfFameGameResponse(__request(f"halloffame/{game}"))
+        return HallOfFameGameResponse(__request(f"halloffame/{game}", timeout))
     else:
-        return HallOfFameResponse(__request("halloffame"))
+        return HallOfFameResponse(__request("halloffame", timeout))
 
 
-def get_rundown(event: t.Optional[str] = None) -> RundownResponse:
+def get_rundown(event: t.Optional[str] = None, *, timeout: int = 5) -> RundownResponse:
     """Get an event's rundown data.
 
     When called with no `event` parameter:
         - Calls the `/rundown <https://api.mcchampionship.com/docs/#/v1/AppController_getRundown>`_ endpoint.
         - Returns a :class:`mcc_api.RundownResponse` representing the latest event.
 
     When called with an `event` parameter:
         - Calls the `/rundown/{event} <https://api.mcchampionship.com/docs/#/v1/AppController_getEventRundown>`_
           endpoint.
         - Returns a :class:`mcc_api.RundownResponse` representing the given event.
         - May raise an :class:`mcc_api.exceptions.InvalidEventError` exception.
+
+    In either case:
+        - May raise a :class:`requests.Timeout` exception, with the number of seconds before timing out specified by the
+          `timeout` parameter and defaulting to 5.
     """
     if event:
-        return RundownResponse(__request(f"rundown/{event}"))
+        return RundownResponse(__request(f"rundown/{event}", timeout))
     else:
-        return RundownResponse(__request("rundown"))
+        return RundownResponse(__request("rundown", timeout))
 
 
 @t.overload
-def get_participants() -> ParticipantsResponse: ...
+def get_participants(*, timeout: int = 5) -> ParticipantsResponse: ...
 @t.overload
-def get_participants(team: Team) -> ParticipantsTeamResponse: ...
+def get_participants(team: Team, *, timeout: int = 5) -> ParticipantsTeamResponse: ...
 
 
-def get_participants(team: t.Optional[Team] = None):
+def get_participants(team: t.Optional[Team] = None, *, timeout: int = 5):
     """Get the participants in the current event cycle.
     
     When called with no `team` parameter:
         - Calls the `/participants <https://api.mcchampionship.com/docs/#/v1/AppController_getParticipants>`_ endpoint.
         - Returns a :class:`mcc_api.ParticipantsResponse` representing all teams and their participants in the current
           event cycle.
 
     When called with a `team` parameter:
         - Calls the `/participants/{team}
           <https://api.mcchampionship.com/docs/#/v1/AppController_getParticipantsByTeam>`_ endpoint.
         - Returns a :class:`mcc_api.ParticipantsTeamResponse` representing the given team and its participants in the
           current event cycle.
         - May raise an :class:`mcc_api.exceptions.InvalidTeamError` exception, which can be avoided by passing an
           :class:`mcc_api.Team` enum.
+
+    In either case:
+        - May raise a :class:`requests.Timeout` exception, with the number of seconds before timing out specified by the
+          `timeout` parameter and defaulting to 5.
     """
     if team:
-        return ParticipantsTeamResponse(__request(f"participants/{team}"))
+        return ParticipantsTeamResponse(__request(f"participants/{team}", timeout))
     else:
-        return ParticipantsResponse(__request("participants"))
+        return ParticipantsResponse(__request("participants", timeout))
```

### Comparing `mcc_api-1.0.4/mcc_api/enums.py` & `mcc_api-1.0.5/mcc_api/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/mcc_api/exceptions.py` & `mcc_api-1.0.5/mcc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/mcc_api/responses.py` & `mcc_api-1.0.5/mcc_api/responses.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/run_tests.py` & `mcc_api-1.0.5/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/test_event.py` & `mcc_api-1.0.5/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/test_halloffame.py` & `mcc_api-1.0.5/tests/test_halloffame.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/test_participants.py` & `mcc_api-1.0.5/tests/test_participants.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/test_rundown.py` & `mcc_api-1.0.5/tests/test_rundown.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/mock_data/200_halloffame.json` & `mcc_api-1.0.5/tests/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/mock_data/200_participants.json` & `mcc_api-1.0.5/tests/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/mock_data/200_participants_team.json` & `mcc_api-1.0.5/tests/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/tests/mock_data/200_rundown.json` & `mcc_api-1.0.5/tests/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/.gitignore` & `mcc_api-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/LICENSE` & `mcc_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/README.md` & `mcc_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/pyproject.toml` & `mcc_api-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.4/PKG-INFO` & `mcc_api-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcc-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

