# Comparing `tmp/home-assistant-intents-2023.6.5.tar.gz` & `tmp/home-assistant-intents-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.6.5.tar", last modified: Mon Jun  5 15:46:39 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.7.24.tar", last modified: Mon Jul 24 20:16:32 2023, max compression
```

## Comparing `home-assistant-intents-2023.6.5.tar` & `home-assistant-intents-2023.7.24.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.6.5/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.6.5/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1286 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2023.6.5/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.6.5/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.329424 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35995 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56864 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3160 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2248 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1600 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1286 2023-06-05 15:46:38.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5253 2023-06-05 15:46:39.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-06-05 15:46:38.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-06-05 15:46:39.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1035 2023-06-05 15:45:56.000000 home-assistant-intents-2023.6.5/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.7.24/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.7.24/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2023.7.24/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.7.24/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.239743 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54168 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36159 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    57384 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      975 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/et.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6147 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/eu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17116 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15293 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    59543 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    60255 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    75862 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1760 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2318 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/eu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3252 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3222 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1914 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1642 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-24 20:16:31.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5395 2023-07-24 20:16:32.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 20:16:31.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-24 20:16:32.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1036 2023-07-24 20:14:44.000000 home-assistant-intents-2023.7.24/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/setup.cfg
```

### Comparing `home-assistant-intents-2023.6.5/LICENSE.md` & `home-assistant-intents-2023.7.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/PKG-INFO` & `home-assistant-intents-2023.7.24/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.6.5
+Version: 2023.7.24
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.6.5/README.md` & `home-assistant-intents-2023.7.24/README.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.7.24/home_assistant_intents/__init__.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bg.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999951774691358%*

 * *Differences: {"'lists'": "{'on_off_domains': {'values': {0: {'in': "*

 * *            "'светлин(а|и|ата|ите)|ламп(а|и|ата|ите)|крушк(а|и|ата|ите)|осветлен(ия|ие|ието|ията)'}}}}"}*

```diff
@@ -1315,15 +1315,15 @@
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "\u0441\u0432\u0442\u043b\u0438\u043d(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043b\u0430\u043c\u043f(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043a\u0440\u0443\u0448\u043a(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043e\u0441\u0432\u0435\u0442\u043b\u0435\u043d(\u0438\u044f|\u0438\u0435|\u0438\u0435\u0442\u043e|\u0438\u044f\u0442\u0430)",
+                    "in": "\u0441\u0432\u0435\u0442\u043b\u0438\u043d(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043b\u0430\u043c\u043f(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043a\u0440\u0443\u0448\u043a(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043e\u0441\u0432\u0435\u0442\u043b\u0435\u043d(\u0438\u044f|\u0438\u0435|\u0438\u0435\u0442\u043e|\u0438\u044f\u0442\u0430)",
                     "out": "light"
                 },
                 {
                     "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440[\u0438|\u0430|\u044a\u0442|\u0438\u0442\u0435]",
                     "out": "fan"
                 },
                 {
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9794848039528891%*

 * *Differences: {"'expansion_rules'": "{'name': '<artikel> {name}', 'area': '((in|an|auf) <artikel>|im|am) "*

 * *                      "{area}', 'alle': '((alle|sämtliche)[r]|jede[r|s|n]|<artikel> "*

 * *                      "(ganze|komplette|sämtliche)[n]) [der]', 'abdeckung': '<artikel> "*

 * *                      "(Rollo[s]|Abdeckung[en]|Rolll(a|ä)den|Jalousie[n]|Raffstore[s]|Markise[n])', "*

 * *                      "'garage': '<artikel> (Garage[n]|Garagentor[e])', 'alle_garagen': '<alle> "*

 * *                      "(Garagen[tore])', 'to […]*

```diff
@@ -1,51 +1,54 @@
 {
     "expansion_rules": {
-        "abdeckung": "(das Rollo|die Rollos|die (Abdeckung|Abdeckungen)|(den|die) Rolll(a|\u00e4)den|die (Jalousie|Jalousien)|(den|die) Raffstore[s]|die (Markise|Markisen))",
+        "abdeckung": "<artikel> (Rollo[s]|Abdeckung[en]|Rolll(a|\u00e4)den|Jalousie[n]|Raffstore[s]|Markise[n])",
         "absperren": "(zu|ab)<sperren>|verrieg(el|le)[n]",
         "aktivieren": "aktivier[e|en]",
-        "alle": "((alle|s\u00e4mtliche)[r]|jede[r|s|n]|[die|der] (ganze|komplette|s\u00e4mtliche)[n]) [der]",
+        "alle": "((alle|s\u00e4mtliche)[r]|jede[r|s|n]|<artikel> (ganze|komplette|s\u00e4mtliche)[n]) [der]",
         "alle_abdeckungen": "<alle> (Rollos|Abdeckungen|Rolll(a|\u00e4)den|Jalousien|Raffstores|Markisen)",
-        "alle_garagen": "<alle> (Garagen|Garagentore)",
+        "alle_garagen": "<alle> (Garagen[tore])",
         "alle_lichter": "(<alle> (<lichter>|Beleuchtung)|von allen [Lichtern|Lampen|Leuchten|Beleuchtungen])",
         "alle_luefter": "<alle> (Ventilatoren|L\u00fcfter)",
         "alle_tore": "<alle> (Tore|Garagentore)",
         "an": "(an|ein|auf)",
-        "area": "((in|an|auf) (der|dem)|im|am) {area}",
+        "area": "((in|an|auf) <artikel>|im|am) {area}",
+        "artikel": "[<artikel_bestimmt>|<artikel_unbestimmt>]",
+        "artikel_bestimmt": "[(der|die|das|dem|der|den|des)]",
+        "artikel_unbestimmt": "[(ein|eine|eines|einer|einem|einen)]",
         "auf": "(auf|hoch|rauf|nach oben)",
         "aus": "(aus|ab|zu)",
         "ausfuehren": "(start[e|en]|ausf\u00fchren)",
-        "batterie": "[die|der|des] (Batterie[n]|Akku[s])",
+        "batterie": "<artikel> (Batterie[n]|Akku[s])",
         "brightness": "{brightness} [Prozent|%]",
         "co": "Kohlen[stoff]monoxid",
         "co-sensor": "<co>[-]Sensor[en]",
         "deaktivieren": "de<aktivieren>",
         "ding": "((Ding|Ger\u00e4t)[e]|Sensor[en]|Gegenstand|Gegenst\u00e4nde)",
         "entsperren": "((ent|auf)<sperren>|\u00f6ffne|entrieg(el|le))[n]",
         "etwas": "[irgend][et]was",
-        "garage": "(die Garage|die Garagen|das Garagentor|die Garagentore)",
-        "irgend": "(irgend(ein[e][s|r]|welche[s])|einige[s]) [der]",
-        "ladestand": "[der] [Lade][zu]Stand",
-        "licht": "([das] Licht|[die] Lampe|[die] Beleuchtung)",
+        "garage": "<artikel> (Garage[n]|Garagentor[e])",
+        "irgend": "(irgend(<artikel_unbestimmt>[s]|welche[s])|(einige|manche)[s]|<artikel_unbestimmt>[s]) <artikel_bestimmt>",
+        "ladestand": "<artikel> [Lade][zu]Stand",
+        "licht": "<artikel> (Licht|Lampe|Beleuchtung)",
         "lichter": "[die|der|von den] (Lichter|Lichtern|Lampen|Leuchten|Beleuchtungen)",
-        "luefter": "([den] Ventilator|[die] Ventilatoren|[den|die] L\u00fcfter)",
+        "luefter": "<artikel> (Ventilator[en]|L\u00fcfter)",
         "machen": "(mach[e|en])",
-        "name": "[(der|den|dem|die|das)] {name}",
+        "name": "<artikel> {name}",
         "schalten": "(schalt[e|en])",
         "schliessen": "(schlie(\u00df|ss)[e|en]|zumachen|zu machen)",
-        "schloss": "[das|die] (Schloss|Schl\u00f6sser)",
+        "schloss": "<artikel> (Schloss|Schl\u00f6sser)",
         "setzen": "(setz[e|en]|stell[e|en]|einstellen|\u00e4nder[e|n]|ver\u00e4nder[e|n])",
-        "skript": "[das] Skript",
+        "skript": "<artikel> Skript",
         "sperren": "(sperr|schlie(ss|\u00df))[e|en]",
-        "szene": "[die] Szene",
+        "szene": "<artikel> Szene",
         "temperature": "{temperature} [Grad] [{temperature_unit}]",
-        "tor": "(das Tor|die Tore)",
-        "tuer": "[die] T\u00fcr[e|en]",
+        "tor": "<artikel> Tor[e]",
+        "tuer": "<artikel> T\u00fcr[e|en]",
         "von_dem": "(von [dem]|vom)",
-        "welche": "(welche[r|s]|was f\u00fcr [ein[e][r|s]]) [der]",
+        "welche": "(welche[r|s]|was f\u00fcr [<artikel_unbestimmt>[s]]) <artikel_bestimmt>",
         "zu": "(zu|[he]runter|nach unten)",
         "\u00f6ffnen": "(\u00f6ffne[n]|aufmachen|auf machen)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
@@ -62,15 +65,15 @@
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "irgendeins",
                     "sentences": [
-                        "(ist|sind) <irgend> <batterie> [<area>] {bs_battery_states:state}"
+                        "(ist|sind) [<irgend>] <batterie> [<area>] {bs_battery_states:state}"
                     ],
                     "slots": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -117,16 +120,16 @@
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "irgendeins",
                     "sentences": [
-                        "(wird|werden) <irgend> <batterie> [<area>] {bs_battery_charging_states:state}",
-                        "{bs_battery_charging_states:state} <irgend> <batterie> [<area>] [auf]"
+                        "(wird|werden) [<irgend>] <batterie> [<area>] {bs_battery_charging_states:state}",
+                        "{bs_battery_charging_states:state} [<irgend>] <batterie> [<area>] [auf]"
                     ],
                     "slots": {
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -173,15 +176,15 @@
                         "device_class": "carbon_monoxide",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "irgendeins",
                     "sentences": [
-                        "(ist|sind|wurde[n]) <irgend> <co-sensor> [<area>] {bs_carbon_monoxide_states:state}"
+                        "(ist|sind|wurde[n]) [<irgend>] <co-sensor> [<area>] {bs_carbon_monoxide_states:state}"
                     ],
                     "slots": {
                         "device_class": "carbon_monoxide",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -302,15 +305,15 @@
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "einzeln",
                     "sentences": [
-                        "(wie|was) ist [der Zustand (<von_dem>|der|des)] <name> [<area>]"
+                        "(wie|was) ist [<artikel> Zustand (<von_dem>|<artikel>)] <name> [<area>]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/en.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984217171717171%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {2: {'sentences': ['<turn> off <name>', '[<turn>] <name> "*

 * *              "[to] off', 'deactivate <name>']}, insert: [(3, OrderedDict([('sentences', ['<turn> "*

 * *              "off <name> (light[s]|[light] switch[es])', '[<turn>] <name> (light[s]|[light] "*

 * *              "switch[es]) [to] off', 'deactivate <name> (light[s]|[light] switch[es])']), "*

 * *              "('requires_context', OrderedDict([('domain', 'light')]))]))]}}, 'HassTurnOn': "*

 * *              "{'data': {10: { […]*

```diff
@@ -1416,17 +1416,27 @@
                             "lock",
                             "scene",
                             "script",
                             "sensor"
                         ]
                     },
                     "sentences": [
-                        "<turn> off <name> [light[s]|switch[es]]",
-                        "[<turn>] <name> [light[s]|switch[es]] [to] off",
-                        "deactivate <name> [light[s]|switch[es]]"
+                        "<turn> off <name>",
+                        "[<turn>] <name> [to] off",
+                        "deactivate <name>"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "sentences": [
+                        "<turn> off <name> (light[s]|[light] switch[es])",
+                        "[<turn>] <name> (light[s]|[light] switch[es]) [to] off",
+                        "deactivate <name> (light[s]|[light] switch[es])"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
                         "<turn> off [all] <light> in <area>",
                         "<turn> off [all] <area> <light>",
@@ -1513,14 +1523,24 @@
                         "[activate|<turn>] <name> [scene] [on]"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "sentences": [
+                        "<turn> on <name> (light[s]|[light] switch[es])",
+                        "[<turn>] <name> (light[s]|[light] switch[es]) [to] on",
+                        "activate <name> (light[s]|[light] switch[es])"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn> on [all] <light> in <area>",
                         "<turn> on [all] <area> <light>",
                         "[<turn>] [all] <area> <light> on",
                         "[<turn>] [all] <light> [in] <area> on",
                         "activate [all] <light> [in] <area>",
@@ -1613,17 +1633,17 @@
                             "lock",
                             "scene",
                             "script",
                             "sensor"
                         ]
                     },
                     "sentences": [
-                        "<turn> on <name> [light[s]|switch[es]]",
-                        "[<turn>] <name> [light[s]|switch[es]] [to] on",
-                        "activate <name> [light[s]|switch[es]]"
+                        "<turn> on <name>",
+                        "[<turn>] <name> [to] on",
+                        "activate <name>"
                     ]
                 }
             ]
         }
     },
     "language": "en",
     "lists": {
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/tr.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6629546957671958%*

 * *Differences: {"'expansion_rules'": "{'area': '{area}<ismin_halleri>', 'name': "*

 * *                      "'{name}<cogulluk><ismin_halleri>', 'ismin_halleri': "*

 * *                      "'[([(n|ın|in|un|ün|y|t|d|nd|nt)]ı|[(n|ın|in|un|ün|y|t|d|nd|nt)]i|[(n|ın|in|un|ün|y|t|d|nd|nt)]ü|[(n|ın|in|un|ün|y|t|d|nd|nt)]u|[(n|ın|in|un|ün|y|t|d|nd|nt)]e|[(n|ın|in|un|ün|y|t|d|nd|nt)]a)][n][ki]', "*

 * *                      "'cogulluk': '[(ler|leri|lar|ları)]', 'temperature': '{temperature} "*

 * *                      "[{temperature_unit}]', delet […]*

```diff
@@ -1,143 +1,228 @@
 {
     "expansion_rules": {
-        "all": "(\u00f6ll|\u00f6llum|\u00f6llu|allt)",
-        "area": "{area}[(inu|nu|i\u00f0|\u00f0|inni|nni|nu|num)]",
-        "light": "(lj\u00f3sinu|lj\u00f3sunum|lj\u00f3sin|lj\u00f3s)",
-        "name": "{name}[(inu|nu|i\u00f0|\u00f0|inni|nni|nu|num)]",
-        "turn-off": "(sl\u00f6kkva|sl\u00f6kktu[ \u00e1]|sl\u00f6kkt \u00fe\u00fa \u00e1|sl\u00f6kkt \u00e1|sl\u00f6kkva [\u00e1])",
-        "turn-on": "(kveikja|kveiktu[ \u00e1]|kveikt \u00fe\u00fa \u00e1|kveikt \u00e1|kveikja [\u00e1])"
+        "area": "{area}<ismin_halleri>",
+        "cogulluk": "[(ler|leri|lar|lar\u0131)]",
+        "ismin_halleri": "[([(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u0131|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]i|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u00fc|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]u|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]e|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]a)][n][ki]",
+        "name": "{name}<cogulluk><ismin_halleri>",
+        "temperature": "{temperature} [{temperature_unit}]"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "lights_area",
                     "sentences": [
-                        "<turn-off> <light> \u00ed <area>",
-                        "<turn-off> <all> [<light>] \u00ed <area>",
-                        "<turn-off> <area><light>"
+                        "<name> (kapa | kapat | s\u00f6nd\u00fcr )"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<name> (kapa | kapat | indir ) "
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<area> <name> (kapa | kapat | indir )"
+                    ]
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "garaj kap\u0131s\u0131n\u0131 (kapa | kapat | indir )"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "lights_name",
+                    "response": "cover_area",
                     "sentences": [
-                        "<turn-off> <name> [\u00ed <area>]"
+                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (kapa | kapat | indir | \u00e7ek)"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "response": "lights_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<turn-on> <light> \u00ed <area>",
-                        "<turn-on> <all> [<light>] \u00ed <area>",
-                        "<turn-on> <area>[ ]<light>"
+                        "garaj kap\u0131s\u0131n\u0131 (a\u00e7 | y\u00fckselt)"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "lights_name",
+                    "response": "cover_area",
                     "sentences": [
-                        "<turn-on> <name> [\u00ed <area>]"
+                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (a\u00e7 | y\u00fckselt)"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<name> ( a\u00e7 | yak | \u00e7al\u0131\u015ft\u0131r)"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<name> (a\u00e7 | y\u00fckselt) "
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<area> <name> (a\u00e7 | y\u00fckselt)"
+                    ]
                 }
             ]
         }
     },
-    "language": "is",
+    "language": "tr",
     "lists": {
+        "brightness": {
+            "range": {
+                "from": 0,
+                "to": 100,
+                "type": "percentage"
+            }
+        },
         "color": {
             "values": [
                 {
-                    "in": "hv\u00edt(t|ur|an|a|um|ri|u|s|rar)",
+                    "in": "beyaz",
                     "out": "white"
                 },
                 {
-                    "in": "(svart|svartur|sv\u00f6rt)",
+                    "in": "siyah",
                     "out": "black"
                 },
                 {
-                    "in": "(rau\u00f0ur|rautt|rau\u00f0)",
+                    "in": "k\u0131rm\u0131z\u0131",
                     "out": "red"
                 },
                 {
-                    "in": "(appels\u00ednugulur|appels\u00ednugult|apples\u00ednugul)",
+                    "in": "turuncu",
                     "out": "orange"
                 },
                 {
-                    "in": "(gulur|gul|gult)",
+                    "in": "sar\u0131",
                     "out": "yellow"
                 },
                 {
-                    "in": "(gr\u00e6nn|gr\u00e6nt|gr\u00e6n)",
+                    "in": "ye\u015fil",
                     "out": "green"
                 },
                 {
-                    "in": "(bl\u00e1r|bl\u00e1|bl\u00e1tt)",
+                    "in": "mavi",
                     "out": "blue"
                 },
                 {
-                    "in": "(fj\u00f3lubl\u00e1tt|fj\u00f3lubl\u00e1r|j\u00f3lubl\u00e1)",
+                    "in": "mor",
                     "out": "purple"
                 },
                 {
-                    "in": "(br\u00fann|br\u00fan|br\u00fant)",
+                    "in": "kahverengi",
                     "out": "brown"
                 },
                 {
-                    "in": "(bleikur|bleikt|bleik)",
+                    "in": "gri",
+                    "out": "grey"
+                },
+                {
+                    "in": "pembe",
                     "out": "pink"
+                },
+                {
+                    "in": "turkuaz",
+                    "out": "turquoise"
+                },
+                {
+                    "in": "bordo",
+                    "out": "maroon"
+                },
+                {
+                    "in": "bej",
+                    "out": "beige"
+                },
+                {
+                    "in": "lacivert",
+                    "out": "navy"
+                }
+            ]
+        },
+        "temperature": {
+            "range": {
+                "from": 0,
+                "to": 100,
+                "type": "temperature"
+            }
+        },
+        "temperature_unit": {
+            "values": [
+                "celsius",
+                {
+                    "in": "c | santigrat",
+                    "out": "celsius"
+                },
+                "fahrenheit",
+                {
+                    "in": "f | fahrenhayt",
+                    "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Vi\u00f0 me\u00f0h\u00f6ndlun \u00e1setningsins kom \u00f3v\u00e6nt villa upp",
-            "no_area": "Ekkert sv\u00e6\u00f0i {{ area }} fannst",
-            "no_device_class": "{{ area }} er ekki me\u00f0 t\u00e6kja tegund {{ device_class }}",
-            "no_domain": "\u00cd {{ area }} er ekkert {{ domain }}",
-            "no_entity": "Ekkert t\u00e6ki e\u00f0a engin eining me\u00f0 nafni {{ entity }} fannst",
-            "no_intent": "Fyrirgef\u00f0u en \u00e9g n\u00e1\u00f0i \u00feessu ekki"
+            "handle_error": "\u0130stenilen ama\u00e7 i\u015flenirken bir hata olu\u015ftu.",
+            "no_area": "{{ area }}  ad\u0131nda alan yok.",
+            "no_device_class": "{{ area }}  bir {{ device_class }} i\u00e7ermiyor.",
+            "no_domain": "{{ area }}  bir {{ domain }} i\u00e7ermiyor.",
+            "no_entity": "{{ entity }} ad\u0131nda bir cihaz yok.",
+            "no_intent": "\u00dczg\u00fcn\u00fcm, bunu anlayamad\u0131m."
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "Loka\u00f0i {{ slots.name }}",
-                "cover_area": "Loka\u00f0i {{ slots.area }}",
-                "default": "Sl\u00f6kkti \u00e1 {{ slots.domain }}",
-                "fans_area": "Sl\u00f6kkti \u00e1 viftum \u00ed {{ slots.area }}",
-                "lights_area": "Sl\u00f6kkti \u00e1 lj\u00f3sum \u00ed {{ slots.area }}",
-                "lights_name": "Sl\u00f6kkti \u00e1 {{ slots.name }}"
+                "cover": "Closed {{ slots.name }}",
+                "cover_area": "Closed {{ slots.area }}",
+                "cover_device_class": "Closed {{ slots.device_class }}",
+                "default": "Turned off {{ slots.name }}",
+                "fans_area": "Turned off fans in {{ slots.area }}",
+                "lights_area": "Turned off lights in {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "Opna\u00f0i {{ slots.name }}",
-                "cover_area": "Opna\u00f0i {{ slots.area }}",
-                "default": "Kveikti \u00e1 {{ slots.domain }}",
-                "fans_area": "Kveikti \u00e1 viftum \u00ed {{ slots.area }}",
-                "lights_area": "Kveikti \u00e1 lj\u00f3sum \u00ed {{ slots.area }}",
-                "lights_name": "Kveikti \u00e1 {{ slots.name }}"
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}",
+                "cover_device_class": "Opened {{ slots.device_class }}",
+                "default": "Turned on {{ slots.name }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "lights_area": "Turned on lights in {{ slots.area }}"
             }
         }
     },
     "skip_words": [
-        "\u00fe\u00fa",
-        "getur\u00f0u",
-        "getur \u00fe\u00fa",
-        "viltu",
-        "vilt \u00fe\u00fa"
+        "L\u00fctfen"
     ]
 }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/it.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9762306221941639%*

 * *Differences: {"'expansion_rules'": "{'of': '(de[l[lo|la|le]]|i|gli|di)', 'fan': '(ventol(a|e) | ventilator(e|i) "*

 * *                      "| ventilazione )', 'climate': "*

 * *                      "'(clima|climatizzator(e|i)|condizionator(e|i)|aria condizionata)', 'all': "*

 * *                      "'tutt(o|e|i|a)', 'garage': '(serrand(a|e) | port(a|e) "*

 * *                      "[basculant(e|i)|de(l|i) garage] | saracinesc(a|he))'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {3: {'sentences': ['<close> [<the>] {name} [<in> "*

 * *         […]*

```diff
@@ -1,17 +1,20 @@
 {
     "expansion_rules": {
+        "all": "tutt(o|e|i|a)",
         "area": "{area}",
         "brightness": "{brightness}[%| percento]",
+        "climate": "(clima|climatizzator(e|i)|condizionator(e|i)|aria condizionata)",
         "close": "(chiud(i|ere) | abbass(a|are))",
         "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|e))",
-        "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione | climatizzator(e|i) | condizionator(e|i))",
+        "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione )",
+        "garage": "(serrand(a|e) | port(a|e) [basculant(e|i)|de(l|i) garage] | saracinesc(a|he))",
         "in": "(in | ne[i|gli|l[lo|la|le]])",
         "name": "{name}",
-        "of": "(de[i|gli|l[lo|la|le]]|di)",
+        "of": "(de[l[lo|la|le]]|i|gli|di)",
         "open": "(apr(i|ire) | alz(a|are))",
         "set": "(impost(a|are) | cambi(a|are) | mett(i|ere) | modific(a|are))",
         "temp": "[la] (temperatura)",
         "temperature": "{temperature}[\u00b0| gradi] [{temperature_unit}]",
         "the": "(l(o|a|e) | i[l] | gli | l')",
         "to": "a[l[lo|la|le] | gli]",
         "turn_off": "(spegn(i|ere) | disattiv(a|are))",
@@ -142,50 +145,62 @@
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
-                        "<close> [<the>] <name> [[<of>|<in>] <area>]"
+                        "<close> [<the>] {name} [<in> {area}]"
                     ]
                 },
                 {
-                    "requires_context": {
+                    "response": "cover_all",
+                    "sentences": [
+                        "<close> <all> [[<the>] casa]"
+                    ],
+                    "slots": {
                         "domain": "cover"
-                    },
+                    }
+                },
+                {
                     "response": "cover_area",
                     "sentences": [
-                        "<close> [<the>] <cover> [[<in> | <of>] <area>]",
-                        "<close> [[<in>] <area>] [<the>] <cover>"
-                    ]
+                        "<close> <all> [<in>|<the>] {area}"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<close> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
-                        "<close> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
+                        "<close> <all> [<the>] {cover_classes:device_class}"
                     ],
                     "slots": {
-                        "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_device_class_area",
                     "sentences": [
-                        "<close> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
-                        "<close> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
+                        "<close> [<all>] [<the>] {cover_classes:device_class} [<in>|<of>] {area}",
+                        "<close> [<in>] {area} [<all>] [<the>] {cover_classes:device_class}"
+                    ]
+                },
+                {
+                    "response": "cover_garage",
+                    "sentences": [
+                        "<close> <the> <garage> [[(in | del)] garage]",
+                        "<close> [[<in>] garage] <the> <garage>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
+                        "device_class": "garage",
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
@@ -200,50 +215,53 @@
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
-                        "<open> [<the>] <name> [[<of>|<in>] <area>]"
+                        "<open> [<the>] {name} [[<in> | <of>] {area}]"
                     ]
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
                     "response": "cover_area",
                     "sentences": [
-                        "<open> [<the>] <cover> [[<in> | <of>] <area>]",
-                        "<open> [[<in>] <area>] [<the>] <cover>"
-                    ]
+                        "<open> [<all>] [<in> | <the>] {area}"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<open> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
-                        "<open> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
+                        "<open> <all> [<the>] {cover_classes:device_class}"
                     ],
                     "slots": {
-                        "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_device_class_area",
                     "sentences": [
-                        "<open> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
-                        "<open> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
+                        "<open> [<all>][<the>] {cover_classes:device_class} [[<in> | <of>] {area}]",
+                        "<open> [[<in>] {area}] [<all>] [<the>] {cover_classes:device_class}"
+                    ]
+                },
+                {
+                    "response": "cover_garage",
+                    "sentences": [
+                        "<open> <the> <garage> [[(in | del)] garage]",
+                        "<open> [[<in>] garage] <the> <garage>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
+                        "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "sentences": [
                         "<turn_on> [(tutt(i|e))] [<the>]<fan> [(<of> | <in>)] <area>",
                         "<turn_on> [<in>] <area> [(tutt(i|e))] [<the>]<fan>"
@@ -325,15 +343,15 @@
                     "out": "curtain"
                 },
                 {
                     "in": "port(a|e)",
                     "out": "door"
                 },
                 {
-                    "in": "(serrand(a|e) | port(a|e) [basculant(e|i)|de(l|i) garage] | saracinesc(a|he))",
+                    "in": "<garage>",
                     "out": "garage"
                 },
                 {
                     "in": "cancell(o|i)",
                     "out": "gate"
                 },
                 {
@@ -448,26 +466,31 @@
                 "how_many": "{{ query.matched | length }}\n",
                 "one": "{{ slots.name | capitalize }} \u00e8 {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched %}\n  S\u00ec\n{% else %}\n  No, \u00e8 {{ state.state_with_unit }}\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  Nessuno\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length == 4 %}\n    {{ match[:3] | join(\", \") }} ed un altro\n  {% elif match | length > 4 %}\n    {{ match[:3] | join(\", \") }} ed altri {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
                 "cover": "Ho chiuso {{ slots.name }}",
-                "cover_area": "Chiuse in {{ slots.area }}",
-                "cover_device_class": "Ho chiuso {{ slots.device_class }}",
+                "cover_all": "Ho chiuso tutto",
+                "cover_area": "Ho chiuso tutto in {{ slots.area }}",
+                "cover_device_class": "Ho chiuso tutte le {{slots.device_class}}",
+                "cover_device_class_area": "Ho chiuso le {{slots.device_class}} in {{slots.area}}",
+                "cover_garage": "Ho chiuso il garage",
                 "default": "Ho spento {{ slots.name }}",
                 "fans_area": "Ho spento la ventilazione in {{ slots.area }}",
                 "lights_area": "Ho spento le luci in {{ slots.area }}",
                 "scene": "Ho disattivato {{ slots.name }}",
                 "script": "Ho arrestato {{ slots.name }}"
             },
             "HassTurnOn": {
                 "cover": "Ho aperto {{ slots.name }}",
-                "cover_area": "Aperte in {{ slots.area }}",
-                "cover_device_class": "Ho aperto {{ slots.device_class }}",
+                "cover_area": "Ho aperto tutto in {{ slots.area }}",
+                "cover_device_class": "Ho aperto tutte le {{slots.device_class}}",
+                "cover_device_class_area": "Ho aperto le {{slots.device_class}} in {{slots.area}}",
+                "cover_garage": "Ho aperto il garage",
                 "default": "Ho acceso {{ slots.name }}",
                 "fans_area": "Ho acceso la ventilazione in {{ slots.area }}",
                 "lights_area": "Ho acceso le luci in {{ slots.area }}",
                 "scene": "Ho attivato {{ slots.name }}",
                 "script": "Ho avviato {{ slots.name }}"
             }
         }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6150859345474301%*

 * *Differences: {"'expansion_rules'": "{replace: OrderedDict([('name', '{name}[的]'), ('area', '{area}[的]'), "*

 * *                      "('let', '[把|将|让|给]'), ('all', '(全部|所有)[的]'), ('what_is', '是什么'), "*

 * *                      "('how_many_is', '(是多少|有多少|有几个)'), ('which', '[有|有没有|有無]哪[一](个|些)'), "*

 * *                      "('brightness', '[百分之]{brightness}[%]'), ('to', '(为|到|成|至)'), ('set_to', "*

 * *                      "'(设置|设定|调节|调|设)(为|到|至)'), ('turn_on', '(打开|开启|开)'), ('turn_off', "*

 * *                      "'(关闭|关掉|关了|关)'), ('open', […]*

```diff
@@ -1,602 +1,611 @@
 {
     "expansion_rules": {
-        "aktiver": "(aktiver|utf\u00f8r|kj\u00f8r)",
-        "alle": "(alle|alt|samtlige)",
-        "bryter": "(bryter[(e|[e]n[e])]|uttak[ene]|kontakt[(er|en[e])])",
-        "d\u00f8r": "(d\u00f8r[(a|er|en[e])])",
-        "endre": "(endre|sett|juster|skru (opp|ned)|vri|dimm[e]|still [inn]|\u00f8k|senk|dim[me])",
-        "farge": "({color}[t[t]])",
-        "garasje": "(garasje[d\u00f8r|port][e][(n|r|ne)])",
-        "gardin": "(gardin[(et|er|ene)]|forheng[et|er|ene])",
-        "hvilke": "(hvilke[n])",
-        "i_p\u00e5": "(i|p\u00e5|ved [siden av])",
-        "kaldt_varmt": "(kald|kaldt|varm|varmt)",
-        "lukk": "(lukk [igjen]|heis [ned]|rull [ned]|steng|senk)",
-        "lukket": "(lukket [igjen]|stengt|senket|rullet ned)",
-        "lys": "(lys[(ene|et)]|lyskilde[r|n|ene]|[gl\u00f8de|led|diode]lamp[e|en|er|ene]|lysr\u00f8r[et|ene]|belysning[en])",
-        "lysstyrke": "{brightness}[%| prosent]",
-        "markise": "(markise[(r|n[e])])",
-        "navn": "{name}[(en|et|n[s])]",
-        "omr\u00e5de": "{area}[(n[s]|en|et[s]|met[s])]",
-        "persienne": "(persienne[(n|r|ene)])",
-        "port": "([hage]port[(er|en[e])])",
-        "rullegardin": "((rullegardin|foldegardin|plissegardin)[(et|er|ene)])",
-        "skodde": "([rulle]skodde[(n|r|ene)]|solskjerm[(en|er|ene)])",
-        "skru_av": "(skru av|slukk|sl\u00e5 av|slukk|steng [av]|stopp)",
-        "skru_p\u00e5": "(skru p\u00e5|tenn|sett[e] (p\u00e5|igang|fart p\u00e5)|sl\u00e5 p\u00e5|start[e])",
-        "temperatur": "({temperature}[\u00b0| grader] [{temperature_unit}])",
-        "tilstand": "((tilstand|status|instilling)[en] [til])",
-        "vifte": "(vifte[(r|n[e])])",
-        "vindu": "([tak]vindu[et|er|ene]|[tak]luke[en|er|ene])",
-        "\u00e5pen": "(\u00e5pen|\u00e5pnet [opp]|rullet opp|lukket opp)",
-        "\u00e5pne": "(\u00e5pne [opp]|heis [opp]|lukk opp|rull opp)"
+        "all": "(\u5168\u90e8|\u6240\u6709)[\u7684]",
+        "area": "{area}[\u7684]",
+        "brightness": "[\u767e\u5206\u4e4b]{brightness}[%]",
+        "close": "(\u5173\u95ed|\u5173\u6389|\u5173\u4e86|\u5173)",
+        "how_many_is": "(\u662f\u591a\u5c11|\u6709\u591a\u5c11|\u6709\u51e0\u4e2a)",
+        "let": "[\u628a|\u5c06|\u8ba9|\u7ed9]",
+        "light": "(\u706f|\u5438\u9876\u706f|\u7b52\u706f|\u5c04\u706f|\u53f0\u706f|\u5e8a\u5934\u706f|\u706f\u5149)[\u7684]",
+        "name": "{name}[\u7684]",
+        "open": "(\u6253\u5f00|\u5f00)",
+        "set_to": "(\u8bbe\u7f6e|\u8bbe\u5b9a|\u8c03\u8282|\u8c03|\u8bbe)(\u4e3a|\u5230|\u81f3)",
+        "temp": "\u6e29\u5ea6",
+        "temperature": "{temperature}[{temperature_unit}]",
+        "to": "(\u4e3a|\u5230|\u6210|\u81f3)",
+        "turn_off": "(\u5173\u95ed|\u5173\u6389|\u5173\u4e86|\u5173)",
+        "turn_on": "(\u6253\u5f00|\u5f00\u542f|\u5f00)",
+        "what_is": "\u662f\u4ec0\u4e48",
+        "which": "[\u6709|\u6709\u6ca1\u6709|\u6709\u7121]\u54ea[\u4e00](\u4e2a|\u4e9b)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
                     "response": "one",
                     "sentences": [
-                        "hva er [<tilstand>] [til] <navn> [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>]<name>[\u72b6\u6001](<what_is>|<how_many_is>)",
+                        "[<area>]<name>[<what_is>]\u72b6\u6001"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "er [<tilstand>] [til] <navn> {on_off_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>]{name}\u662f\u4e0d\u662f{on_off_states:state}",
+                        "[<area>]{name}[\u662f]{on_off_states:state}[\u5417|\u4e0d]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "er noen [av] {on_off_domains:domain} {on_off_states:state} [<i_p\u00e5> <omr\u00e5de>]",
-                        "er noen [av] {on_off_domains:domain} [<i_p\u00e5> <omr\u00e5de>] {on_off_states:state}"
+                        "[{area}][\u6709|\u6709\u6ca1\u6709]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f]{on_off_states:state}[\u5417|\u4e0d]"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "er alle {on_off_domains:domain} {on_off_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>][<all>]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{on_off_states:state}[\u5417|\u4e0d]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "<hvilke> {on_off_domains:domain} er {on_off_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>]<which>{on_off_domains:domain}[\u662f]{on_off_states:state}",
+                        "<which>[<area>]{on_off_domains:domain}[\u662f]{on_off_states:state}"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "hvor mange {on_off_domains:domain} er {on_off_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[{area}]<how_many_is>{on_off_domains:domain}[\u662f]{on_off_states:state}",
+                        "<how_many_is>[<area>]{on_off_domains:domain}[\u662f]{on_off_states:state}"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "er <navn> {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]",
-                        "er <navn> [<i_p\u00e5> <omr\u00e5de>] {cover_states:state}"
+                        "[<area>]{name}(\u662f|\u662f\u4e0d\u662f){cover_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "er noen {cover_classes:device_class} {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[{area}][\u6709|\u6709\u6ca1\u6709]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]{cover_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "er alle {cover_classes:device_class} {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>][<all>]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{cover_states:state}[\u5417|\u4e0d]",
+                        "<all><area>{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{cover_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "<hvilke> {cover_classes:device_class} er {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>]<which>{cover_classes:device_class}[\u662f]{cover_states:state}",
+                        "<which>[<area>]{cover_classes:device_class}[\u662f]{cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "hvor mange {cover_classes:device_class} er {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[{area}]<how_many_is>{cover_classes:device_class}[\u662f]{cover_states:state}",
+                        "<how_many_is>[<area>]{cover_classes:device_class}[\u662f]{cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "er <navn> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>]{name}(\u662f\u4e0d\u662f|\u6709\u6ca1\u6709){lock_states:state}",
+                        "[<area>]{name}[\u662f|\u6709]{lock_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "er noen <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[{area}][\u6709|\u6709\u6ca1\u6709](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}[\u5417|\u4e0d]",
+                        "{area}(\u95e8|\u9501|\u95e8\u9501)[\u6709|\u6709\u6ca1\u6709]{lock_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "er <alle> <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>][<all>](\u95e8|\u9501|\u95e8\u9501)[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{lock_states:state}[\u5417|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "<hvilke> <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[<area>](<which>|\u54ea[\u4e00]\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "(<which>|\u54ea[\u4e00]\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "<area>(\u95e8|\u9501|\u95e8\u9501)(<which>|\u54ea[\u4e00]\u6247)[\u662f]{lock_states:state}"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "hvor mange <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                        "[{area}](<how_many_is>|\u6709\u51e0\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "(<how_many_is>|\u6709\u51e0\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "{area}(\u95e8|\u9501|\u95e8\u9501)(<how_many_is>|\u6709\u51e0\u6247)[\u662f]{lock_states:state}"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
                     "sentences": [
-                        "<skru_av> [<alle>] <vifte> <i_p\u00e5> <omr\u00e5de>",
-                        "<skru_av> [<alle>] <omr\u00e5de> <vifte>"
+                        "<turn_off><area>(\u98ce\u6247|\u540a\u6247)",
+                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_off>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "sentences": [
-                        "<skru_av> <navn>",
-                        "(skru|sl\u00e5) <navn> av"
-                    ]
-                },
-                {
                     "excludes_context": {
                         "domain": [
+                            "binary_sensor",
                             "cover",
+                            "lock",
                             "scene",
-                            "sensor",
                             "script",
-                            "lock"
+                            "sensor"
                         ]
                     },
                     "sentences": [
-                        "<lukk> <navn>",
-                        "<lukk> <navn> <i_p\u00e5> <omr\u00e5de>"
+                        "<turn_off>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_off>"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "<skru_av> [<alle>] <lys> [<i_p\u00e5>] <omr\u00e5de>",
-                        "<skru_av> [<alle>] <omr\u00e5de>[s][ ]<lys>",
-                        "<skru_av> <omr\u00e5de> [<alle>] <lys>"
-                    ],
-                    "slots": {
-                        "domain": "light",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<skru_av> <lys> <navn>"
+                        "<turn_off><area><light>",
+                        "[<let>]<area><light><turn_off>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
-                    "response": "cover",
                     "sentences": [
-                        "<lukk> <navn> [<i_p\u00e5> <omr\u00e5de>]"
+                        "<close>[<area>]{name}",
+                        "[<let>][<area>]{name}<close>"
                     ]
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<lukk> <garasje>"
+                        "<close>\u8f66\u5e93\u7684[\u5927|\u5377\u95f8]\u95e8",
+                        "[<let>]\u8f66\u5e93\u7684[\u5927|\u5377\u95f8]\u95e8<close>"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<lukk> {cover_classes:device_class} <i_p\u00e5> <omr\u00e5de>",
-                        "<lukk> <omr\u00e5de>[s][ ]{cover_classes:device_class}"
+                        "<close>[<area>]{cover_classes:device_class}",
+                        "[<let>][<area>]{cover_classes:device_class}<close>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "[\u6253|\u89e3]\u5f00[<area>]{name}[[\u7684]\u9501]",
+                        "[<let>][<area>]{name}[[\u7684]\u9501](\u6253\u5f00|\u89e3\u9501)"
+                    ]
+                },
+                {
+                    "response": "lock",
+                    "sentences": [
+                        "[\u6253|\u89e3]\u5f00<area>[<all>][\u95e8]\u9501",
+                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u6253\u5f00|\u89e3\u9501)",
+                        "{area}(\u5f00|\u89e3)\u9501"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "scene"
                     },
                     "response": "scene",
                     "sentences": [
-                        "<aktiver> <navn>[s][modus]"
+                        "[\u6fc0\u6d3b|\u5f00\u542f|\u6253\u5f00|\u5207\u6362[\u5230]]<name>[\u573a\u666f|\u6a21\u5f0f]",
+                        "<name>[\u573a\u666f|\u6a21\u5f0f]\u5f00\u542f"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "<skru_p\u00e5> [<alle>] <lys> [<i_p\u00e5>] <omr\u00e5de>",
-                        "<skru_p\u00e5> [<alle>] <omr\u00e5de>[s][ ]<lys>",
-                        "<skru_p\u00e5> <omr\u00e5de> [<alle>] <lys>"
-                    ],
-                    "slots": {
-                        "domain": "light",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<skru_p\u00e5> <lys> <navn>"
+                        "<turn_on><area><light>",
+                        "[<let>]<area><light><turn_on>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
-                    "response": "cover",
                     "sentences": [
-                        "<\u00e5pne> <navn> [<i_p\u00e5> <omr\u00e5de>]"
+                        "<open>[<area>]{name}",
+                        "[<let>][<area>]{name}<open>"
                     ]
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u00e5pne> <garasje>"
+                        "<open>\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8",
+                        "[<let>]\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8<open>"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<\u00e5pne> {cover_classes:device_class} <i_p\u00e5> <omr\u00e5de>",
-                        "<\u00e5pne> <omr\u00e5de>[s][ ]{cover_classes:device_class}"
+                        "<open>[<area>]{cover_classes:device_class}",
+                        "[<let>][<area>]{cover_classes:device_class}<open>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
+                    "response": "fans_area",
                     "sentences": [
-                        "<skru_p\u00e5> [<alle>] <vifte> <i_p\u00e5> <omr\u00e5de>",
-                        "<skru_p\u00e5> [<alle>] <omr\u00e5de> <vifte>"
+                        "<turn_on><area>(\u98ce\u6247|\u540a\u6247)",
+                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_on>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
-                        "domain": "script"
+                        "domain": "lock"
                     },
-                    "response": "script",
+                    "response": "lock",
+                    "sentences": [
+                        "\u5173(\u95ed|\u4e0a)[<area>]{name}[[\u7684]\u9501]",
+                        "[<let>][<area>]{name}[[\u7684]\u9501](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)"
+                    ]
+                },
+                {
+                    "response": "lock",
                     "sentences": [
-                        "(<aktiver>|<skru_p\u00e5>) <navn> [skript]"
+                        "\u5173(\u95ed|\u4e0a)<area>[<all>][\u95e8]\u9501",
+                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)",
+                        "{area}(\u4e0a|\u5173)\u9501"
                     ],
                     "slots": {
-                        "domain": "script"
+                        "domain": "lock"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
                     "sentences": [
-                        "<skru_p\u00e5> <navn>",
-                        "(skru|sl\u00e5) <navn> p\u00e5"
-                    ]
+                        "[\u8fd0\u884c|\u6267\u884c]<name>[\u811a\u672c]"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
                 },
                 {
                     "excludes_context": {
                         "domain": [
+                            "binary_sensor",
                             "cover",
+                            "lock",
                             "scene",
-                            "sensor",
                             "script",
-                            "lock"
+                            "sensor"
                         ]
                     },
                     "sentences": [
-                        "<\u00e5pne> <navn>",
-                        "<\u00e5pne> <navn> <i_p\u00e5> <omr\u00e5de>"
+                        "<turn_on>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_on>"
                     ]
                 }
             ]
         }
     },
-    "language": "nb",
+    "language": "zh-cn",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "brightness_level": {
             "values": [
                 {
-                    "in": "(maks[imum]|[det] h\u00f8yest[e])",
+                    "in": "\u6700(\u4eae|\u9ad8|\u5927)",
                     "out": 100
                 },
                 {
-                    "in": "(medium|[det] mellom[st[e]])",
-                    "out": 50
-                },
-                {
-                    "in": "(minimum|[det] lavest[e])",
+                    "in": "\u6700(\u6697|\u4f4e|\u5c0f)",
                     "out": 1
                 }
             ]
         },
         "color": {
             "values": [
                 {
-                    "in": "bl\u00e5",
-                    "out": "blue"
+                    "in": "\u767d\u8272",
+                    "out": "white"
                 },
                 {
-                    "in": "brun",
-                    "out": "brown"
+                    "in": "\u9ed1\u8272",
+                    "out": "black"
                 },
                 {
-                    "in": "gr\u00f8nn",
-                    "out": "green"
+                    "in": "\u7ea2\u8272",
+                    "out": "red"
                 },
                 {
-                    "in": "gul",
-                    "out": "yellow"
+                    "in": "\u6a59\u8272",
+                    "out": "orange"
                 },
                 {
-                    "in": "hvit",
-                    "out": "white"
+                    "in": "\u9ec4\u8272",
+                    "out": "yellow"
                 },
                 {
-                    "in": "lilla",
-                    "out": "purple"
+                    "in": "\u7eff\u8272",
+                    "out": "green"
                 },
                 {
-                    "in": "oransje",
-                    "out": "orange"
+                    "in": "\u84dd\u8272",
+                    "out": "blue"
                 },
                 {
-                    "in": "r\u00f8d",
-                    "out": "red"
+                    "in": "\u7d2b\u8272",
+                    "out": "purple"
                 },
                 {
-                    "in": "svart",
-                    "out": "black"
+                    "in": "\u68d5\u8272",
+                    "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "<markise>",
+                    "in": "(\u906e\u9633|\u96e8)(\u84ec|\u68da)",
                     "out": "awning"
                 },
                 {
-                    "in": "<persienne>",
+                    "in": "(\u767e\u53f6\u7a97|\u767e\u53f6\u5e18|\u5377\u5e18)",
                     "out": "blind"
                 },
                 {
-                    "in": "<gardin>",
+                    "in": "\u7a97\u5e18",
                     "out": "curtain"
                 },
                 {
-                    "in": "<d\u00f8r>",
+                    "in": "(\u95e8|\u623f\u95e8|\u5377\u95f8\u95e8)",
                     "out": "door"
                 },
                 {
-                    "in": "<garasje>",
+                    "in": "\u8f66\u5e93\u95e8",
                     "out": "garage"
                 },
                 {
-                    "in": "<port>",
+                    "in": "(\u5927\u95e8|\u9662\u5b50\u95e8|\u94c1\u95e8)",
                     "out": "gate"
                 },
                 {
-                    "in": "<rullegardin>",
+                    "in": "\u906e\u9633\u5e18",
                     "out": "shade"
                 },
                 {
-                    "in": "<skodde>",
+                    "in": "\u767e\u53f6\u7a97\u6237",
                     "out": "shutter"
                 },
                 {
-                    "in": "<vindu>",
+                    "in": "\u7a97\u6237",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "<\u00e5pen>",
+                    "in": "(\u6253\u5f00|\u5f00\u7740|\u5f00\u4e86)[\u7684]",
                     "out": "open"
                 },
                 {
-                    "in": "<lukket>",
+                    "in": "(\u5173\u95ed|\u5173\u7740|\u5173\u4e86)[\u7684]",
                     "out": "closed"
                 },
                 {
-                    "in": "\u00e5pner",
+                    "in": "\u6253\u5f00\u4e2d",
                     "out": "opening"
                 },
                 {
-                    "in": "lukker",
+                    "in": "\u5173\u95ed\u4e2d",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "l\u00e5st",
+                    "in": "(\u5df2\u4e0a\u9501|\u9501\u7740|\u9501\u4e0a|\u9501\u4e86)[\u7684]",
                     "out": "locked"
                 },
                 {
-                    "in": "ul\u00e5st",
+                    "in": "(\u5df2\u89e3\u9501|\u6ca1[\u6709][\u4e0a]\u9501)[\u7684]",
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "<lys>",
+                    "in": "(\u706f|\u5438\u9876\u706f|\u7b52\u706f|\u5c04\u706f|\u53f0\u706f|\u5e8a\u5934\u706f|\u706f\u5149)",
                     "out": "light"
                 },
                 {
-                    "in": "<vifte>",
+                    "in": "(\u98ce\u6247|\u7535\u6247|\u5854\u6247|\u540a\u6247)",
                     "out": "fan"
                 },
                 {
-                    "in": "<bryter>",
+                    "in": "(\u5f00\u5173|\u7535\u6e90|\u63d2\u5ea7|\u901a\u65ad\u5668)",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "p\u00e5",
+                    "in": "(\u6253\u5f00|\u5f00\u7740|\u5f00\u4e86)[\u7684]",
                     "out": "on"
                 },
                 {
-                    "in": "av",
+                    "in": "(\u5173\u95ed|\u5173\u7740|\u5173\u4e86)[\u7684]",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "celsius",
                 {
-                    "in": "c",
+                    "in": "(\u6444\u6c0f\u5ea6|\u00b0C|\u2103|\u5ea6)",
                     "out": "celsius"
                 },
-                "fahrenheit",
                 {
-                    "in": "f",
+                    "in": "(\u534e\u6c0f\u5ea6|\u00b0F|\u2109)",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Det oppsto en uventet feil",
-            "no_area": "Det er ingen omr\u00e5der som heter {{ area }}",
-            "no_device_class": "{{ area }} har ingen {{ device_class }}",
-            "no_domain": "{{ area }} har ingen {{ domain }}",
-            "no_entity": "Finner ingen enhet som heter {{ entity }}",
-            "no_intent": "Jeg skj\u00f8nte dessverre ikke det"
+            "handle_error": "\u5904\u7406\u610f\u56fe\u65f6\u53d1\u751f\u610f\u5916\u9519\u8bef",
+            "no_area": "\u627e\u4e0d\u5230\u540d\u4e3a {{ area }} \u7684\u533a\u57df",
+            "no_device_class": "{{ area }} \u4e2d\u627e\u4e0d\u5230 {{ device_class }}",
+            "no_domain": "{{ area }} \u4e2d\u627e\u4e0d\u5230 {{ domain }}",
+            "no_entity": "\u627e\u4e0d\u5230\u540d\u4e3a {{ entity }} \u7684\u5b9e\u4f53",
+            "no_intent": "\u62b1\u6b49\uff0c\u6211\u4e0d\u80fd\u7406\u89e3"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched %}\nJa\n{% else: %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    Nei, ikke {{ no_match[:3] | join(\", \") }} og {{ (no_match | length - 3) }} til\n  {%- else -%}\n    Nei, ikke\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} og {% endif -%}\n      {{ name }}\n    {%- endfor %}\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Ja, {{ match[:3] | join(\", \") }} og {{ (match | length - 3) }} til\n  {%- else -%}\n    Ja,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} og {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else: %}\nNei\n{% endif %}\n",
-                "how_many": "{% if not query.matched: %}\n0\n{% else: %}\n{{ query.matched | length }}\n{% endif %}\n",
-                "one": "{{ slots.name }} er {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\nJa\n{% else: %}\nNei, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\nIngen\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} og {{ (match | length - 3) }} til\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} og {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+                "all": "{% if not query.unmatched: %}\n  \u662f\u7684\n{%- else -%}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  \u4e0d\uff0c{{ no_match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\u9664\u5916\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  \u662f\u7684\uff0c{{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\n  {{- slots.state[:-1] if slots.state[-1] == '\u7684' else slots.state }}\n{%- else -%}\n  \u6ca1\u6709\n{% endif %}\n",
+                "how_many": "{{ query.matched | length }}\n",
+                "one": "{{ slots.name }}\u73b0\u5728\u662f {{ state.state_with_unit }}",
+                "one_yesno": "{% if query.matched: %}\n\u662f\u7684\n{% else: %}\n\u4e0d\uff0c{{ slots.name }}\u662f{{ state.state }}\u7684\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u6ca1\u6709\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}{{ slots.state }}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "Lukket",
-                "cover_area": "Lukket {{ slots.area }}",
-                "cover_device_class": "Lukket {{ slots.device_class }}",
-                "default": "Slo av {{ state.domain }}",
-                "fans_area": "Slo av vifter",
-                "lights_area": "Slo av lys"
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u5173\u95ed",
+                "default": "{{ slots.name|default('') }}\u5df2\u5173\u95ed",
+                "fans_area": "{{ slots.area }}\u98ce\u6247\u5df2\u5173\u95ed",
+                "lights_area": "{{ slots.area }}\u706f\u5df2\u5173\u95ed",
+                "lock": "{{ slots.name|default('') }}\u5df2\u89e3\u9501"
             },
             "HassTurnOn": {
-                "cover": "\u00c5pnet",
-                "cover_area": "\u00c5pnet {{ slots.area }}",
-                "cover_device_class": "\u00c5pnet {{ slots.device_class }}",
-                "default": "Slo p\u00e5 {{ state.domain }}",
-                "fans_area": "Slo p\u00e5 vifter",
-                "lights_area": "Slo p\u00e5 lys",
-                "scene": "Aktivert",
-                "script": "Startet"
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u6253\u5f00",
+                "default": "{{ slots.name|default('') }}\u5df2\u6253\u5f00",
+                "fans_area": "{{ slots.area }}\u98ce\u6247\u5df2\u6253\u5f00",
+                "lights_area": "{{ slots.area }}\u706f\u5df2\u6253\u5f00",
+                "lock": "{{ slots.name|default('') }}\u5df2\u4e0a\u9501",
+                "scene": "{{ slots.name|default('') }}\u5df2\u5f00\u542f",
+                "script": "{{ slots.name|default('') }}\u811a\u672c\u5df2\u6267\u884c"
             }
         }
     },
-    "skip_words": [
-        "v\u00e6r s\u00e5 snill",
-        "takk",
-        "vennligts",
-        "kan du"
-    ]
+    "settings": {
+        "ignore_whitespace": true
+    },
+    "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nl.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962711683249879%*

 * *Differences: {"'expansion_rules'": "{'name_area': '(\\n  [[<in> de|het|een] {area}][ ]<name>\\n  |[de|het|een] "*

 * *                      "{name}[ ][<type>] [[in|op|van|bij] <area>]\\n)\\n', 'sensor_name_area': "*

 * *                      "'(\\n  [[door|met|bij] [de|het|een] {area}][ ]{name}\\n  |[<in> "*

 * *                      '[de|het|een] {area}] [door|met|bij] <name>\\n  |[<met>] [de|het|een] {name} '*

 * *                      "[[in|op|van|bij] <area>]\\n)\\n'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {2: {'sentences': ['[<doe> […]*

```diff
@@ -16,20 +16,21 @@
         "helderheid": "[de] (helderheid|felheid|intensiteit|lichtsterkte)",
         "in": "[in|op|van|bij]",
         "is": "(zijn|is|staa(n|t)|zit[ten]|word[t|en]|lig(t|gen))",
         "lamp": "[de|het|een] (lamp[en]|licht[en]|verlichting)",
         "met": "(door|met|bij)",
         "naar": "(naar|op)",
         "name": "[de|het] {name}",
-        "name_area": "(\n  [[door|met|bij] [de|het] {area}][ ]{name}\n  |[<in> [de|het] {area}] [door|met|bij] <name>\n  |[<met>] [de|het] {name} [[in|op|van|bij] <area>]\n)\n",
+        "name_area": "(\n  [[<in> de|het|een] {area}][ ]<name>\n  |[de|het|een] {name}[ ][<type>] [[in|op|van|bij] <area>]\n)\n",
         "op_slot": "<naar> (slot|vergrendeld)",
         "open": "(open|omhoog|naar boven|opwaarts)",
         "schakelaar": "[de|een] (schakelaar[s]|switch[es]|plug[gen])",
         "sensor": "[een|de] (apparaat|apparaten|sensor[s|en]|iets)",
         "sensor_area": "(\n  [[de|een] {area}][ ](apparaat|apparaten|sensor[s|en])\n  |[<in> [de|het] {area}] <sensor>\n  |[een|de] (apparaat|apparaten|sensor[s|en]|iets) [[in|op|van|bij] <area>]\n)\n",
+        "sensor_name_area": "(\n  [[door|met|bij] [de|het|een] {area}][ ]{name}\n  |[<in> [de|het|een] {area}] [door|met|bij] <name>\n  |[<met>] [de|het|een] {name} [[in|op|van|bij] <area>]\n)\n",
         "shade": "(screen[s]|rolgordijn[en])",
         "shutter": "(rolluik[en]|shutter[s])",
         "slot": "[de|het|een] ([deur]slot[en]|vergrendeling[en])",
         "slot_name_area": "[<in> <area>] (<slot> [van] [{area}[ ]]<name>|[de|het] {name}[ ]([deur]slot[en]|vergrendeling[en])) [[in|op|van|bij] [de|het] {area}]",
         "staat": "(status|staat|stand)",
         "temperature": "{temperature}[\u00b0|graden] [{temperature_unit}]",
         "type": "(<lamp>|<ventilator>|<afdekking>|<schakelaar>)",
@@ -73,215 +74,215 @@
                 {
                     "requires_context": {
                         "device_class": "carbon_monoxide",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<detecteer> [<met>] <name_area> {bs_carbon_monoxide_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_carbon_monoxide_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_carbon_monoxide_states:state} <detecteer> <name_area>",
+                        "<detecteer> [<met>] <sensor_name_area> {bs_carbon_monoxide_states:state} [<in> <area>]",
+                        "neemt <sensor_name_area> {bs_carbon_monoxide_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_carbon_monoxide_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_carbon_monoxide_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_carbon_monoxide_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_carbon_monoxide_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "carbon_monoxide",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "cold",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(is|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_cold_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_cold_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_cold_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_cold_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_cold_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_cold_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area>  {bs_cold_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area>  {bs_cold_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "cold",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "connectivity",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_connectivity_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_connectivity_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "connectivity",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "door",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_door_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_door_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "door",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "garage_door",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_garage_door_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_garage_door_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "garage_door",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "gas",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "<detecteer> [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_gas_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_gas_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_gas_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_gas_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_gas_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_gas_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_gas_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_gas_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "gas",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "heat",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_heat_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_heat_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_heat_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_heat_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_heat_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_heat_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_heat_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_heat_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "heat",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "light",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_light_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_light_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_light_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_light_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_light_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_light_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_light_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_light_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "light",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "lock",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_lock_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_lock_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "lock",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "moisture",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_moisture_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_moisture_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_moisture_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_moisture_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_moisture_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_moisture_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_moisture_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_moisture_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "moisture",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "motion",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "<detecteer> [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_motion_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_motion_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_motion_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_motion_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_motion_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_motion_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_motion_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_motion_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "motion",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "occupancy",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "<detecteer> [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_occupancy_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_occupancy_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "(is|zijn|word[t|en]) [er] [<in> <area>] {bs_occupancy_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_occupancy_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "(is|zijn|word[t|en]) [er] [<in> <area>] {bs_occupancy_states:state} <detecteer> <sensor_name_area>",
                         "(is|zijn|wordt[t|en]) [er] [<in> <area>] {bs_occupancy_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_occupancy_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_occupancy_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "occupancy",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "opening",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_opening_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_opening_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "opening",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -303,51 +304,51 @@
                     "requires_context": {
                         "device_class": "power",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_power_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_power_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_power_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_power_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_power_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_power_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_power_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_power_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "power",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "presence",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_presence_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_presence_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "presence",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "requires_context": {
                         "device_class": "problem",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> er [<in> <area>] {bs_problem_states:state} <name_area>",
-                        "(heeft|<detecteer>) <name_area> {bs_problem_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_problem_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_problem_states:state} <detecteer> <name_area>",
+                        "<is> er [<in> <area>] {bs_problem_states:state} <sensor_name_area>",
+                        "(heeft|<detecteer>) <sensor_name_area> {bs_problem_states:state} [<in> <area>]",
+                        "neemt <sensor_name_area> {bs_problem_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_problem_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_problem_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_problem_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_problem_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "problem",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -399,20 +400,20 @@
                 {
                     "requires_context": {
                         "device_class": "running",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "{bs_running_states:state} <name_area>",
+                        "{bs_running_states:state} <sensor_name_area>",
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_running_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_running_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_running_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_running_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_running_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_running_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_running_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_running_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "running",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -467,18 +468,18 @@
                     "requires_context": {
                         "device_class": "safety",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_safety_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_safety_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_safety_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_safety_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_safety_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_safety_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_safety_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_safety_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "safety",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -531,18 +532,18 @@
                     "requires_context": {
                         "device_class": "smoke",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_smoke_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_smoke_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_smoke_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_smoke_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_smoke_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_smoke_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_smoke_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_smoke_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "smoke",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -593,20 +594,20 @@
                 {
                     "requires_context": {
                         "device_class": "sound",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "maakt <name_area> {bs_sound_states:state}",
+                        "maakt <sensor_name_area> {bs_sound_states:state}",
                         "(<is>|<detecteer>) [er] [<in>|<met>] [<area>][ ]<name> [<in> <area>] {bs_sound_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_sound_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_sound_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_sound_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_sound_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_sound_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_sound_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_sound_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "sound",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -664,18 +665,18 @@
                     "requires_context": {
                         "device_class": "tamper",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "(<is>|<detecteer>) [er] [in|op|van|bij] [<area>][ |door |met |bij ]<name> [<in> <area>] {bs_tamper_states:state} [<in> <area>]",
-                        "neemt <name_area> {bs_tamper_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_tamper_states:state} <detecteer> <name_area>",
+                        "neemt <sensor_name_area> {bs_tamper_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
+                        "<is> [er] [<in> <area>] {bs_tamper_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_tamper_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_tamper_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_tamper_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "tamper",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -731,16 +732,16 @@
                     "requires_context": {
                         "device_class": "update",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "<is> [<in> <area>][ ]<name> [[in|op|van] [<area>]] {bs_update_states:state} [<in> <area>]",
-                        "<is> [er] [<in> <area>] [een] {bs_update_states:state} [klaar|beschikbaar] voor <name_area>",
-                        "<is> [er] voor <name_area> [een] {bs_update_states:state} [klaar|beschikbaar] [<in> <area>]"
+                        "<is> [er] [<in> <area>] [een] {bs_update_states:state} [klaar|beschikbaar] voor <sensor_name_area>",
+                        "<is> [er] voor <sensor_name_area> [een] {bs_update_states:state} [klaar|beschikbaar] [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "update",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -791,20 +792,20 @@
                 {
                     "requires_context": {
                         "device_class": "vibration",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "{bs_vibration_states:state} <name_area>",
-                        "(is|<detecteer>) [er] <name_area> {bs_vibration_states:state} [<in> <area>]",
+                        "{bs_vibration_states:state} <sensor_name_area>",
+                        "(is|<detecteer>) [er] <sensor_name_area> {bs_vibration_states:state} [<in> <area>]",
                         "neemt [<area>][ ]<name> [<in> <area>] {bs_vibration_states:state} (waar [<in> <area>]|[<in> <area>] waar)",
-                        "<is> [er] [<in> <area>] {bs_vibration_states:state} <detecteer> <name_area>",
+                        "<is> [er] [<in> <area>] {bs_vibration_states:state} <detecteer> <sensor_name_area>",
                         "<is> [er] [<in> <area>] {bs_vibration_states:state} <met> [<area>][ ]<name> <detecteer> [<in> <area>]",
-                        "<is> [er] <name_area> {bs_vibration_states:state} <detecteer> [<in> <area>]"
+                        "<is> [er] <sensor_name_area> {bs_vibration_states:state} <detecteer> [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "vibration",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -861,15 +862,15 @@
                 {
                     "requires_context": {
                         "device_class": "window",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
-                        "<is> <name_area> {bs_window_states:state} [<in> <area>]"
+                        "<is> <sensor_name_area> {bs_window_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "device_class": "window",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -1053,17 +1054,20 @@
                     "excludes_context": {
                         "domain": [
                             "cover",
                             "script"
                         ]
                     },
                     "sentences": [
-                        "[<doe>] <name>[ ][<type>] [<naar>] uit",
-                        "<zou> <name>[ ][<type>] [<naar>] (uit willen |uit kunnen |uit [ ])<doe>",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen|doen)"
+                        "[<doe>] <name>[ ][<type>] [<naar>] uit [<in> <area>]",
+                        "[<doe>] <name_area>[ ][<type>] [<naar>] uit",
+                        "<zou> <name>[ ][<type>] [<naar>] (uit willen |uit kunnen |uit [ ])<doe> [<in> <area>]",
+                        "<zou> <name_area>[ ][<type>] [<naar>] (uit willen |uit kunnen |uit [ ])<doe>",
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen|doen) [<in> <area>]",
+                        "[<zou>] <name_area>[ ][<type>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen|doen)"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
                         "[<doe>] [<alle>] <lamp> [<naar>] uit <in> <area>",
                         "<zou> [<alle>] <lamp> [<naar>] (uit willen |uit kunnen |uit[ ])<doe> <in> <area>",
@@ -1422,18 +1426,22 @@
                         "domain": [
                             "cover",
                             "scene",
                             "script"
                         ]
                     },
                     "sentences": [
-                        "[<doe>] <name>[ ][<type>] [<naar>] aan",
-                        "<zou> <name>[ ][<type>] [<naar>] ((aan|in) willen |(aan|in) kunnen |(aan|in) [ ])<doe>",
-                        "schakel <name>[ ][<type>] [<naar>] in",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|doen)"
+                        "[<doe>] <name>[ ][<type>] [<naar>] aan [<in> <area>]",
+                        "[<doe>] <name_area>[ ][<type>] [<naar>] aan",
+                        "<zou> <name>[ ][<type>] [<naar>] ((aan|in) willen |(aan|in) kunnen |(aan|in) [ ])<doe> [<in> <area>]",
+                        "<zou> <name_area>[ ][<type>] [<naar>] ((aan|in) willen |(aan|in) kunnen |(aan|in) [ ])<doe>",
+                        "schakel <name>[ ][<type>] [<naar>] in [<in> <area>]",
+                        "schakel <name_area>[ ][<type>] [<naar>] in",
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|doen) [<in> <area>]",
+                        "[<zou>] <name_area>[ ][<type>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|doen)"
                     ]
                 }
             ]
         }
     },
     "language": "nl",
     "lists": {
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/eu.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6849647266313933%*

 * *Differences: {"'expansion_rules'": "{'area': '{area}[n]', 'name': '{name}[n]', 'piztu': "*

 * *                      "'(piztu|aktibatu|gaitu)', 'itzali': '(itzali|desaktibatu|ezgaitu)', delete: "*

 * *                      "['ismin_halleri', 'cogulluk', 'temperature']}",*

 * * "'intents'": "{'HassTurnOff': {'data': {0: {'sentences': ['<itzali> <name> "*

 * *              "[argia[k]|etengailua[k]]', '<name> [argia[k]|etengailua[k]] itzali', 'desaktibatu "*

 * *              "<name> [argia[k]|etengailua[k]]'], 'excludes_context': OrderedDict([('d […]*

```diff
@@ -1,228 +1,207 @@
 {
     "expansion_rules": {
-        "area": "{area}<ismin_halleri>",
-        "cogulluk": "[(ler|leri|lar|lar\u0131)]",
-        "ismin_halleri": "[([(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u0131|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]i|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u00fc|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]u|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]e|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]a)][n][ki]",
-        "name": "{name}<cogulluk><ismin_halleri>",
-        "temperature": "{temperature} [{temperature_unit}]"
+        "area": "{area}[n]",
+        "itzali": "(itzali|desaktibatu|ezgaitu)",
+        "name": "{name}[n]",
+        "piztu": "(piztu|aktibatu|gaitu)"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
-                    "sentences": [
-                        "<name> (kapa | kapat | s\u00f6nd\u00fcr )"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<name> (kapa | kapat | indir ) "
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> <name> (kapa | kapat | indir )"
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "<itzali> <name> [argia[k]|etengailua[k]]",
+                        "<name> [argia[k]|etengailua[k]] itzali",
+                        "desaktibatu <name> [argia[k]|etengailua[k]]"
                     ]
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "garaj kap\u0131s\u0131n\u0131 (kapa | kapat | indir )"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (kapa | kapat | indir | \u00e7ek)"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "garaj kap\u0131s\u0131n\u0131 (a\u00e7 | y\u00fckselt)"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (a\u00e7 | y\u00fckselt)"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<name> ( a\u00e7 | yak | \u00e7al\u0131\u015ft\u0131r)"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<name> (a\u00e7 | y\u00fckselt) "
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> <name> (a\u00e7 | y\u00fckselt)"
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "<piztu> <name> [argia[k]|etengailua[k]]",
+                        "<name> [argia[k]|etengailua[k]] piztu",
+                        "aktibatu <name> [argia[k]|etengailua[k]]"
                     ]
                 }
             ]
         }
     },
-    "language": "tr",
+    "language": "eu",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
+        "brightness_level": {
+            "values": [
+                {
+                    "in": "(maximoa|altuena|gorena)",
+                    "out": 100
+                },
+                {
+                    "in": "(minimoa|baxuena|txikiena)",
+                    "out": 1
+                }
+            ]
+        },
         "color": {
             "values": [
                 {
-                    "in": "beyaz",
+                    "in": "zuria",
                     "out": "white"
                 },
                 {
-                    "in": "siyah",
+                    "in": "beltza",
                     "out": "black"
                 },
                 {
-                    "in": "k\u0131rm\u0131z\u0131",
+                    "in": "gorria",
                     "out": "red"
                 },
                 {
-                    "in": "turuncu",
+                    "in": "laranja",
                     "out": "orange"
                 },
                 {
-                    "in": "sar\u0131",
+                    "in": "horia",
                     "out": "yellow"
                 },
                 {
-                    "in": "ye\u015fil",
+                    "in": "berdea",
                     "out": "green"
                 },
                 {
-                    "in": "mavi",
+                    "in": "urdina",
                     "out": "blue"
                 },
                 {
-                    "in": "mor",
+                    "in": "morea",
                     "out": "purple"
                 },
                 {
-                    "in": "kahverengi",
+                    "in": "marroia",
                     "out": "brown"
-                },
-                {
-                    "in": "gri",
-                    "out": "grey"
-                },
+                }
+            ]
+        },
+        "on_off_domains": {
+            "values": [
                 {
-                    "in": "pembe",
-                    "out": "pink"
+                    "in": "argi(a)[k]|lanpara[k]",
+                    "out": "light"
                 },
                 {
-                    "in": "turkuaz",
-                    "out": "turquoise"
+                    "in": "haizegailu(a)[k]",
+                    "out": "fan"
                 },
                 {
-                    "in": "bordo",
-                    "out": "maroon"
-                },
+                    "in": "etengailu(a)[k]",
+                    "out": "switch"
+                }
+            ]
+        },
+        "on_off_states": {
+            "values": [
                 {
-                    "in": "bej",
-                    "out": "beige"
+                    "in": "piztu",
+                    "out": "on"
                 },
                 {
-                    "in": "lacivert",
-                    "out": "navy"
+                    "in": "itzali",
+                    "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 "celsius",
                 {
-                    "in": "c | santigrat",
+                    "in": "c",
+                    "out": "celsius"
+                },
+                {
+                    "in": "zentigrado",
                     "out": "celsius"
                 },
                 "fahrenheit",
                 {
-                    "in": "f | fahrenhayt",
+                    "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u0130stenilen ama\u00e7 i\u015flenirken bir hata olu\u015ftu.",
-            "no_area": "{{ area }}  ad\u0131nda alan yok.",
-            "no_device_class": "{{ area }}  bir {{ device_class }} i\u00e7ermiyor.",
-            "no_domain": "{{ area }}  bir {{ domain }} i\u00e7ermiyor.",
-            "no_entity": "{{ entity }} ad\u0131nda bir cihaz yok.",
-            "no_intent": "\u00dczg\u00fcn\u00fcm, bunu anlayamad\u0131m."
+            "handle_error": "Espero ez zen errore bat gertatu da agindua prozesatzean",
+            "no_area": "Ez dago {{ area }} izeneko gunerik",
+            "no_device_class": "Ez dago {{ device_class }} motako elementurik {{ area }} gunean",
+            "no_domain": "{{ area }} guneak ez dauka {{ domain }} moduko elementurik",
+            "no_entity": "Ez da {{ entity }} izeneko gailu edo entitaterik existitzen",
+            "no_intent": "Barkatu, ez dizut ulertu"
         },
         "intents": {
-            "HassGetState": {},
+            "HassGetState": {
+                "all": "TODO: {% if not query.unmatched: %}\n  Yes\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    No, {{ no_match[:3] | join(\", \") }} and {{ (no_match | length - 3) }} more not\n  {%- else -%}\n    No,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor %} not\n  {% endif %}\n{% endif %}\n",
+                "any": "TODO: {% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Yes, {{ match[:3] | join(\", \") }} and {{ (match | length - 3) }} more\n  {%- else -%}\n    Yes,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  No\n{% endif %}\n",
+                "how_many": "TODO: {{ query.matched | length }}\n",
+                "one": "TODO: {{ slots.name | capitalize }} is {{ state.state_with_unit }}\n",
+                "one_yesno": "TODO: {% if query.matched %}\n  Yes\n{% else %}\n  No, {{ state.state_with_unit }}\n{% endif %}\n",
+                "which": "TODO: {% if not query.matched %}\n  Not any\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} and {{ (match | length - 3) }} more\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+            },
             "HassTurnOff": {
-                "cover": "Closed {{ slots.name }}",
-                "cover_area": "Closed {{ slots.area }}",
-                "cover_device_class": "Closed {{ slots.device_class }}",
-                "default": "Turned off {{ slots.name }}",
-                "fans_area": "Turned off fans in {{ slots.area }}",
-                "lights_area": "Turned off lights in {{ slots.area }}"
+                "cover": "Itxita",
+                "cover_device_class": "{{ slots.device_class }} itxita",
+                "default": "{{ slots.name }} itzalita",
+                "fan_all": "Haizegailu guztiak itzalita",
+                "fans_area": "Haizegailuak itzalita",
+                "light_all": "Argi guztiak itzalita",
+                "lights_area": "Argiak itzalita",
+                "lock": "Irekita"
             },
             "HassTurnOn": {
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}",
-                "cover_device_class": "Opened {{ slots.device_class }}",
-                "default": "Turned on {{ slots.name }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "lights_area": "Turned on lights in {{ slots.area }}"
+                "cover": "Irekita",
+                "cover_device_class": "{{ slots.device_class }} irekita",
+                "default": "{{ slots.name }} piztuta",
+                "fans_area": "Haizegailuak piztuta",
+                "lights_area": "Argiak piztuta",
+                "lock": "Itxita",
+                "scene": "Aktibatuta",
+                "script": "Hasita"
             }
         }
     },
     "skip_words": [
-        "L\u00fctfen"
+        "mesedez",
+        "eskerrik asko"
     ]
 }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8691937373118439%*

 * *Differences: {"'expansion_rules'": "{'name': '{name}[的|嘅]', 'area': '{area}[的|嘅]', 'let': '[請|把|给|讓]', 'all': "*

 * *                      "'(全部|所有)[的|嘅]', 'what_is': '是什麼', 'how_many_is': '(是|有)(多少|幾|幾個)', 'which': "*

 * *                      "'[有|有没有|有無]哪[一](個|些)', 'to': '(為|到|至)', 'set_to': '(設置|設定|調節|調)(為|到|至)', "*

 * *                      "'turn_on': '(打開|開啟|開|着)', 'turn_off': '(關閉|關掉|關了|關|閂)', 'open': '(打開|開)', "*

 * *                      "'close': '(關閉|關掉|關了|關|閂)', 'light': '(燈|吸頂燈|筒燈|射燈|檯燈|台燈|床頭燈|燈光)[的|嘅]', "*

 * *                    […]*

```diff
@@ -1,222 +1,154 @@
 {
     "expansion_rules": {
-        "all": "(\u5168\u90e8|\u6240\u6709)[\u7684]",
-        "area": "{area}[\u7684]",
+        "all": "(\u5168\u90e8|\u6240\u6709)[\u7684|\u5605]",
+        "area": "{area}[\u7684|\u5605]",
         "brightness": "[\u767e\u5206\u4e4b]{brightness}[%]",
-        "close": "(\u5173\u95ed|\u5173\u6389|\u5173\u4e86|\u5173)",
-        "how_many_is": "(\u662f\u591a\u5c11|\u6709\u591a\u5c11|\u6709\u51e0\u4e2a)",
-        "let": "[\u628a|\u5c06|\u8ba9|\u7ed9]",
-        "light": "(\u706f|\u5438\u9876\u706f|\u7b52\u706f|\u5c04\u706f|\u53f0\u706f|\u5e8a\u5934\u706f|\u706f\u5149)[\u7684]",
-        "name": "{name}[\u7684]",
-        "open": "(\u6253\u5f00|\u5f00)",
-        "set_to": "(\u8bbe\u7f6e|\u8bbe\u5b9a|\u8c03\u8282|\u8c03|\u8bbe)(\u4e3a|\u5230|\u81f3)",
-        "temp": "\u6e29\u5ea6",
-        "temperature": "{temperature}[{temperature_unit}]",
-        "to": "(\u4e3a|\u5230|\u6210|\u81f3)",
-        "turn_off": "(\u5173\u95ed|\u5173\u6389|\u5173\u4e86|\u5173)",
-        "turn_on": "(\u6253\u5f00|\u5f00\u542f|\u5f00)",
-        "what_is": "\u662f\u4ec0\u4e48",
-        "which": "[\u6709|\u6709\u6ca1\u6709|\u6709\u7121]\u54ea[\u4e00](\u4e2a|\u4e9b)"
+        "close": "(\u95dc\u9589|\u95dc\u6389|\u95dc\u4e86|\u95dc|\u9582)",
+        "how_many_is": "(\u662f|\u6709)(\u591a\u5c11|\u5e7e|\u5e7e\u500b)",
+        "let": "[\u8acb|\u628a|\u7ed9|\u8b93]",
+        "light": "(\u71c8|\u5438\u9802\u71c8|\u7b52\u71c8|\u5c04\u71c8|\u6aaf\u71c8|\u53f0\u71c8|\u5e8a\u982d\u71c8|\u71c8\u5149)[\u7684|\u5605]",
+        "name": "{name}[\u7684|\u5605]",
+        "open": "(\u6253\u958b|\u958b)",
+        "set_to": "(\u8a2d\u7f6e|\u8a2d\u5b9a|\u8abf\u7bc0|\u8abf)(\u70ba|\u5230|\u81f3)",
+        "temp": "\u6eab\u5ea6",
+        "temperature": "{temperature} [{temperature_unit}]",
+        "to": "(\u70ba|\u5230|\u81f3)",
+        "turn_off": "(\u95dc\u9589|\u95dc\u6389|\u95dc\u4e86|\u95dc|\u9582)",
+        "turn_on": "(\u6253\u958b|\u958b\u555f|\u958b|\u7740)",
+        "what_is": "\u662f\u4ec0\u9ebc",
+        "which": "[\u6709|\u6709\u6ca1\u6709|\u6709\u7121]\u54ea[\u4e00](\u500b|\u4e9b)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "scene",
-                            "script"
-                        ]
-                    },
                     "response": "one",
                     "sentences": [
-                        "[<area>]<name>[\u72b6\u6001](<what_is>|<how_many_is>)",
-                        "[<area>]<name>[<what_is>]\u72b6\u6001"
+                        "[<area>]<name>[\u72c0\u614b](<what_is>|<how_many_is>)",
+                        "[<area>]<name>[<what_is>]\u72c0\u614b"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[<area>]{name}\u662f\u4e0d\u662f{on_off_states:state}",
-                        "[<area>]{name}[\u662f]{on_off_states:state}[\u5417|\u4e0d]"
+                        "[<area>]{name}\u4fc2\u5514\u4fc2{on_off_states:state}",
+                        "[<area>]{name}[\u662f]{on_off_states:state}[\u55ce|\u5497|\u5497\u55ce]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "[{area}][\u6709|\u6709\u6ca1\u6709]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f]{on_off_states:state}[\u5417|\u4e0d]"
+                        "[{area}][\u6709|\u6709\u6ca1\u6709|\u6709\u5187|\u6709\u7121]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f|\u4fc2\u5514\u4fc2]{on_off_states:state}[\u55ce|\u4e0d|\u5497\u55ce]"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "[<area>][<all>]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{on_off_states:state}[\u5417|\u4e0d]"
+                        "[<area>][<all>]{on_off_domains:domain}[\u662f|\u662f\u4e0d\u662f|\u4fc2\u5514\u4fc2]\u90fd[\u662f|\u4fc2]{on_off_states:state}[\u55ce|\u4e0d]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "[<area>]<which>{on_off_domains:domain}[\u662f]{on_off_states:state}",
+                        "[<area>]<which>{on_off_domains:domain}[\u662f|\u4fc2]{on_off_states:state}",
                         "<which>[<area>]{on_off_domains:domain}[\u662f]{on_off_states:state}"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "[{area}]<how_many_is>{on_off_domains:domain}[\u662f]{on_off_states:state}",
-                        "<how_many_is>[<area>]{on_off_domains:domain}[\u662f]{on_off_states:state}"
+                        "[{area}]<how_many_is>{on_off_domains:domain}[\u662f|\u4fc2]{on_off_states:state}",
+                        "<how_many_is>[<area>]{on_off_domains:domain}[\u662f|\u4fc2]{on_off_states:state}"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[<area>]{name}(\u662f|\u662f\u4e0d\u662f){cover_states:state}[\u5417|\u4e0d]"
+                        "[<area>]{name}(\u662f|\u662f\u4e0d\u662f|\u4fc2|\u4fc2\u5514\u4fc2){cover_states:state}[\u55ce|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "[{area}][\u6709|\u6709\u6ca1\u6709]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]{cover_states:state}[\u5417|\u4e0d]"
+                        "[{area}][\u6709|\u6709\u6ca1\u6709|\u6709\u7121]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f|\u4fc2|\u4fc2\u5514\u4fc2]{cover_states:state}[\u55ce|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "[<area>][<all>]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{cover_states:state}[\u5417|\u4e0d]",
-                        "<all><area>{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{cover_states:state}[\u5417|\u4e0d]"
+                        "[<area>][<all>]{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f|\u4fc2|\u4fc2\u5514\u4fc2]\u90fd[\u662f|\u4fc2]{cover_states:state}[\u55ce|\u4e0d]",
+                        "<all><area>{cover_classes:device_class}[\u662f|\u662f\u4e0d\u662f|\u4fc2|\u4fc2\u5514\u4fc2]\u90fd[\u662f|\u4fc2]{cover_states:state}[\u55ce|\u4e0d]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "[<area>]<which>{cover_classes:device_class}[\u662f]{cover_states:state}",
-                        "<which>[<area>]{cover_classes:device_class}[\u662f]{cover_states:state}"
+                        "[<area>]<which>{cover_classes:device_class}[\u662f|\u4fc2]{cover_states:state}",
+                        "<which>[<area>]{cover_classes:device_class}[\u662f|\u4fc2]{cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "[{area}]<how_many_is>{cover_classes:device_class}[\u662f]{cover_states:state}",
-                        "<how_many_is>[<area>]{cover_classes:device_class}[\u662f]{cover_states:state}"
+                        "[{area}]<how_many_is>{cover_classes:device_class}[\u662f|\u4fc2]{cover_states:state}",
+                        "<how_many_is>[<area>]{cover_classes:device_class}[\u662f|\u4fc2]{cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "[<area>]{name}(\u662f\u4e0d\u662f|\u6709\u6ca1\u6709){lock_states:state}",
-                        "[<area>]{name}[\u662f|\u6709]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "[{area}][\u6709|\u6709\u6ca1\u6709](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}[\u5417|\u4e0d]",
-                        "{area}(\u95e8|\u9501|\u95e8\u9501)[\u6709|\u6709\u6ca1\u6709]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "[<area>][<all>](\u95e8|\u9501|\u95e8\u9501)[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "[<area>](<which>|\u54ea[\u4e00]\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "(<which>|\u54ea[\u4e00]\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "<area>(\u95e8|\u9501|\u95e8\u9501)(<which>|\u54ea[\u4e00]\u6247)[\u662f]{lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "[{area}](<how_many_is>|\u6709\u51e0\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "(<how_many_is>|\u6709\u51e0\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "{area}(\u95e8|\u9501|\u95e8\u9501)(<how_many_is>|\u6709\u51e0\u6247)[\u662f]{lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "response": "fans_area",
                     "sentences": [
-                        "<turn_off><area>(\u98ce\u6247|\u540a\u6247)",
-                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_off>"
+                        "<turn_off> <area> (\u98a8\u6247 | \u540a\u6247)"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
+                        "domain": "cover"
                     },
                     "sentences": [
                         "<turn_off>[<area>]{name}",
                         "[<let>][<area>]{name}<turn_off>"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_off><area><light>",
-                        "[<let>]<area><light><turn_off>"
+                        "<turn_off> <area> <light>",
+                        "[<let>] <area> <light> <turn_off>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
@@ -225,16 +157,16 @@
                     "sentences": [
                         "<close>[<area>]{name}",
                         "[<let>][<area>]{name}<close>"
                     ]
                 },
                 {
                     "sentences": [
-                        "<close>\u8f66\u5e93\u7684[\u5927|\u5377\u95f8]\u95e8",
-                        "[<let>]\u8f66\u5e93\u7684[\u5927|\u5377\u95f8]\u95e8<close>"
+                        "<close>\u8eca\u623f[\u7684][\u5927|\u6372\u9598]\u9580",
+                        "[<let>]\u8eca\u623f[\u7684][\u5927|\u6372\u9598]\u9580<close>"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
@@ -242,58 +174,24 @@
                     "sentences": [
                         "<close>[<area>]{cover_classes:device_class}",
                         "[<let>][<area>]{cover_classes:device_class}<close>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "[\u6253|\u89e3]\u5f00[<area>]{name}[[\u7684]\u9501]",
-                        "[<let>][<area>]{name}[[\u7684]\u9501](\u6253\u5f00|\u89e3\u9501)"
-                    ]
-                },
-                {
-                    "response": "lock",
-                    "sentences": [
-                        "[\u6253|\u89e3]\u5f00<area>[<all>][\u95e8]\u9501",
-                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u6253\u5f00|\u89e3\u9501)",
-                        "{area}(\u5f00|\u89e3)\u9501"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "scene"
-                    },
-                    "response": "scene",
-                    "sentences": [
-                        "[\u6fc0\u6d3b|\u5f00\u542f|\u6253\u5f00|\u5207\u6362[\u5230]]<name>[\u573a\u666f|\u6a21\u5f0f]",
-                        "<name>[\u573a\u666f|\u6a21\u5f0f]\u5f00\u542f"
-                    ],
-                    "slots": {
-                        "domain": "scene"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_on><area><light>",
-                        "[<let>]<area><light><turn_on>"
+                        "<turn_on> <area> <light>",
+                        "[<let>] <area> <light> <turn_on>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
@@ -302,16 +200,16 @@
                     "sentences": [
                         "<open>[<area>]{name}",
                         "[<let>][<area>]{name}<open>"
                     ]
                 },
                 {
                     "sentences": [
-                        "<open>\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8",
-                        "[<let>]\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8<open>"
+                        "<open>\u8eca\u623f[\u7684][\u5927|\u6372\u9598]\u9580",
+                        "[<let>]\u8eca\u623f[\u7684][\u5927|\u6372\u9598]\u9580<open>"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
@@ -323,288 +221,255 @@
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area",
                     "sentences": [
-                        "<turn_on><area>(\u98ce\u6247|\u540a\u6247)",
-                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_on>"
+                        "<turn_on><area>(\u98a8\u6247|\u540a\u6247)"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "\u5173(\u95ed|\u4e0a)[<area>]{name}[[\u7684]\u9501]",
-                        "[<let>][<area>]{name}[[\u7684]\u9501](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)"
-                    ]
-                },
-                {
-                    "response": "lock",
-                    "sentences": [
-                        "\u5173(\u95ed|\u4e0a)<area>[<all>][\u95e8]\u9501",
-                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)",
-                        "{area}(\u4e0a|\u5173)\u9501"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
-                    "sentences": [
-                        "[\u8fd0\u884c|\u6267\u884c]<name>[\u811a\u672c]"
-                    ],
-                    "slots": {
-                        "domain": "script"
-                    }
-                },
-                {
                     "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
+                        "domain": "cover"
                     },
                     "sentences": [
                         "<turn_on>[<area>]{name}",
                         "[<let>][<area>]{name}<turn_on>"
                     ]
                 }
             ]
         }
     },
-    "language": "zh-cn",
+    "language": "zh-hk",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "brightness_level": {
             "values": [
                 {
-                    "in": "\u6700(\u4eae|\u9ad8|\u5927)",
+                    "in": "(\u6700\u5927|\u6700\u5149|\u6700\u9ad8|\u6700\u4eae)",
                     "out": 100
                 },
                 {
-                    "in": "\u6700(\u6697|\u4f4e|\u5c0f)",
+                    "in": "(\u6700\u5c0f|\u6700\u6697|\u6700\u4f4e|\u6700\u9ed1)",
                     "out": 1
                 }
             ]
         },
         "color": {
             "values": [
                 {
-                    "in": "\u767d\u8272",
-                    "out": "white"
-                },
-                {
-                    "in": "\u9ed1\u8272",
-                    "out": "black"
-                },
-                {
                     "in": "\u7ea2\u8272",
                     "out": "red"
                 },
                 {
                     "in": "\u6a59\u8272",
                     "out": "orange"
                 },
                 {
                     "in": "\u9ec4\u8272",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u7eff\u8272",
+                    "in": "\u7da0\u8272",
                     "out": "green"
                 },
                 {
-                    "in": "\u84dd\u8272",
+                    "in": "\u85cd\u8272",
                     "out": "blue"
                 },
                 {
                     "in": "\u7d2b\u8272",
                     "out": "purple"
                 },
                 {
+                    "in": "\u767d\u8272",
+                    "out": "white"
+                },
+                {
+                    "in": "\u9ed1\u8272",
+                    "out": "black"
+                },
+                {
                     "in": "\u68d5\u8272",
                     "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "(\u906e\u9633|\u96e8)(\u84ec|\u68da)",
+                    "in": "(\u906e\u967d|\u96e8)(\u84ec|\u68da)",
                     "out": "awning"
                 },
                 {
-                    "in": "(\u767e\u53f6\u7a97|\u767e\u53f6\u5e18|\u5377\u5e18)",
+                    "in": "(\u767e\u8449\u7a97|\u767e\u8449\u7c3e|\u6372\u7c3e)",
                     "out": "blind"
                 },
                 {
-                    "in": "\u7a97\u5e18",
+                    "in": "\u7a97\u7c3e",
                     "out": "curtain"
                 },
                 {
-                    "in": "(\u95e8|\u623f\u95e8|\u5377\u95f8\u95e8)",
+                    "in": "(\u9580|\u623f\u9580|\u6372\u9598\u9580)",
                     "out": "door"
                 },
                 {
-                    "in": "\u8f66\u5e93\u95e8",
+                    "in": "\u8eca\u623f\u9580",
                     "out": "garage"
                 },
                 {
-                    "in": "(\u5927\u95e8|\u9662\u5b50\u95e8|\u94c1\u95e8)",
+                    "in": "(\u5927\u9580|\u9662\u5b50\u9580|\u9435\u9580)",
                     "out": "gate"
                 },
                 {
-                    "in": "\u906e\u9633\u5e18",
+                    "in": "\u906e\u967d\u7c3e",
                     "out": "shade"
                 },
                 {
-                    "in": "\u767e\u53f6\u7a97\u6237",
+                    "in": "\u767e\u8449\u7a97\u6236",
                     "out": "shutter"
                 },
                 {
-                    "in": "\u7a97\u6237",
+                    "in": "\u7a97\u6236",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "(\u6253\u5f00|\u5f00\u7740|\u5f00\u4e86)[\u7684]",
+                    "in": "(\u6253\u958b|\u958b\u8457|\u958b\u4e86|\u958b\u5497|\u6253\u958b)[\u7684|\u5497]",
                     "out": "open"
                 },
                 {
-                    "in": "(\u5173\u95ed|\u5173\u7740|\u5173\u4e86)[\u7684]",
+                    "in": "(\u95dc\u9589|\u95dc\u8457|\u95dc\u4e86|\u95dc\u5497|\u9582\u5497)[\u7684|\u5497]",
                     "out": "closed"
                 },
                 {
-                    "in": "\u6253\u5f00\u4e2d",
+                    "in": "\u6253\u958b\u7dca",
                     "out": "opening"
                 },
                 {
-                    "in": "\u5173\u95ed\u4e2d",
+                    "in": "\u95dc\u9589\u7dca",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "(\u5df2\u4e0a\u9501|\u9501\u7740|\u9501\u4e0a|\u9501\u4e86)[\u7684]",
+                    "in": "(\u5df2\u4e0a\u9396|\u9396\u8457|\u9396\u4e0a|\u9396\u4e86|\u9396\u5497)[\u7684|\u5605]",
                     "out": "locked"
                 },
                 {
-                    "in": "(\u5df2\u89e3\u9501|\u6ca1[\u6709][\u4e0a]\u9501)[\u7684]",
+                    "in": "(\u5df2\u89e3\u9396|\u6c92[\u6709][\u4e0a]\u9396|\u7121[\u4e0a]\u9396)[\u7684|\u5605]",
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "(\u706f|\u5438\u9876\u706f|\u7b52\u706f|\u5c04\u706f|\u53f0\u706f|\u5e8a\u5934\u706f|\u706f\u5149)",
+                    "in": "(\u71c8|\u5929\u82b1\u71c8|\u7b52\u71c8|\u5c04\u71c8|\u6aaf\u71c8|\u5e8a\u982d\u71c8|\u71c8\u5149)",
                     "out": "light"
                 },
                 {
-                    "in": "(\u98ce\u6247|\u7535\u6247|\u5854\u6247|\u540a\u6247)",
+                    "in": "(\u98a8\u6247|\u96fb\u98a8\u6247|\u5854\u6247|\u540a\u6247)",
                     "out": "fan"
                 },
                 {
-                    "in": "(\u5f00\u5173|\u7535\u6e90|\u63d2\u5ea7|\u901a\u65ad\u5668)",
+                    "in": "(\u958b\u95dc|\u958b\u95dc\u5236|\u96fb\u6e90|\u63d2\u5ea7|\u901a\u65b7\u5668)",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "(\u6253\u5f00|\u5f00\u7740|\u5f00\u4e86)[\u7684]",
+                    "in": "(\u6253\u958b|\u958b\u8457|\u958b\u4e86|\u958b\u5497|\u958b)[\u7684]",
                     "out": "on"
                 },
                 {
-                    "in": "(\u5173\u95ed|\u5173\u7740|\u5173\u4e86)[\u7684]",
+                    "in": "(\u95dc\u9589|\u95dc\u8457|\u95dc\u4e86|\u95dc\u5497|\u9582\u5497|\u9582)[\u7684]",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 {
-                    "in": "(\u6444\u6c0f\u5ea6|\u00b0C|\u2103|\u5ea6)",
+                    "in": "c|\u651d\u6c0f|\u5ea6|\u00b0C|\u2103",
                     "out": "celsius"
                 },
                 {
-                    "in": "(\u534e\u6c0f\u5ea6|\u00b0F|\u2109)",
+                    "in": "f|\u83ef\u6c0f|\u5ea6|\u00b0F|\u2109",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u5904\u7406\u610f\u56fe\u65f6\u53d1\u751f\u610f\u5916\u9519\u8bef",
-            "no_area": "\u627e\u4e0d\u5230\u540d\u4e3a {{ area }} \u7684\u533a\u57df",
-            "no_device_class": "{{ area }} \u4e2d\u627e\u4e0d\u5230 {{ device_class }}",
-            "no_domain": "{{ area }} \u4e2d\u627e\u4e0d\u5230 {{ domain }}",
-            "no_entity": "\u627e\u4e0d\u5230\u540d\u4e3a {{ entity }} \u7684\u5b9e\u4f53",
-            "no_intent": "\u62b1\u6b49\uff0c\u6211\u4e0d\u80fd\u7406\u89e3"
+            "handle_error": "\u8655\u7406\u6642\u767c\u751f\u610f\u5916\u932f\u8aa4",
+            "no_area": "\u6c92\u6709\u5340\u57df\u540d\u53eb {{ area }}",
+            "no_device_class": "\u5340\u57df\u540d {{ area }} \u4e0d\u5305\u542b {{ device_class }}",
+            "no_domain": "\u5340\u57df\u540d {{ area }} \u4e0d\u5305\u542b {{ domain }}",
+            "no_entity": "\u7121\u8a2d\u5099\u6216\u5be6\u9ad4\u53eb {{ entity }}",
+            "no_intent": "\u5c0d\u5514\u4f4f\uff0c\u6211\u807d\u4e0d\u660e\u767d"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  \u662f\u7684\n{%- else -%}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  \u4e0d\uff0c{{ no_match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\u9664\u5916\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  \u662f\u7684\uff0c{{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\n  {{- slots.state[:-1] if slots.state[-1] == '\u7684' else slots.state }}\n{%- else -%}\n  \u6ca1\u6709\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  \u4fc2\u5440\n{%- else -%}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  \u5514\u4fc2\u5440\uff0c{{ no_match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\u9664\u5916\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  \u4fc2\u5440\uff0c{{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}\n  {{- slots.state[:-1] if slots.state[-1] == '\u7684' else slots.state }}\n{%- else -%}\n  \u7121\u5440\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "{{ slots.name }}\u73b0\u5728\u662f {{ state.state_with_unit }}",
-                "one_yesno": "{% if query.matched: %}\n\u662f\u7684\n{% else: %}\n\u4e0d\uff0c{{ slots.name }}\u662f{{ state.state }}\u7684\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  \u6ca1\u6709\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}{{ slots.state }}\n{% endif %}\n"
+                "one": "{{ slots.name }}\u73fe\u5728\u4fc2{{state.state_with_unit}}",
+                "one_yesno": "{% if query.matched: %}\n\u4fc2\u5440\n{% else: %}\n\u5514\u4fc2\u5440\uff0c{{ slots.name }}\u4fc2{{ state.state }}\u5497\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u7121\u5440\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {{ match[:4] | join(\"\u3001\") }}{{ '\u7b49' if match|length > 4 else '' }}{{ slots.state }}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u5173\u95ed",
-                "default": "{{ slots.name|default('') }}\u5df2\u5173\u95ed",
-                "fans_area": "{{ slots.area }}\u98ce\u6247\u5df2\u5173\u95ed",
-                "lights_area": "{{ slots.area }}\u706f\u5df2\u5173\u95ed",
-                "lock": "{{ slots.name|default('') }}\u5df2\u89e3\u9501"
+                "cover": "{{ slots.name }}\u5df2\u95dc\u9589",
+                "cover_area": "{{ slots.area }}\u7a97\u7c3e\u5df2\u95dc\u9589",
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u95dc\u9589",
+                "cover_door": "{{ slots.area }}\u9580\u5df2\u95dc\u9589",
+                "cover_window": "{{ slots.area }}\u7a97\u6236\u5df2\u95dc\u9589",
+                "default": "{{ slots.name|default('') }}\u5df2\u95dc\u9589",
+                "fans_area": "{{ slots.area }}\u98a8\u6247\u5df2\u95dc\u9589",
+                "lights_area": "{{ slots.area }}\u71c8\u5df2\u95dc\u9589",
+                "lock": "{{ slots.name|default('') }}\u5df2\u89e3\u9396"
             },
             "HassTurnOn": {
-                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u6253\u5f00",
-                "default": "{{ slots.name|default('') }}\u5df2\u6253\u5f00",
-                "fans_area": "{{ slots.area }}\u98ce\u6247\u5df2\u6253\u5f00",
-                "lights_area": "{{ slots.area }}\u706f\u5df2\u6253\u5f00",
-                "lock": "{{ slots.name|default('') }}\u5df2\u4e0a\u9501",
-                "scene": "{{ slots.name|default('') }}\u5df2\u5f00\u542f",
-                "script": "{{ slots.name|default('') }}\u811a\u672c\u5df2\u6267\u884c"
+                "cover": "{{ slots.name }}\u5df2\u6253\u958b",
+                "cover_area": "{{ slots.area }}\u7a97\u7c3e\u5df2\u6253\u958b",
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u6253\u958b",
+                "cover_door": "{{ slots.area }}\u9580\u5df2\u6253\u958b",
+                "cover_window": "{{ slots.area }}\u7a97\u6236\u5df2\u6253\u958b",
+                "default": "{{ slots.name }}\u5df2\u6253\u958b",
+                "fans_area": "{{ slots.area }}\u98a8\u6247\u5df2\u6253\u958b",
+                "lights_area": "{{ slots.area }}\u71c8\u5df2\u6253\u958b",
+                "lock": "{{ slots.name|default('') }}\u5df2\u4e0a\u9396",
+                "scene": "{{ slots.name|default('') }}\u5df2\u958b\u555f",
+                "script": "{{ slots.name|default('') }}\u8173\u672c\u5df2\u57f7\u884c"
             }
         }
     },
     "settings": {
         "ignore_whitespace": true
     },
     "skip_words": []
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919642857142857%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {0: {'sentences': {insert: [(0, '<setzen> <artikel> "*

 * *              "Helligkeit von <name> auf <brightness> [ein]'), (1, '<artikel> Helligkeit von "*

 * *              "<name> auf <brightness> <setzen>'), (2, 'dimme [<artikel> Helligkeit [von] "*

 * *              "<artikel>] <name> [auf|zu] <brightness>')], delete: [2, 1, 0]}}, 1: {'sentences': "*

 * *              "{insert: [(0, '<setzen> <artikel> Helligkeit [<lichter>|<alle_lichter>] [<area>] "*

 * *              "auf <brightness> [ […]*

```diff
@@ -1,55 +1,55 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness",
                     "sentences": [
-                        "<setzen> [die] Helligkeit von <name> auf <brightness> [ein]",
-                        "[die] Helligkeit von <name> auf <brightness> <setzen>",
-                        "dimme [[die] Helligkeit [von] der] <name> [auf|zu] <brightness>",
+                        "<setzen> <artikel> Helligkeit von <name> auf <brightness> [ein]",
+                        "<artikel> Helligkeit von <name> auf <brightness> <setzen>",
+                        "dimme [<artikel> Helligkeit [von] <artikel>] <name> [auf|zu] <brightness>",
                         "<name> [auf|zu] <brightness> dimmen"
                     ]
                 },
                 {
                     "response": "brightness",
                     "sentences": [
-                        "<setzen> [die] Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> [ein]",
-                        "[die] Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> <setzen>",
+                        "<setzen> <artikel> Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> [ein]",
+                        "<artikel> Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> <setzen>",
                         "dimme [<lichter>|<alle_lichter>] [<area>] [auf|zu] <brightness>",
                         "[<lichter>|<alle_lichter>] [<area>] [auf|zu] <brightness> dimmen"
                     ]
                 },
                 {
                     "response": "color",
                     "sentences": [
-                        "<setzen> [die Farbe (von|[von] der)] <name> [auf|zu] {color}",
-                        "[die Farbe (von|[von] der)] <name> auf {color} <setzen>",
+                        "<setzen> <artikel> [Farbe (von|[von] <artikel>)] <name> [auf|zu] {color}",
+                        "[<artikel> Farbe (von|[von] <artikel>)] <name> auf {color} <setzen>",
                         "Lass[e] <name> {color} [er]leuchten",
                         "<name> {color} [er]leuchten lassen"
                     ]
                 },
                 {
                     "response": "color",
                     "sentences": [
-                        "<setzen> die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color}",
-                        "die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color} <setzen>"
+                        "<setzen> <artikel> Farbe [<lichter>|<alle_lichter>] [<area>] auf {color}",
+                        "<artikel> Farbe [<lichter>|<alle_lichter>] [<area>] auf {color} <setzen>"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "brightness",
                     "sentences": [
-                        "<setzen> <name> auf [die|das] {brightness_level:brightness} [Helligkeit|Stufe] [ein]",
-                        "<setzen> [die] Helligkeit [<von_dem>] <name> auf [die|das] {brightness_level:brightness} [Stufe] [ein]",
-                        "[die] Helligkeit [<von_dem>] <name> auf [die|das] {brightness_level:brightness} [Stufe] <setzen>",
-                        "<name> auf [die|das] {brightness_level:brightness} [Helligkeit|Stufe] <setzen>"
+                        "<setzen> <name> auf <artikel> {brightness_level:brightness} [Helligkeit|Stufe] [ein]",
+                        "<setzen> <artikel> Helligkeit [<von_dem>] <name> auf <artikel> {brightness_level:brightness} [Stufe] [ein]",
+                        "<artikel> Helligkeit [<von_dem>] <name> auf <artikel> {brightness_level:brightness} [Stufe] <setzen>",
+                        "<name> auf <artikel> {brightness_level:brightness} [Helligkeit|Stufe] <setzen>"
                     ]
                 }
             ]
         }
     },
     "language": "de",
     "responses": {
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nl.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7928240740740741%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {0: {'sentences': ['[<doe>|<zou>] <name>[ ][<lamp>][ "*

 * *              "][<helderheid>] [<naar>] <brightness> [[willen|kunnen] <doe>]', '[<doe>|<zou>] "*

 * *              '<helderheid> [van] <name>[ ][<lamp>] [<naar>] <brightness> [[willen|kunnen] '*

 * *              "<doe>]']}, 1: {'sentences': ['[<doe>|<zou>] [<helderheid>] <in> <area>[[ ]<lamp>] "*

 * *              "[<naar>] <brightness> [[willen|kunnen] <doe>]', '[<doe>|<zou>] <area>[ "*

 * *              "][<helderheid>|lamp] [<na […]*

```diff
@@ -1,74 +1,72 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness",
                     "sentences": [
-                        "<endre> <navn> [til] [lysstyrke] [til] <lysstyrke>",
-                        "<endre> lysstyrke[n] <i_p\u00e5> <navn> til <lysstyrke>"
+                        "[<doe>|<zou>] <name>[ ][<lamp>][ ][<helderheid>] [<naar>] <brightness> [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <helderheid> [van] <name>[ ][<lamp>] [<naar>] <brightness> [[willen|kunnen] <doe>]"
                     ]
                 },
                 {
                     "response": "brightness",
                     "sentences": [
-                        "<endre> lysstyrke[n] <i_p\u00e5> <omr\u00e5de> til <lysstyrke>",
-                        "<endre> <omr\u00e5de> [til] [lysstyrke[n]] [til] <lysstyrke>"
+                        "[<doe>|<zou>] [<helderheid>] <in> <area>[[ ]<lamp>] [<naar>] <brightness> [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <area>[ ][<helderheid>|lamp] [<naar>] <brightness> [[willen|kunnen] <doe>]"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "brightness",
                     "sentences": [
-                        "<endre> <navn> [til] {brightness_level:brightness}",
-                        "<endre> lysstyrke[n] [til] <navn> [til] {brightness_level:brightness}"
+                        "[<doe>|<zou>] <name>[ ][lamp][ ][<helderheid>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <helderheid> [van] <name>[ ][<lamp>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <name>[ ][lamp] [<naar>] [de|het] {brightness_level:brightness} <helderheid> [[willen|kunnen] <doe>]"
                     ]
                 },
                 {
-                    "response": "brightness_area",
+                    "response": "brightness",
                     "sentences": [
-                        "<endre> lysstyrke[n] <i_p\u00e5> <omr\u00e5de> [til] {brightness_level:brightness}",
-                        "<endre> <omr\u00e5de> [til] [lysstyrke[n]] [til] {brightness_level:brightness}"
+                        "[<doe>|<zou>] [<helderheid>] <in> <area> [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <area>[ ][<helderheid>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] <area> [<naar>] [de|het] {brightness_level:brightness} [<helderheid>] [[willen|kunnen] <doe>]"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
                     "response": "color",
                     "sentences": [
-                        "<endre> <navn> farge til <farge>",
-                        "<endre> [farge[n] <i_p\u00e5>] <navn> til <farge>",
-                        "<endre> <omr\u00e5de>[s][ ]lys"
+                        "[<doe>|<zou>] <name>[ ][<lamp>][ ][kleur] [<naar>] {color} [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] [[de] kleur van] <name>[ ][<lamp>] [<naar>] {color} [[willen|kunnen] <doe>]"
                     ]
                 },
                 {
                     "response": "color",
                     "sentences": [
-                        "<endre> <farge> lys <i_p\u00e5> <omr\u00e5de>",
-                        "<endre> <omr\u00e5de>[s][ ]<lys> til <farge>"
+                        "[<doe>|<zou>] [[de] kleur van] [[<alle>] <lamp>] [in|van] <area>[[ ]<lamp>] [<naar>] {color} [[willen|kunnen] <doe>]"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 }
             ]
         }
     },
-    "language": "nb",
+    "language": "nl",
     "responses": {
         "intents": {
             "HassLightSet": {
-                "brightness": "{{ slots.name }} lysstyrken er satt til {{ slots.brightness }}",
-                "brightness_area": "Lysstyrken i {{ slots.area }} er satt til {{ slots.brightness }}",
-                "color": "{{ slots.name }} satt til {{ slots.color }} farge",
-                "color_area": "Fargen i {{ slots.area }} satt til {{ slots.color }}"
+                "brightness": "Helderheid aangepast",
+                "color": "Kleur aangepast"
             }
         }
     }
 }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ko.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7934027777777778%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {2: {'sentences': ['<area> 밝기를 <brightness>로 "*

 * *              "[<numeric_value_set>]', '<area>의 밝기를 <brightness>로 [<numeric_value_set>]', '<area>을 "*

 * *              "<brightness> 밝기로 [<numeric_value_set>]', '<area> <brightness>로 "*

 * *              "[<numeric_value_set>]'], 'slots': OrderedDict([('name', 'all')])}, 3: {'sentences': "*

 * *              "['<area> <brightness>로 <numeric_value_set>']}, 4: {'sentences': ['<name> 밝기 "*

 * *              "{brightness_level:brightness}[로] [ […]*

```diff
@@ -1,72 +1,103 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "brightness",
+                    "sentences": [
+                        "<name> \ubc1d\uae30 <brightness>[\ub85c] [<numeric_value_set>]",
+                        "<name>\uc758 \ubc1d\uae30 <brightness>[\ub85c] [<numeric_value_set>]",
+                        "<name> <brightness> \ubc1d\uae30[\ub85c] [<numeric_value_set>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
                     "response": "brightness",
                     "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<lamp>][ ][<helderheid>] [<naar>] <brightness> [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <helderheid> [van] <name>[ ][<lamp>] [<naar>] <brightness> [[willen|kunnen] <doe>]"
+                        "<name> <brightness>[\ub85c] <numeric_value_set>"
                     ]
                 },
                 {
                     "response": "brightness",
                     "sentences": [
-                        "[<doe>|<zou>] [<helderheid>] <in> <area>[[ ]<lamp>] [<naar>] <brightness> [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <area>[ ][<helderheid>|lamp] [<naar>] <brightness> [[willen|kunnen] <doe>]"
+                        "<area> \ubc1d\uae30\ub97c <brightness>\ub85c [<numeric_value_set>]",
+                        "<area>\uc758 \ubc1d\uae30\ub97c <brightness>\ub85c [<numeric_value_set>]",
+                        "<area>\uc744 <brightness> \ubc1d\uae30\ub85c [<numeric_value_set>]",
+                        "<area> <brightness>\ub85c [<numeric_value_set>]"
+                    ],
+                    "slots": {
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "brightness",
+                    "sentences": [
+                        "<area> <brightness>\ub85c <numeric_value_set>"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "brightness",
                     "sentences": [
-                        "[<doe>|<zou>] <name>[ ][lamp][ ][<helderheid>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <helderheid> [van] <name>[ ][<lamp>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <name>[ ][lamp] [<naar>] [de|het] {brightness_level:brightness} <helderheid> [[willen|kunnen] <doe>]"
+                        "<name> \ubc1d\uae30 {brightness_level:brightness}[\ub85c] [<numeric_value_set>]",
+                        "<name>\uc758 \ubc1d\uae30 {brightness_level:brightness}[\ub85c] [<numeric_value_set>]",
+                        "<name> {brightness_level:brightness} \ubc1d\uae30[\ub85c] [<numeric_value_set>]",
+                        "<name> {brightness_level:brightness}"
                     ]
                 },
                 {
                     "response": "brightness",
                     "sentences": [
-                        "[<doe>|<zou>] [<helderheid>] <in> <area> [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <area>[ ][<helderheid>] [<naar>] [het] {brightness_level:brightness} [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] <area> [<naar>] [de|het] {brightness_level:brightness} [<helderheid>] [[willen|kunnen] <doe>]"
+                        "<area> \ubc1d\uae30\ub97c [the] {brightness_level:brightness}[\ub85c] [<numeric_value_set>]",
+                        "<area>\uc758 \ubc1d\uae30\ub97c [the] {brightness_level:brightness}[\ub85c] [<numeric_value_set>]",
+                        "<area> {brightness_level:brightness} \ubc1d\uae30[\ub85c] [<numeric_value_set>]",
+                        "<area> \ubc1d\uae30 {brightness_level:brightness}[\ub85c] [<numeric_value_set>]",
+                        "<area> {brightness_level:brightness}"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
                     "response": "color",
                     "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<lamp>][ ][kleur] [<naar>] {color} [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [[de] kleur van] <name>[ ][<lamp>] [<naar>] {color} [[willen|kunnen] <doe>]"
+                        "<name> [\uc0c9\uc0c1] {color}[\ub85c|\uc73c\ub85c] [<set>]",
+                        "<name>\uc758 [\uc0c9\uc0c1] {color}[\ub85c|\uc73c\ub85c] [<set>]"
                     ]
                 },
                 {
                     "response": "color",
                     "sentences": [
-                        "[<doe>|<zou>] [[de] kleur van] [[<alle>] <lamp>] [in|van] <area>[[ ]<lamp>] [<naar>] {color} [[willen|kunnen] <doe>]"
+                        "(<area> | <area> \ubaa8\ub4e0 \uc870\uba85 | \ubaa8\ub4e0 <area> \uc870\uba85)\uc758 [\uc0c9\uc0c1] {color}[\ub85c|\uc73c\ub85c] [<set>]",
+                        "(<area> | <area> \ubaa8\ub4e0 \uc870\uba85 | \ubaa8\ub4e0 <area> \uc870\uba85) [\uc0c9\uc0c1]  {color}[\ub85c|\uc73c\ub85c] [<set>]"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 }
             ]
         }
     },
-    "language": "nl",
+    "language": "ko",
     "responses": {
         "intents": {
             "HassLightSet": {
-                "brightness": "Helderheid aangepast",
-                "color": "Kleur aangepast"
+                "brightness": "\ubc1d\uae30\uac00 \uc124\uc815\ub418\uc5c8\uc2b5\ub2c8\ub2e4",
+                "color": "\uc0c9\uc0c1\uc774 \uc124\uc815\ub418\uc5c8\uc2b5\ub2c8\ub2e4"
             }
         }
     }
 }
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents/domains.py` & `home-assistant-intents-2023.7.24/home_assistant_intents/domains.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,16 @@
         "cs",
         "da",
         "de",
         "de-CH",
         "el",
         "en",
         "es",
+        "et",
+        "eu",
         "fa",
         "fi",
         "fr",
         "fr-CA",
         "gl",
         "gu",
         "he",
@@ -62,14 +64,15 @@
         "cs",
         "da",
         "de",
         "de-CH",
         "el",
         "en",
         "es",
+        "eu",
         "fa",
         "fi",
         "fr",
         "fr-CA",
         "gl",
         "gu",
         "he",
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.6.5
+Version: 2023.7.24
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 home_assistant_intents/data/homeassistant/cs.json
 home_assistant_intents/data/homeassistant/da.json
 home_assistant_intents/data/homeassistant/de-CH.json
 home_assistant_intents/data/homeassistant/de.json
 home_assistant_intents/data/homeassistant/el.json
 home_assistant_intents/data/homeassistant/en.json
 home_assistant_intents/data/homeassistant/es.json
+home_assistant_intents/data/homeassistant/et.json
+home_assistant_intents/data/homeassistant/eu.json
 home_assistant_intents/data/homeassistant/fa.json
 home_assistant_intents/data/homeassistant/fi.json
 home_assistant_intents/data/homeassistant/fr-CA.json
 home_assistant_intents/data/homeassistant/fr.json
 home_assistant_intents/data/homeassistant/gl.json
 home_assistant_intents/data/homeassistant/gu.json
 home_assistant_intents/data/homeassistant/he.json
@@ -69,14 +71,15 @@
 home_assistant_intents/data/light/cs.json
 home_assistant_intents/data/light/da.json
 home_assistant_intents/data/light/de-CH.json
 home_assistant_intents/data/light/de.json
 home_assistant_intents/data/light/el.json
 home_assistant_intents/data/light/en.json
 home_assistant_intents/data/light/es.json
+home_assistant_intents/data/light/eu.json
 home_assistant_intents/data/light/fa.json
 home_assistant_intents/data/light/fi.json
 home_assistant_intents/data/light/fr-CA.json
 home_assistant_intents/data/light/fr.json
 home_assistant_intents/data/light/gl.json
 home_assistant_intents/data/light/gu.json
 home_assistant_intents/data/light/he.json
```

### Comparing `home-assistant-intents-2023.6.5/pyproject.toml` & `home-assistant-intents-2023.7.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.6.5"
+version     = "2023.7.24"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

