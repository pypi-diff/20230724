# Comparing `tmp/linuxnet-iptables-6.3.1.tar.gz` & `tmp/linuxnet-iptables-6.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-6.3.1.tar", last modified: Fri Jul 14 00:04:28 2023, max compression
+gzip compressed data, was "linuxnet-iptables-6.4.5.tar", last modified: Mon Jul 24 18:11:56 2023, max compression
```

## Comparing `linuxnet-iptables-6.3.1.tar` & `linuxnet-iptables-6.4.5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     3742 2023-07-13 23:59:57.000000 linuxnet-iptables-6.3.1/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-6.3.1/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3213 2023-07-12 15:09:37.000000 linuxnet-iptables-6.3.1/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.814235 linuxnet-iptables-6.3.1/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-6.3.1/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-6.3.1/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8110 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.817235 linuxnet-iptables-6.3.1/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/docs/matches/addrtypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1268 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-6.3.1/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1438 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2248 2023-07-13 23:47:22.000000 linuxnet-iptables-6.3.1/docs/matches/recentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2302 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-6.3.1/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.818235 linuxnet-iptables-6.3.1/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.818235 linuxnet-iptables-6.3.1/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.820236 linuxnet-iptables-6.3.1/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    27956 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1467 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.822236 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1376 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/addrtypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5113 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    16568 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7640 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7077 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     9287 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/recentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3049 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    11676 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     6190 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     8386 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    18505 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    29276 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.824236 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.824236 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2769 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-6.3.1/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    70348 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.806003 linuxnet-iptables-6.4.5/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-6.4.5/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     3975 2023-07-24 18:05:37.000000 linuxnet-iptables-6.4.5/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-6.4.5/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-6.4.5/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-24 18:11:56.806003 linuxnet-iptables-6.4.5/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3213 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.794002 linuxnet-iptables-6.4.5/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-6.4.5/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-6.4.5/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-6.4.5/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8110 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3307 2023-07-14 00:19:42.000000 linuxnet-iptables-6.4.5/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-6.4.5/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-6.4.5/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.796002 linuxnet-iptables-6.4.5/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-6.4.5/docs/matches/addrtypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1268 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-6.4.5/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1438 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-6.4.5/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2248 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/docs/matches/recentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2302 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-6.4.5/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-6.4.5/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-6.4.5/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.798003 linuxnet-iptables-6.4.5/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-6.4.5/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-6.4.5/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.798003 linuxnet-iptables-6.4.5/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.4.5/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.799003 linuxnet-iptables-6.4.5/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    29055 2023-07-24 17:58:13.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1467 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.802003 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1376 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/addrtypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5113 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    16568 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7640 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9623 2023-07-24 17:58:12.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    11610 2023-07-24 17:58:12.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/recentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3049 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    11676 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 21:05:25.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     6190 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-07-24 17:58:12.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     8386 2023-07-14 00:05:40.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    19140 2023-07-24 17:58:12.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29318 2023-07-24 17:58:12.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.804003 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-6.4.5/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.805003 linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-24 18:11:56.000000 linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2769 2023-07-24 18:11:56.000000 linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-07-24 18:11:56.000000 linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-07-24 18:11:56.000000 linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-07-24 18:11:56.806003 linuxnet-iptables-6.4.5/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-6.4.5/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-24 18:11:56.805003 linuxnet-iptables-6.4.5/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.4.5/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    72355 2023-07-24 17:58:13.000000 linuxnet-iptables-6.4.5/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-6.3.1/.pylintrc` & `linuxnet-iptables-6.4.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/CHANGELOG.md` & `linuxnet-iptables-6.4.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 ==========
 
+6.4.5 (2023-07-24)
+------------------
+
+- RecentMatch now supports the --mask and --reap options
+- ProtocolCriterion now also accepts protocols specified as numbers
+- Chain class now supports special methods __len__ and __getitem__
+
+
 6.3.1 (2023-07-13)
 ------------------
 
 - added RecentMatch class
 - added ChainRule.iter_matches()
 - added GenericPositiveCriterion class for criteria that do
   not support inequality comparisons
```

### Comparing `linuxnet-iptables-6.3.1/LICENSE` & `linuxnet-iptables-6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/Makefile` & `linuxnet-iptables-6.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/PKG-INFO` & `linuxnet-iptables-6.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 6.3.1
+Version: 6.4.5
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-6.3.1/README.md` & `linuxnet-iptables-6.4.5/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/Makefile` & `linuxnet-iptables-6.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/chain.rst` & `linuxnet-iptables-6.4.5/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/conf.py` & `linuxnet-iptables-6.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/exception.rst` & `linuxnet-iptables-6.4.5/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/extensibility.rst` & `linuxnet-iptables-6.4.5/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/index.rst` & `linuxnet-iptables-6.4.5/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 will probably be different on your system)::
 
     >>> from linuxnet.iptables import IptablesPacketFilterTable
     >>> table = IptablesPacketFilterTable('filter')
     >>> table.read_system_config()
     True
     >>> input_chain = table.get_chain('INPUT')
-    >>> for rule in input_chain.get_rules():
+    >>> for rule in input_chain:
     ...    print(' '.join(rule.to_iptables_args()))
     ...
     -j prod_bad_traffic
     -m state --state RELATED,ESTABLISHED -j ACCEPT
     -j prod_ingress
     -j prod_lsvc
     -j prod_INPUT_ldrop
```

### Comparing `linuxnet-iptables-6.3.1/docs/iptables_api.rst` & `linuxnet-iptables-6.4.5/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/match-example.py` & `linuxnet-iptables-6.4.5/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/match.rst` & `linuxnet-iptables-6.4.5/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/addrtypematch.rst` & `linuxnet-iptables-6.4.5/docs/matches/addrtypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/commentmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/icmpmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/limitmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/markmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/ownermatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/packetmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/packettypematch.rst` & `linuxnet-iptables-6.4.5/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/recentmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/recentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/statematch.rst` & `linuxnet-iptables-6.4.5/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/tcpmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/tcpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/ttlmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/matches/udpmatch.rst` & `linuxnet-iptables-6.4.5/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/rule.rst` & `linuxnet-iptables-6.4.5/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/table.rst` & `linuxnet-iptables-6.4.5/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/target-example.py` & `linuxnet-iptables-6.4.5/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/target.rst` & `linuxnet-iptables-6.4.5/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/chaintarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/connmarktarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/dnattarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/logtarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/marktarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/notracktarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/notracktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/rejecttarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/snattarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/tracetarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/docs/targets/ttltarget.rst` & `linuxnet-iptables-6.4.5/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/__init__.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/chain.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,25 @@
 # pylint: disable=too-many-instance-attributes,too-many-public-methods
 
 class Chain:
     """This class is used to represent an iptables chain.
     A chain contains a list of rules which can be referenced by
     number (rule numbers start with 1).
 
-    A :class:`Chain` object is iterable, returning the chain's rules.
+    A :class:`Chain` instance is iterable, returning the chain's rules.
+
+    The :class:`Chain` class supports the standard :func:`len` function
+    returning the number of rules in the chain.
+
+    The :class:`Chain` class supports integer-based indexing
+    (slices are not supported). Positive integers are interpreteted
+    as rule numbers, i.e. indexing starts at ``1``.
+    Index ``0`` will raise an :exc:`IndexError`.
+    Negative index values are supported with ``-1`` identifying the last rule,
+    ``-2`` identifying the penultimate rule, etc.
     """
 
     def __init__(self, chain_name: str):
         """
         :param chain_name: real chain name
         """
         self.__real_chain_name = chain_name
@@ -49,26 +59,40 @@
         self.__byte_count = 0
         self.__rule_list = []
         self.__pft = None
 
     def __str__(self):
         return f'Chain({self.__real_chain_name})'
 
+    def __len__(self):
+        return len(self.__rule_list)
+
+    def __getitem__(self, rulenum):
+        if not isinstance(rulenum, int):
+            raise TypeError("only integer-based indexing supported")
+        if rulenum > 0:
+            return self.__rule_list[rulenum-1]
+        if rulenum == 0:
+            raise IndexError(f"bad rule number: {rulenum}")
+        return self.__rule_list[rulenum]
+
     def __iter__(self):
         """Iterator for the chain's rules
         """
         return iter(self.__rule_list)
 
     def is_builtin(self) -> bool:       # pylint: disable=no-self-use
         """Returns ``True`` if this is a built-in chain (e.g. ``INPUT``)
         """
         return False
 
     def has_rules(self) -> bool:
-        """Returns ``True`` if the chain contains any rules
+        """Returns ``True`` if the chain contains any rules (note that
+        a :class:`Chain` instance can also be used directly in a boolean
+        content; if empty, it evaluates to ``False``).
         """
         return bool(self.__rule_list)
 
     def get_reference_count(self) -> int:
         """Returns the reference count of a (non-builtin) chain; returns 0
         for builtin chains
         """
@@ -110,15 +134,16 @@
         count = 0
         for rule in self.__rule_list:
             if rule.parsing_failed():
                 count += 1
         return count
 
     def get_rule_count(self) -> int:
-        """Returns the number of rules in the chain
+        """Returns the number of rules in the chain (note that the
+        standard :func:`len` function is also supported)
         """
         return len(self.__rule_list)
 
     def get_rules(self) -> List[ChainRule]:
         """Returns a list that contains the chain rules.
         """
         return self.__rule_list[:]
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/deps.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/extension.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/addrtypematch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/addrtypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/match.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/packetmatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 """
 This module provides the PacketMatch class which supports
 matching against standard packet attributes
 """
 
 from ipaddress import IPv4Network
-from typing import Iterable, Optional
+from typing import Iterable, List, Optional
 
-from ..exceptions import IptablesParsingError
+from ..exceptions import IptablesError, IptablesParsingError
 from ..deps import get_logger
 
-from .match import Match, MatchParser
+from .match import Criterion, Match, MatchParser
 from .util import BooleanCriterion, GenericCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.packetmatch')
 
 
 class InputInterfaceCriterion(GenericCriterion):
     """Compare with the input interface.
@@ -64,21 +64,88 @@
 
     The comparison value is an :class:`IPv4Network`.
     """
     def __init__(self, match: Match):
         super().__init__(match, '-d')
 
 
-class ProtocolCriterion(GenericCriterion):
+class ProtocolCriterion(Criterion):
     """Compare with the protocol.
 
     The comparison value is a protocol name (a string).
     """
-    def __init__(self, match: Match):
-        super().__init__(match, '-p')
+
+    # Key: protocol number
+    # Value: protocol name
+    __proto_map = {}
+    __proto_map_ready = False
+
+    def __init__(self, match: Match):
+        super().__init__(match)
+        self.__proto_name = None
+
+    @classmethod
+    def __getprotobynumber(cls, protonum: int) -> Optional[str]:
+        """Returns the protocol name for the specified protocol
+        """
+        if cls.__proto_map_ready:
+            return cls.__proto_map.get(protonum)
+        try:
+            with open("/etc/protocols", encoding="utf-8") as protofile:
+                for line in protofile:
+                    pos = line.find('#')
+                    if pos < 0:
+                        line = line.strip()
+                    else:
+                        line = line[:pos].strip()
+                    if not line:
+                        continue
+                    fields = line.split()
+                    if len(fields) < 2:
+                        continue
+                    try:
+                        cls.__proto_map[int(fields[1])] = fields[0]
+                    except ValueError:
+                        pass
+        except Exception:               # pylint: disable=broad-except
+            _logger.exception("unable to process /etc/protocols")
+        finally:
+            cls.__proto_map_ready = True
+        return cls.__proto_map.get(protonum)
+
+    def get_value(self) -> str:
+        """Return protocol name
+        """
+        return self.__proto_name
+
+    def equals(self, proto) -> Match:   # pylint: disable=arguments-differ
+        """Compare with the specified protocol.
+
+        :param proto: the parameter can a string or an integer; if it
+            is an integer, it will be converted to the corresponding
+            protocol name, if possible, otherwise it will be used as-is
+            in string form (i.e. 199 will be converted to "199")
+        """
+        if isinstance(proto, str):
+            # Check if is a number in string form
+            try:
+                self.__proto_name = self.__getprotobynumber(int(proto)) or proto
+            except ValueError:
+                self.__proto_name = proto
+        elif isinstance(proto, int):
+            self.__proto_name = self.__getprotobynumber(int(proto)) or \
+                                                str(proto)
+        else:
+            raise IptablesError(f'unexpected argument type: {proto}')
+        return self._set_polarity(True)
+
+    def _crit_iptables_args(self) -> List[str]:
+        """Returns **iptables(8)** arguments for the specified protocol
+        """
+        return ['-p', self.__proto_name]
 
 
 class FragmentCriterion(BooleanCriterion):
     """Check if a packet is a fragment.
     """
 
     def __init__(self, match: Match):
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/recentmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/recentmatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides access to the ``recent`` match
 """
 
 from enum import Enum
-from typing import Iterable, List
+from ipaddress import IPv4Address
+from typing import Iterable, List, Optional
 
 from ..deps import get_logger
 from ..exceptions import IptablesError, IptablesParsingError
 
 from .match import Criterion, Match, MatchParser
 from .util import GenericPositiveCriterion, BooleanCriterion
 
@@ -56,14 +57,20 @@
     def get_value(self) -> RecentMatchAction:
         """Returns the action
         """
         return self.__action
 
     def equals(self,                    # pylint: disable=arguments-differ
                 action: RecentMatchAction, *, match_if_found=True):
+        """
+        :param action: identifies the action to take
+        :param match_if_found: if ``False``, when the packet address
+            is present in the identified list, the ``recent`` match will
+            cause the rule to **fail** to match the packet
+        """
         self.__action = action
         return self._set_polarity(match_if_found)
 
     def not_equals(self, *args, **kwargs):
         """This criterion does not support inequality testing.
         This method will raise an :exc:`IptablesError`
         """
@@ -111,14 +118,51 @@
         """Returns **iptables(8)** arguments for the specified selection.
         """
         if self.__selection is not None:
             return [self.__selection.value]
         return []
 
 
+class MaskCriterion(Criterion):
+    """Apply the specified mask.
+
+    The value is an :class:`IPv4Address`.
+    """
+
+    SKIP_MASK = IPv4Address('255.255.255.255')
+
+    def __init__(self, match: Match):
+        super().__init__(match)
+        self.__mask = None
+
+    def get_value(self) -> Optional[IPv4Address]:
+        """Returns the mask
+        """
+        return self.__mask
+
+    def equals(self, mask) -> Match:    # pylint: disable=arguments-differ
+        """Use the specified source mask
+        """
+        self.__mask = mask
+        self._set_polarity(True)
+
+    def not_equals(self, *args, **kwargs):
+        """This :class:`Criterion` method is not supported
+        """
+        raise IptablesError('method not_equals() not supported')
+
+    def _crit_iptables_args(self) -> List[str]:
+        """Returns **iptables(8)** arguments for the specified rate
+        """
+        if self.__mask == self.SKIP_MASK:
+            return []
+        return ['--mask', str(self.__mask)]
+
+
+
 class RecentMatch(Match):
     """Match against list of IP addresses.
     """
 
     #: SET action
     SET = RecentMatchAction.SET
     #: UPDATE action
@@ -136,14 +180,16 @@
     def __init__(self):
         self.__action_crit = None
         self.__name_crit = None
         self.__seconds_crit = None
         self.__hitcount_crit = None
         self.__same_ttl_crit = None
         self.__address_selection_crit = None
+        self.__reap_crit = None
+        self.__mask_crit = None
 
     @staticmethod
     def get_match_name() -> str:
         """Returns the **iptables(8)** match extension name
         """
         return 'recent'
 
@@ -152,16 +198,22 @@
         """
         # We create a temporary AddressSelectionCriterion with
         # the default match behavior.
         address_selection_crit = self.__address_selection_crit
         if address_selection_crit is None:
             address_selection_crit = AddressSelectionCriterion(self)
             address_selection_crit.equals(self.SOURCE_ADDRESS)
+        # We create a temporary MaskCritetion with the default mask
+        mask_crit = self.__mask_crit
+        if mask_crit is None:
+            mask_crit = MaskCriterion(self)
+            mask_crit.equals(MaskCriterion.SKIP_MASK)
         return (self.__action_crit, self.__name_crit, self.__seconds_crit,
-            self.__hitcount_crit, self.__same_ttl_crit, address_selection_crit)
+            self.__hitcount_crit, self.__same_ttl_crit, address_selection_crit,
+            self.__reap_crit, mask_crit)
 
     def name(self) -> GenericPositiveCriterion:
         """Identify the list name
         """
         if self.__name_crit is None:
             self.__name_crit = GenericPositiveCriterion(self, '--name')
         return self.__name_crit
@@ -198,14 +250,29 @@
         """Specify same-TTL comparison.
         """
         if self.__same_ttl_crit is None:
             self.__same_ttl_crit = BooleanCriterion(self, "--rttl",
                                                 supports_negation=False)
         return self.__same_ttl_crit
 
+    def reap(self) -> BooleanCriterion:
+        """Specify old address reaping
+        """
+        if self.__reap_crit is None:
+            self.__reap_crit = BooleanCriterion(self, "--reap",
+                                                supports_negation=False)
+        return self.__reap_crit
+
+    def mask(self) -> MaskCriterion:
+        """Specify a source mask
+        """
+        if self.__mask_crit is None:
+            self.__mask_crit = MaskCriterion(self)
+        return self.__mask_crit
+
     # pylint: disable=too-many-branches
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Possible output::
 
         recent: CHECK TTL-Match name: foobar side: source LOG flags 0 level 4
         !recent: SET name: foobar side: source LOG flags 0 level 4
@@ -251,14 +318,18 @@
                 if address_selection == 'source':
                     match.address_selection().equals(cls.SOURCE_ADDRESS)
                 elif address_selection.startswith('dest'):
                     match.address_selection().equals(cls.DEST_ADDRESS)
                     rest = address_selection[4:]
                     if rest:
                         criteria_iter.put_back(rest, replace_token=True)
+            elif val == 'reap':
+                match.reap().equals()
+            elif val == 'mask:':
+                match.mask().equals(IPv4Address(next(criteria_iter)))
             else:
                 criteria_iter.put_back(val)
                 break
         return match
     # pylint: enable=too-many-branches
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/statematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/tcpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/matches/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/metadata.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "6.3.1"
+_version_ = "6.4.5"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/parsing.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/rule.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,36 +43,47 @@
     However, there can be at most one :class:`PacketMatch` object included.
 
     A :class:`ChainRule` object is iterable, returning the rule's
     :class:`Match` instances.
     """
 
     def __init__(self, *,
-                match:Optional[Match] =None,
-                match_list:Optional[List[Match]] =None,
-                target:Optional[Target] =None,
-                uses_goto:Optional[bool] =False):
+                match: Optional[Match] =None,
+                match_list: Optional[List[Match]] =None,
+                target: Optional[Target] =None,
+                uses_goto: Optional[bool] =False,
+                goto_chain: Optional['Chain'] = None):
         """
         :param match: optional :class:`Match` object; if present, it is added
             to the rule's list of :class:`Match` objects
         :param match_list: optional list of :class:`Match` objects;
             if present, it is appended to the rule's list of :class:`Match`
             objects
-        :param target: a :class:`Target` object
+        :param target: a :class:`Target` object; either this parameter or
+            the ``goto_chain`` parameter may be specified
         :param uses_goto:  if ``True``, rule processing continues at the
             specified target (which **must** be a :class:`ChainTarget`)
             short-circuiting any rules following this one in the chain
+        :param goto_chain: an optional :class:`Chain` object that is
+            the target of this rule via a ``goto`` (instead of ``jump``);
+            either this parameter or the ``target`` parameter may be
+            specified
         """
+        if goto_chain is not None and target is not None:
+            raise IptablesError('both target and goto chain specified')
         self.__match_list = []
         if match is not None:
             self.__match_list.append(match)
         if match_list:
             self.__match_list += match_list
         self.__target = target
         self.__uses_goto = uses_goto
+        if goto_chain is not None:
+            self.__target = ChainTarget(chain=goto_chain)
+            self.__uses_goto = True
         self.__packet_count = 0
         self.__byte_count = 0
         self.__owner_chain = None
         self.__rulenum = 0
         # __iptables_line is not None if this rule is created from
         # iptables(8) output
         self.__iptables_line = None
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/table.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,16 +266,18 @@
 
     def get_chain_by_rcn(self, real_chain_name: str) -> Optional[Chain]:
         """Returns the :class:`Chain` object with the specified name
         or ``None`` if there is no such chain
 
         :param real_chain_name: real chain name
         """
-        return (self.__chain_map.get(real_chain_name) or
-                        self.__other_chain_map.get(real_chain_name))
+        chain = self.__chain_map.get(real_chain_name)
+        if chain is not None:
+            return chain
+        return self.__other_chain_map.get(real_chain_name)
 
     def get_chain_by_lcn_prefix(self, prefix: str) -> List[Chain]:
         """Returns a list of :class:`Chain` objects whose logical name
         starts with the specified prefix.
 
         :param prefix: prefix of logical chain name
         """
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/notracktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/tracetarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/tracetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-6.4.5/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 6.3.1
+Version: 6.4.5
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-6.4.5/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/setup.py` & `linuxnet-iptables-6.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.3.1/tests/iptables_test.py` & `linuxnet-iptables-6.4.5/tests/iptables_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """Unit-test code for linuxnet.iptables
 """
 
+# pylint: disable=line-too-long, too-many-lines, wrong-import-position
+
 import logging
 import os
 import subprocess
 import unittest
 import sys
 
 from collections import namedtuple
@@ -74,17 +76,21 @@
     def __init__(self, exitcode, output):
         self.__output = output
         self.__exitcode = exitcode
         # A run is a list of ExecutedCommand instances
         self.__run = []
 
     def get_run(self):
+        """Retuns the run list
+        """
         return self.__run
 
     def clear_run(self):
+        """Clear the run list
+        """
         self.__run.clear()
 
     def __call__(self, cmd, *args, **kwargs):
         self.__run.append(ExecutedCommand(cmd, args, kwargs))
         proc = subprocess.CompletedProcess(args, self.__exitcode)
         proc.stdout = self.__output
         return proc
@@ -95,31 +101,31 @@
 
     This class contains generic tests; match-specific
     or target-specific tests have their own class below.
     """
 
     EMPTY_FORWARD = """\
 Chain FORWARD (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_OUTPUT = """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_PREROUTING = """\
 Chain PREROUTING (policy ACCEPT 429581 packets, 46536920 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_POSTROUTING = """\
 Chain POSTROUTING (policy ACCEPT 26246841 packets, 13324987010 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_INPUT = """\
 Chain INPUT (policy ACCEPT 28770515 packets, 54867569862 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
 
     def test_parsing_goto(self):
         """Parse output with goto
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
@@ -180,64 +186,82 @@
 
 class TestMatchParsing(unittest.TestCase):
     """Test parsing of matches in iptables output
     """
 
     EMPTY_FORWARD = """\
 Chain FORWARD (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_OUTPUT = """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_PREROUTING = """\
 Chain PREROUTING (policy ACCEPT 429581 packets, 46536920 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_POSTROUTING = """\
 Chain POSTROUTING (policy ACCEPT 26246841 packets, 13324987010 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_INPUT = """\
 Chain INPUT (policy ACCEPT 28770515 packets, 54867569862 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
 
     def test_parsing_packet_match(self):
         """Parse output with packet match (protocol, fragment,
         source addr, dest addr).
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
        0        0 DROP         all  -f  *      *       127.0.0.0/8          0.0.0.0/0
-      29     9862 ACCEPT     udp  --  *      *       0.0.0.0/0            10.10.0.0/16
+       0        0 DROP         2    --  *      *       0.0.0.0/0            0.0.0.0/0
+      29     9862 ACCEPT       udp  --  *      *       0.0.0.0/0              10.10.0.0/16
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        self.assertEqual(input_chain.get_rule_count(), 2)
+        self.assertEqual(input_chain.get_rule_count(), 3)
         for rule in input_chain:
             if rule.get_rulenum() == 1:
                 self.assertEqual(rule.get_match_count(), 1)
                 match = next(iter(rule))
                 self.assertTrue(match.fragment().is_positive())
                 src = match.source_address()
                 self.assertTrue(src.is_positive() and
                     src.get_value() == IPv4Network('127.0.0.0/8'))
             elif rule.get_rulenum() == 2:
                 self.assertEqual(rule.get_match_count(), 1)
                 match = next(iter(rule))
                 prot = match.protocol()
                 self.assertTrue(prot.is_positive() and
+                    prot.get_value() == 'igmp')
+            elif rule.get_rulenum() == 3:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                prot = match.protocol()
+                self.assertTrue(prot.is_positive() and
                     prot.get_value() == 'udp')
                 dest = match.dest_address()
                 self.assertTrue(dest.is_positive() and
                     dest.get_value() == IPv4Network('10.10.0.0/16'))
+        #
+        # Test protocol comparison by number, number-in-string-form,
+        # and protocol name, where the protocol name is reported by iptables
+        # as a number. We use IGMP (protocol number 2) for this.
+        #
+        rule = next(input_chain.iter_rules(match=PacketMatch().protocol().equals(2)), None)
+        self.assertTrue(rule is not None and
+                        next(iter(rule)).protocol().get_value() == 'igmp')
+        rule = next(input_chain.iter_rules(match=PacketMatch().protocol().equals("2")), None)
+        self.assertTrue(rule is not None and
+                        next(iter(rule)).protocol().get_value() == 'igmp')
 
     def test_parsing_packet_type_match(self):
         """Parse output with packet type match
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
@@ -385,19 +409,20 @@
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: CHECK TTL-Match name: foobar side: source LOG flags 0 level 4
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           !recent: SET name: foobar side: source LOG flags 0 level 4
        0        0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: REMOVE name: foobar side: destMARK set 0xa
        0        0            all  --  *      *       0.0.0.0/0            0.0.0.0/0           !recent: UPDATE seconds: 4 hit_count: 3 name: foobar side: source
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: REMOVE name: foobar side: dest/* silly */ LOG flags 0 level 4
+       0        0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: SET name: OUTPUT side: source mask: 255.255.255.255
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        self.assertEqual(input_chain.get_rule_count(), 5)
+        self.assertEqual(input_chain.get_rule_count(), 6)
         for rule in input_chain:
             rulenum = rule.get_rulenum()
             if rulenum == 1:
                 match = next(iter(rule))
                 self.assertTrue(isinstance(match, RecentMatch))
                 action = match.action()
                 self.assertTrue(action.is_positive() and
@@ -447,27 +472,32 @@
                 match = match_list[0]
                 self.assertTrue(isinstance(match, RecentMatch))
                 action = match.action()
                 self.assertTrue(action.is_positive() and
                     action.get_value() == RecentMatch.REMOVE)
                 self.assertTrue(match.name().get_value() == 'foobar')
                 self.assertTrue(isinstance(match_list[1], CommentMatch))
+            elif rulenum == 6:
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, RecentMatch))
+                self.assertEqual(match.mask().get_value(),
+                                        IPv4Address('255.255.255.255'))
 
     def test_parsing_owner_match(self):
         """Parse output with match related to UID/GID
         """
         output = self.EMPTY_INPUT + '\n' + self.EMPTY_FORWARD + '\n' + \
 """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner UID match 100
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           ! owner GID match 100
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner UID match 100-300 ! owner UID match 200
-       8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner socket exists 
-       8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner GID match 100 ! owner socket exists 
+       8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner socket exists
+       8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner GID match 100 ! owner socket exists
 """
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         output_chain = pft.get_builtin_chain('OUTPUT')
         self.assertEqual(output_chain.get_rule_count(), 5)
         for rule in output_chain:
             if rule.get_rulenum() == 1:
@@ -515,15 +545,15 @@
 
     def test_parsing_connmark_match(self):
         """Parse output with connmark match
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
-  558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK set 0x11 
+  558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK set 0x11
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('PREROUTING')
         self.assertEqual(input_chain.get_rule_count(), 1)
         rule = next(iter(input_chain))
@@ -556,18 +586,18 @@
                 burst.get_value() == 5)
 
     def test_parsing_comment_match(self):
         """Parse output with comment matches
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-       0        0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* my comment */ 
-       0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW reject-with icmp-port-unreachable 
-       0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW /* foo bar */ reject-with icmp-port-unreachable 
+    pkts      bytes target     prot opt in     out     source               destination
+       0        0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* my comment */
+       0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW reject-with icmp-port-unreachable
+       0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW /* foo bar */ reject-with icmp-port-unreachable
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
         for rule in input_chain:
             rulenum = rule.get_rulenum()
             if rulenum == 1:
@@ -644,46 +674,46 @@
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
 196245663 314408786102 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_INPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
     0     0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           DSCP match 0x10
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         init_ok = pft.init_from_output(output, log_parsing_failures=False)
         self.assertFalse(init_ok, 'failed bad output')
 
 
 
 class TestTargetParsing(unittest.TestCase):
     """Test parsing of targets in iptables output
     """
 
     EMPTY_FORWARD = """\
 Chain FORWARD (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_OUTPUT = """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_PREROUTING = """\
 Chain PREROUTING (policy ACCEPT 429581 packets, 46536920 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_POSTROUTING = """\
 Chain POSTROUTING (policy ACCEPT 26246841 packets, 13324987010 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
     EMPTY_INPUT = """\
 Chain INPUT (policy ACCEPT 28770515 packets, 54867569862 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 """
 
     def test_parsing_log_target(self):
         """Parse output with LOG target
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
@@ -723,19 +753,19 @@
 
     def test_parsing_mark_target(self):
         """Parse output with MARK target
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
-    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK set 0xf 
-    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK xset 0x11/0xffff0011 
-    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK xor 0xf 
-    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK or 0xf 
-    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK and 0xff 
+    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK set 0xf
+    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK xset 0x11/0xffff0011
+    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK xor 0xf
+    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK or 0xf
+    0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK and 0xff
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
         for rule in input_chain:
             rulenum = rule.get_rulenum()
             if rulenum == 1:
@@ -772,15 +802,15 @@
 
     def test_parsing_connmark_target(self):
         """Parse output with CONNMARK target
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
-  558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK set 0x11 
+  558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK set 0x11
   558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK save nfmask 0xfffff ctmask ~0x1f
   558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK restore ctmask 0x1f nfmask ~0xfffff
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         prerouting_chain = pft.get_builtin_chain('PREROUTING')
@@ -806,17 +836,17 @@
 
     def test_parsing_ttl_target(self):
         """Parse output with TTL target
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
-       0        0 TTL        all  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL set to 10 
-       0        0 TTL        tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL increment by 1 
-       0        0 TTL        udp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL decrement by 2 
+       0        0 TTL        all  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL set to 10
+       0        0 TTL        tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL increment by 1
+       0        0 TTL        udp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL decrement by 2
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         prerouting_chain = pft.get_builtin_chain('PREROUTING')
         for rule in prerouting_chain:
             rulenum = rule.get_rulenum()
@@ -833,35 +863,35 @@
                                 target.get_ttl_dec() == 2)
 
     def test_parsing_snat_target(self):
         """Parse output with SNAT target
         """
         output = (self.EMPTY_PREROUTING + '\n' + """\
 Chain POSTROUTING (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
-  466007 51946882 SNAT       all  --  *      eth1    0.0.0.0/0            0.0.0.0/0           to:10.10.10.18 
+    pkts      bytes target     prot opt in     out     source               destination
+  466007 51946882 SNAT       all  --  *      eth1    0.0.0.0/0            0.0.0.0/0           to:10.10.10.18
 """ + '\n' + self.EMPTY_OUTPUT)
         pft = IptablesPacketFilterTable('nat')
         self.assertTrue(pft.init_from_output(output))
         postrouting_chain = pft.get_builtin_chain('POSTROUTING')
         rule = next(iter(postrouting_chain))
         target = rule.get_target()
         self.assertEqual(target.get_target_name(), 'SNAT')
         self.assertEqual(target.get_address(), IPv4Address('10.10.10.18'))
 
     def test_parsing_masquerade_target(self):
         """Parse output with MASQUERADE target
         """
         output = (self.EMPTY_PREROUTING + '\n' + """\
 Chain POSTROUTING (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
-       0        0 MASQUERADE  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
-       0        0 MASQUERADE  all  --  *      *       0.0.0.0/0            0.0.0.0/0           random 
-       0        0 MASQUERADE  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           masq ports: 2000 
-       0        0 MASQUERADE  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp spts:1000:2000 masq ports: 2000 random 
+    pkts      bytes target     prot opt in     out     source               destination
+       0        0 MASQUERADE  all  --  *      *       0.0.0.0/0            0.0.0.0/0
+       0        0 MASQUERADE  all  --  *      *       0.0.0.0/0            0.0.0.0/0           random
+       0        0 MASQUERADE  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           masq ports: 2000
+       0        0 MASQUERADE  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp spts:1000:2000 masq ports: 2000 random
        0        0 MASQUERADE  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp spts:1000:2000 masq ports: 20000-30000
 """ + '\n' + self.EMPTY_OUTPUT)
         pft = IptablesPacketFilterTable('nat')
         self.assertTrue(pft.init_from_output(output))
         postrouting_chain = pft.get_builtin_chain('POSTROUTING')
         self.assertEqual(postrouting_chain.get_rule_count(), 5)
         for rule in postrouting_chain:
@@ -918,15 +948,15 @@
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
 196245663 314408786102 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_INPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
     0     0 AUDIT      all  --  *      *       1.2.3.4              0.0.0.0/0           AUDIT accept
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         init_ok = pft.init_from_output(output, log_parsing_failures=False)
         self.assertFalse(init_ok, 'failed bad output')
 
 
@@ -963,35 +993,35 @@
 
 class TestPrefix(unittest.TestCase):
     """Test chain prefix handling
     """
 
     GOOD_OUTPUT = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-129651288 230406442471 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+129651288 230406442471 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain FORWARD (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-378613942 278529707859 prod_FORWARD  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+378613942 278529707859 prod_FORWARD  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-62441650 9685307040 prod_OUTPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+62441650 9685307040 prod_OUTPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_FORWARD (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 377452936 278361749795 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_INPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 128158511 230312235930 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_OUTPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 55238105 5261597979 ACCEPT  all  --  *      eth1    0.0.0.0/0            0.0.0.0/0
 """
 
     def test_creating_table_using_prefix(self):
         """Parse valid output with no errors when a prefix is specified
         """
         prefix = 'prod_'
@@ -1025,35 +1055,35 @@
 
 class TestMiscellaneous(unittest.TestCase):
     """Test miscellaneous operations
     """
 
     GOOD_OUTPUT = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-129651288 230406442471 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+129651288 230406442471 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain FORWARD (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-378613942 278529707859 prod_FORWARD  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+378613942 278529707859 prod_FORWARD  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
-    pkts      bytes target     prot opt in     out     source               destination         
-62441650 9685307040 prod_OUTPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0           
+    pkts      bytes target     prot opt in     out     source               destination
+62441650 9685307040 prod_OUTPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_FORWARD (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 377452936 278361749795 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_INPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 128158511 230312235930 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain prod_OUTPUT (1 references)
-    pkts      bytes target     prot opt in     out     source               destination         
+    pkts      bytes target     prot opt in     out     source               destination
 55238105 5261597979 ACCEPT  all  --  *      eth1    0.0.0.0/0            0.0.0.0/0
 """
 
     def test_epoch(self):
         """Check that the epoch is initialized properly
         """
         pft = IptablesPacketFilterTable('filter')
@@ -1102,15 +1132,15 @@
         output = """\
 Chain INPUT (policy DROP 10 packets, 500 bytes)
     pkts      bytes target     prot opt in     out     source               destination
     500       50000 fw_INPUT   all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain fw_INPUT (1 references)
     pkts      bytes target     prot opt in     out     source               destination
-    400       40000 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           state RELATED,ESTABLISHED 
+    400       40000 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           state RELATED,ESTABLISHED
     100       10000 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0
 
 Chain FORWARD (policy DROP 20 packets, 2000 bytes)
     pkts      bytes target     prot opt in     out     source               destination
 
 Chain OUTPUT (policy ACCEPT 30 packets, 3000 bytes)
     pkts      bytes target     prot opt in     out     source               destination
@@ -1468,10 +1498,31 @@
             rule = ChainRule(target=Targets.ACCEPT)
             chain.insert_rule(rule, rulenum=1)
             rule_list.append(rule)
         for i in range(4):
             expected_num = 4-i
             self.assertEqual(rule_list[i].get_rulenum(), expected_num)
 
+    def test_chain_rule_indexing(self):
+        """Verify chain rule indexing
+        """
+        pft = IptablesPacketFilterTable('filter', runner=self._runner)
+        chain = pft.create_chain('test_chain')
+        rule_list = []
+        # Always inserting as rule #1 forces previously inserted
+        # rules to be renumbered.
+        for i in range(4):
+            rule = ChainRule(target=Targets.ACCEPT)
+            chain.insert_rule(rule, rulenum=1)
+            rule_list.append(rule)
+        self.assertEqual(len(chain), 4)
+        for rule in chain:
+            self.assertTrue(rule is chain[rule.get_rulenum()])
+        num_rules = len(chain)
+        for i in range(num_rules):
+            rule = chain[i-num_rules]
+            self.assertEqual(rule.get_rulenum(), i+1)
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

