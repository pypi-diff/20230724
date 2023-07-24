# Comparing `tmp/Pandora-ChatGPT-1.2.9.tar.gz` & `tmp/Pandora-ChatGPT-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-1necve0v/Pandora-ChatGPT-1.2.9.tar", last modified: Thu Jul 20 10:29:24 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-fm412_qb/Pandora-ChatGPT-1.3.0.tar", last modified: Mon Jul 24 06:47:16 2023, max compression
```

## Comparing `Pandora-ChatGPT-1.2.9.tar` & `Pandora-ChatGPT-1.3.0.tar`

### file list

```diff
@@ -1,115 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:29:24.000000 Pandora-ChatGPT-1.2.9/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-07-20 10:29:11.000000 Pandora-ChatGPT-1.2.9/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305737 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:16.000000 Pandora-ChatGPT-1.3.0/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-07-24 06:47:02.000000 Pandora-ChatGPT-1.3.0/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-1.2.9/LICENSE` & `Pandora-ChatGPT-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/PKG-INFO` & `Pandora-ChatGPT-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.2.9
+Version: 1.3.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.9 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.3.0 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.2.9
+Version: 1.3.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.9 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.3.0 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Pandora-ChatGPT-1.2.9/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.3.0/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 src/pandora/py.typed
 src/pandora/bots/__init__.py
 src/pandora/bots/legacy.py
 src/pandora/bots/server.py
 src/pandora/exts/__init__.py
 src/pandora/exts/config.py
 src/pandora/exts/hooks.py
-src/pandora/exts/sentry.py
 src/pandora/exts/token.py
 src/pandora/flask/static/apple-touch-icon.png
 src/pandora/flask/static/favicon-16x16.png
 src/pandora/flask/static/favicon-32x32.png
 src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
 src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
 src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
```

### Comparing `Pandora-ChatGPT-1.2.9/README.md` & `Pandora-ChatGPT-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/setup.py` & `Pandora-ChatGPT-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/pengzhile/pandora',
     packages=find_packages('src'),
     package_dir={'pandora': 'src/pandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['pandora-cloud~=0.5.0'],
+        'cloud': ['pandora-cloud~=0.5.1'],
     },
     entry_points={
         'console_scripts': [
             'pandora = pandora.launcher:run',
             'pandora-cloud = pandora.cloud_launcher:run',
         ]
     },
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.3.0/src/pandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.3.0/src/pandora/bots/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,19 +111,15 @@
     def __get_token_key():
         return request.headers.get('X-Use-Token', request.cookies.get('token-key'))
 
     def chat(self, conversation_id=None):
         query = {'chatId': [conversation_id]} if conversation_id else {}
 
         token_key = request.args.get('token')
-        rendered = render_template('chat.html',
-                                   pandora_base=request.url_root.strip('/'),
-                                   pandora_sentry=self.sentry,
-                                   query=query
-                                   )
+        rendered = render_template('chat.html', pandora_base=request.url_root.strip('/'), query=query)
         resp = make_response(rendered)
 
         if token_key:
             self.__set_cookie(resp, token_key, timedelta(days=30))
 
         return resp
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.3.0/src/pandora/cloud_launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import argparse
 
 from loguru import logger
 
 from . import __version__
-from .exts import sentry
 from .exts.hooks import hook_except_handle
 from .openai.utils import Console
 
 __show_verbose = False
 
 
 def main():
@@ -44,43 +43,39 @@
         '--threads',
         help='Define the number of server workers, default: 4',
         required=False,
         type=int,
         default=4,
     )
     parser.add_argument(
-        '--sentry',
-        help='Enable sentry to send error reports when errors occur.',
+        '-l',
+        '--local',
+        help='Login locally. Pay attention to the risk control of the login ip!',
         action='store_true',
     )
     parser.add_argument(
         '-v',
         '--verbose',
         help='Show exception traceback.',
         action='store_true',
     )
     args, _ = parser.parse_known_args()
     __show_verbose = args.verbose
 
-    if args.sentry:
-        sentry.init(args.proxy)
-
     try:
         from pandora_cloud.server import ChatBot as CloudServer
 
-        return CloudServer(args.proxy, args.verbose, args.sentry, True).run(args.server, args.threads)
+        return CloudServer(args.proxy, args.verbose, login_local=args.local).run(args.server, args.threads)
     except (ImportError, ModuleNotFoundError):
         Console.error_bh('### You need `pip install Pandora-ChatGPT[cloud]` to support cloud mode.')
 
 
 def run():
     hook_except_handle()
 
     try:
         main()
     except Exception as e:
         Console.error_bh('### Error occurred: ' + str(e))
 
         if __show_verbose:
             logger.exception('Exception occurred.')
-
-        sentry.capture(e)
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/exts/config.py` & `Pandora-ChatGPT-1.3.0/src/pandora/exts/config.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.3.0/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.3.0/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7361,15 +7361,15 @@
                 clear() {
                     this.queryCache.clear(), this.mutationCache.clear()
                 }
             }
             try {
                 (r = {
                     dsn: "https://9fbadd18a49b4e91921fec0494ce9939@o4504791776755712.ingest.sentry.io/4504797047750656",
-                    enabled: window.__pandora_sentry
+                    enabled: false
                 })._metadata = r._metadata || {}, r._metadata.sdk = r._metadata.sdk || {
                         name: "sentry.javascript.react",
                         packages: [{
                             name: "npm:@sentry/react",
                             version: c
                         }, ],
                         version: c
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.3.0/src/pandora/flask/templates/chat.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/><title>New chat</title><meta name="next-head-count" content="3"/><link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/><link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/><link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png"/><link rel="preload" href="/fonts/Signifier-Regular.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/Sohne-Buch.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/Sohne-Halbfett.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/SohneMono-Buch.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/SohneMono-Halbfett.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/KaTeX_Caligraphic-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Caligraphic-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Fraktur-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Fraktur-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-BoldItalic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Math-BoldItalic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Math-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Script-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size1-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size2-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size3-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size4-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Typewriter-Regular.woff" as="font"/><meta name="description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:title" content="ChatGPT"/><meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:url" content="https://chat.openai.com"/><link rel="preload" href="/_next/static/css/ac221fb2caad35a6.css" as="style"/><link rel="stylesheet" href="/_next/static/css/ac221fb2caad35a6.css" data-n-g=""/><noscript data-n-css=""></noscript><script>window.__pandora_base='{{pandora_base|safe}}';window.__pandora_sentry={{pandora_sentry|lower}};</script><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c9a868e8e0796ec6.js" defer=""></script><script src="/_next/static/chunks/framework-7a789ee31d2a7534.js" defer=""></script><script src="/_next/static/chunks/main-149b337e061b4d04.js" defer=""></script><script src="/_next/static/chunks/pages/_app-aaa11de1926dcafe.js" defer=""></script><script src="/_next/static/chunks/68a27ff6-1185184b61bc22d0.js" defer=""></script><script src="/_next/static/chunks/1f110208-44a6f43ddc5e9011.js" defer=""></script><script src="/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js" defer=""></script><script src="/_next/static/chunks/762-222df1028c0c1555.js" defer=""></script><script src="/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js" defer=""></script><script src="/_next/static/chunks/174-bd28069f281ef76f.js" defer=""></script><script src="/_next/static/chunks/360-442b869f1ba4bb1b.js" defer=""></script><script src="/_next/static/chunks/113-23682f80a24dd00d.js" defer=""></script><script src="/_next/static/chunks/264-13e92c51b0315184.js" defer=""></script><script src="/_next/static/chunks/14-0cb0d20affbd720d.js" defer=""></script><script src="/_next/static/chunks/pages/chat/%5B%5B...chatId%5D%5D-76751174916fa3f7.js" defer=""></script><script src="/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js" defer=""></script><script src="/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js" defer=""></script></head><body><div id="__next"><script>!function(){try{var d=document.documentElement,c=d.classList;c.remove('light','dark');var e=localStorage.getItem('theme');if('system'===e||(!e&&true)){var t='(prefers-color-scheme: dark)',m=window.matchMedia(t);if(m.media!==t||m.matches){d.style.colorScheme = 'dark';c.add('dark')}else{d.style.colorScheme = 'light';c.add('light')}}else if(e){c.add(e|| '')}if(e==='light'||e==='dark')d.style.colorScheme=e}catch(e){}}()</script><div class="overflow-hidden w-full h-full relative"><div class="flex h-full flex-1 flex-col md:pl-[260px]"><main class="relative h-full w-full transition-width flex flex-col overflow-hidden items-stretch flex-1"><div class="flex-1 overflow-hidden"></div><div class="absolute bottom-0 left-0 w-full border-t md:border-t-0 dark:border-white/20 md:border-transparent md:dark:border-transparent md:bg-vert-light-gradient bg-white dark:bg-gray-800 md:!bg-transparent dark:md:bg-vert-dark-gradient pt-2"><form class="stretch mx-2 flex flex-row gap-3 last:mb-2 md:mx-4 md:last:mb-6 lg:mx-auto lg:max-w-3xl"><div class="relative flex h-full flex-1 md:flex-col"><div class="flex ml-1 md:w-full md:m-auto md:mb-2 gap-0 md:gap-2 justify-center"></div><div class="flex flex-col w-full py-2 flex-grow md:py-3 md:pl-4 relative border border-black/10 bg-white dark:border-gray-900/50 dark:text-white dark:bg-gray-700 rounded-md shadow-[0_0_10px_rgba(0,0,0,0.10)] dark:shadow-[0_0_15px_rgba(0,0,0,0.10)]"><textarea tabindex="0" data-id="root" style="max-height:200px" rows="1" class="m-0 w-full resize-none border-0 bg-transparent p-0 pr-7 focus:ring-0 focus-visible:ring-0 dark:bg-transparent pl-2 md:pl-0"></textarea><button class="absolute p-1 rounded-md text-gray-500 bottom-1.5 md:bottom-2.5 hover:bg-gray-100 dark:hover:text-gray-400 dark:hover:bg-gray-900 disabled:hover:bg-transparent dark:disabled:hover:bg-transparent right-1 md:right-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4 mr-1" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><line x1="22" y1="2" x2="11" y2="13"></line><polygon points="22 2 15 22 11 13 2 9 22 2"></polygon></svg></button></div></div></form></div></main></div><div class="dark hidden bg-gray-900 md:fixed md:inset-y-0 md:flex md:w-[260px] md:flex-col"><div class="flex h-full min-h-0 flex-col "><div class="scrollbar-trigger flex h-full w-full flex-1 items-start border-white/20"><nav class="flex h-full flex-1 flex-col space-y-1 p-2"><a class="flex py-3 px-3 items-center gap-3 rounded-md hover:bg-gray-500/10 transition-colors duration-200 text-white cursor-pointer text-sm mb-2 flex-shrink-0 border border-white/20"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><line x1="12" y1="5" x2="12" y2="19"></line><line x1="5" y1="12" x2="19" y2="12"></line></svg>New chat</a><div class="flex-col flex-1 overflow-y-auto border-b border-white/20"><div class="flex flex-col gap-2 text-gray-100 text-sm"><div class="p-3 text-center italic text-gray-500">History is temporarily unavailable.</div></div></div><a href="https://github.com/pengzhile/pandora" target="_blank" class="flex py-3 px-3 items-center gap-3 rounded-md hover:bg-gray-500/10 transition-colors duration-200 text-white cursor-pointer text-sm"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>Pandora on GitHub</a></nav></div></div></div></div><div class="absolute top-0 left-0 right-0 z-[2]"></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"user":{"id":"user-000000000000000000000000","name":"admin@openai.com","email":"admin@openai.com","image":null,"picture":null,"groups":[]},"serviceStatus":{},"userCountry":"US","geoOk":true,"serviceAnnouncement":{"paid":{},"public":{}},"isUserInCanPayGroup":true},"__N_SSP":true},"page":"/chat/[[...chatId]]","query":{{query|tojson|safe}},"buildId":"olf4sv64FWIcQ_zCGl90t","isFallback":false,"gssp":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/><title>New chat</title><meta name="next-head-count" content="3"/><link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/><link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/><link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png"/><link rel="preload" href="/fonts/Signifier-Regular.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/Sohne-Buch.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/Sohne-Halbfett.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/SohneMono-Buch.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/SohneMono-Halbfett.otf" as="font" crossorigin=""/><link rel="preload" href="/fonts/KaTeX_Caligraphic-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Caligraphic-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Fraktur-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Fraktur-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-BoldItalic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Main-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Math-BoldItalic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Math-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Bold.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Italic.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_SansSerif-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Script-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size1-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size2-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size3-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Size4-Regular.woff" as="font"/><link rel="preload" href="/fonts/KaTeX_Typewriter-Regular.woff" as="font"/><meta name="description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:title" content="ChatGPT"/><meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:url" content="https://chat.openai.com"/><link rel="preload" href="/_next/static/css/ac221fb2caad35a6.css" as="style"/><link rel="stylesheet" href="/_next/static/css/ac221fb2caad35a6.css" data-n-g=""/><noscript data-n-css=""></noscript><script>window.__pandora_base='{{pandora_base|safe}}';</script><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c9a868e8e0796ec6.js" defer=""></script><script src="/_next/static/chunks/framework-7a789ee31d2a7534.js" defer=""></script><script src="/_next/static/chunks/main-149b337e061b4d04.js" defer=""></script><script src="/_next/static/chunks/pages/_app-aaa11de1926dcafe.js" defer=""></script><script src="/_next/static/chunks/68a27ff6-1185184b61bc22d0.js" defer=""></script><script src="/_next/static/chunks/1f110208-44a6f43ddc5e9011.js" defer=""></script><script src="/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js" defer=""></script><script src="/_next/static/chunks/762-222df1028c0c1555.js" defer=""></script><script src="/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js" defer=""></script><script src="/_next/static/chunks/174-bd28069f281ef76f.js" defer=""></script><script src="/_next/static/chunks/360-442b869f1ba4bb1b.js" defer=""></script><script src="/_next/static/chunks/113-23682f80a24dd00d.js" defer=""></script><script src="/_next/static/chunks/264-13e92c51b0315184.js" defer=""></script><script src="/_next/static/chunks/14-0cb0d20affbd720d.js" defer=""></script><script src="/_next/static/chunks/pages/chat/%5B%5B...chatId%5D%5D-76751174916fa3f7.js" defer=""></script><script src="/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js" defer=""></script><script src="/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js" defer=""></script></head><body><div id="__next"><script>!function(){try{var d=document.documentElement,c=d.classList;c.remove('light','dark');var e=localStorage.getItem('theme');if('system'===e||(!e&&true)){var t='(prefers-color-scheme: dark)',m=window.matchMedia(t);if(m.media!==t||m.matches){d.style.colorScheme = 'dark';c.add('dark')}else{d.style.colorScheme = 'light';c.add('light')}}else if(e){c.add(e|| '')}if(e==='light'||e==='dark')d.style.colorScheme=e}catch(e){}}()</script><div class="overflow-hidden w-full h-full relative"><div class="flex h-full flex-1 flex-col md:pl-[260px]"><main class="relative h-full w-full transition-width flex flex-col overflow-hidden items-stretch flex-1"><div class="flex-1 overflow-hidden"></div><div class="absolute bottom-0 left-0 w-full border-t md:border-t-0 dark:border-white/20 md:border-transparent md:dark:border-transparent md:bg-vert-light-gradient bg-white dark:bg-gray-800 md:!bg-transparent dark:md:bg-vert-dark-gradient pt-2"><form class="stretch mx-2 flex flex-row gap-3 last:mb-2 md:mx-4 md:last:mb-6 lg:mx-auto lg:max-w-3xl"><div class="relative flex h-full flex-1 md:flex-col"><div class="flex ml-1 md:w-full md:m-auto md:mb-2 gap-0 md:gap-2 justify-center"></div><div class="flex flex-col w-full py-2 flex-grow md:py-3 md:pl-4 relative border border-black/10 bg-white dark:border-gray-900/50 dark:text-white dark:bg-gray-700 rounded-md shadow-[0_0_10px_rgba(0,0,0,0.10)] dark:shadow-[0_0_15px_rgba(0,0,0,0.10)]"><textarea tabindex="0" data-id="root" style="max-height:200px" rows="1" class="m-0 w-full resize-none border-0 bg-transparent p-0 pr-7 focus:ring-0 focus-visible:ring-0 dark:bg-transparent pl-2 md:pl-0"></textarea><button class="absolute p-1 rounded-md text-gray-500 bottom-1.5 md:bottom-2.5 hover:bg-gray-100 dark:hover:text-gray-400 dark:hover:bg-gray-900 disabled:hover:bg-transparent dark:disabled:hover:bg-transparent right-1 md:right-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4 mr-1" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><line x1="22" y1="2" x2="11" y2="13"></line><polygon points="22 2 15 22 11 13 2 9 22 2"></polygon></svg></button></div></div></form></div></main></div><div class="dark hidden bg-gray-900 md:fixed md:inset-y-0 md:flex md:w-[260px] md:flex-col"><div class="flex h-full min-h-0 flex-col "><div class="scrollbar-trigger flex h-full w-full flex-1 items-start border-white/20"><nav class="flex h-full flex-1 flex-col space-y-1 p-2"><a class="flex py-3 px-3 items-center gap-3 rounded-md hover:bg-gray-500/10 transition-colors duration-200 text-white cursor-pointer text-sm mb-2 flex-shrink-0 border border-white/20"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><line x1="12" y1="5" x2="12" y2="19"></line><line x1="5" y1="12" x2="19" y2="12"></line></svg>New chat</a><div class="flex-col flex-1 overflow-y-auto border-b border-white/20"><div class="flex flex-col gap-2 text-gray-100 text-sm"><div class="p-3 text-center italic text-gray-500">History is temporarily unavailable.</div></div></div><a href="https://github.com/pengzhile/pandora" target="_blank" class="flex py-3 px-3 items-center gap-3 rounded-md hover:bg-gray-500/10 transition-colors duration-200 text-white cursor-pointer text-sm"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>Pandora on GitHub</a></nav></div></div></div></div><div class="absolute top-0 left-0 right-0 z-[2]"></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"user":{"id":"user-000000000000000000000000","name":"admin@openai.com","email":"admin@openai.com","image":null,"picture":null,"groups":[]},"serviceStatus":{},"userCountry":"US","geoOk":true,"serviceAnnouncement":{"paid":{},"public":{}},"isUserInCanPayGroup":true},"__N_SSP":true},"page":"/chat/[[...chatId]]","query":{{query|tojson|safe}},"buildId":"olf4sv64FWIcQ_zCGl90t","isFallback":false,"gssp":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/launcher.py` & `Pandora-ChatGPT-1.3.0/src/pandora/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from loguru import logger
 from rich.prompt import Prompt, Confirm
 
 from . import __version__
 from .bots.legacy import ChatBot as ChatBotLegacy
 from .bots.server import ChatBot as ChatBotServer
-from .exts import sentry
 from .exts.config import USER_CONFIG_DIR, default_api_prefix
 from .exts.hooks import hook_except_handle
 from .exts.token import check_access_token_out
 from .openai.api import ChatGPT
 from .openai.auth import Auth0
 from .openai.utils import Console
 
@@ -163,33 +162,31 @@
     parser.add_argument(
         '-a',
         '--api',
         help='Use gpt-3.5-turbo chat api. Note: OpenAI will bill you.',
         action='store_true',
     )
     parser.add_argument(
-        '--sentry',
-        help='Enable sentry to send error reports when errors occur.',
+        '-l',
+        '--local',
+        help='Login locally. Pay attention to the risk control of the login ip!',
         action='store_true',
     )
     parser.add_argument(
         '-v',
         '--verbose',
         help='Show exception traceback.',
         action='store_true',
     )
     args, _ = parser.parse_known_args()
     __show_verbose = args.verbose
 
     Console.debug_b(''', Mode: {}, Engine: {}
         '''.format('server' if args.server else 'cli', 'turbo' if args.api else 'free'))
 
-    if args.sentry:
-        sentry.init(args.proxy)
-
     if args.api:
         try:
             from .openai.token import gpt_num_tokens
             from .migrations.migrate import do_migrate
 
             do_migrate()
         except (ImportError, ModuleNotFoundError):
@@ -198,19 +195,22 @@
 
     access_tokens = parse_access_tokens(args.tokens_file, args.api) if args.tokens_file else None
 
     if not access_tokens:
         access_token, need_save = confirm_access_token(args.token_file, args.server, args.api)
         if not access_token:
             Console.info_b('Please enter your email and password to log in ChatGPT!')
+            if not args.local:
+                Console.warn('We login via {}'.format(api_prefix))
+
             email = getenv('OPENAI_EMAIL') or Prompt.ask('  Email')
             password = getenv('OPENAI_PASSWORD') or Prompt.ask('  Password', password=True)
             mfa = getenv('OPENAI_MFA_CODE') or Prompt.ask('  MFA Code(Optional if not set)')
             Console.warn('### Do login, please wait...')
-            access_token = Auth0(email, password, args.proxy, mfa=mfa).auth(True)
+            access_token = Auth0(email, password, args.proxy, mfa=mfa).auth(args.local)
 
         if not check_access_token_out(access_token, args.api):
             return
 
         if need_save:
             if args.server or Confirm.ask('Do you want to save your access token for the next login?', default=True):
                 save_access_token(access_token)
@@ -221,24 +221,22 @@
         from .turbo.chat import TurboGPT
 
         chatgpt = TurboGPT(access_tokens, args.proxy)
     else:
         chatgpt = ChatGPT(access_tokens, args.proxy)
 
     if args.server:
-        return ChatBotServer(chatgpt, args.verbose, args.sentry).run(args.server, args.threads)
+        return ChatBotServer(chatgpt, args.verbose).run(args.server, args.threads)
 
     ChatBotLegacy(chatgpt).run()
 
 
 def run():
     hook_except_handle()
 
     try:
         main()
     except Exception as e:
         Console.error_bh('### Error occurred: ' + str(e))
 
         if __show_verbose:
             logger.exception('Exception occurred.')
-
-        sentry.capture(e)
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.3.0/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.3.0/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.3.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.3.0/src/pandora/openai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             yield await self.__process_sse_except(resp)
             return
 
         async for utf8_line in resp.aiter_lines():
             if 'data: [DONE]' == utf8_line[0:12]:
                 break
 
-            if 'data: {"message":' == utf8_line[0:17]:
+            if 'data: {"message":' == utf8_line[0:17] or 'data: {"id":' == utf8_line[0:12]:
                 yield json.loads(utf8_line[6:])
 
     @staticmethod
     async def __process_sse_except(resp):
         result = b''
         async for line in resp.aiter_bytes():
             result += line
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.3.0/src/pandora/openai/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,22 +34,22 @@
                           'Chrome/109.0.0.0 Safari/537.36'
 
     @staticmethod
     def __check_email(email: str):
         regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
         return re.fullmatch(regex, email)
 
-    def auth(self, login_local=True) -> str:
+    def auth(self, login_local=False) -> str:
         if self.use_cache and self.access_token and self.expires and self.expires > dt.now():
             return self.access_token
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception('invalid email or password.')
 
-        return self.__part_one()
+        return self.__part_one() if login_local else self.get_access_token_proxy()
 
     def get_refresh_token(self):
         return self.refresh_token
 
     def __part_one(self) -> str:
         url = '{}/auth/preauth'.format(default_api_prefix())
         resp = self.session.get(url, allow_redirects=False, **self.req_kwargs)
@@ -185,14 +185,29 @@
             return self.__part_six(code_verifier, location, url)
 
         if resp.status_code == 400:
             raise Exception('Wrong MFA code.')
         else:
             raise Exception('Error login.')
 
+    def __parse_access_token(self, resp):
+        if resp.status_code == 200:
+            json = resp.json()
+            if 'access_token' not in json:
+                raise Exception('Get access token failed, maybe you need a proxy.')
+
+            if 'refresh_token' in json:
+                self.refresh_token = json['refresh_token']
+
+            self.access_token = json['access_token']
+            self.expires = dt.utcnow() + datetime.timedelta(seconds=json['expires_in']) - datetime.timedelta(minutes=5)
+            return self.access_token
+        else:
+            raise Exception(resp.text)
+
     def get_access_token(self, code_verifier: str, callback_url: str) -> str:
         url_params = parse_qs(urlparse(callback_url).query)
 
         if 'error' in url_params:
             error = url_params['error'][0]
             error_description = url_params['error_description'][0] if 'error_description' in url_params else ''
             raise Exception('{}: {}'.format(error, error_description))
@@ -209,20 +224,22 @@
             'grant_type': 'authorization_code',
             'client_id': 'pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh',
             'code': url_params['code'][0],
             'code_verifier': code_verifier,
         }
         resp = self.session.post(url, headers=headers, json=data, allow_redirects=False, **self.req_kwargs)
 
-        if resp.status_code == 200:
-            json = resp.json()
-            if 'access_token' not in json:
-                raise Exception('Get access token failed, maybe you need a proxy.')
+        return self.__parse_access_token(resp)
 
-            if 'refresh_token' in json:
-                self.refresh_token = json['refresh_token']
+    def get_access_token_proxy(self) -> str:
+        url = '{}/auth/login'.format(default_api_prefix())
+        headers = {
+            'User-Agent': self.user_agent,
+        }
+        data = {
+            'username': self.email,
+            'password': self.password,
+            'mfa_code': self.mfa,
+        }
+        resp = self.session.post(url=url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs)
 
-            self.access_token = json['access_token']
-            self.expires = dt.utcnow() + datetime.timedelta(seconds=json['expires_in']) - datetime.timedelta(minutes=5)
-            return self.access_token
-        else:
-            raise Exception(resp.text)
+        return self.__parse_access_token(resp)
```

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.3.0/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.3.0/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.9/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.3.0/src/pandora/turbo/chat.py`

 * *Files identical despite different names*

