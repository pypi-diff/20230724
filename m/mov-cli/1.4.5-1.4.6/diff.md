# Comparing `tmp/mov_cli-1.4.5.tar.gz` & `tmp/mov_cli-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.5.tar", max compression
+gzip compressed data, was "mov_cli-1.4.6.tar", max compression
```

## Comparing `mov_cli-1.4.5.tar` & `mov_cli-1.4.6.tar`

### file list

```diff
@@ -1,58 +1,74 @@
--rw-r--r--   0        0        0    35149 2023-07-04 17:42:07.620723 mov_cli-1.4.5/LICENSE
--rw-r--r--   0        0        0     7112 2023-07-04 17:42:07.620723 mov_cli-1.4.5/README.md
--rw-r--r--   0        0        0      235 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/__init__.py
--rw-r--r--   0        0        0     2612 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2559 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1484 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2715 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1584 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/player.py
--rw-r--r--   0        0        0      958 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8708 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    10970 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4177 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4208 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1943 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1724 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3210 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     3736 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2509 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2563 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4662 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4422 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4217 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1644 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2132 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2895 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4516 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3395 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3983 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3503 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      731 2023-07-04 17:42:07.624723 mov_cli-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     8095 1970-01-01 00:00:00.000000 mov_cli-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 19:39:52.997461 mov_cli-1.4.6/LICENSE
+-rw-r--r--   0        0        0     6933 2023-07-24 19:39:52.997461 mov_cli-1.4.6/README.md
+-rw-r--r--   0        0        0      686 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0      341 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/tukipasti.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2772 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0      356 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ar.json
+-rw-r--r--   0        0        0      356 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/de.json
+-rw-r--r--   0        0        0      309 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/en.json
+-rw-r--r--   0        0        0      348 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/fr.json
+-rw-r--r--   0        0        0      338 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ko.json
+-rw-r--r--   0        0        0      194 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/langs
+-rw-r--r--   0        0        0      308 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/pl.json
+-rw-r--r--   0        0        0      289 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/pt.json
+-rw-r--r--   0        0        0      418 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ru.json
+-rw-r--r--   0        0        0      660 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ta.json
+-rw-r--r--   0        0        0     1752 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1563 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1171 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/props.py
+-rw-r--r--   0        0        0     7383 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0     4630 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/select.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/anime/__init__.py
+-rw-r--r--   0        0        0     3286 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/anime/gogoanime.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/__init__.py
+-rw-r--r--   0        0        0     3767 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/viewasian.py
+-rw-r--r--   0        0        0     3394 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/watchasian.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/cartoons/__init__.py
+-rw-r--r--   0        0        0     3734 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/cartoons/kisscartoon.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/english/__init__.py
+-rw-r--r--   0        0        0     7381 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/actvid.py
+-rw-r--r--   0        0        0     3856 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/dopebox.py
+-rw-r--r--   0        0        0     4242 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/remotestream.py
+-rw-r--r--   0        0        0     3734 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/sflix.py
+-rw-r--r--   0        0        0     1841 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/solar.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/__init__.py
+-rw-r--r--   0        0        0     1943 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/einthusan.py
+-rw-r--r--   0        0        0     2165 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/tamilyogi.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/international/__init__.py
+-rw-r--r--   0        0        0     3962 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/international/wlext.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/livetv/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/livetv/eja.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/sports/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/sports/scdn.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/__init__.py
+-rw-r--r--   0        0        0     2330 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/turkish123.py
+-rw-r--r--   0        0        0     2921 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/yoturkish.py
+-rw-r--r--   0        0        0      736 2023-07-24 19:39:53.005462 mov_cli-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 mov_cli-1.4.6/PKG-INFO
```

### Comparing `mov_cli-1.4.5/LICENSE` & `mov_cli-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/README.md` & `mov_cli-1.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: mov-cli
+Version: 1.4.6
+Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
+Home-page: https://github.com/mov-cli/mov-cli
+License: GPLv3
+Author: Pain
+Author-email: painedposeidon444@gmail.com
+Maintainer: Ananas
+Maintainer-email: ananas@r3tr0ananas.lol
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: krfzf-py (>=0.0.4,<0.0.5)
+Requires-Dist: pycryptodome (>=3.17,<4.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: tldextract (>=3.4.3,<4.0.0)
+Project-URL: Bug Tracker, https://github.com/mov-cli/mov-cli/issues
+Project-URL: Repository, https://github.com/mov-cli/mov-cli
+Description-Content-Type: text/markdown
+
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
@@ -28,15 +54,15 @@
 <br />
 <div align="center">
   <a href="https://github.com/mov-cli/mov-cli">
     <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="80" height="80">
   </a>
 
   <p align="center">
- A cli tool to browse and watch Movies/Shows/TV/Sports. 
+    A cli tool to browse and watch Movies/Shows/TV/Sports. 
     <br />
     <br />
     <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
     ·
     <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
   </p>
 </div>
@@ -68,22 +94,20 @@
   <li><a href="#inspiration">inspiration</a></li>
 </ol>
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
+The new and improved mov-cli is here.
+
 mov-cli is a Commandline Tool to watch and download shows and movies.
 
-Shows and Movies are scraped from Streaming Sites.
+Shows and Movies are sourced from Streaming Sites.
 
-mov-cli currently scrapes 15 Providers:
-```
-Actvid · SFlix · Solar · DopeBox · WLEXT · KinoX · StreamBlasters · TamilYogi · Einthusan · ViewAsian · Watchasian · GogoAnime · Eja · KimCartoon · Turkish123
-```
 <p align="right">(<a href="#readme-top">back to top</a>)</p
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 
 
@@ -218,7 +242,8 @@
 [forks-url]: https://github.com/mov-cli/mov-cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli.svg?style=for-the-badge
 [stars-url]: https://github.com/mov-cli/mov-cli/stargazers
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli.svg?style=for-the-badge
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli.svg?style=for-the-badge
 [license-url]: https://github.com/mov-cli/mov-cli/blob/master/LICENSE.txt
+
```

#### html2text {}

```diff
@@ -1,9 +1,22 @@
-      [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
-[issues-url] [![MIT License][license-shield]][license-url]
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.6 Summary: A cli tool to
+browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
+mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
+Maintainer: Ananas Maintainer-email: ananas@r3tr0ananas.lol Requires-Python:
+>=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
+(>=4.11.2,<5.0.0) Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: krfzf-
+py (>=0.0.4,<0.0.5) Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist:
+six (>=1.16.0,<2.0.0) Requires-Dist: tldextract (>=3.4.3,<4.0.0) Project-URL:
+Bug Tracker, https://github.com/mov-cli/mov-cli/issues Project-URL: Repository,
+https://github.com/mov-cli/mov-cli Description-Content-Type: text/markdown
+[![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
                                     [Logo]
             A cli tool to browse and watch Movies/Shows/TV/Sports.
 
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
@@ -15,19 +28,17 @@
    3. Usage
    4. Disclaimer
    5. Contributing
    6. Adding_Languages
    7. License
    8. Contact
    9. inspiration
- ## About The Project mov-cli is a Commandline Tool to watch and download shows
-and movies. Shows and Movies are scraped from Streaming Sites. mov-cli
-currently scrapes 15 Providers: ``` Actvid Â· SFlix Â· Solar Â· DopeBox Â·
-WLEXT Â· KinoX Â· StreamBlasters Â· TamilYogi Â· Einthusan Â· ViewAsian Â·
-Watchasian Â· GogoAnime Â· Eja Â· KimCartoon Â· Turkish123 ```
+ ## About The Project The new and improved mov-cli is here. mov-cli is a
+Commandline Tool to watch and download shows and movies. Shows and Movies are
+sourced from Streaming Sites.
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
 [`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
              (https://iina.io) - player used for MacOS - [`Outplayer`](https://
   outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
        FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
   selection Menu ## Installation  ### Windows / Linux - Run this Command inside
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
```

### Comparing `mov_cli-1.4.5/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.6/mov_cli/extractors/doodstream.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import re
 import httpx
+from ..utils.props import SelectedNotAvailable
 
 
 def dood(url):
     print(url)
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:91.0) Gecko/20100101 Firefox/91.0"
     }
     video_id = httpx.URL(url).path.split("/")[-1]
     print(video_id)
     webpage_html = httpx.get(
         f"https://dood.to/e/{video_id}", headers=headers, follow_redirects=True
     )
     webpage_html = webpage_html.text
-    print(webpage_html)
-    pass_md5 = re.search(r"/pass_md5/[^']*", webpage_html).group()
+    try:
+        pass_md5 = re.search(r"/pass_md5/[^']*", webpage_html).group()
+    except:
+        raise SelectedNotAvailable
     urlh = f"https://dood.to{pass_md5}"
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:91.0) Gecko/20100101 Firefox/91.0",
         "referer": "https://dood.to",
     }
     res = httpx.get(urlh, headers=headers).text
     md5 = pass_md5.split("/")
```

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.6/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.5/mov_cli/players/player.py` & `mov_cli-1.4.6/mov_cli/players/player.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,53 +24,68 @@
                     "-n",
                     "is.xyz.mpv/is.xyz.mpv.MPVActivity",
                     "-e",
                     "filepath",
                     f"{url}",
                 ]
             )
-    
+
         elif self.os == "iOS":
             print("[!] Detected your using iOS. \r\n")
-            
-            print(f'\033]8;;outplayer://{url}\033\\-------------------------\n- Tap to open Outplayer -\n-------------------------\033]8;;\033\\\n')
+
+            print(
+                f"\033]8;;outplayer://{url}\033\\-------------------------\n- Tap to open Outplayer -\n-------------------------\033]8;;\033\\\n"
+            )
 
             sys.exit(1)
 
         else:  # Windows, Linux and Other
             try:
                 if self.os == "Linux" or self.os == "Windows":
                     mpv_args = [
                         f"--referrer={referrer}",
                         f"{url}",
                         f"--force-media-title=mov-cli:{media_title}",
                         "--no-terminal",
                     ]
 
-                    if CMD_ARGS.flatpak_mpv and self.os == "Linux": # Support for MPV on Flatpak.
+                    if (
+                        CMD_ARGS.flatpak_mpv and self.os == "Linux"
+                    ):  # Support for MPV on Flatpak.
                         print("Using flatpak installation of MPV.")
                         return subprocess.Popen(
                             ["flatpak", "run", "io.mpv.Mpv"] + mpv_args
                         )
 
-                    return subprocess.Popen(
-                        ["mpv"] + mpv_args
-                    )
+                    if CMD_ARGS.vlc:
+                        vlc_args = [
+                            "vlc",
+                            f'--http-referrer="{referrer}"',
+                            f'"{url}"',
+                            f'--meta-title="mov-cli:{media_title}"',
+                            "--no-terminal",
+                        ]
+                        try:
+                            return subprocess.Popen(vlc_args)
+                        except:
+                            raise PlayerNotFound(self)
+                    return subprocess.Popen(["mpv"] + mpv_args)
 
                 elif self.os == "Darwin":
                     return subprocess.Popen(
                         [
                             "iina",
                             "--no-stdin",
                             "--keep-running",
                             f"--mpv-referrer={referrer}",
                             url,
                             f"--mpv-force-media-title=mov-cli:{media_title}",
                         ]
                     )
 
                 else:
-                    print("[!] Could not determine what Player to use on your OS")
-                    sys.exit(1)
+                    raise Exception(
+                        "[!] Could not determine what Player to use on your OS"
+                    )
 
             except ModuleNotFoundError:
                 raise PlayerNotFound(self)
```

### Comparing `mov_cli-1.4.5/mov_cli/utils/httpclient.py` & `mov_cli-1.4.6/mov_cli/utils/httpclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import sys
 
 import httpx
 
-default_header: dict = {
+DEFAULT_HEADERS: dict = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
     "Chrome/80.0.3987.163 "
     "Safari/537.36",
     "Accept-Language": "en-GB,en;q=0.5",
 }
 
 
 class HttpClient:
     def __init__(self, headers: dict = None, cookies: dict = None):
         if headers is None:
-            headers = default_header
+            headers = DEFAULT_HEADERS
         self.session = httpx.Client(timeout=10.0, headers=headers, cookies=cookies)
 
     def get(self, page: str, redirects: bool = False) -> httpx.Response:
         print(page)
         try:
             req = self.session.get(page, follow_redirects=redirects)
             self.session.headers["Referer"] = page
-        except Exception as e:
+        except httpx.TimeoutException:
             print(
-                f"Error: {e}",
+                f"Error: Timeout",
                 "\n Please open an issue if this is not due to your internet connection",
             )
             sys.exit(-1)
         return req
 
     def post(self, page: str, data: dict = None, json=None) -> httpx.Response:
         print(page)
         if json is None:
             try:
                 req = self.session.post(page, data=data)
                 self.session.headers["Referer"] = page
-            except Exception as e:
+            except httpx.TimeoutException:
                 print(
-                    f"Error: {e}",
+                    f"Error: Timeout",
                     "\n Please open an issue if this is not due to your internet connection",
                 )
                 sys.exit(-1)
             return req
         else:
             try:
                 req = self.session.post(page, json=json)
                 self.session.headers["Referer"] = page
-            except Exception as e:
+            except httpx.TimeoutException:
                 print(
-                    f"Error: {e}",
+                    f"Error: Timeout",
                     "\n Please open an issue if this is not due to your internet connection",
                 )
                 sys.exit(-1)
             return req
 
-    def head(self, page: str, redirects: False) -> httpx.Response:
+    def head(self, page: str, redirects: bool = False) -> httpx.Response:
         print(page)
         try:
             req = self.session.head(page, follow_redirects=redirects)
             self.session.headers["Referer"] = page
-        except Exception as e:
+        except httpx.TimeoutException:
             print(
-                f"Error: {e}",
+                f"Error: Timeout",
                 "\n Please open an issue if this is not due to your internet connection",
             )
             sys.exit(-1)
         return req
 
     def set_headers(self, header: dict) -> None:
         self.session.headers = header
```

### Comparing `mov_cli-1.4.5/mov_cli/utils/lang.py` & `mov_cli-1.4.6/mov_cli/utils/lang.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,64 @@
 import httpx
-import platform as pf
-import os
-from os import environ
-import json
 from fzf import fzf_prompt
-
-sel = eval(
-    httpx.get("https://raw.githubusercontent.com/mov-cli/translations/main/langs").text
-)
-
-
-def homepath() -> str:
-    plt = pf.system()
-    if plt == "Windows":
-        username = environ["username"]
-        return f"C:/Users/{username}/"
-    elif (plt == "Linux") or (plt == "Darwin"):
-        return f"/home/{os.getlogin()}/"
-
+from .props import home
+import mov_cli.__main__ as mc
+from json import loads
+from .props import RestartNeeded, LanguageNotAOption
+from pkgutil import get_data
+
+langsfile = get_data(__name__, "lang/langs")
+
+sel = eval(langsfile)
+
+def existing(language: str, g=False):
+    js = loads(langsfile)
+
+    exist = False
+
+    if g is False:
+        for _, value in js.items():
+            if value == language:
+                exist = True
+        if not exist:
+            raise LanguageNotAOption(language)
+    else:
+        for _, value in js.items():
+            if value == language:
+                exist = True
+        return exist
 
 def getlang():
     try:
-        with open(homepath() + "lang.json", "r") as f:
-            t = json.load(f)
+        with open(home() + "lang.mov-cli", "r") as f:
+            lang = f.read()
+        existing(lang)
+        t = loads(get_data(__name__, f"lang/{lang}.json"))
         ask = t["ASK"]
         ex = t["EXIT"]
         searcha = t["SEARCHA"]
         download = t["DOWNLOAD"]
         spro = t["SPROVIDER"]
         dshow = t["DSHOW"]
         dseason = t["DSEASON"]
         season = t["SEASON"]
         episode = t["EPISODE"]
         change = t["CHANGE"]
         t = [ask, ex, searcha, download, spro, dshow, dseason, season, episode, change]
         return t
     except FileNotFoundError:
-        t = httpx.get(
-            "https://raw.githubusercontent.com/mov-cli/translations/main/languages/en.json"
-        ).json()
-        ask = t["ASK"]
-        ex = t["EXIT"]
-        searcha = t["SEARCHA"]
-        download = t["DOWNLOAD"]
-        spro = t["SPROVIDER"]
-        dshow = t["DSHOW"]
-        dseason = t["DSEASON"]
-        season = t["SEASON"]
-        episode = t["EPISODE"]
-        change = t["CHANGE"]
-        t = [ask, ex, searcha, download, spro, dshow, dseason, season, episode, change]
-        return t
-    except json.decoder.JSONDecodeError:
-        plt = pf.system()
-        if plt == "Windows":
-            username = environ["username"]
-            print(
-                rf"Please delete the lang.json in this directory: C:\Users\{username}"
-            )
-            exit(0)
-        elif (plt == "Linux") or (plt == "Darwin"):
-            print(
-                f"Please delete the lang.json in this directory: /home/{os.getlogin()}/"
-            )
-            exit(0)
+        import locale
 
+        localLang = locale.getdefaultlocale()[0][:2]
+        check = existing(localLang, True)
+        if check is True:
+            lang = localLang
+        else:
+            lang = "en"
+        open(home() + "lang.mov-cli", "w").write(lang)
+        print(f"[?] Your Language was set to {lang}")
+        raise RestartNeeded
 
 def setlang():
     s = fzf_prompt(sel)
     selection = sel.get(s)
-    print(selection)
-    txt = httpx.get(
-        f"https://raw.githubusercontent.com/mov-cli/translations/main/languages/{selection}.json"
-    ).text
-    with open(homepath() + "lang.json", "w") as f:
-        f.write(txt)
+    open(home() + "lang.mov-cli", "w").write(selection)
```

### Comparing `mov_cli-1.4.5/mov_cli/utils/player.py` & `mov_cli-1.4.6/mov_cli/utils/player.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     def display_name(self) -> str:
         """Returns display name of player."""
         return self.__display_name
 
     @property
     def os(self) -> str:
         """
-        Returns the operating system we're currently running on. (Adds android detection.)
+        Returns the operating system we're currently running on.
 
-        E.g. Windows, Linux, Android, Darwin
+        E.g. Windows, Linux, Android, Darwin, iOS
         """
         if self.__os == "Linux":
             if hasattr(sys, "getandroidapilevel"):
                 return "Android"
             elif "ish" in self.__platform:
                 return "iOS"
             return self.__os
```

### Comparing `mov_cli-1.4.5/mov_cli/utils/scraper.py` & `mov_cli-1.4.6/mov_cli/utils/scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,24 @@
-import logging
-import os
-
-# import platform
+from platform import system as pf
 import re
 import subprocess
-import sys
 
 import mov_cli.__main__ as movcli
 from fzf import fzf_prompt
 
 from .httpclient import HttpClient
 from .lang import getlang, setlang
 from .player import PlayerNotFound
 from ..players.player import ply
 from ..extractors.doodstream import dood
+from ..extractors.tukipasti import tukipasti
 
 # import shlex
 # required for development
 
-# Not needed
-# def determine_path() -> str:
-#    plt = platform.system()
-#    if plt == "Windows":
-#        return f"C://Users//{os.getenv('username')}//Downloads"
-#    elif (plt == "Linux") or (plt == "Darwin"):
-#        return f"/home/{os.getlogin()}/Downloads"
-#    else:
-#        print("Please open an issue for your os")
-#        sys.exit(-2)
-
 
 class WebScraper:
     def __init__(self, base_url: str) -> None:
         self.client = HttpClient()
         self.base_url = base_url
         (self.title, self.url, self.aid, self.mv_tv) = (0, 1, 2, 3)
         self.translated = getlang()
@@ -45,14 +31,16 @@
             self.dshow,
             self.dseason,
             self.tse,
             self.tep,
             self.change,
         ) = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
         self.scraper = self.parser()
+        self.dseasonp = False
+        self.dshowp = False
         pass
 
     def parser(self):
         try:
             import lxml
 
             return "lxml"
@@ -69,15 +57,15 @@
         name: str,
         subtitle: str = None,
         season="",
         episode=None,
         referrer: str = None,
     ):
         name = self.parse(name)
-        fixname = re.sub(r"-+", " ", name)
+        fixname = re.sub(r"-+ +", " ", name)
         if episode:
             fixname = f"{fixname} S{season}E{episode}"
 
         if referrer:
             referrer = referrer
         else:
             referrer = self.base_url
@@ -93,45 +81,43 @@
             f"{url}",
             "-c",
             "copy",
             f"{fixname}.mp4",
         ]
 
         if subtitle:
-            # args.extend(f'-vf subtitle="{subtitle}" {self.parse(name)}.mp4')
             args.extend(["-vf", f"subtitle={subtitle}", f"{fixname}.mp4"])
         ffmpeg_process = subprocess.Popen(args)
         ffmpeg_process.wait()
-
-        return print(f"Downloaded at {os.getcwd()}")
+        return
 
     def play(self, url: str, name: str, referrer=None):
         if referrer is None:
             referrer = self.base_url
         try:
             ply_process = ply(self).play(url, referrer, name)
             ply_process.wait()
         except PlayerNotFound as e:
-            txt = f"{self.red('[!]')} Could not play {name}: Correct Player for your OS was not found| {e}"
+            txt = f"[!] Could not play: Correct Player for your OS was not found | {e}"
             # logging.log(logging.ERROR, txt)
             print(txt)  # TODO implement logging to a file
-            sys.exit(1)
+            exit(1)
 
     def search(self, q: str = None) -> str:
         pass
         # return NotImplementedError()
 
     def results(self, data: str) -> list:
         pass
         # return NotImplementedError()
 
-    def TV_PandDP(self, t: list, state: str = "d" or "p"):
+    def TV_PandDP(self, t: list, state: str):
         pass
 
-    def MOV_PandDP(self, m: list, state: str = "d" or "p"):
+    def MOV_PandDP(self, m: list, state: str):
         pass
 
     def SandR(self, q: str = None):
         return self.results(self.search(q))
 
     def display(self, q: str = None, result_no: int = None):
         result = self.SandR(q)
@@ -140,116 +126,93 @@
             r.append(f"[{ix + 1}] {vl[self.title]} {vl[self.mv_tv]}")
         r.extend(
             [
                 f"[q] {self.translated[self.exit]}",
                 f"[s] {self.translated[self.searcha]}",
                 f"[d] {self.translated[self.download]}",
                 f"[p] {self.translated[self.sprovider]}",
-                f"[sd] {self.translated[self.dshow]}",
-                f"[ds] {self.translated[self.dseason]}",
                 f"[c] {self.translated[self.change]}",
             ]
         )
         r = r[::-1]
         choice = ""
         while choice not in range(len(result) + 1):
-            pre = fzf_prompt(r)
-            choice = re.findall(r"\[(.*?)\]", pre)[0] if not result_no else result_no
+            choice = (
+                re.findall(r"\[(.*?)\]", fzf_prompt(r))[0]
+                if not result_no
+                else result_no
+            )
             if choice == "q":
-                sys.exit()
+                exit()
             elif choice == "s":
                 return self.redo()
             elif choice == "p":
                 return movcli.movcli()
             elif choice == "c":
                 setlang()
                 return movcli.movcli()
             elif choice == "d":
                 try:
-                    pre = fzf_prompt(r)
-                    choice = (
-                        re.findall(r"\[(.*?)\]", pre)[0] if not result_no else result_no
-                    )
-                    mov_or_tv = result[int(choice) - 1]
-                    if mov_or_tv[self.mv_tv] == "TV":
-                        self.TV_PandDP(mov_or_tv, "d")
+                    modes = [f"[d] {self.translated[self.download]}"]
+                    if self.dshowp and self.dseasonp:
+                        modes.extend(
+                            [
+                                f"[s] {self.translated[self.dshow]}",
+                                f"[e] {self.translated[self.dseason]}",
+                            ]
+                        )
+                    elif self.dseasonp is True:
+                        modes.append(f"[e] {self.translated[self.dseason]}")
+                    elif self.dshowp is True:
+                        modes.append(f"[s] {self.translated[self.dshow]}")
                     else:
-                        self.MOV_PandDP(mov_or_tv, "d")
-                except ValueError as e:
-                    print(
-                        "[!]  Invalid Choice Entered! | ",
-                        str(e),
-                    )
-                    sys.exit(1)
-                except IndexError as e:
-                    print(
-                        "[!]  This Episode is coming soon! | ",
-                        str(e),
-                    )
-                    sys.exit(2)
-            elif choice == "sd":
-                try:
-                    pre = fzf_prompt(r)
+                        pass
+                    modes = modes[::-1]
+                    mode = fzf_prompt(modes, header="Select a mode:")[1]
                     choice = (
-                        re.findall(r"\[(.*?)\]", pre)[0] if not result_no else result_no
+                        re.findall(r"\[(.*?)\]", fzf_prompt(r))[0]
+                        if not result_no
+                        else result_no
                     )
                     mov_or_tv = result[int(choice) - 1]
                     if mov_or_tv[self.mv_tv] == "TV":
-                        self.TV_PandDP(mov_or_tv, "sd")
+                        self.TV_PandDP(mov_or_tv, mode)
                     else:
-                        print("You selected a Movie")
-                        exit(0)
+                        if mode == "e" or mode == "s":
+                            print(
+                                "Those options are not unavailable for movies. Using d."
+                            )
+                            mode = "d"
+                        self.MOV_PandDP(mov_or_tv, mode)
                 except ValueError as e:
                     print(
                         "[!]  Invalid Choice Entered! | ",
                         str(e),
                     )
-                    sys.exit(1)
+                    exit(1)
                 except IndexError as e:
                     print(
                         "[!]  This Episode is coming soon! | ",
                         str(e),
                     )
-                    sys.exit(2)
-            elif choice == "ds":
-                try:
-                    pre = fzf_prompt(r)
-                    choice = (
-                        re.findall(r"\[(.*?)\]", pre)[0] if not result_no else result_no
-                    )
-                    mov_or_tv = result[int(choice) - 1]
-                    if mov_or_tv[self.mv_tv] == "TV":
-                        self.TV_PandDP(mov_or_tv, "ds")
-                    else:
-                        print("You selected a Movie")
-                        exit(0)
-                except ValueError as e:
-                    print(
-                        "[!]  Invalid Choice Entered! | ",
-                        str(e),
-                    )
-                    sys.exit(1)
-                except IndexError as e:
-                    print(
-                        "[!]  This Episode is coming soon! | ",
-                        str(e),
-                    )
-                    sys.exit(2)
+                    exit(2)
             else:
                 mov_or_tv = result[int(choice) - 1]
                 if mov_or_tv[self.mv_tv] == "TV":
                     self.TV_PandDP(mov_or_tv, "p")
                 else:
                     self.MOV_PandDP(mov_or_tv, "p")
 
+    def tuki(self, html: str):
+        return tukipasti(html)
+
     def doodstream(self, url: str):
         return dood(url)
 
     def redo(self, search: str = None, result: int = None):
-        print(result)
         return self.display(search, result)
 
     def askseason(self, seasons: int):
         texts = []
         for i in range(seasons):
             texts.append(f"{self.translated[self.tse]} {i+1}")
         choice = fzf_prompt(texts).split(" ")[-1]
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/animefox.py` & `mov_cli-1.4.6/mov_cli/websites/international/wlext.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,105 @@
-from ..utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
+from ...utils.scraper import WebScraper
+from ...utils.props import NoSupportedProvider, SelectedNotAvailable
 import re
 
 
-class animefox(WebScraper):
-    def __init__(self, base_url):
+class Provider(WebScraper):
+    def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
-        req = self.client.get(f"https://animefox.to/search?keyword={data}")
-        soup = BS(req, self.scraper)
-        items = soup.findAll("a", {"class": "film-poster-ahref"})
-        urls = [items[i]["href"] for i in range(len(items))]
-        title = [items[i]["title"] for i in range(len(items))]
-        ids = [i for i in range(len(items))]
-        mov_or_tv = [
-            "MOVIE" if items[i].__contains__("Movie") else "TV"
-            for i in range(len(items))
+        m = self.client.get(
+            f"{self.base_url}/ptb-search/?f=search_movies&ptb-search=1&title={data}"
+        )
+        s = self.client.get(
+            f"{self.base_url}/ptb-search/?f=search_series_1&ptb-search=1&title={data}"
+        )
+        show = BS(s, self.scraper)
+        shows = show.findAll("h5", {"class": "ptb_post_title"})
+        movie = BS(m, self.scraper)
+        movies = movie.findAll("h5", {"class": "ptb_post_title"})
+        urls = [movies[i].find("a")["href"] for i in range(len(movies))] + [
+            shows[i].find("a")["href"] for i in range(len(shows))
+        ]
+        title = [movies[i].find("a").text for i in range(len(movies))] + [
+            shows[i].find("a").text for i in range(len(shows))
+        ]
+        ids = [i for i in range(len(movies))] + [i for i in range(len(shows))]
+        mov_or_tv = ["MOVIE" for i in range(len(movies))] + [
+            "TV" for i in range(len(shows))
         ]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        a = self.client.get(f"{self.base_url}{url}")
-        soup = BS(a, self.scraper)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        req = self.client.get(self.base_url + url)
+        req = self.client.get(url)
         soup = BS(req, self.scraper)
-        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
-        episode = self.askepisode(episodes)
-        return self.base_url + url[:-1] + episode, episode
-
-    def mov(self, url):
-        a = self.client.get(f"{self.base_url}{url}")
-        soup = BS(a, self.scraper)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        return self.base_url + url
+        t = soup.find("select", {"id": "loadepisode"})
+        try:
+            episodes = len(t.findAll("option"))
+        except:
+            raise SelectedNotAvailable
+        episode = int(self.askepisode(episodes))
+        req = self.client.get(f"{url}?server=cajitatop&episode={episode}").text
+        soup = BS(req, self.scraper)
+        try:
+            t = soup.find("iframe", {"loading": "lazy"})["src"]
+            print(t)
+        except:
+            raise NoSupportedProvider
+        return t, episode
 
     def cdn_url(self, url):
-        req = self.client.get(url)
-        soup = BS(req, self.scraper)
-        goload = soup.find("select", {"id": "select-iframe-to-display"}).findAll(
-            "option"
-        )[-1]["value"]
-        url = f"https://{goload}".split("-")[0]
-        a = self.client.head(url, redirects=False).headers["location"]
-        a = self.client.get(a)
-        soup = BS(a, self.scraper)
-        server = []
-        servers = soup.findAll("li", {"class": "linkserver"})
-        for video in servers:
-            if "dood.wf" in str(video["data-video"]):
-                server.append(video["data-video"])
-        return self.doodstream(server[0])
-
-    def doodstream(self, url):
-        domain = re.findall("""([^"']*)\/e""", url)[0]
-        req = self.client.get(url).text
-        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
-        token = pass_md.split("/")[-1]
-        self.client.set_headers(
-            {
-                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
-                "Referer": f"{url}",
-                "Accept-Language": "en-GB,en;q=0.5",
-            }
-        )
-        drylink = self.client.get(f"{domain}{pass_md}").text
-        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
-        print(streamlink)
-        return streamlink
+        self.client.set_headers({"origin": "cajita.top", "referer": f"{url}"})
+        string = re.findall("""v\/([^"']*)""", url)[0]
+        request = self.client.post(
+            f"https://cajita.top/api/source/{string}",
+            data={"r": f"{self.base_url}", "d": "cajita.top"},
+        ).json()
+        file = request["data"]
+        if file == "Video not found or has been removed":
+            raise SelectedNotAvailable
+        else:
+            file = request["data"][-1]["file"]
+        return file
 
     def download(self, t):
-        a = self.client.get(f"{self.base_url}{t[self.url]}")
-        soup = BS(a, self.scraper)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        req = self.client.get(self.base_url + url)
+        req = self.client.get(t[self.url])
         soup = BS(req, self.scraper)
-        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
-        for e in range(episodes):
-            url = self.cdn_url(self.base_url + url[:-1] + e + 1)
-            self.dl(url, name=t[self.title], episode=e + 1)
+        t = soup.find("select", {"id": "loadepisode"})
+        try:
+            episodes = len(t.findAll("option"))
+        except:
+            return print("Episode unavailable")
+        for e in range(len(episodes)):
+            req = self.client.get(f"{[self.url]}?server=cajitatop&episode={e+1}").text
+            soup = BS(req, self.scraper)
+            try:
+                t = soup.find("iframe", {"loading": "lazy"})["src"]
+            except:
+                raise SelectedNotAvailable
+            url = str(self.cdn_url(t))
+            self.dl(url, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
-        if state == "sd":
-            self.download(t)
-            return
         name = t[self.title]
-        link, episode = self.ask(t[self.url])
-        url = self.cdn_url(link)
+        url, episode = self.ask(t[self.url])
+        url = str(self.cdn_url(url))
         if state == "d":
             self.dl(url, name, season=".", episode=episode)
             return
         self.play(url, name)
 
-    def MOV_PandDP(self, t: list, state: str = "d" or "p"):
-        name = t[self.title]
-        link = self.mov(t[self.url])
-        url = self.cdn_url(link)
+    def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
+        name = m[self.title]
+        url, episode = self.ask(m[self.url])
+        url = self.cdn_url(url)
         if state == "d":
             self.dl(url, name)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/dopebox.py` & `mov_cli-1.4.6/mov_cli/websites/english/dopebox.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-from .actvid import actvid
+from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 
 
-class dopebox(actvid):
+class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
-        self.rep_key = "6LeWLCYeAAAAAL1caYzkrIY-M59Vu41vIblXQZ48"
-        # self.redo()
-
-    """def cdn_url(self, rabbid, rose, num):
-        self.client.set_headers({"X-Requested-With": "XMLHttpRequest"})
-        # data = json.loads(self.client.get(
-        #    f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"))['sources'][0][
-        #    'file']
-        data = json.loads(
-            self.client.get(
-                f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
-            ).text
-        )["sources"][0]["file"]
-        return data"""
+        self.dseasonp = True
+        self.dshowp = True
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
@@ -54,14 +42,21 @@
         return text
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
+    def get_link(self, thing_id: str) -> tuple:
+        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()[
+            "link"
+        ]
+        print(req)
+        return req, self.rabbit_id(req)
+
     def ep_server_id(self, ep_id):
         rem = self.client.get(
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/einthusan.py` & `mov_cli-1.4.6/mov_cli/websites/indian/einthusan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
 import re
 from fzf import fzf_prompt
 
 
-class einthusan(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/eja.py` & `mov_cli-1.4.6/mov_cli/websites/livetv/eja.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import httpx
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
+from re import findall
 
 
-class eja(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
         self.headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:80.0) Gecko/20100101 Firefox/80.0"
         }
 
@@ -24,25 +24,18 @@
         urls = [col[i].findAll("a")[1]["href"] for i in range(len(col))]
         title = [col[i].findAll("a")[1].text for i in range(len(col))]
         ids = [col[i].findAll("a")[1]["href"].strip("?") for i in range(len(col))]
         mov_or_tv = [col[i].findAll("img")[0]["alt"] for i in range(len(col))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def get_hls(self, url):
-        link = str(httpx.get(f"https://eja.tv/?{url}", follow_redirects=True).url)
-        print(link)
-        link = "".join(link)
-        link = link.split("?")[1]
-        link = link.split("#")[0]
-        print(link)
-        return link
+        link = self.client.get(f"https://eja.tv/?{url}", redirects=True)
+        link = link.url
+        return findall("\?(.*)#", link)[0]
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
         name = m[self.title]
         url = self.get_hls(m[self.aid])
         if state == "d":
             self.dl(url, name)
             return
         self.play(url, name)
-
-    def SandR(self, q: str = None):
-        return self.results(self.search(q))
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.6/mov_cli/websites/anime/gogoanime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
 import re
 
 
-class gogoanime(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "-")
 
     def results(self, data: str) -> list:
         results = []
         page = 1
         while True:
-            req = self.client.get(f"{self.base_url}/search.html?keyword={data}&page={page}")
+            req = self.client.get(
+                f"{self.base_url}/search.html?keyword={data}&page={page}"
+            )
             soup = BS(req, self.scraper)
             items = soup.find("ul", {"class": "items"}).findAll("li")
-            if len(items) == 0: break
+            if len(items) == 0:
+                break
             urls = [items[i].find("a")["href"] for i in range(len(items))]
             title = [items[i].find("a")["title"] for i in range(len(items))]
             ids = [items[i].find("a")["title"] for i in range(len(items))]
             mov_or_tv = ["TV" for i in range(len(items))]
-            results.extend([list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)])
+            results.extend(
+                [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
+            )
             page += 1
         return results
 
     def ask(self, url):
         req = self.client.get(f"{self.base_url}{url}")
         soup = BS(req, self.scraper)
         episodes = soup.find("ul", {"id": "episode_page"}).find_all("a")[-1]["ep_end"]
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.6/mov_cli/websites/cartoons/kisscartoon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 import re
 import httpx
 
 cdn_url_re = r"/\\\/cdn\\\/hls\\\/([a-fA-F\d]{32})\\\/master\.txt/gm"
 
 
-class kisscartoon(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.6/mov_cli/websites/asian/watchasian.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,87 @@
+from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+import re
 
 
-class openloadmov(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
-        self.getvid = "https://hlspanel.xyz/player/index.php?data={}&do=getVideo"
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
-    def results(self, data: str) -> list:
-        req = self.client.get(f"{self.base_url}/?s={data}")
+    def results(self, data: str):
+        req = self.client.get(f"{self.base_url}/search?type=movies&keyword={data}").text
         soup = BS(req, self.scraper)
-        items = soup.findAll("div", {"class": "result-item"})
-        title = [items[i].find("img")["alt"] for i in range(len(items))]
-        urls = [items[i].find("a")["href"] for i in range(len(items))]
-        ids = [i for i in range(len(items))]
-        mov_or_tv = [
-            "MOVIE" if items[i].find("span").text.__contains__("Movie") else "TV"
-            for i in range(len(items))
-        ]
+        ul = soup.find("ul", {"class": "switch-block list-episode-item"}).findAll("li")
+        urls = [ul[i].find("a")["href"] for i in range(len(ul))]
+        title = [ul[i].find("h3").text for i in range(len(ul))]
+        ids = ["1" for i in range(len(ul))]
+        mov_or_tv = ["TV" for i in range(len(ul))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        req = self.client.get(url)
+        req = self.client.get(f"{self.base_url}{url}").text
         soup = BS(req, self.scraper)
-        seasons = soup.findAll("div", {"class": "se-c"})
-        season = int(self.askseason(len(seasons)))
-        se_c = seasons[season - 1]
-        episodes = se_c.find("ul").findAll("li")
+        episodes = soup.find(
+            "ul", {"class": "list-episode-item-2 all-episode"}
+        ).findAll("li")
         episode = int(self.askepisode(len(episodes)))
-        ep = episodes[episode - 1].find("a")["href"]
-        return ep, episode, season
+        episodes = episodes[::-1]
+        href = episodes[episode - 1].find("a")["href"]
+        q = self.client.get(self.base_url + href).text
+        soup = BS(q, self.scraper)
+        if re.search("doodstream", q):
+            li = soup.find("li", {"class": "doodstream"})["data-video"]
+        else:
+            raise Exception("Unable to find URL")
+        return li, episode
+
+    def doodstream(self, url):
+        domain = re.findall("""([^"']*)\/e""", url)[0]
+        req = self.client.get(url).text
+        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
+        token = pass_md.split("/")[-1]
+        self.client.set_headers(
+            {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
+                "Referer": f"{url}",
+                "Accept-Language": "en-GB,en;q=0.5",
+            }
+        )
+        drylink = self.client.get(f"{domain}{pass_md}").text
+        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
+        print(streamlink)
+        return streamlink
 
-    def cdn_url(self, url):
-        req = self.client.get(url)
+    def download(self, t):
+        req = self.client.get(f"{self.base_url}{t[self.url]}").text
         soup = BS(req, self.scraper)
-        iframe = soup.find("iframe")["src"]
-        vidhash = iframe.split("/")[-1]
-        self.client.set_headers({"x-requested-with": "XMLHttpRequest"})
-        awd = self.client.post(
-            self.getvid.format(vidhash),
-            data={"hash": vidhash, "r": self.base_url + "/"},
-        ).json()["securedLink"]
-        print(awd)
-        return awd
+        episodes = soup.find(
+            "ul", {"class": "list-episode-item-2 all-episode"}
+        ).findAll("li")
+        episodes = episodes[::-1]
+        for e in range(len(episodes)):
+            href = episodes[e].find("a")["href"]
+            q = self.client.get(self.base_url + href).text
+            soup = BS(q, self.scraper)
+            if re.search("doodstream", q):
+                li = soup.find("li", {"class": "doodstream"})["data-video"]
+            else:
+                raise Exception("Unable to find URL")
+            url = self.doodstream(li)
+            self.dl(url, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
-        name = t[self.title]
-        url, episode, season = self.ask(t[self.url])
-        url = self.cdn_url(url)
-        if state == "d":
-            self.dl(url, name, season=season, episode=episode)
+        if state == "sd":
+            self.download(t)
             return
-        self.play(url, name)
-
-    def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
-        name = m[self.title]
-        url = self.cdn_url(m[self.url])
+        name = t[self.title]
+        link, episode = self.ask(t[self.url])
+        url = self.doodstream(link)
         if state == "d":
-            self.dl(url, name)
+            self.dl(url, name, season=".", episode=episode)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.6/mov_cli/websites/turkish/turkish123.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,65 @@
+from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
 import re
 
 
-class kimcartoon(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
-        return q
+        return q.replace(" ", "+")
 
-    def results(self, q):
-        res = self.client.post(f"{self.base_url}/Search/Cartoon", data={"keyword": q})
-        soup = BS(res.text, self.scraper)
-        div = soup.find("div", {"class": "list-cartoon"})
-        cartoons = div.findAll("div", {"class": "item"})
-        title = [cartoons[i].find("span").text for i in range(len(cartoons))]
-        urls = [cartoons[i].find("a")["href"] for i in range(len(cartoons))]
-        ids = [i for i in range(len(cartoons))]
-        mov_or_tv = ["TV" for i in range(len(cartoons))]
+    def results(self, data: str) -> list:
+        req = self.client.get(f"{self.base_url}/?s={data}").text
+        soup = BS(req, self.scraper)
+        mlitem = soup.findAll("div", {"class": "ml-item"})
+        items = []
+        for i in range(len(mlitem)):
+            if str(mlitem[i]).__contains__("episode"):
+                pass
+            else:
+                items.append(mlitem[i])
+        urls = [items[i].find("a")["href"] for i in range(len(items))]
+        title = [items[i].find("a")["oldtitle"] for i in range(len(items))]
+        ids = [items[i]["class"] for i in range(len(items))]
+        mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        res = self.client.get(self.base_url + url)
-        soup = BS(res, self.scraper)
-        table = soup.find("table", {"class": "listing"})
-        episodes = table.findAll("a", {"rel": "noreferrer noopener"})
+        req = self.client.get(url).text
+        soup = BS(req, self.scraper)
+        episodes = soup.findAll("a", {"class": "episodi"})
         episode = int(self.askepisode(len(episodes)))
-        url = episodes[len(episodes) - episode]["href"]
-        return url, episode
-
-    def download(self, t: list):
-        res = self.client.get(self.base_url + t[self.url])
-        soup = BS(res, self.scraper)
-        table = soup.find("table", {"class": "listing"})
-        episodes = table.findAll("a", {"rel": "noreferrer noopener"})
+        req = self.client.get(episodes[episode - 1]["href"]).text
+        url, tukibase = self.tuki(req)
+        return url, episode, tukibase
+
+    def download(self, t):
+        req = self.client.get(t[self.url]).text
+        soup = BS(req, self.scraper)
+        episodes = soup.findAll("a", {"class": "episodi"})
         for e in range(len(episodes)):
-            epi = e + 1
-            link = episodes[len(episodes) - epi]["href"]
-            url = self.cdn_url(link)
-            self.dl(url, t[self.title], episode=e + 1)
-
-    def cdn_url(self, url):
-        res = self.client.get(self.base_url + url + "&s=sb").text
-        iframe_id = re.findall('''src="https:\/\/www.luxubu.review\/v\/(.*?)\"''', res)[
-            0
-        ]
-        r = self.client.post(
-            f"https://www.luxubu.review/api/source/{iframe_id}", data=None
-        ).json()["data"]
-        return r[-1]["file"]
+            req = self.client.get(episodes[e]["href"]).text
+            url, tukibase = self.tuki(req)
+            print(url)
+            self.dl(
+                url,
+                t[self.title],
+                season="",
+                episode=e + 1,
+                referrer=tukibase,
+            )
 
-    def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
+    def TV_PandDP(self, t: list, state: str):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
-        link, episode = self.ask(t[self.url])
-        url = self.cdn_url(link)
+        url, episode, ref = self.ask(t[self.url])
         if state == "d":
             self.dl(url, name, season=".", episode=episode)
             return
-        self.play(url, name)
+        self.play(url, name, referrer=ref)
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/remotestream.py` & `mov_cli-1.4.6/mov_cli/websites/english/remotestream.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 import re
+from ...utils.props import SelectedNotAvailable
 
 
-class remotestream(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
         self.movdb = "https://www.themoviedb.org"
+        self.dseasonp = False
+        self.dshowp = True
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
 
     def results(self, data: str) -> list:
         title = []
         urls = []
         ids = []
         mov_or_tv = []
-        tv = self.client.get(self.movdb + f"/search/tv?query={data}&language=en").text
-        movie = self.client.get(
-            self.movdb + f"/search/movie?query={data}&language=en"
-        ).text
-        # MOVIE
-        soupm = BS(movie, self.scraper)
-        mcards = soupm.findAll("div", {"class": "card v4 tight"})
-        if mcards is not []:
-            title.extend([mcards[i].find("h2").text for i in range(len(mcards))])
-            urls.extend(["" for i in range(len(mcards))])
-            ids.extend(
-                [
-                    mcards[i].find("a")["href"].split("/")[-1].split("?")[0]
-                    for i in range(len(mcards))
-                ]
-            )
-            mov_or_tv.extend(["MOVIE" for i in range(len(mcards))])
-        soups = BS(tv, self.scraper)
-        scards = soups.findAll("div", {"class": "card v4 tight"})
-        if scards is not []:
-            title.extend([scards[i].find("h2").text for i in range(len(scards))])
-            urls.extend(["" for i in range(len(scards))])
-            ids.extend(
-                [
-                    scards[i].find("a")["href"].split("/")[-1].split("?")[0]
-                    for i in range(len(scards))
-                ]
-            )
-            mov_or_tv.extend(["TV" for i in range(len(scards))])
+        for i in range(2):
+            if i == 0:
+                get = "movie"
+            else:
+                get = "tv"
+            req = self.client.get(
+                self.movdb + f"/search/{get}?query={data}&language=en"
+            ).text
+            soup = BS(req, self.scraper)
+            cards = soup.findAll("div", {"class": "card v4 tight"})
+            if cards is not []:
+                title.extend([cards[i].find("h2").text for i in range(len(cards))])
+                urls.extend(["" for i in range(len(cards))])
+                ids.extend(
+                    [
+                        cards[i].find("a")["href"].split("/")[-1].split("?")[0]
+                        for i in range(len(cards))
+                    ]
+                )
+                mov_or_tv.extend([get.upper() for i in range(len(cards))])
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, id):
         rlurl = self.client.head(f"{self.movdb}/tv/{id}", redirects=True).url
         res = self.client.get(f"{rlurl}/seasons")
         soup = BS(res, self.scraper)
         seasons = soup.findAll("div", {"class": "season"})
@@ -76,16 +70,15 @@
         else:
             res = self.client.get(
                 f"{self.base_url}/e/?tmdb={id}&s={season}&e={episode}"
             ).text
         try:
             file = re.findall('"file":"(.*?)"', res)[0]
         except IndexError as e:
-            print("This show or movie is not available.")
-            exit(1)
+            raise SelectedNotAvailable
         return file
 
     def sd(self, name, id):
         rlurl = self.client.head(f"{self.movdb}/tv/{id}", redirects=True).url
         res = self.client.get(f"{rlurl}/seasons")
         soup = BS(res, self.scraper)
         seasons = soup.findAll("div", {"class": "season"})
@@ -105,18 +98,18 @@
         name = m[self.title]
         url = self.cdn_url(m[self.aid])
         if state == "d":
             self.dl(url, name)
             return
         self.play(url, name)
 
-    def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
-        if state == "sd":
+    def TV_PandDP(self, t: list, state: str):
+        if state == "s":
             self.sd(t[self.title], t[self.aid])
             return
         name = t[self.title]
         season, episode = self.ask(t[self.aid])
         url = self.cdn_url(t[self.aid], season, episode)
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, season=season, episode=episode)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/scdn.py` & `mov_cli-1.4.6/mov_cli/websites/sports/scdn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import re
 import importlib
 import tldextract
 from fzf import fzf_prompt
 from datetime import datetime
 from urllib.parse import urlparse
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 
 """
 Original Code from https://github.com/edl2/sportsapi
 Rewritten for mov-cli
+Needs a rework
 """
 
 
-class scdn(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
         self.sport = None
         self.extractor = tldextract.TLDExtract()
 
     def date(self):
@@ -114,19 +115,19 @@
         A = urlparse(url).netloc
         extracted_url = self.extractor(A).domain
         try:
             get_link = importlib.import_module(
                 f"..extractors.scdn.{extracted_url}.get_link"
             )
         except ImportError:
-            from ..extractors.scdn.ripple import get_link
+            from ...extractors.scdn.ripple import get_link
 
         m3u8 = get_link(url)
         return m3u8, A
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
         name = m[self.title]
         url, domain = self.cdn_url(m[self.aid])
         if state == "d":
-            self.dl(url, name)
+            self.dl(url, name, referrer=f"https://{domain}/")
             return
         self.play(url, name, referrer=f"https://{domain}/")
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/sflix.py` & `mov_cli-1.4.6/mov_cli/websites/english/sflix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-from .actvid import actvid
+from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 
 
-class sflix(actvid):
+class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
-        self.rep_key = "6LeWLCYeAAAAAL1caYzkrIY-M59Vu41vIblXQZ48"
-        # self.redo()
-
-    """def cdn_url(self, rabbid, rose, num):
-        self.client.set_headers({"X-Requested-With": "XMLHttpRequest"})
-        # data = json.loads(self.client.get(
-        #    f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"))['sources'][0][
-        #    'file']
-        data = json.loads(
-            self.client.get(
-                f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
-            ).text
-        )["sources"][0]["file"]
-        return data"""
+        self.dseasonp = True
+        self.dshowp = True
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
-        episode = episodes[int(self.askepisode(len(episodes))) - 1]
-        ep = self.getep(
-            f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
-            data_id=episode,
-        )
+        ep = self.askepisode(len(episodes))
+        episode = episodes[int(ep) - 1]
         return episode, season, ep
 
+    def get_link(self, thing_id: str) -> tuple:
+        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()[
+            "link"
+        ]
+        print(req)
+        return req, self.rabbit_id(req)
+
+
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
         soup = BS(source, self.scraper)
 
         unformated = soup.find("div", {"data-id": f"{data_id}"})
 
         children = unformated.findChildren("div", {"class": "episode-number"})
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/solar.py` & `mov_cli-1.4.6/mov_cli/websites/english/solar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .actvid import actvid
+from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 
 
-class solar(actvid):
+class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
-        self.rep_key = "6LeWLCYeAAAAAL1caYzkrIY-M59Vu41vIblXQZ48"
-        self.redo()
+        self.dseasonp = True
+        self.dshowp = True
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
@@ -22,14 +22,22 @@
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
             episode,
         )
         return episode, season, ep
 
+    def get_link(self, thing_id: str) -> tuple:
+        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()[
+            "link"
+        ]
+        print(req)
+        return req, self.rabbit_id(req)
+
+
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
 
         soup = BS(source, self.scraper)
 
         unformated = soup.find("a", {"data-id": f"{data_id}"})["title"]
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.6/mov_cli/websites/indian/streamblasters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
+from ...utils.props import NoSupportedProvider
+
 from bs4 import BeautifulSoup as BS
 import re
 
 
-class streamblasters(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
@@ -37,15 +39,15 @@
         data = {"action": "doo_player_ajax", "post": post, "nume": "1", "type": "movie"}
         post = self.client.post(
             f"{self.base_url}/wp-admin/admin-ajax.php", data=data
         ).text
         try:
             src = re.findall('''"https:(.*?)"''', post)[0].replace("\/", "/")
         except:
-            raise Exception("No URL was found")
+            raise NoSupportedProvider
         if "\\" in src:
             src = src.replace("\\", "")
         src = f"https:{src}"
         print(src)
         return src
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.6/mov_cli/websites/indian/tamilyogi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 import re
 
 
-class tamilyogi(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/turkish123.py` & `mov_cli-1.4.6/mov_cli/websites/turkish/yoturkish.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
 import re
 
 
-class turkish123(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
-    def search(self, q: str = None) -> str:
+    def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
         soup = BS(req, self.scraper)
-        mlitem = soup.findAll("div", {"class": "ml-item"})
         items = []
+        mlitem = soup.findAll("div", {"class": "item"})
         for i in range(len(mlitem)):
             if str(mlitem[i]).__contains__("episode"):
                 pass
             else:
                 items.append(mlitem[i])
+        if soup.find_all("ul", {"class": "pagination"}):
+            pagination = soup.find("ul", {"class": "pagination"}).findAll("li")[1:]
+            for page in pagination:
+                req = self.client.get(page.find("a")["href"]).text
+                soup = BS(req, self.scraper)
+                pageitem = soup.findAll("div", {"class": "item"})
+                for i in range(len(pageitem)):
+                    if str(pageitem[i]).__contains__("episode"):
+                        pass
+                    else:
+                        items.append(pageitem[i])
         urls = [items[i].find("a")["href"] for i in range(len(items))]
-        title = [items[i].find("a")["oldtitle"] for i in range(len(items))]
+        title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [items[i]["class"] for i in range(len(items))]
         mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        req = self.client.get(url).text
+        req = self.client.get(url, True).text
         soup = BS(req, self.scraper)
-        episodes = soup.findAll("a", {"class": "episodi"})
+        episodes = soup.findAll("a", {"class": "episod"})
         episode = int(self.askepisode(len(episodes)))
-        req = self.client.get(episodes[episode - 1]["href"]).text
-        regex = r'''var copyTexti= \['<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
-        s = re.findall(regex, req)[0]
-        req = self.client.get(f"https://tukipasti.com{s}").text
-        url = re.findall("var urlPlay = '(.*?)'", req)[0]
-        print(url)
-        return url, episode, f"https://tukipasti.com{s}"
+        req = self.client.get(episodes[episode - 1]["href"], True).text
+        url, tukibase = self.tuki(req)
+        return url, episode, tukibase
 
     def download(self, t):
         req = self.client.get(t[self.url]).text
         soup = BS(req, self.scraper)
-        episodes = soup.findAll("a", {"class": "episodi"})
+        episodes = soup.findAll("a", {"class": "episod"})
         for e in range(len(episodes)):
             req = self.client.get(episodes[e]["href"]).text
-            regex = r'''var copyTexti= \['<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
-            s = re.findall(regex, req)[0]
-            req = self.client.get(f"https://tukipasti.com{s}").text
-            url = re.findall("var urlPlay = '(.*?)'", req)[0]
+            url, tukibase = self.tuki(req)
             print(url)
             self.dl(
                 url,
                 t[self.title],
                 season="",
                 episode=e + 1,
-                referrer=f"https://tukipasti.com{s}",
+                referrer=tukibase,
             )
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd" or "ds"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
```

### Comparing `mov_cli-1.4.5/mov_cli/websites/viewasian.py` & `mov_cli-1.4.6/mov_cli/websites/asian/viewasian.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bs4 import BeautifulSoup as BS
-from ..utils.scraper import WebScraper
+from ...utils.scraper import WebScraper
 import re
 
 
-class viewasian(WebScraper):
+class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "-")
@@ -51,31 +51,14 @@
             for tuple in results:
                 url = tuple[0]
                 rest = tuple[1]
             li = f"https:{url}{rest[3:]}"
             return li
         raise Exception("Video not found or removed")
 
-    #    def doodstream(self, url):
-    #        domain = re.findall("""([^"']*)\/e""", url)[0]
-    #        req = self.client.get(url).text
-    #        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
-    #        token = pass_md.split("/")[-1]
-    #        self.client.set_headers(
-    #            {
-    #                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
-    #                "Referer": f"{url}",
-    #                "Accept-Language": "en-GB,en;q=0.5",
-    #            }
-    #        )
-    #        drylink = self.client.get(f"{domain}{pass_md}").text
-    #        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
-    #        print(streamlink)
-    #        return streamlink
-
     def download(self, t):
         request = self.client.get(f"{self.base_url}{t[self.url]}")
         soup = BS(request, self.scraper)
         href = soup.find("a", {"class": "bwac-btn"})["href"]
         request = self.client.get(f"{self.base_url}{href}")
         soup = BS(request, self.scraper)
         episodes = soup.findAll("li", {"class": "ep-item"})
```

### Comparing `mov_cli-1.4.5/pyproject.toml` & `mov_cli-1.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.5"
+version = "1.4.6"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
-maintainers = ["Ananas <ananas@ad1hl.xyz>"]
+maintainers = ["Ananas <ananas@r3tr0ananas.lol>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -22,8 +22,8 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 mov-cli = "mov_cli.__main__:movcli"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/mov-cli/mov-cli/issues"
+"Bug Tracker" = "https://github.com/mov-cli/mov-cli/issues"
```

### Comparing `mov_cli-1.4.5/PKG-INFO` & `mov_cli-1.4.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: mov-cli
-Version: 1.4.5
-Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
-Home-page: https://github.com/mov-cli/mov-cli
-License: GPLv3
-Author: Pain
-Author-email: painedposeidon444@gmail.com
-Maintainer: Ananas
-Maintainer-email: ananas@ad1hl.xyz
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: krfzf-py (>=0.0.4,<0.0.5)
-Requires-Dist: pycryptodome (>=3.17,<4.0)
-Requires-Dist: six (>=1.16.0,<2.0.0)
-Requires-Dist: tldextract (>=3.4.3,<4.0.0)
-Project-URL: Bug Tracker, https://github.com/mov-cli/mov-cli/issues
-Project-URL: Repository, https://github.com/mov-cli/mov-cli
-Description-Content-Type: text/markdown
-
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
@@ -54,15 +28,15 @@
 <br />
 <div align="center">
   <a href="https://github.com/mov-cli/mov-cli">
     <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="80" height="80">
   </a>
 
   <p align="center">
- A cli tool to browse and watch Movies/Shows/TV/Sports. 
+    A cli tool to browse and watch Movies/Shows/TV/Sports. 
     <br />
     <br />
     <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
     ·
     <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
   </p>
 </div>
@@ -94,22 +68,20 @@
   <li><a href="#inspiration">inspiration</a></li>
 </ol>
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
+The new and improved mov-cli is here.
+
 mov-cli is a Commandline Tool to watch and download shows and movies.
 
-Shows and Movies are scraped from Streaming Sites.
+Shows and Movies are sourced from Streaming Sites.
 
-mov-cli currently scrapes 15 Providers:
-```
-Actvid · SFlix · Solar · DopeBox · WLEXT · KinoX · StreamBlasters · TamilYogi · Einthusan · ViewAsian · Watchasian · GogoAnime · Eja · KimCartoon · Turkish123
-```
 <p align="right">(<a href="#readme-top">back to top</a>)</p
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 
 
@@ -244,8 +216,7 @@
 [forks-url]: https://github.com/mov-cli/mov-cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli.svg?style=for-the-badge
 [stars-url]: https://github.com/mov-cli/mov-cli/stargazers
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli.svg?style=for-the-badge
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli.svg?style=for-the-badge
 [license-url]: https://github.com/mov-cli/mov-cli/blob/master/LICENSE.txt
-
```

#### html2text {}

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.5 Summary: A cli tool to
-browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
-mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
-Maintainer: Ananas Maintainer-email: ananas@ad1hl.xyz Requires-Python:
->=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
-(>=4.11.2,<5.0.0) Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: krfzf-
-py (>=0.0.4,<0.0.5) Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist:
-six (>=1.16.0,<2.0.0) Requires-Dist: tldextract (>=3.4.3,<4.0.0) Project-URL:
-Bug Tracker, https://github.com/mov-cli/mov-cli/issues Project-URL: Repository,
-https://github.com/mov-cli/mov-cli Description-Content-Type: text/markdown
-[![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
+      [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![MIT License][license-shield]][license-url]
                                     [Logo]
             A cli tool to browse and watch Movies/Shows/TV/Sports.
 
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
@@ -28,19 +15,17 @@
    3. Usage
    4. Disclaimer
    5. Contributing
    6. Adding_Languages
    7. License
    8. Contact
    9. inspiration
- ## About The Project mov-cli is a Commandline Tool to watch and download shows
-and movies. Shows and Movies are scraped from Streaming Sites. mov-cli
-currently scrapes 15 Providers: ``` Actvid Â· SFlix Â· Solar Â· DopeBox Â·
-WLEXT Â· KinoX Â· StreamBlasters Â· TamilYogi Â· Einthusan Â· ViewAsian Â·
-Watchasian Â· GogoAnime Â· Eja Â· KimCartoon Â· Turkish123 ```
+ ## About The Project The new and improved mov-cli is here. mov-cli is a
+Commandline Tool to watch and download shows and movies. Shows and Movies are
+sourced from Streaming Sites.
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
 [`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
              (https://iina.io) - player used for MacOS - [`Outplayer`](https://
   outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
        FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
   selection Menu ## Installation  ### Windows / Linux - Run this Command inside
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
```

