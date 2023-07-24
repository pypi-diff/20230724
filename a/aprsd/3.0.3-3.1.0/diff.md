# Comparing `tmp/aprsd-3.0.3.tar.gz` & `tmp/aprsd-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-3.0.3.tar", last modified: Tue Apr 25 18:44:13 2023, max compression
+gzip compressed data, was "aprsd-3.1.0.tar", last modified: Mon Jul 24 15:27:34 2023, max compression
```

## Comparing `aprsd-3.0.3.tar` & `aprsd-3.1.0.tar`

### file list

```diff
@@ -1,229 +1,234 @@
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.399247 aprsd-3.0.3/
--rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.0.3/.coveragerc
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.309467 aprsd-3.0.3/.github/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.448006 aprsd-3.0.3/.github/workflows/
--rw-r--r--   0 i530566    (501) staff       (20)     1624 2022-12-16 13:25:52.000000 aprsd-3.0.3/.github/workflows/master-build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      526 2022-11-23 18:33:33.000000 aprsd-3.0.3/.github/workflows/python.yml
--rw-r--r--   0 i530566    (501) staff       (20)     1283 2022-12-16 13:25:52.000000 aprsd-3.0.3/.github/workflows/release_build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.0.3/.pre-commit-config.yaml
--rw-r--r--   0 i530566    (501) staff       (20)      397 2023-04-25 18:43:57.000000 aprsd-3.0.3/AUTHORS
--rw-r--r--   0 i530566    (501) staff       (20)    20802 2023-04-25 18:43:56.000000 aprsd-3.0.3/ChangeLog
--rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.0.3/INSTALL.txt
--rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.0.3/LICENSE
--rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.0.3/MANIFEST.in
--rw-r--r--   0 i530566    (501) staff       (20)     2730 2022-12-29 19:14:43.000000 aprsd-3.0.3/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-04-25 18:44:13.399639 aprsd-3.0.3/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)    20002 2022-12-29 19:14:43.000000 aprsd-3.0.3/README.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.479151 aprsd-3.0.3/aprsd/
--rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     4566 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/aprsd.py
--rw-r--r--   0 i530566    (501) staff       (20)     3212 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/cli_helper.py
--rw-r--r--   0 i530566    (501) staff       (20)     8651 2023-04-10 17:40:19.000000 aprsd-3.0.3/aprsd/client.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.510176 aprsd-3.0.3/aprsd/clients/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.0.3/aprsd/clients/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     7021 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/clients/aprsis.py
--rw-r--r--   0 i530566    (501) staff       (20)     3413 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/clients/kiss.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.543321 aprsd-3.0.3/aprsd/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1764 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/cmds/completion.py
--rw-r--r--   0 i530566    (501) staff       (20)     3075 2023-04-17 14:51:22.000000 aprsd-3.0.3/aprsd/cmds/dev.py
--rw-r--r--   0 i530566    (501) staff       (20)     2810 2022-12-31 21:31:43.000000 aprsd-3.0.3/aprsd/cmds/healthcheck.py
--rw-r--r--   0 i530566    (501) staff       (20)     7921 2022-12-12 18:34:06.000000 aprsd-3.0.3/aprsd/cmds/list_plugins.py
--rw-r--r--   0 i530566    (501) staff       (20)     6056 2023-04-17 19:37:53.000000 aprsd-3.0.3/aprsd/cmds/listen.py
--rw-r--r--   0 i530566    (501) staff       (20)     4717 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/cmds/send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     3401 2023-04-20 18:32:02.000000 aprsd-3.0.3/aprsd/cmds/server.py
--rw-r--r--   0 i530566    (501) staff       (20)    14234 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/cmds/webchat.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.554285 aprsd-3.0.3/aprsd/conf/
--rw-r--r--   0 i530566    (501) staff       (20)     1733 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2353 2023-01-02 19:20:16.000000 aprsd-3.0.3/aprsd/conf/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     4863 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/conf/common.py
--rw-r--r--   0 i530566    (501) staff       (20)     1235 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/conf/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/opts.py
--rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/plugin_common.py
--rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.0.3/aprsd/conf/plugin_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/exception.py
--rw-r--r--   0 i530566    (501) staff       (20)    10299 2022-12-31 21:31:43.000000 aprsd-3.0.3/aprsd/flask.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.559034 aprsd-3.0.3/aprsd/logging/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/aprsd/logging/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2690 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/logging/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     5549 2022-12-12 18:34:07.000000 aprsd-3.0.3/aprsd/logging/rich.py
--rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/messaging.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.585487 aprsd-3.0.3/aprsd/packets/
--rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.0.3/aprsd/packets/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    16872 2023-04-17 14:51:23.000000 aprsd-3.0.3/aprsd/packets/core.py
--rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/packet_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/seen_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/tracker.py
--rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/watch_list.py
--rw-r--r--   0 i530566    (501) staff       (20)    16435 2023-04-25 18:29:36.000000 aprsd-3.0.3/aprsd/plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/plugin_utils.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.598755 aprsd-3.0.3/aprsd/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    23077 2022-12-29 19:18:54.000000 aprsd-3.0.3/aprsd/plugins/email.py
--rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     2844 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/location.py
--rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/plugins/notify.py
--rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.0.3/aprsd/plugins/ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/plugins/query.py
--rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/time.py
--rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/version.py
--rw-r--r--   0 i530566    (501) staff       (20)    13054 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/plugins/weather.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.603258 aprsd-3.0.3/aprsd/rpc/
--rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.0.3/aprsd/rpc/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     4192 2022-12-31 21:45:32.000000 aprsd-3.0.3/aprsd/rpc/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     2454 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/rpc/server.py
--rw-r--r--   0 i530566    (501) staff       (20)     6790 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/stats.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.630698 aprsd-3.0.3/aprsd/threads/
--rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/threads/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2023 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/aprsd.py
--rw-r--r--   0 i530566    (501) staff       (20)     3588 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/keep_alive.py
--rw-r--r--   0 i530566    (501) staff       (20)     2040 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/threads/log_monitor.py
--rw-r--r--   0 i530566    (501) staff       (20)    10431 2023-04-18 18:13:29.000000 aprsd-3.0.3/aprsd/threads/rx.py
--rw-r--r--   0 i530566    (501) staff       (20)     5977 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/tx.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.640640 aprsd-3.0.3/aprsd/utils/
--rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.0.3/aprsd/utils/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/counter.py
--rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/utils/fuzzyclock.py
--rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/json.py
--rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/utils/objectstore.py
--rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/ring_buffer.py
--rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/utils/trace.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.641786 aprsd-3.0.3/aprsd/web/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/web/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.642669 aprsd-3.0.3/aprsd/web/admin/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/web/admin/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.333545 aprsd-3.0.3/aprsd/web/admin/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.659116 aprsd-3.0.3/aprsd/web/admin/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/prism.css
--rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.701818 aprsd-3.0.3/aprsd/web/admin/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.798151 aprsd-3.0.3/aprsd/web/admin/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/web/admin/static/js/charts.js
--rw-r--r--   0 i530566    (501) staff       (20)      658 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/logs.js
--rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/prism.js
--rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.830654 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.840171 aprsd-3.0.3/aprsd/web/admin/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     8010 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/templates/index.html
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.336687 aprsd-3.0.3/aprsd/web/chat/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.336274 aprsd-3.0.3/aprsd/web/chat/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.911909 aprsd-3.0.3/aprsd/web/chat/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/style.css.map
--rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.953583 aprsd-3.0.3/aprsd/web/chat/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.034365 aprsd-3.0.3/aprsd/web/chat/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.0.3/aprsd/web/chat/static/js/gps.js
--rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/static/js/send-message-mobile.js
--rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.045921 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.084993 aprsd-3.0.3/aprsd/web/chat/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/templates/index.html
--rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/templates/mobile.html
--rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.0.3/aprsd-lnav.json
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.504980 aprsd-3.0.3/aprsd.egg-info/
--rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)     4947 2023-04-25 18:44:12.000000 aprsd-3.0.3/aprsd.egg-info/SOURCES.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/dependency_links.txt
--rw-r--r--   0 i530566    (501) staff       (20)      172 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/entry_points.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/not-zip-safe
--rw-r--r--   0 i530566    (501) staff       (20)       47 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/pbr.json
--rw-r--r--   0 i530566    (501) staff       (20)     1104 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/requires.txt
--rw-r--r--   0 i530566    (501) staff       (20)        6 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/top_level.txt
--rw-r--r--   0 i530566    (501) staff       (20)      221 2022-12-07 14:15:59.000000 aprsd-3.0.3/dev-requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     3919 2023-01-19 19:14:47.000000 aprsd-3.0.3/dev-requirements.txt
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.105666 aprsd-3.0.3/docker/
--rw-r--r--   0 i530566    (501) staff       (20)     1640 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/Dockerfile
--rw-r--r--   0 i530566    (501) staff       (20)     2032 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/Dockerfile-dev
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.134451 aprsd-3.0.3/docker/bin/
--rwxr-xr-x   0 i530566    (501) staff       (20)      857 2023-04-17 19:30:57.000000 aprsd-3.0.3/docker/bin/listen.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)      812 2022-12-30 15:13:03.000000 aprsd-3.0.3/docker/bin/run.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/build.sh
--rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.0.3/docker/docker-compose.yml
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.243913 aprsd-3.0.3/docs/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.259216 aprsd-3.0.3/docs/_static/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/_static/.keep
--rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/_static/aprsd_overview.png
--rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/_static/aprsd_overview.svg
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.261261 aprsd-3.0.3/docs/_templates/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/_templates/.keep
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.349525 aprsd-3.0.3/docs/apidoc/
--rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.clients.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.cmds.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.conf.rst
--rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.logging.rst
--rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.packets.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.0.3/docs/apidoc/aprsd.plugins.rst
--rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.rpc.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.rst
--rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.threads.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.utils.rst
--rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.web.admin.rst
--rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.web.rst
--rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.0.3/docs/apidoc/modules.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/aprsd.drawio
--rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.0.3/docs/changelog.rst
--rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.0.3/docs/clean_docs.py
--rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/conf.py
--rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/configure.rst
--rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/index.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/install.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/links.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/plugin.rst
--rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.0.3/docs/readme.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/server.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.339922 aprsd-3.0.3/examples/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.357473 aprsd-3.0.3/examples/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/examples/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)      409 2022-12-20 22:38:48.000000 aprsd-3.0.3/examples/plugins/example_plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.0.3/gray.conf
--rw-r--r--   0 i530566    (501) staff       (20)      538 2021-08-30 17:18:20.000000 aprsd-3.0.3/pyproject.toml
--rw-r--r--   0 i530566    (501) staff       (20)      551 2023-01-19 19:14:47.000000 aprsd-3.0.3/requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     3401 2023-01-19 19:14:47.000000 aprsd-3.0.3/requirements.txt
--rw-r--r--   0 i530566    (501) staff       (20)     1246 2023-04-25 18:44:13.406996 aprsd-3.0.3/setup.cfg
--rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.0.3/setup.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.382803 aprsd-3.0.3/tests/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/tests/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.385445 aprsd-3.0.3/tests/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.0.3/tests/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1819 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/cmds/test_send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     2505 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/cmds/test_webchat.py
--rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.0.3/tests/fake.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.394355 aprsd-3.0.3/tests/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/tests/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     3793 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_location.py
--rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_notify.py
--rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_query.py
--rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_time.py
--rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_version.py
--rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_weather.py
--rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_main.py
--rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.0.3/tests/test_packets.py
--rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_plugin.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.398513 aprsd-3.0.3/tools/
--rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.0.3/tools/fast8.sh
--rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.0.3/tox.ini
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.308052 aprsd-3.1.0/
+-rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.1.0/.coveragerc
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.284960 aprsd-3.1.0/.github/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.429268 aprsd-3.1.0/.github/workflows/
+-rw-r--r--   0 i530566    (501) staff       (20)     1461 2023-07-18 00:59:03.000000 aprsd-3.1.0/.github/workflows/manual_build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)     1629 2023-07-20 18:34:31.000000 aprsd-3.1.0/.github/workflows/master-build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      523 2023-06-22 11:55:10.000000 aprsd-3.1.0/.github/workflows/python.yml
+-rw-r--r--   0 i530566    (501) staff       (20)     1270 2023-07-20 19:10:23.000000 aprsd-3.1.0/.github/workflows/release_build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.1.0/.readthedocs.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)      430 2023-07-24 15:26:54.000000 aprsd-3.1.0/AUTHORS
+-rw-r--r--   0 i530566    (501) staff       (20)    22689 2023-07-24 15:26:54.000000 aprsd-3.1.0/ChangeLog
+-rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.1.0/INSTALL.txt
+-rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.1.0/LICENSE
+-rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.1.0/MANIFEST.in
+-rw-r--r--   0 i530566    (501) staff       (20)     2737 2023-07-08 18:22:21.000000 aprsd-3.1.0/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-07-24 15:27:34.309527 aprsd-3.1.0/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)    20387 2023-07-16 20:28:02.000000 aprsd-3.1.0/README.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.513219 aprsd-3.1.0/aprsd/
+-rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10517 2023-07-18 17:07:59.000000 aprsd-3.1.0/aprsd/admin_web.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3208 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cli_helper.py
+-rw-r--r--   0 i530566    (501) staff       (20)     8776 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/client.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.572345 aprsd-3.1.0/aprsd/clients/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.1.0/aprsd/clients/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7207 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/clients/aprsis.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3413 2023-01-19 19:14:47.000000 aprsd-3.1.0/aprsd/clients/kiss.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.610912 aprsd-3.1.0/aprsd/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/completion.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3074 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/dev.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5348 2023-07-22 21:05:15.000000 aprsd-3.1.0/aprsd/cmds/fetch_stats.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2801 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cmds/healthcheck.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7920 2023-07-08 21:30:27.000000 aprsd-3.1.0/aprsd/cmds/list_plugins.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6241 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cmds/listen.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4716 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3416 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)    13478 2023-07-23 23:19:27.000000 aprsd-3.1.0/aprsd/cmds/webchat.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.633954 aprsd-3.1.0/aprsd/conf/
+-rw-r--r--   0 i530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.1.0/aprsd/conf/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2349 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/conf/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4863 2023-01-19 19:14:47.000000 aprsd-3.1.0/aprsd/conf/common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1379 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/conf/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/conf/opts.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/conf/plugin_common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.1.0/aprsd/conf/plugin_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/exception.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.662518 aprsd-3.1.0/aprsd/log/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2678 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5545 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/rich.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4571 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/main.py
+-rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/messaging.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.673148 aprsd-3.1.0/aprsd/packets/
+-rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.1.0/aprsd/packets/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    18801 2023-07-14 15:35:51.000000 aprsd-3.1.0/aprsd/packets/core.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/packet_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/seen_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/tracker.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/watch_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)    16435 2023-04-25 18:29:36.000000 aprsd-3.1.0/aprsd/plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2458 2023-04-07 15:21:31.000000 aprsd-3.1.0/aprsd/plugin_utils.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.730992 aprsd-3.1.0/aprsd/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    23073 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/plugins/email.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3287 2023-07-10 15:01:50.000000 aprsd-3.1.0/aprsd/plugins/location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/plugins/notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.1.0/aprsd/plugins/ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/plugins/query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/version.py
+-rw-r--r--   0 i530566    (501) staff       (20)    13034 2023-07-15 22:22:29.000000 aprsd-3.1.0/aprsd/plugins/weather.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.772094 aprsd-3.1.0/aprsd/rpc/
+-rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.1.0/aprsd/rpc/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4641 2023-07-23 23:46:10.000000 aprsd-3.1.0/aprsd/rpc/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2760 2023-07-20 20:43:39.000000 aprsd-3.1.0/aprsd/rpc/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7177 2023-07-10 14:44:27.000000 aprsd-3.1.0/aprsd/stats.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.816413 aprsd-3.1.0/aprsd/threads/
+-rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/threads/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2270 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/threads/aprsd.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3921 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/threads/keep_alive.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2036 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/threads/log_monitor.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10431 2023-07-20 18:38:55.000000 aprsd-3.1.0/aprsd/threads/rx.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6437 2023-07-08 21:30:27.000000 aprsd-3.1.0/aprsd/threads/tx.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.877028 aprsd-3.1.0/aprsd/utils/
+-rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.1.0/aprsd/utils/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/counter.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/utils/fuzzyclock.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/json.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/utils/objectstore.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/ring_buffer.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/utils/trace.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.879119 aprsd-3.1.0/aprsd/web/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/web/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.881149 aprsd-3.1.0/aprsd/web/admin/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/web/admin/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.314036 aprsd-3.1.0/aprsd/web/admin/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.907620 aprsd-3.1.0/aprsd/web/admin/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/prism.css
+-rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.928268 aprsd-3.1.0/aprsd/web/admin/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.962973 aprsd-3.1.0/aprsd/web/admin/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/web/admin/static/js/charts.js
+-rw-r--r--   0 i530566    (501) staff       (20)      658 2023-07-23 01:28:13.000000 aprsd-3.1.0/aprsd/web/admin/static/js/logs.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/web/admin/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/js/prism.js
+-rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/web/admin/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.005749 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.007162 aprsd-3.1.0/aprsd/web/admin/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     8034 2023-07-23 23:46:10.000000 aprsd-3.1.0/aprsd/web/admin/templates/index.html
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.318699 aprsd-3.1.0/aprsd/web/chat/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.318180 aprsd-3.1.0/aprsd/web/chat/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.016733 aprsd-3.1.0/aprsd/web/chat/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/style.css.map
+-rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.037680 aprsd-3.1.0/aprsd/web/chat/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.064005 aprsd-3.1.0/aprsd/web/chat/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.1.0/aprsd/web/chat/static/js/gps.js
+-rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/static/js/send-message-mobile.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.066743 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.069691 aprsd-3.1.0/aprsd/web/chat/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/templates/index.html
+-rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/templates/mobile.html
+-rw-r--r--   0 i530566    (501) staff       (20)    10009 2023-07-24 13:39:24.000000 aprsd-3.1.0/aprsd/wsgi.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.1.0/aprsd-lnav.json
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.568338 aprsd-3.1.0/aprsd.egg-info/
+-rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)     5051 2023-07-24 15:27:33.000000 aprsd-3.1.0/aprsd.egg-info/SOURCES.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/dependency_links.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      171 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/entry_points.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-07-24 15:19:29.000000 aprsd-3.1.0/aprsd.egg-info/not-zip-safe
+-rw-r--r--   0 i530566    (501) staff       (20)       46 2023-07-24 15:26:55.000000 aprsd-3.1.0/aprsd.egg-info/pbr.json
+-rw-r--r--   0 i530566    (501) staff       (20)     1296 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/requires.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        6 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/top_level.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.1.0/dev-requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     3898 2023-07-23 23:46:10.000000 aprsd-3.1.0/dev-requirements.txt
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.081769 aprsd-3.1.0/docker/
+-rw-r--r--   0 i530566    (501) staff       (20)     1748 2023-05-05 15:07:23.000000 aprsd-3.1.0/docker/Dockerfile
+-rw-r--r--   0 i530566    (501) staff       (20)     1557 2023-07-24 00:22:47.000000 aprsd-3.1.0/docker/Dockerfile-dev
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.107767 aprsd-3.1.0/docker/bin/
+-rwxr-xr-x   0 i530566    (501) staff       (20)     1106 2023-07-24 00:22:47.000000 aprsd-3.1.0/docker/bin/admin.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)      864 2023-07-18 00:59:03.000000 aprsd-3.1.0/docker/bin/listen.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)      819 2023-07-18 00:59:03.000000 aprsd-3.1.0/docker/bin/run.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.1.0/docker/build.sh
+-rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.1.0/docker/docker-compose.yml
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.137728 aprsd-3.1.0/docs/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.164061 aprsd-3.1.0/docs/_static/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/_static/.keep
+-rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/_static/aprsd_overview.png
+-rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/_static/aprsd_overview.svg
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.166276 aprsd-3.1.0/docs/_templates/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/_templates/.keep
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.225686 aprsd-3.1.0/docs/apidoc/
+-rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.clients.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.cmds.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.conf.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.logging.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.packets.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.1.0/docs/apidoc/aprsd.plugins.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.rpc.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.threads.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.utils.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.web.admin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.web.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.1.0/docs/apidoc/modules.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/aprsd.drawio
+-rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.1.0/docs/changelog.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.1.0/docs/clean_docs.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/conf.py
+-rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/configure.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/index.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/install.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/links.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/plugin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.1.0/docs/readme.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/server.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.323523 aprsd-3.1.0/examples/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.229188 aprsd-3.1.0/examples/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.0/examples/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.1.0/examples/plugins/example_plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.1.0/gray.conf
+-rw-r--r--   0 i530566    (501) staff       (20)      538 2021-08-30 17:18:20.000000 aprsd-3.1.0/pyproject.toml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2023-07-23 23:46:10.000000 aprsd-3.1.0/requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     4086 2023-07-23 23:46:10.000000 aprsd-3.1.0/requirements.txt
+-rw-r--r--   0 i530566    (501) staff       (20)     1245 2023-07-24 15:27:34.321796 aprsd-3.1.0/setup.cfg
+-rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.1.0/setup.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.257471 aprsd-3.1.0/tests/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.0/tests/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.264798 aprsd-3.1.0/tests/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.1.0/tests/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.1.0/tests/cmds/test_send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2498 2023-07-20 19:10:23.000000 aprsd-3.1.0/tests/cmds/test_webchat.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.1.0/tests/fake.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.283374 aprsd-3.1.0/tests/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/tests/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.1.0/tests/plugins/test_location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_version.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_weather.py
+-rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_main.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.1.0/tests/test_packets.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_plugin.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.304991 aprsd-3.1.0/tools/
+-rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.1.0/tools/fast8.sh
+-rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.1.0/tox.ini
```

### Comparing `aprsd-3.0.3/.github/workflows/master-build.yml` & `aprsd-3.1.0/.github/workflows/master-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
         - "master"
 
 jobs:
   tox:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox tox-gh-actions
+        pip install tox tox-gh>=1.2
     - name: Test with tox
       run: tox
 
   build:
     needs: tox
     runs-on: ubuntu-latest
     steps:
```

### Comparing `aprsd-3.0.3/.github/workflows/python.yml` & `aprsd-3.1.0/.github/workflows/python.yml`

 * *Files 22% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox tox-gh-actions
+        pip install tox tox-gh>=1.2
     - name: Test with tox
       run: tox
```

### Comparing `aprsd-3.0.3/.github/workflows/release_build.yml` & `aprsd-3.1.0/.github/workflows/release_build.yml`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       with:
         username: ${{ secrets.DOCKERHUB_USERNAME }}
         password: ${{ secrets.DOCKERHUB_TOKEN }}
     - name: Build the Docker image
       uses: docker/build-push-action@v3
       with:
         context: "{{defaultContext}}:docker"
-        platforms: linux/amd64,linux/arm64,linux/arm/v7
+        platforms: linux/amd64,linux/arm64
         file: ./Dockerfile
         build-args: |
             VERSION=${{ inputs.aprsd_version }}
             BUILDX_QEMU_ENV=true
         push: true
         tags: |
           hemna6969/aprsd:v${{ inputs.aprsd_version }}
```

### Comparing `aprsd-3.0.3/.pre-commit-config.yaml` & `aprsd-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/ChangeLog` & `aprsd-3.1.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,10 @@
 CHANGES
 =======
 
-v3.0.3
-------
-
-* cleanup some debug messages
-* Fixed loading of plugins for server
-* Don't load help plugin for listen command
-* Added listen args
-* Change listen command plugins
-* Added listen.sh for docker
-* Update Listen command
-* Update Dockerfile
-* Add ratelimiting for acks and other packets
-
-v3.0.2
-------
-
-* Update Changelog for 3.0.2
-* Import RejectPacket
-
-v3.0.1
-------
-
-* 3.0.1
-* Add support to Reject messages
-* Update Docker builds for 3.0.0
-
-v3.0.0
-------
-
-* Update Changelog for 3.0.0
-* Ensure server command main thread doesn't exit
-* Fixed save directory default
-* Fixed pep8 failure
-* Cleaned up KISS interfaces use of old config
-* reworked usage of importlib.metadata
-* Added new docs files for 3.0.0
-* Removed url option from healthcheck in dev
-* Updated Healthcheck to use rpc to call aprsd
-* Updated docker/bin/run.sh to use new conf
-* Added ObjectPacket
-* Update regex processing and regex for plugins
-* Change ordering of starting up of server command
-* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.0.3/INSTALL.txt` & `aprsd-3.1.0/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/LICENSE` & `aprsd-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/Makefile` & `aprsd-3.1.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 .PHONY: dev docs server test
 
 include Makefile.venv
 Makefile.venv:
 	curl \
 		-o Makefile.fetched \
-		-L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/Makefile.venv"
-	echo "147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8 *Makefile.fetched" \
+		-L "https://raw.githubusercontent.com/sio/Makefile.venv/master/Makefile.venv"
+	echo " fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82 *Makefile.fetched" \
 		| sha256sum --check - \
 		&& mv Makefile.fetched Makefile.venv
 
 help:	# Help for the Makefile
 	@egrep -h '\s##\s' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-20s\033[0m %s\n", $$1, $$2}'
 
 dev: REQUIREMENTS_TXT = requirements.txt dev-requirements.txt
```

### Comparing `aprsd-3.0.3/PKG-INFO` & `aprsd-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.0.3
+Version: 3.1.0
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
@@ -306,14 +306,28 @@
     To          : KM6XXX-6
     Ack         : 2
     Sending ack _______________ Complete
 
 AND... ping, fortune, time.....
 
 
+Web Admin Interface
+===================
+To start the web admin interface, You have to install gunicorn in your virtualenv that already has aprsd installed.
+
+::
+
+  source <path to APRSD's virtualenv>/bin/activate
+  pip install gunicorn
+  gunicorn --bind 0.0.0.0:8080 "aprsd.wsgi:app"
+
+The web admin interface will be running on port 8080 on the local machine.  http://localhost:8080
+
+
+
 Development
 ===========
 
 * ``git clone git@github.com:craigerl/aprsd.git``
 * ``cd aprsd``
 * ``make``
```

### Comparing `aprsd-3.0.3/README.rst` & `aprsd-3.1.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/__init__.py` & `aprsd-3.1.0/aprsd/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/aprsd.py` & `aprsd-3.1.0/aprsd/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 # local imports here
 import aprsd
 from aprsd import cli_helper, packets, stats, threads, utils
 
 
 # setup the global logger
-# logging.basicConfig(level=logging.DEBUG) # level=10
+# log.basicConfig(level=log.DEBUG) # level=10
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 flask_enabled = False
 rpc_serv = None
 
 
@@ -66,16 +66,16 @@
     pass
 
 
 def main():
     # First import all the possible commands for the CLI
     # The commands themselves live in the cmds directory
     from .cmds import (  # noqa
-        completion, dev, healthcheck, list_plugins, listen, send_message,
-        server, webchat,
+        completion, dev, fetch_stats, healthcheck, list_plugins, listen,
+        send_message, server, webchat,
     )
     cli(auto_envvar_prefix="APRSD")
 
 
 def signal_handler(sig, frame):
     global flask_enabled
```

### Comparing `aprsd-3.0.3/aprsd/cli_helper.py` & `aprsd-3.1.0/aprsd/cli_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing as t
 
 import click
 from oslo_config import cfg
 
 import aprsd
 from aprsd import conf  # noqa: F401
-from aprsd.logging import log
+from aprsd.log import log
 from aprsd.utils import trace
 
 
 CONF = cfg.CONF
 home = str(Path.home())
 DEFAULT_CONFIG_DIR = f"{home}/.config/aprsd/"
 DEFAULT_SAVE_FILE = f"{home}/.config/aprsd/aprsd.p"
```

### Comparing `aprsd-3.0.3/aprsd/client.py` & `aprsd-3.1.0/aprsd/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         packet_list.PacketList().tx(packet)
         self.client.send(packet)
 
     def reset(self):
         """Call this to force a rebuild/reconnect."""
         if self._client:
             del self._client
+        else:
+            LOG.warning("Client not initialized, nothing to reset.")
 
     @abc.abstractmethod
     def setup_connection(self):
         pass
 
     @staticmethod
     @abc.abstractmethod
@@ -140,25 +142,26 @@
         connected = False
         backoff = 1
         aprs_client = None
         while not connected:
             try:
                 LOG.info("Creating aprslib client")
                 aprs_client = aprsis.Aprsdis(user, passwd=password, host=host, port=port)
-                # Force the logging to be the same
+                # Force the log to be the same
                 aprs_client.logger = LOG
                 aprs_client.connect()
                 connected = True
                 backoff = 1
             except LoginError as e:
                 LOG.error(f"Failed to login to APRS-IS Server '{e}'")
                 connected = False
-                raise e
+                time.sleep(backoff)
             except Exception as e:
                 LOG.error(f"Unable to connect to APRS-IS server. '{e}' ")
+                connected = False
                 time.sleep(backoff)
                 backoff = backoff * 2
                 continue
         LOG.debug(f"Logging in to APRS-IS with user '{user}'")
         self._client = aprs_client
         return aprs_client
```

### Comparing `aprsd-3.0.3/aprsd/clients/aprsis.py` & `aprsd-3.1.0/aprsd/clients/aprsis.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,50 +108,55 @@
 
         self.logger.info("Sending login information")
 
         try:
             self._sendall(login_str)
             self.sock.settimeout(5)
             test = self.sock.recv(len(login_str) + 100)
+            self.logger.debug("Server: '%s'", test)
             if is_py3:
                 test = test.decode("latin-1")
             test = test.rstrip()
 
-            self.logger.debug("Server: %s", test)
+            self.logger.debug("Server: '%s'", test)
 
-            a, b, callsign, status, e = test.split(" ", 4)
+            if not test:
+                raise LoginError(f"Server Response Empty: '{test}'")
+
+            _, _, callsign, status, e = test.split(" ", 4)
             s = e.split(",")
             if len(s):
                 server_string = s[0].replace("server ", "")
             else:
                 server_string = e.replace("server ", "")
 
-            self.logger.info(f"Connected to {server_string}")
-            self.server_string = server_string
-            stats.APRSDStats().set_aprsis_server(server_string)
-
             if callsign == "":
                 raise LoginError("Server responded with empty callsign???")
             if callsign != self.callsign:
                 raise LoginError(f"Server: {test}")
             if status != "verified," and self.passwd != "-1":
                 raise LoginError("Password is incorrect")
 
             if self.passwd == "-1":
                 self.logger.info("Login successful (receive only)")
             else:
                 self.logger.info("Login successful")
 
+            self.logger.info(f"Connected to {server_string}")
+            self.server_string = server_string
+            stats.APRSDStats().set_aprsis_server(server_string)
+
         except LoginError as e:
             self.logger.error(str(e))
             self.close()
             raise
         except Exception as e:
             self.close()
             self.logger.error(f"Failed to login '{e}'")
+            self.logger.exception(e)
             raise LoginError("Failed to login")
 
     def consumer(self, callback, blocking=True, immortal=False, raw=False):
         """
         When a position sentence is received, it will be passed to the callback function
 
         blocking: if true (default), runs forever, otherwise will return after one sentence
```

### Comparing `aprsd-3.0.3/aprsd/clients/kiss.py` & `aprsd-3.1.0/aprsd/clients/kiss.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/cmds/completion.py` & `aprsd-3.1.0/aprsd/cmds/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 import click_completion
 
-from aprsd.aprsd import cli
+from aprsd.main import cli
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @cli.group(help="Click Completion subcommands", context_settings=CONTEXT_SETTINGS)
 @click.pass_context
```

### Comparing `aprsd-3.0.3/aprsd/cmds/dev.py` & `aprsd-3.1.0/aprsd/cmds/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 import click
 from oslo_config import cfg
 
 # local imports here
 from aprsd import cli_helper, client, conf, packets, plugin
-from aprsd.aprsd import cli
+from aprsd.main import cli
 from aprsd.utils import trace
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
```

### Comparing `aprsd-3.0.3/aprsd/cmds/healthcheck.py` & `aprsd-3.1.0/aprsd/cmds/healthcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 from oslo_config import cfg
 from rich.console import Console
 
 import aprsd
 from aprsd import cli_helper, utils
 from aprsd import conf  # noqa
 # local imports here
-from aprsd.aprsd import cli
+from aprsd.main import cli
 from aprsd.rpc import client as aprsd_rpc_client
 
 
 # setup the global logger
-# logging.basicConfig(level=logging.DEBUG) # level=10
+# log.basicConfig(level=log.DEBUG) # level=10
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 console = Console()
 
 
 @cli.command()
 @cli_helper.add_options(cli_helper.common_options)
```

### Comparing `aprsd-3.0.3/aprsd/cmds/list_plugins.py` & `aprsd-3.1.0/aprsd/cmds/list_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from thesmuggler import smuggle
 
 from aprsd import cli_helper
 from aprsd import plugin as aprsd_plugin
-from aprsd.aprsd import cli
+from aprsd.main import cli
 from aprsd.plugins import (
     email, fortune, location, notify, ping, query, time, version, weather,
 )
 
 
 LOG = logging.getLogger("APRSD")
```

### Comparing `aprsd-3.0.3/aprsd/cmds/listen.py` & `aprsd-3.1.0/aprsd/cmds/listen.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 import click
 from oslo_config import cfg
 from rich.console import Console
 
 # local imports here
 import aprsd
 from aprsd import cli_helper, client, packets, plugin, stats, threads
-from aprsd.aprsd import cli
+from aprsd.main import cli
+from aprsd.rpc import server as rpc_server
 from aprsd.threads import rx
 
 
 # setup the global logger
-# logging.basicConfig(level=logging.DEBUG) # level=10
+# log.basicConfig(level=log.DEBUG) # level=10
 LOG = logging.getLogger("APRSD")
 CONF = cfg.CONF
 console = Console()
 
 
 def signal_handler(sig, frame):
     threads.APRSDThreadList().stop_all()
@@ -177,14 +178,18 @@
 
     LOG.debug(f"Filter by '{filter}'")
     aprs_client.set_filter(filter)
 
     keepalive = threads.KeepAliveThread()
     keepalive.start()
 
+    if CONF.rpc_settings.enabled:
+        rpc = rpc_server.APRSDRPCThread()
+        rpc.start()
+
     pm = None
     pm = plugin.PluginManager()
     if load_plugins:
         LOG.info("Loading plugins")
         pm.setup_plugins(load_help_plugin=False)
     else:
         LOG.warning(
@@ -200,7 +205,10 @@
     )
     LOG.debug("Start APRSDListenThread")
     listen_thread.start()
     LOG.debug("keepalive Join")
     keepalive.join()
     LOG.debug("listen_thread Join")
     listen_thread.join()
+
+    if CONF.rpc_settings.enabled:
+        rpc.join()
```

### Comparing `aprsd-3.0.3/aprsd/cmds/send_message.py` & `aprsd-3.1.0/aprsd/cmds/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from aprslib.exceptions import LoginError
 import click
 from oslo_config import cfg
 
 import aprsd
 from aprsd import cli_helper, client, packets
 from aprsd import conf  # noqa : F401
-from aprsd.aprsd import cli
+from aprsd.main import cli
 from aprsd.threads import tx
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
```

### Comparing `aprsd-3.0.3/aprsd/cmds/server.py` & `aprsd-3.1.0/aprsd/cmds/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import signal
 import sys
 
 import click
 from oslo_config import cfg
 
 import aprsd
-from aprsd import aprsd as aprsd_main
-from aprsd import cli_helper, client, packets, plugin, threads, utils
-from aprsd.aprsd import cli
+from aprsd import cli_helper, client
+from aprsd import main as aprsd_main
+from aprsd import packets, plugin, threads, utils
+from aprsd.main import cli
 from aprsd.rpc import server as rpc_server
 from aprsd.threads import rx
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
```

### Comparing `aprsd-3.0.3/aprsd/cmds/webchat.py` & `aprsd-3.1.0/aprsd/cmds/webchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,42 @@
 import time
 
 from aprslib import util as aprslib_util
 import click
 import flask
 from flask import request
 from flask.logging import default_handler
-import flask_classful
 from flask_httpauth import HTTPBasicAuth
 from flask_socketio import Namespace, SocketIO
 from oslo_config import cfg
 from user_agents import parse as ua_parse
 from werkzeug.security import check_password_hash, generate_password_hash
 import wrapt
 
 import aprsd
 from aprsd import cli_helper, client, conf, packets, stats, threads, utils
-from aprsd.aprsd import cli
-from aprsd.logging import rich as aprsd_logging
+from aprsd.log import rich as aprsd_logging
+from aprsd.main import cli
 from aprsd.threads import rx, tx
 from aprsd.utils import objectstore, trace
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 auth = HTTPBasicAuth()
-users = None
+users = {}
 socketio = None
 
+flask_app = flask.Flask(
+    "aprsd",
+    static_url_path="/static",
+    static_folder="web/chat/static",
+    template_folder="web/chat/templates",
+)
+
 
 def signal_handler(sig, frame):
 
     click.echo("signal_handler: called")
     LOG.info(
         f"Ctrl+C, Sending all threads({len(threads.APRSDThreadList())}) exit! "
         f"Can take up to 10 seconds {datetime.datetime.now()}",
@@ -170,114 +176,116 @@
         }
         self.socketio.emit(
             "new", msg,
             namespace="/sendmsg",
         )
 
 
-class WebChatFlask(flask_classful.FlaskView):
+def set_config():
+    global users
 
-    def set_config(self):
-        global users
-        self.users = {}
-        user = CONF.admin.user
-        self.users[user] = generate_password_hash(CONF.admin.password)
-        users = self.users
-
-    def _get_transport(self, stats):
-        if CONF.aprs_network.enabled:
-            transport = "aprs-is"
-            aprs_connection = (
-                "APRS-IS Server: <a href='http://status.aprs2.net' >"
-                "{}</a>".format(stats["stats"]["aprs-is"]["server"])
-            )
-        else:
-            # We might be connected to a KISS socket?
-            if client.KISSClient.is_enabled():
-                transport = client.KISSClient.transport()
-                if transport == client.TRANSPORT_TCPKISS:
-                    aprs_connection = (
-                        "TCPKISS://{}:{}".format(
-                            CONF.kiss_tcp.host,
-                            CONF.kiss_tcp.port,
-                        )
-                    )
-                elif transport == client.TRANSPORT_SERIALKISS:
-                    # for pep8 violation
-                    aprs_connection = (
-                        "SerialKISS://{}@{} baud".format(
-                            CONF.kiss_serial.device,
-                            CONF.kiss_serial.baudrate,
-                        ),
+
+def _get_transport(stats):
+    if CONF.aprs_network.enabled:
+        transport = "aprs-is"
+        aprs_connection = (
+            "APRS-IS Server: <a href='http://status.aprs2.net' >"
+            "{}</a>".format(stats["stats"]["aprs-is"]["server"])
+        )
+    else:
+        # We might be connected to a KISS socket?
+        if client.KISSClient.is_enabled():
+            transport = client.KISSClient.transport()
+            if transport == client.TRANSPORT_TCPKISS:
+                aprs_connection = (
+                    "TCPKISS://{}:{}".format(
+                        CONF.kiss_tcp.host,
+                        CONF.kiss_tcp.port,
                     )
+                )
+            elif transport == client.TRANSPORT_SERIALKISS:
+                # for pep8 violation
+                aprs_connection = (
+                    "SerialKISS://{}@{} baud".format(
+                        CONF.kiss_serial.device,
+                        CONF.kiss_serial.baudrate,
+                    ),
+                )
+
+    return transport, aprs_connection
+
+
+@auth.login_required
+@flask_app.route("/")
+def index():
+    ua_str = request.headers.get("User-Agent")
+    # this takes about 2 seconds :(
+    user_agent = ua_parse(ua_str)
+    LOG.debug(f"Is mobile? {user_agent.is_mobile}")
+    stats = _stats()
 
-        return transport, aprs_connection
+    if user_agent.is_mobile:
+        html_template = "mobile.html"
+    else:
+        html_template = "index.html"
 
-    @auth.login_required
-    def index(self):
-        ua_str = request.headers.get("User-Agent")
-        # this takes about 2 seconds :(
-        user_agent = ua_parse(ua_str)
-        LOG.debug(f"Is mobile? {user_agent.is_mobile}")
-        stats = self._stats()
-
-        if user_agent.is_mobile:
-            html_template = "mobile.html"
-        else:
-            html_template = "index.html"
-
-        # For development
-        # html_template = "mobile.html"
-
-        LOG.debug(f"Template {html_template}")
-
-        transport, aprs_connection = self._get_transport(stats)
-        LOG.debug(f"transport {transport} aprs_connection {aprs_connection}")
-
-        stats["transport"] = transport
-        stats["aprs_connection"] = aprs_connection
-        LOG.debug(f"initial stats = {stats}")
-
-        return flask.render_template(
-            html_template,
-            initial_stats=stats,
-            aprs_connection=aprs_connection,
-            callsign=CONF.callsign,
-            version=aprsd.__version__,
-        )
+    # For development
+    # html_template = "mobile.html"
 
-    @auth.login_required
-    def send_message_status(self):
-        LOG.debug(request)
-        msgs = SentMessages()
-        info = msgs.get_all()
-        return json.dumps(info)
+    LOG.debug(f"Template {html_template}")
 
-    def _stats(self):
-        stats_obj = stats.APRSDStats()
-        now = datetime.datetime.now()
-
-        time_format = "%m-%d-%Y %H:%M:%S"
-        stats_dict = stats_obj.stats()
-        # Webchat doesnt need these
-        del stats_dict["aprsd"]["watch_list"]
-        del stats_dict["aprsd"]["seen_list"]
-        # del stats_dict["email"]
-        # del stats_dict["plugins"]
-        # del stats_dict["messages"]
-
-        result = {
-            "time": now.strftime(time_format),
-            "stats": stats_dict,
-        }
+    transport, aprs_connection = _get_transport(stats)
+    LOG.debug(f"transport {transport} aprs_connection {aprs_connection}")
+
+    stats["transport"] = transport
+    stats["aprs_connection"] = aprs_connection
+    LOG.debug(f"initial stats = {stats}")
+
+    return flask.render_template(
+        html_template,
+        initial_stats=stats,
+        aprs_connection=aprs_connection,
+        callsign=CONF.callsign,
+        version=aprsd.__version__,
+    )
 
-        return result
 
-    def stats(self):
-        return json.dumps(self._stats())
+@auth.login_required
+@flask_app.route("//send-message-status")
+def send_message_status():
+    LOG.debug(request)
+    msgs = SentMessages()
+    info = msgs.get_all()
+    return json.dumps(info)
+
+
+def _stats():
+    stats_obj = stats.APRSDStats()
+    now = datetime.datetime.now()
+
+    time_format = "%m-%d-%Y %H:%M:%S"
+    stats_dict = stats_obj.stats()
+    # Webchat doesnt need these
+    del stats_dict["aprsd"]["watch_list"]
+    del stats_dict["aprsd"]["seen_list"]
+    # del stats_dict["email"]
+    # del stats_dict["plugins"]
+    # del stats_dict["messages"]
+
+    result = {
+        "time": now.strftime(time_format),
+        "stats": stats_dict,
+    }
+
+    return result
+
+
+@flask_app.route("/stats")
+def get_stats():
+    return json.dumps(_stats())
 
 
 class SendMessageNamespace(Namespace):
     """Class to handle the socketio interactions."""
     got_ack = False
     reply_sent = False
     msg = None
@@ -373,29 +381,17 @@
         )
         fh.setFormatter(log_formatter)
         flask_log.addHandler(fh)
 
 
 @trace.trace
 def init_flask(loglevel, quiet):
-    global socketio
+    global socketio, flask_app
 
-    flask_app = flask.Flask(
-        "aprsd",
-        static_url_path="/static",
-        static_folder="web/chat/static",
-        template_folder="web/chat/templates",
-    )
     setup_logging(flask_app, loglevel, quiet)
-    server = WebChatFlask()
-    server.set_config()
-    flask_app.route("/", methods=["GET"])(server.index)
-    flask_app.route("/stats", methods=["GET"])(server.stats)
-    # flask_app.route("/send-message", methods=["GET"])(server.send_message)
-    flask_app.route("/send-message-status", methods=["GET"])(server.send_message_status)
 
     socketio = SocketIO(
         flask_app, logger=False, engineio_logger=False,
         async_mode="threading",
     )
     # async_mode="gevent",
     # async_mode="eventlet",
@@ -403,15 +399,15 @@
     #    eventlet.monkey_patch()
 
     socketio.on_namespace(
         SendMessageNamespace(
             "/sendmsg",
         ),
     )
-    return socketio, flask_app
+    return socketio
 
 
 # main() ###
 @cli.command()
 @cli_helper.add_options(cli_helper.common_options)
 @click.option(
     "-f",
@@ -444,14 +440,16 @@
     if level:
         LOG.warning(msg)
     else:
         LOG.info(msg)
     LOG.info(f"APRSD Started version: {aprsd.__version__}")
 
     CONF.log_opt_values(LOG, logging.DEBUG)
+    user = CONF.admin.user
+    users[user] = generate_password_hash(CONF.admin.password)
 
     # Initialize the client factory and create
     # The correct client object ready for use
     client.ClientFactory.setup()
     # Make sure we have 1 client transport enabled
     if not client.factory.is_client_enabled():
         LOG.error("No Clients are enabled in config.")
@@ -462,15 +460,15 @@
         sys.exit(-1)
 
     packets.PacketList()
     packets.PacketTrack()
     packets.WatchList()
     packets.SeenList()
 
-    (socketio, app) = init_flask(loglevel, quiet)
+    socketio = init_flask(loglevel, quiet)
     rx_thread = rx.APRSDPluginRXThread(
         packet_queue=threads.packet_queue,
     )
     rx_thread.start()
     process_thread = WebChatProcessPacketThread(
         packet_queue=threads.packet_queue,
         socketio=socketio,
@@ -478,14 +476,14 @@
     process_thread.start()
 
     keepalive = threads.KeepAliveThread()
     LOG.info("Start KeepAliveThread")
     keepalive.start()
     LOG.info("Start socketio.run()")
     socketio.run(
-        app,
+        flask_app,
         ssl_context="adhoc",
         host=CONF.admin.web_ip,
         port=port,
     )
 
     LOG.info("WebChat exiting!!!!  Bye.")
```

### Comparing `aprsd-3.0.3/aprsd/conf/__init__.py` & `aprsd-3.1.0/aprsd/conf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Update default value of oslo_log default_log_levels and
     # logging_context_format_string config option.
     set_log_defaults()
 
 
 def set_log_defaults():
-    # logging.set_defaults(default_log_levels=logging.get_default_log_levels())
+    # log.set_defaults(default_log_levels=log.get_default_log_levels())
     pass
 
 
 def conf_to_dict():
     """Convert the CONF options to a single level dictionary."""
     entries = {}
```

### Comparing `aprsd-3.0.3/aprsd/conf/client.py` & `aprsd-3.1.0/aprsd/conf/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The options for logging setup
+The options for log setup
 """
 
 from oslo_config import cfg
 
 
 DEFAULT_LOGIN = "NOCALL"
```

### Comparing `aprsd-3.0.3/aprsd/conf/common.py` & `aprsd-3.1.0/aprsd/conf/common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/conf/log.py` & `aprsd-3.1.0/aprsd/conf/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The options for logging setup
+The options for log setup
 """
 import logging
 
 from oslo_config import cfg
 
 
 LOG_LEVELS = {
@@ -29,26 +29,32 @@
         "date_format",
         default=DEFAULT_DATE_FORMAT,
         help="Date format for log entries",
     ),
     cfg.BoolOpt(
         "rich_logging",
         default=True,
-        help="Enable Rich logging",
+        help="Enable Rich log",
     ),
     cfg.StrOpt(
         "logfile",
         default=None,
         help="File to log to",
     ),
     cfg.StrOpt(
         "logformat",
         default=DEFAULT_LOG_FORMAT,
         help="Log file format, unless rich_logging enabled.",
     ),
+    cfg.StrOpt(
+        "log_level",
+        default="INFO",
+        choices=LOG_LEVELS.keys(),
+        help="Log level for logging of events.",
+    ),
 ]
 
 
 def register_opts(config):
     config.register_group(logging_group)
     config.register_opts(logging_opts, group=logging_group)
```

### Comparing `aprsd-3.0.3/aprsd/conf/opts.py` & `aprsd-3.1.0/aprsd/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/conf/plugin_common.py` & `aprsd-3.1.0/aprsd/conf/plugin_common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/conf/plugin_email.py` & `aprsd-3.1.0/aprsd/conf/plugin_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/flask.py` & `aprsd-3.1.0/aprsd/admin_web.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from flask_httpauth import HTTPBasicAuth
 from flask_socketio import Namespace, SocketIO
 from oslo_config import cfg
 from werkzeug.security import check_password_hash, generate_password_hash
 
 import aprsd
 from aprsd import cli_helper, client, conf, packets, plugin, threads
-from aprsd.logging import rich as aprsd_logging
+from aprsd.log import rich as aprsd_logging
 from aprsd.rpc import client as aprsd_rpc_client
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 auth = HTTPBasicAuth()
@@ -331,17 +331,30 @@
     flask_app.logger.handlers = gunicorn_logger.handlers
     flask_app.logger.setLevel(gunicorn_logger.level)
 
     socketio.on_namespace(LoggingNamespace("/logs"))
     return socketio, flask_app
 
 
+def create_app(config_file=None, log_level=None):
+    global socketio
+    global app
+
+    default_config_file = cli_helper.DEFAULT_CONFIG_FILE
+    if not config_file:
+        config_file = default_config_file
+
+    CONF(
+        [], project="aprsd", version=aprsd.__version__,
+        default_config_files=[config_file],
+    )
+
+    if not log_level:
+        log_level = CONF.logging.log_level
+
+    socketio, app = init_flask(log_level, False)
+    setup_logging(app, log_level, False)
+    return app
+
+
 if __name__ == "aprsd.flask":
-    try:
-        default_config_file = cli_helper.DEFAULT_CONFIG_FILE
-        CONF(
-            [], project="aprsd", version=aprsd.__version__,
-            default_config_files=[default_config_file],
-        )
-    except cfg.ConfigFilesNotFoundError:
-        pass
-    sio, app = init_flask("DEBUG", False)
+    sio, app = create_app()
```

### Comparing `aprsd-3.0.3/aprsd/logging/log.py` & `aprsd-3.1.0/aprsd/log/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from logging.handlers import RotatingFileHandler
 import queue
 import sys
 
 from oslo_config import cfg
 
 from aprsd import conf
-from aprsd.logging import rich as aprsd_logging
+from aprsd.log import rich as aprsd_logging
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 logging_queue = queue.Queue()
 
 
-# Setup the logging faciility
-# to disable logging to stdout, but still log to file
+# Setup the log faciility
+# to disable log to stdout, but still log to file
 # use the --quiet option on the cmdln
 def setup_logging(loglevel, quiet):
     log_level = conf.log.LOG_LEVELS[loglevel]
     LOG.setLevel(log_level)
     date_format = CONF.logging.date_format
     rh = None
     fh = None
```

### Comparing `aprsd-3.0.3/aprsd/logging/rich.py` & `aprsd-3.1.0/aprsd/log/rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         self, *, record: LogRecord,
         traceback: Optional[Traceback],
         message_renderable: "ConsoleRenderable",
     ) -> "ConsoleRenderable":
         """Render log for display.
 
         Args:
-            record (LogRecord): logging Record.
+            record (LogRecord): log Record.
             traceback (Optional[Traceback]): Traceback instance or None for no Traceback.
             message_renderable (ConsoleRenderable): Renderable (typically Text) containing log message contents.
 
         Returns:
             ConsoleRenderable: Renderable to display log.
         """
         path = Path(record.pathname).name
```

### Comparing `aprsd-3.0.3/aprsd/packets/core.py` & `aprsd-3.1.0/aprsd/packets/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,17 +122,51 @@
             # Try and figure it out here
             if "latitude" in raw:
                 class_name = GPSPacket
 
         if packet_type == PACKET_TYPE_WX:
             # the weather information is in a dict
             # this brings those values out to the outer dict
+
             for key in raw["weather"]:
                 raw[key] = raw["weather"][key]
 
+            # If we have the broken aprslib, then we need to
+            # Convert the course and speed to wind_speed and wind_direction
+            # aprslib issue #80
+            # https://github.com/rossengeorgiev/aprs-python/issues/80
+            # Wind speed and course is option in the SPEC.
+            # For some reason aprslib multiplies the speed by 1.852.
+            if "wind_speed" not in raw and "wind_direction" not in raw:
+                # Most likely this is the broken aprslib
+                # So we need to convert the wind_gust speed
+                raw["wind_gust"] = round(raw.get("wind_gust", 0) / 0.44704, 3)
+            if "wind_speed" not in raw:
+                wind_speed = raw.get("speed")
+                if wind_speed:
+                    raw["wind_speed"] = round(wind_speed / 1.852, 3)
+                    raw["weather"]["wind_speed"] = raw["wind_speed"]
+                if "speed" in raw:
+                    del raw["speed"]
+                # Let's adjust the rain numbers as well, since it's wrong
+                raw["rain_1h"] = round((raw.get("rain_1h", 0) / .254) * .01, 3)
+                raw["weather"]["rain_1h"] = raw["rain_1h"]
+                raw["rain_24h"] = round((raw.get("rain_24h", 0) / .254) * .01, 3)
+                raw["weather"]["rain_24h"] = raw["rain_24h"]
+                raw["rain_since_midnight"] = round((raw.get("rain_since_midnight", 0) / .254) * .01, 3)
+                raw["weather"]["rain_since_midnight"] = raw["rain_since_midnight"]
+
+            if "wind_direction" not in raw:
+                wind_direction = raw.get("course")
+                if wind_direction:
+                    raw["wind_direction"] = wind_direction
+                    raw["weather"]["wind_direction"] = raw["wind_direction"]
+                if "course" in raw:
+                    del raw["course"]
+
         return dacite.from_dict(data_class=class_name, data=raw)
 
     def log(self, header=None):
         """LOG a packet to the logfile."""
         asdict(self)
         log_list = ["\n"]
         name = self.__class__.__name__
@@ -277,18 +311,14 @@
     longitude: float = 0.00
     altitude: float = 0.00
     rng: float = 0.00
     posambiguity: int = 0
     comment: str = None
     symbol: str = field(default="l")
     symbol_table: str = field(default="/")
-    # in MPH
-    speed: float = 0.00
-    # 0 to 360
-    course: int = 0
 
     def decdeg2dms(self, degrees_decimal):
         is_positive = degrees_decimal >= 0
         degrees_decimal = abs(degrees_decimal)
         minutes, seconds = divmod(degrees_decimal * 3600, 60)
         degrees, minutes = divmod(minutes, 60)
         degrees = degrees if is_positive else -degrees
@@ -383,24 +413,32 @@
 
 
 @dataclass
 class MicEPacket(GPSPacket):
     messagecapable: bool = False
     mbits: str = None
     mtype: str = None
+    # in MPH
+    speed: float = 0.00
+    # 0 to 360
+    course: int = 0
 
     def _build_raw(self):
         raise NotImplementedError
 
 
 @dataclass
 class ObjectPacket(GPSPacket):
     alive: bool = True
     raw_timestamp: str = None
     symbol: str = field(default="r")
+    # in MPH
+    speed: float = 0.00
+    # 0 to 360
+    course: int = 0
 
     def _build_raw(self):
         """
         REPEAT builds packets like
         reply = "{}>APZ100:;{:9s}*{}z{}r{:.3f}MHz {} {}".format(
                 fromcall, callsign, time_zulu, latlon, freq, uplink_tone, offset,
             )
@@ -420,14 +458,16 @@
         if self.comment:
             self.raw = f"{self.raw}{self.comment}"
 
 
 @dataclass()
 class WeatherPacket(GPSPacket):
     symbol: str = "_"
+    wind_speed: float = 0.00
+    wind_direction: int = 0
     wind_gust: float = 0.00
     temperature: float = 0.00
     # in inches.  1.04 means 1.04 inches
     rain_1h: float = 0.00
     rain_24h: float = 0.00
     rain_since_midnight: float = 0.00
     humidity: int = 0
@@ -457,24 +497,21 @@
         See notes on remotes below
         % shows software type d=Dos, m=Mac, w=Win, etc
         type shows type of WX instrument
 
         """
         time_zulu = self._build_time_zulu()
 
-        course = "%03u" % self.course
-
         contents = [
             f"{self.from_call}>{self.to_call},WIDE1-1,WIDE2-1:",
             f"@{time_zulu}z{self.latitude}{self.symbol_table}",
             f"{self.longitude}{self.symbol}",
-            # Add CSE = Course
-            f"{course}",
+            f"{self.wind_direction:03d}",
             # Speed = sustained 1 minute wind speed in mph
-            f"{self.symbol_table}", f"{self.speed:03.0f}",
+            f"{self.symbol_table}", f"{self.wind_speed:03.0f}",
             # wind gust (peak wind speed in mph in the last 5 minutes)
             f"g{self.wind_gust:03.0f}",
             # Temperature in degrees F
             f"t{self.temperature:03.0f}",
             # Rainfall (in hundredths of an inch) in the last hour
             f"r{self.rain_1h*100:03.0f}",
             # Rainfall (in hundredths of an inch) in last 24 hours
```

### Comparing `aprsd-3.0.3/aprsd/packets/packet_list.py` & `aprsd-3.1.0/aprsd/packets/packet_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/packets/seen_list.py` & `aprsd-3.1.0/aprsd/packets/seen_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/packets/tracker.py` & `aprsd-3.1.0/aprsd/packets/tracker.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/packets/watch_list.py` & `aprsd-3.1.0/aprsd/packets/watch_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugin.py` & `aprsd-3.1.0/aprsd/plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugin_utils.py` & `aprsd-3.1.0/aprsd/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/email.py` & `aprsd-3.1.0/aprsd/plugins/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,15 +662,15 @@
                     except Exception:
                         LOG.exception("Couldn't remove seen flag from email")
 
                     # check email more often since we just received an email
                     EmailInfo().delay = 60
 
             # reset clock
-            LOG.debug("Done looping over Server.fetch, logging out.")
+            LOG.debug("Done looping over Server.fetch, log out.")
             self.past = datetime.datetime.now()
             try:
                 server.logout()
             except Exception:
                 LOG.exception("IMAP failed to logout: ")
                 return True
         else:
```

### Comparing `aprsd-3.0.3/aprsd/plugins/fortune.py` & `aprsd-3.1.0/aprsd/plugins/fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/location.py` & `aprsd-3.1.0/aprsd/plugins/location.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import re
 import time
 
+from geopy.geocoders import Nominatim
 from oslo_config import cfg
 
 from aprsd import packets, plugin, plugin_utils
 from aprsd.utils import trace
 
 
 CONF = cfg.CONF
@@ -46,41 +47,51 @@
             return "Failed to fetch aprs.fi location"
 
         LOG.debug(f"LocationPlugin: aprs_data = {aprs_data}")
         if not len(aprs_data["entries"]):
             LOG.error("Didn't get any entries from aprs.fi")
             return "Failed to fetch aprs.fi location"
 
-        lat = aprs_data["entries"][0]["lat"]
-        lon = aprs_data["entries"][0]["lng"]
+        lat = float(aprs_data["entries"][0]["lat"])
+        lon = float(aprs_data["entries"][0]["lng"])
+
+        # Get some information about their location
+        try:
+            tic = time.perf_counter()
+            geolocator = Nominatim(user_agent="APRSD")
+            coordinates = f"{lat:0.6f}, {lon:0.6f}"
+            location = geolocator.reverse(coordinates)
+            address = location.raw.get("address")
+            toc = time.perf_counter()
+            if address:
+                LOG.info(f"Geopy address {address} took {toc - tic:0.4f}")
+            if address.get("country_code") == "us":
+                area_info = f"{address.get('county')}, {address.get('state')}"
+            else:
+                # what to do for address for non US?
+                area_info = f"{address.get('country'), 'Unknown'}"
+        except Exception as ex:
+            LOG.error(f"Failed to fetch Geopy address {ex}")
+            area_info = "Unknown Location"
+
         try:  # altitude not always provided
             alt = float(aprs_data["entries"][0]["altitude"])
         except Exception:
             alt = 0
         altfeet = int(alt * 3.28084)
         aprs_lasttime_seconds = aprs_data["entries"][0]["lasttime"]
         # aprs_lasttime_seconds = aprs_lasttime_seconds.encode(
         #    "ascii", errors="ignore"
         # )  # unicode to ascii
         delta_seconds = time.time() - int(aprs_lasttime_seconds)
         delta_hours = delta_seconds / 60 / 60
 
-        try:
-            wx_data = plugin_utils.get_weather_gov_for_gps(lat, lon)
-        except Exception as ex:
-            LOG.error(f"Couldn't fetch forecast.weather.gov '{ex}'")
-            wx_data = {"location": {"areaDescription": "Unknown Location"}}
-
-        if "location" not in wx_data:
-            LOG.error(f"Couldn't fetch forecast.weather.gov '{wx_data}'")
-            wx_data = {"location": {"areaDescription": "Unknown Location"}}
-
         reply = "{}: {} {}' {},{} {}h ago".format(
             searchcall,
-            wx_data["location"]["areaDescription"],
+            area_info,
             str(altfeet),
-            str(lat),
-            str(lon),
+            f"{lat:0.2f}",
+            f"{lon:0.2f}",
             str("%.1f" % round(delta_hours, 1)),
         ).rstrip()
 
         return reply
```

### Comparing `aprsd-3.0.3/aprsd/plugins/notify.py` & `aprsd-3.1.0/aprsd/plugins/notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/ping.py` & `aprsd-3.1.0/aprsd/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/query.py` & `aprsd-3.1.0/aprsd/plugins/query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/time.py` & `aprsd-3.1.0/aprsd/plugins/time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/version.py` & `aprsd-3.1.0/aprsd/plugins/version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/plugins/weather.py` & `aprsd-3.1.0/aprsd/plugins/weather.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     This service does not require an apiKey.
 
     How to Call: Send a message to aprsd
     "weather" - returns weather near the calling callsign
     """
 
-    command_regex = r"^([w]|[w]\s|[w][x]|[w][x]\s|weather)"
+    command_regex = r"^([w][x]|[w][x]\s|weather)"
     command_name = "USWeather"
     short_description = "Provide USA only weather of GPS Beacon location"
 
     def setup(self):
         self.ensure_aprs_fi_key()
 
     @trace.trace
@@ -88,15 +88,15 @@
 
     How to Call: Send a message to aprsd
     "metar" - returns metar report near the calling callsign
     "metar CALLSIGN" - returns metar report near CALLSIGN
 
     """
 
-    command_regex = r"^([m]|[m]|[m]\s|metar)"
+    command_regex = r"^([m]|[M]|[m]\s|metar)"
     command_name = "USMetar"
     short_description = "USA only METAR of GPS Beacon location"
 
     def setup(self):
         self.ensure_aprs_fi_key()
 
     @trace.trace
@@ -178,15 +178,15 @@
     To use this plugin you need to get an openweathermap
     account and apikey.
 
     https://home.openweathermap.org/api_keys
 
     """
 
-    command_regex = r"^([w]|[w]\s|[w][x]|[w][x]\s|weather)"
+    command_regex = r"^([w][x]|[w][x]\s|weather)"
     command_name = "OpenWeatherMap"
     short_description = "OpenWeatherMap weather of GPS Beacon location"
 
     def setup(self):
         if not CONF.owm_weather_plugin.apiKey:
             LOG.error("Config.owm_weather_plugin.apiKey is not set.  Disabling")
             self.enabled = False
```

### Comparing `aprsd-3.0.3/aprsd/rpc/client.py` & `aprsd-3.1.0/aprsd/rpc/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,56 +12,71 @@
 LOG = logging.getLogger("APRSD")
 
 
 class RPCClient:
     _instance = None
     _rpc_client = None
 
+    ip = None
+    port = None
+    magic_word = None
+
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
-    def __init__(self):
+    def __init__(self, ip=None, port=None, magic_word=None):
+        if ip:
+            self.ip = ip
+        else:
+            self.ip = CONF.rpc_settings.ip
+        if port:
+            self.port = int(port)
+        else:
+            self.port = CONF.rpc_settings.port
+        if magic_word:
+            self.magic_word = magic_word
+        else:
+            self.magic_word = CONF.rpc_settings.magic_word
         self._check_settings()
         self.get_rpc_client()
 
     def _check_settings(self):
         if not CONF.rpc_settings.enabled:
-            LOG.error("RPC is not enabled, no way to get stats!!")
+            LOG.warning("RPC is not enabled, no way to get stats!!")
 
-        if CONF.rpc_settings.magic_word == conf.common.APRSD_DEFAULT_MAGIC_WORD:
+        if self.magic_word == conf.common.APRSD_DEFAULT_MAGIC_WORD:
             LOG.warning("You are using the default RPC magic word!!!")
             LOG.warning("edit aprsd.conf and change rpc_settings.magic_word")
 
+        LOG.debug(f"RPC Client: {self.ip}:{self.port} {self.magic_word}")
+
     def _rpyc_connect(
-        self, host, port,
-        service=rpyc.VoidService,
-        config={}, ipv6=False,
-        keepalive=False, authorizer=None,
-    ):
+            self, host, port, service=rpyc.VoidService,
+            config={}, ipv6=False,
+            keepalive=False, authorizer=None, ):
 
-        print(f"Connecting to RPC host {host}:{port}")
+        LOG.info(f"Connecting to RPC host '{host}:{port}'")
         try:
             s = rpc.AuthSocketStream.connect(
                 host, port, ipv6=ipv6, keepalive=keepalive,
                 authorizer=authorizer,
             )
             return rpyc.utils.factory.connect_stream(s, service, config=config)
         except ConnectionRefusedError:
-            LOG.error(f"Failed to connect to RPC host {host}")
+            LOG.error(f"Failed to connect to RPC host '{host}:{port}'")
             return None
 
     def get_rpc_client(self):
         if not self._rpc_client:
-            magic = CONF.rpc_settings.magic_word
             self._rpc_client = self._rpyc_connect(
-                CONF.rpc_settings.ip,
-                CONF.rpc_settings.port,
-                authorizer=lambda sock: sock.send(magic.encode()),
+                self.ip,
+                self.port,
+                authorizer=lambda sock: sock.send(self.magic_word.encode()),
             )
         return self._rpc_client
 
     def get_stats_dict(self):
         cl = self.get_rpc_client()
         result = {}
         if not cl:
```

### Comparing `aprsd-3.0.3/aprsd/rpc/server.py` & `aprsd-3.1.0/aprsd/rpc/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,36 +56,44 @@
         # code that runs after the connection has already closed
         # (to finalize the service, if needed)
         LOG.info("Disconnected")
         self._conn = None
 
     @rpyc.exposed
     def get_stats(self):
+        LOG.info("get_stats")
         stat = stats.APRSDStats()
         stats_dict = stat.stats()
-        LOG.debug(stats_dict)
-        return json.dumps(stats_dict, indent=4, sort_keys=True, default=str)
+        return_str = json.dumps(stats_dict, indent=4, sort_keys=True, default=str)
+        LOG.info(f"get_stats: return size {len(return_str)}")
+        return return_str
 
     @rpyc.exposed
     def get_stats_obj(self):
+        LOG.info("get_stats_obj")
         return stats.APRSDStats()
 
     @rpyc.exposed
     def get_packet_list(self):
+        LOG.info("get_packet_list")
         return packets.PacketList()
 
     @rpyc.exposed
     def get_packet_track(self):
+        LOG.info("get_packet_track")
         return packets.PacketTrack()
 
     @rpyc.exposed
     def get_watch_list(self):
+        LOG.info("get_watch_list")
         return packets.WatchList()
 
     @rpyc.exposed
     def get_seen_list(self):
+        LOG.info("get_seen_list")
         return packets.SeenList()
 
     @rpyc.exposed
     def get_log_entries(self):
+        LOG.info("get_log_entries")
         entries = log_monitor.LogEntries().get_all_and_purge()
         return json.dumps(entries, default=str)
```

### Comparing `aprsd-3.0.3/aprsd/stats.py` & `aprsd-3.1.0/aprsd/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     _email_thread_last_time = None
     _email_tx = 0
     _email_rx = 0
 
     _mem_current = 0
     _mem_peak = 0
 
+    _thread_info = {}
+
     _pkt_cnt = {
         "Packet": {
             "tx": 0,
             "rx": 0,
         },
         "AckPacket": {
             "tx": 0,
@@ -92,14 +94,23 @@
         return self._mem_peak
 
     @wrapt.synchronized(lock)
     def set_memory_peak(self, memory):
         self._mem_peak = memory
 
     @wrapt.synchronized(lock)
+    def set_thread_info(self, thread_info):
+        self._thread_info = thread_info
+
+    @wrapt.synchronized(lock)
+    @property
+    def thread_info(self):
+        return self._thread_info
+
+    @wrapt.synchronized(lock)
     @property
     def aprsis_server(self):
         return self._aprsis_server
 
     @wrapt.synchronized(lock)
     def set_aprsis_server(self, server):
         self._aprsis_server = server
@@ -203,26 +214,28 @@
                 "version": aprsd.__version__,
                 "uptime": utils.strfdelta(self.uptime),
                 "callsign": CONF.callsign,
                 "memory_current": int(self.memory),
                 "memory_current_str": utils.human_size(self.memory),
                 "memory_peak": int(self.memory_peak),
                 "memory_peak_str": utils.human_size(self.memory_peak),
+                "threads": self._thread_info,
                 "watch_list": wl.get_all(),
                 "seen_list": sl.get_all(),
             },
             "aprs-is": {
                 "server": str(self.aprsis_server),
                 "callsign": CONF.aprs_network.login,
                 "last_update": last_aprsis_keepalive,
             },
             "packets": {
-                "tracked": int(pl.total_tx() + pl.total_rx()),
-                "sent": int(pl.total_tx()),
-                "received": int(pl.total_rx()),
+                "total_tracked": int(pl.total_tx() + pl.total_rx()),
+                "total_sent": int(pl.total_tx()),
+                "total_received": int(pl.total_rx()),
+                "by_type": self._pkt_cnt,
             },
             "messages": {
                 "sent": self._pkt_cnt["MessagePacket"]["tx"],
                 "received": self._pkt_cnt["MessagePacket"]["tx"],
                 "ack_sent": self._pkt_cnt["AckPacket"]["tx"],
             },
             "email": {
@@ -230,14 +243,15 @@
                 "sent": int(self._email_tx),
                 "received": int(self._email_rx),
                 "thread_last_update": last_update,
             },
             "plugins": plugin_stats,
         }
         LOG.debug(f"STATS = {stats}")
+        LOG.info("APRSD Stats: DONE")
         return stats
 
     def __str__(self):
         pl = packets.PacketList()
         return (
             "Uptime:{} Msgs TX:{} RX:{} "
             "ACK: TX:{} RX:{} "
```

### Comparing `aprsd-3.0.3/aprsd/threads/aprsd.py` & `aprsd-3.1.0/aprsd/threads/aprsd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import datetime
 import logging
 import threading
 
 import wrapt
 
 
 LOG = logging.getLogger("APRSD")
@@ -46,14 +47,15 @@
 
 class APRSDThread(threading.Thread, metaclass=abc.ABCMeta):
 
     def __init__(self, name):
         super().__init__(name=name)
         self.thread_stop = False
         APRSDThreadList().add(self)
+        self._last_loop = datetime.datetime.now()
 
     def _should_quit(self):
         """ see if we have a quit message from the global queue."""
         if self.thread_stop:
             return True
 
     def stop(self):
@@ -66,16 +68,21 @@
     def _cleanup(self):
         """Add code to subclass to do any cleanup"""
 
     def __str__(self):
         out = f"Thread <{self.__class__.__name__}({self.name}) Alive? {self.is_alive()}>"
         return out
 
+    def loop_age(self):
+        """How old is the last loop call?"""
+        return datetime.datetime.now() - self._last_loop
+
     def run(self):
         LOG.debug("Starting")
         while not self._should_quit():
             can_loop = self.loop()
+            self._last_loop = datetime.datetime.now()
             if not can_loop:
                 self.stop()
         self._cleanup()
         APRSDThreadList().remove(self)
         LOG.debug("Exiting")
```

### Comparing `aprsd-3.0.3/aprsd/threads/log_monitor.py` & `aprsd-3.1.0/aprsd/threads/log_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import threading
 
 import wrapt
 
 from aprsd import threads
-from aprsd.logging import log
+from aprsd.log import log
 
 
 LOG = logging.getLogger("APRSD")
 
 
 class LogEntries:
     entries = []
```

### Comparing `aprsd-3.0.3/aprsd/threads/rx.py` & `aprsd-3.1.0/aprsd/threads/rx.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/threads/tx.py` & `aprsd-3.1.0/aprsd/threads/tx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 import datetime
 import logging
 import time
 
 from oslo_config import cfg
-from ratelimiter import RateLimiter
+from rush import quota, throttle
+from rush.contrib import decorator
+from rush.limiters import periodic
+from rush.stores import dictionary
 
 from aprsd import client
+from aprsd import conf  # noqa
 from aprsd import threads as aprsd_threads
 from aprsd.packets import core, tracker
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
+msg_t = throttle.Throttle(
+    limiter=periodic.PeriodicLimiter(
+        store=dictionary.DictionaryStore(),
+    ),
+    rate=quota.Quota.per_second(
+        count=CONF.msg_rate_limit_period,
+    ),
+)
+ack_t = throttle.Throttle(
+    limiter=periodic.PeriodicLimiter(
+        store=dictionary.DictionaryStore(),
+    ),
+    rate=quota.Quota.per_second(
+        count=CONF.ack_rate_limit_period,
+    ),
+)
 
-def limited(until):
-    duration = int(round(until - time.time()))
-    LOG.debug(f"Rate limited, sleeping for {duration:d} seconds")
+msg_throttle_decorator = decorator.ThrottleDecorator(throttle=msg_t)
+ack_throttle_decorator = decorator.ThrottleDecorator(throttle=ack_t)
 
 
 def send(packet: core.Packet, direct=False, aprs_client=None):
     """Send a packet either in a thread or directly to the client."""
     # prepare the packet for sending.
     # This constructs the packet.raw
     packet.prepare()
     if isinstance(packet, core.AckPacket):
         _send_ack(packet, direct=direct, aprs_client=aprs_client)
     else:
         _send_packet(packet, direct=direct, aprs_client=aprs_client)
 
 
-@RateLimiter(max_calls=1, period=CONF.msg_rate_limit_period, callback=limited)
+@msg_throttle_decorator.sleep_and_retry
 def _send_packet(packet: core.Packet, direct=False, aprs_client=None):
     if not direct:
         thread = SendPacketThread(packet=packet)
         thread.start()
     else:
         _send_direct(packet, aprs_client=aprs_client)
 
 
-@RateLimiter(max_calls=1, period=CONF.ack_rate_limit_period, callback=limited)
+@ack_throttle_decorator.sleep_and_retry
 def _send_ack(packet: core.AckPacket, direct=False, aprs_client=None):
     if not direct:
         thread = SendAckThread(packet=packet)
         thread.start()
     else:
         _send_direct(packet, aprs_client=aprs_client)
```

### Comparing `aprsd-3.0.3/aprsd/utils/__init__.py` & `aprsd-3.1.0/aprsd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/counter.py` & `aprsd-3.1.0/aprsd/utils/counter.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/fuzzyclock.py` & `aprsd-3.1.0/aprsd/utils/fuzzyclock.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/json.py` & `aprsd-3.1.0/aprsd/utils/json.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/objectstore.py` & `aprsd-3.1.0/aprsd/utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/ring_buffer.py` & `aprsd-3.1.0/aprsd/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/utils/trace.py` & `aprsd-3.1.0/aprsd/utils/trace.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/css/index.css` & `aprsd-3.1.0/aprsd/web/admin/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/css/prism.css` & `aprsd-3.1.0/aprsd/web/admin/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/css/tabs.css` & `aprsd-3.1.0/aprsd/web/admin/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/Untitled.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png` & `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/charts.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/logs.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/logs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/main.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/prism.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/send-message.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/js/tabs.js` & `aprsd-3.1.0/aprsd/web/admin/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/admin/templates/index.html` & `aprsd-3.1.0/aprsd/web/admin/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <html>
     <head>
         <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
         <link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/jqueryui/1.12.1/themes/smoothness/jquery-ui.css">
         <script src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.12.1/jquery-ui.min.js"></script>
-        <script src="https://cdn.socket.io/4.1.2/socket.io.min.js" integrity="sha384-toS6mmwu70G0fw54EGlWWeA4z3dyJ+dlXBtSURSKN4vyRFOcxd3Bzjj/AoOwY+Rg" crossorigin="anonymous"></script>
+        <script src="https://cdn.socket.io/4.7.1/socket.io.min.js" integrity="sha512-+NaO7d6gQ1YPxvc/qHIqZEchjGm207SszoNeMgppoqD/67fEqmc1edS8zrbxPD+4RQI3gDgT/83ihpFW61TG/Q==" crossorigin="anonymous"></script>
 
         <script src="https://cdn.jsdelivr.net/npm/chart.js@2.9.4/dist/Chart.bundle.js"></script>
 
         <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/semantic-ui@2.4.2/dist/semantic.min.css">
         <script src="https://cdn.jsdelivr.net/npm/semantic-ui@2.4.2/dist/semantic.min.js"></script>
 
         <link rel="stylesheet" href="/static/css/index.css">
```

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/css/index.css` & `aprsd-3.1.0/aprsd/web/chat/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/css/style.css.map` & `aprsd-3.1.0/aprsd/web/chat/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/css/tabs.css` & `aprsd-3.1.0/aprsd/web/chat/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/Untitled.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png` & `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/js/gps.js` & `aprsd-3.1.0/aprsd/web/chat/static/js/gps.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/js/main.js` & `aprsd-3.1.0/aprsd/web/chat/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/js/send-message-mobile.js` & `aprsd-3.1.0/aprsd/web/chat/static/js/send-message-mobile.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/js/send-message.js` & `aprsd-3.1.0/aprsd/web/chat/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/js/tabs.js` & `aprsd-3.1.0/aprsd/web/chat/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/templates/index.html` & `aprsd-3.1.0/aprsd/web/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd/web/chat/templates/mobile.html` & `aprsd-3.1.0/aprsd/web/chat/templates/mobile.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd-lnav.json` & `aprsd-3.1.0/aprsd-lnav.json`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/aprsd.egg-info/PKG-INFO` & `aprsd-3.1.0/aprsd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.0.3
+Version: 3.1.0
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
@@ -306,14 +306,28 @@
     To          : KM6XXX-6
     Ack         : 2
     Sending ack _______________ Complete
 
 AND... ping, fortune, time.....
 
 
+Web Admin Interface
+===================
+To start the web admin interface, You have to install gunicorn in your virtualenv that already has aprsd installed.
+
+::
+
+  source <path to APRSD's virtualenv>/bin/activate
+  pip install gunicorn
+  gunicorn --bind 0.0.0.0:8080 "aprsd.wsgi:app"
+
+The web admin interface will be running on port 8080 on the local machine.  http://localhost:8080
+
+
+
 Development
 ===========
 
 * ``git clone git@github.com:craigerl/aprsd.git``
 * ``cd aprsd``
 * ``make``
```

### Comparing `aprsd-3.0.3/aprsd.egg-info/SOURCES.txt` & `aprsd-3.1.0/aprsd.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS
 ChangeLog
 INSTALL.txt
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
@@ -13,57 +14,60 @@
 gray.conf
 pyproject.toml
 requirements.in
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/manual_build.yml
 .github/workflows/master-build.yml
 .github/workflows/python.yml
 .github/workflows/release_build.yml
 aprsd/__init__.py
-aprsd/aprsd.py
+aprsd/admin_web.py
 aprsd/cli_helper.py
 aprsd/client.py
 aprsd/exception.py
-aprsd/flask.py
+aprsd/main.py
 aprsd/messaging.py
 aprsd/plugin.py
 aprsd/plugin_utils.py
 aprsd/stats.py
+aprsd/wsgi.py
 aprsd.egg-info/PKG-INFO
 aprsd.egg-info/SOURCES.txt
 aprsd.egg-info/dependency_links.txt
 aprsd.egg-info/entry_points.txt
 aprsd.egg-info/not-zip-safe
 aprsd.egg-info/pbr.json
 aprsd.egg-info/requires.txt
 aprsd.egg-info/top_level.txt
 aprsd/clients/__init__.py
 aprsd/clients/aprsis.py
 aprsd/clients/kiss.py
 aprsd/cmds/__init__.py
 aprsd/cmds/completion.py
 aprsd/cmds/dev.py
+aprsd/cmds/fetch_stats.py
 aprsd/cmds/healthcheck.py
 aprsd/cmds/list_plugins.py
 aprsd/cmds/listen.py
 aprsd/cmds/send_message.py
 aprsd/cmds/server.py
 aprsd/cmds/webchat.py
 aprsd/conf/__init__.py
 aprsd/conf/client.py
 aprsd/conf/common.py
 aprsd/conf/log.py
 aprsd/conf/opts.py
 aprsd/conf/plugin_common.py
 aprsd/conf/plugin_email.py
-aprsd/logging/__init__.py
-aprsd/logging/log.py
-aprsd/logging/rich.py
+aprsd/log/__init__.py
+aprsd/log/log.py
+aprsd/log/rich.py
 aprsd/packets/__init__.py
 aprsd/packets/core.py
 aprsd/packets/packet_list.py
 aprsd/packets/seen_list.py
 aprsd/packets/tracker.py
 aprsd/packets/watch_list.py
 aprsd/plugins/__init__.py
@@ -130,14 +134,15 @@
 aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
 aprsd/web/chat/templates/index.html
 aprsd/web/chat/templates/mobile.html
 docker/Dockerfile
 docker/Dockerfile-dev
 docker/build.sh
 docker/docker-compose.yml
+docker/bin/admin.sh
 docker/bin/listen.sh
 docker/bin/run.sh
 docs/aprsd.drawio
 docs/changelog.rst
 docs/clean_docs.py
 docs/conf.py
 docs/configure.rst
```

### Comparing `aprsd-3.0.3/aprsd.egg-info/requires.txt` & `aprsd-3.1.0/aprsd.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,76 @@
+anyio==3.7.1
 aprslib==0.7.2
-attrs==22.2.0
+attrs==23.1.0
 ax253==0.1.5.post1
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
 bidict==0.22.1
-bitarray==2.6.2
-certifi==2022.12.7
+bitarray==2.8.0
+blinker==1.6.2
+certifi==2023.7.22
 cffi==1.15.1
-charset-normalizer==3.0.1
-click==8.1.3
+charset-normalizer==3.2.0
+click==8.1.6
 click-completion==0.5.2
+click-params==0.4.1
 commonmark==0.9.1
-cryptography==38.0.1
+cryptography==41.0.2
 dacite2==2.0.0
 dataclasses==0.6
 debtcollector==2.5.0
-dnspython==2.3.0
+decorator==5.1.1
+dnspython==2.4.0
 eventlet==0.33.3
-flask==2.1.2
-flask-classful==0.14.2
-flask-httpauth==4.7.0
-flask-socketio==5.3.2
-greenlet==2.0.1
+exceptiongroup==1.1.2
+flask==2.3.2
+flask-httpauth==4.8.0
+flask-socketio==5.3.4
+geographiclib==2.0
+geopy==2.3.0
+gevent==23.7.0
+greenlet==2.0.2
+h11==0.14.0
+httpcore==0.17.3
 idna==3.4
 imapclient==2.3.1
-importlib-metadata==6.0.0
+importlib-metadata==6.8.0
 itsdangerous==2.1.2
 jinja2==3.1.2
 kiss3==8.0.0
-markupsafe==2.1.2
+markupsafe==2.1.3
 netaddr==0.8.0
-oslo-config==9.1.0
-oslo-i18n==5.1.0
+oslo-config==9.1.1
+oslo-i18n==6.0.0
 pbr==5.11.1
-pluggy==1.0.0
-plumbum==1.8.1
+pluggy==1.2.0
+plumbum==1.8.2
 pycparser==2.21
-pygments==2.14.0
-pyopenssl==23.0.0
+pygments==2.15.1
+pyopenssl==23.2.0
 pyserial==3.5
 pyserial-asyncio==0.6
-python-engineio==4.3.4
-python-socketio==5.7.2
-pytz==2022.7.1
-pyyaml==6.0
-ratelimiter==1.2.0.post0
-requests==2.28.2
+python-engineio==4.5.1
+python-socketio==5.8.0
+pytz==2023.3
+pyyaml==6.0.1
+requests==2.31.0
 rfc3986==2.0.0
 rich==12.6.0
-rpyc==5.3.0
+rpyc==5.3.1
+rush==2021.4.0
 shellingham==1.5.0.post1
 six==1.16.0
-soupsieve==2.3.2.post1
-stevedore==4.1.1
+sniffio==1.3.0
+soupsieve==2.4.1
+stevedore==5.1.0
 tabulate==0.9.0
 thesmuggler==1.0.1
-ua-parser==0.16.1
+ua-parser==0.18.0
 update-checker==0.18.0
-urllib3==1.26.14
+urllib3==2.0.4
 user-agents==2.2.0
-werkzeug==2.1.2
-wrapt==1.14.1
-zipp==3.11.0
+validators==0.20.0
+werkzeug==2.3.6
+wrapt==1.15.0
+zipp==3.16.2
+zope-event==5.0
+zope-interface==6.0
```

### Comparing `aprsd-3.0.3/dev-requirements.txt` & `aprsd-3.1.0/dev-requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --annotation-style=line --resolver=backtracking dev-requirements.in
+#    pip-compile --annotation-style=line dev-requirements.in
 #
-add-trailing-comma==2.4.0  # via gray
+add-trailing-comma==3.0.0  # via gray
 alabaster==0.7.13         # via sphinx
-attrs==22.2.0             # via jsonschema, pytest
+attrs==23.1.0             # via jsonschema, referencing
 autoflake==1.5.3          # via gray
-babel==2.11.0             # via sphinx
-black==22.12.0            # via gray
+babel==2.12.1             # via sphinx
+black==23.7.0             # via gray
 build==0.10.0             # via pip-tools
-cachetools==5.2.1         # via tox
-certifi==2022.12.7        # via requests
+cachetools==5.3.1         # via tox
+certifi==2023.7.22        # via requests
 cfgv==3.3.1               # via pre-commit
 chardet==5.1.0            # via tox
-charset-normalizer==3.0.1  # via requests
-click==8.1.3              # via black, pip-tools
+charset-normalizer==3.2.0  # via requests
+click==8.1.6              # via black, pip-tools
 colorama==0.4.6           # via tox
 commonmark==0.9.1         # via rich
-configargparse==1.5.3     # via gray
-coverage[toml]==7.0.5     # via pytest-cov
-distlib==0.3.6            # via virtualenv
-docutils==0.19            # via sphinx
-exceptiongroup==1.1.0     # via pytest
-filelock==3.9.0           # via tox, virtualenv
+configargparse==1.7       # via gray
+coverage[toml]==7.2.7     # via pytest-cov
+distlib==0.3.7            # via virtualenv
+docutils==0.20.1          # via sphinx
+exceptiongroup==1.1.2     # via pytest
+filelock==3.12.2          # via tox, virtualenv
 fixit==0.1.4              # via gray
 flake8==6.0.0             # via -r dev-requirements.in, fixit, pep8-naming
 gray==0.13.0              # via -r dev-requirements.in
-identify==2.5.13          # via pre-commit
+identify==2.5.26          # via pre-commit
 idna==3.4                 # via requests
 imagesize==1.4.1          # via sphinx
-importlib-metadata==6.0.0  # via sphinx
-importlib-resources==5.10.2  # via fixit
+importlib-resources==6.0.0  # via fixit
 iniconfig==2.0.0          # via pytest
-isort==5.11.4             # via -r dev-requirements.in, gray
+isort==5.12.0             # via -r dev-requirements.in, gray
 jinja2==3.1.2             # via sphinx
-jsonschema==4.17.3        # via fixit
-libcst==0.4.9             # via fixit
-markupsafe==2.1.2         # via jinja2
+jsonschema==4.18.4        # via fixit
+jsonschema-specifications==2023.7.1  # via jsonschema
+libcst==1.0.1             # via fixit
+markupsafe==2.1.3         # via jinja2
 mccabe==0.7.0             # via flake8
-mypy==0.991               # via -r dev-requirements.in
-mypy-extensions==0.4.3    # via black, mypy, typing-inspect
-nodeenv==1.7.0            # via pre-commit
-packaging==23.0           # via build, pyproject-api, pytest, sphinx, tox
-pathspec==0.10.3          # via black
+mypy==1.4.1               # via -r dev-requirements.in
+mypy-extensions==1.0.0    # via black, mypy, typing-inspect
+nodeenv==1.8.0            # via pre-commit
+packaging==23.1           # via black, build, pyproject-api, pytest, sphinx, tox
+pathspec==0.11.1          # via black
 pep8-naming==0.13.3       # via -r dev-requirements.in
-pip-tools==6.12.1         # via -r dev-requirements.in
-platformdirs==2.6.2       # via black, tox, virtualenv
-pluggy==1.0.0             # via pytest, tox
-pre-commit==2.21.0        # via -r dev-requirements.in
+pip-tools==7.1.0          # via -r dev-requirements.in
+platformdirs==3.9.1       # via black, tox, virtualenv
+pluggy==1.2.0             # via pytest, tox
+pre-commit==3.3.3         # via -r dev-requirements.in
 pycodestyle==2.10.0       # via flake8
 pyflakes==3.0.1           # via autoflake, flake8
-pygments==2.14.0          # via rich, sphinx
-pyproject-api==1.5.0      # via tox
+pygments==2.15.1          # via rich, sphinx
+pyproject-api==1.5.3      # via tox
 pyproject-hooks==1.0.0    # via build
-pyrsistent==0.19.3        # via jsonschema
-pytest==7.2.1             # via -r dev-requirements.in, pytest-cov
-pytest-cov==4.0.0         # via -r dev-requirements.in
-pytz==2022.7.1            # via babel
-pyupgrade==3.3.1          # via gray
-pyyaml==6.0               # via fixit, libcst, pre-commit
-requests==2.28.2          # via sphinx
+pytest==7.4.0             # via -r dev-requirements.in, pytest-cov
+pytest-cov==4.1.0         # via -r dev-requirements.in
+pyupgrade==3.9.0          # via gray
+pyyaml==6.0.1             # via fixit, libcst, pre-commit
+referencing==0.30.0       # via jsonschema, jsonschema-specifications
+requests==2.31.0          # via sphinx
 rich==12.6.0              # via gray
+rpds-py==0.9.2            # via jsonschema, referencing
 snowballstemmer==2.2.0    # via sphinx
-sphinx==6.1.3             # via -r dev-requirements.in
-sphinxcontrib-applehelp==1.0.3  # via sphinx
+sphinx==7.0.1             # via -r dev-requirements.in
+sphinxcontrib-applehelp==1.0.4  # via sphinx
 sphinxcontrib-devhelp==1.0.2  # via sphinx
-sphinxcontrib-htmlhelp==2.0.0  # via sphinx
+sphinxcontrib-htmlhelp==2.0.1  # via sphinx
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.3  # via sphinx
 sphinxcontrib-serializinghtml==1.1.5  # via sphinx
-tokenize-rt==5.0.0        # via add-trailing-comma, pyupgrade
+tokenize-rt==5.1.0        # via add-trailing-comma, pyupgrade
 toml==0.10.2              # via autoflake
-tomli==2.0.1              # via black, build, coverage, mypy, pyproject-api, pyproject-hooks, pytest, tox
-tox==4.3.5                # via -r dev-requirements.in
-typing-extensions==4.4.0  # via black, libcst, mypy, typing-inspect
-typing-inspect==0.8.0     # via libcst
+tomli==2.0.1              # via black, build, coverage, mypy, pip-tools, pyproject-api, pyproject-hooks, pytest, tox
+tox==4.6.4                # via -r dev-requirements.in
+typing-extensions==4.7.1  # via libcst, mypy, typing-inspect
+typing-inspect==0.9.0     # via libcst
 unify==0.5                # via gray
 untokenize==0.1.1         # via unify
-urllib3==1.26.14          # via requests
-virtualenv==20.17.1       # via pre-commit, tox
-wheel==0.38.4             # via pip-tools
-zipp==3.11.0              # via importlib-metadata, importlib-resources
+urllib3==2.0.4            # via requests
+virtualenv==20.24.1       # via pre-commit, tox
+wheel==0.41.0             # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `aprsd-3.0.3/docker/Dockerfile` & `aprsd-3.1.0/docker/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 FROM ubuntu:22.04 as aprsd
 
 # Dockerfile for building a container during aprsd development.
 
 ARG UID
 ARG GID
 ARG TZ
-ARG VERSION=3.0.0
+ARG VERSION=3.0.3
 ARG BUILDX_QEMU_ENV
 ENV APRS_USER=aprs
 ENV HOME=/home/aprs
 ENV TZ=${TZ:-US/Eastern}
 ENV UID=${UID:-1000}
 ENV GID=${GID:-1000}
 ENV LC_ALL=C.UTF-8
@@ -18,17 +18,20 @@
 ENV APRSD_PIP_VERSION=${VERSION}
 
 
 ENV DEBIAN_FRONTEND=noninteractive
 RUN apt update
 RUN apt install -y git build-essential
 RUN apt install -y libffi-dev python3-dev libssl-dev libxml2-dev libxslt-dev
-RUN apt install -y python3 python3-pip python3-dev python3-lxml
+RUN apt install -y python3 python3-pip python3-dev python3-lxml python3-setuptools-rust
+RUN apt install -y libffi-dev cargo pkg-config
 
 RUN pip3 install -U pip
+RUN pip3 install -U setuptools_rust
+
 
 RUN addgroup --gid $GID $APRS_USER
 RUN useradd -m -u $UID -g $APRS_USER $APRS_USER
 
 # Handle an extremely specific issue when building the cryptography package for
 # 32-bit architectures within QEMU running on a 64-bit host (issue #30).
 RUN if [ "${BUILDX_QEMU_ENV}" = "true" -a "$(getconf LONG_BIT)" = "32" ]; then \
```

### Comparing `aprsd-3.0.3/docker/bin/listen.sh` & `aprsd-3.1.0/docker/bin/listen.sh`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     OLDIFS=$IFS
     IFS=','
     echo "Installing pypi plugins '$APRSD_PLUGINS'";
     for plugin in ${APRSD_PLUGINS}; do
         IFS=$OLDIFS
         # call your procedure/other scripts here below
         echo "Installing '$plugin'"
-        pip3 install $plugin
+        pip3 install --user $plugin
     done
 fi
 
 if [ -z "${LOG_LEVEL}" ] || [[ ! "${LOG_LEVEL}" =~ ^(CRITICAL|ERROR|WARNING|INFO)$ ]]; then
     LOG_LEVEL="DEBUG"
 fi
```

### Comparing `aprsd-3.0.3/docker/bin/run.sh` & `aprsd-3.1.0/docker/bin/run.sh`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     OLDIFS=$IFS
     IFS=','
     echo "Installing pypi plugins '$APRSD_PLUGINS'";
     for plugin in ${APRSD_PLUGINS}; do
         IFS=$OLDIFS
         # call your procedure/other scripts here below
         echo "Installing '$plugin'"
-        pip3 install $plugin
+        pip3 install --user $plugin
     done
 fi
 
 if [ -z "${LOG_LEVEL}" ] || [[ ! "${LOG_LEVEL}" =~ ^(CRITICAL|ERROR|WARNING|INFO)$ ]]; then
     LOG_LEVEL="DEBUG"
 fi
```

### Comparing `aprsd-3.0.3/docker/build.sh` & `aprsd-3.1.0/docker/build.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/_static/aprsd_overview.png` & `aprsd-3.1.0/docs/_static/aprsd_overview.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/_static/aprsd_overview.svg` & `aprsd-3.1.0/docs/_static/aprsd_overview.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.cmds.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.cmds.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.conf.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.conf.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.packets.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.packets.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.plugins.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.plugins.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.threads.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.threads.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/apidoc/aprsd.utils.rst` & `aprsd-3.1.0/docs/apidoc/aprsd.utils.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/aprsd.drawio` & `aprsd-3.1.0/docs/aprsd.drawio`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/changelog.rst` & `aprsd-3.1.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,110 @@
 CHANGES
 =======
 
+v3.1.0
+------
+
+* Changelog updates for v3.1.0
+* Use CONF.admin.web\_port for single launch web admin
+* Fixed sio namespace registration
+* Update Dockerfile-dev to include uwsgi
+* Fixed pep8
+* change port to 8000
+* replacement of flask-socketio with python-socketio
+* Change how fetch-stats gets it's defaults
+* Ensure fetch-stats ip is a string
+* Add info logging for rpc server calls
+* updated wsgi config default /config/aprsd.conf
+* Added timing after each thread loop
+* Update docker bin/admin.sh
+* Removed flask-classful from webchat
+* Remove flask pinning
+* removed linux/arm/v8
+* Update master build to include linux/arm/v8
+* Update Dockerfile-dev to fix plugin permissions
+* update manual build github
+* Update requirements for upgraded cryptography
+* Added more libs for Dockerfile-dev
+* Replace Dockerfile-dev with python3 slim
+* Moved logging to log for wsgi.py
+* Changed weather plugin regex pattern
+* Limit the float values to 3 decimal places
+* Fixed rain numbers from aprslib
+* Fixed rpc client initialization
+* Fix in for aprslib issue #80
+* Try and fix Dockerfile-dev
+* Fixed pep8 errors
+* Populate stats object with threads info
+* added counts to the fetch-stats table
+* Added the fetch-stats command
+* Replace ratelimiter with rush
+* Added some utilities to Dockerfile-dev
+* add arm64 for manual github build
+* Added manual master build
+* Update master-build.yml
+* Add github manual trigger for master build
+* Fixed unit tests for Location plugin
+* USe new tox and update githubworkflows
+* Updated requirements
+* force tox to 4.3.5
+* Update github workflows
+* Fixed pep8 violation
+* Added rpc server for listen
+* Update location plugin and reworked requirements
+* Fixed .readthedocs.yaml format
+* Add .readthedocs.yaml
+* Example plugin wrong function
+* Ensure conf is imported for threads/tx
+* Update Dockerfile to help build cryptography
+
+v3.0.3
+------
+
+* Update Changelog to 3.0.3
+* cleanup some debug messages
+* Fixed loading of plugins for server
+* Don't load help plugin for listen command
+* Added listen args
+* Change listen command plugins
+* Added listen.sh for docker
+* Update Listen command
+* Update Dockerfile
+* Add ratelimiting for acks and other packets
+
+v3.0.2
+------
+
+* Update Changelog for 3.0.2
+* Import RejectPacket
+
+v3.0.1
+------
+
+* 3.0.1
+* Add support to Reject messages
+* Update Docker builds for 3.0.0
+
+v3.0.0
+------
+
+* Update Changelog for 3.0.0
+* Ensure server command main thread doesn't exit
+* Fixed save directory default
+* Fixed pep8 failure
+* Cleaned up KISS interfaces use of old config
+* reworked usage of importlib.metadata
+* Added new docs files for 3.0.0
+* Removed url option from healthcheck in dev
+* Updated Healthcheck to use rpc to call aprsd
+* Updated docker/bin/run.sh to use new conf
+* Added ObjectPacket
+* Update regex processing and regex for plugins
+* Change ordering of starting up of server command
+* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.0.3/docs/clean_docs.py` & `aprsd-3.1.0/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/conf.py` & `aprsd-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/configure.rst` & `aprsd-3.1.0/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/index.rst` & `aprsd-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/install.rst` & `aprsd-3.1.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/links.rst` & `aprsd-3.1.0/docs/links.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/plugin.rst` & `aprsd-3.1.0/docs/plugin.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/docs/readme.rst` & `aprsd-3.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,28 @@
     To          : KM6XXX-6
     Ack         : 2
     Sending ack _______________ Complete
 
 AND... ping, fortune, time.....
 
 
+Web Admin Interface
+===================
+To start the web admin interface, You have to install gunicorn in your virtualenv that already has aprsd installed.
+
+::
+
+  source <path to APRSD's virtualenv>/bin/activate
+  pip install gunicorn
+  gunicorn --bind 0.0.0.0:8080 "aprsd.wsgi:app"
+
+The web admin interface will be running on port 8080 on the local machine.  http://localhost:8080
+
+
+
 Development
 ===========
 
 * ``git clone git@github.com:craigerl/aprsd.git``
 * ``cd aprsd``
 * ``make``
```

### Comparing `aprsd-3.0.3/docs/server.rst` & `aprsd-3.1.0/docs/server.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/pyproject.toml` & `aprsd-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/requirements.in` & `aprsd-3.1.0/requirements.in`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 aprslib>=0.7.0
 click
+click-params
 click-completion
-flask==2.1.2
-werkzeug==2.1.2
-flask-classful
+flask
+werkzeug
 flask-httpauth
 imapclient
 pluggy
 pbr
 pyyaml
 requests
 pytz
 six
 thesmuggler
 update_checker
 flask-socketio
+python-socketio
+gevent
 eventlet
 tabulate
 # Pinned due to gray needing 12.6.0
 rich==12.6.0
 # For the list-plugins pypi.org search scraping
 beautifulsoup4
 wrapt
@@ -30,10 +32,11 @@
 pyopenssl
 dataclasses
 dacite2
 oslo.config
 rpyc
 # Pin this here so it doesn't require a compile on
 # raspi
-cryptography==38.0.1
-shellingham==1.5.0.post1
-ratelimiter
+cryptography
+shellingham
+geopy
+rush
```

### Comparing `aprsd-3.0.3/requirements.txt` & `aprsd-3.1.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,85 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --annotation-style=line --resolver=backtracking requirements.in
+#    pip-compile --annotation-style=line requirements.in
 #
+anyio==3.7.1              # via httpcore
 aprslib==0.7.2            # via -r requirements.in
-attrs==22.2.0             # via -r requirements.in, ax253, kiss3
+attrs==23.1.0             # via -r requirements.in, ax253, kiss3, rush
 ax253==0.1.5.post1        # via kiss3
-beautifulsoup4==4.11.1    # via -r requirements.in
+beautifulsoup4==4.12.2    # via -r requirements.in
 bidict==0.22.1            # via python-socketio
-bitarray==2.6.2           # via ax253, kiss3
-certifi==2022.12.7        # via requests
+bitarray==2.8.0           # via ax253, kiss3
+blinker==1.6.2            # via flask
+certifi==2023.7.22        # via httpcore, requests
 cffi==1.15.1              # via cryptography
-charset-normalizer==3.0.1  # via requests
-click==8.1.3              # via -r requirements.in, click-completion, flask
+charset-normalizer==3.2.0  # via requests
+click==8.1.6              # via -r requirements.in, click-completion, click-params, flask
 click-completion==0.5.2   # via -r requirements.in
+click-params==0.4.1       # via -r requirements.in
 commonmark==0.9.1         # via rich
-cryptography==38.0.1      # via -r requirements.in, pyopenssl
+cryptography==41.0.2      # via -r requirements.in, pyopenssl
 dacite2==2.0.0            # via -r requirements.in
 dataclasses==0.6          # via -r requirements.in
 debtcollector==2.5.0      # via oslo-config
-dnspython==2.3.0          # via eventlet
+decorator==5.1.1          # via validators
+dnspython==2.4.0          # via eventlet
 eventlet==0.33.3          # via -r requirements.in
-flask==2.1.2              # via -r requirements.in, flask-classful, flask-httpauth, flask-socketio
-flask-classful==0.14.2    # via -r requirements.in
-flask-httpauth==4.7.0     # via -r requirements.in
-flask-socketio==5.3.2     # via -r requirements.in
-greenlet==2.0.1           # via eventlet
-idna==3.4                 # via requests
+exceptiongroup==1.1.2     # via anyio
+flask==2.3.2              # via -r requirements.in, flask-httpauth, flask-socketio
+flask-httpauth==4.8.0     # via -r requirements.in
+flask-socketio==5.3.4     # via -r requirements.in
+geographiclib==2.0        # via geopy
+geopy==2.3.0              # via -r requirements.in
+gevent==23.7.0            # via -r requirements.in
+greenlet==2.0.2           # via eventlet, gevent
+h11==0.14.0               # via httpcore
+httpcore==0.17.3          # via dnspython
+idna==3.4                 # via anyio, requests
 imapclient==2.3.1         # via -r requirements.in
-importlib-metadata==6.0.0  # via ax253, flask, kiss3
+importlib-metadata==6.8.0  # via ax253, kiss3
 itsdangerous==2.1.2       # via flask
 jinja2==3.1.2             # via click-completion, flask
 kiss3==8.0.0              # via -r requirements.in
-markupsafe==2.1.2         # via jinja2
+markupsafe==2.1.3         # via jinja2, werkzeug
 netaddr==0.8.0            # via oslo-config
-oslo-config==9.1.0        # via -r requirements.in
-oslo-i18n==5.1.0          # via oslo-config
+oslo-config==9.1.1        # via -r requirements.in
+oslo-i18n==6.0.0          # via oslo-config
 pbr==5.11.1               # via -r requirements.in, oslo-i18n, stevedore
-pluggy==1.0.0             # via -r requirements.in
-plumbum==1.8.1            # via rpyc
+pluggy==1.2.0             # via -r requirements.in
+plumbum==1.8.2            # via rpyc
 pycparser==2.21           # via cffi
-pygments==2.14.0          # via rich
-pyopenssl==23.0.0         # via -r requirements.in
+pygments==2.15.1          # via rich
+pyopenssl==23.2.0         # via -r requirements.in
 pyserial==3.5             # via pyserial-asyncio
 pyserial-asyncio==0.6     # via kiss3
-python-engineio==4.3.4    # via python-socketio
-python-socketio==5.7.2    # via flask-socketio
-pytz==2022.7.1            # via -r requirements.in
-pyyaml==6.0               # via -r requirements.in, oslo-config
-ratelimiter==1.2.0.post0  # via -r requirements.in
-requests==2.28.2          # via -r requirements.in, oslo-config, update-checker
+python-engineio==4.5.1    # via python-socketio
+python-socketio==5.8.0    # via -r requirements.in, flask-socketio
+pytz==2023.3              # via -r requirements.in
+pyyaml==6.0.1             # via -r requirements.in, oslo-config
+requests==2.31.0          # via -r requirements.in, oslo-config, update-checker
 rfc3986==2.0.0            # via oslo-config
 rich==12.6.0              # via -r requirements.in
-rpyc==5.3.0               # via -r requirements.in
+rpyc==5.3.1               # via -r requirements.in
+rush==2021.4.0            # via -r requirements.in
 shellingham==1.5.0.post1  # via -r requirements.in, click-completion
 six==1.16.0               # via -r requirements.in, click-completion, eventlet, imapclient
-soupsieve==2.3.2.post1    # via beautifulsoup4
-stevedore==4.1.1          # via oslo-config
+sniffio==1.3.0            # via anyio, dnspython, httpcore
+soupsieve==2.4.1          # via beautifulsoup4
+stevedore==5.1.0          # via oslo-config
 tabulate==0.9.0           # via -r requirements.in
 thesmuggler==1.0.1        # via -r requirements.in
-ua-parser==0.16.1         # via user-agents
+ua-parser==0.18.0         # via user-agents
 update-checker==0.18.0    # via -r requirements.in
-urllib3==1.26.14          # via requests
+urllib3==2.0.4            # via requests
 user-agents==2.2.0        # via -r requirements.in
-werkzeug==2.1.2           # via -r requirements.in, flask
-wrapt==1.14.1             # via -r requirements.in, debtcollector
-zipp==3.11.0              # via importlib-metadata
+validators==0.20.0        # via click-params
+werkzeug==2.3.6           # via -r requirements.in, flask
+wrapt==1.15.0             # via -r requirements.in, debtcollector
+zipp==3.16.2              # via importlib-metadata
+zope-event==5.0           # via gevent
+zope-interface==6.0       # via gevent
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `aprsd-3.0.3/setup.cfg` & `aprsd-3.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [files]
 packages = 
 	aprsd
 
 [entry_points]
 console_scripts = 
-	aprsd = aprsd.aprsd:main
+	aprsd = aprsd.main:main
 oslo.config.opts = 
 	aprsd.conf = aprsd.conf.opts:list_opts
 oslo.config.opts.defaults = 
 	aprsd.conf = aprsd.conf:set_lib_defaults
 
 [build_sphinx]
 source-dir = docs
```

### Comparing `aprsd-3.0.3/setup.py` & `aprsd-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/cmds/test_send_message.py` & `aprsd-3.1.0/tests/cmds/test_send_message.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import unittest
 from unittest import mock
 
 from click.testing import CliRunner
 from oslo_config import cfg
 
 from aprsd import conf  # noqa : F401
-from aprsd.aprsd import cli
 from aprsd.cmds import send_message  # noqa
+from aprsd.main import cli
 
 from .. import fake
 
 
 CONF = cfg.CONF
 F = t.TypeVar("F", bound=t.Callable[..., t.Any])
 
@@ -26,15 +26,15 @@
             CONF.aprs_network.login = login
         if password:
             CONF.aprs_network.password = password
 
         CONF.admin.user = "admin"
         CONF.admin.password = "password"
 
-    @mock.patch("aprsd.logging.log.setup_logging")
+    @mock.patch("aprsd.log.log.setup_logging")
     def test_no_tocallsign(self, mock_logging):
         """Make sure we get an error if there is no tocallsign."""
 
         self.config_and_init(
             login="something",
             password="another",
         )
@@ -43,15 +43,15 @@
         result = runner.invoke(
             cli, ["send-message"],
             catch_exceptions=False,
         )
         assert result.exit_code == 2
         assert "Error: Missing argument 'TOCALLSIGN'" in result.output
 
-    @mock.patch("aprsd.logging.log.setup_logging")
+    @mock.patch("aprsd.log.log.setup_logging")
     def test_no_command(self, mock_logging):
         """Make sure we get an error if there is no command."""
 
         self.config_and_init(
             login="something",
             password="another",
         )
```

### Comparing `aprsd-3.0.3/tests/cmds/test_webchat.py` & `aprsd-3.1.0/tests/cmds/test_webchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
             CONF.aprs_network.login = login
         if password:
             CONF.aprs_network.password = password
 
         CONF.admin.user = "admin"
         CONF.admin.password = "password"
 
-    @mock.patch("aprsd.logging.log.setup_logging")
+    @mock.patch("aprsd.log.log.setup_logging")
     def test_init_flask(self, mock_logging):
         """Make sure we get an error if there is no login and config."""
 
         CliRunner()
         self.config_and_init()
 
-        socketio, flask_app = webchat.init_flask("DEBUG", False)
+        socketio = webchat.init_flask("DEBUG", False)
         self.assertIsInstance(socketio, flask_socketio.SocketIO)
-        self.assertIsInstance(flask_app, flask.Flask)
+        self.assertIsInstance(webchat.flask_app, flask.Flask)
 
     @mock.patch("aprsd.packets.tracker.PacketTrack.remove")
     @mock.patch("aprsd.cmds.webchat.socketio")
     def test_process_ack_packet(
         self,
         mock_remove, mock_socketio,
     ):
```

### Comparing `aprsd-3.0.3/tests/fake.py` & `aprsd-3.1.0/tests/fake.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_fortune.py` & `aprsd-3.1.0/tests/plugins/test_fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_location.py` & `aprsd-3.1.0/tests/plugins/test_location.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,55 +45,65 @@
         fortune = location_plugin.LocationPlugin()
         expected = "Failed to fetch aprs.fi location"
         packet = fake.fake_packet(message="location")
         actual = fortune.filter(packet)
         self.assertEqual(expected, actual)
 
     @mock.patch("aprsd.plugin_utils.get_aprs_fi")
-    @mock.patch("aprsd.plugin_utils.get_weather_gov_for_gps")
+    @mock.patch("geopy.geocoders.Nominatim.reverse")
     @mock.patch("time.time")
-    def test_location_unknown_gps(self, mock_time, mock_weather, mock_check_aprs):
+    def test_location_unknown_gps(self, mock_time, mock_geocode, mock_check_aprs):
         # When the aprs.fi api key isn't set, then
         # the LocationPlugin will be disabled.
         mock_check_aprs.return_value = {
             "entries": [
                 {
-                    "lat": 10,
-                    "lng": 11,
+                    "lat": 1,
+                    "lng": 1,
                     "lasttime": 10,
                 },
             ],
         }
-        mock_weather.side_effect = Exception
+        mock_geocode.side_effect = Exception
         mock_time.return_value = 10
         CONF.callsign = fake.FAKE_TO_CALLSIGN
         fortune = location_plugin.LocationPlugin()
-        expected = "KFAKE: Unknown Location 0' 10,11 0.0h ago"
+        expected = "KFAKE: Unknown Location 0' 1.00,1.00 0.0h ago"
         packet = fake.fake_packet(message="location")
         actual = fortune.filter(packet)
         self.assertEqual(expected, actual)
 
     @mock.patch("aprsd.plugin_utils.get_aprs_fi")
-    @mock.patch("aprsd.plugin_utils.get_weather_gov_for_gps")
+    @mock.patch("geopy.geocoders.Nominatim.reverse")
     @mock.patch("time.time")
-    def test_location_works(self, mock_time, mock_weather, mock_check_aprs):
+    def test_location_works(self, mock_time, mock_geocode, mock_check_aprs):
         # When the aprs.fi api key isn't set, then
         # the LocationPlugin will be disabled.
         mock_check_aprs.return_value = {
             "entries": [
                 {
-                    "lat": 10,
-                    "lng": 11,
+                    "lat": 1,
+                    "lng": 1,
                     "lasttime": 10,
                 },
             ],
         }
-        expected_town = "Appomattox, VA"
-        wx_data = {"location": {"areaDescription": expected_town}}
-        mock_weather.return_value = wx_data
+        expected = "Appomattox"
+        state = "VA"
+
+        class TempLocation:
+            raw = {
+                "address": {
+                    "county": expected,
+                    "country_code": "us",
+                    "state": state,
+                    "country": "United States",
+                },
+            }
+        mock_geocode.return_value = TempLocation()
         mock_time.return_value = 10
         CONF.callsign = fake.FAKE_TO_CALLSIGN
         fortune = location_plugin.LocationPlugin()
-        expected = f"KFAKE: {expected_town} 0' 10,11 0.0h ago"
+        expected = f"KFAKE: {expected}, {state} 0' 1.00,1.00 0.0h ago"
         packet = fake.fake_packet(message="location")
         actual = fortune.filter(packet)
         self.assertEqual(expected, actual)
```

### Comparing `aprsd-3.0.3/tests/plugins/test_notify.py` & `aprsd-3.1.0/tests/plugins/test_notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_ping.py` & `aprsd-3.1.0/tests/plugins/test_ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_query.py` & `aprsd-3.1.0/tests/plugins/test_query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_time.py` & `aprsd-3.1.0/tests/plugins/test_time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_version.py` & `aprsd-3.1.0/tests/plugins/test_version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/plugins/test_weather.py` & `aprsd-3.1.0/tests/plugins/test_weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/test_email.py` & `aprsd-3.1.0/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/test_main.py` & `aprsd-3.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/test_packets.py` & `aprsd-3.1.0/tests/test_packets.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tests/test_plugin.py` & `aprsd-3.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tools/fast8.sh` & `aprsd-3.1.0/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.3/tox.ini` & `aprsd-3.1.0/tox.ini`

 * *Files identical despite different names*

