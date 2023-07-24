# Comparing `tmp/streamingcommunity_unofficialapi-0.0.1.tar.gz` & `tmp/streamingcommunity_unofficialapi-0.0.2.tar.gz`

## Comparing `streamingcommunity_unofficialapi-0.0.1.tar` & `streamingcommunity_unofficialapi-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/SCuapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/LICENSE
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/README.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/SCuapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/README.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2/PKG-INFO
```

### Comparing `streamingcommunity_unofficialapi-0.0.1/SCuapi.py` & `streamingcommunity_unofficialapi-0.0.2/SCuapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,18 @@
         headers = {'user-agent': self.userAgent}
         main_url = requests.get(self.URL, headers=headers).url
         query_formatted = query.replace(" ", "%20")
         url = f"{main_url}api/search?q={query_formatted}"
         #print(url)
         document = requests.get(url, headers=headers)
         search_results = document.json()['data']
-        return [result for result in search_results]
+        for result in search_results:
+            result['url'] = f"{self.URL}/titles/{result['id']}-{result['slug']}"
+
+        return search_results #[result for result in search_results]
 
 
     def getLinkByIndex(self, search_result, index):
         link = f"{self.URL}/titles/{search_result[index]['id']}-{search_result[index]['slug']}"
         return link
 
 
@@ -42,14 +45,15 @@
 
 
         type = 'Movie' if datajs['type'] == 'movie' else 'TvSeries'
 
         year = datajs['release_date'].split('-')[0]
 
         pagedata = soup.find(id="app")["data-page"]
+        #print(pagedata)
         props = json.loads(pagedata)['props']
 
         trailer_info = props['title']['trailers']
         trailer_url = f"https://www.youtube.com/watch?v={trailer_info[0]['youtube_id']}" if trailer_info else None
         #print(trailer_url)
 
 
@@ -57,39 +61,51 @@
         size = min(len(correlates), 15)
         correlates_list = correlates[:size]
 
         plot = props['title']['plot']
 
         score = props['title']['score']
 
+        tmdb_id = props['title']['tmdb_id']
+        imdb_id = props['title']['imdb_id']
+        netflix_id = props['title']['netflix_id']
+        prime_id = props['title']['prime_id']
+        disney_id = props['title']['disney_id']
+        release_date = props['title']['release_date']
+        sub_ita = props['title']['sub_ita']
+
         if type == 'TvSeries':
 
             name = props['title']['name']
 
             seasons = props['title']['seasons']
 
+            seasons_count = int(props['title']['seasons_count'])
+
             episode_list = []
             for se in seasons:
                 season = int(se['number'])
                 document = requests.get(f'{url}/stagione-{season}', headers=headers)
                 soup = BeautifulSoup(document.content, 'html.parser')
                 pagedata = soup.find(id="app")["data-page"]
+                #print(pagedata)
                 episodes = json.loads(pagedata)['props']['loadedSeason']['episodes']
                 sid = se['title_id']
                 for ep in episodes:
                     scws_id = ep['scws_id']
                     href = f"{self.URL}/watch/{sid}?e={ep['id']}"
                     post_image = 'https://cdn.' + self.DOMAIN + '/images/' + ep['images'][0]['filename'] if ep['images'] else None
                     #print(post_image)
 
                     episode = {
                         'name': ep['name'],
                         'season': season,
                         'episode': int(ep['number']),
                         'description': ep['plot'],
+                        'duration': int(ep['duration']),
                         'posterUrl': post_image,
                         'url': href,
                         'scws_id': scws_id
                     }
                     episode_list.append(episode)
 
             if not episode_list:
@@ -99,28 +115,43 @@
                 'name': name,
                 'url': url,
                 'type': type,
                 'episodeList': episode_list,
                 'posterUrl': poster,
                 'year': int(''.join(filter(str.isdigit, year))),
                 'plot': plot,
+                'tmdb_id': tmdb_id,
+                'imdb_id': imdb_id,
+                'netflix_id': netflix_id,
+                'prime_id': prime_id,
+                'disney_id': disney_id,
+                'release_date': release_date,
+                'sub_ita': bool(sub_ita),
                 'rating': int(float(score) * 1000),
+                'seasons_count': seasons_count,
                 'tags': [genre['name'] for genre in datajs['genres']],
                 'trailerUrl': trailer_url,
                 'recommendations': correlates_list
             }
         else:
             return {
                 'name': soup.select_one("div > div > h1").text,
                 'url': f"{self.URL}/watch/{props['title']['id']}",
                 'scws_id': props['title']['scws_id'],
                 'type': type,
                 'posterUrl': poster,
                 'year': int(''.join(filter(str.isdigit, year))),
                 'plot': plot,
+                'tmdb_id': tmdb_id,
+                'imdb_id': imdb_id,
+                'netflix_id': netflix_id,
+                'prime_id': prime_id,
+                'disney_id': disney_id,
+                'release_date': release_date,
+                'sub_ita': bool(sub_ita),
                 'rating': int(float(score) * 1000),
                 'tags': [genre['name'] for genre in datajs['genres']],
                 'duration': int(props['title']['runtime']),
                 'trailerUrl': trailer_url,
                 'recommendations': correlates_list
             }
 
@@ -165,9 +196,7 @@
             link = f'https://vixcloud.co/v2/playlist/{scwsid}?token={token}&token480p={token}&expires={expire}&n=1'
                     #https://vixcloud.co/v2/playlist/159536?token=t5OmJHPGf9Ti3DXdd0l_AQ&token360p=&token480p=cEjEiuArJcYsrbPzksSQTQ&token720p=n-00eKBvOxqRh0ISQjbu3Q&token1080p=&expires=1695317130&canCast=1&n=1&b=1
 
             #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=&expires=1695316859&canCast=1&b=1&n=1
             #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=HjLZ1Qbx0oNt7u7DbDHM3w&expires=1690305563&n=1
 
             return link
-
-
```

### Comparing `streamingcommunity_unofficialapi-0.0.1/LICENSE` & `streamingcommunity_unofficialapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcommunity_unofficialapi-0.0.1/pyproject.toml` & `streamingcommunity_unofficialapi-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "streamingcommunity-unofficialapi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Beqir Stafa", email="beqirstafa@gmail.com" },
 ]
 description = "A simple unofficial api for the italian StreamingCommunity website"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

