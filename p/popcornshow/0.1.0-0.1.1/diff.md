# Comparing `tmp/popcornshow-0.1.0.tar.gz` & `tmp/popcornshow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popcornshow-0.1.0.tar", max compression
+gzip compressed data, was "popcornshow-0.1.1.tar", max compression
```

## Comparing `popcornshow-0.1.0.tar` & `popcornshow-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       30 2023-07-16 06:40:25.287069 popcornshow-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-08 04:34:41.268232 popcornshow-0.1.0/popcorn/__init__.py
--rw-r--r--   0        0        0     7672 2023-07-09 04:14:08.738462 popcornshow-0.1.0/popcorn/api/api.py
--rw-r--r--   0        0        0      448 2023-07-08 20:30:49.768143 popcornshow-0.1.0/popcorn/api/models/PersonApi.py
--rw-r--r--   0        0        0      182 2023-07-08 19:58:56.355271 popcornshow-0.1.0/popcorn/api/models/Result.py
--rw-r--r--   0        0        0     3418 2023-07-08 20:30:49.783769 popcornshow-0.1.0/popcorn/api/models/SearchApi.py
--rw-r--r--   0        0        0     8192 2023-07-17 02:03:01.016953 popcornshow-0.1.0/popcorn/cli.py
--rw-r--r--   0        0        0       35 2023-07-08 19:57:50.362411 popcornshow-0.1.0/popcorn/config.py
--rw-r--r--   0        0        0     2596 2023-07-17 02:03:01.016953 popcornshow-0.1.0/popcorn/controller.py
--rw-r--r--   0        0        0      619 2023-07-17 02:03:01.017951 popcornshow-0.1.0/popcorn/dto.py
--rw-r--r--   0        0        0      291 2023-03-16 02:28:48.138564 popcornshow-0.1.0/popcorn/models/AlsoWatched.py
--rw-r--r--   0        0        0      394 2023-07-08 20:30:49.785775 popcornshow-0.1.0/popcorn/models/Content.py
--rw-r--r--   0        0        0      967 2023-07-08 19:58:56.402579 popcornshow-0.1.0/popcorn/models/Creative.py
--rw-r--r--   0        0        0      115 2023-07-08 19:58:56.402579 popcornshow-0.1.0/popcorn/models/Ios.py
--rw-r--r--   0        0        0     8032 2023-07-17 02:03:01.017951 popcornshow-0.1.0/popcorn/models/ItemMovie.py
--rw-r--r--   0        0        0     8300 2023-07-17 02:03:01.018953 popcornshow-0.1.0/popcorn/models/ItemShow.py
--rw-r--r--   0        0        0      282 2023-07-08 19:58:56.355271 popcornshow-0.1.0/popcorn/models/Links.py
--rw-r--r--   0        0        0      246 2023-03-16 02:25:09.533167 popcornshow-0.1.0/popcorn/models/ListingKey.py
--rw-r--r--   0        0        0      118 2023-07-08 19:58:56.355271 popcornshow-0.1.0/popcorn/models/Metadata.py
--rw-r--r--   0        0        0      847 2023-07-08 20:30:49.815419 popcornshow-0.1.0/popcorn/models/Person.py
--rw-r--r--   0        0        0      300 2023-07-08 19:58:56.370912 popcornshow-0.1.0/popcorn/models/Rank.py
--rw-r--r--   0        0        0      578 2023-07-08 19:58:56.380927 popcornshow-0.1.0/popcorn/models/ReelgoodScores.py
--rw-r--r--   0        0        0      601 2023-07-08 19:58:56.386939 popcornshow-0.1.0/popcorn/models/RegionalAvailability.py
--rw-r--r--   0        0        0      354 2023-07-08 20:30:49.815419 popcornshow-0.1.0/popcorn/models/ScoreBreakdown.py
--rw-r--r--   0        0        0      903 2023-07-17 02:03:01.018953 popcornshow-0.1.0/popcorn/models/Search.py
--rw-r--r--   0        0        0      832 2023-07-08 19:58:56.386939 popcornshow-0.1.0/popcorn/models/Seasons.py
--rw-r--r--   0        0        0     1770 2023-07-08 20:30:49.831042 popcornshow-0.1.0/popcorn/models/SourceAdPlacement.py
--rw-r--r--   0        0        0      161 2023-07-08 19:58:56.386939 popcornshow-0.1.0/popcorn/models/Streamability.py
--rw-r--r--   0        0        0      183 2023-07-08 19:58:56.386939 popcornshow-0.1.0/popcorn/models/Tag.py
--rw-r--r--   0        0        0      206 2023-07-08 19:58:56.386939 popcornshow-0.1.0/popcorn/models/Trailer.py
--rw-r--r--   0        0        0     3452 2023-03-25 22:50:45.329984 popcornshow-0.1.0/popcorn/models/TVShowEpisode.py
--rw-r--r--   0        0        0     1951 2023-07-17 02:03:01.019953 popcornshow-0.1.0/popcorn/tables/people.py
--rw-r--r--   0        0        0     5478 2023-07-17 02:03:01.019953 popcornshow-0.1.0/popcorn/tables/sources.py
--rw-r--r--   0        0        0     1473 2023-07-17 02:03:01.020951 popcornshow-0.1.0/popcorn/tables/table_details_movie.py
--rw-r--r--   0        0        0     1221 2023-07-17 02:03:01.020951 popcornshow-0.1.0/popcorn/tables/table_person.py
--rw-r--r--   0        0        0     1321 2023-07-17 02:03:01.021952 popcornshow-0.1.0/popcorn/tables/table_search.py
--rw-r--r--   0        0        0     1243 2023-07-08 20:30:49.846667 popcornshow-0.1.0/popcorn/tables/tableDetailsShow.py
--rw-r--r--   0        0        0      357 2023-07-08 19:58:56.418205 popcornshow-0.1.0/popcorn/tables/TableInterface.py
--rw-r--r--   0        0        0     2376 2023-07-17 02:03:01.021952 popcornshow-0.1.0/popcorn/utils.py
--rw-r--r--   0        0        0     1672 2023-07-21 01:33:42.400354 popcornshow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2077 2023-07-20 23:28:18.956278 popcornshow-0.1.0/README.md
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 popcornshow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-16 06:40:25.287069 popcornshow-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-08 04:34:41.268232 popcornshow-0.1.1/popcorn/__init__.py
+-rw-r--r--   0        0        0     7672 2023-07-09 04:14:08.738462 popcornshow-0.1.1/popcorn/api/api.py
+-rw-r--r--   0        0        0      448 2023-07-08 20:30:49.768143 popcornshow-0.1.1/popcorn/api/models/PersonApi.py
+-rw-r--r--   0        0        0      182 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/api/models/Result.py
+-rw-r--r--   0        0        0     3418 2023-07-08 20:30:49.783769 popcornshow-0.1.1/popcorn/api/models/SearchApi.py
+-rw-r--r--   0        0        0     8167 2023-07-24 21:45:48.324416 popcornshow-0.1.1/popcorn/cli.py
+-rw-r--r--   0        0        0       35 2023-07-08 19:57:50.362411 popcornshow-0.1.1/popcorn/config.py
+-rw-r--r--   0        0        0     2596 2023-07-17 02:03:01.016953 popcornshow-0.1.1/popcorn/controller.py
+-rw-r--r--   0        0        0      619 2023-07-17 02:03:01.017951 popcornshow-0.1.1/popcorn/dto.py
+-rw-r--r--   0        0        0      291 2023-03-16 02:28:48.138564 popcornshow-0.1.1/popcorn/models/AlsoWatched.py
+-rw-r--r--   0        0        0      394 2023-07-08 20:30:49.785775 popcornshow-0.1.1/popcorn/models/Content.py
+-rw-r--r--   0        0        0      967 2023-07-08 19:58:56.402579 popcornshow-0.1.1/popcorn/models/Creative.py
+-rw-r--r--   0        0        0      115 2023-07-08 19:58:56.402579 popcornshow-0.1.1/popcorn/models/Ios.py
+-rw-r--r--   0        0        0     8032 2023-07-17 02:03:01.017951 popcornshow-0.1.1/popcorn/models/ItemMovie.py
+-rw-r--r--   0        0        0     8300 2023-07-17 02:03:01.018953 popcornshow-0.1.1/popcorn/models/ItemShow.py
+-rw-r--r--   0        0        0      282 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/models/Links.py
+-rw-r--r--   0        0        0      246 2023-03-16 02:25:09.533167 popcornshow-0.1.1/popcorn/models/ListingKey.py
+-rw-r--r--   0        0        0      118 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/models/Metadata.py
+-rw-r--r--   0        0        0      847 2023-07-08 20:30:49.815419 popcornshow-0.1.1/popcorn/models/Person.py
+-rw-r--r--   0        0        0      300 2023-07-08 19:58:56.370912 popcornshow-0.1.1/popcorn/models/Rank.py
+-rw-r--r--   0        0        0      578 2023-07-08 19:58:56.380927 popcornshow-0.1.1/popcorn/models/ReelgoodScores.py
+-rw-r--r--   0        0        0      601 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/RegionalAvailability.py
+-rw-r--r--   0        0        0      354 2023-07-08 20:30:49.815419 popcornshow-0.1.1/popcorn/models/ScoreBreakdown.py
+-rw-r--r--   0        0        0      903 2023-07-17 02:03:01.018953 popcornshow-0.1.1/popcorn/models/Search.py
+-rw-r--r--   0        0        0      832 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Seasons.py
+-rw-r--r--   0        0        0     1770 2023-07-08 20:30:49.831042 popcornshow-0.1.1/popcorn/models/SourceAdPlacement.py
+-rw-r--r--   0        0        0      161 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Streamability.py
+-rw-r--r--   0        0        0      183 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Tag.py
+-rw-r--r--   0        0        0      206 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Trailer.py
+-rw-r--r--   0        0        0     3452 2023-03-25 22:50:45.329984 popcornshow-0.1.1/popcorn/models/TVShowEpisode.py
+-rw-r--r--   0        0        0     1951 2023-07-17 02:03:01.019953 popcornshow-0.1.1/popcorn/tables/people.py
+-rw-r--r--   0        0        0     5478 2023-07-17 02:03:01.019953 popcornshow-0.1.1/popcorn/tables/sources.py
+-rw-r--r--   0        0        0     1473 2023-07-17 02:03:01.020951 popcornshow-0.1.1/popcorn/tables/table_details_movie.py
+-rw-r--r--   0        0        0     1221 2023-07-17 02:03:01.020951 popcornshow-0.1.1/popcorn/tables/table_person.py
+-rw-r--r--   0        0        0     1321 2023-07-17 02:03:01.021952 popcornshow-0.1.1/popcorn/tables/table_search.py
+-rw-r--r--   0        0        0     1243 2023-07-08 20:30:49.846667 popcornshow-0.1.1/popcorn/tables/tableDetailsShow.py
+-rw-r--r--   0        0        0      357 2023-07-08 19:58:56.418205 popcornshow-0.1.1/popcorn/tables/TableInterface.py
+-rw-r--r--   0        0        0     2376 2023-07-17 02:03:01.021952 popcornshow-0.1.1/popcorn/utils.py
+-rw-r--r--   0        0        0     1672 2023-07-24 21:48:16.190210 popcornshow-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2287 2023-07-22 21:17:14.185532 popcornshow-0.1.1/README.md
+-rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 popcornshow-0.1.1/PKG-INFO
```

### Comparing `popcornshow-0.1.0/popcorn/api/api.py` & `popcornshow-0.1.1/popcorn/api/api.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/api/models/SearchApi.py` & `popcornshow-0.1.1/popcorn/api/models/SearchApi.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/cli.py` & `popcornshow-0.1.1/popcorn/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 from rich.prompt import Prompt
 from rich.table import Table
 from rich.tree import Tree
 
 from popcorn.api.models.PersonApi import PersonApi
 from popcorn.api.models.Result import Result
 from popcorn.api.models.SearchApi import Item
-from popcorn.controller import person_reel, search_reel, transform_item
+from popcorn.controller import person_reel, searchReel, transformItem
 from popcorn.models.ItemMovie import ItemMovie
 from popcorn.models.ItemShow import ItemShow
 from popcorn.models.Person import Person
 from popcorn.models.Search import Search
 from popcorn.tables.people import people, people_biography, person_media
-from popcorn.tables.sources import collumn_seasons, pop_collumns
+from popcorn.tables.sources import columns, columnsSeasons
 from popcorn.tables.table_details_movie import table_details
 from popcorn.tables.table_person import table_details_person
-from popcorn.tables.table_search import table_search
+from popcorn.tables.table_search import tableSearch
 from popcorn.tables.tableDetailsShow import table_details_show
-from popcorn.utils import format_date
+from popcorn.utils import formatDate
 
 app = typer.Typer(help="PopCorn Show")
 console = Console()
 
 
 @app.command(name="search")
 def search(
     name: str,
     year: int = typer.Option(None, "--year", "-y", help="type Year"),
     type: str = typer.Option(None, "--type", "-t", help="'m' or 's'"),
     luck: bool = typer.Option(False, "--luck", "-l"),
 ):
-    list = search_reel(name, year=year, type=type)
+    list = searchReel(name, year=year, type=type)
     if list:
         if luck:
             order = sorted(list, key=lambda x: x.imdbStr(), reverse=True)
-            result = transform_item(order[0].slug, order[0].type)
+            result = transformItem(order[0].slug, order[0].type)
             chooseTypes(result)
         else:
-            console.print(table_search(list))
-            choose_number(list)
+            console.print(tableSearch(list))
+            chooseNumber(list)
     else:
         typer.echo("Not Found")
 
 
 def person(name: str):
     result: Result = person_reel(name)
     if result.error is None:
@@ -69,15 +69,15 @@
         __showTvshow(result.value)
 
 
 def __showTvshow(show: ItemShow):
     tree = Tree("")
     tree.add(__rich__())
     details = Tree(
-        f":blue_book: [blue][b]Details - {show.title} {format_date(show.released_on).year}[/b] - :link: [blue][link={show.createUrl()}]Details in Reelgood.com[/link]",
+        f":blue_book: [blue][b]Details - {show.title} {formatDate(show.released_on).year}[/b] - :link: [blue][link={show.createUrl()}]Details in Reelgood.com[/link]",
         expanded=True,
     )
     details.add(table_details_show(show), highlight=False)
 
     person = Tree(":busts_in_silhouette:[bold][purple] People")
     person.add(people(show.people))
 
@@ -85,15 +85,15 @@
     if person.children.__len__() > 0:
         tree.add(person)
     if show.seasons.__len__() > 0:
         tv = Tree(
             f":movie_camera: [red][b]Where to Watch: {show.title} [/red]| [yellow]With Season {show.seasons.__len__()}"
         )
         tv.add(
-            collumn_seasons(show.episodes, reversed(show.seasons)),
+            columnsSeasons(show.episodes, reversed(show.seasons)),
             expanded=True,
             highlight=False,
         )
         tree.add(tv)
     tree.add(__footer__(show))
     console.print(tree)
 
@@ -101,28 +101,28 @@
         __choosePerson(show.people)
 
 
 def __showMovie(movie: ItemMovie):
     tree = Tree("")
     tree.add(__rich__())
     details = Tree(
-        f":blue_book:[blue][b] Details - {movie.title} {format_date(movie.released_on).year if format_date(movie.released_on) != None else '-- --'}[/b] - :link: [blue][link={movie.createUrl()}]Details in Reelgood.com[/link]",
+        f":blue_book:[blue][b] Details - {movie.title} {formatDate(movie.released_on).year if formatDate(movie.released_on) != None else '-- --'}[/b] - :link: [blue][link={movie.createUrl()}]Details in Reelgood.com[/link]",
         expanded=True,
     )
     details.add(table_details(movie), highlight=False)
 
     person = Tree(":busts_in_silhouette:[bold][purple] People")
     person.add(people(movie.people))
 
     tree.add(details)
     if person.children.__len__() > 0:
         tree.add(person)
     if movie.availability:
         tv = Tree(f":movie_camera:[red][b] Where to Watch: {movie.title}")
-        tv.add(pop_collumns(movie.availability), expanded=True, highlight=False)
+        tv.add(columns(movie.availability), expanded=True, highlight=False)
         tree.add(tv)
     tree.add(__footer__(movie))
     console.print(tree)
     if movie.people.__len__() > 0:
         __choosePerson(movie.people)
 
 
@@ -166,16 +166,16 @@
         + "[red]for details - Zero to exit\n"
     )
     try:
         value = int(number)
         if value < 1:
             return
         item: Item = person.initial_credits[value - 1]
-        media: Result = trabsform_item(item["slug"], item["content_type"])
-        oseTypes(media)
+        media: Result = transformItem(item["slug"], item["content_type"])
+        chooseTypes(media)
     except (IndexError, ValueError):
         choose_media_by_person(person)
 
 
 def __rich__() -> Panel:
     grid = Table.grid(expand=True)
     grid.add_column(justify="center", ratio=1)
@@ -214,32 +214,32 @@
         grid.add_row(
             "",
             f"[b][link=https://play.google.com/store/apps/details?id=br.com.icaro.filme][yellow]App Android => [/link]",
         )
     return Panel(grid, style="red1 on black")
 
 
-def choose_number(list: list[Search], hasError=False):
+def chooseNumber(list: list[Search], hasError=False):
     item: None
     number = Prompt.ask(
         f"[red]For details, write a number between 1 and {list.__len__()}. Zero to exit\n"
     )
     if hasError or number == "0":
         return
 
     try:
         number = int(number)
         if number > 0 and number <= list.__len__():
             item = list[number - 1]
         else:
             print("Number off the list.")
-            choose_number(list, True)
+            chooseNumber(list, True)
             return
 
     except ValueError:
         print("Number Error! - write '0' to exit ")
-        choose_number(list, True)
+        chooseNumber(list, True)
         return
 
     if item is not None:
-        result = transform_item(item.slug, item.type)
+        result = transformItem(item.slug, item.type)
         fillByType(result)
```

### Comparing `popcornshow-0.1.0/popcorn/controller.py` & `popcornshow-0.1.1/popcorn/controller.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/dto.py` & `popcornshow-0.1.1/popcorn/dto.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/Creative.py` & `popcornshow-0.1.1/popcorn/models/Creative.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/ItemMovie.py` & `popcornshow-0.1.1/popcorn/models/ItemMovie.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/ItemShow.py` & `popcornshow-0.1.1/popcorn/models/ItemShow.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/Person.py` & `popcornshow-0.1.1/popcorn/models/Person.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/ReelgoodScores.py` & `popcornshow-0.1.1/popcorn/models/ReelgoodScores.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/RegionalAvailability.py` & `popcornshow-0.1.1/popcorn/models/RegionalAvailability.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/Search.py` & `popcornshow-0.1.1/popcorn/models/Search.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/Seasons.py` & `popcornshow-0.1.1/popcorn/models/Seasons.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/SourceAdPlacement.py` & `popcornshow-0.1.1/popcorn/models/SourceAdPlacement.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/models/TVShowEpisode.py` & `popcornshow-0.1.1/popcorn/models/TVShowEpisode.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/people.py` & `popcornshow-0.1.1/popcorn/tables/people.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/sources.py` & `popcornshow-0.1.1/popcorn/tables/sources.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/table_details_movie.py` & `popcornshow-0.1.1/popcorn/tables/table_details_movie.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/table_person.py` & `popcornshow-0.1.1/popcorn/tables/table_person.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/table_search.py` & `popcornshow-0.1.1/popcorn/tables/table_search.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/tables/tableDetailsShow.py` & `popcornshow-0.1.1/popcorn/tables/tableDetailsShow.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/popcorn/utils.py` & `popcornshow-0.1.1/popcorn/utils.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.0/pyproject.toml` & `popcornshow-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "popcornshow"
 packages = [{include = "popcorn"}]
-version = "0.1.0"
+version = "0.1.1"
 description = "Show information about movie and movies"
 authors = ["Icaro Nunes <icarornunes@gmail.com>"]
 license = "BeerWare"
 readme = "README.md"
 classifiers = [
   "Topic :: Utilities",
   "Programming Language :: Python :: 3"
```

### Comparing `popcornshow-0.1.0/README.md` & `popcornshow-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 ### 🍿🍿🍿 Popcorn Show CLI 🍿🍿🍿
 
 [![Documentation Status](https://readthedocs.org/projects/popcornshow-cli/badge/?version=latest)](https://popcornshow-cli.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/icaronunes/popcornshow-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/icaronunes/popcornshow-cli/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/icaronunes/popcornshow-cli/branch/master/graph/badge.svg?token=OL7MWQKQKR)](https://codecov.io/gh/icaronunes/popcornshow-cli)
 
-CLI com o objetivo de obter informações sobre filmes/séries e pessoas envolvidas na produção via terminal.
-Apresentando as informações mais relevantes diretamente no seu terminal.
+CLI with the objective of obtaining information about movies/series and people involved in production via the terminal.
+Presenting the most relevant information directly on your terminal.
 
-- nome
-- link para streming
-- datas
-- elenco/produção
-- trailer
-- notas do IMDB
-- resumo da obra
+- Title
+- Streaming link
+- Dates
+- Cast/Crew
+- Trailer
+- IMDB ratings
+- Summary
 
-possibilidade de navegar entre pessoas e obras
+Ability to navigate between people and works.
 
-## Instalação
+## Installation
 
-```` bash
+```bash
 pip install popcornshow
-````
-## Prints
+```
 
-**Busca** 
-![]()
+**Search** 
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/cli_search.png)
 
-**Filmes**
-![](docs/assets/show_movie.png)  
+**Movies**
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/show_movie.png)  
 
-**Séries**
-![](docs/assets/show_serie.png)  
+**Shows**
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/show_serie.png)  
 
-**Pessoa**
-![](docs/assets/person.png)
+**Person**
+ci![](https://popcornshow-cli.readthedocs.io/en/latest/assets/person.png)
 
-## Comandos para usar
+## Commands to use
 
-* `popcornshow [nome do filme ou serie]` - Busca por uma lista que corresponde a texto enviada.
-* `popcornshow --year -y [2000]` - Busca por uma midia com esse ano de lançamento.
-* `popcornshow --type -t [m] [s]` - Busca por apenas o tipo escolhido. Filme ou Série.
-* `popcornshow  -l --luck` - Retorna/escolhe a primeira opção retornada pela busca.
-* `popcornshow -h` - Mostra a tela de Ajuda padrão.
+* popcornshow [movie or series name] - Search for a list that matches the given text.
 
-* em cada tela, pode haver uma opção de navegação
+* popcornshow --year -y [2000] - Search for media released in a specific year.
 
-![](docs/assets/help.png)
+* popcornshow --type -t [m] [s] - Search for media of a specific type. Movie or Series.
 
-## Sobre
-Documentação do [ReadTheDocs](https://popcornshow-cli.readthedocs.io/en/latest/?)
+* popcornshow -l --luck - Return/choose the first option returned by the search.
 
+* popcornshow -h - Show the default Help screen.
 
-Aplicação feita 100% em python
+#### on each screen, there might be a navigation option
 
-Informações obtidas do site [RealGood](https://reelgood.com/)
 
-<img src=docs/assets/android.png width=120px />Há uma versão mais completa para Android: [play.google.com/popcornshow](https://play.google.com/store/apps/details?id=br.com.icaro.filme) ![alt text](docs/assets/popcorn.png)
+## About
+Documentation on [ReadTheDocs](https://popcornshow-cli.readthedocs.io/en/latest/?)
+
+Application made 100% in Python
+
+Information obtained from [RealGood](https://reelgood.com/)
+
+<img src=https://popcornshow-cli.readthedocs.io/en/latest/assets/android.svg width=50px />There is a more comprehensive version for Android: [play.google.com/popcornshow](https://play.google.com/store/apps/details?id=br.com.icaro.filme) ![alt text](https://popcornshow-cli.readthedocs.io/en/latest/assets/popcorn.png)
```

### Comparing `popcornshow-0.1.0/PKG-INFO` & `popcornshow-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popcornshow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Show information about movie and movies
 License: Beerware
 Author: Icaro Nunes
 Author-email: icarornunes@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -24,61 +24,61 @@
 
 ### 🍿🍿🍿 Popcorn Show CLI 🍿🍿🍿
 
 [![Documentation Status](https://readthedocs.org/projects/popcornshow-cli/badge/?version=latest)](https://popcornshow-cli.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/icaronunes/popcornshow-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/icaronunes/popcornshow-cli/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/icaronunes/popcornshow-cli/branch/master/graph/badge.svg?token=OL7MWQKQKR)](https://codecov.io/gh/icaronunes/popcornshow-cli)
 
-CLI com o objetivo de obter informações sobre filmes/séries e pessoas envolvidas na produção via terminal.
-Apresentando as informações mais relevantes diretamente no seu terminal.
+CLI with the objective of obtaining information about movies/series and people involved in production via the terminal.
+Presenting the most relevant information directly on your terminal.
 
-- nome
-- link para streming
-- datas
-- elenco/produção
-- trailer
-- notas do IMDB
-- resumo da obra
+- Title
+- Streaming link
+- Dates
+- Cast/Crew
+- Trailer
+- IMDB ratings
+- Summary
 
-possibilidade de navegar entre pessoas e obras
+Ability to navigate between people and works.
 
-## Instalação
+## Installation
 
-```` bash
+```bash
 pip install popcornshow
-````
-## Prints
+```
 
-**Busca** 
-![]()
+**Search** 
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/cli_search.png)
 
-**Filmes**
-![](docs/assets/show_movie.png)  
+**Movies**
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/show_movie.png)  
 
-**Séries**
-![](docs/assets/show_serie.png)  
+**Shows**
+![](https://popcornshow-cli.readthedocs.io/en/latest/assets/show_serie.png)  
 
-**Pessoa**
-![](docs/assets/person.png)
+**Person**
+ci![](https://popcornshow-cli.readthedocs.io/en/latest/assets/person.png)
 
-## Comandos para usar
+## Commands to use
 
-* `popcornshow [nome do filme ou serie]` - Busca por uma lista que corresponde a texto enviada.
-* `popcornshow --year -y [2000]` - Busca por uma midia com esse ano de lançamento.
-* `popcornshow --type -t [m] [s]` - Busca por apenas o tipo escolhido. Filme ou Série.
-* `popcornshow  -l --luck` - Retorna/escolhe a primeira opção retornada pela busca.
-* `popcornshow -h` - Mostra a tela de Ajuda padrão.
+* popcornshow [movie or series name] - Search for a list that matches the given text.
 
-* em cada tela, pode haver uma opção de navegação
+* popcornshow --year -y [2000] - Search for media released in a specific year.
 
-![](docs/assets/help.png)
+* popcornshow --type -t [m] [s] - Search for media of a specific type. Movie or Series.
 
-## Sobre
-Documentação do [ReadTheDocs](https://popcornshow-cli.readthedocs.io/en/latest/?)
+* popcornshow -l --luck - Return/choose the first option returned by the search.
 
+* popcornshow -h - Show the default Help screen.
 
-Aplicação feita 100% em python
+#### on each screen, there might be a navigation option
 
-Informações obtidas do site [RealGood](https://reelgood.com/)
 
-<img src=docs/assets/android.png width=120px />Há uma versão mais completa para Android: [play.google.com/popcornshow](https://play.google.com/store/apps/details?id=br.com.icaro.filme) ![alt text](docs/assets/popcorn.png)
+## About
+Documentation on [ReadTheDocs](https://popcornshow-cli.readthedocs.io/en/latest/?)
 
+Application made 100% in Python
+
+Information obtained from [RealGood](https://reelgood.com/)
+
+<img src=https://popcornshow-cli.readthedocs.io/en/latest/assets/android.svg width=50px />There is a more comprehensive version for Android: [play.google.com/popcornshow](https://play.google.com/store/apps/details?id=br.com.icaro.filme) ![alt text](https://popcornshow-cli.readthedocs.io/en/latest/assets/popcorn.png)
```

