# Comparing `tmp/streamingcommunity_unofficialapi-0.0.2.1.tar.gz` & `tmp/streamingcommunity_unofficialapi-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "streamingcommunity_unofficialapi-0.0.3.1.tar", last modified: Mon Jul 24 12:57:15 2023, max compression
```

## Comparing `streamingcommunity_unofficialapi-0.0.2.1.tar` & `streamingcommunity_unofficialapi-0.0.3.1.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/SCuapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/README.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 streamingcommunity_unofficialapi-0.0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:57:15.434737 streamingcommunity_unofficialapi-0.0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 12:56:54.000000 streamingcommunity_unofficialapi-0.0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 12:57:15.434737 streamingcommunity_unofficialapi-0.0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-24 12:56:54.000000 streamingcommunity_unofficialapi-0.0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:57:15.434737 streamingcommunity_unofficialapi-0.0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 12:56:54.000000 streamingcommunity_unofficialapi-0.0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:57:15.430737 streamingcommunity_unofficialapi-0.0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:56:54.000000 streamingcommunity_unofficialapi-0.0.3.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-24 12:56:54.000000 streamingcommunity_unofficialapi-0.0.3.1/src/scuapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:57:15.434737 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 12:57:15.000000 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 12:57:15.000000 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:57:15.000000 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 12:57:15.000000 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 12:57:15.000000 streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/top_level.txt
```

### Comparing `streamingcommunity_unofficialapi-0.0.2.1/SCuapi.py` & `streamingcommunity_unofficialapi-0.0.3.1/src/scuapi.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-import requests
-from bs4 import BeautifulSoup
-import time
-import hashlib
-import base64
-import json
-import re
-
-
-#streamingcommunity bet
-
-class SCAPI:
-    def __init__(self, DOMAIN, userAgent="Mozilla/5.0 (Windows NT 11.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"):
-        self.userAgent = userAgent
-        self.DOMAIN = DOMAIN
-        self.URL = 'https://' + self.DOMAIN
-
-    def search(self, query):
-        headers = {'user-agent': self.userAgent}
-        main_url = requests.get(self.URL, headers=headers).url
-        query_formatted = query.replace(" ", "%20")
-        url = f"{main_url}api/search?q={query_formatted}"
-        #print(url)
-        document = requests.get(url, headers=headers)
-        search_results = document.json()['data']
-        #print(search_results)
-        output_dict = {}
-        for result in search_results:
-            result['url'] = f"{self.URL}/titles/{result['id']}-{result['slug']}"
-            output_dict[result['name']] = result
-
-        return output_dict #[result for result in search_results]
-
-
-    def load(self, url):
-        headers = {'user-agent': self.userAgent}
-        document = requests.get(url, headers=headers)
-        soup = BeautifulSoup(document.content, 'html.parser')
-        poster = re.search("url\((.*)\)", soup.find("div", class_="title-container")['style']).group(1)
-        #print(poster)
-        id = ''.join(filter(str.isdigit, url.split('-')[0]))
-        datajs = requests.post(f"{self.URL}/api/titles/preview/{id}", headers=headers).json()
-
-
-        type = 'Movie' if datajs['type'] == 'movie' else 'TvSeries'
-
-        year = datajs['release_date'].split('-')[0]
-
-        pagedata = soup.find(id="app")["data-page"]
-        #print(pagedata)
-        props = json.loads(pagedata)['props']
-
-        trailer_info = props['title']['trailers']
-        trailer_url = f"https://www.youtube.com/watch?v={trailer_info[0]['youtube_id']}" if trailer_info else None
-        #print(trailer_url)
-
-
-        correlates = props['sliders'][0]['titles']
-        size = min(len(correlates), 15)
-        correlates_list = correlates[:size]
-
-        plot = props['title']['plot']
-
-        score = props['title']['score']
-
-        tmdb_id = props['title']['tmdb_id']
-        imdb_id = props['title']['imdb_id']
-        netflix_id = props['title']['netflix_id']
-        prime_id = props['title']['prime_id']
-        disney_id = props['title']['disney_id']
-        release_date = props['title']['release_date']
-        sub_ita = props['title']['sub_ita']
-
-        if type == 'TvSeries':
-
-            name = props['title']['name']
-
-            seasons = props['title']['seasons']
-
-            seasons_count = int(props['title']['seasons_count'])
-
-            episode_list = []
-            for se in seasons:
-                season = int(se['number'])
-                document = requests.get(f'{url}/stagione-{season}', headers=headers)
-                soup = BeautifulSoup(document.content, 'html.parser')
-                pagedata = soup.find(id="app")["data-page"]
-                #print(pagedata)
-                episodes = json.loads(pagedata)['props']['loadedSeason']['episodes']
-                sid = se['title_id']
-                for ep in episodes:
-                    scws_id = ep['scws_id']
-                    href = f"{self.URL}/watch/{sid}?e={ep['id']}"
-                    post_image = 'https://cdn.' + self.DOMAIN + '/images/' + ep['images'][0]['filename'] if ep['images'] else None
-                    #print(post_image)
-
-                    episode = {
-                        'name': ep['name'],
-                        'season': season,
-                        'episode': int(ep['number']),
-                        'description': ep['plot'],
-                        'duration': int(ep['duration']),
-                        'posterUrl': post_image,
-                        'url': href,
-                        'scws_id': scws_id
-                    }
-                    episode_list.append(episode)
-
-            if not episode_list:
-                raise Exception("No Seasons Found")
-
-            return {
-                'name': name,
-                'url': url,
-                'type': type,
-                'episodeList': episode_list,
-                'posterUrl': poster,
-                'year': int(''.join(filter(str.isdigit, year))),
-                'plot': plot,
-                'tmdb_id': tmdb_id,
-                'imdb_id': imdb_id,
-                'netflix_id': netflix_id,
-                'prime_id': prime_id,
-                'disney_id': disney_id,
-                'release_date': release_date,
-                'sub_ita': bool(sub_ita),
-                'rating': int(float(score) * 1000),
-                'seasons_count': seasons_count,
-                'tags': [genre['name'] for genre in datajs['genres']],
-                'trailerUrl': trailer_url,
-                'recommendations': correlates_list
-            }
-        else:
-            return {
-                'name': soup.select_one("div > div > h1").text,
-                'url': f"{self.URL}/watch/{props['title']['id']}",
-                'scws_id': props['title']['scws_id'],
-                'type': type,
-                'posterUrl': poster,
-                'year': int(''.join(filter(str.isdigit, year))),
-                'plot': plot,
-                'tmdb_id': tmdb_id,
-                'imdb_id': imdb_id,
-                'netflix_id': netflix_id,
-                'prime_id': prime_id,
-                'disney_id': disney_id,
-                'release_date': release_date,
-                'sub_ita': bool(sub_ita),
-                'rating': int(float(score) * 1000),
-                'tags': [genre['name'] for genre in datajs['genres']],
-                'duration': int(props['title']['runtime']),
-                'trailerUrl': trailer_url,
-                'recommendations': correlates_list
-            }
-
-
-    def load_links(self, data):
-        ip = requests.get("https://api.ipify.org/").text
-
-        type = 'Movie' if data['type'] == 'Movie' else 'TvSeries'
-
-        #print(type)
-        return 'Still working on it!'
-
-        if type == 'TvSeries':
-            links = []
-            for ep in data['episodeList']:
-                scwsid = ep['scws_id']
-
-                expire = str(int(time.time()) + 172800)
-                token0 = (expire + ip + " Yc8U6r8KjAKAepEA").encode()
-                token1 = hashlib.md5(token0).digest()
-                token2 = base64.b64encode(token1).decode()
-                token = token2.replace("=", "").replace("+", "-").replace("/", "_")
-
-                link = f'https://vixcloud.co/v2/playlist/{scwsid}?token={token}&token480p={token}&expires={expire}&n=1'
-
-                links.append(link)
-
-            return links
-
-        else:
-            scwsid = data['scws_id']
-
-
-            expire = str(int(time.time()) + 172800)
-
-            token0 = (expire + ip + " Yc8U6r8KjAKAepEA").encode()
-            token1 = hashlib.md5(token0).digest()
-            token2 = base64.b64encode(token1).decode()
-            token = token2.replace("=", "").replace("+", "-").replace("/", "_")
-
-            #link = f'https://scws.work/master/{scwsid}?token={token}&expires={expire}&n=1'
-            link = f'https://vixcloud.co/v2/playlist/{scwsid}?token={token}&token480p={token}&expires={expire}&n=1'
-                    #https://vixcloud.co/v2/playlist/159536?token=t5OmJHPGf9Ti3DXdd0l_AQ&token360p=&token480p=cEjEiuArJcYsrbPzksSQTQ&token720p=n-00eKBvOxqRh0ISQjbu3Q&token1080p=&expires=1695317130&canCast=1&n=1&b=1
-
-            #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=&expires=1695316859&canCast=1&b=1&n=1
-            #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=HjLZ1Qbx0oNt7u7DbDHM3w&expires=1690305563&n=1
-
-            return link
+import requests
+from bs4 import BeautifulSoup
+import time
+import hashlib
+import base64
+import json
+import re
+
+
+#streamingcommunity bet
+
+class SCAPI:
+    def __init__(self, DOMAIN, userAgent="Mozilla/5.0 (Windows NT 11.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"):
+        self.userAgent = userAgent
+        self.DOMAIN = DOMAIN
+        self.URL = 'https://' + self.DOMAIN
+
+    def search(self, query):
+        headers = {'user-agent': self.userAgent}
+        main_url = requests.get(self.URL, headers=headers).url
+        query_formatted = query.replace(" ", "%20")
+        url = f"{main_url}api/search?q={query_formatted}"
+        #print(url)
+        document = requests.get(url, headers=headers)
+        search_results = document.json()['data']
+        #print(search_results)
+        output_dict = {}
+        for result in search_results:
+            result['url'] = f"{self.URL}/titles/{result['id']}-{result['slug']}"
+            output_dict[result['name']] = result
+
+        return output_dict #[result for result in search_results]
+
+
+    def load(self, url):
+        headers = {'user-agent': self.userAgent}
+        document = requests.get(url, headers=headers)
+        soup = BeautifulSoup(document.content, 'html.parser')
+        poster = re.search("url\((.*)\)", soup.find("div", class_="title-container")['style']).group(1)
+        #print(poster)
+        id = ''.join(filter(str.isdigit, url.split('-')[0]))
+        datajs = requests.post(f"{self.URL}/api/titles/preview/{id}", headers=headers).json()
+
+
+        type = 'Movie' if datajs['type'] == 'movie' else 'TvSeries'
+
+        year = datajs['release_date'].split('-')[0]
+
+        pagedata = soup.find(id="app")["data-page"]
+        #print(pagedata)
+        props = json.loads(pagedata)['props']
+
+        trailer_info = props['title']['trailers']
+        trailer_url = f"https://www.youtube.com/watch?v={trailer_info[0]['youtube_id']}" if trailer_info else None
+        #print(trailer_url)
+
+
+        correlates = props['sliders'][0]['titles']
+        size = min(len(correlates), 15)
+        correlates_list = correlates[:size]
+
+        plot = props['title']['plot']
+
+        score = props['title']['score']
+
+        tmdb_id = props['title']['tmdb_id']
+        imdb_id = props['title']['imdb_id']
+        netflix_id = props['title']['netflix_id']
+        prime_id = props['title']['prime_id']
+        disney_id = props['title']['disney_id']
+        release_date = props['title']['release_date']
+        sub_ita = props['title']['sub_ita']
+
+        if type == 'TvSeries':
+
+            name = props['title']['name']
+
+            seasons = props['title']['seasons']
+
+            seasons_count = int(props['title']['seasons_count'])
+
+            episode_list = []
+            for se in seasons:
+                season = int(se['number'])
+                document = requests.get(f'{url}/stagione-{season}', headers=headers)
+                soup = BeautifulSoup(document.content, 'html.parser')
+                pagedata = soup.find(id="app")["data-page"]
+                #print(pagedata)
+                episodes = json.loads(pagedata)['props']['loadedSeason']['episodes']
+                sid = se['title_id']
+                for ep in episodes:
+                    scws_id = ep['scws_id']
+                    href = f"{self.URL}/watch/{sid}?e={ep['id']}"
+                    post_image = 'https://cdn.' + self.DOMAIN + '/images/' + ep['images'][0]['filename'] if ep['images'] else None
+                    #print(post_image)
+
+                    episode = {
+                        'name': ep['name'],
+                        'season': season,
+                        'episode': int(ep['number']),
+                        'description': ep['plot'],
+                        'duration': int(ep['duration']),
+                        'posterUrl': post_image,
+                        'url': href,
+                        'scws_id': scws_id
+                    }
+                    episode_list.append(episode)
+
+            if not episode_list:
+                raise Exception("No Seasons Found")
+
+            return {
+                'name': name,
+                'url': url,
+                'type': type,
+                'episodeList': episode_list,
+                'posterUrl': poster,
+                'year': int(''.join(filter(str.isdigit, year))),
+                'plot': plot,
+                'tmdb_id': tmdb_id,
+                'imdb_id': imdb_id,
+                'netflix_id': netflix_id,
+                'prime_id': prime_id,
+                'disney_id': disney_id,
+                'release_date': release_date,
+                'sub_ita': bool(sub_ita),
+                'rating': int(float(score) * 1000),
+                'seasons_count': seasons_count,
+                'tags': [genre['name'] for genre in datajs['genres']],
+                'trailerUrl': trailer_url,
+                'recommendations': correlates_list
+            }
+        else:
+            return {
+                'name': soup.select_one("div > div > h1").text,
+                'url': f"{self.URL}/watch/{props['title']['id']}",
+                'scws_id': props['title']['scws_id'],
+                'type': type,
+                'posterUrl': poster,
+                'year': int(''.join(filter(str.isdigit, year))),
+                'plot': plot,
+                'tmdb_id': tmdb_id,
+                'imdb_id': imdb_id,
+                'netflix_id': netflix_id,
+                'prime_id': prime_id,
+                'disney_id': disney_id,
+                'release_date': release_date,
+                'sub_ita': bool(sub_ita),
+                'rating': int(float(score) * 1000),
+                'tags': [genre['name'] for genre in datajs['genres']],
+                'duration': int(props['title']['runtime']),
+                'trailerUrl': trailer_url,
+                'recommendations': correlates_list
+            }
+
+
+    def load_links(self, data):
+        ip = requests.get("https://api.ipify.org/").text
+
+        type = 'Movie' if data['type'] == 'Movie' else 'TvSeries'
+
+        #print(type)
+        return 'Still working on it!'
+
+        if type == 'TvSeries':
+            links = []
+            for ep in data['episodeList']:
+                scwsid = ep['scws_id']
+
+                expire = str(int(time.time()) + 172800)
+                token0 = (expire + ip + " Yc8U6r8KjAKAepEA").encode()
+                token1 = hashlib.md5(token0).digest()
+                token2 = base64.b64encode(token1).decode()
+                token = token2.replace("=", "").replace("+", "-").replace("/", "_")
+
+                link = f'https://vixcloud.co/v2/playlist/{scwsid}?token={token}&token480p={token}&expires={expire}&n=1'
+
+                links.append(link)
+
+            return links
+
+        else:
+            scwsid = data['scws_id']
+
+
+            expire = str(int(time.time()) + 172800)
+
+            token0 = (expire + ip + " Yc8U6r8KjAKAepEA").encode()
+            token1 = hashlib.md5(token0).digest()
+            token2 = base64.b64encode(token1).decode()
+            token = token2.replace("=", "").replace("+", "-").replace("/", "_")
+
+            #link = f'https://scws.work/master/{scwsid}?token={token}&expires={expire}&n=1'
+            link = f'https://vixcloud.co/v2/playlist/{scwsid}?token={token}&token480p={token}&expires={expire}&n=1'
+                    #https://vixcloud.co/v2/playlist/159536?token=t5OmJHPGf9Ti3DXdd0l_AQ&token360p=&token480p=cEjEiuArJcYsrbPzksSQTQ&token720p=n-00eKBvOxqRh0ISQjbu3Q&token1080p=&expires=1695317130&canCast=1&n=1&b=1
+
+            #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=&expires=1695316859&canCast=1&b=1&n=1
+            #https://vixcloud.co/v2/playlist/159536?type=video&rendition=1080p&token=HjLZ1Qbx0oNt7u7DbDHM3w&expires=1690305563&n=1
+
+            return link
```

### Comparing `streamingcommunity_unofficialapi-0.0.2.1/README.md` & `streamingcommunity_unofficialapi-0.0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,219 @@
-A simple unofficial api for the italian StreamingCommunity website.
-
-
-
-# StreamingCommunity-API
-
-## Installazione
-
-Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
-
-È Possibile installarare la libreria tramite pip:
-
-
-```
-pip install streamingcommunity-unofficialapi
-```
-
-
-## Utilizzo
-
-Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-
-```
-
-### Ricerca
-Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
-
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-sc.search('John Wick')
-
-```
-
-La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
-
-#### Esempio:
-```
-{
-    "John Wick": {
-        "id": 6,
-        "slug": "john-wick",
-        "name": "John Wick",
-        "type": "movie",
-        "score": "8.1",
-        "sub_ita": 0,
-        "last_air_date": "2014-10-22",
-        "seasons_count": 0,
-        "images": [
-            {
-                "imageable_id": 6,
-                "imageable_type": "title",
-                "filename": "f7887fba-d2d3-4252-b2e9-45129e1ecfd9.webp",
-                "type": "poster",
-                "original_url_field": None,
-            },
-            {
-                "imageable_id": 6,
-                "imageable_type": "title",
-                "filename": "3ca16987-4229-4369-ba0b-670e0ec2b4df.webp",
-                "type": "background",
-                "original_url_field": None,
-            }
-        ],
-        "url": "https://StreamingCommunity.esempio/titles/6-john-wick",
-    },
-    "John Wick 4": {
-        "id": 6203,
-        "slug": "john-wick-4",
-        "name": "John Wick 4",
-        "type": "movie",
-        "score": "8.6",
-        "sub_ita": 0,
-        "last_air_date": "2023-03-22",
-        "seasons_count": 0,
-        "images": [
-            {
-                "imageable_id": 6203,
-                "imageable_type": "title",
-                "filename": "8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
-                "type": "cover_mobile",
-                "original_url_field": None,
-            },
-            {
-                "imageable_id": 6203,
-                "imageable_type": "title",
-                "filename": "64934c02-794f-4307-a860-758eed06b717.webp",
-                "type": "logo",
-                "original_url_field": None,
-            }
-        ],
-        "url": "https://StreamingCommunity.esempio/titles/6203-john-wick-4",
-    },
-}
-```
-
-### Info Film/Serie
-
-Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
-
-```
-from SCuapi import SCAPI
-
-sc = SCAPI('StreamingCommunity.esempio')
-sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
-```
-
-La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
-
-#### Esempio:
-```
-{
-    "name": "John Wick 4",
-    "url": "https://StreamingCommunity.esempio/watch/6203",
-    "scws_id": 157670,
-    "type": "Movie",
-    "posterUrl": "https://cdn.StreamingCommunity.esempio/images/8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
-    "year": 2023,
-    "plot": "John Wick trova una via per sconfiggere la Gran Tavola. Ma prima di guadagnare la libertà, Wick deve affrontare un nuovo nemico che ha potenti alleanze in tutto il mondo e ha mezzi tali da tramutare vecchi amici in nuovi nemici.",
-    "tmdb_id": 603692,
-    "imdb_id": "tt10366206",
-    "netflix_id": None,
-    "prime_id": None,
-    "disney_id": None,
-    "release_date": "2023-03-22",
-    "sub_ita": False,
-    "rating": 8600,
-    "tags": ["Crime", "Azione", "Thriller"],
-    "duration": 169,
-    "trailerUrl": "https://www.youtube.com/watch?v=049RtZzgAtA",
-    "recommendations": [
-        {
-            "id": 5077,
-            "slug": "luomo-ombra",
-            "name": "L'uomo ombra",
-            "type": "movie",
-            "score": "6.0",
-            "sub_ita": 0,
-            "last_air_date": "1994-07-01",
-            "seasons_count": 0,
-            "images": [
-                {
-                    "imageable_id": 5077,
-                    "imageable_type": "title",
-                    "filename": "125664cb-82c6-403b-a262-916080307f77.webp",
-                    "type": "poster",
-                    "original_url_field": None,
-                },
-                {
-                    "imageable_id": 5077,
-                    "imageable_type": "title",
-                    "filename": "1666007b-f7df-4308-910b-4e4ae414f35a.webp",
-                    "type": "background",
-                    "original_url_field": None,
-                }
-            ],
-        },
-        {
-            "id": 1636,
-            "slug": "il-padrino",
-            "name": "Il padrino",
-            "type": "movie",
-            "score": "9.2",
-            "sub_ita": 0,
-            "last_air_date": "1972-03-14",
-            "seasons_count": 0,
-            "images": [
-                {
-                    "imageable_id": 1636,
-                    "imageable_type": "title",
-                    "filename": "37beda03-f1c5-4958-9456-b696b9d8918f.webp",
-                    "type": "cover",
-                    "original_url_field": None,
-                },
-                {
-                    "imageable_id": 1636,
-                    "imageable_type": "title",
-                    "filename": "d6bf67db-6644-4381-a3a1-7d5a75b393c6.webp",
-                    "type": "cover_mobile",
-                    "original_url_field": None,
-                }
-            ],
-        }
-    ],
-}
-
-```
-
-### Download link
-
-In progresso.
+Metadata-Version: 2.1
+Name: streamingcommunity_unofficialapi
+Version: 0.0.3.1
+Summary: A simple unofficial api for the italian StreamingCommunity website.
+Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
+Author: Beqir Stafa
+Author-email: beqirstafa@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Requires-Python: >= 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A simple unofficial api for the italian StreamingCommunity website.
+
+
+![PyPI](https://img.shields.io/pypi/v/streamingcommunity-unofficialapi)
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/Blu-Tiger/streamingcommunity-unofficialapi)
+
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+
+
+# StreamingCommunity-API
+
+## Installazione
+
+Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
+
+È Possibile installarare la libreria tramite pip:
+
+
+```
+pip install streamingcommunity-unofficialapi
+```
+
+
+## Utilizzo
+
+Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
+```
+from scuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+
+```
+
+### Ricerca
+Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
+
+```
+from scuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+sc.search('John Wick')
+
+```
+
+La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
+
+#### Esempio:
+```
+{
+    "John Wick": {
+        "id": 6,
+        "slug": "john-wick",
+        "name": "John Wick",
+        "type": "movie",
+        "score": "8.1",
+        "sub_ita": 0,
+        "last_air_date": "2014-10-22",
+        "seasons_count": 0,
+        "images": [
+            {
+                "imageable_id": 6,
+                "imageable_type": "title",
+                "filename": "f7887fba-d2d3-4252-b2e9-45129e1ecfd9.webp",
+                "type": "poster",
+                "original_url_field": None,
+            },
+            {
+                "imageable_id": 6,
+                "imageable_type": "title",
+                "filename": "3ca16987-4229-4369-ba0b-670e0ec2b4df.webp",
+                "type": "background",
+                "original_url_field": None,
+            }
+        ],
+        "url": "https://StreamingCommunity.esempio/titles/6-john-wick",
+    },
+    "John Wick 4": {
+        "id": 6203,
+        "slug": "john-wick-4",
+        "name": "John Wick 4",
+        "type": "movie",
+        "score": "8.6",
+        "sub_ita": 0,
+        "last_air_date": "2023-03-22",
+        "seasons_count": 0,
+        "images": [
+            {
+                "imageable_id": 6203,
+                "imageable_type": "title",
+                "filename": "8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
+                "type": "cover_mobile",
+                "original_url_field": None,
+            },
+            {
+                "imageable_id": 6203,
+                "imageable_type": "title",
+                "filename": "64934c02-794f-4307-a860-758eed06b717.webp",
+                "type": "logo",
+                "original_url_field": None,
+            }
+        ],
+        "url": "https://StreamingCommunity.esempio/titles/6203-john-wick-4",
+    },
+}
+```
+
+### Info Film/Serie
+
+Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
+
+```
+from scuapi import SCAPI
+
+sc = SCAPI('StreamingCommunity.esempio')
+sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
+```
+
+La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
+
+#### Esempio:
+```
+{
+    "name": "John Wick 4",
+    "url": "https://StreamingCommunity.esempio/watch/6203",
+    "scws_id": 157670,
+    "type": "Movie",
+    "posterUrl": "https://cdn.StreamingCommunity.esempio/images/8babb029-90b3-4237-aff2-2395b2dfb5ce.webp",
+    "year": 2023,
+    "plot": "John Wick trova una via per sconfiggere la Gran Tavola. Ma prima di guadagnare la libertà, Wick deve affrontare un nuovo nemico che ha potenti alleanze in tutto il mondo e ha mezzi tali da tramutare vecchi amici in nuovi nemici.",
+    "tmdb_id": 603692,
+    "imdb_id": "tt10366206",
+    "netflix_id": None,
+    "prime_id": None,
+    "disney_id": None,
+    "release_date": "2023-03-22",
+    "sub_ita": False,
+    "rating": 8600,
+    "tags": ["Crime", "Azione", "Thriller"],
+    "duration": 169,
+    "trailerUrl": "https://www.youtube.com/watch?v=049RtZzgAtA",
+    "recommendations": [
+        {
+            "id": 5077,
+            "slug": "luomo-ombra",
+            "name": "L'uomo ombra",
+            "type": "movie",
+            "score": "6.0",
+            "sub_ita": 0,
+            "last_air_date": "1994-07-01",
+            "seasons_count": 0,
+            "images": [
+                {
+                    "imageable_id": 5077,
+                    "imageable_type": "title",
+                    "filename": "125664cb-82c6-403b-a262-916080307f77.webp",
+                    "type": "poster",
+                    "original_url_field": None,
+                },
+                {
+                    "imageable_id": 5077,
+                    "imageable_type": "title",
+                    "filename": "1666007b-f7df-4308-910b-4e4ae414f35a.webp",
+                    "type": "background",
+                    "original_url_field": None,
+                }
+            ],
+        },
+        {
+            "id": 1636,
+            "slug": "il-padrino",
+            "name": "Il padrino",
+            "type": "movie",
+            "score": "9.2",
+            "sub_ita": 0,
+            "last_air_date": "1972-03-14",
+            "seasons_count": 0,
+            "images": [
+                {
+                    "imageable_id": 1636,
+                    "imageable_type": "title",
+                    "filename": "37beda03-f1c5-4958-9456-b696b9d8918f.webp",
+                    "type": "cover",
+                    "original_url_field": None,
+                },
+                {
+                    "imageable_id": 1636,
+                    "imageable_type": "title",
+                    "filename": "d6bf67db-6644-4381-a3a1-7d5a75b393c6.webp",
+                    "type": "cover_mobile",
+                    "original_url_field": None,
+                }
+            ],
+        }
+    ],
+}
+
+```
+
+### Download link
+
+In progresso.
```

### Comparing `streamingcommunity_unofficialapi-0.0.2.1/PKG-INFO` & `streamingcommunity_unofficialapi-0.0.3.1/streamingcommunity_unofficialapi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: streamingcommunity-unofficialapi
-Version: 0.0.2.1
-Summary: A simple unofficial api for the italian StreamingCommunity website
-Author-email: Beqir Stafa <beqirstafa@gmail.com>
-License-File: LICENSE
+Version: 0.0.3.1
+Summary: A simple unofficial api for the italian StreamingCommunity website.
+Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
+Author: Beqir Stafa
+Author-email: beqirstafa@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Classifier: Topic :: Utilities
+Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 A simple unofficial api for the italian StreamingCommunity website.
 
 
+![PyPI](https://img.shields.io/pypi/v/streamingcommunity-unofficialapi)
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/Blu-Tiger/streamingcommunity-unofficialapi)
+
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/streamingcommunity-unofficialapi)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/streamingcommunity-unofficialapi)
+
 
 # StreamingCommunity-API
 
 ## Installazione
 
 Questa libreria richiede [Python 3.10](https://www.python.org/) o superiore.
 
@@ -28,25 +39,25 @@
 ```
 
 
 ## Utilizzo
 
 Per iniziare bisona impostare il dominio di StreamingCommunity che si desidera utilizzare.
 ```
-from SCuapi import SCAPI
+from scuapi import SCAPI
 
 sc = SCAPI('StreamingCommunity.esempio')
 
 ```
 
 ### Ricerca
 Per ricercare un Film o una Serie per nome nel sito di StreamingCommunity è possibile usare la funzione search().
 
 ```
-from SCuapi import SCAPI
+from scuapi import SCAPI
 
 sc = SCAPI('StreamingCommunity.esempio')
 sc.search('John Wick')
 
 ```
 
 La funzione restituirà un dizionario contentente per chiave il nome del Film o Serie e per valore un dizionario contenente tutte le informazioni correllate.
@@ -112,15 +123,15 @@
 ```
 
 ### Info Film/Serie
 
 Per ottenere informazioni su un Film o una Serie è possibile usare la funzione load().
 
 ```
-from SCuapi import SCAPI
+from scuapi import SCAPI
 
 sc = SCAPI('StreamingCommunity.esempio')
 sc.load('https://StreamingCommunity.esempio/titles/6203-john-wick-4')
 ```
 
 La funzione restituirà un dizionario contentente tutte le informazioni su Film o Serie.
 
@@ -201,8 +212,8 @@
     ],
 }
 
 ```
 
 ### Download link
 
-In progresso.
+In progresso.
```

