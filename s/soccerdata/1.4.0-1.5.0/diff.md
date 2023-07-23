# Comparing `tmp/soccerdata-1.4.0.tar.gz` & `tmp/soccerdata-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.4.0.tar", max compression
+gzip compressed data, was "soccerdata-1.5.0.tar", max compression
```

## Comparing `soccerdata-1.4.0.tar` & `soccerdata-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1384 2023-05-30 09:46:00.237763 soccerdata-1.4.0/LICENSE.rst
--rw-r--r--   0        0        0     3130 2023-05-30 09:46:00.237763 soccerdata-1.4.0/README.rst
--rw-r--r--   0        0        0     2352 2023-05-30 09:46:16.973858 soccerdata-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      457 2023-05-30 09:46:16.973858 soccerdata-1.4.0/soccerdata/__init__.py
--rw-r--r--   0        0        0    20702 2023-05-30 09:46:00.245763 soccerdata-1.4.0/soccerdata/_common.py
--rw-r--r--   0        0        0     5120 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/_config.py
--rw-r--r--   0        0        0     6382 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/clubelo.py
--rw-r--r--   0        0        0    12890 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/espn.py
--rw-r--r--   0        0        0    42225 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/fbref.py
--rw-r--r--   0        0        0     8536 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0     4547 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/match_history.py
--rw-r--r--   0        0        0    16744 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/sofifa.py
--rw-r--r--   0        0        0    32302 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/whoscored.py
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.4.0/setup.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1384 2023-07-23 22:15:29.151558 soccerdata-1.5.0/LICENSE.rst
+-rw-r--r--   0        0        0     3130 2023-07-23 22:15:29.151558 soccerdata-1.5.0/README.rst
+-rw-r--r--   0        0        0     2328 2023-07-23 22:15:49.399722 soccerdata-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-07-23 22:15:49.399722 soccerdata-1.5.0/soccerdata/__init__.py
+-rw-r--r--   0        0        0    20702 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/_common.py
+-rw-r--r--   0        0        0     5207 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/_config.py
+-rw-r--r--   0        0        0     6382 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    12890 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/espn.py
+-rw-r--r--   0        0        0    44941 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8536 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0     4657 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/match_history.py
+-rw-r--r--   0        0        0    16744 2023-07-23 22:15:29.163558 soccerdata-1.5.0/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    32695 2023-07-23 22:15:29.163558 soccerdata-1.5.0/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 soccerdata-1.5.0/PKG-INFO
```

### Comparing `soccerdata-1.4.0/LICENSE.rst` & `soccerdata-1.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/README.rst` & `soccerdata-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/pyproject.toml` & `soccerdata-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.4.0"
+version = "1.5.0"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -12,22 +12,21 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-pandas = "^1.0"
+pandas = "^2.0.0"
 requests = "^2.23"
 unicode = "^2.7"
 lxml = "^4.6"
 selenium = "^4.0.0"
 Unidecode = "^1.2.0"
 rich = "^13.0.0"
-pretty-errors = "^1.2.25"
 PySocks = "^1.7.1"
 html5lib = "^1.1"
 undetected-chromedriver = "^3.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 mypy = "^1.0"
```

### Comparing `soccerdata-1.4.0/soccerdata/_common.py` & `soccerdata-1.5.0/soccerdata/_common.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/soccerdata/_config.py` & `soccerdata-1.5.0/soccerdata/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 import logging
 import logging.config
 import os
 import sys
 from pathlib import Path
 
-import pretty_errors  # NOQA: F401 (imported but unused)
 from rich.logging import RichHandler
 
 # Configuration
 NOCACHE = os.environ.get("SOCCERDATA_NOCACHE", 'False').lower() in ('true', '1', 't')
 NOSTORE = os.environ.get("SOCCERDATA_NOSTORE", 'False').lower() in ('true', '1', 't')
 LOGLEVEL = os.environ.get('SOCCERDATA_LOGLEVEL', 'INFO').upper()
 
@@ -145,14 +144,18 @@
         "season_start": "Aug",
         "season_end": "May",
     },
     "INT-World Cup": {
         "FBref": "FIFA World Cup",
         "WhoScored": "International - FIFA World Cup",
     },
+    "INT-Women's World Cup": {
+        "FBref": "FIFA Women's World Cup",
+        "WhoScored": "International - FIFA Women's World Cup",
+    },
 }
 _f_custom_league_dict = CONFIG_DIR / "league_dict.json"
 if _f_custom_league_dict.is_file():
     with open(_f_custom_league_dict, encoding='utf8') as json_file:
         LEAGUE_DICT = {**LEAGUE_DICT, **json.load(json_file)}
     logger.info("Custom league dict loaded from %s.", _f_custom_league_dict)
 else:
```

### Comparing `soccerdata-1.4.0/soccerdata/clubelo.py` & `soccerdata-1.5.0/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/soccerdata/espn.py` & `soccerdata-1.5.0/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/soccerdata/fbref.py` & `soccerdata-1.5.0/soccerdata/fbref.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,31 +131,28 @@
         filepath = self.data_dir / "leagues.html"
         reader = self.get(url, filepath)
 
         # extract league links
         leagues = []
         tree = html.parse(reader)
         for html_table in tree.xpath("//table[contains(@id, 'comps')]"):
-            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table = _parse_table(html_table)
             df_table["url"] = html_table.xpath(".//th[@data-stat='league_name']/a/@href")
             leagues.append(df_table)
         df = (
             pd.concat(leagues)
             .pipe(standardize_colnames)
             .rename(columns={"competition_name": "league"})
             .pipe(self._translate_league)
             .drop_duplicates(subset="league")
             .set_index("league")
             .sort_index()
         )
         df["first_season"] = df["first_season"].apply(season_code)
         df["last_season"] = df["last_season"].apply(season_code)
-        df["country"] = df["country"].apply(
-            lambda x: x.split(" ")[1] if isinstance(x, str) else None
-        )
         return df[df.index.isin(self.leagues)]
 
     def read_seasons(self) -> pd.DataFrame:
         """Retrieve the selected seasons for the selected leagues.
 
         Returns
         -------
@@ -169,15 +166,15 @@
             url = FBREF_API + league.url
             filepath = self.data_dir / filemask.format(lkey)
             reader = self.get(url, filepath)
 
             # extract season links
             tree = html.parse(reader)
             (html_table,) = tree.xpath("//table[@id='seasons']")
-            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table = _parse_table(html_table)
             df_table["url"] = html_table.xpath(
                 "//th[@data-stat='year_id' or @data-stat='year']/a/@href"
             )
             # Override the competition name or add if missing
             df_table["Competition Name"] = lkey
             # Some tournaments have a "year" column instead of "season"
             if "Year" in df_table.columns:
@@ -192,15 +189,15 @@
         df = pd.concat(seasons).pipe(standardize_colnames)
         df = df.rename(columns={"competition_name": "league"})
         df["season"] = df["season"].apply(season_code)
         # if both a 20xx and 19xx season are available, drop the 19xx season
         df.drop_duplicates(subset=["league", "season"], keep="first", inplace=True)
         df = df.set_index(["league", "season"]).sort_index()
         return df.loc[
-            df.index.isin(itertools.product(self.leagues, self.seasons)), ["format", "url"]
+            df.index.isin(list(itertools.product(self.leagues, self.seasons))), ["format", "url"]
         ]
 
     def read_team_season_stats(  # noqa: C901
         self, stat_type: str = "standard", opponent_stats: bool = False
     ) -> pd.DataFrame:
         """Retrieve aggregated season stats for all teams in the selected leagues and seasons.
 
@@ -276,49 +273,43 @@
 
         # collect teams
         teams = []
         for (lkey, skey), season in seasons.iterrows():
             big_five = lkey == "Big 5 European Leagues Combined"
             tournament = season["format"] == "elimination"
             # read html page (league overview)
-            filepath = self.data_dir / filemask.format(
-                lkey, skey, stat_type if big_five else "all"
-            )
+            filepath = self.data_dir / filemask.format(lkey, skey, stat_type if big_five else page)
             url = (
                 FBREF_API
                 + "/".join(season.url.split("/")[:-1])
                 + (f"/{page}/squads/" if big_five else f"/{page}/" if tournament else "/")
                 + season.url.split("/")[-1]
             )
             reader = self.get(url, filepath)
 
             # parse HTML and select table
             tree = html.parse(reader)
             (html_table,) = tree.xpath(
                 f"//table[@id='stats_teams_{stat_type}' or @id='stats_squads_{stat_type}']"
             )
-            # remove icons
-            for elem in html_table.xpath("//span"):
-                elem.getparent().remove(elem)
-            # parse table
-            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table = _parse_table(html_table)
             df_table["league"] = lkey
             df_table["season"] = skey
             df_table["url"] = html_table.xpath(".//*[@data-stat='team']/a/@href")
             if big_five:
                 df_table["league"] = (
                     df_table.xs("Comp", axis=1, level=1).squeeze().map(BIG_FIVE_DICT)
                 )
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
                 df_table.drop("Rk", axis=1, level=1, inplace=True)
             teams.append(df_table)
 
         # return data frame
         df = (
-            _concat(teams)
+            _concat(teams, key=['league', 'season'])
             .rename(columns={"Squad": "team", "# Pl": "players_used"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             # .pipe(standardize_colnames)
             .set_index(["league", "season", "team"])
             .sort_index()
         )
         return df
@@ -403,70 +394,62 @@
             if len(iterator) == 0:
                 raise ValueError("No data found for the given teams in the selected seasons.")
         else:
             iterator = df_teams
 
         # collect match logs for each team
         stats = []
-        for (lkey, skey, team), team_url in iterator.url.items():
+        for (_, skey, team), team_url in iterator.url.items():
             # read html page
             filepath = self.data_dir / filemask.format(team, skey, stat_type)
             url = (
                 FBREF_API
                 + team_url.rsplit("/", 1)[0]
                 + "/matchlogs"
                 + "/all_comps"
                 + f"/{stat_type}"
             )
             reader = self.get(url, filepath)
 
             # parse HTML and select table
             tree = html.parse(reader)
             (html_table,) = tree.xpath(f"//table[@id='matchlogs_{opp_type}']")
-            # remove icons
-            for elem in html_table.xpath("//span"):
-                elem.getparent().remove(elem)
             # remove for / against header
             for elem in html_table.xpath("//th[@data-stat='header_for_against']"):
                 elem.text = ""
-            # remove table sections
-            for elem in html_table.xpath("//tr[contains(@class, 'thead')]"):
-                elem.getparent().remove(elem)
             # remove aggregate rows
             for elem in html_table.xpath("//tfoot"):
                 elem.getparent().remove(elem)
             # parse table
-            (df_table,) = pd.read_html(html.tostring(html_table))
-            df_table["league"] = lkey
+            df_table = _parse_table(html_table)
             df_table["season"] = skey
             df_table["team"] = team
             df_table["Time"] = html_table.xpath(".//td[@data-stat='start_time']/@csk")
             df_table["Match Report"] = [
                 mlink.xpath("./a/@href")[0]
                 if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
                 else None
                 for mlink in html_table.xpath(".//td[@data-stat='match_report']")
             ]
             nb_levels = df_table.columns.nlevels
             if nb_levels == 2:
-                df_table = df_table.drop("Comp", axis=1, level=1)
                 df_table = df_table.drop("Match Report", axis=1, level=1)
                 df_table = df_table.drop("Time", axis=1, level=1)
-            else:
-                del df_table["Comp"]
             stats.append(df_table)
 
         # return data frame
         df = (
-            _concat(stats)
+            _concat(stats, key=['league', 'season', 'team'])
             .replace(
                 {
                     "Opponent": TEAMNAME_REPLACEMENTS,
                 }
             )
+            .rename(columns={"Comp": "league"})
+            .pipe(self._translate_league)
             .pipe(
                 standardize_colnames,
                 cols=[
                     "Team",
                     "Opponent",
                     "Venue",
                     "Date",
@@ -571,30 +554,34 @@
             )
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             # remove icons
             for elem in tree.xpath("//td[@data-stat='comp_level']//span"):
                 elem.getparent().remove(elem)
             if big_five:
-                (df_table,) = pd.read_html(html.tostring(tree))
+                df_table = _parse_table(tree)
                 df_table[("Unnamed: league", "league")] = (
                     df_table.xs("Comp", axis=1, level=1).squeeze().map(BIG_FIVE_DICT)
                 )
                 df_table[("Unnamed: season", "season")] = skey
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
             else:
                 (el,) = tree.xpath(f"//comment()[contains(.,'div_stats_{stat_type}')]")
-                (df_table,) = pd.read_html(el.text, attrs={"id": f"stats_{stat_type}"})
+                parser = etree.HTMLParser(recover=True)
+                (html_table,) = etree.fromstring(el.text, parser).xpath(
+                    f"//table[contains(@id, 'stats_{stat_type}')]"
+                )
+                df_table = _parse_table(html_table)
                 df_table[("Unnamed: league", "league")] = lkey
                 df_table[("Unnamed: season", "season")] = skey
             df_table = _fix_nation_col(df_table)
             players.append(df_table)
 
         # return dataframe
-        df = _concat(players)
+        df = _concat(players, key=["league", "season"])
         df = df[df.Player != "Player"]
         df = (
             df.drop("Matches", axis=1, level=0)
             .drop("Rk", axis=1, level=0)
             .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(standardize_colnames, cols=["Player", "Nation", "Pos", "Age", "Born"])
@@ -633,15 +620,15 @@
             filepath_fixtures = self.data_dir / f"schedule_{lkey}_{skey}.html"
             current_season = not self._is_complete(lkey, skey)
             reader = self.get(
                 url_fixtures, filepath_fixtures, no_cache=current_season and not force_cache
             )
             tree = html.parse(reader)
             html_table = tree.xpath("//table[contains(@id, 'sched')]")[0]
-            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table = _parse_table(html_table)
             df_table["Match Report"] = [
                 mlink.xpath("./a/@href")[0]
                 if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
                 else None
                 for mlink in html_table.xpath(".//td[@data-stat='match_report']")
             ]
             df_table["league"] = lkey
@@ -774,38 +761,36 @@
             (home_team, away_team) = self._parse_teams(tree)
             if stat_type == "keepers":
                 id_format = "keeper_stats_{}"
             else:
                 id_format = "stats_{}_" + stat_type
             html_table = tree.find("//table[@id='" + id_format.format(home_team["id"]) + "']")
             if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table = _parse_table(html_table)
                 df_table["team"] = home_team["name"]
                 df_table["game"] = game["game"]
                 df_table["league"] = game["league"]
                 df_table["season"] = game["season"]
                 df_table["game_id"] = game["game_id"]
-                df_table = _fix_nation_col(df_table)
                 stats.append(df_table)
             else:
                 logger.warning("No stats found for home team for game with id=%s", game["game_id"])
             html_table = tree.find("//table[@id='" + id_format.format(away_team["id"]) + "']")
             if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table = _parse_table(html_table)
                 df_table["team"] = away_team["name"]
                 df_table["game"] = game["game"]
                 df_table["league"] = game["league"]
                 df_table["season"] = game["season"]
                 df_table["game_id"] = game["game_id"]
-                df_table = _fix_nation_col(df_table)
                 stats.append(df_table)
             else:
                 logger.warning("No stats found for away team for game with id=%s", game["game_id"])
 
-        df = _concat(stats)
+        df = _concat(stats, key=['game'])
         df = df[~df.Player.str.contains(r"^\d+\sPlayers$")]
         df = (
             df.rename(columns={"#": "jersey_number"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(standardize_colnames, cols=["Player", "Nation", "Pos", "Age", "Min"])
             .set_index(["league", "season", "game", "team", "player"])
             .sort_index()
@@ -861,15 +846,15 @@
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
             html_tables = tree.xpath("//div[@class='lineup']")
             for i, html_table in enumerate(html_tables):
                 # parse lineup table
-                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table = _parse_table(html_table)
                 df_table.columns = ["jersey_number", "player"]
                 df_table["team"] = teams[i]["name"]
                 if "Bench" in df_table.jersey_number.values:
                     bench_idx = df_table.index[df_table.jersey_number == "Bench"][0]
                     df_table.loc[:bench_idx, "is_starter"] = True
                     df_table.loc[bench_idx:, "is_starter"] = False
                     df_table["game"] = game["game"]
@@ -877,15 +862,15 @@
                     df_table["season"] = game["season"]
                     df_table["game"] = game["game"]
                     df_table.drop(bench_idx, inplace=True)
                 # augment with stats
                 html_stats_table = tree.find(
                     "//table[@id='" + "stats_{}_summary".format(teams[i]["id"]) + "']"
                 )
-                (df_stats_table,) = pd.read_html(html.tostring(html_stats_table))
+                df_stats_table = _parse_table(html_stats_table)
                 df_stats_table = df_stats_table.droplevel(0, axis=1)[["Player", "Pos", "Min"]]
                 df_stats_table.columns = ["player", "position", "minutes_played"]
                 lineups.append(pd.merge(df_table, df_stats_table, on="player", how="left"))
         df = pd.concat(lineups).set_index(["league", "season", "game"])
         return df
 
     def read_events(
@@ -944,15 +929,16 @@
             teams = self._parse_teams(tree)
             for team, tid in zip(teams, ["a", "b"]):
                 html_events = tree.xpath(f"////*[@id='events_wrap']/div/div[@class='event {tid}']")
                 for e in html_events:
                     minute = e.xpath("./div[1]")[0].text.replace("&rsquor;", "").strip()
                     score = e.xpath("./div[1]/small/span")[0].text
                     player1 = e.xpath("./div[2]/div[2]/div/a")[0].text
-                    if e.xpath("./div[2]/div[2]/small"):
+                    print(minute, score, player1)
+                    if e.xpath("./div[2]/div[2]/small/a"):
                         player2 = e.xpath("./div[2]/div[2]/small/a")[0].text
                     else:
                         player2 = None
                     event_type = e.xpath("./div[2]/div[1]/@class")[0].split(" ")[1]
                     match_events.append(
                         {
                             "team": team["name"],
@@ -969,15 +955,15 @@
             df_match_events["season"] = game["season"]
             events.append(df_match_events)
 
         if len(events) == 0:
             return pd.DataFrame()
 
         df = (
-            _concat(events)
+            pd.concat(events)
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .set_index(["league", "season", "game"])
             .sort_index()
             .dropna(how="all")
         )
         return df
 
@@ -1023,118 +1009,194 @@
                 raise ValueError("No games found with the given IDs in the selected seasons.")
         else:
             iterator = df_schedule
 
         shots = []
         for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
-            # get league and season
+            # get league anigd season
             logger.info(
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             html_table = tree.find("//table[@id='shots_all']")
             if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table), flavor="lxml")
+                df_table = _parse_table(html_table)
                 df_table["league"] = game["league"]
                 df_table["season"] = game["season"]
                 df_table["game"] = game["game"]
                 shots.append(df_table)
             else:
                 logger.warning("No shot data found for game with id=%s", game["game_id"])
 
         if len(shots) == 0:
             return pd.DataFrame()
 
         df = (
-            _concat(shots)
+            _concat(shots, key=['game'])
             .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(
                 standardize_colnames,
                 cols=["Outcome", "Minute", "Distance", "Player", "Body Part", "Notes", "Event"],
             )
             .set_index(["league", "season", "game"])
             .sort_index()
             .dropna(how="all")
         )
         return df
 
 
-def _concat(dfs: List[pd.DataFrame]) -> pd.DataFrame:
+def _parse_table(html_table: html.HtmlElement) -> pd.DataFrame:
+    """Parse HTML table into a dataframe.
+
+    Parameters
+    ----------
+    html_table : lxml.html.HtmlElement
+        HTML table to clean up.
+
+    Returns
+    -------
+    pd.DataFrame
+    """
+    # remove icons
+    for elem in html_table.xpath("//span[contains(@class, 'f-i')]"):
+        etree.strip_elements(elem.getparent(), "span", with_tail=False)
+    # remove sep rows
+    for elem in html_table.xpath("//tbody/tr[contains(@class, 'spacer')]"):
+        elem.getparent().remove(elem)
+    # remove thead rows in the table body
+    for elem in html_table.xpath("//tbody/tr[contains(@class, 'thead')]"):
+        elem.getparent().remove(elem)
+    # parse HTML to dataframe
+    (df_table,) = pd.read_html(html.tostring(html_table), flavor="lxml")
+    return df_table.convert_dtypes()
+
+
+def _concat(dfs: List[pd.DataFrame], key: List[str]) -> pd.DataFrame:
     """Merge matching tables scraped from different pages.
 
-    The level 0 headers are not consitent across seasons and leagues, this
+    The level 0 headers are not consistent across seasons and leagues, this
     function tries to determine uniform column names.
 
     Parameters
     ----------
     dfs : list(pd.DataFrame)
         Input dataframes.
+    key : list(str)
+        List of columns that uniquely identify each df.
+
+    Raises
+    ------
+    RuntimeError
+        If the dfs cannot be merged due to the columns not matching each other.
 
     Returns
     -------
     pd.DataFrame
         Concatenated dataframe with uniform column names.
     """
-    # Look for the most complete level 0 columns
     all_columns = []
+
+    # Step 1: Clean up the columns of each dataframe that should be merged
     for df in dfs:
         columns = pd.DataFrame(df.columns.tolist())
-        # Move missing columns to level 0
+        # Set "Unnamed: ..." column names to None
+        columns.replace(to_replace=r"^Unnamed:.*", value=None, regex=True, inplace=True)
         if columns.shape[1] == 2:
-            columns.replace({"": None}, inplace=True)
+            # Set "" column names to None
+            columns.replace(to_replace="", value=None, inplace=True)
+            # Move None column names to level 0
             mask = pd.isnull(columns[1])
             columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
-        # Rename unnamed columns
-        mask = columns[0].str.startswith("Unnamed:").fillna(False)
-        columns.loc[mask, 0] = None
-        all_columns.append(columns)
-    columns = reduce(lambda left, right: left.combine_first(right), all_columns)
+            # We'll try to replace some the None values in step 2
+            all_columns.append(columns.copy())
+            # But for now, we assume that we cannot replace them and move all
+            # missing columns to level 1 and replace them with the empty string
+            mask = pd.isnull(columns[0])
+            columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
+            columns.loc[mask, 1] = ""
+            df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
+
+    # all dataframes should now have the same length and level 1 columns
+    if len(all_columns) and all_columns[0].shape[1] == 2:
+        for i, columns in enumerate(all_columns):
+            if not columns[1].equals(all_columns[0][1]):
+                res = all_columns[0].merge(columns, indicator=True, how='outer')
+                raise RuntimeError(
+                    (
+                        "Cannot merge the data for {first} and {cur}.\n\n"
+                        + "The following columns are missing in {first}: {extra_cols}.\n\n"
+                        + "The following columns are missing in {cur}: {missing_cols}.\n\n"
+                        + "Please try to scrape the data again with caching disabled."
+                    ).format(
+                        first=dfs[0].loc[0, key].values,
+                        cur=dfs[i].loc[0, key].values,
+                        extra_cols=", ".join(
+                            map(
+                                str,
+                                res.loc[res['_merge'] == "left_only", [0, 1]]
+                                .to_records(index=False)
+                                .tolist(),
+                            )
+                        ),
+                        missing_cols=", ".join(
+                            map(
+                                str,
+                                res.loc[res['_merge'] == "right_only", [0, 1]]
+                                .to_records(index=False)
+                                .tolist(),
+                            )
+                        ),
+                    ),
+                )
+
+        # Step 2: Look for the most complete level 0 columns
+        columns = reduce(lambda left, right: left.combine_first(right), all_columns)
 
-    # Move the remaining missing columns back to level 1 and replace with empyt string
-    if columns.shape[1] == 2:
+        # Step 3: Make sure columns are consistent
         mask = pd.isnull(columns[0])
         columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
         columns.loc[mask, 1] = ""
+        column_idx = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
 
         for df in dfs:
-            df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
+            if df.columns.equals(column_idx):
+                # This dataframe already has the uniform column index
+                pass
+            elif len(df.columns) == len(column_idx):
+                # This dataframe has the same number of columns and the same
+                # level 1 columns, we assume that the level 0 columns can be
+                # replaced
+                df.columns = column_idx
 
     return pd.concat(dfs)
 
 
 def _fix_nation_col(df_table: pd.DataFrame) -> pd.DataFrame:
     """Fix the "Nation" column.
 
-    Removes the flag icon for domestic games and adds a 'nations' column for
-    international games based on the team's name.
+    Adds a 'nations' column for international games based on the team's name.
 
     Parameters
     ----------
     df_table : pd.DataFrame
         Input dataframe.
 
     Returns
     -------
     pd.DataFrame
     """
     if "Nation" not in df_table.columns.get_level_values(1):
         df_table.loc[:, (slice(None), "Squad")] = (
             df_table.xs("Squad", axis=1, level=1)
             .squeeze()
-            .apply(lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Squad" else None)
+            .apply(lambda x: x if isinstance(x, str) and x != "Squad" else None)
         )
         df_table.insert(
             2,
             ("Unnamed: nation", "Nation"),
             df_table.xs("Squad", axis=1, level=1).squeeze(),
         )
-    else:
-        df_table.loc[:, (slice(None), "Nation")] = (
-            df_table.xs("Nation", axis=1, level=1)
-            .squeeze(axis=1)
-            .apply(lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Nation" else None)
-        )
     return df_table
```

### Comparing `soccerdata-1.4.0/soccerdata/fivethirtyeight.py` & `soccerdata-1.5.0/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/soccerdata/match_history.py` & `soccerdata-1.5.0/soccerdata/match_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,30 +94,33 @@
             reader = self.get(url, filepath, no_cache=current_season)
 
             df_games = pd.read_csv(
                 reader,
                 encoding='ISO-8859-1',
             ).assign(season=skey)
             if 'Time' not in df_games.columns:
-                df_games['Time'] = "12:00:00"
-            df_games["Time"] = df_games["Time"].fillna("12:00:00")
+                df_games['Time'] = "12:00"
+            df_games["Time"] = df_games["Time"].fillna("12:00")
             df_list.append(df_games)
 
         df = (
             pd.concat(df_list, sort=False)
             .rename(columns=col_rename)
-            .assign(date=lambda x: pd.to_datetime(x["date"] + ' ' + x['time']))
+            .assign(
+                date=lambda x: pd.to_datetime(x["date"] + ' ' + x['time'], format="%d/%m/%Y %H:%M")
+            )
             .drop("time", axis=1)
             .pipe(self._translate_league)
             .replace(
                 {
                     'home_team': TEAMNAME_REPLACEMENTS,
                     'away_team': TEAMNAME_REPLACEMENTS,
                 }
             )
             .dropna(subset=['home_team', 'away_team'])
         )
 
+        df = df.loc[:, ~df.columns.str.contains('^Unnamed')]
         df['game'] = df.apply(make_game_id, axis=1)
         df.set_index(['league', 'season', 'game'], inplace=True)
         df.sort_index(inplace=True)
         return df
```

### Comparing `soccerdata-1.4.0/soccerdata/sofifa.py` & `soccerdata-1.5.0/soccerdata/sofifa.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.4.0/soccerdata/whoscored.py` & `soccerdata-1.5.0/soccerdata/whoscored.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Scraper for http://whoscored.com."""
 import itertools
 import json
+import re
 import time
 from datetime import datetime
 from pathlib import Path
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
@@ -280,15 +281,17 @@
         WebDriverWait(self._driver, 30, poll_frequency=1).until(
             ec.presence_of_element_located((By.XPATH, match_selector))
         )
         node_stages_selector = "//select[contains(@id,'stages')]/option"
         node_stages = self._driver.find_elements(By.XPATH, node_stages_selector)
         stages = []
         for stage in node_stages:
-            stages.append({"url": stage.get_attribute("value"), "name": stage.text})
+            if not re.search(r"Grp. ([A-Z])$", stage.text):
+                # there is always a page with all group stage games combined
+                stages.append({"url": stage.get_attribute("value"), "name": stage.text})
         return stages
 
     def _parse_schedule_page(self) -> Tuple[List[Dict], Optional[WebElement]]:
         match_selector = (
             "//div[contains(@id,'tournament-fixture')]//div[contains(@class,'divtable-row')]"
         )
         date_selector = "./div[contains(@class,'divtable-header')]"
@@ -350,15 +353,15 @@
                 self._handle_banner()
             # Parse next page
             page_schedule, next_page = self._parse_schedule_page()
             schedule.extend(page_schedule)
         schedule = [dict(item, stage=stage) for item in schedule]
         return schedule
 
-    def read_schedule(self, force_cache: bool = False) -> pd.DataFrame:
+    def read_schedule(self, force_cache: bool = False) -> pd.DataFrame:  # noqa: C901
         """Retrieve the game schedule for the selected leagues and seasons.
 
         Parameters
         ----------
         force_cache : bool
              By default no cached data is used for the current season.
              If True, will force the use of cached data anyway.
@@ -432,14 +435,17 @@
             else:
                 # Load cached data
                 logger.info("Retrieving game schedule of %s - %s from the cache", lkey, skey)
                 df_schedule = pd.read_csv(filepath)
 
             all_schedules.append(df_schedule)
 
+        if len(all_schedules) == 0:
+            return pd.DataFrame(index=["league", "season", "game"])
+
         # Construct the output dataframe
         df = (
             pd.concat(all_schedules)
             .drop_duplicates()
             .replace(
                 {
                     "home_team": TEAMNAME_REPLACEMENTS,
@@ -574,14 +580,18 @@
                         ),
                         "reason": node.xpath("./td[contains(@class,'reason')]/span")[0].get(
                             "title"
                         ),
                         "status": node.xpath("./td[contains(@class,'confirmed')]")[0].text,
                     }
                 )
+
+        if len(match_sheets) == 0:
+            return pd.DataFrame(index=["league", "season", "game", "team", "player"])
+
         df = (
             pd.DataFrame(match_sheets)
             .set_index(["league", "season", "game", "team", "player"])
             .sort_index()
         )
         return df
```

### Comparing `soccerdata-1.4.0/setup.py` & `soccerdata-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: soccerdata
+Version: 1.5.0
+Summary: A collection of wrappers over soccer data from various websites / APIs.
+Home-page: https://github.com/probberechts/soccerdata
+License: Apache-2.0
+Keywords: soccer,football,soccer data,web scraping,soccer analytics
+Author: Pieter Robberechts
+Author-email: pieter.robberechts@kuleuven.be
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PySocks (>=1.7.1,<2.0.0)
+Requires-Dist: Unidecode (>=1.2.0,<2.0.0)
+Requires-Dist: html5lib (>=1.1,<2.0)
+Requires-Dist: lxml (>=4.6,<5.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.23,<3.0)
+Requires-Dist: rich (>=13.0.0,<14.0.0)
+Requires-Dist: selenium (>=4.0.0,<5.0.0)
+Requires-Dist: undetected-chromedriver (>=3.1.3,<4.0.0)
+Requires-Dist: unicode (>=2.7,<3.0)
+Project-URL: Repository, https://github.com/probberechts/soccerdata
+Description-Content-Type: text/x-rst
+
+.. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png
+   :align: center
+   :alt: SoccerData
+   :width: 600px
+
+.. badges-begin
+
+|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov| |pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/soccerdata.svg
+   :target: https://pypi.org/project/soccerdata/
+   :alt: PyPI
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/soccerdata
+   :target: https://pypi.org/project/soccerdata
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/soccerdata.svg
+   :target: https://opensource.org/licenses/Apache-2.0
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/soccerdata/latest.svg?label=Read%20the%20Docs
+   :target: https://soccerdata.readthedocs.io/
+   :alt: Read the documentation at https://soccerdata.readthedocs.io/
+.. |Tests| image:: https://github.com/probberechts/soccerdata/workflows/CI/badge.svg
+   :target: https://github.com/probberechts/soccerdata/actions?workflow=CI
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/probberechts/soccerdata/branch/master/graph/badge.svg
+   :target: https://app.codecov.io/gh/probberechts/soccerdata
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. badges-end
+
+SoccerData is a collection of wrappers over soccer data from `Club Elo`_,
+`ESPN`_, `FBref`_, `FiveThirtyEight`_, `Football-Data.co.uk`_, `SoFIFA`_ and
+`WhoScored`_. You get Pandas DataFrames with sensible, matching column names
+and identifiers across datasets. Data is downloaded when needed and cached
+locally.
+
+.. code:: python
+
+   import soccerdata as sd
+
+   # Create scraper class instance for the Premier League
+   five38 = sd.FiveThirtyEight('ENG-Premier League', '1819')
+
+   # Fetch dataframes
+   games = five38.read_games()
+
+To learn how to install, configure and use SoccerData, see the
+`Quickstart guide <https://soccerdata.readthedocs.io/en/latest/usage.html>`__. For documentation on each of the
+supported data sources, see the `example notebooks <https://soccerdata.readthedocs.io/en/latest/datasources/>`__ and `API reference <https://soccerdata.readthedocs.io/en/latest/reference/>`__.
+
+.. _Club Elo: https://www.clubelo.com/
+.. _ESPN: https://www.espn.com/soccer/
+.. _FBref: https://www.fbref.com/en/
+.. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/
+.. _Football-Data.co.uk: https://www.football-data.co.uk/
+.. _SoFIFA: https://sofifa.com/
+.. _WhoScored: https://www.whoscored.com/
+
+**Disclaimer:** As soccerdata relies on web scraping, any changes to the
+scraped websites will break the package. Hence, do not expect that all code
+will work all the time. If you spot any bugs, then please `fork it and start
+a pull request <https://github.com/probberechts/soccerdata/blob/master/CONTRIBUTING.rst>`__.
 
-packages = \
-['soccerdata']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PySocks>=1.7.1,<2.0.0',
- 'Unidecode>=1.2.0,<2.0.0',
- 'html5lib>=1.1,<2.0',
- 'lxml>=4.6,<5.0',
- 'pandas>=1.0,<2.0',
- 'pretty-errors>=1.2.25,<2.0.0',
- 'requests>=2.23,<3.0',
- 'rich>=13.0.0,<14.0.0',
- 'selenium>=4.0.0,<5.0.0',
- 'undetected-chromedriver>=3.1.3,<4.0.0',
- 'unicode>=2.7,<3.0']
-
-setup_kwargs = {
-    'name': 'soccerdata',
-    'version': '1.4.0',
-    'description': 'A collection of wrappers over soccer data from various websites / APIs.',
-    'long_description': ".. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png\n   :align: center\n   :alt: SoccerData\n   :width: 600px\n\n.. badges-begin\n\n|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/soccerdata.svg\n   :target: https://pypi.org/project/soccerdata/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/soccerdata\n   :target: https://pypi.org/project/soccerdata\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/soccerdata.svg\n   :target: https://opensource.org/licenses/Apache-2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/soccerdata/latest.svg?label=Read%20the%20Docs\n   :target: https://soccerdata.readthedocs.io/\n   :alt: Read the documentation at https://soccerdata.readthedocs.io/\n.. |Tests| image:: https://github.com/probberechts/soccerdata/workflows/CI/badge.svg\n   :target: https://github.com/probberechts/soccerdata/actions?workflow=CI\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/probberechts/soccerdata/branch/master/graph/badge.svg\n   :target: https://app.codecov.io/gh/probberechts/soccerdata\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\nSoccerData is a collection of wrappers over soccer data from `Club Elo`_,\n`ESPN`_, `FBref`_, `FiveThirtyEight`_, `Football-Data.co.uk`_, `SoFIFA`_ and\n`WhoScored`_. You get Pandas DataFrames with sensible, matching column names\nand identifiers across datasets. Data is downloaded when needed and cached\nlocally.\n\n.. code:: python\n\n   import soccerdata as sd\n\n   # Create scraper class instance for the Premier League\n   five38 = sd.FiveThirtyEight('ENG-Premier League', '1819')\n\n   # Fetch dataframes\n   games = five38.read_games()\n\nTo learn how to install, configure and use SoccerData, see the\n`Quickstart guide <https://soccerdata.readthedocs.io/en/latest/usage.html>`__. For documentation on each of the\nsupported data sources, see the `example notebooks <https://soccerdata.readthedocs.io/en/latest/datasources/>`__ and `API reference <https://soccerdata.readthedocs.io/en/latest/reference/>`__.\n\n.. _Club Elo: https://www.clubelo.com/\n.. _ESPN: https://www.espn.com/soccer/\n.. _FBref: https://www.fbref.com/en/\n.. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/\n.. _Football-Data.co.uk: https://www.football-data.co.uk/\n.. _SoFIFA: https://sofifa.com/\n.. _WhoScored: https://www.whoscored.com/\n\n**Disclaimer:** As soccerdata relies on web scraping, any changes to the\nscraped websites will break the package. Hence, do not expect that all code\nwill work all the time. If you spot any bugs, then please `fork it and start\na pull request <https://github.com/probberechts/soccerdata/blob/master/CONTRIBUTING.rst>`__.\n",
-    'author': 'Pieter Robberechts',
-    'author_email': 'pieter.robberechts@kuleuven.be',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/probberechts/soccerdata',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

