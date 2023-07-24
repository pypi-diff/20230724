# Comparing `tmp/porn_cli-1.0.3.tar.gz` & `tmp/porn_cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porn_cli-1.0.3.tar", max compression
+gzip compressed data, was "porn_cli-1.0.5.tar", max compression
```

## Comparing `porn_cli-1.0.3.tar` & `porn_cli-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-02-21 03:34:35.918096 porn_cli-1.0.3/LICENSE
--rw-r--r--   0        0        0     6436 2023-02-21 03:34:35.918096 porn_cli-1.0.3/README.md
--rw-r--r--   0        0        0       23 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/__init__.py
--rw-r--r--   0        0        0     1058 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/players/__init__.py
--rw-r--r--   0        0        0     1869 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/players/mpv.py
--rw-r--r--   0        0        0     1457 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/players/vlc.py
--rw-r--r--   0        0        0        0 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/__init__.py
--rw-r--r--   0        0        0      135 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/dbs.py
--rw-r--r--   0        0        0     2610 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/httpclient.py
--rw-r--r--   0        0        0     1485 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/player.py
--rw-r--r--   0        0        0      171 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/provider.py
--rw-r--r--   0        0        0     7447 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/websites/__init__.py
--rw-r--r--   0        0        0     2044 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/websites/hentaimama.py
--rw-r--r--   0        0        0     3083 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/websites/javct.py
--rw-r--r--   0        0        0     1392 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/websites/pornhub.py
--rw-r--r--   0        0        0     1794 2023-02-21 03:34:35.918096 porn_cli-1.0.3/porn_cli/websites/xxxmax.py
--rw-r--r--   0        0        0      692 2023-02-21 03:34:35.918096 porn_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7287 1970-01-01 00:00:00.000000 porn_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 20:02:06.740492 porn_cli-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2653 2023-07-24 20:02:06.740492 porn_cli-1.0.5/README.md
+-rw-r--r--   0        0        0       23 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/hentaimama.py
+-rw-r--r--   0        0        0     3092 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/javct.py
+-rw-r--r--   0        0        0     1400 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/pornhub.py
+-rw-r--r--   0        0        0     1810 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/xxxmax.py
+-rw-r--r--   0        0        0      564 2023-07-24 20:02:06.740492 porn_cli-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 porn_cli-1.0.5/PKG-INFO
```

### Comparing `porn_cli-1.0.3/LICENSE` & `porn_cli-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `porn_cli-1.0.3/porn_cli/websites/hentaimama.py` & `porn_cli-1.0.5/porn_cli/websites/porn/hentaimama.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ..utils.scraper import WebScraper
+from mov_cli.utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
 import re
 
 
-class hentaimama(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str):
         q = (
             input("[!] Please Enter the name of the Porn: ")
@@ -19,15 +19,15 @@
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
         soup = BS(req, "lxml")
         items = soup.findAll("div", {"class": "result-item"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("img")["alt"] for i in range(len(items))]
         ids = [i for i in range(len(items))]
-        mov_or_tv = ["PORNOS" for i in range(len(items))]
+        mov_or_tv = ["Hentai" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(url).text
         soup = BS(req, "lxml")
         episodes = soup.findAll("article", {"class": "item se episodes"})
         print(episodes)
@@ -53,8 +53,8 @@
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         name = t[self.title]
         url, episode = self.ask(t[self.url])
         url = self.cdn_url(url)
         if state == "d":
             self.dl(url, name, season=".", episode=episode)
             return
-        self.play(url, name)
+        self.play(url, name)
```

### Comparing `porn_cli-1.0.3/porn_cli/websites/javct.py` & `porn_cli-1.0.5/porn_cli/websites/porn/javct.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from mov_cli.utils.scraper import WebScraper
 import re
 from base64 import b64encode
 
-class javct(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
     
     def search(self, q: str):
         q = (
             input("[!] Please Enter the name of the Porn: ")
```

### Comparing `porn_cli-1.0.3/porn_cli/websites/pornhub.py` & `porn_cli-1.0.5/porn_cli/websites/porn/pornhub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from mov_cli.utils.scraper import WebScraper
 
-class pornhub(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
     
     def search(self, q: str):
         q = (
             input("[!] Please Enter the name of the Porn: ")
@@ -30,8 +30,8 @@
     
     def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
         name = m[self.title]
         url = self.cdn_url(f"{m[self.aid]}")
         if state == "d":
             self.dl(url, name)
             return
-        self.play(url, name)
+        self.play(url, name)
```

### Comparing `porn_cli-1.0.3/porn_cli/websites/xxxmax.py` & `porn_cli-1.0.5/porn_cli/websites/porn/xxxmax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from mov_cli.utils.scraper import WebScraper
+from mov_cli.utils.props import SelectedNotAvailable
 import re
 from urllib.parse import unquote
 from base64 import b64decode
 
-class xxxmax(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
     
     def search(self, q: str):
         q = (
             input("[!] Please Enter the name of the Porn: ")
@@ -29,22 +30,21 @@
     
     def cdn_url(self, url):
         req = self.client.get(url).text
         soup = BS(req, "lxml")
         items = soup.find("div", {"class": "responsive-player"})
         try:
             iframe = items.find("iframe")["src"]
-        except AttributeError as e:
-            print(f"Couldn't find the iframe | {e}")
-            return exit(0)
+        except AttributeError:
+            raise SelectedNotAvailable
         encrypted = re.findall('q=(.*)', iframe)[0]
         decrypted = unquote(str(b64decode(encrypted)))
         url = re.findall('src="(.*?)"', decrypted)[0]
         return url
     
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
         name = m[self.title]
         url = self.cdn_url(m[self.url])
         if state == "d":
             self.dl(url, name)
             return
-        self.play(url, name, referrer=m[self.url])
+        self.play(url, name, referrer=m[self.url])
```

